# Comparing `tmp/cobra-archiver-0.0.4.tar.gz` & `tmp/cobra-archiver-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobra-archiver-0.0.4.tar", last modified: Mon Feb 20 20:29:09 2023, max compression
+gzip compressed data, was "cobra-archiver-0.0.5.tar", last modified: Thu May 11 19:55:43 2023, max compression
```

## Comparing `cobra-archiver-0.0.4.tar` & `cobra-archiver-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-02-20 20:29:09.167556 cobra-archiver-0.0.4/
--rw-r--r--   0 q         (1000) q         (1000)     1023 2023-02-02 05:43:02.000000 cobra-archiver-0.0.4/LICENSE
--rw-r--r--   0 q         (1000) q         (1000)     6249 2023-02-20 20:29:09.167556 cobra-archiver-0.0.4/PKG-INFO
--rw-r--r--   0 q         (1000) q         (1000)     5671 2023-02-20 20:28:43.000000 cobra-archiver-0.0.4/README.md
--rw-r--r--   0 q         (1000) q         (1000)      100 2023-02-09 16:37:57.000000 cobra-archiver-0.0.4/pyproject.toml
--rw-r--r--   0 q         (1000) q         (1000)     1600 2023-02-20 20:29:09.167556 cobra-archiver-0.0.4/setup.cfg
-drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-02-20 20:29:09.150890 cobra-archiver-0.0.4/src/
-drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-02-20 20:29:09.164223 cobra-archiver-0.0.4/src/cobra/
--rw-r--r--   0 q         (1000) q         (1000)       23 2023-02-20 20:28:58.000000 cobra-archiver-0.0.4/src/cobra/__init__.py
--rw-r--r--   0 q         (1000) q         (1000)       79 2023-02-07 21:59:32.000000 cobra-archiver-0.0.4/src/cobra/__main__.py
--rw-r--r--   0 q         (1000) q         (1000)    15265 2023-02-20 20:06:57.000000 cobra-archiver-0.0.4/src/cobra/api.py
--rw-r--r--   0 q         (1000) q         (1000)    13930 2023-02-19 13:10:57.000000 cobra-archiver-0.0.4/src/cobra/api_test.py
--rw-r--r--   0 q         (1000) q         (1000)      287 2023-02-06 18:20:28.000000 cobra-archiver-0.0.4/src/cobra/aux_stuff.py
--rw-r--r--   0 q         (1000) q         (1000)    30698 2023-02-20 11:00:26.000000 cobra-archiver-0.0.4/src/cobra/banner.py
--rw-r--r--   0 q         (1000) q         (1000)    12573 2023-02-20 20:05:02.000000 cobra-archiver-0.0.4/src/cobra/cli.py
--rw-r--r--   0 q         (1000) q         (1000)      855 2023-02-08 20:52:04.000000 cobra-archiver-0.0.4/src/cobra/cli_handler.py
--rw-r--r--   0 q         (1000) q         (1000)     2378 2023-02-08 20:48:15.000000 cobra-archiver-0.0.4/src/cobra/cli_handler_test.py
--rw-r--r--   0 q         (1000) q         (1000)     4783 2023-02-17 16:08:36.000000 cobra-archiver-0.0.4/src/cobra/cli_test.py
--rw-r--r--   0 q         (1000) q         (1000)      615 2023-02-19 13:31:50.000000 cobra-archiver-0.0.4/src/cobra/conftest.py
--rw-r--r--   0 q         (1000) q         (1000)      134 2023-02-07 22:02:02.000000 cobra-archiver-0.0.4/src/cobra/exc.py
--rw-r--r--   0 q         (1000) q         (1000)     3852 2023-02-10 21:53:36.000000 cobra-archiver-0.0.4/src/cobra/google_drive.py
--rw-r--r--   0 q         (1000) q         (1000)     3807 2023-02-19 14:01:06.000000 cobra-archiver-0.0.4/src/cobra/hooks.py
--rw-r--r--   0 q         (1000) q         (1000)     3177 2023-02-19 14:03:12.000000 cobra-archiver-0.0.4/src/cobra/hooks_test.py
-drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-02-20 20:29:09.167556 cobra-archiver-0.0.4/src/cobra_archiver.egg-info/
--rw-r--r--   0 q         (1000) q         (1000)     6249 2023-02-20 20:29:09.000000 cobra-archiver-0.0.4/src/cobra_archiver.egg-info/PKG-INFO
--rw-r--r--   0 q         (1000) q         (1000)      624 2023-02-20 20:29:09.000000 cobra-archiver-0.0.4/src/cobra_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 q         (1000) q         (1000)        1 2023-02-20 20:29:09.000000 cobra-archiver-0.0.4/src/cobra_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 q         (1000) q         (1000)       41 2023-02-20 20:29:09.000000 cobra-archiver-0.0.4/src/cobra_archiver.egg-info/entry_points.txt
--rw-r--r--   0 q         (1000) q         (1000)      757 2023-02-20 20:29:09.000000 cobra-archiver-0.0.4/src/cobra_archiver.egg-info/requires.txt
--rw-r--r--   0 q         (1000) q         (1000)        6 2023-02-20 20:29:09.000000 cobra-archiver-0.0.4/src/cobra_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-11 19:55:43.308005 cobra-archiver-0.0.5/
+-rw-r--r--   0 q         (1000) q         (1000)     1023 2023-02-02 05:43:02.000000 cobra-archiver-0.0.5/LICENSE
+-rw-r--r--   0 q         (1000) q         (1000)     6403 2023-05-11 19:55:43.308005 cobra-archiver-0.0.5/PKG-INFO
+-rw-r--r--   0 q         (1000) q         (1000)     5825 2023-05-10 20:45:47.000000 cobra-archiver-0.0.5/README.md
+-rw-r--r--   0 q         (1000) q         (1000)      100 2023-02-09 16:37:57.000000 cobra-archiver-0.0.5/pyproject.toml
+-rw-r--r--   0 q         (1000) q         (1000)     1572 2023-05-11 19:55:43.311338 cobra-archiver-0.0.5/setup.cfg
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-11 19:55:43.264672 cobra-archiver-0.0.5/src/
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-11 19:55:43.304672 cobra-archiver-0.0.5/src/cobra/
+-rw-r--r--   0 q         (1000) q         (1000)       23 2023-05-11 19:55:34.000000 cobra-archiver-0.0.5/src/cobra/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)       79 2023-02-07 21:59:32.000000 cobra-archiver-0.0.5/src/cobra/__main__.py
+-rw-r--r--   0 q         (1000) q         (1000)    15265 2023-05-10 17:59:26.000000 cobra-archiver-0.0.5/src/cobra/api.py
+-rw-r--r--   0 q         (1000) q         (1000)    13930 2023-02-19 13:10:57.000000 cobra-archiver-0.0.5/src/cobra/api_test.py
+-rw-r--r--   0 q         (1000) q         (1000)      287 2023-02-06 18:20:28.000000 cobra-archiver-0.0.5/src/cobra/aux_stuff.py
+-rw-r--r--   0 q         (1000) q         (1000)    30698 2023-02-20 11:00:26.000000 cobra-archiver-0.0.5/src/cobra/banner.py
+-rw-r--r--   0 q         (1000) q         (1000)    12573 2023-02-20 20:05:02.000000 cobra-archiver-0.0.5/src/cobra/cli.py
+-rw-r--r--   0 q         (1000) q         (1000)      855 2023-02-08 20:52:04.000000 cobra-archiver-0.0.5/src/cobra/cli_handler.py
+-rw-r--r--   0 q         (1000) q         (1000)     2378 2023-02-08 20:48:15.000000 cobra-archiver-0.0.5/src/cobra/cli_handler_test.py
+-rw-r--r--   0 q         (1000) q         (1000)     4783 2023-02-17 16:08:36.000000 cobra-archiver-0.0.5/src/cobra/cli_test.py
+-rw-r--r--   0 q         (1000) q         (1000)      615 2023-02-19 13:31:50.000000 cobra-archiver-0.0.5/src/cobra/conftest.py
+-rw-r--r--   0 q         (1000) q         (1000)      134 2023-02-07 22:02:02.000000 cobra-archiver-0.0.5/src/cobra/exc.py
+-rw-r--r--   0 q         (1000) q         (1000)     3168 2023-05-11 19:48:58.000000 cobra-archiver-0.0.5/src/cobra/google_drive.py
+-rw-r--r--   0 q         (1000) q         (1000)     3807 2023-02-19 14:01:06.000000 cobra-archiver-0.0.5/src/cobra/hooks.py
+-rw-r--r--   0 q         (1000) q         (1000)     3177 2023-02-19 14:03:12.000000 cobra-archiver-0.0.5/src/cobra/hooks_test.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-11 19:55:43.308005 cobra-archiver-0.0.5/src/cobra_archiver.egg-info/
+-rw-r--r--   0 q         (1000) q         (1000)     6403 2023-05-11 19:55:43.000000 cobra-archiver-0.0.5/src/cobra_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 q         (1000) q         (1000)      624 2023-05-11 19:55:43.000000 cobra-archiver-0.0.5/src/cobra_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 q         (1000) q         (1000)        1 2023-05-11 19:55:43.000000 cobra-archiver-0.0.5/src/cobra_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 q         (1000) q         (1000)       41 2023-05-11 19:55:43.000000 cobra-archiver-0.0.5/src/cobra_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 q         (1000) q         (1000)      730 2023-05-11 19:55:43.000000 cobra-archiver-0.0.5/src/cobra_archiver.egg-info/requires.txt
+-rw-r--r--   0 q         (1000) q         (1000)        6 2023-05-11 19:55:43.000000 cobra-archiver-0.0.5/src/cobra_archiver.egg-info/top_level.txt
```

### Comparing `cobra-archiver-0.0.4/LICENSE` & `cobra-archiver-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cobra-archiver-0.0.4/PKG-INFO` & `cobra-archiver-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobra-archiver
-Version: 0.0.4
+Version: 0.0.5
 Summary: Comprehensive Backing up and Restoration Archiver. Docker volumes, bind mounts and plain directory backup automation tool.
 Home-page: https://github.com/yell0w4x/cobra
 Author: yell0w4x
 Author-email: yell0w4x@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yell0w4x/cobra/issues
 Keywords: Docker volumes backup
