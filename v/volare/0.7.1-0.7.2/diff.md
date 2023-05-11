# Comparing `tmp/volare-0.7.1.tar.gz` & `tmp/volare-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/volare-0.7.1.tar", last modified: Tue Mar 21 11:21:34 2023, max compression
+gzip compressed data, was "dist/volare-0.7.2.tar", last modified: Thu May 11 10:02:08 2023, max compression
```

## Comparing `volare-0.7.1.tar` & `volare-0.7.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-21 11:21:34.000000 volare-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (122)     8665 2023-03-21 11:21:34.000000 volare-0.7.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-21 11:21:34.000000 volare-0.7.1/volare/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-21 11:21:20.000000 volare-0.7.1/volare/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      671 2023-03-21 11:21:20.000000 volare-0.7.1/volare/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)      766 2023-03-21 11:21:20.000000 volare-0.7.1/volare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-03-21 11:21:20.000000 volare-0.7.1/volare/families.py
--rw-r--r--   0 runner    (1001) docker     (122)    13864 2023-03-21 11:21:20.000000 volare-0.7.1/volare/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-21 11:21:34.000000 volare-0.7.1/volare/build/
--rw-r--r--   0 runner    (1001) docker     (122)     7450 2023-03-21 11:21:20.000000 volare-0.7.1/volare/build/git_multi_clone.py
--rw-r--r--   0 runner    (1001) docker     (122)     4931 2023-03-21 11:21:20.000000 volare-0.7.1/volare/build/asap7.py
--rw-r--r--   0 runner    (1001) docker     (122)     5550 2023-03-21 11:21:20.000000 volare-0.7.1/volare/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13921 2023-03-21 11:21:20.000000 volare-0.7.1/volare/build/sky130.py
--rw-r--r--   0 runner    (1001) docker     (122)     3559 2023-03-21 11:21:20.000000 volare-0.7.1/volare/build/magic.py
--rw-r--r--   0 runner    (1001) docker     (122)     9202 2023-03-21 11:21:20.000000 volare-0.7.1/volare/build/gf180mcu.py
--rw-r--r--   0 runner    (1001) docker     (122)     3289 2023-03-21 11:21:20.000000 volare-0.7.1/volare/click_common.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1667 2023-03-21 11:21:20.000000 volare-0.7.1/volare/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7734 2023-03-21 11:21:20.000000 volare-0.7.1/volare/common.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      931 2023-03-21 11:21:20.000000 volare-0.7.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-21 11:21:34.000000 volare-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-21 11:21:34.000000 volare-0.7.1/volare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8665 2023-03-21 11:21:34.000000 volare-0.7.1/volare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-03-21 11:21:34.000000 volare-0.7.1/volare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-03-21 11:21:34.000000 volare-0.7.1/volare.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-21 11:21:34.000000 volare-0.7.1/volare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-03-21 11:21:34.000000 volare-0.7.1/volare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)      491 2023-03-21 11:21:34.000000 volare-0.7.1/volare.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:02:08.000000 volare-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 10:02:08.000000 volare-0.7.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)      931 2023-05-11 10:01:50.000000 volare-0.7.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8665 2023-05-11 10:02:08.000000 volare-0.7.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:02:08.000000 volare-0.7.2/volare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-11 10:02:08.000000 volare-0.7.2/volare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-11 10:02:08.000000 volare-0.7.2/volare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 10:02:08.000000 volare-0.7.2/volare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8665 2023-05-11 10:02:08.000000 volare-0.7.2/volare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-11 10:02:08.000000 volare-0.7.2/volare.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      491 2023-05-11 10:02:08.000000 volare-0.7.2/volare.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:02:08.000000 volare-0.7.2/volare/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:02:08.000000 volare-0.7.2/volare/build/
+-rw-r--r--   0 runner    (1001) docker     (122)     7450 2023-05-11 10:01:50.000000 volare-0.7.2/volare/build/git_multi_clone.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9219 2023-05-11 10:01:50.000000 volare-0.7.2/volare/build/gf180mcu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4931 2023-05-11 10:01:50.000000 volare-0.7.2/volare/build/asap7.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13938 2023-05-11 10:01:50.000000 volare-0.7.2/volare/build/sky130.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3559 2023-05-11 10:01:50.000000 volare-0.7.2/volare/build/magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5550 2023-05-11 10:01:50.000000 volare-0.7.2/volare/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-05-11 10:01:50.000000 volare-0.7.2/volare/families.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13864 2023-05-11 10:01:50.000000 volare-0.7.2/volare/manage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      671 2023-05-11 10:01:50.000000 volare-0.7.2/volare/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 10:01:50.000000 volare-0.7.2/volare/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     7734 2023-05-11 10:01:50.000000 volare-0.7.2/volare/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3289 2023-05-11 10:01:50.000000 volare-0.7.2/volare/click_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1667 2023-05-11 10:01:50.000000 volare-0.7.2/volare/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-05-11 10:01:50.000000 volare-0.7.2/volare/__init__.py
```

### Comparing `volare-0.7.1/PKG-INFO` & `volare-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volare
-Version: 0.7.1
+Version: 0.7.2
 Summary: An open_pdks PDK builder/version manager
 Home-page: UNKNOWN
 Author: Efabless Corporation
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: <h1 align="center">⛰️ Volare</h1>
         <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: volare Version: 0.7.1 Summary: An open_pdks PDK
