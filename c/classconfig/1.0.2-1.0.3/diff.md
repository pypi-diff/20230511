# Comparing `tmp/classconfig-1.0.2.tar.gz` & `tmp/classconfig-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classconfig-1.0.2.tar", last modified: Wed May  3 08:15:34 2023, max compression
+gzip compressed data, was "classconfig-1.0.3.tar", last modified: Thu May 11 12:40:41 2023, max compression
```

## Comparing `classconfig-1.0.2.tar` & `classconfig-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-05-03 08:15:34.227396 classconfig-1.0.2/
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1211 2022-05-31 11:17:31.000000 classconfig-1.0.2/LICENSE
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       24 2023-04-27 11:55:37.000000 classconfig-1.0.2/MANIFEST.in
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3770 2023-05-03 08:15:34.227396 classconfig-1.0.2/PKG-INFO
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3320 2023-04-27 10:43:07.000000 classconfig-1.0.2/README.md
-drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-05-03 08:15:34.223396 classconfig-1.0.2/classconfig/
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      111 2023-04-26 13:54:46.000000 classconfig-1.0.2/classconfig/__init__.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2845 2023-04-26 14:19:24.000000 classconfig-1.0.2/classconfig/base.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2527 2023-04-26 13:46:41.000000 classconfig-1.0.2/classconfig/classes.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)    38658 2023-05-03 08:13:31.000000 classconfig-1.0.2/classconfig/configurable.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     7128 2023-04-27 11:23:40.000000 classconfig-1.0.2/classconfig/transforms.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     9236 2023-04-27 10:56:32.000000 classconfig-1.0.2/classconfig/validators.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      382 2023-04-26 15:16:39.000000 classconfig-1.0.2/classconfig/yaml.py
-drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-05-03 08:15:34.227396 classconfig-1.0.2/classconfig.egg-info/
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3770 2023-05-03 08:15:34.000000 classconfig-1.0.2/classconfig.egg-info/PKG-INFO
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      516 2023-05-03 08:15:34.000000 classconfig-1.0.2/classconfig.egg-info/SOURCES.txt
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)        1 2023-05-03 08:15:34.000000 classconfig-1.0.2/classconfig.egg-info/dependency_links.txt
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       21 2023-05-03 08:15:34.000000 classconfig-1.0.2/classconfig.egg-info/requires.txt
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       12 2023-05-03 08:15:34.000000 classconfig-1.0.2/classconfig.egg-info/top_level.txt
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       20 2023-04-26 13:45:04.000000 classconfig-1.0.2/requirements.txt
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       38 2023-05-03 08:15:34.227396 classconfig-1.0.2/setup.cfg
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1115 2023-05-03 08:15:02.000000 classconfig-1.0.2/setup.py
-drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-05-03 08:15:34.227396 classconfig-1.0.2/tests/
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2626 2023-04-27 11:14:46.000000 classconfig-1.0.2/tests/test_classes.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)    23630 2023-04-26 15:10:49.000000 classconfig-1.0.2/tests/test_configurable.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1948 2023-04-27 10:43:21.000000 classconfig-1.0.2/tests/test_readme.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2521 2023-04-27 11:32:32.000000 classconfig-1.0.2/tests/test_transforms.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     5872 2023-04-27 11:12:58.000000 classconfig-1.0.2/tests/test_validators.py
+drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-05-11 12:40:41.205677 classconfig-1.0.3/
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1211 2022-05-31 11:17:31.000000 classconfig-1.0.3/LICENSE
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       24 2023-04-27 11:55:37.000000 classconfig-1.0.3/MANIFEST.in
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3771 2023-05-11 12:40:41.205677 classconfig-1.0.3/PKG-INFO
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3321 2023-05-04 05:03:52.000000 classconfig-1.0.3/README.md
+drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-05-11 12:40:41.201677 classconfig-1.0.3/classconfig/
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      111 2023-04-26 13:54:46.000000 classconfig-1.0.3/classconfig/__init__.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2845 2023-04-26 14:19:24.000000 classconfig-1.0.3/classconfig/base.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2527 2023-05-11 12:12:31.000000 classconfig-1.0.3/classconfig/classes.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)    40390 2023-05-11 12:36:30.000000 classconfig-1.0.3/classconfig/configurable.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     7128 2023-04-27 11:23:40.000000 classconfig-1.0.3/classconfig/transforms.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     9236 2023-04-27 10:56:32.000000 classconfig-1.0.3/classconfig/validators.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      382 2023-04-26 15:16:39.000000 classconfig-1.0.3/classconfig/yaml.py
+drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-05-11 12:40:41.201677 classconfig-1.0.3/classconfig.egg-info/
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3771 2023-05-11 12:40:41.000000 classconfig-1.0.3/classconfig.egg-info/PKG-INFO
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      516 2023-05-11 12:40:41.000000 classconfig-1.0.3/classconfig.egg-info/SOURCES.txt
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)        1 2023-05-11 12:40:41.000000 classconfig-1.0.3/classconfig.egg-info/dependency_links.txt
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       21 2023-05-11 12:40:41.000000 classconfig-1.0.3/classconfig.egg-info/requires.txt
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       12 2023-05-11 12:40:41.000000 classconfig-1.0.3/classconfig.egg-info/top_level.txt
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       20 2023-04-26 13:45:04.000000 classconfig-1.0.3/requirements.txt
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       38 2023-05-11 12:40:41.205677 classconfig-1.0.3/setup.cfg
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1115 2023-05-11 12:39:58.000000 classconfig-1.0.3/setup.py
+drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-05-11 12:40:41.205677 classconfig-1.0.3/tests/
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2626 2023-04-27 11:14:46.000000 classconfig-1.0.3/tests/test_classes.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)    25594 2023-05-11 12:36:30.000000 classconfig-1.0.3/tests/test_configurable.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1948 2023-04-27 10:43:21.000000 classconfig-1.0.3/tests/test_readme.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2521 2023-04-27 11:32:32.000000 classconfig-1.0.3/tests/test_transforms.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     5872 2023-04-27 11:12:58.000000 classconfig-1.0.3/tests/test_validators.py
```

### Comparing `classconfig-1.0.2/LICENSE` & `classconfig-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.2/PKG-INFO` & `classconfig-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classconfig
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package for creating configuration files automatically and loading objects from those configuration files.
 Home-page: https://github.com/mdocekal/classconfig
 Author: Martin Dočekal
 Keywords: configuration,auto config,config,configurable,configurable class,configurable object,configurable attribute
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -55,14 +55,22 @@
 from classconfig import Config
 
 Config(Character).save("config.yaml")
 ```
 
 You will get a file with the following content:
 
+
+```yaml
+lvl: 1  # Level of a character
+name: # Name of a character
+inventory: # Character's inventory
+  size: 10  # Size of an inventory
+```
+
 ### Validation
 As you have seen in the previous example, it is possible to add a validator. 
 A validator could be any callable that takes one argument and return `True` when valid. 
 You can also raise an exception if the argument is invalid to specify the reason for the failure.
 
 There are various predefined validators in `classconfig.validators` module.
 
@@ -70,21 +78,14 @@
 It is possible to specify a transformation (`transform` attribute) that will transform user input. The transformation
 is done before the validation. Thus, it can be used to transform input into valid form.
 
 It can be any callable that takes one argument and returns the transformed value, but there also exist some predefined
 transformations in `classconfig.transforms` module.
 
 
-```yaml
-lvl: 1  # Level of a character
-name: # Name of a character
-inventory: # Character's inventory
-  size: 10  # Size of an inventory
-```
-
 ### Loading
 Now let's load the configuration file we just created and create an instance of `Character` class:
 
 ```python
 from classconfig import Config, ConfigurableFactory
 
 config = Config(Character).load(path)   # load configuration file
