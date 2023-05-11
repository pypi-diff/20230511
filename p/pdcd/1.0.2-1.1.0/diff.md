# Comparing `tmp/pdcd-1.0.2-py3-none-any.whl.zip` & `tmp/pdcd-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 24815 bytes, number of entries: 17
+Zip file size: 24591 bytes, number of entries: 17
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 pdcd/__init__.py
 -rw-r--r--  2.0 unx     3238 b- defN 80-Jan-01 00:00 pdcd/cli.py
 -rw-r--r--  2.0 unx     6290 b- defN 80-Jan-01 00:00 pdcd/config.py
 -rw-r--r--  2.0 unx     5816 b- defN 80-Jan-01 00:00 pdcd/connectors.py
--rw-r--r--  2.0 unx    19746 b- defN 80-Jan-01 00:00 pdcd/external.py
+-rw-r--r--  2.0 unx    18805 b- defN 80-Jan-01 00:00 pdcd/external.py
 -rw-r--r--  2.0 unx     9390 b- defN 80-Jan-01 00:00 pdcd/files.py
 -rw-r--r--  2.0 unx     3312 b- defN 80-Jan-01 00:00 pdcd/jobs.py
 -rw-r--r--  2.0 unx      574 b- defN 80-Jan-01 00:00 pdcd/log.py
 -rw-r--r--  2.0 unx     6560 b- defN 80-Jan-01 00:00 pdcd/routines.py
 -rw-r--r--  2.0 unx     2047 b- defN 80-Jan-01 00:00 pdcd/settings.py
 -rw-r--r--  2.0 unx     2257 b- defN 80-Jan-01 00:00 pdcd/shellcode.py
 -rw-r--r--  2.0 unx     2447 b- defN 80-Jan-01 00:00 pdcd/utils.py
-?rw-r--r--  2.0 unx       38 b- defN 16-Jan-01 00:00 pdcd-1.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx     1079 b- defN 80-Jan-01 00:00 pdcd-1.0.2.dist-info/LICENSE
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 pdcd-1.0.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1799 b- defN 16-Jan-01 00:00 pdcd-1.0.2.dist-info/METADATA
-?rw-r--r--  2.0 unx     1228 b- defN 16-Jan-01 00:00 pdcd-1.0.2.dist-info/RECORD
-17 files, 65904 bytes uncompressed, 22861 bytes compressed:  65.3%
+-rw-r--r--  2.0 unx     1079 b- defN 80-Jan-01 00:00 pdcd-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1899 b- defN 80-Jan-01 00:00 pdcd-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pdcd-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       38 b- defN 80-Jan-01 00:00 pdcd-1.1.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1228 b- defN 16-Jan-01 00:00 pdcd-1.1.0.dist-info/RECORD
+17 files, 65068 bytes uncompressed, 22637 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: pdcd/shellcode.py
 Comment: 
 
 Filename: pdcd/utils.py
 Comment: 
 
-Filename: pdcd-1.0.2.dist-info/entry_points.txt
+Filename: pdcd-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: pdcd-1.0.2.dist-info/LICENSE
+Filename: pdcd-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: pdcd-1.0.2.dist-info/WHEEL
+Filename: pdcd-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: pdcd-1.0.2.dist-info/METADATA
+Filename: pdcd-1.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pdcd-1.0.2.dist-info/RECORD
+Filename: pdcd-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pdcd/external.py