@@ -71,15 +71,15 @@
          'before_pull', 'after_pull', 'before_restore', 'after_restore')
 ```
 
 One can either issue `cobra hooks init` that populates hook files to the default directory. 
 Or put the hook files with the names e.g. `before_build.py` or `before_build.sh`. 
 For shell script `chmod +x before_build.sh` is necessary.
 
-Cobra searches for `.py` file first if found imports it and execute `hook` fucntion as.
+Cobra searches for `.py` file first if found imports it and execute `hook` function as.
 
 ```python
 hook(hook_name=hook_name, hooks_dir=hooks_dir, backup_dir=backup_dir, 
      filename=backup_filename, docker=docker_client)
 ```
 
 * `hook_name` is the one from the list above
@@ -102,15 +102,15 @@
 # Stop any containers that mangle database while dumping to have consistent dump
 docker stop my-excellent-app
 
 MONGO_DUMP_DIR=/tmp/mongodump
 mkdir -p "${MONGO_DUMP_DIR}"
 mongodump --archive="${MONGO_DUMP_DIR}/mongo-dump-by-hook.tar.gz" --db=test --gzip mongodb://mongo-container-name:27017
 
-Then start them again
+# Then start them again
 docker start my-excellent-app
 ```
 
 Errors that are propagated from hooks stop farther processing. 
 To see more details please inspect e2e test sources.
 
 ### Default locations
