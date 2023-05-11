# Comparing `tmp/magic-module-skaffolder-0.0.2.tar.gz` & `tmp/magic-module-skaffolder-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magic-module-skaffolder-0.0.2.tar", last modified: Wed May  3 08:46:31 2023, max compression
+gzip compressed data, was "magic-module-skaffolder-0.0.3.tar", last modified: Thu May 11 19:11:13 2023, max compression
```

## Comparing `magic-module-skaffolder-0.0.2.tar` & `magic-module-skaffolder-0.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:46:31.299054 magic-module-skaffolder-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:46:31.291053 magic-module-skaffolder-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:46:31.295054 magic-module-skaffolder-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:46:31.295054 magic-module-skaffolder-0.0.2/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/.idea/jpa-buddy.xml
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/.idea/magic-module-skaffolder.iml
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/.release
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-03 08:46:31.299054 magic-module-skaffolder-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-03 08:46:31.299054 magic-module-skaffolder-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:46:31.295054 magic-module-skaffolder-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:46:31.295054 magic-module-skaffolder-0.0.2/src/magic_module_skaffolder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/src/magic_module_skaffolder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/src/magic_module_skaffolder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/src/magic_module_skaffolder/api_descriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/src/magic_module_skaffolder/magic_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    15533 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/src/magic_module_skaffolder/skaffolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/src/magic_module_skaffolder/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:46:31.299054 magic-module-skaffolder-0.0.2/src/magic_module_skaffolder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-03 08:46:31.000000 magic-module-skaffolder-0.0.2/src/magic_module_skaffolder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-03 08:46:31.000000 magic-module-skaffolder-0.0.2/src/magic_module_skaffolder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 08:46:31.000000 magic-module-skaffolder-0.0.2/src/magic_module_skaffolder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-03 08:46:31.000000 magic-module-skaffolder-0.0.2/src/magic_module_skaffolder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 08:46:31.000000 magic-module-skaffolder-0.0.2/src/magic_module_skaffolder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 08:46:31.000000 magic-module-skaffolder-0.0.2/src/magic_module_skaffolder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 08:46:30.000000 magic-module-skaffolder-0.0.2/src/magic_module_skaffolder.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:46:31.295054 magic-module-skaffolder-0.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:46:31.295054 magic-module-skaffolder-0.0.2/tests/mmv1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:46:31.295054 magic-module-skaffolder-0.0.2/tests/mmv1/products/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:46:31.299054 magic-module-skaffolder-0.0.2/tests/mmv1/products/certificatemanager/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/tests/mmv1/products/certificatemanager/product.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:46:31.299054 magic-module-skaffolder-0.0.2/tests/mmv1/products/compute/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/tests/mmv1/products/compute/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    59948 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/tests/mmv1/products/compute/BackendService.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/tests/mmv1/products/compute/FirewallPolicy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/tests/mmv1/products/compute/product.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:46:31.299054 magic-module-skaffolder-0.0.2/tests/mmv1/products/networksecurity/
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/tests/mmv1/products/networksecurity/AdressGroup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/tests/mmv1/products/networksecurity/GatewaySecurityPolicies.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/tests/mmv1/products/networksecurity/GatewaySecurityPoliciesRules.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/tests/mmv1/products/networksecurity/UrlLists.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-03 08:46:06.000000 magic-module-skaffolder-0.0.2/tests/mmv1/products/networksecurity/product.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:11:13.004536 magic-module-skaffolder-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:11:12.996536 magic-module-skaffolder-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:11:13.000536 magic-module-skaffolder-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:11:13.000536 magic-module-skaffolder-0.0.3/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/.idea/jpa-buddy.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/.idea/magic-module-skaffolder.iml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/.release
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-11 19:11:13.004536 magic-module-skaffolder-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-11 19:11:13.004536 magic-module-skaffolder-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:11:12.996536 magic-module-skaffolder-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:11:13.000536 magic-module-skaffolder-0.0.3/src/magic_module_skaffolder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/src/magic_module_skaffolder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/src/magic_module_skaffolder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/src/magic_module_skaffolder/api_descriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/src/magic_module_skaffolder/magic_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/src/magic_module_skaffolder/skaffolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/src/magic_module_skaffolder/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:11:13.000536 magic-module-skaffolder-0.0.3/src/magic_module_skaffolder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-11 19:11:12.000000 magic-module-skaffolder-0.0.3/src/magic_module_skaffolder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-11 19:11:12.000000 magic-module-skaffolder-0.0.3/src/magic_module_skaffolder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:11:12.000000 magic-module-skaffolder-0.0.3/src/magic_module_skaffolder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 19:11:12.000000 magic-module-skaffolder-0.0.3/src/magic_module_skaffolder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-11 19:11:12.000000 magic-module-skaffolder-0.0.3/src/magic_module_skaffolder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-11 19:11:12.000000 magic-module-skaffolder-0.0.3/src/magic_module_skaffolder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:11:12.000000 magic-module-skaffolder-0.0.3/src/magic_module_skaffolder.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:11:12.996536 magic-module-skaffolder-0.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:11:12.996536 magic-module-skaffolder-0.0.3/tests/mmv1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:11:13.000536 magic-module-skaffolder-0.0.3/tests/mmv1/products/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:11:13.000536 magic-module-skaffolder-0.0.3/tests/mmv1/products/certificatemanager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/tests/mmv1/products/certificatemanager/product.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:11:13.000536 magic-module-skaffolder-0.0.3/tests/mmv1/products/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/tests/mmv1/products/compute/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    59948 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/tests/mmv1/products/compute/BackendService.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/tests/mmv1/products/compute/FirewallPolicy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/tests/mmv1/products/compute/product.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:11:13.004536 magic-module-skaffolder-0.0.3/tests/mmv1/products/networksecurity/
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/tests/mmv1/products/networksecurity/AdressGroup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/tests/mmv1/products/networksecurity/GatewaySecurityPolicies.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/tests/mmv1/products/networksecurity/GatewaySecurityPoliciesRules.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/tests/mmv1/products/networksecurity/UrlLists.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-11 19:10:55.000000 magic-module-skaffolder-0.0.3/tests/mmv1/products/networksecurity/product.yaml
```

### Comparing `magic-module-skaffolder-0.0.2/.github/workflows/python-publish.yml` & `magic-module-skaffolder-0.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `magic-module-skaffolder-0.0.2/.gitignore` & `magic-module-skaffolder-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `magic-module-skaffolder-0.0.2/.idea/magic-module-skaffolder.iml` & `magic-module-skaffolder-0.0.3/.idea/magic-module-skaffolder.iml`

 * *Files 10% similar despite different names*

#### Comparing `magic-module-skaffolder-0.0.2/.idea/magic-module-skaffolder.iml` & `magic-module-skaffolder-0.0.3/.idea/magic-module-skaffolder.iml`

```diff
@@ -1,12 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <module type="JAVA_MODULE" version="4">
   <component name="NewModuleRootManager" inherit-compiler-output="true">
     <exclude-output/>
     <content url="file://$MODULE_DIR$">
       <sourceFolder url="file://$MODULE_DIR$/src" isTestSource="false"/>
       <sourceFolder url="file://$MODULE_DIR$/tests" isTestSource="true"/>
