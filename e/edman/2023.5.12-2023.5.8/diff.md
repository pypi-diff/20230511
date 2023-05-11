# Comparing `tmp/edman-2023.5.12.tar.gz` & `tmp/edman-2023.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edman-2023.5.12.tar", last modified: Thu May 11 08:07:05 2023, max compression
+gzip compressed data, was "edman-2023.5.8.tar", last modified: Mon May  8 02:04:22 2023, max compression
```

## Comparing `edman-2023.5.12.tar` & `edman-2023.5.8.tar`

### file list

```diff
@@ -1,60 +1,30 @@
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-11 08:07:05.340586 edman-2023.5.12/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-11 08:07:05.330586 edman-2023.5.12/.github/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-11 08:07:05.330586 edman-2023.5.12/.github/workflows/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1379 2023-05-10 06:43:20.000000 edman-2023.5.12/.github/workflows/unittest.yml
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2266 2022-07-27 01:25:38.000000 edman-2023.5.12/.gitignore
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-11 08:07:05.330586 edman-2023.5.12/.idea/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      238 2022-04-13 07:00:02.000000 edman-2023.5.12/.idea/.gitignore
--rw-r--r--   0 ohno      (1000) ohno      (1000)      557 2023-04-10 07:58:11.000000 edman-2023.5.12/.idea/edman.iml
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-11 08:07:05.330586 edman-2023.5.12/.idea/inspectionProfiles/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      179 2022-04-13 07:00:02.000000 edman-2023.5.12/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      254 2023-04-10 07:58:11.000000 edman-2023.5.12/.idea/misc.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      269 2022-04-13 07:00:02.000000 edman-2023.5.12/.idea/modules.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      185 2022-04-13 07:00:02.000000 edman-2023.5.12/.idea/vcs.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-02-17 05:03:50.000000 edman-2023.5.12/LICENSE.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7613 2023-05-11 08:07:05.340586 edman-2023.5.12/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)     6049 2023-01-20 03:28:32.000000 edman-2023.5.12/README.rst
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-11 08:07:05.330586 edman-2023.5.12/edman/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      167 2023-05-09 07:38:50.000000 edman-2023.5.12/edman/__init__.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1373 2023-03-15 05:16:00.000000 edman-2023.5.12/edman/config.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    16457 2023-03-15 05:16:00.000000 edman-2023.5.12/edman/convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    47757 2023-04-05 05:00:36.000000 edman-2023.5.12/edman/db.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)      644 2022-04-13 07:00:02.000000 edman-2023.5.12/edman/exceptions.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    21859 2023-05-11 08:05:20.000000 edman-2023.5.12/edman/file.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1520 2023-03-09 05:51:32.000000 edman-2023.5.12/edman/json_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     9907 2023-04-10 07:58:11.000000 edman-2023.5.12/edman/search.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    10958 2023-03-09 05:51:32.000000 edman-2023.5.12/edman/utils.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-11 08:07:05.330586 edman-2023.5.12/edman.egg-info/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7613 2023-05-11 08:07:05.000000 edman-2023.5.12/edman.egg-info/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      971 2023-05-11 08:07:05.000000 edman-2023.5.12/edman.egg-info/SOURCES.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-05-11 08:07:05.000000 edman-2023.5.12/edman.egg-info/dependency_links.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       54 2023-05-11 08:07:05.000000 edman-2023.5.12/edman.egg-info/requires.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       34 2023-05-11 08:07:05.000000 edman-2023.5.12/edman.egg-info/top_level.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1069 2023-05-11 08:05:20.000000 edman-2023.5.12/pyproject.toml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      859 2023-05-10 06:13:28.000000 edman-2023.5.12/requirements.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2023-05-11 08:07:05.340586 edman-2023.5.12/setup.cfg
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-11 08:07:05.330586 edman-2023.5.12/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2022-04-13 07:00:02.000000 edman-2023.5.12/tests/__init__.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-11 08:07:05.330586 edman-2023.5.12/tests/ini/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      166 2022-11-15 02:42:20.000000 edman-2023.5.12/tests/ini/test_db.ini.sample
--rw-r--r--   0 ohno      (1000) ohno      (1000)    12303 2022-04-13 07:00:02.000000 edman-2023.5.12/tests/test_convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    86854 2023-04-20 03:03:49.000000 edman-2023.5.12/tests/test_db.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    37062 2023-05-11 08:05:20.000000 edman-2023.5.12/tests/test_file.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     5837 2023-03-09 05:51:32.000000 edman-2023.5.12/tests/test_multiuser.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    19062 2023-04-05 05:00:36.000000 edman-2023.5.12/tests/test_search.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7898 2022-04-13 07:00:02.000000 edman-2023.5.12/tests/test_utils.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-11 08:07:05.330586 edman-2023.5.12/venv/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-11 08:07:05.340586 edman-2023.5.12/venv/bin/
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1725 2023-04-07 00:37:51.000000 edman-2023.5.12/venv/bin/jp.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      632 2023-05-10 00:30:10.000000 edman-2023.5.12/venv/bin/rst2html.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      754 2023-05-10 00:30:10.000000 edman-2023.5.12/venv/bin/rst2html4.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1089 2023-05-10 00:30:10.000000 edman-2023.5.12/venv/bin/rst2html5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      831 2023-05-10 00:30:10.000000 edman-2023.5.12/venv/bin/rst2latex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      654 2023-05-10 00:30:10.000000 edman-2023.5.12/venv/bin/rst2man.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      820 2023-05-10 00:30:10.000000 edman-2023.5.12/venv/bin/rst2odt.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     2176 2023-05-10 00:30:10.000000 edman-2023.5.12/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      639 2023-05-10 00:30:10.000000 edman-2023.5.12/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      675 2023-05-10 00:30:10.000000 edman-2023.5.12/venv/bin/rst2s5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      911 2023-05-10 00:30:10.000000 edman-2023.5.12/venv/bin/rst2xetex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      640 2023-05-10 00:30:10.000000 edman-2023.5.12/venv/bin/rst2xml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      708 2023-05-10 00:30:10.000000 edman-2023.5.12/venv/bin/rstpep2html.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 02:04:22.028113 edman-2023.5.8/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-02-17 05:03:50.000000 edman-2023.5.8/LICENSE.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       19 2022-04-13 07:00:02.000000 edman-2023.5.8/MANIFEST.in
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6379 2023-05-08 02:04:22.028113 edman-2023.5.8/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6049 2023-01-20 03:28:32.000000 edman-2023.5.8/README.rst
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 02:04:22.028113 edman-2023.5.8/edman/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      167 2022-04-13 07:00:02.000000 edman-2023.5.8/edman/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1373 2023-03-15 05:16:00.000000 edman-2023.5.8/edman/config.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    16457 2023-03-15 05:16:00.000000 edman-2023.5.8/edman/convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    47757 2023-04-05 05:00:36.000000 edman-2023.5.8/edman/db.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      644 2022-04-13 07:00:02.000000 edman-2023.5.8/edman/exceptions.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    21800 2023-05-08 02:02:11.000000 edman-2023.5.8/edman/file.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1520 2023-03-09 05:51:32.000000 edman-2023.5.8/edman/json_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     9907 2023-04-10 07:58:11.000000 edman-2023.5.8/edman/search.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    10958 2023-03-09 05:51:32.000000 edman-2023.5.8/edman/utils.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 02:04:22.028113 edman-2023.5.8/edman.egg-info/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6379 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      470 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/SOURCES.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/dependency_links.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       54 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/requires.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        6 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/top_level.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      707 2023-05-08 02:04:22.028113 edman-2023.5.8/setup.cfg
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       41 2022-04-13 07:00:02.000000 edman-2023.5.8/setup.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 02:04:22.028113 edman-2023.5.8/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    12303 2022-04-13 07:00:02.000000 edman-2023.5.8/tests/test_convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    86854 2023-04-20 03:03:49.000000 edman-2023.5.8/tests/test_db.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    36850 2023-05-08 02:02:11.000000 edman-2023.5.8/tests/test_file.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     5837 2023-03-09 05:51:32.000000 edman-2023.5.8/tests/test_multiuser.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    19062 2023-04-05 05:00:36.000000 edman-2023.5.8/tests/test_search.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     7898 2022-04-13 07:00:02.000000 edman-2023.5.8/tests/test_utils.py
```

### Comparing `edman-2023.5.12/LICENSE.txt` & `edman-2023.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edman-2023.5.12/PKG-INFO` & `edman-2023.5.8/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 Metadata-Version: 2.1
 Name: edman