```

### Comparing `classconfig-1.0.2/README.md` & `classconfig-1.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,22 @@
 from classconfig import Config
 
 Config(Character).save("config.yaml")
 ```
 
 You will get a file with the following content:
 
+
+```yaml
+lvl: 1  # Level of a character
+name: # Name of a character
+inventory: # Character's inventory
+  size: 10  # Size of an inventory
+```
+
 ### Validation
 As you have seen in the previous example, it is possible to add a validator. 
 A validator could be any callable that takes one argument and return `True` when valid. 
 You can also raise an exception if the argument is invalid to specify the reason for the failure.
 
 There are various predefined validators in `classconfig.validators` module.
 
@@ -59,21 +67,14 @@
 It is possible to specify a transformation (`transform` attribute) that will transform user input. The transformation
 is done before the validation. Thus, it can be used to transform input into valid form.
 
 It can be any callable that takes one argument and returns the transformed value, but there also exist some predefined
 transformations in `classconfig.transforms` module.
 
 
-```yaml
-lvl: 1  # Level of a character
-name: # Name of a character
-inventory: # Character's inventory
-  size: 10  # Size of an inventory
-```
-
 ### Loading
 Now let's load the configuration file we just created and create an instance of `Character` class:
 
 ```python
 from classconfig import Config, ConfigurableFactory
 
 config = Config(Character).load(path)   # load configuration file