@@ -136,14 +136,19 @@
 
 api = Api(gateway=DockerClient(), hooks=Hooks())
 api.backup_build()
 ```
 
 Method parameters are described in cli help `cobra backup --help` e.g.
 
+### Security notice
+
+This code is subject to command injection vulnerabilty. There are no such a checks. 
+The caller should provide all checks on his own.
+
 ## Run tests
 
 ```bash
 git clone https://github.com/yell0w4x/cobra.git
 cd cobra
 ./run-tests --unit
 ```
@@ -161,15 +166,15 @@
 GOOGLE_DRIVE_FOLDER_ID=goolge-drive-folder-id GOOGLE_SERVICE_ACC_KEY=path/to/key.json ./run-tests --e2e
 ```
 
 The tests are based on pytest. All the extra arguments are passed to pytest. 
 E.g. to have verbose output use `-v` or `-vv`. To show stdout `-s`. 
 To run certain tests use `-k test_name` and etc. For details see the pytest docs.
 
-```bash
+```
 ./run-tests --help
 Run cobra unit and e2e tests.
 
 Usage:
     ./run-tests [OPTIONS] [EXTRA_ARGS]
 
 All the EXTRA_ARGS are passed to pytest
```

### Comparing `cobra-archiver-0.0.4/README.md` & `cobra-archiver-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
          'before_pull', 'after_pull', 'before_restore', 'after_restore')
 ```
 
 One can either issue `cobra hooks init` that populates hook files to the default directory. 
 Or put the hook files with the names e.g. `before_build.py` or `before_build.sh`. 
 For shell script `chmod +x before_build.sh` is necessary.
 
-Cobra searches for `.py` file first if found imports it and execute `hook` fucntion as.
+Cobra searches for `.py` file first if found imports it and execute `hook` function as.
 
 ```python
 hook(hook_name=hook_name, hooks_dir=hooks_dir, backup_dir=backup_dir, 
      filename=backup_filename, docker=docker_client)
 ```
 
 * `hook_name` is the one from the list above
@@ -86,15 +86,15 @@
 # Stop any containers that mangle database while dumping to have consistent dump
 docker stop my-excellent-app
 
 MONGO_DUMP_DIR=/tmp/mongodump
 mkdir -p "${MONGO_DUMP_DIR}"
 mongodump --archive="${MONGO_DUMP_DIR}/mongo-dump-by-hook.tar.gz" --db=test --gzip mongodb://mongo-container-name:27017
 
-Then start them again
+# Then start them again
 docker start my-excellent-app
 ```
 
 Errors that are propagated from hooks stop farther processing. 
 To see more details please inspect e2e test sources.
 
 ### Default locations