-Version: 2023.5.12
+Version: 2023.5.8
 Summary: KEK IMSS SBRC/PF Experimental Data Management System
-Author-email: Masaki Ohno <masakio@post.kek.jp>
+Home-page: https://github.com/ryde/edman
+Author: Masaki Ohno
+Author-email: masakio@post.kek.jp
 License: MIT License
-        
-        Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Yusuke Yamada, Masaki Ohno
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-Project-URL: documentation, https://ryde.github.io/edman/
-Project-URL: repository, https://github.com/ryde/edman
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 edman
 =====
```

### Comparing `edman-2023.5.12/README.rst` & `edman-2023.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `edman-2023.5.12/edman/config.py` & `edman-2023.5.8/edman/config.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.12/edman/convert.py` & `edman-2023.5.8/edman/convert.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.12/edman/db.py` & `edman-2023.5.8/edman/db.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.12/edman/exceptions.py` & `edman-2023.5.8/edman/exceptions.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.12/edman/file.py` & `edman-2023.5.8/edman/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,17 +219,17 @@
             results = []
             for file_oid in file_oid_list:
                 fs_out = self.fs.get(file_oid)
                 save_path = p / fs_out.filename
                 try:
                     with save_path.open('wb') as f:
                         tmp = fs_out.read()
-                        # if hasattr(fs_out,
-                        #            'compress') and fs_out.compress == 'gzip':
-                        #     tmp = gzip.decompress(tmp)
+                        if hasattr(fs_out,
+                                   'compress') and fs_out.compress == 'gzip':
+                            tmp = gzip.decompress(tmp)
                         f.write(tmp)
                         f.flush()
                         os.fsync(f.fileno())
                 except IOError:
                     raise
                 results.append(save_path.exists())
         return all(results)
@@ -239,15 +239,15 @@
                query=None) -> bool:
         """
         ドキュメントにファイルリファレンスを追加する
         ファイルのインサート処理、圧縮処理なども行う
         :param str collection:
         :param oid:
         :type oid: ObjectId or str
-        :param tuple file_path:ドキュメントに添付する単数or複数のファイルパス
+        :param tuple file_path:ドキュメントに添付する単数or複数のファイルパスと圧縮可否のタプル
         :param str structure:
         :param query:
         :type query: list or None
         :return:
         :rtype: bool
         """
 
@@ -283,33 +283,32 @@
         else:  # 差し替えができなかった時は添付ファイルは削除
             self.fs_delete(inserted_file_oids)
             return False
 
     def grid_in(self, files: Tuple[Tuple[Any, bool]]) -> list[Any]:
         """
         Gridfsへ複数のデータをアップロードし
+        compressに圧縮指定があればgzipで圧縮する
 
         :param tuple files:
         :return: inserted
         :rtype: list
         """
         inserted = []
         for file, compress in files:
             try:
                 with file.open('rb') as f:
                     fb = f.read()
-                    # if compress:
-                    #     fb = gzip.compress(fb, compresslevel=self.comp_level)
-                    #     compress = 'gzip'
-                    # else:
-                    #     compress = None
-                    # metadata = {'filename': os.path.basename(f.name),
-                    #             'compress': compress}
-                    metadata = {'filename': os.path.basename(f.name)}
-
+                    if compress:
+                        fb = gzip.compress(fb, compresslevel=self.comp_level)
+                        compress = 'gzip'
+                    else:
+                        compress = None
+                    metadata = {'filename': os.path.basename(f.name),
+                                'compress': compress}
             except (IOError, OSError) as e:
                 raise EdmanDbProcessError(e)
             try:
                 inserted.append(self.fs.put(fb, **metadata))
             except GridFSError as e:
                 raise EdmanDbProcessError(e)
         return inserted
@@ -417,19 +416,18 @@
                         content = self.fs.get(file_ref)
                     except NoFile:
                         raise EdmanDbProcessError('指定の関連ファイルが存在しません')
                     except GridFSError:
                         raise
                     else:
                         # 圧縮設定の場合はその拡張子を追加
-                        # if content.compress is not None:
-                        #     filename = content.name + '.' + content.compress
-                        # else:
-                        #     filename = content.name
-                        filename = content.name
+                        if content.compress is not None:
+                            filename = content.name + '.' + content.compress
+                        else:
+                            filename = content.name
                         filepath = os.path.join(dir_path, filename)
                     try:
                         with open(filepath, 'wb') as f:
                             f.write(content.read())
                     except (FileNotFoundError, IOError):
                         EdmanInternalError('ファイルを保存することが出来ませんでした')
                     except GridFSError:
```

