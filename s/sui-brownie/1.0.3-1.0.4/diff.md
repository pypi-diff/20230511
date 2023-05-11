# Comparing `tmp/sui_brownie-1.0.3-py3-none-any.whl.zip` & `tmp/sui_brownie-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 27946 bytes, number of entries: 16
+Zip file size: 27902 bytes, number of entries: 16
 -rw-r--r--  2.0 unx       10 b- defN 22-Dec-02 09:41 sui_brownie/MANIFEST.in
 -rw-r--r--  2.0 unx      878 b- defN 23-Apr-01 13:03 sui_brownie/README.md
 -rw-r--r--  2.0 unx       38 b- defN 23-Apr-11 02:45 sui_brownie/__init__.py
 -rw-r--r--  2.0 unx     2514 b- defN 23-Apr-01 12:52 sui_brownie/account.py
 -rw-r--r--  2.0 unx    12144 b- defN 23-Apr-21 09:58 sui_brownie/bcs.py
 -rw-r--r--  2.0 unx     4326 b- defN 23-Apr-01 12:53 sui_brownie/ed25519.py
 -rw-r--r--  2.0 unx    10047 b- defN 22-Dec-02 09:41 sui_brownie/parallelism.py
--rw-r--r--  2.0 unx    95206 b- defN 23-May-09 10:06 sui_brownie/sui_brownie.py
+-rw-r--r--  2.0 unx    94854 b- defN 23-May-11 09:08 sui_brownie/sui_brownie.py
 -rw-r--r--  2.0 unx    32439 b- defN 23-Apr-19 08:03 sui_brownie/sui_client.py
 -rw-r--r--  2.0 unx      140 b- defN 22-Dec-02 09:41 sui_brownie/sui_config.template.yaml
 -rw-r--r--  2.0 unx       19 b- defN 22-Dec-02 09:41 sui_brownie/sui_keystore.template.keystore
 -rw-r--r--  2.0 unx      866 b- defN 23-Apr-11 02:45 sui_brownie/utils.py
--rw-r--r--  2.0 unx      982 b- defN 23-May-09 10:07 sui_brownie-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-09 10:07 sui_brownie-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-09 10:07 sui_brownie-1.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1296 b- defN 23-May-09 10:07 sui_brownie-1.0.3.dist-info/RECORD
-16 files, 161009 bytes uncompressed, 25812 bytes compressed:  84.0%
+-rw-r--r--  2.0 unx      982 b- defN 23-May-11 09:14 sui_brownie-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-11 09:14 sui_brownie-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-11 09:14 sui_brownie-1.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1296 b- defN 23-May-11 09:14 sui_brownie-1.0.4.dist-info/RECORD
+16 files, 160657 bytes uncompressed, 25768 bytes compressed:  84.0%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: sui_brownie/sui_keystore.template.keystore
 Comment: 
 
 Filename: sui_brownie/utils.py
 Comment: 
 
-Filename: sui_brownie-1.0.3.dist-info/METADATA
+Filename: sui_brownie-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: sui_brownie-1.0.3.dist-info/WHEEL
+Filename: sui_brownie-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: sui_brownie-1.0.3.dist-info/top_level.txt
+Filename: sui_brownie-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: sui_brownie-1.0.3.dist-info/RECORD
+Filename: sui_brownie-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sui_brownie/sui_brownie.py