@@ -120,14 +120,19 @@
 
 api = Api(gateway=DockerClient(), hooks=Hooks())
 api.backup_build()
 ```
 
 Method parameters are described in cli help `cobra backup --help` e.g.
 
+### Security notice
+
+This code is subject to command injection vulnerabilty. There are no such a checks. 
+The caller should provide all checks on his own.
+
 ## Run tests
 
 ```bash
 git clone https://github.com/yell0w4x/cobra.git
 cd cobra
 ./run-tests --unit
 ```
@@ -145,15 +150,15 @@
 GOOGLE_DRIVE_FOLDER_ID=goolge-drive-folder-id GOOGLE_SERVICE_ACC_KEY=path/to/key.json ./run-tests --e2e
 ```
 
 The tests are based on pytest. All the extra arguments are passed to pytest. 
 E.g. to have verbose output use `-v` or `-vv`. To show stdout `-s`. 
 To run certain tests use `-k test_name` and etc. For details see the pytest docs.
 
-```bash
+```
 ./run-tests --help
 Run cobra unit and e2e tests.
 
 Usage:
     ./run-tests [OPTIONS] [EXTRA_ARGS]
 
 All the EXTRA_ARGS are passed to pytest
```

### Comparing `cobra-archiver-0.0.4/setup.cfg` & `cobra-archiver-0.0.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.0.4
+version = 0.0.5
 name = cobra-archiver
 author = yell0w4x
 author_email = yell0w4x@gmail.com
 description = Comprehensive Backing up and Restoration Archiver. Docker volumes, bind mounts and plain directory backup automation tool.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/yell0w4x/cobra
