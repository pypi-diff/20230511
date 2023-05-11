# Comparing `tmp/unitlab-1.7.9.tar.gz` & `tmp/unitlab-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitlab-1.7.9.tar", last modified: Mon Mar 20 06:01:36 2023, max compression
+gzip compressed data, was "unitlab-1.8.0.tar", last modified: Tue Apr  4 11:28:26 2023, max compression
```

## Comparing `unitlab-1.7.9.tar` & `unitlab-1.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-03-20 06:01:36.551939 unitlab-1.7.9/
--rw-rw-r--   0 me        (1000) me        (1000)     1060 2022-11-07 13:04:44.000000 unitlab-1.7.9/LICENSE.md
--rw-rw-r--   0 me        (1000) me        (1000)       84 2023-02-15 09:26:00.000000 unitlab-1.7.9/MANIFEST.in
--rw-rw-r--   0 me        (1000) me        (1000)      648 2023-03-20 06:01:36.551939 unitlab-1.7.9/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)     2015 2023-02-15 09:26:00.000000 unitlab-1.7.9/README.md
--rw-rw-r--   0 me        (1000) me        (1000)      106 2023-03-20 06:01:36.551939 unitlab-1.7.9/setup.cfg
--rw-rw-r--   0 me        (1000) me        (1000)     1142 2023-03-20 06:01:24.000000 unitlab-1.7.9/setup.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-03-20 06:01:36.551939 unitlab-1.7.9/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-03-20 06:01:36.551939 unitlab-1.7.9/src/unitlab/
--rw-rw-r--   0 me        (1000) me        (1000)       70 2023-03-20 05:56:45.000000 unitlab-1.7.9/src/unitlab/__init__.py
--rw-rw-r--   0 me        (1000) me        (1000)     9702 2023-03-20 05:57:39.000000 unitlab-1.7.9/src/unitlab/client.py
--rw-rw-r--   0 me        (1000) me        (1000)     7492 2023-03-20 06:00:59.000000 unitlab-1.7.9/src/unitlab/core.py
--rw-rw-r--   0 me        (1000) me        (1000)      746 2023-03-03 08:56:41.000000 unitlab-1.7.9/src/unitlab/exceptions.py
--rw-rw-r--   0 me        (1000) me        (1000)     4109 2023-02-27 14:18:44.000000 unitlab-1.7.9/src/unitlab/pretty.py
--rw-rw-r--   0 me        (1000) me        (1000)     4476 2023-03-20 05:58:36.000000 unitlab-1.7.9/src/unitlab/run.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-03-20 06:01:36.551939 unitlab-1.7.9/src/unitlab.egg-info/
--rw-rw-r--   0 me        (1000) me        (1000)      648 2023-03-20 06:01:36.000000 unitlab-1.7.9/src/unitlab.egg-info/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      396 2023-03-20 06:01:36.000000 unitlab-1.7.9/src/unitlab.egg-info/SOURCES.txt
--rw-rw-r--   0 me        (1000) me        (1000)        1 2023-03-20 06:01:36.000000 unitlab-1.7.9/src/unitlab.egg-info/dependency_links.txt
--rw-rw-r--   0 me        (1000) me        (1000)       46 2023-03-20 06:01:36.000000 unitlab-1.7.9/src/unitlab.egg-info/entry_points.txt
--rw-rw-r--   0 me        (1000) me        (1000)       61 2023-03-20 06:01:36.000000 unitlab-1.7.9/src/unitlab.egg-info/requires.txt
--rw-rw-r--   0 me        (1000) me        (1000)        8 2023-03-20 06:01:36.000000 unitlab-1.7.9/src/unitlab.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-04-04 11:28:26.414363 unitlab-1.8.0/
+-rw-rw-r--   0 me        (1000) me        (1000)     1060 2022-11-07 13:04:44.000000 unitlab-1.8.0/LICENSE.md
+-rw-rw-r--   0 me        (1000) me        (1000)       84 2023-02-15 09:26:00.000000 unitlab-1.8.0/MANIFEST.in
+-rw-rw-r--   0 me        (1000) me        (1000)      648 2023-04-04 11:28:26.414363 unitlab-1.8.0/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)     2015 2023-02-15 09:26:00.000000 unitlab-1.8.0/README.md
+-rw-rw-r--   0 me        (1000) me        (1000)      106 2023-04-04 11:28:26.414363 unitlab-1.8.0/setup.cfg
+-rw-rw-r--   0 me        (1000) me        (1000)     1142 2023-04-04 11:28:18.000000 unitlab-1.8.0/setup.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-04-04 11:28:26.414363 unitlab-1.8.0/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-04-04 11:28:26.414363 unitlab-1.8.0/src/unitlab/
+-rw-rw-r--   0 me        (1000) me        (1000)       70 2023-03-20 05:56:45.000000 unitlab-1.8.0/src/unitlab/__init__.py
+-rw-rw-r--   0 me        (1000) me        (1000)     9702 2023-03-20 05:57:39.000000 unitlab-1.8.0/src/unitlab/client.py
+-rw-rw-r--   0 me        (1000) me        (1000)     7950 2023-04-04 11:26:30.000000 unitlab-1.8.0/src/unitlab/core.py
+-rw-rw-r--   0 me        (1000) me        (1000)      746 2023-03-03 08:56:41.000000 unitlab-1.8.0/src/unitlab/exceptions.py
+-rw-rw-r--   0 me        (1000) me        (1000)     4109 2023-02-27 14:18:44.000000 unitlab-1.8.0/src/unitlab/pretty.py
+-rw-rw-r--   0 me        (1000) me        (1000)     4476 2023-04-04 11:22:43.000000 unitlab-1.8.0/src/unitlab/run.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-04-04 11:28:26.414363 unitlab-1.8.0/src/unitlab.egg-info/
+-rw-rw-r--   0 me        (1000) me        (1000)      648 2023-04-04 11:28:26.000000 unitlab-1.8.0/src/unitlab.egg-info/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)      396 2023-04-04 11:28:26.000000 unitlab-1.8.0/src/unitlab.egg-info/SOURCES.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        1 2023-04-04 11:28:26.000000 unitlab-1.8.0/src/unitlab.egg-info/dependency_links.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       46 2023-04-04 11:28:26.000000 unitlab-1.8.0/src/unitlab.egg-info/entry_points.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       61 2023-04-04 11:28:26.000000 unitlab-1.8.0/src/unitlab.egg-info/requires.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        8 2023-04-04 11:28:26.000000 unitlab-1.8.0/src/unitlab.egg-info/top_level.txt
```

### Comparing `unitlab-1.7.9/LICENSE.md` & `unitlab-1.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unitlab-1.7.9/PKG-INFO` & `unitlab-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 1.7.9
+Version: 1.8.0
 Summary: UNKNOWN
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Platform: UNKNOWN
```

### Comparing `unitlab-1.7.9/README.md` & `unitlab-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `unitlab-1.7.9/setup.py` & `unitlab-1.8.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="unitlab",
-    version="1.7.9",
+    version="1.8.0",
     license="MIT",
     author="Unitlab Inc.",
     author_email="team@unitlab.ai",
     packages=find_packages("src"),
     include_package_data=True,
     package_data={"static": ["*"], "Potato": ["*.so"]},
     classifiers=[
```