```diff
@@ -5,18 +5,16 @@
 import string
 import random
 import boto3
 import subprocess
 import json
 from dataclasses import dataclass, field
 from typing import Optional, TYPE_CHECKING, Tuple
-from mythic import mythic_rest
+import mythic.mythic as mythic_sdk
 import asyncio
-import os
-import contextlib
 from abc import ABC, abstractmethod
 import base64
 from functools import lru_cache
 
 from .shellcode import Shellcode
 from .log import logger
 from .utils import shell, find_free_local_port, generate_uuid, pad_list, file_is_empty
@@ -195,74 +193,67 @@
         resolved_token = f"/shared/{binfile_o.name}"
         logger.info(f"Resolved token {token} to value {resolved_token} for {type(self).__name__}")
 
         return resolved_token, cleanup_files
 
     @lru_cache(maxsize=None)
     def export_shellcode(self, profile: str, scformat: str = "Shellcode") -> Shellcode:
-        # redirecting to stdout in this method is used to suppress print statements from the
-        # "mythic" library as it uses print statements instead of warnings for notices
-        with open(os.devnull, "w") as devnull:
-            with contextlib.redirect_stdout(devnull):
-                mythic = mythic_rest.Mythic(
-                    username=self.__user,
-                    password=self.__password,
-                    server_ip=self.__host,
-                    server_port=self.__port,
-                    ssl=True,
-                    global_timeout=-1,
-                )
-                asyncio.run(mythic.login())
-        asyncio.run(mythic.set_or_create_apitoken())
+        mythic = asyncio.run(mythic_sdk.login(
+            username=self.__user,
+            password=self.__password,
+            server_ip=self.__host,
+            server_port=int(self.__port),
+            ssl=True,
+            timeout=-1,
+        ))
 
         # mythic payload settings are defined per payload rather than per listener,
         #   meaning you need to provide them via this tool
         #   default values are provided here but some can be overridden via env vars
         if profile.lower() == "smb":
-            build_vars = [
-                {"name": "pipename", "value": global_settings.mythic_smb_pipename},
-                {"name": "killdate", "value": "2030-10-12"},
-                {"name": "encrypted_exchange_check", "value": "T"},
-            ]
+            build_vars = {
+                "pipename": global_settings.mythic_smb_pipename,
+                "killdate": "2030-10-12",
+                "encrypted_exchange_check": "T"
+            }
         else:
-            build_vars = [
-                {"name": "callback_host", "value": self.__callback_url},
-                {"name": "callback_interval", "value": global_settings.mythic_callback_interval},
-                {"name": "c2_profile", "value": profile.lower()},
-                {"name": "AESPSK", "value": "aes256_hmac"},
-                {"name": "get_uri", "value": global_settings.mythic_http_geturi},
-                {"name": "post_uri", "value": global_settings.mythic_http_posturi},
-                {"name": "query_path_name", "value": global_settings.mythic_http_queryuri},
-                {"name": "proxy_host", "value": ""},
-                {"name": "proxy_port", "value": ""},
-                {"name": "proxy_user", "value": ""},
-                {"name": "proxy_pass", "value": ""},
-                {"name": "callback_port", "value": self.__callback_port},
-                {"name": "killdate", "value": "2030-10-12"},
-                {"name": "encrypted_exchange_check", "value": "T"},
-                {"name": "callback_jitter", "value": global_settings.mythic_jitter_percent},
-                {"name": "headers", "value": global_settings.mythic_http_useragent},
-            ]
+            build_vars = {
+                "callback_host": self.__callback_url,
+                "callback_interval": global_settings.mythic_callback_interval,
+                "c2_profile": profile.lower(),
+                "AESPSK": "aes256_hmac",
+                "get_uri": global_settings.mythic_http_geturi,
+                "post_uri": global_settings.mythic_http_posturi,
+                "query_path_name": global_settings.mythic_http_queryuri,
+                "proxy_host": "",
+                "proxy_port": "",
+                "proxy_user": "",
+                "proxy_pass": "",
+                "callback_port": self.__callback_port,
+                "killdate": "2030-10-12",
+                "encrypted_exchange_check": True,
+                "callback_jitter": global_settings.mythic_jitter_percent,
+                "headers": {"User-Agent": global_settings.mythic_http_useragent}
+            }
 
-        mythic_payload = mythic_rest.Payload(
+        payload = asyncio.run(mythic_sdk.create_payload(
             # TODO: currently hardcoded but should make configurable
             #   this will require different configs for different payloads
-            payload_type="apollo",
-            c2_profiles={profile.lower(): build_vars},
-            build_parameters=[{"name": "version", "value": 1.0}, {"name": "output_type", "value": scformat}],
-            tag="Built with PDCD",
-            selected_os="Windows",
+            mythic=mythic,
+            payload_type_name="apollo",
+            operating_system="Windows",
+            c2_profiles=[{"c2_profile": profile.lower(), "c2_profile_parameters": build_vars}],
+            build_parameters=[{"name": "output_type", "value": scformat}],
+            description="Built with PDCD",
             filename="pdcd",
-        )
-        resp = asyncio.run(mythic.create_payload(mythic_payload, all_commands=True, wait_for_build=True))
-        if resp.status == "error":
-            raise Exception(f"Error when generating Mythic payload: Error: {resp.response.get('error', '<ERROR>')}")
-        payload_contents = asyncio.run(mythic.download_payload(resp.response))
-        # cannot delete payloads as mythic does not allow spawning from dead payloads
-        #   asyncio.run(mythic.remove_payload(resp.response))
+            return_on_complete=True,
+            include_all_commands=True
+        ))
+        payload_contents = asyncio.run(mythic_sdk.download_payload(mythic=mythic, payload_uuid=payload.get("uuid")))
+        # note: cannot delete payloads as mythic does not allow spawning from dead payloads
         if len(payload_contents) == 0:
             raise Exception(f"Shellcode is empty")
         return Shellcode(shellcode=payload_contents)
 
 
 @dataclass
 class AWSPortForwardParams:
```

