# Comparing `tmp/nvosscript-1.2.8.tar.gz` & `tmp/nvosscript-1.2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.2.8.tar", last modified: Mon May  8 02:53:25 2023, max compression
+gzip compressed data, was "nvosscript-1.2.9.1.tar", last modified: Thu May 11 02:24:08 2023, max compression
```

## Comparing `nvosscript-1.2.8.tar` & `nvosscript-1.2.9.1.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-08 02:53:25.127411 nvosscript-1.2.8/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.2.8/LICENSE
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-05-08 02:53:25.127238 nvosscript-1.2.8/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.2.8/README.md
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-08 02:53:25.123672 nvosscript-1.2.8/nvos/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.2.8/nvos/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)    13019 2023-05-08 02:51:58.000000 nvosscript-1.2.8/nvos/file.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1662 2023-04-24 10:46:35.000000 nvosscript-1.2.8/nvos/login.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     8571 2023-04-25 06:40:19.000000 nvosscript-1.2.8/nvos/remote.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     4796 2023-04-24 10:50:50.000000 nvosscript-1.2.8/nvos/run.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      985 2023-04-25 03:15:56.000000 nvosscript-1.2.8/nvos/utils.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-08 02:53:25.124739 nvosscript-1.2.8/nvosscript.egg-info/
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-05-08 02:53:25.000000 nvosscript-1.2.8/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)      474 2023-05-08 02:53:25.000000 nvosscript-1.2.8/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-05-08 02:53:25.000000 nvosscript-1.2.8/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-05-08 02:53:25.000000 nvosscript-1.2.8/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-05-08 02:53:25.000000 nvosscript-1.2.8/nvosscript.egg-info/requires.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       28 2023-05-08 02:53:25.000000 nvosscript-1.2.8/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-05-08 02:53:25.127460 nvosscript-1.2.8/setup.cfg
--rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-05-08 02:52:29.000000 nvosscript-1.2.8/setup.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-08 02:53:25.125506 nvosscript-1.2.8/skyeye/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-18 06:53:13.000000 nvosscript-1.2.8/skyeye/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      712 2023-04-25 06:34:28.000000 nvosscript-1.2.8/skyeye/datahandler.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1797 2023-04-25 03:19:08.000000 nvosscript-1.2.8/skyeye/remote.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      240 2023-04-24 10:14:48.000000 nvosscript-1.2.8/skyeye/skyeyecommand.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-08 02:53:25.126607 nvosscript-1.2.8/start/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.2.8/start/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      185 2023-04-25 03:16:06.000000 nvosscript-1.2.8/start/commonUtil.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     4529 2023-05-08 02:52:35.000000 nvosscript-1.2.8/start/main.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-08 02:53:25.126895 nvosscript-1.2.8/win/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1273 2023-04-24 10:15:28.000000 nvosscript-1.2.8/win/win_auto_script.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-11 02:24:08.809830 nvosscript-1.2.9.1/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1073 2023-04-11 06:52:30.000000 nvosscript-1.2.9.1/LICENSE
+-rw-r--r--   0 matador.wang   (503) staff       (20)      335 2023-05-11 02:24:08.809695 nvosscript-1.2.9.1/PKG-INFO
+-rw-r--r--   0 matador.wang   (503) staff       (20)       78 2023-04-11 06:52:30.000000 nvosscript-1.2.9.1/README.md
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-11 02:24:08.807087 nvosscript-1.2.9.1/nvos/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 06:52:30.000000 nvosscript-1.2.9.1/nvos/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)    13051 2023-05-10 10:01:20.000000 nvosscript-1.2.9.1/nvos/file.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1662 2023-04-11 07:50:33.000000 nvosscript-1.2.9.1/nvos/login.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     9021 2023-05-10 10:01:27.000000 nvosscript-1.2.9.1/nvos/remote.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     4796 2023-05-04 01:42:28.000000 nvosscript-1.2.9.1/nvos/run.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      985 2023-05-04 01:42:28.000000 nvosscript-1.2.9.1/nvos/utils.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-11 02:24:08.808077 nvosscript-1.2.9.1/nvosscript.egg-info/
+-rw-r--r--   0 matador.wang   (503) staff       (20)      335 2023-05-11 02:24:08.000000 nvosscript-1.2.9.1/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 matador.wang   (503) staff       (20)      500 2023-05-11 02:24:08.000000 nvosscript-1.2.9.1/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)        1 2023-05-11 02:24:08.000000 nvosscript-1.2.9.1/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       41 2023-05-11 02:24:08.000000 nvosscript-1.2.9.1/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       47 2023-05-11 02:24:08.000000 nvosscript-1.2.9.1/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       27 2023-05-11 02:24:08.000000 nvosscript-1.2.9.1/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       38 2023-05-11 02:24:08.809865 nvosscript-1.2.9.1/setup.cfg
+-rw-r--r--   0 matador.wang   (503) staff       (20)      808 2023-05-11 02:23:52.000000 nvosscript-1.2.9.1/setup.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-11 02:24:08.808651 nvosscript-1.2.9.1/skyeye/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-05-04 01:42:28.000000 nvosscript-1.2.9.1/skyeye/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      712 2023-05-04 01:42:28.000000 nvosscript-1.2.9.1/skyeye/datahandler.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1797 2023-05-04 01:42:28.000000 nvosscript-1.2.9.1/skyeye/remote.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      240 2023-05-04 01:42:28.000000 nvosscript-1.2.9.1/skyeye/skyeyecommand.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-11 02:24:08.809031 nvosscript-1.2.9.1/start/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:50:33.000000 nvosscript-1.2.9.1/start/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      185 2023-05-04 01:42:28.000000 nvosscript-1.2.9.1/start/commonUtil.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     4532 2023-05-11 02:23:52.000000 nvosscript-1.2.9.1/start/main.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-11 02:24:08.805051 nvosscript-1.2.9.1/venv/
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-11 02:24:08.809256 nvosscript-1.2.9.1/venv/bin/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1175 2023-05-09 08:53:30.000000 nvosscript-1.2.9.1/venv/bin/activate_this.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-11 02:24:08.809499 nvosscript-1.2.9.1/win/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1273 2023-05-04 01:42:28.000000 nvosscript-1.2.9.1/win/win_auto_script.py
```

### Comparing `nvosscript-1.2.8/LICENSE` & `nvosscript-1.2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.8/nvos/file.py` & `nvosscript-1.2.9.1/nvos/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     file_list = []
     find_json_config(workspace_path, file_list, project_space_list)
     # 将来可以优化上传文件信息，针对于已经上传过的就不在上传
     with open(os.path.join(nvos_dir, "config"), 'w') as file:
         for item in file_list:
             file.write(json.dumps(item) + "\n")
 
