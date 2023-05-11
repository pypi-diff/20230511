# Comparing `tmp/neon-tts-plugin-coqui-0.7.2a3.tar.gz` & `tmp/neon-tts-plugin-coqui-0.7.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-tts-plugin-coqui-0.7.2a3.tar", last modified: Tue Feb 14 18:17:39 2023, max compression
+gzip compressed data, was "neon-tts-plugin-coqui-0.7.3a0.tar", last modified: Thu May 11 00:43:13 2023, max compression
```

## Comparing `neon-tts-plugin-coqui-0.7.2a3.tar` & `neon-tts-plugin-coqui-0.7.3a0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 18:17:39.070542 neon-tts-plugin-coqui-0.7.2a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-02-14 18:17:31.000000 neon-tts-plugin-coqui-0.7.2a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-02-14 18:17:39.070542 neon-tts-plugin-coqui-0.7.2a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-02-14 18:17:31.000000 neon-tts-plugin-coqui-0.7.2a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 18:17:39.070542 neon-tts-plugin-coqui-0.7.2a3/neon_tts_plugin_coqui/
--rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-02-14 18:17:31.000000 neon-tts-plugin-coqui-0.7.2a3/neon_tts_plugin_coqui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-02-14 18:17:31.000000 neon-tts-plugin-coqui-0.7.2a3/neon_tts_plugin_coqui/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 18:17:39.070542 neon-tts-plugin-coqui-0.7.2a3/neon_tts_plugin_coqui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-02-14 18:17:38.000000 neon-tts-plugin-coqui-0.7.2a3/neon_tts_plugin_coqui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-02-14 18:17:39.000000 neon-tts-plugin-coqui-0.7.2a3/neon_tts_plugin_coqui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 18:17:38.000000 neon-tts-plugin-coqui-0.7.2a3/neon_tts_plugin_coqui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-14 18:17:38.000000 neon-tts-plugin-coqui-0.7.2a3/neon_tts_plugin_coqui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-14 18:17:38.000000 neon-tts-plugin-coqui-0.7.2a3/neon_tts_plugin_coqui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-14 18:17:38.000000 neon-tts-plugin-coqui-0.7.2a3/neon_tts_plugin_coqui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 18:17:38.000000 neon-tts-plugin-coqui-0.7.2a3/neon_tts_plugin_coqui.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 18:17:39.070542 neon-tts-plugin-coqui-0.7.2a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-02-14 18:17:31.000000 neon-tts-plugin-coqui-0.7.2a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:43:13.699954 neon-tts-plugin-coqui-0.7.3a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-11 00:43:09.000000 neon-tts-plugin-coqui-0.7.3a0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-11 00:43:13.699954 neon-tts-plugin-coqui-0.7.3a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-11 00:43:09.000000 neon-tts-plugin-coqui-0.7.3a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:43:13.699954 neon-tts-plugin-coqui-0.7.3a0/neon_tts_plugin_coqui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-05-11 00:43:09.000000 neon-tts-plugin-coqui-0.7.3a0/neon_tts_plugin_coqui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-05-11 00:43:09.000000 neon-tts-plugin-coqui-0.7.3a0/neon_tts_plugin_coqui/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:43:13.699954 neon-tts-plugin-coqui-0.7.3a0/neon_tts_plugin_coqui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-11 00:43:13.000000 neon-tts-plugin-coqui-0.7.3a0/neon_tts_plugin_coqui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-11 00:43:13.000000 neon-tts-plugin-coqui-0.7.3a0/neon_tts_plugin_coqui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 00:43:13.000000 neon-tts-plugin-coqui-0.7.3a0/neon_tts_plugin_coqui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-11 00:43:13.000000 neon-tts-plugin-coqui-0.7.3a0/neon_tts_plugin_coqui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-11 00:43:13.000000 neon-tts-plugin-coqui-0.7.3a0/neon_tts_plugin_coqui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-11 00:43:13.000000 neon-tts-plugin-coqui-0.7.3a0/neon_tts_plugin_coqui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 00:43:13.000000 neon-tts-plugin-coqui-0.7.3a0/neon_tts_plugin_coqui.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 00:43:13.699954 neon-tts-plugin-coqui-0.7.3a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-11 00:43:09.000000 neon-tts-plugin-coqui-0.7.3a0/setup.py
```

### Comparing `neon-tts-plugin-coqui-0.7.2a3/LICENSE.md` & `neon-tts-plugin-coqui-0.7.3a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-0.7.2a3/PKG-INFO` & `neon-tts-plugin-coqui-0.7.3a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-tts-plugin-coqui
-Version: 0.7.2a3
+Version: 0.7.3a0
 Summary: A Coqui AI TTS plugin for Neon
 Home-page: https://github.com/NeonGeckoCom/neon-tts-plugin-coqui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3.0
 Description: # NeonAI Coqui AI TTS Plugin
         [Mycroft](https://mycroft-ai.gitbook.io/docs/mycroft-technologies/mycroft-core/plugins) compatible
@@ -74,7 +74,8 @@
         
 Keywords: mycroft plugin tts
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+Provides-Extra: docker
```

### Comparing `neon-tts-plugin-coqui-0.7.2a3/README.md` & `neon-tts-plugin-coqui-0.7.3a0/README.md`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-0.7.2a3/neon_tts_plugin_coqui/__init__.py` & `neon-tts-plugin-coqui-0.7.3a0/neon_tts_plugin_coqui/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-0.7.2a3/neon_tts_plugin_coqui/configs.py` & `neon-tts-plugin-coqui-0.7.3a0/neon_tts_plugin_coqui/configs.py`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-0.7.2a3/neon_tts_plugin_coqui.egg-info/PKG-INFO` & `neon-tts-plugin-coqui-0.7.3a0/neon_tts_plugin_coqui.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-tts-plugin-coqui
-Version: 0.7.2a3
+Version: 0.7.3a0
 Summary: A Coqui AI TTS plugin for Neon
 Home-page: https://github.com/NeonGeckoCom/neon-tts-plugin-coqui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3.0
 Description: # NeonAI Coqui AI TTS Plugin
         [Mycroft](https://mycroft-ai.gitbook.io/docs/mycroft-technologies/mycroft-core/plugins) compatible
@@ -74,7 +74,8 @@
         
 Keywords: mycroft plugin tts
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+Provides-Extra: docker
```

### Comparing `neon-tts-plugin-coqui-0.7.2a3/setup.py` & `neon-tts-plugin-coqui-0.7.3a0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,27 +27,31 @@
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from setuptools import setup, find_packages
 from os import path, getenv
 
 
 def get_requirements(requirements_filename: str):
-    requirements_file = path.join(path.abspath(path.dirname(__file__)), "requirements", requirements_filename)
+    requirements_file = path.join(path.abspath(path.dirname(__file__)),
+                                  "requirements", requirements_filename)
     with open(requirements_file, 'r', encoding='utf-8') as r:
         requirements = r.readlines()
-    requirements = [r.strip() for r in requirements if r.strip() and not r.strip().startswith("#")]
+    requirements = [r.strip() for r in requirements if r.strip() and not
+                    r.strip().startswith("#")]
 
     for i in range(0, len(requirements)):
         r = requirements[i]
         if "@" in r:
-            parts = [p.lower() if p.strip().startswith("git+http") else p for p in r.split('@')]
+            parts = [p.lower() if p.strip().startswith("git+http") else p
+                     for p in r.split('@')]
             r = "@".join(parts)
             if getenv("GITHUB_TOKEN"):
                 if "github.com" in r:
-                    r = r.replace("github.com", f"{getenv('GITHUB_TOKEN')}@github.com")
+                    r = r.replace("github.com",
+                                  f"{getenv('GITHUB_TOKEN')}@github.com")
             requirements[i] = r
     return requirements
 
 
 PLUGIN_ENTRY_POINT = 'coqui = neon_tts_plugin_coqui:CoquiTTS'
 CONFIG_ENTRY_POINT = 'coqui.config = neon_tts_plugin_coqui.configs:tts_config'
 
@@ -70,14 +74,15 @@
     long_description_content_type='text/markdown',
     url='https://github.com/NeonGeckoCom/neon-tts-plugin-coqui',
     author='Neongecko',
     author_email='developers@neon.ai',
     license='BSD-3.0',
     packages=find_packages(),
     install_requires=get_requirements("requirements.txt"),
+    extras_require={"docker": get_requirements("docker.txt")},
     zip_safe=True,
     classifiers=[
         'Intended Audience :: Developers',
         'Topic :: Text Processing :: Linguistic',
 
         'Programming Language :: Python :: 3.6',
     ],
```