## Comparing `pdcd-1.0.2.dist-info/LICENSE` & `pdcd-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pdcd-1.0.2.dist-info/METADATA` & `pdcd-1.1.0.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: pdcd
-Version: 1.0.2
+Version: 1.1.0
 Summary: Tool that orchestrates executing Docker containers to build payloads
 License: MIT
 Author: 2XXE
 Author-email: root@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
 Requires-Dist: boto3 (>=1.24.54,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: desert (>=2020.11.18,<2021.0.0)
 Requires-Dist: docker (>=5.0.0,<6.0.0)
 Requires-Dist: impacket (>=0.10.0,<0.11.0)
-Requires-Dist: mythic (>=0.0.38,<0.0.39)
+Requires-Dist: mythic (>=0.1.0,<0.2.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Description-Content-Type: text/markdown
 
 # PDC Docker ("PDCD")
 
 PDC Docker is a lightweight tool that orchestrates executing Docker containers.
```

## Comparing `pdcd-1.0.2.dist-info/RECORD` & `pdcd-1.1.0.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 pdcd/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pdcd/cli.py,sha256=FZR_VENLfoKLnQ64zVddB70cpU_ASqzJGLRqifzM_Ck,3238
 pdcd/config.py,sha256=RXghqophhzHvTLoVekwtl8c872-hfMBip5K1TIVML0g,6290
 pdcd/connectors.py,sha256=x2rrwFQaTXgxURX_6O9JTnJ_UHMRpjzdnYvT5z4q1mY,5816
-pdcd/external.py,sha256=nVtxwphaeFAVgqr4UL27XRmxcQGp0G34OpVI2KWwiNM,19746
+pdcd/external.py,sha256=YX_U5EWYPHP3iC5ls12iYgQMR1kIxwcFnRCTNFOz0hI,18805
 pdcd/files.py,sha256=u6ozYD8orFnZXSHwMjrvaR036mZNcju9Zv1UTOC-UZM,9390
 pdcd/jobs.py,sha256=Oz08E3T7XUovlhWF6BTpMF_d97Xo5h5_HayMcg34B8E,3312
 pdcd/log.py,sha256=OxcLhUcDNH5muLyidZVP2qjbFvILPr0PDySJnmkMB4o,574
 pdcd/routines.py,sha256=jJSy_IP0ZPwmiiAml86Z3pE6leWTE0V5oIAMUU0n7_w,6560
 pdcd/settings.py,sha256=gxmMVEo4dGZqMdN8XTfZBK4aKFtz7lr8rXLV6aAqmOI,2047
 pdcd/shellcode.py,sha256=6ZmQwjxbMzGeC7SuGsc-v9V74PiiQeT5KRBkop7xceU,2257
 pdcd/utils.py,sha256=yKQWF02SNE9GMW1d7_ZywL-9xqTPtzTEaNlXKW9HYP0,2447
-pdcd-1.0.2.dist-info/entry_points.txt,sha256=mRscLiWpZp0wpqO99VyBCR542JJ12fpzK8uOISMdxF0,38
-pdcd-1.0.2.dist-info/LICENSE,sha256=NvRKe1dCnpR_vAVve_f8PqyRFjNpUuh8p1_Qfdlt7ns,1079
-pdcd-1.0.2.dist-info/WHEEL,sha256=SrtnPGVTMeYWttls9xnWA01eUhCZ3ufFdJUYb1J3r-U,83
-pdcd-1.0.2.dist-info/METADATA,sha256=N-mnOPKb7YaKVBMx3Tfvebtv9V4aSMmDvWXRBp_Mr7I,1799
-pdcd-1.0.2.dist-info/RECORD,,
+pdcd-1.1.0.dist-info/LICENSE,sha256=NvRKe1dCnpR_vAVve_f8PqyRFjNpUuh8p1_Qfdlt7ns,1079
+pdcd-1.1.0.dist-info/METADATA,sha256=mIhjam5kB3kN7MLFO36HlUjZD3W7Q2v1Uen_86XTiTs,1899
+pdcd-1.1.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+pdcd-1.1.0.dist-info/entry_points.txt,sha256=mRscLiWpZp0wpqO99VyBCR542JJ12fpzK8uOISMdxF0,38
+pdcd-1.1.0.dist-info/RECORD,,
```