-    remote.upload_file(file_list, project_space_list)
+    remote.upload_file(workspace_path, file_list, project_space_list)
 
     workspace_env = []
     if os.path.exists(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace_env"))):
         with open(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace_env")), 'r') as f:
             for line in f:
                 workspace_env.append(line.strip())
     workspace_env.append(workspace_path)
@@ -66,15 +66,15 @@
     find_json_config(workspace_path, file_list, project_space_list)
     add_file_list = []
     for temp in file_list:
         if "%s_%s" % (temp["file_path"], temp["git_branch"]) not in origin_file_map:
             add_file_list.append(temp)
     logger.info(f"push add_file_list: {add_file_list}")
     if len(add_file_list) > 0:
-        remote.upload_file(add_file_list, project_space_list)
+        remote.upload_file(workspace_path, add_file_list, project_space_list)
         logger.info(f"start save all file config ")
         origin_file_list.extend(add_file_list)
         with open(os.path.join(nvos_path, "config"), 'w') as f:
             for item in origin_file_list:
                 f.write(json.dumps(item) + "\n")
```

### Comparing `nvosscript-1.2.8/nvos/login.py` & `nvosscript-1.2.9.1/nvos/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.8/nvos/remote.py` & `nvosscript-1.2.9.1/nvos/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import hashlib
 import json
 import re
 import concurrent.futures
 import multiprocessing
 from tqdm import tqdm
 from nvos import login
+from start import commonUtil
 import logging
 
 # 导入全局日志记录器
 logger = logging.getLogger(__name__)
 daemon_network = "https://nvos-toolchain.nioint.com"
 
 daemon_network_mapping = {
@@ -63,15 +64,23 @@
     aws_sk = s3_secret["sk"]
     aws_region = s3_secret["regionId"]
     s3 = boto3.resource('s3', region_name=aws_region, aws_access_key_id=aws_ak,
                         aws_secret_access_key=aws_sk)
     bucket = s3.Bucket(bucket_name)
     bucket.upload_file(file_path, file_name)
 
-def upload_file(file_path_list, project_space_list):
+
+def file_upload_notify(workspace_path, project_list):
+    get_current_env()
+    url = "%s%s" % (daemon_network, "/workspace/analyse")
+    post_param = {"userId": login.get_user_id(), "fileDirectory": workspace_path, "projectSpaceList": project_list}
+    data = post_data(url, post_param)
+    return data
+
+def upload_file(workspace_path, file_path_list, project_space_list):
     s3_secret = get_s3_secret()
     bucket_name = s3_secret["bucket"]
     aws_ak = s3_secret["ak"]
     aws_sk = s3_secret["sk"]
     aws_region = s3_secret["regionId"]
     s3 = boto3.resource('s3', region_name=aws_region, aws_access_key_id=aws_ak,
                         aws_secret_access_key=aws_sk)
@@ -95,14 +104,15 @@
                                           .find(os.path.basename(project_space["project_space"])):])
                 file_name = file_name.replace("\\", "/")
                 local_file_path = file_path["file_path"]
                 temp_file = {"local_file_path": local_file_path, "file_name": file_name}
                 upload_list.append(temp_file)
     upload_process(upload_list, bucket)
 
+    file_upload_notify(workspace_path, project_space_list)
 
 def upload_process(upload_list, bucket):
     global global_var
     multiprocessing.set_start_method('spawn', True)
     cores = multiprocessing.cpu_count()
     with concurrent.futures.ThreadPoolExecutor(max_workers=cores) as executor, tqdm(desc="uploading", total=len(upload_list)) as progress:
         for index, file in enumerate(upload_list):
@@ -158,15 +168,15 @@
     post_param = {"userId": login.get_user_id(), "fileDirectory": workspace_path, "projectSpaceList": project_list}
     return post_data(url, post_param)
 
 
 def pull_workspace(workspace, project_list):
     get_current_env()
     url = "%s%s" % (daemon_network, "/workspace/getChangedFiles")
-    post_param = {"userId": login.get_user_id(), "fileDirectory": workspace,"projectSpaceList": project_list}
+    post_param = {"userId": login.get_user_id(), "fileDirectory": workspace, "projectSpaceList": project_list}
     return post_data(url, post_param)
 
 
 def post_data(url, params):
     headers = {"content-type": "application/json"}
     logger.info(f'request url:{url} params:{params}')
     response = requests.post(url, headers=headers, data=json.dumps(params))
@@ -207,14 +217,15 @@
 
 def switch_env(env):
     val = daemon_network_mapping.get(env)
     if len(val) == 0:
         return
     tip = daemon_network_front_mapping.get(env)
     result = {"cloud":val,"tip":tip,"env":env}
+    commonUtil.check_local_workspace()
     with open(os.path.expanduser(os.path.join('~','.ndtcrc' ,'nvos_env')), 'w') as f:
         f.writelines(json.dumps(result))
     print(f"this script current env:{env} and cloud linked:{tip}")
 
 
 def get_current_env():
     global daemon_network
```

### Comparing `nvosscript-1.2.8/nvos/run.py` & `nvosscript-1.2.9.1/nvos/run.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.8/nvos/utils.py` & `nvosscript-1.2.9.1/nvos/utils.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.8/setup.py` & `nvosscript-1.2.9.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.2.8',
+    version='1.2.9.01',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.2.8/skyeye/datahandler.py` & `nvosscript-1.2.9.1/skyeye/datahandler.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.8/skyeye/remote.py` & `nvosscript-1.2.9.1/skyeye/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.8/start/main.py` & `nvosscript-1.2.9.1/start/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     elif args.subcommand == "async":
         run.command_async(args.type)
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.2.8")
+        print("1.2.9.01")
     elif args.subcommand == 'env':
         switch_command_env(args.module, args.switch)
     elif args.subcommand == "upload":
         switch_command_upload(args.module, args.log)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
```

### Comparing `nvosscript-1.2.8/win/win_auto_script.py` & `nvosscript-1.2.9.1/win/win_auto_script.py`

 * *Files identical despite different names*

