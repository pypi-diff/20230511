# Comparing `tmp/gtki_module_orup_errors-1.35.7-py3-none-any.whl.zip` & `tmp/gtki_module_orup_errors-1.35.71-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 12425 bytes, number of entries: 17
+Zip file size: 12442 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Oct-20 07:03 orup_errors/__init__.py
 -rw-rw-rw-  2.0 fat    15672 b- defN 23-May-10 13:48 orup_errors/all_errors.py
--rw-rw-rw-  2.0 fat     5090 b- defN 23-May-10 13:48 orup_errors/check_funcs.py
+-rw-rw-rw-  2.0 fat     5094 b- defN 23-May-10 14:00 orup_errors/check_funcs.py
 -rw-rw-rw-  2.0 fat     2526 b- defN 23-Mar-28 11:24 orup_errors/general_functions.py
 -rw-rw-rw-  2.0 fat     2340 b- defN 23-Mar-28 11:17 orup_errors/main.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Oct-20 07:03 orup_errors/tests/__init__.py
 -rw-rw-rw-  2.0 fat     1545 b- defN 21-Oct-20 07:03 orup_errors/tests/all_errors_test.py
 -rw-rw-rw-  2.0 fat      744 b- defN 21-Oct-20 07:03 orup_errors/tests/args_test.py
 -rw-rw-rw-  2.0 fat      288 b- defN 21-Dec-03 04:31 orup_errors/tests/check_funcs_test.py
 -rw-rw-rw-  2.0 fat     1385 b- defN 21-Oct-20 07:03 orup_errors/tests/draw_win_test.py
 -rw-rw-rw-  2.0 fat     1300 b- defN 21-Dec-03 04:20 orup_errors/tests/general_functions_test.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Oct-20 07:03 orup_errors/tests/orup_errors_operator_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-10 13:49 gtki_module_orup_errors-1.35.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      156 b- defN 23-May-10 13:49 gtki_module_orup_errors-1.35.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-10 13:49 gtki_module_orup_errors-1.35.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-May-10 13:49 gtki_module_orup_errors-1.35.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1524 b- defN 23-May-10 13:49 gtki_module_orup_errors-1.35.7.dist-info/RECORD
-17 files, 33765 bytes uncompressed, 9863 bytes compressed:  70.8%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-10 14:05 gtki_module_orup_errors-1.35.71.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      157 b- defN 23-May-10 14:05 gtki_module_orup_errors-1.35.71.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-10 14:05 gtki_module_orup_errors-1.35.71.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-May-10 14:05 gtki_module_orup_errors-1.35.71.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1529 b- defN 23-May-10 14:05 gtki_module_orup_errors-1.35.71.dist-info/RECORD
+17 files, 33775 bytes uncompressed, 9870 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: orup_errors/tests/general_functions_test.py
 Comment: 
 
 Filename: orup_errors/tests/orup_errors_operator_test.py
 Comment: 
 
-Filename: gtki_module_orup_errors-1.35.7.dist-info/LICENSE
+Filename: gtki_module_orup_errors-1.35.71.dist-info/LICENSE
 Comment: 
 
-Filename: gtki_module_orup_errors-1.35.7.dist-info/METADATA
+Filename: gtki_module_orup_errors-1.35.71.dist-info/METADATA
 Comment: 
 
-Filename: gtki_module_orup_errors-1.35.7.dist-info/WHEEL
+Filename: gtki_module_orup_errors-1.35.71.dist-info/WHEEL
 Comment: 
 
-Filename: gtki_module_orup_errors-1.35.7.dist-info/top_level.txt
+Filename: gtki_module_orup_errors-1.35.71.dist-info/top_level.txt
 Comment: 
 
-Filename: gtki_module_orup_errors-1.35.7.dist-info/RECORD
+Filename: gtki_module_orup_errors-1.35.71.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## orup_errors/check_funcs.py

