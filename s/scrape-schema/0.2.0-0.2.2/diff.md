# Comparing `tmp/scrape_schema-0.2.0.tar.gz` & `tmp/scrape_schema-0.2.2.tar.gz`

## Comparing `scrape_schema-0.2.0.tar` & `scrape_schema-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/__init__.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/_base_configs.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/_logger.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/_type_caster.py
--rw-r--r--   0        0        0    21507 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/base.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/exceptions.py
--rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/callbacks/__init__.py
--rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/callbacks/parsel.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/callbacks/slax.py
--rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/callbacks/soup.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/factory/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/fields/__init__.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/fields/mock.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/fields/nested.py
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/fields/parsel.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/fields/regex.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/fields/slax.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/fields/soup.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/LICENSE
--rw-r--r--   0        0        0     5911 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/README.md
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     8204 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/scrape_schema/__init__.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/scrape_schema/_base_configs.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/scrape_schema/_logger.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/scrape_schema/_type_caster.py
+-rw-r--r--   0        0        0    19793 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/scrape_schema/base.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/scrape_schema/exceptions.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/scrape_schema/hooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/scrape_schema/callbacks/__init__.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/scrape_schema/callbacks/parsel.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/scrape_schema/callbacks/slax.py
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/scrape_schema/callbacks/soup.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/scrape_schema/factory/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/scrape_schema/fields/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/scrape_schema/fields/mock.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/scrape_schema/fields/nested.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/scrape_schema/fields/parsel.py
+-rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/scrape_schema/fields/regex.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/scrape_schema/fields/slax.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/scrape_schema/fields/soup.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/LICENSE
+-rw-r--r--   0        0        0     5911 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/README.md
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     8204 2020-02-02 00:00:00.000000 scrape_schema-0.2.2/PKG-INFO
```

### Comparing `scrape_schema-0.2.0/scrape_schema/_base_configs.py` & `scrape_schema-0.2.2/scrape_schema/_base_configs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 from typing import Any, ClassVar, Dict, Optional, Type
 
-from scrape_schema.hooks import HooksStorage
-
 
 class BaseFieldConfig:
     """BaseField configuration class:
 
     * parser: Optional[Type[Any]] - parser backend object. If value None - work with python str
     """
 
     parser: ClassVar[Optional[Type[Any]]] = None
-    hooks: ClassVar["HooksStorage"] = HooksStorage()
 
 
 class BaseSchemaConfig:
     """Schema configuration for BaseSchema
 
     parsers_config: dict[Type[Any], dict[str, Any]] parser classes for usage backend
 
@@ -31,8 +28,7 @@
 
     hooks_priority: bool - defined hooks overwrite Field attributes in params. Default True
     """
 
     parsers_config: ClassVar[Dict[Type[Any], Dict[str, Any]]] = {}
     type_cast: ClassVar[bool] = True
     fails_attempt: ClassVar[int] = -1
-    hooks_priority: ClassVar[bool] = True
```

### Comparing `scrape_schema-0.2.0/scrape_schema/_logger.py` & `scrape_schema-0.2.2/scrape_schema/_logger.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.2.0/scrape_schema/_type_caster.py` & `scrape_schema-0.2.2/scrape_schema/_type_caster.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.2.0/scrape_schema/base.py` & `scrape_schema-0.2.2/scrape_schema/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,49 +42,49 @@
 def extract_fields(markup: MARKUP_TYPE, **fields: "BaseField") -> Dict[str, Any]:
     return {key: field.extract(markup) for key, field in fields.items()}
 
 
 class ABCField(ABC):
     @abstractmethod
     def _parse(self, markup: MARKUP_TYPE) -> Any:
-        ...
+        pass
 
     @abstractmethod
     def _filter(
         self,
         value: T,
         *,
         schema_instance: Optional["BaseSchema"] = None,
         name: Optional[str] = None,
     ) -> bool:
-        ...
+        pass
 
     @abstractmethod
     def _factory(
         self,
         value: T,
         *,
         schema_instance: Optional["BaseSchema"] = None,
         name: Optional[str] = None,
     ) -> T:
-        ...
+        pass
 
     @abstractmethod
     def _callback(
         self,
         value: T,
         *,
         schema_instance: Optional["BaseSchema"] = None,
         name: Optional[str] = None,
     ) -> T:
-        ...
+        pass
 
     @abstractmethod
     def _typing(self, instance: "BaseSchema", name: str, value: T) -> T:
-        ...
+        pass
 
 
 class BaseField(ABCField):
     class Config(BaseFieldConfig):
         pass
 
     def __init__(
@@ -204,15 +204,15 @@
         else:
             logger.debug(
                 "{}.{} := {} raw value(s)", instance.__schema_name__, name, value
             )
 
         value = self._filter(value, schema_instance=instance, name=name)
         value = self._callback(value, schema_instance=instance, name=name)
-        if self.factory or self.Config.hooks.get_factory(name):
+        if self.factory:
             value = self._factory(value, schema_instance=instance, name=name)
         else:
             value = self._typing(instance, name, value)
         logger.info("{}.{} = `{}` Done", instance.__class__.__name__, name, value)
         return value
 
     def _filter(
@@ -223,27 +223,15 @@
         name: Optional[str] = None,
     ) -> Any:
         """filter parsed value by filter_ function, if it passed
 
         :param value: list or dict value. dict filter by values
         :return: filtered value
         """
-        if schema_instance and name:
-            if schema_instance.Config.hooks_priority:
-                hook = self.Config.hooks.get_filter(
-                    f"{schema_instance.__schema_name__}.{name}"
-                )
-                filter_ = hook or self.filter_
-            else:
-                hook = self.Config.hooks.get_filter(
-                    f"{schema_instance.__schema_name__}.{name}"
-                )
-                filter_ = self.filter_ or hook
-        else:
-            filter_ = self.filter_
+        filter_ = self.filter_
 
         if filter_ and self._is_iterable_and_not_string_value(value):
             logger.debug(
                 "{}.{} := filter_({})",
                 schema_instance.__schema_name__
                 if schema_instance
                 else self.__class__.__name__,
@@ -264,27 +252,15 @@
         name: Optional[str] = None,
     ) -> Any:
         """factory result value entrypoint
 
         :param value: parsed value
         :return:
         """
-        if schema_instance and name:
-            if schema_instance.Config.hooks_priority:
-                hook = self.Config.hooks.get_factory(
-                    f"{schema_instance.__schema_name__}.{name}"
-                )
-                factory = hook or self.factory
-            else:
-                hook = self.Config.hooks.get_factory(
-                    f"{schema_instance.__schema_name__}.{name}"
-                )
-                factory = self.factory or hook
-        else:
-            factory = self.factory
+        factory = self.factory
         if factory:
             logger.debug(
                 "{}.{} := factory({})",
                 schema_instance.__schema_name__
                 if schema_instance
                 else self.__class__.__name__,
                 name or "extract",
@@ -300,27 +276,15 @@
         name: Optional[str] = None,
     ) -> Any:
         """eval value by callback function
 
         :param value:
         :return:
         """
-        if schema_instance and name:
-            if schema_instance.Config.hooks_priority:
-                hook = self.Config.hooks.get_callback(
-                    f"{schema_instance.__schema_name__}.{name}"
-                )
-                callback = hook or self.callback
-            else:
-                hook = self.Config.hooks.get_callback(
-                    f"{schema_instance.__schema_name__}.{name}"
-                )
-                callback = self.callback or hook
-        else:
-            callback = self.callback
+        callback = self.callback
 
         if not callback:
             return value
         logger.debug(
             "{}.{} := callback({})",
             schema_instance.__schema_name__
             if schema_instance
@@ -401,20 +365,19 @@
     def _get_parser(self, field_parser_class: Type) -> Optional[Dict[str, Any]]:
         return self.Config.parsers_config.get(field_parser_class, None)
 
     def _check_parser_config(self, field: BaseField, field_parser: Type) -> bool:
         if self._get_parser(field_parser) is None:
             try:
                 raise MarkupNotFoundError(
-                    f"{field.__class__.__name__} required "
-                    f"{type(field_parser).__name__} configuration"
+                    f"{field.__class__.__name__} required {type(field_parser).__name__} configuration"
                 )
             except MarkupNotFoundError as e:
-                logger.exception(e)
-                raise e
+                logger.exception("{}", e)
+                raise
         return True
 
     @staticmethod
     def _success_field_parse(field: BaseField, value) -> bool:
         return (
             hasattr(field, "default")
             and value != field.default
@@ -593,18 +556,14 @@
     def _to_dict(value: Union["BaseSchema", List, Dict, Any]):
         if isinstance(value, BaseSchema):
             return value.dict()
 
         elif isinstance(value, list):
             if all(isinstance(val, BaseSchema) for val in value):
                 return [val.dict() for val in value]
-
-        elif isinstance(value, dict):
-            if all(isinstance(val, BaseSchema) for val in value.values()):
-                return {k: v.dict() for k, v in value.items()}
         return value
 
     def raw_dict(self) -> Dict[str, Any]:
         """convert schema object to python dict"""
         return {k: self._to_dict(v) for k, v in self.__dict__.items() if k != "Config"}
 
     def dict(self) -> Dict[str, Any]:
```

### Comparing `scrape_schema-0.2.0/scrape_schema/callbacks/parsel.py` & `scrape_schema-0.2.2/scrape_schema/callbacks/parsel.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,15 @@
     def wrapper(
         element: Union[SelectorList[_SelectorType], Any]
     ) -> Union[Optional[str], Any]:
         if isinstance(element, (SelectorList, Selector)):
             if deep:
                 text = sep.join(element.css("::text").getall())
             else:
-                # TODO
                 text = element.css("::text").get(default=default)  # type: ignore
-
             if text:
                 return text.strip() if strip else text
             return text
         return element
 
     return wrapper
```

### Comparing `scrape_schema-0.2.0/scrape_schema/callbacks/slax.py` & `scrape_schema-0.2.2/scrape_schema/callbacks/slax.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.2.0/scrape_schema/callbacks/soup.py` & `scrape_schema-0.2.2/scrape_schema/callbacks/soup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """build-in callbacks for fields.soup"""
 import re
 from typing import Any, Callable, Dict, List, Optional, Union
 
 from bs4 import BeautifulSoup, Tag
 
 RE_TAG_NAME = re.compile(r"<(\w+)")
-RE_TAG_ATTRS = re.compile(r'(?P<name>[\w_\-:.]+)="(?P<value>[\w_\-:.]+)"')
+RE_TAG_ATTRS = re.compile(r'(?P<name>[\w_\-:.]+)="(?P<value>[\w_\-:.\s]+)"')
 
 __all__ = [
     "get_attr",
     "get_text",
     "replace_text",
     "crop_by_tag",
     "crop_by_tag_all",
@@ -42,15 +42,15 @@
         <a id="1", class="thing"> -> {"name": "a", "attrs": {"id": "1", "class": "thing"}}
     """
     if not (match := RE_TAG_NAME.search(element)):
         raise TypeError(f"Element `{element}` is not valid HTML tag")
     tag_name = match.group(1)
     attrs = dict(RE_TAG_ATTRS.findall(element))
     if (klass := attrs.get("class")) and len(klass.split(" ")) != 1:
-        attrs["class"] = klass.split(" ")
+        attrs["class"] = klass.split()
     return {"name": tag_name, "attrs": attrs}
 
 
 def get_text(
     separator: str = "", strip: bool = False
 ) -> Callable[[Union[Tag, Any]], Union[str, Any]]:
     """get text from bs4.Tag
```

### Comparing `scrape_schema-0.2.0/scrape_schema/fields/mock.py` & `scrape_schema-0.2.2/scrape_schema/fields/mock.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.2.0/scrape_schema/fields/nested.py` & `scrape_schema-0.2.2/scrape_schema/fields/nested.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.2.0/scrape_schema/fields/parsel.py` & `scrape_schema-0.2.2/scrape_schema/fields/parsel.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.2.0/scrape_schema/fields/regex.py` & `scrape_schema-0.2.2/scrape_schema/fields/regex.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,17 +95,15 @@
         )
         self.pattern = (
             re.compile(pattern, flags) if isinstance(pattern, str) else pattern
         )
         self.group = group
 
     def _parse(self, markup: str) -> List[str]:
-        if matches := self.pattern.finditer(markup):
-            return [m.group(self.group) for m in matches]
-        return []
+        return [m.group(self.group) for m in self.pattern.finditer(markup)]
 
 
 class ReMatchDict(BaseField):
     def __init__(
         self,
         pattern: Union[str, Pattern],
         flags: Union[int, re.RegexFlag] = 0,
@@ -159,10 +157,8 @@
         self.pattern = (
             re.compile(pattern, flags) if isinstance(pattern, str) else pattern
         )
         if not self.pattern.groupindex:
             raise AttributeError(f"{pattern.pattern} required named groups")  # type: ignore
 
     def _parse(self, markup: str) -> List[Dict[str, str]]:
-        if results := self.pattern.finditer(markup):
-            return [result.groupdict() for result in results]
-        return []
+        return [result.groupdict() for result in self.pattern.finditer(markup)]
```

### Comparing `scrape_schema-0.2.0/scrape_schema/fields/slax.py` & `scrape_schema-0.2.2/scrape_schema/fields/slax.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.2.0/scrape_schema/fields/soup.py` & `scrape_schema-0.2.2/scrape_schema/fields/soup.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.2.0/.gitignore` & `scrape_schema-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.2.0/LICENSE` & `scrape_schema-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.2.0/README.md` & `scrape_schema-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.2.0/pyproject.toml` & `scrape_schema-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -84,21 +84,23 @@
 packages = ["scrape_schema"]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = [
   "scrape_schema/__about__.py",
+  "scrape_schema/factory/__init__.py"
 ]
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
+  "@abstractmethod"
 ]
 
 [tool.mypy]
 python_version = 3.8
 pretty = true
 ignore_missing_imports = true
 exclude = ["env", ".env", "venv", "tests/*", "__pycache__", "examples"]
```

### Comparing `scrape_schema-0.2.0/PKG-INFO` & `scrape_schema-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-schema
-Version: 0.2.0
+Version: 0.2.2
 Summary: A library for converting any text (xml, html, plain text, stdout, etc) to python datatypes
 Project-URL: Documentation, https://github.com/vypivshiy/scrape-schema#readme
 Project-URL: Issues, https://github.com/vypivshiy/scrape-schema/issues
 Project-URL: Source, https://github.com/vypivshiy/scrape-schema
 Project-URL: Examples, https://github.com/vypivshiy/scrape-schema/examples
 Author: vypivshiy
 License-Expression: MIT
```