```

### Comparing `classconfig-1.0.2/classconfig/base.py` & `classconfig-1.0.3/classconfig/base.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.2/classconfig/classes.py` & `classconfig-1.0.3/classconfig/classes.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.2/classconfig/configurable.py` & `classconfig-1.0.3/classconfig/configurable.py`

 * *Files 4% similar despite different names*

```diff
@@ -566,14 +566,55 @@
             else:
                 raise ValueError(f"Unknown type {type(var)}")
 
             yaml.insert(i, var.name, generated, comment=var.desc if comments else None)
 
         return yaml
 
+    @classmethod
+    def config_from_object(cls, o: Any) -> "Config":
+        """
+        Creates configuration with user default values from given object.
+
+        :param o: object with values
+        :return: configuration
+        """
+
+        return Config(o.__class__, file_override_user_defaults=cls.configurable_values_from_object(o))
+
+    @classmethod
+    def configurable_values_from_object(cls, o: Any) -> Dict:
+        """
+        Creates dictionary with values associated for configurable attributes from given object.
+
+        :param o: object with values
+        :return: dictionary with user default values
+        """
+        config = {}
+
+        for i, (var_name, var) in enumerate(get_configurable_attributes(o.__class__).items()):
+            if isinstance(var, ConfigurableValue):
+                config[var_name] = getattr(o, var_name)
+            elif isinstance(var, ConfigurableFactory):
+                config[var_name] = cls.configurable_values_from_object(getattr(o, var_name))
+            elif isinstance(var, ConfigurableSubclassFactory):
+                config[var_name] = {}
+                config[var_name]["cls"] = getattr(o, var_name).__class__.__name__
+                config[var_name]["config"] = cls.configurable_values_from_object(getattr(o, var_name))
+            elif isinstance(var, ListOfConfigurableSubclassFactoryAttributes):
+                config[var_name] = []
+                for sub_o in enumerate(getattr(o, var_name)):
+                    config[var_name].append(cls.configurable_values_from_object(sub_o))
+            elif isinstance(var, UsedConfig):
+                continue
+            else:
+                raise ValueError(f"Unknown type {type(var)}")
+
+        return config
+
     def save(self, file_path: Union[str, TextIO], comments: bool = True) -> None:
         """
         Saves configuration into file.
 
         :param file_path: path to file
         :param comments: true inserts comments
         """
```

### Comparing `classconfig-1.0.2/classconfig/transforms.py` & `classconfig-1.0.3/classconfig/transforms.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.2/classconfig/validators.py` & `classconfig-1.0.3/classconfig/validators.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.2/classconfig.egg-info/PKG-INFO` & `classconfig-1.0.3/classconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classconfig
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package for creating configuration files automatically and loading objects from those configuration files.
 Home-page: https://github.com/mdocekal/classconfig
 Author: Martin Dočekal
 Keywords: configuration,auto config,config,configurable,configurable class,configurable object,configurable attribute
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -55,14 +55,22 @@
 from classconfig import Config
 
 Config(Character).save("config.yaml")
 ```
 
 You will get a file with the following content:
 
+
+```yaml
+lvl: 1  # Level of a character
+name: # Name of a character
+inventory: # Character's inventory
+  size: 10  # Size of an inventory
+```
+
 ### Validation
 As you have seen in the previous example, it is possible to add a validator. 
 A validator could be any callable that takes one argument and return `True` when valid. 
 You can also raise an exception if the argument is invalid to specify the reason for the failure.
 
 There are various predefined validators in `classconfig.validators` module.
 
@@ -70,21 +78,14 @@
 It is possible to specify a transformation (`transform` attribute) that will transform user input. The transformation
 is done before the validation. Thus, it can be used to transform input into valid form.
 
 It can be any callable that takes one argument and returns the transformed value, but there also exist some predefined
 transformations in `classconfig.transforms` module.
 
 
-```yaml
-lvl: 1  # Level of a character
-name: # Name of a character
-inventory: # Character's inventory
-  size: 10  # Size of an inventory
-```
-
 ### Loading
 Now let's load the configuration file we just created and create an instance of `Character` class:
 
 ```python
 from classconfig import Config, ConfigurableFactory
 
 config = Config(Character).load(path)   # load configuration file