@@ -46,15 +46,14 @@
 	protobuf==4.21.12
 	pyasn1==0.4.8
 	pyasn1-modules==0.2.8
 	Pygments==2.14.0
 	pyparsing==3.0.9
 	pyproject_hooks==1.0.0
 	pytest==7.2.1
-	pytest-lazy-fixture==0.6.3
 	python-dateutil==2.8.2
 	requests==2.28.2
 	requests-oauthlib==1.3.1
 	rich==13.3.1
 	rsa==4.9
 	six==1.16.0
 	tomli==2.0.1
```

### Comparing `cobra-archiver-0.0.4/src/cobra/api.py` & `cobra-archiver-0.0.5/src/cobra/api.py`

 * *Files identical despite different names*

### Comparing `cobra-archiver-0.0.4/src/cobra/api_test.py` & `cobra-archiver-0.0.5/src/cobra/api_test.py`

 * *Files identical despite different names*

### Comparing `cobra-archiver-0.0.4/src/cobra/banner.py` & `cobra-archiver-0.0.5/src/cobra/banner.py`

 * *Files identical despite different names*

### Comparing `cobra-archiver-0.0.4/src/cobra/cli.py` & `cobra-archiver-0.0.5/src/cobra/cli.py`

 * *Files identical despite different names*

### Comparing `cobra-archiver-0.0.4/src/cobra/cli_handler.py` & `cobra-archiver-0.0.5/src/cobra/cli_handler.py`

 * *Files identical despite different names*

### Comparing `cobra-archiver-0.0.4/src/cobra/cli_handler_test.py` & `cobra-archiver-0.0.5/src/cobra/cli_handler_test.py`

 * *Files identical despite different names*

### Comparing `cobra-archiver-0.0.4/src/cobra/cli_test.py` & `cobra-archiver-0.0.5/src/cobra/cli_test.py`

 * *Files identical despite different names*

### Comparing `cobra-archiver-0.0.4/src/cobra/conftest.py` & `cobra-archiver-0.0.5/src/cobra/conftest.py`

 * *Files identical despite different names*

### Comparing `cobra-archiver-0.0.4/src/cobra/google_drive.py` & `cobra-archiver-0.0.5/src/cobra/google_drive.py`

 * *Files 18% similar despite different names*

```diff
@@ -86,24 +86,7 @@
                                    fields='files(id,name,createdTime,modifiedTime,size,md5Checksum)',
                                    corpora='allDrives',
                                    supportsAllDrives=True, 
                                    includeItemsFromAllDrives=True,
                                    orderBy='createdTime').execute()
 
     return results.get('files', [])
-
-
-if __name__ == '__main__':
-    # drive_list('../../.temp/4xybox-service-account-key.json')
-    # drives_create('../../.temp/4xybox-service-account-key.json')
-    # drive_info('../../.temp/4xybox-service-account-key.json')
-    # upload_file('../../.temp/4xybox-service-account-key.json', 
-    #             './__init__.py', 'application/json', 
-    #             '__init__.py', '100d96r89SxvJvm7ZUqFCOztaiZv6sBIA')
-    try:
-        gen = download_file('.temp/4xybox-service-account-key.json', '1-dooih8zN9ze0BH6Asu7rxuMqMfRoRyq', './.temp')
-        while True:
-            status = next(gen)
-    except StopIteration as e:
-        # content, fn = e.value
-        print(e.value)
-
```

### Comparing `cobra-archiver-0.0.4/src/cobra/hooks.py` & `cobra-archiver-0.0.5/src/cobra/hooks.py`

 * *Files identical despite different names*

### Comparing `cobra-archiver-0.0.4/src/cobra/hooks_test.py` & `cobra-archiver-0.0.5/src/cobra/hooks_test.py`

 * *Files identical despite different names*

### Comparing `cobra-archiver-0.0.4/src/cobra_archiver.egg-info/PKG-INFO` & `cobra-archiver-0.0.5/src/cobra_archiver.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobra-archiver
-Version: 0.0.4
+Version: 0.0.5
 Summary: Comprehensive Backing up and Restoration Archiver. Docker volumes, bind mounts and plain directory backup automation tool.
 Home-page: https://github.com/yell0w4x/cobra
 Author: yell0w4x
 Author-email: yell0w4x@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yell0w4x/cobra/issues
 Keywords: Docker volumes backup