```diff
@@ -57,17 +57,17 @@
 
 
 def check_object_incorrectness(object_name: str, objects_list: list, *args,
                                **kwargs):
     return check_type_incorrectness(object_name, objects_list)
 
 
-def check_platform_incorrectness(object_name: str, platforms_list: list, *args,
+def check_platform_incorrectness(platform_name: str, platforms_list: list, *args,
                                **kwargs):
-    return check_type_incorrectness(object_name, platforms_list)
+    return check_type_incorrectness(platform_name, platforms_list)
 
 def check_tc_incorrectness(chosen_trash_cat, cats_list, *args, **kwargs):
     return check_type_incorrectness(chosen_trash_cat, cats_list)
 
 
 def check_tt_incorrectness(type_name: str, types_list: list, *args, **kwargs):
     return check_type_incorrectness(type_name, types_list)
```

## Comparing `gtki_module_orup_errors-1.35.7.dist-info/LICENSE` & `gtki_module_orup_errors-1.35.71.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gtki_module_orup_errors-1.35.7.dist-info/RECORD` & `gtki_module_orup_errors-1.35.71.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 orup_errors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 orup_errors/all_errors.py,sha256=wcua7YwipqBGlAS1EWsNwiscnj8S0rwa683DzZpNYcI,15672
-orup_errors/check_funcs.py,sha256=1jfpnf4tbR-mzmHwfvJxCD7GOw8MxZhlOzqyQPWHclc,5090
+orup_errors/check_funcs.py,sha256=aYpspCiR7NYckN-gBD9BScTTZCielMikANBS6BFDHr0,5094
 orup_errors/general_functions.py,sha256=urdTLpnec8vJi7An2pBiu_qx34RYvJfMTRe9myNVtNU,2526
 orup_errors/main.py,sha256=0rAbiAqmCHK-T_hmEedmofODsCQPEaxR57b2AYb9wWI,2340
 orup_errors/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 orup_errors/tests/all_errors_test.py,sha256=Lxq5C6Ka5XaHPOVMCQdMSuZT3l07TaJuoGP5l4ZJU_0,1545
 orup_errors/tests/args_test.py,sha256=rz64Iv4D8nPuDlATAHuO_4wFRS20b71gYsIyotaw1pI,744
 orup_errors/tests/check_funcs_test.py,sha256=m5e0kAHg5AcEi2VfRLBEslCAKfFDs8ARWb8emZ_j1Pk,288
 orup_errors/tests/draw_win_test.py,sha256=dsrfPhbnArm08IukF_zypmUFYOw1wjHD_5qYHYjk-88,1385
 orup_errors/tests/general_functions_test.py,sha256=CHoOqcw6k2qLUfgHnGA4TTgACt25jIZNDkF0UnKRtlQ,1300
 orup_errors/tests/orup_errors_operator_test.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gtki_module_orup_errors-1.35.7.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-gtki_module_orup_errors-1.35.7.dist-info/METADATA,sha256=jNTbunpeHXA_u-lJH_V5J5t52-myaqS5nO0OATo39x8,156
-gtki_module_orup_errors-1.35.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gtki_module_orup_errors-1.35.7.dist-info/top_level.txt,sha256=WzasBtx2xqnJAQK3vavyWJNr2nwUAPObo6jw7F1FFko,12
-gtki_module_orup_errors-1.35.7.dist-info/RECORD,,
+gtki_module_orup_errors-1.35.71.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+gtki_module_orup_errors-1.35.71.dist-info/METADATA,sha256=cTCxzXSFW49lj7D0SdEm-_eh5zz4DCMYPFHIJqSq-MA,157
+gtki_module_orup_errors-1.35.71.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gtki_module_orup_errors-1.35.71.dist-info/top_level.txt,sha256=WzasBtx2xqnJAQK3vavyWJNr2nwUAPObo6jw7F1FFko,12
+gtki_module_orup_errors-1.35.71.dist-info/RECORD,,
```

