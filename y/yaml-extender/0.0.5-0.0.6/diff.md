# Comparing `tmp/yaml-extender-0.0.5.tar.gz` & `tmp/yaml-extender-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml-extender-0.0.5.tar", last modified: Thu Mar  2 11:27:31 2023, max compression
+gzip compressed data, was "yaml-extender-0.0.6.tar", last modified: Thu May 11 18:06:56 2023, max compression
```

## Comparing `yaml-extender-0.0.5.tar` & `yaml-extender-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-03-02 11:27:31.146826 yaml-extender-0.0.5/
--rw-rw-rw-   0        0        0      496 2023-03-02 11:26:38.000000 yaml-extender-0.0.5/CHANGELOG.rst
--rw-rw-rw-   0        0        0     1507 2023-01-31 17:42:46.000000 yaml-extender-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      364 2022-11-12 09:32:28.000000 yaml-extender-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     7135 2023-03-02 11:27:31.145825 yaml-extender-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4580 2023-01-31 18:06:45.000000 yaml-extender-0.0.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-02 11:27:31.111831 yaml-extender-0.0.5/docs/
--rw-rw-rw-   0        0        0     6717 2022-11-12 09:32:28.000000 yaml-extender-0.0.5/docs/conf.py
--rw-rw-rw-   0        0        0     1373 2023-01-31 18:53:09.000000 yaml-extender-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-02 11:27:31.146826 yaml-extender-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-02 11:27:31.103829 yaml-extender-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-03-02 11:27:31.126848 yaml-extender-0.0.5/src/yaml_extender/
--rw-rw-rw-   0        0        0       68 2023-03-02 11:26:03.000000 yaml-extender-0.0.5/src/yaml_extender/__init__.py
--rw-rw-rw-   0        0        0       96 2023-02-02 18:58:26.000000 yaml-extender-0.0.5/src/yaml_extender/__main__.py
--rw-rw-rw-   0        0        0     1378 2023-03-01 16:56:04.000000 yaml-extender-0.0.5/src/yaml_extender/cli.py
--rw-rw-rw-   0        0        0      796 2022-11-12 14:08:22.000000 yaml-extender-0.0.5/src/yaml_extender/logger.py
-drwxrwxrwx   0        0        0        0 2023-03-02 11:27:31.144825 yaml-extender-0.0.5/src/yaml_extender/resolver/
--rw-rw-rw-   0        0        0        0 2022-11-17 17:18:02.000000 yaml-extender-0.0.5/src/yaml_extender/resolver/__init__.py
--rw-rw-rw-   0        0        0     5876 2023-03-01 17:07:08.000000 yaml-extender-0.0.5/src/yaml_extender/resolver/include_resolver.py
--rw-rw-rw-   0        0        0     2975 2023-02-27 17:47:13.000000 yaml-extender-0.0.5/src/yaml_extender/resolver/loop_resolver.py
--rw-rw-rw-   0        0        0     5542 2023-02-27 17:47:13.000000 yaml-extender-0.0.5/src/yaml_extender/resolver/reference_resolver.py
--rw-rw-rw-   0        0        0      683 2023-02-27 18:52:59.000000 yaml-extender-0.0.5/src/yaml_extender/resolver/resolver.py
--rw-rw-rw-   0        0        0      469 2023-02-27 18:50:34.000000 yaml-extender-0.0.5/src/yaml_extender/xyml_exception.py
--rw-rw-rw-   0        0        0     1845 2023-03-01 17:09:48.000000 yaml-extender-0.0.5/src/yaml_extender/xyml_file.py
--rw-rw-rw-   0        0        0      963 2023-01-15 11:35:59.000000 yaml-extender-0.0.5/src/yaml_extender/yaml_loader.py
-drwxrwxrwx   0        0        0        0 2023-03-02 11:27:31.140820 yaml-extender-0.0.5/src/yaml_extender.egg-info/
--rw-rw-rw-   0        0        0     7135 2023-03-02 11:27:31.000000 yaml-extender-0.0.5/src/yaml_extender.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      751 2023-03-02 11:27:31.000000 yaml-extender-0.0.5/src/yaml_extender.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-02 11:27:31.000000 yaml-extender-0.0.5/src/yaml_extender.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-03-02 11:27:31.000000 yaml-extender-0.0.5/src/yaml_extender.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-03-02 11:27:31.000000 yaml-extender-0.0.5/src/yaml_extender.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-02 11:27:31.000000 yaml-extender-0.0.5/src/yaml_extender.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 18:06:56.390165 yaml-extender-0.0.6/
+-rw-rw-rw-   0        0        0      605 2023-05-11 18:06:24.000000 yaml-extender-0.0.6/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     1507 2023-01-31 17:42:46.000000 yaml-extender-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      364 2022-11-12 09:32:28.000000 yaml-extender-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     7135 2023-05-11 18:06:56.389163 yaml-extender-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4580 2023-01-31 18:06:45.000000 yaml-extender-0.0.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-11 18:06:56.361138 yaml-extender-0.0.6/docs/
+-rw-rw-rw-   0        0        0     6717 2022-11-12 09:32:28.000000 yaml-extender-0.0.6/docs/conf.py
+-rw-rw-rw-   0        0        0     1373 2023-01-31 18:53:09.000000 yaml-extender-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 18:06:56.390165 yaml-extender-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 18:06:56.351599 yaml-extender-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 18:06:56.373149 yaml-extender-0.0.6/src/yaml_extender/
+-rw-rw-rw-   0        0        0       68 2023-05-11 18:05:30.000000 yaml-extender-0.0.6/src/yaml_extender/__init__.py
+-rw-rw-rw-   0        0        0       96 2023-02-02 18:58:26.000000 yaml-extender-0.0.6/src/yaml_extender/__main__.py
+-rw-rw-rw-   0        0        0     1505 2023-05-11 18:01:55.000000 yaml-extender-0.0.6/src/yaml_extender/cli.py
+-rw-rw-rw-   0        0        0      796 2022-11-12 14:08:22.000000 yaml-extender-0.0.6/src/yaml_extender/logger.py
+drwxrwxrwx   0        0        0        0 2023-05-11 18:06:56.388162 yaml-extender-0.0.6/src/yaml_extender/resolver/
+-rw-rw-rw-   0        0        0        0 2022-11-17 17:18:02.000000 yaml-extender-0.0.6/src/yaml_extender/resolver/__init__.py
+-rw-rw-rw-   0        0        0     5876 2023-03-01 17:07:08.000000 yaml-extender-0.0.6/src/yaml_extender/resolver/include_resolver.py
+-rw-rw-rw-   0        0        0     2975 2023-02-27 17:47:13.000000 yaml-extender-0.0.6/src/yaml_extender/resolver/loop_resolver.py
+-rw-rw-rw-   0        0        0     5542 2023-02-27 17:47:13.000000 yaml-extender-0.0.6/src/yaml_extender/resolver/reference_resolver.py
+-rw-rw-rw-   0        0        0      683 2023-02-27 18:52:59.000000 yaml-extender-0.0.6/src/yaml_extender/resolver/resolver.py
+-rw-rw-rw-   0        0        0      469 2023-02-27 18:50:34.000000 yaml-extender-0.0.6/src/yaml_extender/xyml_exception.py
+-rw-rw-rw-   0        0        0     1883 2023-05-11 18:04:26.000000 yaml-extender-0.0.6/src/yaml_extender/xyml_file.py
+-rw-rw-rw-   0        0        0      963 2023-01-15 11:35:59.000000 yaml-extender-0.0.6/src/yaml_extender/yaml_loader.py
+drwxrwxrwx   0        0        0        0 2023-05-11 18:06:56.385160 yaml-extender-0.0.6/src/yaml_extender.egg-info/
+-rw-rw-rw-   0        0        0     7135 2023-05-11 18:06:56.000000 yaml-extender-0.0.6/src/yaml_extender.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      751 2023-05-11 18:06:56.000000 yaml-extender-0.0.6/src/yaml_extender.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 18:06:56.000000 yaml-extender-0.0.6/src/yaml_extender.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-11 18:06:56.000000 yaml-extender-0.0.6/src/yaml_extender.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2023-05-11 18:06:56.000000 yaml-extender-0.0.6/src/yaml_extender.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-11 18:06:56.000000 yaml-extender-0.0.6/src/yaml_extender.egg-info/top_level.txt
```

### Comparing `yaml-extender-0.0.5/LICENSE` & `yaml-extender-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.5/PKG-INFO` & `yaml-extender-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-extender
-Version: 0.0.5
+Version: 0.0.6
 Summary: Extends the common .yaml syntax to provide more complex configuration options
 Author-email: Simon Gallitscher <adun.sg@gmx.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Simon Gallitscher
         All rights reserved.