```diff
@@ -418,14 +418,17 @@
         object_ids = []
         for i in range(len(call_arg)):
             param_type = parameters[i]
             if isinstance(param_type, dict):
                 if ("Reference" in param_type or "MutableReference" in param_type or "Struct" in param_type) \
                         and isinstance(call_arg[i], str):
                     object_ids.append(call_arg[i])
+                if ("Reference" in param_type or "MutableReference" in param_type or "Struct" in param_type) \
+                        and isinstance(call_arg[i], list):
+                    object_ids.extend(call_arg[i])
                 elif "Vector" in param_type and "Struct" in param_type["Vector"]:
                     assert isinstance(call_arg[i], list)
                     object_ids.extend(call_arg[i])
 
         return cls.get_objects(object_ids)
 
     @classmethod
@@ -468,15 +471,24 @@
 
     @classmethod
     def generate_call_arg(cls, param_type, data, object_infos):
         if isinstance(param_type, dict) and \
                 ("MutableReference" in param_type or
                  "Reference" in param_type or
                  "Struct" in param_type):
-            return CallArg("Object", cls.generate_object_arg(data, object_infos, param_type))
+            if "Vector" in param_type.get("MutableReference", {}) or "Vector" in param_type.get("Reference",
+                                                                                                {}) or "Vector" in param_type.get(
+                    "Struct", {}):
+                assert isinstance(data, list)
+                call_args = []
+                for object_id in data:
+                    call_args.append(CallArg("Object", cls.generate_object_arg(object_id, object_infos, param_type)))
+                return call_args
+            else:
+                return CallArg("Object", cls.generate_object_arg(data, object_infos, param_type))
         elif isinstance(param_type, dict) and "Vector" in param_type and "Struct" in param_type["Vector"]:
             assert isinstance(data, list)
             call_args = []
             for object_id in data:
                 call_args.append(CallArg("Object", cls.generate_object_arg(object_id, object_infos)))
             return call_args
         else:
@@ -846,39 +858,21 @@
         for (package_id, abi, type_args, call_args) in transactions:
             call_args, type_args = cls.check_args(abi, call_args, type_args)
             # format param
             abi = cls.format_abi_param(abi, type_args)
 
             for i in range(len(call_args)):
                 call_arg = call_args[i]
-                if isinstance(call_arg, list):
-                    for j in range(len(call_arg)):
-                        assert isinstance(call_arg[j], Argument), f"Not support:{call_arg[j]}"
-                        actual_params_index = call_arg[j].value.v0
-                        if call_arg[j].key == "Input" and not has_actual_params[actual_params_index]:
-                            batch_call_args_index[len(batch_call_args)] = actual_params_index
-                            batch_call_args.append(actual_params[actual_params_index])
-                            batch_parameters.append(abi["parameters"][i])
-                            has_actual_params[actual_params_index] = True
-                        batch_commands.append(
-                            Command("MakeMoveVec",
-                                    MakeMoveVec(
-                                        OptionTypeTag("NONE", NONE()),
-                                        call_arg)
-                                    ))
-                        call_args[i] = Argument("Result", U16(len(batch_commands) - 1))
-
-                else:
-                    assert isinstance(call_arg, Argument), f"Not support:{call_arg}"
-                    actual_params_index = call_arg.value.v0
-                    if call_arg.key == "Input" and not has_actual_params[actual_params_index]:
-                        batch_call_args_index[len(batch_call_args)] = actual_params_index
-                        batch_call_args.append(actual_params[actual_params_index])
-                        batch_parameters.append(abi["parameters"][i])
-                        has_actual_params[actual_params_index] = True
+                assert isinstance(call_arg, Argument), f"Not support:{call_arg}"
+                actual_params_index = call_arg.value.v0
+                if call_arg.key == "Input" and not has_actual_params[actual_params_index]:
+                    batch_call_args_index[len(batch_call_args)] = actual_params_index
+                    batch_call_args.append(actual_params[actual_params_index])
+                    batch_parameters.append(abi["parameters"][i])
+                    has_actual_params[actual_params_index] = True
             # generate commands
             type_arguments = [
                 cls.generate_type_arg(v) for v in type_args
             ]
             commands = [
                 Command("MoveCall", ProgrammableMoveCall(
                     ObjectID(package_id),
```

## Comparing `sui_brownie-1.0.3.dist-info/METADATA` & `sui_brownie-1.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sui-brownie
-Version: 1.0.3
+Version: 1.0.4
 Summary: Sui Package Tool
 Home-page: https://github.com/OmniBTC/DolaProtocol/blob/main/utils
 Author: DaiWei
 Author-email: dw1253464613@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `sui_brownie-1.0.3.dist-info/RECORD` & `sui_brownie-1.0.4.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 sui_brownie/MANIFEST.in,sha256=BzExY9sw9x0Pqk6SYHuMRRvYS-cm75AxBOBjsYGFfU4,10
 sui_brownie/README.md,sha256=-7DxT6cGHbWLr_VufOEwIzl4Vtojp5dZc_r89lwnK3o,878
 sui_brownie/__init__.py,sha256=ROrbn7qi0haZjB8FG5JqXpD5mQ6qQPDNOwe0-rPnKeM,38
 sui_brownie/account.py,sha256=suZRI__kDNhyuoCZ9_q4mIV673lJDz0jgj0HyEj_hsQ,2514
 sui_brownie/bcs.py,sha256=8LwJihqmjLGwtzq87XKAQhE7ZgxiRDUsUYRbK6yRy7s,12144
 sui_brownie/ed25519.py,sha256=8hLHtC21og60B3MzXi4JmdQoOCbUutExyQIJhypJ9dg,4326
 sui_brownie/parallelism.py,sha256=Thh7TUrRU1fn47lNTF30RrcL5lBPBeMT2DX9A_swXDg,10047
-sui_brownie/sui_brownie.py,sha256=oAR5mg7QEwBHPsMigFBOXYCXO-DMZXglQFE42bDZgi0,95206
+sui_brownie/sui_brownie.py,sha256=-BcQJj13TIXHqf8TfWwGQWfa0OwkHR-FNQUJ8BleVqQ,94854
 sui_brownie/sui_client.py,sha256=Epyu5pXAI6jl_L-lzBg4gnNLYQVjdQTZ8kR4YrJfnqk,32439
 sui_brownie/sui_config.template.yaml,sha256=Qa6n48nf4qeLDhZnpVNjZJIYDm8jYFs7dVLCyLjxMTs,140
 sui_brownie/sui_keystore.template.keystore,sha256=dIQsJL_H6FdnGlET9u5NYXSmjTc1-8dk8wZWKrzcLOM,19
 sui_brownie/utils.py,sha256=bttovGstKoozRoMvzYFOFs_z73aled7UFbNBDPxX9Uo,866
-sui_brownie-1.0.3.dist-info/METADATA,sha256=3dBcdBXmVBmXeJClA1VIzJTaSTp3g2yQ1LsI2wXtPBk,982
-sui_brownie-1.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-sui_brownie-1.0.3.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
-sui_brownie-1.0.3.dist-info/RECORD,,
+sui_brownie-1.0.4.dist-info/METADATA,sha256=InbTzbxWdOelznyTittfwPQD6UkMUVtOlDM0W3J_mB4,982
+sui_brownie-1.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+sui_brownie-1.0.4.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
+sui_brownie-1.0.4.dist-info/RECORD,,
```

