# Comparing `tmp/teko-cli-0.9.5.tar.gz` & `tmp/teko-cli-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/teko-cli-0.9.5.tar", last modified: Fri Jan  8 04:36:01 2021, max compression
+gzip compressed data, was "dist/teko-cli-0.9.6.tar", last modified: Wed Jan 20 04:27:10 2021, max compression
```

## Comparing `teko-cli-0.9.5.tar` & `teko-cli-0.9.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2021-01-08 04:36:01.981826 teko-cli-0.9.5/
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)       24 2020-12-08 08:11:12.000000 teko-cli-0.9.5/MANIFEST.in
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)    11831 2021-01-08 04:36:01.970788 teko-cli-0.9.5/PKG-INFO
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)     8848 2020-12-11 09:48:07.000000 teko-cli-0.9.5/README.md
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)       38 2021-01-08 04:36:01.982799 teko-cli-0.9.5/setup.cfg
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)     1080 2021-01-08 04:35:22.000000 teko-cli-0.9.5/setup.py
-drwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2021-01-08 04:36:01.381565 teko-cli-0.9.5/teko/
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2020-12-08 08:09:33.000000 teko-cli-0.9.5/teko/__init__.py
-drwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2021-01-08 04:36:01.476191 teko-cli-0.9.5/teko/cli/
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2020-10-29 07:05:32.000000 teko-cli-0.9.5/teko/cli/__init__.py
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)      266 2020-12-08 08:17:55.000000 teko-cli-0.9.5/teko/cli/cs_command.py
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)      812 2020-12-11 03:59:04.000000 teko-cli-0.9.5/teko/cli/jira_command.py
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)      215 2020-12-08 08:19:14.000000 teko-cli-0.9.5/teko/cli/main.py
-drwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2021-01-08 04:36:01.543785 teko-cli-0.9.5/teko/helpers/
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2020-12-09 08:12:34.000000 teko-cli-0.9.5/teko/helpers/__init__.py
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)     1950 2021-01-08 04:35:13.000000 teko-cli-0.9.5/teko/helpers/clog.py
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)       49 2020-12-11 09:06:49.000000 teko-cli-0.9.5/teko/helpers/exceptions.py
-drwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2021-01-08 04:36:01.596785 teko-cli-0.9.5/teko/models/
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2020-12-09 08:15:20.000000 teko-cli-0.9.5/teko/models/__init__.py
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)     1673 2021-01-08 04:35:13.000000 teko-cli-0.9.5/teko/models/jira_testcase.py
-drwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2021-01-08 04:36:01.620787 teko-cli-0.9.5/teko/services/
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2020-12-08 08:19:46.000000 teko-cli-0.9.5/teko/services/__init__.py
-drwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2021-01-08 04:36:01.669787 teko-cli-0.9.5/teko/services/jira/
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2020-12-08 08:19:50.000000 teko-cli-0.9.5/teko/services/jira/__init__.py
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)    21533 2021-01-08 04:35:13.000000 teko-cli-0.9.5/teko/services/jira/jira_service.py
-drwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2021-01-08 04:36:01.832806 teko-cli-0.9.5/teko/templates/
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)      513 2020-12-11 04:01:11.000000 teko-cli-0.9.5/teko/templates/cycle.json
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)      561 2020-12-25 03:56:38.000000 teko-cli-0.9.5/teko/templates/cycle.yaml
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)      944 2020-12-25 03:27:36.000000 teko-cli-0.9.5/teko/templates/testcases.json
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)     1053 2020-12-25 06:40:25.000000 teko-cli-0.9.5/teko/templates/testcases.yaml
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)     1346 2020-12-11 04:01:39.000000 teko-cli-0.9.5/teko/templates/testcases_with_cycle_bundle.json
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)     1470 2020-12-25 09:12:01.000000 teko-cli-0.9.5/teko/templates/testcases_with_cycle_bundle.yaml
-drwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2021-01-08 04:36:01.951785 teko-cli-0.9.5/teko_cli.egg-info/
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)    11831 2021-01-08 04:36:00.000000 teko-cli-0.9.5/teko_cli.egg-info/PKG-INFO
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)      753 2021-01-08 04:36:01.000000 teko-cli-0.9.5/teko_cli.egg-info/SOURCES.txt
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        1 2021-01-08 04:36:00.000000 teko-cli-0.9.5/teko_cli.egg-info/dependency_links.txt
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)       62 2021-01-08 04:36:00.000000 teko-cli-0.9.5/teko_cli.egg-info/entry_points.txt
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)       77 2021-01-08 04:36:00.000000 teko-cli-0.9.5/teko_cli.egg-info/requires.txt
--rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        5 2021-01-08 04:36:00.000000 teko-cli-0.9.5/teko_cli.egg-info/top_level.txt
+drwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2021-01-20 04:27:10.096570 teko-cli-0.9.6/
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)       24 2020-12-08 08:11:12.000000 teko-cli-0.9.6/MANIFEST.in
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)    11910 2021-01-20 04:27:10.081516 teko-cli-0.9.6/PKG-INFO
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)     8848 2020-12-11 09:48:07.000000 teko-cli-0.9.6/README.md
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)       38 2021-01-20 04:27:10.097552 teko-cli-0.9.6/setup.cfg
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)     1080 2021-01-20 04:26:14.000000 teko-cli-0.9.6/setup.py
+drwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2021-01-20 04:27:09.458592 teko-cli-0.9.6/teko/
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2020-12-08 08:09:33.000000 teko-cli-0.9.6/teko/__init__.py
+drwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2021-01-20 04:27:09.549703 teko-cli-0.9.6/teko/cli/
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2020-10-29 07:05:32.000000 teko-cli-0.9.6/teko/cli/__init__.py
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)      266 2020-12-08 08:17:55.000000 teko-cli-0.9.6/teko/cli/cs_command.py
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)      812 2020-12-11 03:59:04.000000 teko-cli-0.9.6/teko/cli/jira_command.py
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)      215 2020-12-08 08:19:14.000000 teko-cli-0.9.6/teko/cli/main.py
+drwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2021-01-20 04:27:09.620720 teko-cli-0.9.6/teko/helpers/
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2020-12-09 08:12:34.000000 teko-cli-0.9.6/teko/helpers/__init__.py
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)     1950 2021-01-08 04:35:13.000000 teko-cli-0.9.6/teko/helpers/clog.py
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)       49 2020-12-11 09:06:49.000000 teko-cli-0.9.6/teko/helpers/exceptions.py
+drwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2021-01-20 04:27:09.668254 teko-cli-0.9.6/teko/models/
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2020-12-09 08:15:20.000000 teko-cli-0.9.6/teko/models/__init__.py
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)     1673 2021-01-08 04:35:13.000000 teko-cli-0.9.6/teko/models/jira_testcase.py
+drwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2021-01-20 04:27:09.691884 teko-cli-0.9.6/teko/services/
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2020-12-08 08:19:46.000000 teko-cli-0.9.6/teko/services/__init__.py
+drwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2021-01-20 04:27:09.746891 teko-cli-0.9.6/teko/services/jira/
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2020-12-08 08:19:50.000000 teko-cli-0.9.6/teko/services/jira/__init__.py
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)    21532 2021-01-20 04:24:52.000000 teko-cli-0.9.6/teko/services/jira/jira_service.py
+drwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2021-01-20 04:27:09.925564 teko-cli-0.9.6/teko/templates/
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)      513 2020-12-11 04:01:11.000000 teko-cli-0.9.6/teko/templates/cycle.json
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)      561 2020-12-25 03:56:38.000000 teko-cli-0.9.6/teko/templates/cycle.yaml
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)      944 2020-12-25 03:27:36.000000 teko-cli-0.9.6/teko/templates/testcases.json
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)     1053 2020-12-25 06:40:25.000000 teko-cli-0.9.6/teko/templates/testcases.yaml
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)     1346 2020-12-11 04:01:39.000000 teko-cli-0.9.6/teko/templates/testcases_with_cycle_bundle.json
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)     1470 2020-12-25 09:12:01.000000 teko-cli-0.9.6/teko/templates/testcases_with_cycle_bundle.yaml
+drwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        0 2021-01-20 04:27:10.059993 teko-cli-0.9.6/teko_cli.egg-info/
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)    11910 2021-01-20 04:27:08.000000 teko-cli-0.9.6/teko_cli.egg-info/PKG-INFO
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)      753 2021-01-20 04:27:09.000000 teko-cli-0.9.6/teko_cli.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        1 2021-01-20 04:27:08.000000 teko-cli-0.9.6/teko_cli.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)       62 2021-01-20 04:27:08.000000 teko-cli-0.9.6/teko_cli.egg-info/entry_points.txt
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)       77 2021-01-20 04:27:08.000000 teko-cli-0.9.6/teko_cli.egg-info/requires.txt
+-rwxrwxrwx   0 thucnguyen  (1000) thucnguyen  (1000)        5 2021-01-20 04:27:08.000000 teko-cli-0.9.6/teko_cli.egg-info/top_level.txt
```

### Comparing `teko-cli-0.9.5/PKG-INFO` & `teko-cli-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teko-cli
-Version: 0.9.5
+Version: 0.9.6
 Summary: Teko CLI tools
 Home-page: https://git.teko.vn/vnpay-marketing-portal/teko-tools
 Author: Thuc Nguyen
 Author-email: thuc.nc@teko.vn
 License: MIT
 Download-URL: https://pypi.org/project/teko/
 Description: # Teko CLI Tools