+      <excludeFolder url="file://$MODULE_DIR$/build"/>
+      <excludeFolder url="file://$MODULE_DIR$/dist"/>
+      <excludeFolder url="file://$MODULE_DIR$/venv"/>
     </content>
     <orderEntry type="jdk" jdkName="Pipenv (magic-module-skaffolder)" jdkType="Python SDK"/>
     <orderEntry type="sourceFolder" forTests="false"/>
   </component>
 </module>
```

### Comparing `magic-module-skaffolder-0.0.2/PKG-INFO` & `magic-module-skaffolder-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-module-skaffolder
-Version: 0.0.2
+Version: 0.0.3
 Summary: generate and update Magic Module resource definitions
 Home-page: https://github.com/binxio/magic-module-skaffolder
 Author: Mark van Holsteijn
 Author-email: mark.vanholsteijn@xebia.com
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `magic-module-skaffolder-0.0.2/README.md` & `magic-module-skaffolder-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `magic-module-skaffolder-0.0.2/setup.cfg` & `magic-module-skaffolder-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = magic-module-skaffolder
-version = 0.0.2
+version = 0.0.3
 author = Mark van Holsteijn
 url = https://github.com/binxio/magic-module-skaffolder
 author_email = mark.vanholsteijn@xebia.com
 description = generate and update Magic Module resource definitions
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `magic-module-skaffolder-0.0.2/src/magic_module_skaffolder/api_descriptions.py` & `magic-module-skaffolder-0.0.3/src/magic_module_skaffolder/api_descriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,16 @@
             )
             if self.get("type", "") == "string"
             else None
         )
 
     @property
     def is_output_only(self) -> bool:
-        return "[output only]" in self.get("description", "").lower()
+        description = self.get("description", "").lower()
+        return description.startswith("output only") or "[output only]" in description
 
     @property
     def is_input_only(self) -> bool:
         return "@inputonly" in self.get("description", "").lower()
 
     @property
     def is_deprecated(self) -> bool:
```