```

### Comparing `yaml-extender-0.0.5/README.rst` & `yaml-extender-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.5/docs/conf.py` & `yaml-extender-0.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.5/pyproject.toml` & `yaml-extender-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.5/src/yaml_extender/cli.py` & `yaml-extender-0.0.6/src/yaml_extender/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,24 +12,25 @@
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("input", help="Input yaml file to be parsed", type=Path)
     parser.add_argument("output", help="Output file to save to", type=Path)
     parser.add_argument("-i", "--include", help="Include paths", type=Path, action="append")
+    parser.add_argument("--sort-keys", help="When set output file will have keys sorted", action="store_true")
     args, unknown_args = parser.parse_known_args()
 
     if not args.input.is_file:
         raise FileNotFoundError(f"Path {args.input} is no valid file.")
     additional_args = parse_unknown_args(unknown_args)
     LOGGER.info("Additional parameters:\n" + "\n".join([f"{k}: {v}" for k, v in additional_args.items()]))
     xyml_file = XYmlFile(args.input, additional_args, args.include)
     output_dir: Path = args.output.parent
     output_dir.mkdir(exist_ok=True, parents=True)
-    xyml_file.save(args.output)
+    xyml_file.save(args.output, args.sort_keys)
 
 
 def parse_unknown_args(args: List) -> Dict:
     arg_dict = dict(zip(args[:-1:2], args[1::2]))
     ret_val = {}
     # Parse numbers from strings
     for k, v in arg_dict.items():
