# Comparing `tmp/rddl_verify-0.1.1.tar.gz` & `tmp/rddl_verify-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rddl_verify-0.1.1.tar", max compression
+gzip compressed data, was "rddl_verify-0.2.0.tar", max compression
```

## Comparing `rddl_verify-0.1.1.tar` & `rddl_verify-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2023-05-10 12:10:40.531141 rddl_verify-0.1.1/LICENSE
--rw-r--r--   0        0        0        8 2023-05-10 12:10:40.531141 rddl_verify-0.1.1/README.md
--rw-r--r--   0        0        0      590 2023-05-10 12:10:40.535141 rddl_verify-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 12:10:40.535141 rddl_verify-0.1.1/rddl_verify/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 12:10:40.535141 rddl_verify-0.1.1/rddl_verify/app/__init__.py
--rw-r--r--   0        0        0      216 2023-05-10 12:10:40.535141 rddl_verify-0.1.1/rddl_verify/app/hash_data.py
--rw-r--r--   0        0        0     1154 2023-05-10 12:10:40.535141 rddl_verify-0.1.1/rddl_verify/app/verify_signature.py
--rw-r--r--   0        0        0      483 2023-05-10 12:10:40.535141 rddl_verify-0.1.1/rddl_verify/main.py
--rw-r--r--   0        0        0        0 2023-05-10 12:10:40.535141 rddl_verify-0.1.1/rddl_verify/models/__init__.py
--rw-r--r--   0        0        0      145 2023-05-10 12:10:40.535141 rddl_verify-0.1.1/rddl_verify/models/validation_result.py
--rw-r--r--   0        0        0        0 2023-05-10 12:10:40.535141 rddl_verify-0.1.1/rddl_verify/routers/__init__.py
--rw-r--r--   0        0        0      550 2023-05-10 12:10:40.535141 rddl_verify-0.1.1/rddl_verify/routers/hash_data.py
--rw-r--r--   0        0        0     1892 2023-05-10 12:10:40.535141 rddl_verify-0.1.1/rddl_verify/routers/validate_content.py
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 rddl_verify-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-11 11:57:22.311722 rddl_verify-0.2.0/LICENSE
+-rw-r--r--   0        0        0        8 2023-05-11 11:57:22.311722 rddl_verify-0.2.0/README.md
+-rw-r--r--   0        0        0      590 2023-05-11 11:57:22.311722 rddl_verify-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-11 11:57:22.311722 rddl_verify-0.2.0/rddl_verify/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 11:57:22.311722 rddl_verify-0.2.0/rddl_verify/app/__init__.py
+-rw-r--r--   0        0        0      214 2023-05-11 11:57:22.311722 rddl_verify-0.2.0/rddl_verify/app/hash_data.py
+-rw-r--r--   0        0        0     1152 2023-05-11 11:57:22.311722 rddl_verify-0.2.0/rddl_verify/app/verify_signature.py
+-rw-r--r--   0        0        0      483 2023-05-11 11:57:22.311722 rddl_verify-0.2.0/rddl_verify/main.py
+-rw-r--r--   0        0        0        0 2023-05-11 11:57:22.311722 rddl_verify-0.2.0/rddl_verify/models/__init__.py
+-rw-r--r--   0        0        0      145 2023-05-11 11:57:22.311722 rddl_verify-0.2.0/rddl_verify/models/validation_result.py
+-rw-r--r--   0        0        0        0 2023-05-11 11:57:22.311722 rddl_verify-0.2.0/rddl_verify/routers/__init__.py
+-rw-r--r--   0        0        0      540 2023-05-11 11:57:22.311722 rddl_verify-0.2.0/rddl_verify/routers/hash_data.py
+-rw-r--r--   0        0        0     1891 2023-05-11 11:57:22.311722 rddl_verify-0.2.0/rddl_verify/routers/validate_content.py
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 rddl_verify-0.2.0/PKG-INFO
```

### Comparing `rddl_verify-0.1.1/LICENSE` & `rddl_verify-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rddl_verify-0.1.1/pyproject.toml` & `rddl_verify-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rddl_verify"
-version = "0.1.1"
+version = "0.2.0"
 description = ""
 authors = ["Jürgen Eckel <juergen@riddleandcode.com>"]
 license = "AGPL"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `rddl_verify-0.1.1/rddl_verify/app/verify_signature.py` & `rddl_verify-0.2.0/rddl_verify/app/verify_signature.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     result = validate_signature_data_string(pub_key, signature, json_obj_str)
     result.json_obj = json_obj
     return result
 
 
 def validate_signature_data_string(pub_key: bytearray, signature: bytearray, data_string: str) -> ValidationResult:
     byte_string = bytes(data_string, "utf-8")
-    hash_local = hashlib.sha3_256()
+    hash_local = hashlib.sha256()
     hash_local.update(byte_string)
     result = validate_signature_data_hash(pub_key, signature, hash_local.digest())
     result.data_str = data_string
     return result
 
 
 def validate_signature_data_hash(pub_key: bytearray, signature: bytearray, data_digest: bytes) -> ValidationResult:
```