+Metadata-Version: 2.1 Name: volare Version: 0.7.2 Summary: An open_pdks PDK
 builder/version manager Home-page: UNKNOWN Author: Efabless Corporation Author-
 email: donn@efabless.com License: UNKNOWN Description:
                           ****** â°ï¸ Volare ******
   [License:_Apache_2.0] [CI Status] [Invite_to_the_Skywater_PDK_Slack] [Code
                                  Style:_Black]
 Volare is a version manager (and builder) for builds of Google_open-source_PDKs
                                using open_pdks.
```

### Comparing `volare-0.7.1/volare/__version__.py` & `volare-0.7.2/volare/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.7.1"
+__version__ = "0.7.2"
 
 if __name__ == "__main__":
     print(__version__, end="")
```

### Comparing `volare-0.7.1/volare/__init__.py` & `volare-0.7.2/volare/__init__.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.1/volare/families.py` & `volare-0.7.2/volare/families.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.1/volare/manage.py` & `volare-0.7.2/volare/manage.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.1/volare/build/git_multi_clone.py` & `volare-0.7.2/volare/build/git_multi_clone.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.1/volare/build/asap7.py` & `volare-0.7.2/volare/build/asap7.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.1/volare/build/__init__.py` & `volare-0.7.2/volare/build/__init__.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.1/volare/build/sky130.py` & `volare-0.7.2/volare/build/sky130.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,15 +289,15 @@
         magic_dirname = os.path.dirname(magic_bin)
 
         with console.status("Configuring open_pdks…"):
             run_sh(
                 f"""
                     set -e
                     export PATH="{magic_dirname}:$PATH"
-                    ./configure --enable-sky130-pdk={sky130_path}/libraries {sram_opt}
+                    ./configure --enable-sky130-pdk={sky130_path}/libraries {sram_opt} --with-reference
                 """,
                 log_to=os.path.join(log_dir, "config.log"),
             )
         console.log("Configured open_pdks.")
 
         with console.status("Building variants using open_pdks…"):
             run_sh(
```

### Comparing `volare-0.7.1/volare/build/magic.py` & `volare-0.7.2/volare/build/magic.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.1/volare/build/gf180mcu.py` & `volare-0.7.2/volare/build/gf180mcu.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         magic_dirname = os.path.dirname(magic_bin)
 
         with console.status("Configuring open_pdks…"):
             run_sh(
                 f"""
                     set -e
                     export PATH="{magic_dirname}:$PATH"
-                    ./configure --enable-gf180mcu-pdk {' '.join(library_flags)}
+                    ./configure --enable-gf180mcu-pdk {' '.join(library_flags)} --with-reference
                 """,
                 log_to=os.path.join(log_dir, "config.log"),
             )
         console.log("Configured open_pdks.")
 
         with console.status("Building variants using open_pdks…"):
             run_sh(
```

### Comparing `volare-0.7.1/volare/click_common.py` & `volare-0.7.2/volare/click_common.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.1/volare/__main__.py` & `volare-0.7.2/volare/__main__.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.1/volare/common.py` & `volare-0.7.2/volare/common.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.1/setup.py` & `volare-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.1/volare.egg-info/PKG-INFO` & `volare-0.7.2/volare.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volare
-Version: 0.7.1
+Version: 0.7.2
 Summary: An open_pdks PDK builder/version manager
 Home-page: UNKNOWN
 Author: Efabless Corporation
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: <h1 align="center">⛰️ Volare</h1>
         <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: volare Version: 0.7.1 Summary: An open_pdks PDK
+Metadata-Version: 2.1 Name: volare Version: 0.7.2 Summary: An open_pdks PDK
 builder/version manager Home-page: UNKNOWN Author: Efabless Corporation Author-
 email: donn@efabless.com License: UNKNOWN Description:
                           ****** â°ï¸ Volare ******
   [License:_Apache_2.0] [CI Status] [Invite_to_the_Skywater_PDK_Slack] [Code
                                  Style:_Black]
 Volare is a version manager (and builder) for builds of Google_open-source_PDKs
                                using open_pdks.
```