```

### Comparing `yaml-extender-0.0.5/src/yaml_extender/logger.py` & `yaml-extender-0.0.6/src/yaml_extender/logger.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.5/src/yaml_extender/resolver/include_resolver.py` & `yaml-extender-0.0.6/src/yaml_extender/resolver/include_resolver.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.5/src/yaml_extender/resolver/loop_resolver.py` & `yaml-extender-0.0.6/src/yaml_extender/resolver/loop_resolver.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.5/src/yaml_extender/resolver/reference_resolver.py` & `yaml-extender-0.0.6/src/yaml_extender/resolver/reference_resolver.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.5/src/yaml_extender/resolver/resolver.py` & `yaml-extender-0.0.6/src/yaml_extender/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.5/src/yaml_extender/xyml_file.py` & `yaml-extender-0.0.6/src/yaml_extender/xyml_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,12 +43,12 @@
         config["xyml"] = {}
         config["xyml"][ENV_KEY] = os.environ
         config["xyml"][PARAM_KEY] = self.params
         ref_resolver = ReferenceResolver(False)
         processed_content = ref_resolver.resolve(processed_content, config)
         return processed_content
 
-    def save(self, path: str):
+    def save(self, path: str, sort_keys=False):
         with open(path, 'w') as file:
-            yaml.dump(self.content, file)
+            yaml.dump(self.content, file, sort_keys=sort_keys)
```

### Comparing `yaml-extender-0.0.5/src/yaml_extender/yaml_loader.py` & `yaml-extender-0.0.6/src/yaml_extender/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.5/src/yaml_extender.egg-info/PKG-INFO` & `yaml-extender-0.0.6/src/yaml_extender.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-extender
-Version: 0.0.5
+Version: 0.0.6
 Summary: Extends the common .yaml syntax to provide more complex configuration options
 Author-email: Simon Gallitscher <adun.sg@gmx.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Simon Gallitscher
         All rights reserved.
```

### Comparing `yaml-extender-0.0.5/src/yaml_extender.egg-info/SOURCES.txt` & `yaml-extender-0.0.6/src/yaml_extender.egg-info/SOURCES.txt`

 * *Files identical despite different names*