@@ -339,14 +339,18 @@
             "testrun_date": "2020-12-12T14:54:00Z"
           }
         ]
         ```
         
         # Change log
         
+        ## \[0.9.6\] - 2021-01-20
+        ### Fix 
+        - Fix typo
+        
         ## \[0.9.5\] - 2021-01-08
         ### Add 
         - Add confluence link and some refactoring
         
         ## \[0.1.0\] - 2020-12-08
         ### Add
         - Initiate
```

### Comparing `teko-cli-0.9.5/README.md` & `teko-cli-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `teko-cli-0.9.5/setup.py` & `teko-cli-0.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='teko-cli',
-    version='0.9.5',
+    version='0.9.6',
     description='Teko CLI tools',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(exclude=('tests', )),
     include_package_data=True,
     author='Thuc Nguyen',
```

### Comparing `teko-cli-0.9.5/teko/cli/jira_command.py` & `teko-cli-0.9.6/teko/cli/jira_command.py`

 * *Files identical despite different names*

### Comparing `teko-cli-0.9.5/teko/helpers/clog.py` & `teko-cli-0.9.6/teko/helpers/clog.py`

 * *Files identical despite different names*

### Comparing `teko-cli-0.9.5/teko/models/jira_testcase.py` & `teko-cli-0.9.6/teko/models/jira_testcase.py`

 * *Files identical despite different names*

### Comparing `teko-cli-0.9.5/teko/services/jira/jira_service.py` & `teko-cli-0.9.6/teko/services/jira/jira_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
         load_dotenv()
         self.project_key = config.get('project_key') or os.getenv('JIRA_PROJECT_KEY')
         server = config.get('server') or os.getenv('JIRA_SERVER')
         jira_username = config.get('jira_username') or os.getenv('JIRA_USERNAME')
         jira_password = config.get('jira_password') or os.getenv('JIRA_PASSWORD')
         confluence_username = config.get('confluence_username') or os.getenv('CONFLUENCE_USERNAME')