### Comparing `edman-2023.5.12/edman/json_manager.py` & `edman-2023.5.8/edman/json_manager.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.12/edman/search.py` & `edman-2023.5.8/edman/search.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.12/edman/utils.py` & `edman-2023.5.8/edman/utils.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.12/edman.egg-info/PKG-INFO` & `edman-2023.5.8/edman.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 Metadata-Version: 2.1
 Name: edman
-Version: 2023.5.12
+Version: 2023.5.8
 Summary: KEK IMSS SBRC/PF Experimental Data Management System
-Author-email: Masaki Ohno <masakio@post.kek.jp>
+Home-page: https://github.com/ryde/edman
+Author: Masaki Ohno
+Author-email: masakio@post.kek.jp
 License: MIT License
-        
-        Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Yusuke Yamada, Masaki Ohno
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-Project-URL: documentation, https://ryde.github.io/edman/
-Project-URL: repository, https://github.com/ryde/edman
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 edman
 =====
```

### Comparing `edman-2023.5.12/tests/test_convert.py` & `edman-2023.5.8/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.12/tests/test_db.py` & `edman-2023.5.8/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.12/tests/test_file.py` & `edman-2023.5.8/tests/test_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -637,20 +637,18 @@
             # ファイル読み込み、ファイルをgridfsに入れる
             files_oid = []
             self.fs = gridfs.GridFS(self.testdb)
             test_vars = {}
             for filename in files:
                 with filename.open('rb') as f:
                     content = f.read()
