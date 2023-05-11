# Comparing `tmp/apkupload-0.0.8.tar.gz` & `tmp/apkupload-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkupload-0.0.8.tar", last modified: Tue Apr  4 02:52:13 2023, max compression
+gzip compressed data, was "apkupload-0.0.9.tar", last modified: Tue Apr  4 06:21:11 2023, max compression
```

## Comparing `apkupload-0.0.8.tar` & `apkupload-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shareit    (501) staff       (20)        0 2023-04-04 02:52:13.382161 apkupload-0.0.8/
--rw-r--r--   0 shareit    (501) staff       (20)     1065 2023-02-16 09:11:36.000000 apkupload-0.0.8/LICENSE
--rw-r--r--   0 shareit    (501) staff       (20)      381 2023-04-04 02:52:13.382011 apkupload-0.0.8/PKG-INFO
--rw-r--r--   0 shareit    (501) staff       (20)       12 2023-04-04 02:51:33.000000 apkupload-0.0.8/README.md
-drwxr-xr-x   0 shareit    (501) staff       (20)        0 2023-04-04 02:52:13.380807 apkupload-0.0.8/apkupload/
--rw-r--r--   0 shareit    (501) staff       (20)        0 2023-02-16 09:32:25.000000 apkupload-0.0.8/apkupload/__init__.py
--rw-r--r--   0 shareit    (501) staff       (20)       62 2023-02-16 10:22:55.000000 apkupload-0.0.8/apkupload/__main__.py
--rw-r--r--   0 shareit    (501) staff       (20)     7486 2023-04-04 02:40:54.000000 apkupload-0.0.8/apkupload/upload.py
-drwxr-xr-x   0 shareit    (501) staff       (20)        0 2023-04-04 02:52:13.381828 apkupload-0.0.8/apkupload.egg-info/
--rw-r--r--   0 shareit    (501) staff       (20)      381 2023-04-04 02:52:13.000000 apkupload-0.0.8/apkupload.egg-info/PKG-INFO
--rw-r--r--   0 shareit    (501) staff       (20)      258 2023-04-04 02:52:13.000000 apkupload-0.0.8/apkupload.egg-info/SOURCES.txt
--rw-r--r--   0 shareit    (501) staff       (20)        1 2023-04-04 02:52:13.000000 apkupload-0.0.8/apkupload.egg-info/dependency_links.txt
--rw-r--r--   0 shareit    (501) staff       (20)       52 2023-04-04 02:52:13.000000 apkupload-0.0.8/apkupload.egg-info/entry_points.txt
--rw-r--r--   0 shareit    (501) staff       (20)       10 2023-04-04 02:52:13.000000 apkupload-0.0.8/apkupload.egg-info/top_level.txt
--rw-r--r--   0 shareit    (501) staff       (20)       38 2023-04-04 02:52:13.382200 apkupload-0.0.8/setup.cfg
--rw-r--r--   0 shareit    (501) staff       (20)      670 2023-04-04 02:48:51.000000 apkupload-0.0.8/setup.py
+drwxr-xr-x   0 shareit    (501) staff       (20)        0 2023-04-04 06:21:11.196390 apkupload-0.0.9/
+-rw-r--r--   0 shareit    (501) staff       (20)     1065 2023-02-16 09:11:36.000000 apkupload-0.0.9/LICENSE
+-rw-r--r--   0 shareit    (501) staff       (20)      381 2023-04-04 06:21:11.196246 apkupload-0.0.9/PKG-INFO
+-rw-r--r--   0 shareit    (501) staff       (20)       12 2023-04-04 02:51:33.000000 apkupload-0.0.9/README.md
+drwxr-xr-x   0 shareit    (501) staff       (20)        0 2023-04-04 06:21:11.195286 apkupload-0.0.9/apkupload/
+-rw-r--r--   0 shareit    (501) staff       (20)        0 2023-02-16 09:32:25.000000 apkupload-0.0.9/apkupload/__init__.py
+-rw-r--r--   0 shareit    (501) staff       (20)       62 2023-02-16 10:22:55.000000 apkupload-0.0.9/apkupload/__main__.py
+-rw-r--r--   0 shareit    (501) staff       (20)     7866 2023-04-04 06:19:48.000000 apkupload-0.0.9/apkupload/upload.py
+drwxr-xr-x   0 shareit    (501) staff       (20)        0 2023-04-04 06:21:11.196082 apkupload-0.0.9/apkupload.egg-info/
+-rw-r--r--   0 shareit    (501) staff       (20)      381 2023-04-04 06:21:11.000000 apkupload-0.0.9/apkupload.egg-info/PKG-INFO
+-rw-r--r--   0 shareit    (501) staff       (20)      258 2023-04-04 06:21:11.000000 apkupload-0.0.9/apkupload.egg-info/SOURCES.txt
+-rw-r--r--   0 shareit    (501) staff       (20)        1 2023-04-04 06:21:11.000000 apkupload-0.0.9/apkupload.egg-info/dependency_links.txt
+-rw-r--r--   0 shareit    (501) staff       (20)       52 2023-04-04 06:21:11.000000 apkupload-0.0.9/apkupload.egg-info/entry_points.txt
+-rw-r--r--   0 shareit    (501) staff       (20)       10 2023-04-04 06:21:11.000000 apkupload-0.0.9/apkupload.egg-info/top_level.txt
+-rw-r--r--   0 shareit    (501) staff       (20)       38 2023-04-04 06:21:11.196426 apkupload-0.0.9/setup.cfg
+-rw-r--r--   0 shareit    (501) staff       (20)      670 2023-04-04 06:20:53.000000 apkupload-0.0.9/setup.py
```

### Comparing `apkupload-0.0.8/LICENSE` & `apkupload-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `apkupload-0.0.8/apkupload/upload.py` & `apkupload-0.0.9/apkupload/upload.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,16 +31,18 @@
 """
 
 
 def parse():
     p = configargparse.ArgParser(
         config_file_parser_class=configargparse.YAMLConfigFileParser)
     p.add('--config', required=True, is_config_file=True)
-    p.add('--version_code_prefix', required=True)
-    p.add('--version_name_list', required=True, nargs="+")
+    p.add('--version_code', required=True)
+    p.add('--version_code_suffix', required=True)
+    p.add('--version_name', required=True, nargs="+")
+    p.add('--delete', required=True)
     p.add('--send', required=True)
     p.add('--package', required=True)
     p.add('--name', required=True)
     p.add('--base', required=True)
     p.add('--input', required=True)
     p.add('--output', required=True)
     p.add('--key', required=True)
@@ -89,15 +91,14 @@
         headers=headers,
         json=body
     )
     print(r.status_code)
 
 
 def change_version(output, input, version_code, version_name):
-    os.system('rm -rf ' + output)
     os.system('rm -rf ' + input + "/build")
     result = ""
     print(">>>> change version <<<<")
     with open(input + "/apktool.yml", 'r') as f:
         lines = f.readlines()
         for line in lines[:-2]:
             result += line
@@ -160,19 +161,21 @@
         if (count < retry_count):
             url = upload(upload_url,file, count, retry_count)
     return url
 
 
 def main():
     args = parse()
-    version_code_prefix = args.version_code_prefix
-    version_name_list = args.version_name_list
+    version_code_suffix = args.version_code_suffix
+    version_name_list = args.version_name
+    version_code = args.version_code
     name = args.name
     base = args.base
     send = args.send
+    delete = args.delete
     input = args.input
     output = args.output
     key = args.key
     password = args.password
     secret = args.secret
     url = args.url
     upload_url = args.upload_url
@@ -188,28 +191,34 @@
     repository = args.repository
     image = args.image
     headers = {"Accept": "application/vnd.github.v3+json",
                "Authorization": f"token {github}"}
     retry_count = int(args.retry_count)
     apk_info = ""
     content = []
-    for version_name in version_name_list:
-        versoin_code = version_name.split("_")[0].split(".")[-1]
-        versoin_code = f"{version_code_prefix}{versoin_code}"
+    if (send == "True"):
+        print(f"删除{output}文件夹")
+        os.system('rm -rf ' + output)
+    for version_name in version_name_list: 
+        new_version_code = version_code       
+        if (version_code_suffix=="True"):
+            suffix = version_name.split("_")[0].split(".")[-1]
+            new_version_code = f"{version_code}{suffix}"
+        print(f"version_code = {new_version_code} version_name = {version_name}")
         path = datetime.now().strftime("%Y%m%d%H%M")
         apk = generate_apk_name(output, name, version_name)
-        change_version(output, input, versoin_code, version_name)
+        change_version(output, input, new_version_code, version_name)
         build_apk(output, input, apk, key, password)
         md5 = hashlib.md5(open(apk, 'rb').read()).hexdigest()
         size = str(os.path.getsize(apk))+"字节"
         download_url = upload(upload_url,apk, 0, retry_count)
         content.append(build_json(name,  version_name,
-                       versoin_code, md5, size,  changelog, base, path, download_url,package))
+                       new_version_code, md5, size,  changelog, base, path, download_url,package))
         apk_info += apk_info_template.format(name=name, download_url=download_url,
-                                             md5=md5, version_name=version_name, version_code=versoin_code, size=size)
+                                             md5=md5, version_name=version_name, version_code=new_version_code, size=size)
     build_web(user, repository, workflow, headers, content)
     if send == 'True':
         send_to_dingding(name, url, changelog, apk_info,
                          secret, token, at, image,package)
 
 
 if __name__ == "__main__":
```

### Comparing `apkupload-0.0.8/setup.py` & `apkupload-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="apkupload",
-    version="0.0.8",
+    version="0.0.9",
     author="malinkang",
     author_email="linkang.ma@gmail.com",
     description="apk 上传",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://malinkang.com",
     packages=setuptools.find_packages(),
```