### Comparing `rddl_verify-0.1.1/rddl_verify/routers/hash_data.py` & `rddl_verify-0.2.0/rddl_verify/routers/hash_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 router = APIRouter(
     prefix="/hash_sha256",
     tags=["Hash SHA256"],
     responses={404: {"detail": "Not found"}},
 )
 
 
-@router.get("/hash/data")
+@router.get("/data")
 async def hash_data_endpoint(data: List[dict]):
     return {"hash": hash_data(data)}
 
 
-@router.get("/hash/file")
+@router.get("/file")
 async def hash_file(file: UploadFile = File(...)):
     contents = await file.read()
     data = json.loads(contents)
     return {"hash": hash_data(data)}
```

### Comparing `rddl_verify-0.1.1/rddl_verify/routers/validate_content.py` & `rddl_verify-0.2.0/rddl_verify/routers/validate_content.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import codecs
 from fastapi import APIRouter, HTTPException
 from rddl_verify.app import verify_signature
 from rddl_verify.models.validation_result import ValidationResult
 
 router = APIRouter(
     prefix="/validate",
-    tags=["Validate Transaction"],
+    tags=["Validate Data"],
     responses={404: {"detail": "Not found"}},
 )
 
 
 def convert_key_sig(pub_key: str, signature: bytes):
     try:
         pub_key_bytes = codecs.decode(pub_key, "hex_codec")
@@ -19,29 +19,29 @@
         signature_bytes = codecs.decode(signature, "hex_codec")
     except ValueError as e:
         raise HTTPException(status_code=404, detail=f"signature: Invalid input parameter {e}")
     return pub_key_bytes, signature_bytes
 
 
 @router.post("/json", response_model=ValidationResult)
-async def validate_signature(pub_key: str, signature: str, data: dict):
+async def validate_json_object(pub_key: str, signature: str, data: dict):
     pub_key_bytes, signature_bytes = convert_key_sig(pub_key, signature)
 
     return verify_signature.validate_signature_json_data(pub_key_bytes, signature_bytes, data)
 
 
-@router.get("/string", response_model=ValidationResult)
-async def validate_signature(pub_key: str, signature: str, data: str):
+@router.post("/string", response_model=ValidationResult)
+async def validate_data_string(pub_key: str, signature: str, data: str):
     pub_key_bytes, signature_bytes = convert_key_sig(pub_key, signature)
 
     return verify_signature.validate_signature_data_string(pub_key_bytes, signature_bytes, data)
 
 
-@router.get("/hash", response_model=ValidationResult)
-async def validate_signature(pub_key: str, signature: str, data: str):
+@router.post("/hash", response_model=ValidationResult)
+async def validate_data_hash(pub_key: str, signature: str, data: str):
     pub_key_bytes, signature_bytes = convert_key_sig(pub_key, signature)
     try:
         data_hash_bytes = codecs.decode(data, "hex_codec")
     except ValueError as e:
         raise HTTPException(status_code=404, detail=f"data: Invalid input parameter {e}")
 
     result = verify_signature.validate_signature_data_hash(pub_key_bytes, signature_bytes, data_hash_bytes)
```

### Comparing `rddl_verify-0.1.1/PKG-INFO` & `rddl_verify-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rddl-verify
-Version: 0.1.1
+Version: 0.2.0
 Summary: 
 License: AGPL
 Author: Jürgen Eckel
 Author-email: juergen@riddleandcode.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