```

### Comparing `classconfig-1.0.2/classconfig.egg-info/SOURCES.txt` & `classconfig-1.0.3/classconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.2/setup.py` & `classconfig-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 with open("requirements.txt") as f:
     REQUIREMENTS = [line.strip() for line in f if is_requirement(line)]
 
 
 setup_args = dict(
     name='classconfig',
-    version='1.0.2',
+    version='1.0.3',
     description='Package for creating configuration files automatically and loading objects from those configuration files.',
     long_description_content_type="text/markdown",
     long_description=README,
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     author='Martin Dočekal',
     keywords=['configuration', 'auto config', 'config', 'configurable', 'configurable class', 'configurable object',
               'configurable attribute'],
```

### Comparing `classconfig-1.0.2/tests/test_classes.py` & `classconfig-1.0.3/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.2/tests/test_configurable.py` & `classconfig-1.0.3/tests/test_configurable.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,14 +406,69 @@
                         "child_a_attribute": 6
                     }
                 }
             ]
         }, config)
 
 
+class Inventory(ConfigurableMixin):
+    size: int = ConfigurableValue(desc="Size of an inventory", user_default=10, validator=lambda x: x > 0)
+    parent = ConfigurableSubclassFactory(parent_cls_type=ParentC, desc="description of parent")
+
+
+class Character(ConfigurableMixin):
+    lvl: int = ConfigurableValue(desc="Level of a character", user_default=1, validator=lambda x: x > 0)
+    name: str = ConfigurableValue(desc="Name of a character")
+    inventory: Inventory = ConfigurableFactory(desc="Character's inventory", cls_type=Inventory)
+
+
+class TestConfigurableValuesForObject(TestCase):
+
+    def setUp(self) -> None:
+        self.configurable_object = Character(lvl=99,
+                                             name="John",
+                                             inventory=Inventory(size=666, parent=ChildA(child_a_attribute="abc")))
+
+    def test_config_from_object(self):
+        config = Config.config_from_object(self.configurable_object)
+        self.assertEqual({
+            "lvl": 99,
+            "name": "John",
+            "inventory": {
+                "size": 666,
+                "parent": {
+                    "cls": "ChildA",
+                    "config": {
+                        "child_a_attribute": "abc"
+                    }
+                }
+            }
+        }, config.file_override_user_defaults)
+        self.assertEqual(Character, config.cls_type)
+
+    def test_configurable_values_from_object(self):
+        vals = Config.configurable_values_from_object(self.configurable_object)
+        self.assertEqual(
+            {
+                "lvl": 99,
+                "name": "John",
+                "inventory": {
+                    "size": 666,
+                    "parent": {
+                        "cls": "ChildA",
+                        "config": {
+                            "child_a_attribute": "abc"
+                        }
+                    }
+                }
+            },
+            vals
+        )
+
+
 class ConfigurableClassWithOverridenUserDefaults:
     a = ConfigurableValue(desc="description of a", user_default=1)
     another = ConfigurableFactory(desc="class that needs configuration", cls_type=AnotherConfigurableClass,
                                   voluntary=True, file_override_user_defaults={"d": "cba"})
     c = ConfigurableSubclassFactory(parent_cls_type=BaseOfAnotherConfigurableClass,
                                     desc="description of c", user_default=AnotherConfigurableClass,
                                     file_override_user_defaults={"c": "opk", "d": "lmn"})
```

### Comparing `classconfig-1.0.2/tests/test_readme.py` & `classconfig-1.0.3/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.2/tests/test_transforms.py` & `classconfig-1.0.3/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.2/tests/test_validators.py` & `classconfig-1.0.3/tests/test_validators.py`

 * *Files identical despite different names*