-                    # file_obj = gzip.compress(content, compresslevel=6)
-                    # files_oid.append(
-                    #     self.fs.put(file_obj, filename=filename.name,
-                    #                 compress='gzip'))
+                    file_obj = gzip.compress(content, compresslevel=6)
                     files_oid.append(
-                        self.fs.put(content, filename=filename.name))
+                        self.fs.put(file_obj, filename=filename.name,
+                                    compress='gzip'))
                     test_vars.update({filename.name: content.decode()})
 
         with tempfile.TemporaryDirectory() as tmp_dl_dir:
             path = Path(tmp_dl_dir)
 
             grid_out_result = self.file._grid_out(files_oid, tmp_dl_dir)
             # 実行結果
@@ -887,31 +885,28 @@
         if not self.db_server_connect:
             return
 
         # 正常系
         with tempfile.TemporaryDirectory() as tmp_dir:
             sample_files = self.make_txt_files(tmp_dir, name='grid_in_test',
                                                qty=2)
-            compress_settings = [False, False]
+            compress_settings = [True, False]
             td = tuple(
                 [(p, b) for (p, b) in zip(sample_files, compress_settings)])
 
             self.fs = gridfs.GridFS(self.testdb)
             actual = []
             for oid in self.file.grid_in(td):
                 data = self.fs.get(oid)
-                # if data.compress == 'gzip':
-                #     f_data = gzip.decompress(data.read()).decode()
-                #     b_data = True
-                # else:
-                #     f_data = data.read().decode()
-                #     b_data = False
-
-                f_data = data.read().decode()
-                b_data = False
+                if data.compress == 'gzip':
+                    f_data = gzip.decompress(data.read()).decode()
+                    b_data = True
+                else:
+                    f_data = data.read().decode()
+                    b_data = False
                 actual.append([data.filename, f_data, b_data])
 
             expected = []
             for file_path, compress in zip(sample_files, compress_settings):
                 with file_path.open() as f:
                     expected.append([file_path.name, f.read(), compress])
```

### Comparing `edman-2023.5.12/tests/test_multiuser.py` & `edman-2023.5.8/tests/test_multiuser.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.12/tests/test_search.py` & `edman-2023.5.8/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.12/tests/test_utils.py` & `edman-2023.5.8/tests/test_utils.py`

 * *Files identical despite different names*

