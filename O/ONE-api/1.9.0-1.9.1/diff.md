# Comparing `tmp/ONE-api-1.9.0.tar.gz` & `tmp/ONE-api-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ONE-api-1.9.0.tar", last modified: Thu Feb 24 20:11:44 2022, max compression
+gzip compressed data, was "ONE-api-1.9.1.tar", last modified: Thu Mar 10 08:26:59 2022, max compression
```

## Comparing `ONE-api-1.9.0.tar` & `ONE-api-1.9.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxrwx   0        0        0        0 2022-02-24 20:11:44.671499 ONE-api-1.9.0/
--rw-rw-rw-   0        0        0       26 2021-05-11 13:53:45.000000 ONE-api-1.9.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2022-02-24 20:11:44.618129 ONE-api-1.9.0/ONE_api.egg-info/
--rw-rw-rw-   0        0        0     3548 2022-02-24 20:11:44.000000 ONE-api-1.9.0/ONE_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      999 2022-02-24 20:11:44.000000 ONE-api-1.9.0/ONE_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-24 20:11:44.000000 ONE-api-1.9.0/ONE_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2022-02-24 20:11:44.000000 ONE-api-1.9.0/ONE_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2022-02-24 20:11:44.000000 ONE-api-1.9.0/ONE_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3548 2022-02-24 20:11:44.671499 ONE-api-1.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     2630 2022-02-23 11:50:16.000000 ONE-api-1.9.0/README.md
-drwxrwxrwx   0        0        0        0 2022-02-24 20:11:44.618129 ONE-api-1.9.0/one/
--rw-rw-rw-   0        0        0       77 2022-02-24 20:10:21.000000 ONE-api-1.9.0/one/__init__.py
-drwxrwxrwx   0        0        0        0 2022-02-24 20:11:44.633749 ONE-api-1.9.0/one/alf/
--rw-rw-rw-   0        0        0       70 2021-09-13 19:50:22.000000 ONE-api-1.9.0/one/alf/__init__.py
--rw-rw-rw-   0        0        0     9403 2022-02-23 11:50:16.000000 ONE-api-1.9.0/one/alf/cache.py
--rw-rw-rw-   0        0        0     3140 2022-02-23 11:50:16.000000 ONE-api-1.9.0/one/alf/exceptions.py
--rw-rw-rw-   0        0        0    13246 2022-02-07 18:31:32.000000 ONE-api-1.9.0/one/alf/files.py
--rw-rw-rw-   0        0        0    25822 2022-02-23 11:50:16.000000 ONE-api-1.9.0/one/alf/io.py
--rw-rw-rw-   0        0        0    17354 2022-02-07 18:31:32.000000 ONE-api-1.9.0/one/alf/spec.py
--rw-rw-rw-   0        0        0    91874 2022-02-24 20:10:01.000000 ONE-api-1.9.0/one/api.py
--rw-rw-rw-   0        0        0    26452 2022-02-23 11:50:16.000000 ONE-api-1.9.0/one/converters.py
--rw-rw-rw-   0        0        0    13047 2022-02-23 11:50:16.000000 ONE-api-1.9.0/one/params.py
--rw-rw-rw-   0        0        0    22671 2021-11-02 10:36:18.000000 ONE-api-1.9.0/one/registration.py
-drwxrwxrwx   0        0        0        0 2022-02-24 20:11:44.602506 ONE-api-1.9.0/one/tests/
-drwxrwxrwx   0        0        0        0 2022-02-24 20:11:44.633749 ONE-api-1.9.0/one/tests/fixtures/
--rw-rw-rw-   0        0        0    29918 2021-05-13 19:38:01.000000 ONE-api-1.9.0/one/tests/fixtures/datasets.pqt
-drwxrwxrwx   0        0        0        0 2022-02-24 20:11:44.671499 ONE-api-1.9.0/one/tests/fixtures/params/
--rw-rw-rw-   0        0        0      140 2021-09-13 19:50:22.000000 ONE-api-1.9.0/one/tests/fixtures/params/.caches
--rw-rw-rw-   0        0        0      276 2021-09-13 19:50:22.000000 ONE-api-1.9.0/one/tests/fixtures/params/.test.alyx.internationalbrainlab.org
-drwxrwxrwx   0        0        0        0 2022-02-24 20:11:44.671499 ONE-api-1.9.0/one/tests/fixtures/rest_responses/
--rw-rw-rw-   0        0        0      283 2021-09-13 19:50:22.000000 ONE-api-1.9.0/one/tests/fixtures/rest_responses/1f187d80fd59677b395fcdb18e68e4401bfa1cc9
--rw-rw-rw-   0        0        0     1370 2021-09-13 19:50:22.000000 ONE-api-1.9.0/one/tests/fixtures/rest_responses/47893cf67c985e6361cdee009334963f49fb0746
--rw-rw-rw-   0        0        0     1451 2021-09-13 19:50:22.000000 ONE-api-1.9.0/one/tests/fixtures/rest_responses/535d0e9a1e2c1efbdeba0d673b131e00361a2edb
--rw-rw-rw-   0        0        0      210 2021-09-13 19:50:22.000000 ONE-api-1.9.0/one/tests/fixtures/rest_responses/db1731fb8df0208944ae85f76718430813a8bf50
--rw-rw-rw-   0        0        0    22531 2021-05-12 14:50:16.000000 ONE-api-1.9.0/one/tests/fixtures/rest_responses/f530d6022f61cdc9e38cc66beb3cb71f3003c9a1
--rw-rw-rw-   0        0        0     6916 2021-05-13 19:38:01.000000 ONE-api-1.9.0/one/tests/fixtures/sessions.pqt
--rw-rw-rw-   0        0        0      324 2021-09-16 15:52:39.000000 ONE-api-1.9.0/one/tests/fixtures/test_dbs.json
--rw-rw-rw-   0        0        0   828598 2021-09-13 19:50:22.000000 ONE-api-1.9.0/one/tests/fixtures/test_img.png
--rw-rw-rw-   0        0        0    20558 2022-02-23 11:50:16.000000 ONE-api-1.9.0/one/util.py
--rw-rw-rw-   0        0        0    44825 2022-02-23 11:50:16.000000 ONE-api-1.9.0/one/webclient.py
--rw-rw-rw-   0        0        0       42 2022-02-24 20:11:44.671499 ONE-api-1.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1679 2022-02-23 11:50:16.000000 ONE-api-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-03-10 08:26:59.144333 ONE-api-1.9.1/
+-rw-rw-rw-   0        0        0       26 2021-05-11 13:53:45.000000 ONE-api-1.9.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2022-03-10 08:26:58.986750 ONE-api-1.9.1/ONE_api.egg-info/
+-rw-rw-rw-   0        0        0     3548 2022-03-10 08:26:58.000000 ONE-api-1.9.1/ONE_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1074 2022-03-10 08:26:58.000000 ONE-api-1.9.1/ONE_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-03-10 08:26:58.000000 ONE-api-1.9.1/ONE_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2022-03-10 08:26:58.000000 ONE-api-1.9.1/ONE_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2022-03-10 08:26:58.000000 ONE-api-1.9.1/ONE_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3548 2022-03-10 08:26:59.141336 ONE-api-1.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2630 2022-02-25 09:19:47.000000 ONE-api-1.9.1/README.md
+drwxrwxrwx   0        0        0        0 2022-03-10 08:26:59.003705 ONE-api-1.9.1/one/
+-rw-rw-rw-   0        0        0       77 2022-03-10 08:26:21.000000 ONE-api-1.9.1/one/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-10 08:26:59.018664 ONE-api-1.9.1/one/alf/
+-rw-rw-rw-   0        0        0       70 2021-09-13 19:50:22.000000 ONE-api-1.9.1/one/alf/__init__.py
+-rw-rw-rw-   0        0        0     9403 2022-02-25 09:19:47.000000 ONE-api-1.9.1/one/alf/cache.py
+-rw-rw-rw-   0        0        0     3140 2022-02-25 09:19:47.000000 ONE-api-1.9.1/one/alf/exceptions.py
+-rw-rw-rw-   0        0        0    13246 2022-02-07 18:31:32.000000 ONE-api-1.9.1/one/alf/files.py
+-rw-rw-rw-   0        0        0    25822 2022-02-25 09:19:47.000000 ONE-api-1.9.1/one/alf/io.py
+-rw-rw-rw-   0        0        0    17354 2022-02-07 18:31:32.000000 ONE-api-1.9.1/one/alf/spec.py
+-rw-rw-rw-   0        0        0    91408 2022-03-10 08:26:21.000000 ONE-api-1.9.1/one/api.py
+-rw-rw-rw-   0        0        0    26452 2022-02-25 09:19:47.000000 ONE-api-1.9.1/one/converters.py
+-rw-rw-rw-   0        0        0    13047 2022-02-25 09:19:47.000000 ONE-api-1.9.1/one/params.py
+-rw-rw-rw-   0        0        0    22671 2021-11-02 10:36:18.000000 ONE-api-1.9.1/one/registration.py
+drwxrwxrwx   0        0        0        0 2022-03-10 08:26:58.971790 ONE-api-1.9.1/one/tests/
+drwxrwxrwx   0        0        0        0 2022-03-10 08:26:59.030633 ONE-api-1.9.1/one/tests/fixtures/
+-rw-rw-rw-   0        0        0    29918 2021-05-13 19:38:01.000000 ONE-api-1.9.1/one/tests/fixtures/datasets.pqt
+drwxrwxrwx   0        0        0        0 2022-03-10 08:26:59.046589 ONE-api-1.9.1/one/tests/fixtures/params/
+-rw-rw-rw-   0        0        0      140 2021-09-13 19:50:22.000000 ONE-api-1.9.1/one/tests/fixtures/params/.caches
+-rw-rw-rw-   0        0        0      276 2021-09-13 19:50:22.000000 ONE-api-1.9.1/one/tests/fixtures/params/.test.alyx.internationalbrainlab.org
+drwxrwxrwx   0        0        0        0 2022-03-10 08:26:59.139349 ONE-api-1.9.1/one/tests/fixtures/rest_responses/
+-rw-rw-rw-   0        0        0      283 2021-09-13 19:50:22.000000 ONE-api-1.9.1/one/tests/fixtures/rest_responses/1f187d80fd59677b395fcdb18e68e4401bfa1cc9
+-rw-rw-rw-   0        0        0     1370 2021-09-13 19:50:22.000000 ONE-api-1.9.1/one/tests/fixtures/rest_responses/47893cf67c985e6361cdee009334963f49fb0746
+-rw-rw-rw-   0        0        0     1451 2021-09-13 19:50:22.000000 ONE-api-1.9.1/one/tests/fixtures/rest_responses/535d0e9a1e2c1efbdeba0d673b131e00361a2edb
+-rw-rw-rw-   0        0        0      210 2021-09-13 19:50:22.000000 ONE-api-1.9.1/one/tests/fixtures/rest_responses/db1731fb8df0208944ae85f76718430813a8bf50
+-rw-rw-rw-   0        0        0      417 2022-03-10 08:26:21.000000 ONE-api-1.9.1/one/tests/fixtures/rest_responses/dcce48259bb929661f60a02a48563f70aa6185b3
+-rw-rw-rw-   0        0        0    22531 2021-05-12 14:50:16.000000 ONE-api-1.9.1/one/tests/fixtures/rest_responses/f530d6022f61cdc9e38cc66beb3cb71f3003c9a1
+-rw-rw-rw-   0        0        0     6916 2021-05-13 19:38:01.000000 ONE-api-1.9.1/one/tests/fixtures/sessions.pqt
+-rw-rw-rw-   0        0        0      324 2021-09-16 15:52:39.000000 ONE-api-1.9.1/one/tests/fixtures/test_dbs.json
+-rw-rw-rw-   0        0        0   828598 2021-09-13 19:50:22.000000 ONE-api-1.9.1/one/tests/fixtures/test_img.png
+-rw-rw-rw-   0        0        0    20558 2022-02-25 09:19:47.000000 ONE-api-1.9.1/one/util.py
+-rw-rw-rw-   0        0        0    44825 2022-02-25 09:19:47.000000 ONE-api-1.9.1/one/webclient.py
+-rw-rw-rw-   0        0        0       42 2022-03-10 08:26:59.145325 ONE-api-1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1679 2022-02-25 09:19:47.000000 ONE-api-1.9.1/setup.py
```

### Comparing `ONE-api-1.9.0/ONE_api.egg-info/PKG-INFO` & `ONE-api-1.9.1/ONE_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ONE-api
-Version: 1.9.0
+Version: 1.9.1
 Summary: Open Neurophysiology Environment
 Home-page: https://github.com/int-brain-lab/ONE
 Author: IBL Staff
 License: MIT
 Description: # Open Neurophysiology Environment
         [![Coverage Status](https://coveralls.io/repos/github/int-brain-lab/ONE/badge.svg?branch=main)](https://coveralls.io/github/int-brain-lab/ONE?branch=main)
         ![CI workflow](https://github.com/int-brain-lab/ONE/actions/workflows/main.yaml/badge.svg?branch=main)
```

### Comparing `ONE-api-1.9.0/ONE_api.egg-info/SOURCES.txt` & `ONE-api-1.9.1/ONE_api.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -25,8 +25,9 @@
 one/tests/fixtures/test_img.png
 one/tests/fixtures/params/.caches
 one/tests/fixtures/params/.test.alyx.internationalbrainlab.org
 one/tests/fixtures/rest_responses/1f187d80fd59677b395fcdb18e68e4401bfa1cc9
 one/tests/fixtures/rest_responses/47893cf67c985e6361cdee009334963f49fb0746
 one/tests/fixtures/rest_responses/535d0e9a1e2c1efbdeba0d673b131e00361a2edb
 one/tests/fixtures/rest_responses/db1731fb8df0208944ae85f76718430813a8bf50
+one/tests/fixtures/rest_responses/dcce48259bb929661f60a02a48563f70aa6185b3
 one/tests/fixtures/rest_responses/f530d6022f61cdc9e38cc66beb3cb71f3003c9a1
```

### Comparing `ONE-api-1.9.0/PKG-INFO` & `ONE-api-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ONE-api
-Version: 1.9.0
+Version: 1.9.1
 Summary: Open Neurophysiology Environment
 Home-page: https://github.com/int-brain-lab/ONE
 Author: IBL Staff
 License: MIT
 Description: # Open Neurophysiology Environment
         [![Coverage Status](https://coveralls.io/repos/github/int-brain-lab/ONE/badge.svg?branch=main)](https://coveralls.io/github/int-brain-lab/ONE?branch=main)
         ![CI workflow](https://github.com/int-brain-lab/ONE/actions/workflows/main.yaml/badge.svg?branch=main)
```

### Comparing `ONE-api-1.9.0/README.md` & `ONE-api-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ONE-api-1.9.0/one/alf/cache.py` & `ONE-api-1.9.1/one/alf/cache.py`

 * *Files identical despite different names*

### Comparing `ONE-api-1.9.0/one/alf/exceptions.py` & `ONE-api-1.9.1/one/alf/exceptions.py`

 * *Files identical despite different names*

### Comparing `ONE-api-1.9.0/one/alf/files.py` & `ONE-api-1.9.1/one/alf/files.py`

 * *Files identical despite different names*

### Comparing `ONE-api-1.9.0/one/alf/io.py` & `ONE-api-1.9.1/one/alf/io.py`

 * *Files identical despite different names*

### Comparing `ONE-api-1.9.0/one/alf/spec.py` & `ONE-api-1.9.1/one/alf/spec.py`

 * *Files identical despite different names*

### Comparing `ONE-api-1.9.0/one/api.py` & `ONE-api-1.9.1/one/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1530,57 +1530,48 @@
             if 'exists_aws' in dsets and dsets['exists_aws'].all():
                 _logger.info('Downloading from AWS')
                 return self._download_aws(map(lambda x: x[1], dsets.iterrows()), **kwargs)
         except Exception as ex:
             _logger.debug(ex)
         return self._download_dataset(dsets, **kwargs)
 
-    def _download_aws(self, dsets, clobber=False, **kwargs) -> List[Path]:
+    def _download_aws(self, dsets, **kwargs) -> List[Path]:
         # Download datasets from AWS
         from tqdm import tqdm
         import boto3
         from botocore.exceptions import NoCredentialsError, PartialCredentialsError, ClientError
 
         def _callback_hook(t):
             # https://gist.github.com/wy193777/e7607d12fad13459e8992d4f69b53586
             # For example that uses actual file size:
             # boto3.amazonaws.com/v1/documentation/api/latest/_modules/boto3/s3/transfer.html
             def inner(bytes_amount):
                 t.update(bytes_amount)
             return inner
 
+        if self._index_type() is int:
+            raise NotImplementedError('AWS download only supported for str index cache')
         repo_json = self.alyx.rest('data-repository', 'read', id='aws_cortexlab')['json']
         bucket_name = repo_json['bucket_name']
         session_keys = {
             'aws_access_key_id': repo_json.get('Access key ID', None),
             'aws_secret_access_key': repo_json.get('Secret access key', None)
         }
         session = boto3.Session(**session_keys)
         s3 = session.resource('s3')
         out_files = []
         for dset in dsets:
-            dset_uuid = parquet.np2str(np.array(dset.name))
+            eid, dset_uuid = dset.name
             source_path = PurePosixPath('data').joinpath(
                 dset['session_path'], add_uuid_string(dset['rel_path'], dset_uuid)
             )
             local_path = alfio.remove_uuid_file(
                 self.cache_dir.joinpath(dset['session_path'], dset['rel_path']), dry=True)
             local_path.parent.mkdir(exist_ok=True, parents=True)
             out_files.append(local_path)
-            if local_path.exists():
-                # the local file hash doesn't match the dataset table cached hash
-                hash_mismatch = dset['hash'] and hashfile.md5(local_path) != dset['hash']
-                if hash_mismatch:
-                    clobber = True
-                    if not self.alyx.silent:
-                        _logger.warning(f'local md5 or size mismatch, re-downloading {local_path}')
-            else:
-                clobber = True
-            if local_path.exists() and not clobber:
-                continue
             try:
                 file_object = s3.Object(bucket_name, source_path.as_posix())
                 filesize = file_object.content_length
                 with tqdm(total=filesize, unit='B',
                           unit_scale=True, desc=local_path.as_posix()) as t:
                     file_object.download_file(Filename=str(local_path), Callback=_callback_hook(t))
             except (NoCredentialsError, PartialCredentialsError) as ex:
```

### Comparing `ONE-api-1.9.0/one/converters.py` & `ONE-api-1.9.1/one/converters.py`

 * *Files identical despite different names*

### Comparing `ONE-api-1.9.0/one/params.py` & `ONE-api-1.9.1/one/params.py`

 * *Files identical despite different names*

### Comparing `ONE-api-1.9.0/one/registration.py` & `ONE-api-1.9.1/one/registration.py`

 * *Files identical despite different names*

### Comparing `ONE-api-1.9.0/one/tests/fixtures/datasets.pqt` & `ONE-api-1.9.1/one/tests/fixtures/datasets.pqt`

 * *Files identical despite different names*

### Comparing `ONE-api-1.9.0/one/tests/fixtures/rest_responses/47893cf67c985e6361cdee009334963f49fb0746` & `ONE-api-1.9.1/one/tests/fixtures/rest_responses/47893cf67c985e6361cdee009334963f49fb0746`

 * *Files identical despite different names*

### Comparing `ONE-api-1.9.0/one/tests/fixtures/rest_responses/535d0e9a1e2c1efbdeba0d673b131e00361a2edb` & `ONE-api-1.9.1/one/tests/fixtures/rest_responses/535d0e9a1e2c1efbdeba0d673b131e00361a2edb`

 * *Files identical despite different names*

### Comparing `ONE-api-1.9.0/one/tests/fixtures/rest_responses/f530d6022f61cdc9e38cc66beb3cb71f3003c9a1` & `ONE-api-1.9.1/one/tests/fixtures/rest_responses/f530d6022f61cdc9e38cc66beb3cb71f3003c9a1`

 * *Files identical despite different names*

### Comparing `ONE-api-1.9.0/one/tests/fixtures/sessions.pqt` & `ONE-api-1.9.1/one/tests/fixtures/sessions.pqt`

 * *Files identical despite different names*

### Comparing `ONE-api-1.9.0/one/tests/fixtures/test_img.png` & `ONE-api-1.9.1/one/tests/fixtures/test_img.png`

 * *Files identical despite different names*

### Comparing `ONE-api-1.9.0/one/util.py` & `ONE-api-1.9.1/one/util.py`

 * *Files identical despite different names*

### Comparing `ONE-api-1.9.0/one/webclient.py` & `ONE-api-1.9.1/one/webclient.py`

 * *Files identical despite different names*

### Comparing `ONE-api-1.9.0/setup.py` & `ONE-api-1.9.1/setup.py`

 * *Files identical despite different names*

