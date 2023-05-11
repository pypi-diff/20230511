# Comparing `tmp/fastapi_oracle-0.9.0-py3-none-any.whl.zip` & `tmp/fastapi_oracle-0.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 13543 bytes, number of entries: 11
+Zip file size: 13586 bytes, number of entries: 11
 -rw-r--r--  2.0 unx     1500 b- defN 80-Jan-01 00:00 fastapi_oracle/__init__.py
 -rw-r--r--  2.0 unx      767 b- defN 80-Jan-01 00:00 fastapi_oracle/config.py
 -rw-r--r--  2.0 unx      893 b- defN 80-Jan-01 00:00 fastapi_oracle/constants.py
 -rw-r--r--  2.0 unx     8671 b- defN 80-Jan-01 00:00 fastapi_oracle/core.py
 -rw-r--r--  2.0 unx     2202 b- defN 80-Jan-01 00:00 fastapi_oracle/errors.py
 -rw-r--r--  2.0 unx      207 b- defN 80-Jan-01 00:00 fastapi_oracle/pools.py
 -rw-r--r--  2.0 unx     2487 b- defN 80-Jan-01 00:00 fastapi_oracle/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 fastapi_oracle-0.9.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4624 b- defN 80-Jan-01 00:00 fastapi_oracle-0.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fastapi_oracle-0.9.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      888 b- defN 16-Jan-01 00:00 fastapi_oracle-0.9.0.dist-info/RECORD
-11 files, 33684 bytes uncompressed, 12047 bytes compressed:  64.2%
+-rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 fastapi_oracle-0.9.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4781 b- defN 80-Jan-01 00:00 fastapi_oracle-0.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fastapi_oracle-0.9.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx      888 b- defN 16-Jan-01 00:00 fastapi_oracle-0.9.1.dist-info/RECORD
+11 files, 33841 bytes uncompressed, 12090 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: fastapi_oracle/pools.py
 Comment: 
 
 Filename: fastapi_oracle/utils.py
 Comment: 
 
-Filename: fastapi_oracle-0.9.0.dist-info/LICENSE
+Filename: fastapi_oracle-0.9.1.dist-info/LICENSE
 Comment: 
 
-Filename: fastapi_oracle-0.9.0.dist-info/METADATA
+Filename: fastapi_oracle-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: fastapi_oracle-0.9.0.dist-info/WHEEL
+Filename: fastapi_oracle-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: fastapi_oracle-0.9.0.dist-info/RECORD
+Filename: fastapi_oracle-0.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fastapi_oracle-0.9.0.dist-info/LICENSE` & `fastapi_oracle-0.9.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fastapi_oracle-0.9.0.dist-info/METADATA` & `fastapi_oracle-0.9.1.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-oracle
-Version: 0.9.0
+Version: 0.9.1
 Summary: Helpers for using the cx_Oracle_async library with the FastAPI framework.
 Home-page: https://github.com/Jaza/fastapi-oracle
 License: Apache-2.0
 Author: Jeremy Epstein
 Author-email: jazepstein@gmail.com
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: Apache Software License
@@ -37,14 +37,15 @@
    DB_PORT=1521
    DB_USER=foouser
    DB_PASSWORD=foopass
    DB_SERVICE_NAME=foodb1.aintitfootastic.com
 6. Use the utils:
    ```python
    from collections.abc import AsyncIterable, Mapping
+   from contextlib import asynccontextmanager
    from typing import Any, AsyncGenerator
 
    from fastapi import APIRouter, Depends, FastAPI, Request, status
    from fastapi.responses import JSONResponse
    from fastapi_oracle import (
        DbPoolConnAndCursor,
        IntermittentDatabaseError,
@@ -116,16 +117,22 @@
                ],
            },
        )
 
 
    def get_app() -> FastAPI:
        """Create a FastAPI app instance."""
+       @asynccontextmanager
+       async def lifespan(app: FastAPI):
+           yield
+
+           await close_db_pools()
+
        app = FastAPI(
-           on_shutdown=[close_db_pools],
+           lifespan=lifespan,
            exception_handlers={
                IntermittentDatabaseError: intermittent_database_error_handler,
            },
        )
        app.include_router(router)
        return app
    ```
```

## Comparing `fastapi_oracle-0.9.0.dist-info/RECORD` & `fastapi_oracle-0.9.1.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 fastapi_oracle/__init__.py,sha256=QS90PIZVzlCkEaBomoXTGx0bmZd6Jh8F4UvdqvuSETE,1500
 fastapi_oracle/config.py,sha256=hDQbaVzjX2vOb8ujxYWDGM-n39_r5lXQeCJd__Qeo9M,767
 fastapi_oracle/constants.py,sha256=Zh3D4PEPSL6SlSdyC2dwDNGz_wBkPACjDNoMre35KLs,893
 fastapi_oracle/core.py,sha256=9LyLb-jhc11JBrId0pxigbHLzNGWAzoe0XHevWoxFqI,8671
 fastapi_oracle/errors.py,sha256=VK3VBKZgGAUH9QC1KcoQhPvUFvd7i2q8Wk9SYrDicGA,2202
 fastapi_oracle/pools.py,sha256=fVkOPrtwoQMhlI85szk6k7m6tvPUGLmGKCBHGOqyl2U,207
 fastapi_oracle/utils.py,sha256=ututbmPjoUz0gc8CSDhGw6DBxbccIgYnn-luns0DuXA,2487
-fastapi_oracle-0.9.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-fastapi_oracle-0.9.0.dist-info/METADATA,sha256=bcOkJpqQn5Yk0Hw8-1UNfyW94zgITumY7_5hfq6SHNY,4624
-fastapi_oracle-0.9.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-fastapi_oracle-0.9.0.dist-info/RECORD,,
+fastapi_oracle-0.9.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+fastapi_oracle-0.9.1.dist-info/METADATA,sha256=csOaovnZHhKoXRRpTZeEG3oifoVngkgiq9wwZJ1StdY,4781
+fastapi_oracle-0.9.1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+fastapi_oracle-0.9.1.dist-info/RECORD,,
```