### Comparing `magic-module-skaffolder-0.0.2/src/magic_module_skaffolder/magic_module.py` & `magic-module-skaffolder-0.0.3/src/magic_module_skaffolder/magic_module.py`

 * *Files identical despite different names*

### Comparing `magic-module-skaffolder-0.0.2/src/magic_module_skaffolder/skaffolder.py` & `magic-module-skaffolder-0.0.3/src/magic_module_skaffolder/skaffolder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os
+import sys
 import logging
 import re
 from pathlib import Path
 from typing import Optional, Dict, Any
 
 import click
 from pattern.text.en import singularize
@@ -96,14 +96,16 @@
                 result["type"] = target_type
             elif value_format == "byte" and name == "fingerprint":
                 result["type"] = "Api::Type::Fingerprint"
             elif "in RFC3339 text format" in description or (
                 name and "timestamp" in name.lower()
             ):
                 result["type"] = "Api::Type::Time"
+            elif name == "etag":
+                result["type"] = "Api::Type::Fingerprint"
             elif type_definition.is_resource_ref:
                 # see https://googlecloudplatform.github.io/magic-modules/docs/how-to/add-mmv1-resource/#resourceref
                 resource_reference = type_definition.is_resource_ref.group(1)
                 (
                     resource_reference_name,
                     resource_reference_type,
                 ) = resource_reference.split(".", 1)
@@ -188,24 +190,23 @@
             def _singular_snake_case(match: re.Match) -> str:
                 return "{{" + parameter_camel_case_to_snake_case(match.group(1)) + "}}"
 
             base_url = re.sub(r"{([^}]*)}", _singular_snake_case, base_url)
             result["base_url"] = base_url
 
         def add_self_link():
-            if "name" in type_definition.properties.keys():
-                result["self_link"] = result["base_url"] + "/{{name}}"
-
             if "self_link" in type_definition.properties.keys():
                 result["has_self_link"] = True
+            elif "name" in type_definition.properties.keys():
+                result["self_link"] = result["base_url"] + "/{{name}}"
 
         def add_update_verb():
             patch_method = resource_definition.methods.get("patch")
             if patch_method:
-                result["update_verb"] = "PATCH"
+                result["update_verb"] = ":PATCH"
                 if "updateMask" in patch_method.parameters:
                     result["update_mask"] = True
 
         def add_create_link():
             id_name = type_name[0].lower() + type_name[1:] + "Id"
             if (
                 id_name not in method.parameters
@@ -217,15 +218,15 @@
 
             query_parameters = {}
             parameters = []
             readable_name = parameter_camel_case_to_snake_case(type_name).replace(
                 "_", " "
             )
             for name, value in method.parameters.items():
-                if not value.get("required"):
+                if not value.is_required:
                     continue
 
                 if name == id_name:
                     parameter = self.create_magic_module_field(
                         api, "name", type_definition.properties["name"]
                     )
                     parameter[
@@ -233,15 +234,14 @@
                     ] = f"A user-defined name which uniquely identifies a {readable_name}."
                     parameter["url_param_only"] = True
                     parameters.append(parameter)
                     if value.get("location") == "query":
                         query_parameters[name] = "{{name}}"
                 elif name == "parent":
                     parameter = self.create_magic_module_field(api, "location", value)
-                    parameter["default"] = "global"
                     parameter["url_param_only"] = True
                     parameter["description"] = f"the location of the {readable_name}."
                     if value.get("location") == "query":
                         query_parameters[name] = "{{location}}"
 
                     parameters.append(parameter)
                 elif name == "updateMask":
@@ -253,15 +253,15 @@
                     if value.get("location") == "query":
                         query_parameters[name] = (
                             "{{" + parameter_camel_case_to_snake_case(name) + "}}"
                         )
                     parameters.append(parameter)
 
             if query_parameters:
-                result["create_link"] = (
+                result["create_url"] = (
                     result["base_url"]
                     + "/?"
                     + "&".join(
                         map(lambda q: f"{q[0]}={q[1]}", query_parameters.items())
                     )
                 )
             if parameters:
@@ -407,8 +407,8 @@
         defined = updater.create_magic_module_resource(api, resource_name, type_name)
         Resource.merge_resources(existing, defined, provider_version)
 
     if inplace:
         with open(resource_file, "w") as file:
             yaml.dump(existing, file)
     else:
-        yaml.dump(existing, os.stdout)
+        yaml.dump(existing, sys.stdout)
```

### Comparing `magic-module-skaffolder-0.0.2/src/magic_module_skaffolder.egg-info/PKG-INFO` & `magic-module-skaffolder-0.0.3/src/magic_module_skaffolder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-module-skaffolder
-Version: 0.0.2
+Version: 0.0.3
 Summary: generate and update Magic Module resource definitions
 Home-page: https://github.com/binxio/magic-module-skaffolder
 Author: Mark van Holsteijn
 Author-email: mark.vanholsteijn@xebia.com
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `magic-module-skaffolder-0.0.2/src/magic_module_skaffolder.egg-info/SOURCES.txt` & `magic-module-skaffolder-0.0.3/src/magic_module_skaffolder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magic-module-skaffolder-0.0.2/tests/mmv1/products/certificatemanager/product.yaml` & `magic-module-skaffolder-0.0.3/tests/mmv1/products/certificatemanager/product.yaml`

 * *Files identical despite different names*

### Comparing `magic-module-skaffolder-0.0.2/tests/mmv1/products/compute/BackendService.yaml` & `magic-module-skaffolder-0.0.3/tests/mmv1/products/compute/BackendService.yaml`

 * *Files identical despite different names*

### Comparing `magic-module-skaffolder-0.0.2/tests/mmv1/products/compute/FirewallPolicy.yaml` & `magic-module-skaffolder-0.0.3/tests/mmv1/products/compute/FirewallPolicy.yaml`

 * *Files identical despite different names*

### Comparing `magic-module-skaffolder-0.0.2/tests/mmv1/products/compute/product.yaml` & `magic-module-skaffolder-0.0.3/tests/mmv1/products/compute/product.yaml`

 * *Files identical despite different names*

### Comparing `magic-module-skaffolder-0.0.2/tests/mmv1/products/networksecurity/AdressGroup.yaml` & `magic-module-skaffolder-0.0.3/tests/mmv1/products/networksecurity/AdressGroup.yaml`

 * *Files identical despite different names*

### Comparing `magic-module-skaffolder-0.0.2/tests/mmv1/products/networksecurity/GatewaySecurityPolicies.yaml` & `magic-module-skaffolder-0.0.3/tests/mmv1/products/networksecurity/GatewaySecurityPolicies.yaml`

 * *Files identical despite different names*

### Comparing `magic-module-skaffolder-0.0.2/tests/mmv1/products/networksecurity/GatewaySecurityPoliciesRules.yaml` & `magic-module-skaffolder-0.0.3/tests/mmv1/products/networksecurity/GatewaySecurityPoliciesRules.yaml`

 * *Files identical despite different names*

### Comparing `magic-module-skaffolder-0.0.2/tests/mmv1/products/networksecurity/UrlLists.yaml` & `magic-module-skaffolder-0.0.3/tests/mmv1/products/networksecurity/UrlLists.yaml`

 * *Files identical despite different names*

### Comparing `magic-module-skaffolder-0.0.2/tests/mmv1/products/networksecurity/product.yaml` & `magic-module-skaffolder-0.0.3/tests/mmv1/products/networksecurity/product.yaml`

 * *Files identical despite different names*