@@ -71,15 +71,15 @@
          'before_pull', 'after_pull', 'before_restore', 'after_restore')
 ```
 
 One can either issue `cobra hooks init` that populates hook files to the default directory. 
 Or put the hook files with the names e.g. `before_build.py` or `before_build.sh`. 
 For shell script `chmod +x before_build.sh` is necessary.
 
-Cobra searches for `.py` file first if found imports it and execute `hook` fucntion as.
+Cobra searches for `.py` file first if found imports it and execute `hook` function as.
 
 ```python
 hook(hook_name=hook_name, hooks_dir=hooks_dir, backup_dir=backup_dir, 
      filename=backup_filename, docker=docker_client)
 ```
 
 * `hook_name` is the one from the list above
@@ -102,15 +102,15 @@
 # Stop any containers that mangle database while dumping to have consistent dump
 docker stop my-excellent-app
 
 MONGO_DUMP_DIR=/tmp/mongodump
 mkdir -p "${MONGO_DUMP_DIR}"
 mongodump --archive="${MONGO_DUMP_DIR}/mongo-dump-by-hook.tar.gz" --db=test --gzip mongodb://mongo-container-name:27017
 
-Then start them again
+# Then start them again
 docker start my-excellent-app
 ```
 
 Errors that are propagated from hooks stop farther processing. 
 To see more details please inspect e2e test sources.
 
 ### Default locations
@@ -136,14 +136,19 @@
 
 api = Api(gateway=DockerClient(), hooks=Hooks())
 api.backup_build()
 ```
 
 Method parameters are described in cli help `cobra backup --help` e.g.
 
+### Security notice
+
+This code is subject to command injection vulnerabilty. There are no such a checks. 
+The caller should provide all checks on his own.
+
 ## Run tests
 
 ```bash
 git clone https://github.com/yell0w4x/cobra.git
 cd cobra
 ./run-tests --unit
 ```
@@ -161,15 +166,15 @@
 GOOGLE_DRIVE_FOLDER_ID=goolge-drive-folder-id GOOGLE_SERVICE_ACC_KEY=path/to/key.json ./run-tests --e2e
 ```
 
 The tests are based on pytest. All the extra arguments are passed to pytest. 
 E.g. to have verbose output use `-v` or `-vv`. To show stdout `-s`. 
 To run certain tests use `-k test_name` and etc. For details see the pytest docs.
 
-```bash
+```
 ./run-tests --help
 Run cobra unit and e2e tests.
 
 Usage:
     ./run-tests [OPTIONS] [EXTRA_ARGS]
 
 All the EXTRA_ARGS are passed to pytest
```

### Comparing `cobra-archiver-0.0.4/src/cobra_archiver.egg-info/SOURCES.txt` & `cobra-archiver-0.0.5/src/cobra_archiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cobra-archiver-0.0.4/src/cobra_archiver.egg-info/requires.txt` & `cobra-archiver-0.0.5/src/cobra_archiver.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 protobuf==4.21.12
 pyasn1==0.4.8
 pyasn1-modules==0.2.8
 Pygments==2.14.0
 pyparsing==3.0.9
 pyproject_hooks==1.0.0
 pytest==7.2.1
-pytest-lazy-fixture==0.6.3
 python-dateutil==2.8.2
 requests==2.28.2
 requests-oauthlib==1.3.1
 rich==13.3.1
 rsa==4.9
 six==1.16.0
 tomli==2.0.1
```