### Comparing `unitlab-1.7.9/src/unitlab/client.py` & `unitlab-1.8.0/src/unitlab/client.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.7.9/src/unitlab/core.py` & `unitlab-1.8.0/src/unitlab/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import argparse
 import asyncio
-import errno
 import glob
-import logging
 import os
 import re
 from io import BytesIO
 from uuid import UUID
 
 import aiohttp
 import cv2
@@ -112,62 +110,68 @@
         url=ENPOINTS[namespace.func.__name__].format(namespace.uuid),
         headers=get_headers(namespace),
     )
     pretty.print_task_statistics(r.json())
 
 
 def task_upload_datasources(namespace):
-    logging.basicConfig(level=logging.INFO, format=None)
+    if not os.path.exists(namespace.input_dir):
+        raise ValueError(f"Directory {namespace.input_dir} does not exist.")
 
-    try:
-        os.makedirs(namespace.input_dir)
-    except OSError as e:
-        if e.errno != errno.EEXIST:
-            raise
-
-    async def post_image(session: aiohttp.ClientSession, image: str, task_id: str):
-        with open(image, "rb") as img:
-            await session.request(
-                "POST",
-                url=ENPOINTS[namespace.func.__name__],
-                data=aiohttp.FormData(fields={"task": task_id, "image": img}),
-            )
-            return os.path.getsize(image)
-
-    async def data_upload(folder: str, api_key: str, task_id: str):
-        async with aiohttp.ClientSession(
-            headers={"Authorization": f"Api-Key {api_key}"}
-        ) as session:
-            total_bytes = 0
-            tasks = []
-            images = [
-                image
-                for images_list in [
-                    glob.glob(os.path.join(folder, "") + extension)
-                    for extension in ["*jpg", "*png"]
-                ]
-                for image in images_list
+    async def upload_images(session, endpoint, task_id, images, progress_bar):
+        for file_path in images:
+            with open(file_path, "rb") as image:
+                async with session.post(
+                    endpoint,
+                    data=aiohttp.FormData(fields={"task": task_id, "image": image}),
+                ) as response:
+                    if response.status != 201:
+                        raise Exception(
+                            f"Failed to upload file {file_path}. HTTP status code: {response.status}"
+                        )
+                    progress_bar.update(os.path.getsize(file_path))
+                    await response.read()
+
+    async def upload_images_in_batches(
+        folder: str, api_key: str, task_id: str, batch_size=1000
+    ):
+        images = [
+            image
+            for images_list in [
+                glob.glob(os.path.join(folder, "") + extension)
+                for extension in ["*jpg", "*png"]
             ]
-            for image in images:
-                total_bytes += os.path.getsize(image)
-            for image in images:
-                tasks.append(post_image(session=session, image=image, task_id=task_id))
-
-            pbar = tqdm.tqdm(
-                total=total_bytes,
-                unit="B",
-                unit_scale=True,
-                unit_divisor=1024,
-                ncols=80,
-            )
-            for f in asyncio.as_completed(tasks):
-                value = await f
-                pbar.update(value)
+            for image in images_list
+        ]
+        total_size = sum(os.path.getsize(f) for f in images)
+        endpoint = ENPOINTS[namespace.func.__name__]
+
+        with tqdm.tqdm(total=total_size, unit="B", unit_scale=True) as progress_bar:
+            async with aiohttp.ClientSession(
+                headers={"Authorization": f"Api-Key {api_key}"}
+            ) as session:
+                for i in range(0, len(images), batch_size):
+                    batch_images = images[i : i + batch_size]
+                    tasks = [
+                        asyncio.create_task(
+                            upload_images(
+                                session, endpoint, task_id, batch_images, progress_bar
+                            )
+                        )
+                    ]
+                    await asyncio.gather(*tasks)
 
-    asyncio.run(data_upload(namespace.input_dir, namespace.api_key, namespace.uuid))
+    try:
+        asyncio.run(
+            upload_images_in_batches(
+                namespace.input_dir, namespace.api_key, namespace.uuid, batch_size=1000
+            )
+        )
+    except Exception as e:
+        print(str(e))
 
 
 def task_download_data(namespace):
     response = requests.get(
         url=ENPOINTS[namespace.func.__name__].format(namespace.uuid),
         headers=get_headers(namespace),
     )
```

### Comparing `unitlab-1.7.9/src/unitlab/exceptions.py` & `unitlab-1.8.0/src/unitlab/exceptions.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.7.9/src/unitlab/pretty.py` & `unitlab-1.8.0/src/unitlab/pretty.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.7.9/src/unitlab/run.py` & `unitlab-1.8.0/src/unitlab/run.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.7.9/src/unitlab.egg-info/PKG-INFO` & `unitlab-1.8.0/src/unitlab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 1.7.9
+Version: 1.8.0
 Summary: UNKNOWN
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Platform: UNKNOWN
```