-        confluence_password = config.get('confluence_password') or os.getenv('CONFLUENCE_PASSWOPRD')
+        confluence_password = config.get('confluence_password') or os.getenv('CONFLUENCE_PASSWORD')
 
         if not self.project_key or not server or not jira_username or not jira_password or not confluence_username or not confluence_password:
             msg = "No valid JIRA configuration found, please set JIRA_SERVER, JIRA_PROJECT_KEY, JIRA_USERNAME, " \
                   "JIRA_PASSWORD, CONFLUENCE_USERNAME and CONFLUENCE_PASSWORD environment variables first."
             CLog.error(msg)
             raise TekoJiraException(msg)
```

### Comparing `teko-cli-0.9.5/teko/templates/cycle.json` & `teko-cli-0.9.6/teko/templates/cycle.json`

 * *Files identical despite different names*

### Comparing `teko-cli-0.9.5/teko/templates/cycle.yaml` & `teko-cli-0.9.6/teko/templates/cycle.yaml`

 * *Files identical despite different names*

### Comparing `teko-cli-0.9.5/teko/templates/testcases.json` & `teko-cli-0.9.6/teko/templates/testcases.json`

 * *Files identical despite different names*

### Comparing `teko-cli-0.9.5/teko/templates/testcases.yaml` & `teko-cli-0.9.6/teko/templates/testcases.yaml`

 * *Files identical despite different names*

### Comparing `teko-cli-0.9.5/teko/templates/testcases_with_cycle_bundle.json` & `teko-cli-0.9.6/teko/templates/testcases_with_cycle_bundle.json`

 * *Files identical despite different names*

### Comparing `teko-cli-0.9.5/teko/templates/testcases_with_cycle_bundle.yaml` & `teko-cli-0.9.6/teko/templates/testcases_with_cycle_bundle.yaml`

 * *Files identical despite different names*

### Comparing `teko-cli-0.9.5/teko_cli.egg-info/PKG-INFO` & `teko-cli-0.9.6/teko_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teko-cli
-Version: 0.9.5
+Version: 0.9.6
 Summary: Teko CLI tools
 Home-page: https://git.teko.vn/vnpay-marketing-portal/teko-tools
 Author: Thuc Nguyen
 Author-email: thuc.nc@teko.vn
 License: MIT
 Download-URL: https://pypi.org/project/teko/
 Description: # Teko CLI Tools
@@ -339,14 +339,18 @@
             "testrun_date": "2020-12-12T14:54:00Z"
           }
         ]
         ```
         
         # Change log
         
+        ## \[0.9.6\] - 2021-01-20
+        ### Fix 
+        - Fix typo
+        
         ## \[0.9.5\] - 2021-01-08
         ### Add 
         - Add confluence link and some refactoring
         
         ## \[0.1.0\] - 2020-12-08
         ### Add
         - Initiate
```

### Comparing `teko-cli-0.9.5/teko_cli.egg-info/SOURCES.txt` & `teko-cli-0.9.6/teko_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

