# Comparing `tmp/dqops-0.2.0.0.tar.gz` & `tmp/dqops-0.2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dqops-0.2.0.0.tar", last modified: Thu May 11 10:32:20 2023, max compression
+gzip compressed data, was "dqops-0.2.0.1.tar", last modified: Thu May 11 11:49:31 2023, max compression
```

## Comparing `dqops-0.2.0.0.tar` & `dqops-0.2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 10:32:20.859304 dqops-0.2.0.0/
--rw-rw-rw-   0        0        0    11554 2022-05-05 14:08:06.000000 dqops-0.2.0.0/LICENSE
--rw-rw-rw-   0        0        0     4822 2023-05-11 10:32:20.859304 dqops-0.2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3301 2023-05-11 10:17:32.000000 dqops-0.2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 10:32:20.744818 dqops-0.2.0.0/dqops/
--rw-rw-rw-   0        0        0      799 2023-05-11 10:17:32.000000 dqops-0.2.0.0/dqops/__init__.py
--rw-rw-rw-   0        0        0     3409 2023-05-11 10:17:32.000000 dqops-0.2.0.0/dqops/install.py
--rw-rw-rw-   0        0        0     2766 2023-05-11 10:17:32.000000 dqops-0.2.0.0/dqops/startdqo.py
--rw-rw-rw-   0        0        0      974 2023-05-11 10:30:46.000000 dqops-0.2.0.0/dqops/version.py
-drwxrwxrwx   0        0        0        0 2023-05-11 10:32:20.856045 dqops-0.2.0.0/dqops.egg-info/
--rw-rw-rw-   0        0        0     4822 2023-05-11 10:32:20.000000 dqops-0.2.0.0/dqops.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-05-11 10:32:20.000000 dqops-0.2.0.0/dqops.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 10:32:20.000000 dqops-0.2.0.0/dqops.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-11 10:32:20.000000 dqops-0.2.0.0/dqops.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-05-11 10:32:20.000000 dqops-0.2.0.0/dqops.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-11 10:32:20.000000 dqops-0.2.0.0/dqops.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      168 2022-05-05 14:08:06.000000 dqops-0.2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      118 2023-05-11 10:32:20.876887 dqops-0.2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     6154 2023-05-11 10:17:32.000000 dqops-0.2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:49:31.445331 dqops-0.2.0.1/
+-rw-rw-rw-   0        0        0    11554 2022-05-05 14:08:06.000000 dqops-0.2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     4822 2023-05-11 11:49:31.446476 dqops-0.2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3301 2023-05-11 10:17:32.000000 dqops-0.2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 11:49:31.378549 dqops-0.2.0.1/dqops/
+-rw-rw-rw-   0        0        0      799 2023-05-11 10:17:32.000000 dqops-0.2.0.1/dqops/__init__.py
+-rw-rw-rw-   0        0        0     3409 2023-05-11 10:17:32.000000 dqops-0.2.0.1/dqops/install.py
+-rw-rw-rw-   0        0        0     2923 2023-05-11 11:48:41.000000 dqops-0.2.0.1/dqops/startdqo.py
+-rw-rw-rw-   0        0        0      974 2023-05-11 11:48:41.000000 dqops-0.2.0.1/dqops/version.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:49:31.442850 dqops-0.2.0.1/dqops.egg-info/
+-rw-rw-rw-   0        0        0     4822 2023-05-11 11:49:31.000000 dqops-0.2.0.1/dqops.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-05-11 11:49:31.000000 dqops-0.2.0.1/dqops.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 11:49:31.000000 dqops-0.2.0.1/dqops.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-11 11:49:31.000000 dqops-0.2.0.1/dqops.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-05-11 11:49:31.000000 dqops-0.2.0.1/dqops.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-11 11:49:31.000000 dqops-0.2.0.1/dqops.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      168 2022-05-05 14:08:06.000000 dqops-0.2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      118 2023-05-11 11:49:31.460195 dqops-0.2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     6154 2023-05-11 10:17:32.000000 dqops-0.2.0.1/setup.py
```

### Comparing `dqops-0.2.0.0/LICENSE` & `dqops-0.2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dqops-0.2.0.0/PKG-INFO` & `dqops-0.2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqops
-Version: 0.2.0.0
+Version: 0.2.0.1
 Summary: DQO Data Quality Operations Center
 Home-page: https://github.com/dqops/dqo/tree/master/distribution/python
 Author: DQO Developers
 Author-email: support@dqo.ai
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dqops-0.2.0.0/README.md` & `dqops-0.2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dqops-0.2.0.0/dqops/__init__.py` & `dqops-0.2.0.1/dqops/__init__.py`

 * *Files identical despite different names*

### Comparing `dqops-0.2.0.0/dqops/install.py` & `dqops-0.2.0.1/dqops/install.py`

 * *Files identical despite different names*

### Comparing `dqops-0.2.0.0/dqops/startdqo.py` & `dqops-0.2.0.1/dqops/startdqo.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,17 @@
         install.install_dqo_home_if_missing(dqo_home)
 
     # TODO: detect if the user has Java 17 or newer on the JAVA_HOME, we can use it
     java_install_dir = os.path.join(module_dir, 'jre' + JAVA_VERSION)
     install.install_jre_if_missing(java_install_dir)
     java_home = os.path.join(java_install_dir, os.listdir(java_install_dir)[0])
 
+    if os.path.exists(os.path.join(java_home, 'Contents/Home')):
+        java_home = os.path.join(java_home, 'Contents/Home')  # support MacOS correctly
+
     os_platform = sys.platform.lower()[0:3]
     dqo_envs = os.environ.copy()
     dqo_envs['DQO_HOME'] = dqo_home
     dqo_envs['JAVA_HOME'] = java_home
     dqo_envs['DQO_PYTHON_INTERPRETER'] = sys.executable
 
     if os_platform == 'win':
```

### Comparing `dqops-0.2.0.0/dqops/version.py` & `dqops-0.2.0.1/dqops/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limit
 
 VERSION = "0.2.0-alpha0"
-PIP_VERSION = "0.2.0.0"
+PIP_VERSION = "0.2.0.1"
 GITHUB_RELEASE = "v" + VERSION + ""
 JAVA_VERSION = "17"
 
 
 def get_dqo_version():
     return VERSION, PIP_VERSION, GITHUB_RELEASE, JAVA_VERSION
```

### Comparing `dqops-0.2.0.0/dqops.egg-info/PKG-INFO` & `dqops-0.2.0.1/dqops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqops
-Version: 0.2.0.0
+Version: 0.2.0.1
 Summary: DQO Data Quality Operations Center
 Home-page: https://github.com/dqops/dqo/tree/master/distribution/python
 Author: DQO Developers
 Author-email: support@dqo.ai
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dqops-0.2.0.0/setup.py` & `dqops-0.2.0.1/setup.py`

 * *Files identical despite different names*

