# Comparing `tmp/scrape_schema-0.1.4.tar.gz` & `tmp/scrape_schema-0.2.0.tar.gz`

## Comparing `scrape_schema-0.1.4.tar` & `scrape_schema-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/__init__.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/_base_configs.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/_logger.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/_type_caster.py
--rw-r--r--   0        0        0    20804 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/base.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/exceptions.py
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/callbacks/__init__.py
--rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/callbacks/parsel.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/callbacks/slax.py
--rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/callbacks/soup.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/factory/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/fields/__init__.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/fields/mock.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/fields/nested.py
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/fields/parsel.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/fields/regex.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/fields/slax.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/fields/soup.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/LICENSE
--rw-r--r--   0        0        0     5882 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/README.md
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     8151 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/__init__.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/_base_configs.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/_logger.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/_type_caster.py
+-rw-r--r--   0        0        0    21507 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/base.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/exceptions.py
+-rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/hooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/callbacks/__init__.py
+-rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/callbacks/parsel.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/callbacks/slax.py
+-rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/callbacks/soup.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/factory/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/fields/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/fields/mock.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/fields/nested.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/fields/parsel.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/fields/regex.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/fields/slax.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/scrape_schema/fields/soup.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5911 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/README.md
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8204 2020-02-02 00:00:00.000000 scrape_schema-0.2.0/PKG-INFO
```

### Comparing `scrape_schema-0.1.4/scrape_schema/_base_configs.py` & `scrape_schema-0.2.0/scrape_schema/_base_configs.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.4/scrape_schema/_type_caster.py` & `scrape_schema-0.2.0/scrape_schema/_type_caster.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,40 +22,40 @@
     def cast(self, type_hint: Type, value: Any) -> Any:
         if sys.version_info >= (3, 9):
             type_hint = self._typing_to_builtin(type_hint)
 
         origin = get_origin(type_hint)
         args = get_args(type_hint)
         logger.info(
-            "`%s` Cast type start. `value=%s`, type_annotation=%s, `origin=%s`, `args=%s`",
+            "`{}` Cast type start. `value={}`, type_annotation={}, `origin={}`, `args={}`",
             self.__class__.__name__,
             value,
             type_hint,
             origin,
             args,
         )
         # None
         if value is None and type_hint is not bool:
             return value
 
         if origin is not None and args:
             # list
             if origin is list:
                 logger.debug(
-                    "List cast %s -> arg=%s, value=%s",
+                    "List cast {} -> arg={}, value={}",
                     self.__class__.__name__,
                     args[0],
                     value,
                 )
                 return [self.cast(type_hint=args[0], value=v) for v in value]
             # dict
             elif origin is dict:
                 key_type, value_type = args
                 logger.debug(
-                    "Dict cast %s -> key=%s, value=%s  `%s`",
+                    "Dict cast {} -> key={}, value={}  `{}`",
                     self.__class__.__name__,
                     key_type.__name__,
                     value_type.__name__,
                     value,
                 )
                 return {
                     self.cast(type_hint=key_type, value=k): self.cast(
@@ -63,25 +63,25 @@
                     )
                     for k, v in value.items()
                 }
             # Optional
             elif origin is Union:
                 if value is None and NoneType in args:
                     logger.debug(
-                        "Optional cast %s -> %s", self.__class__.__name__, value
+                        "Optional cast {} -> {}", self.__class__.__name__, value
                     )
                     return None
                 # in python3.8 raise TypeError: issubclass() arg 1 must be a class
                 # example _cast_type(Optional[List[int]], [])
                 non_none_args = [arg for arg in args if arg is not NoneType]
                 if len(non_none_args) == 1:
                     return self.cast(type_hint=non_none_args[0], value=value)
         # bool cast
         elif type_hint is bool:
-            logger.debug("Cast %s `%s()` -> bool", self.__class__.__name__, value)
+            logger.debug("Cast {} `{}()` -> bool", self.__class__.__name__, value)
             return bool(value)
         else:
             # direct cast
             logger.debug(
-                "Cast `%s` := `%s(%s)`", self.__class__.__name__, type_hint, value
+                "Cast `{}` := `{}({})`", self.__class__.__name__, type_hint, value
             )
             return type_hint(value)
```

### Comparing `scrape_schema-0.1.4/scrape_schema/base.py` & `scrape_schema-0.2.0/scrape_schema/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,15 +134,15 @@
     def extract(self, markup: MARKUP_TYPE, *, type_: Optional[Type] = None) -> Any:
         """parse markup without BaseSchema Instance
 
         :param markup: string target
         :param type_: optional type for type-casting
         """
         logger.info(
-            "%s[%s] start extract value. Field attrs: factory=%s, callback=%s, filter_=%s, default=%s",
+            "{}[{}] start extract value. Field attrs: factory={}, callback={}, filter_={}, default={}",
             self.__class__.__name__,
             self.Config.parser or "str",
             repr(self.factory),
             repr(self.callback),
             repr(self.filter_),
             self.default,
         )
@@ -150,73 +150,73 @@
             raise TypeError(
                 f"markup argument excepted {self.Config.parser.__name__} "
                 f"not {type(markup).__name__}"
             )
         value = self._parse(markup)
         if not value:
             logger.debug(
-                "%s.extract value not found, set default `%s` value",
+                "{}.extract value not found, set default `{}` value",
                 self.__class__.__name__,
                 self.default,
             )
             value = self.default
         if self._is_iterable_and_not_string_value(value):
             if self.filter_:
-                logger.debug("%s.extract `filter_(%s)`", self.__class__.__name__, value)
+                logger.debug("{}.extract `filter_({})`", self.__class__.__name__, value)
             value = self._filter(value)
         if self.callback:
-            logger.debug("%s.extract `callback(%s)`", self.__class__.__name__, value)
+            logger.debug("{}.extract `callback({})`", self.__class__.__name__, value)
             value = self._callback(value)
         if self.factory:
-            logger.debug("%s.extract `factory(%s)`", self.__class__.__name__, value)
+            logger.debug("{}.extract `factory({})`", self.__class__.__name__, value)
             value = self._factory(value)
         elif type_:
             value = self._type_caster.cast(type_, value)
         logger.info(
-            "%s.extract return `%s[%s]`",
+            "{}.extract return `{}[{}]`",
             self.__class__.__name__,
             value,
             type(value).__name__,
         )
         return value
 
     def __call__(self, instance: "BaseSchema", name: str, markup: MARKUP_TYPE) -> Any:
         """parser entrypoint inside a BaseSchema object"""
         logger.info(
-            "%s.%s[%s]: Field attrs: factory=%s, callback=%s, filter_=%s, default=%s",
+            "{}.{}[{}]: Field attrs: factory={}, callback={}, filter_={}, default={}",
             instance.__schema_name__,
             name,
             self.Config.parser or "str",
             repr(self.factory),
             repr(self.callback),
             repr(self.filter_),
             self.default,
         )
         value = self._parse(markup)
         if not value:
             logger.debug(
-                "%s.%s: value is %s, set default `%s`",
+                "{}.{}: value is {}, set default `{}`",
                 instance.__schema_name__,
                 name,
                 value,
                 self.default,
             )
             value = self.default
         else:
             logger.debug(
-                "%s.%s := %s raw value(s)", instance.__schema_name__, name, value
+                "{}.{} := {} raw value(s)", instance.__schema_name__, name, value
             )
 
         value = self._filter(value, schema_instance=instance, name=name)
         value = self._callback(value, schema_instance=instance, name=name)
         if self.factory or self.Config.hooks.get_factory(name):
             value = self._factory(value, schema_instance=instance, name=name)
         else:
             value = self._typing(instance, name, value)
-        logger.info("%s.%s = `%s` Done", instance.__class__.__name__, name, value)
+        logger.info("{}.{} = `{}` Done", instance.__class__.__name__, name, value)
         return value
 
     def _filter(
         self,
         value: T,
         *,
         schema_instance: Optional["BaseSchema"] = None,
@@ -239,15 +239,15 @@
                 )
                 filter_ = self.filter_ or hook
         else:
             filter_ = self.filter_
 
         if filter_ and self._is_iterable_and_not_string_value(value):
             logger.debug(
-                "%s.%s := filter_(%s)",
+                "{}.{} := filter_({})",
                 schema_instance.__schema_name__
                 if schema_instance
                 else self.__class__.__name__,
                 name or "extract",
                 value,
             )
             if isinstance(value, list):
@@ -279,15 +279,15 @@
                     f"{schema_instance.__schema_name__}.{name}"
                 )
                 factory = self.factory or hook
         else:
             factory = self.factory
         if factory:
             logger.debug(
-                "%s.%s := factory(%s)",
+                "{}.{} := factory({})",
                 schema_instance.__schema_name__
                 if schema_instance
                 else self.__class__.__name__,
                 name or "extract",
                 value,
             )
         return factory(value) if factory else value
@@ -317,15 +317,15 @@
                 callback = self.callback or hook
         else:
             callback = self.callback
 
         if not callback:
             return value
         logger.debug(
-            "%s.%s := callback(%s)",
+            "{}.{} := callback({})",
             schema_instance.__schema_name__
             if schema_instance
             else self.__class__.__name__,
             name or "extract",
             value,
         )
         if not self._is_iterable_and_not_string_value(value):
@@ -482,57 +482,57 @@
                 f"[{fails_counter}] Failed parse `{self.__class__.__name__}.{attr_name}` "
                 f"by {field.__class__.__name__} field, set `{value}`.",
                 stacklevel=2,
                 category=RuntimeWarning,
             )
 
             logger.warning(
-                "[%i] Failed parse `%s.%s` by `%s`, set `%s`",
+                "[{}] Failed parse `{}.{}` by `{}`, set `{}`",
                 fails_counter,
                 self.__class__.__name__,
                 attr_name,
                 field.__class__.__name__,
                 value,
             )
 
             if fails_counter > self.Config.fails_attempt:
                 raise ParseFailAttemptsError(
                     f"{fails_counter} of {len(self.__schema_fields__.keys())} "
                     "fields failed parse."
                 )
         logger.debug(
-            "`%s.%s[%s] = %s`",
+            "`{}.{}[{}] = {}`",
             self.__class__.__name__,
             attr_name,
             field.__class__.__name__,
             value,
         )
         return fails_counter
 
     def __init_fields__(self, markup: str) -> None:
         """
         :param str markup: text target
         """
         _parsers: Dict[Type[Any], Any] = {}
         _fails_counter = 0
         logger.info(
-            "Start parse `%s`. Fields count: %i",
+            "Start parse `{}`. Fields count: {}",
             self.__schema_name__,
             len(self.__schema_fields__.keys()),
         )
 
         for name, fields in self.__schema_fields__.items():
             field, value = self._parse_field_value(
                 cached_parsers=_parsers, name=name, _fields=fields, markup=markup
             )
             _fails_counter = self._calculate_attempt_parse_errors(
                 fails_counter=_fails_counter, field=field, attr_name=name, value=value
             )
             setattr(self, name, value)
-        logger.debug("%s done! Fields fails: %i", self.__schema_name__, _fails_counter)
+        logger.debug("{} done! Fields fails: {}", self.__schema_name__, _fails_counter)
 
     def __init__(self, markup: str, *, parse_markup: bool = True, **kwargs):
         """
         :param markup: markup string target
         :param parse_markup: parse field markups. Default True
         :param kwargs: any kwargs attrs
         """
@@ -586,42 +586,62 @@
         """
         if kwargs.get("parse_markup"):
             kwargs.pop("parse_markup")
 
         return cls("", parse_markup=False, **kwargs)
 
     @staticmethod
-    def _to_dict(value: Union["BaseSchema", list, Dict]):
+    def _to_dict(value: Union["BaseSchema", List, Dict, Any]):
         if isinstance(value, BaseSchema):
             return value.dict()
 
         elif isinstance(value, list):
             if all(isinstance(val, BaseSchema) for val in value):
                 return [val.dict() for val in value]
 
         elif isinstance(value, dict):
             if all(isinstance(val, BaseSchema) for val in value.values()):
                 return {k: v.dict() for k, v in value.items()}
         return value
 
-    def dict(self) -> Dict[str, Any]:
+    def raw_dict(self) -> Dict[str, Any]:
         """convert schema object to python dict"""
-        return {
-            k: self._to_dict(v)
-            for k, v in self.__dict__.items()
-            if not k.startswith("_") and k != "Config"
+        return {k: self._to_dict(v) for k, v in self.__dict__.items() if k != "Config"}
+
+    def dict(self) -> Dict[str, Any]:
+        # parse properties
+        result: Dict[str, Any] = {
+            k: getattr(self, k)
+            for k, v in self.__class__.__dict__.items()
+            if isinstance(v, property)
         }
+        # parse public field keys
+        for k, v in self.__dict__.items():
+            if not k.startswith("_") and self.__schema_fields__.get(k):
+                result[k] = self._to_dict(v)
+        return result
 
     def __repr_args__(self) -> List[str]:
+        # parse properties
+
+        args: Dict[str, Any] = {
+            k: getattr(self, k)
+            for k, v in self.__class__.__dict__.items()
+            if isinstance(v, property)
+        }
+        # parse public field keys
+        for k, v in self.__dict__.items():
+            if not k.startswith("_") and self.__schema_fields__.get(k):
+                args[k] = v
+
         return [
             f"{k}={repr(v)}"
             if isinstance(v, BaseSchema)
             else f"{k}:{type(v).__name__}={repr(v)}"
-            for k, v in self.__dict__.items()
-            if not k.startswith("_") and k != "Config"
+            for k, v in args.items()
         ]
 
     def __repr__(self):
         return f'{self.__schema_name__}({", ".join(self.__repr_args__())})'
 
     @property
     def __schema_name__(self) -> str:
```

### Comparing `scrape_schema-0.1.4/scrape_schema/hooks.py` & `scrape_schema-0.2.0/scrape_schema/hooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from typing import Any, Callable, Dict, KeysView, Optional, Tuple, TypedDict, Union
 
 from scrape_schema._logger import logger
 
 __all__ = ["FieldHook", "FieldHookList", "HooksStorage"]
 
 
@@ -26,14 +27,20 @@
 
     __callback_hooks__: Dict[str, Optional[Callable]] = {}
     __factory_hooks__: Dict[str, Optional[Callable]] = {}
     __filter_hooks__: Dict[str, Optional[Callable]] = {}
     __field_hooks__: Dict[str, Union[FieldHook, FieldHookList]] = {}
 
     def __new__(cls):
+        warnings.warn(
+            stacklevel=0,
+            category=DeprecationWarning,
+            message="HooksStorage will be deleted in next updates, use @property decorators in BaseSchema "
+            "classes",
+        )
         if cls._instance is None:
             cls._instance = super().__new__(cls)
         return cls._instance
 
     @staticmethod
     def _register_hook(
         hooks_dict: Dict[str, Optional[Callable]],
@@ -47,41 +54,41 @@
     def on_filter(self, *attrs_names: str):
         """add filter param for attr names in schemas
 
         :param attrs_names: schema attribute names
         """
 
         def decorator(func):
-            logger.debug("Register `on_filter` hook: %s %s", attrs_names, func)
+            logger.debug("Register `on_filter` hook: {} {}", attrs_names, func)
             self._register_hook(self.__filter_hooks__, attrs_names, func)
             return func
 
         return decorator
 
     def on_factory(self, *attrs_names: str):
         """add factory param for attr names in schemas
 
         :param attrs_names: schema attribute names
         """
 
         def decorator(func):
-            logger.debug("Register `on_factory` hook: %s %s", attrs_names, func)
+            logger.debug("Register `on_factory` hook: {} {}", attrs_names, func)
             self._register_hook(self.__factory_hooks__, attrs_names, func)
             return func
 
         return decorator
 
     def on_callback(self, *attrs_names: str):
         """add callback param for attr names in schemas
 
         :param attrs_names: schema attribute names
         """
 
         def decorator(func):
-            logger.debug("Register on_callback hook: %s %s", attrs_names, func)
+            logger.debug("Register on_callback hook: {} {}", attrs_names, func)
             self._register_hook(self.__callback_hooks__, attrs_names, func)
             return func
 
         return decorator
 
     def get_callback(self, name: str) -> Optional[Callable]:
         """get callback by name. if not contains - return None"""
@@ -93,28 +100,28 @@
 
     def get_factory(self, name: str) -> Optional[Callable]:
         """get factory by name. if not contains - return None"""
         return self.__factory_hooks__.get(name)
 
     def add_hook(self, name: str, hook: Union[FieldHook, FieldHookList]):
         """add FieldHook or FieldHookList in storage."""
-        logger.debug("Add `%s` %s", name, hook)
+        logger.debug("Add `{}` {}", name, hook)
         self.__field_hooks__[name] = hook
 
     def add_kwargs_hook(
         self,
         name: str,
         default: Optional[Any] = None,
         callback: Optional[Callable] = None,
         filter_: Optional[Callable] = None,
         factory: Optional[Callable] = None,
     ):
         """create hook by keyword arguments and add in storage."""
         logger.debug(
-            "Add `%s` FieldHook. Arguments: default=%s, callback=%s, filter_=%s, factory=%s",
+            "Add `{}` FieldHook. Arguments: default={}, callback={}, filter_={}, factory={}",
             name,
             default,
             callback,
             filter_,
             factory,
         )
 
@@ -127,15 +134,15 @@
             default=default, callback=callback, factory=factory
         )
         return
 
     def get_hook(self, name: str) -> Union[FieldHook, FieldHookList]:
         """return stored hook. If not founded key - return empty dict"""
         if hook := self.__field_hooks__.get(name):
-            logger.debug("Get hook %s. Values: %s", name, hook)
+            logger.debug("Get hook {}. Values: {}", name, hook)
             return hook
-        logger.debug("Not contains hook in `%s` key. Return empty dict", name)
+        logger.debug("Not contains hook in `{}` key. Return empty dict", name)
         return {}
 
     def hook_keys(self) -> KeysView[str]:
         """get all hook keys"""
         return self.__field_hooks__.keys()
```

### Comparing `scrape_schema-0.1.4/scrape_schema/callbacks/parsel.py` & `scrape_schema-0.2.0/scrape_schema/callbacks/parsel.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.4/scrape_schema/callbacks/slax.py` & `scrape_schema-0.2.0/scrape_schema/callbacks/slax.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.4/scrape_schema/callbacks/soup.py` & `scrape_schema-0.2.0/scrape_schema/callbacks/soup.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.4/scrape_schema/fields/mock.py` & `scrape_schema-0.2.0/scrape_schema/fields/mock.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.4/scrape_schema/fields/nested.py` & `scrape_schema-0.2.0/scrape_schema/fields/nested.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Nested fields for create BaseSchema objects"""
 from typing import Any, Callable, List, Optional, Type, Union
 
+from scrape_schema._logger import logger
+
 from ..base import BaseField, BaseSchema  # type: ignore
 
 __all__ = ["BaseNested", "Nested", "NestedList"]
 
 
 class BaseNested(BaseField):
     def _parse(self, _: str) -> str:
@@ -28,18 +30,29 @@
         super().__init__(factory=factory)
         self._schema = schema
         self.crop_rule = crop_rule
 
     def __call__(
         self, instance: BaseSchema, name: str, markup: str
     ) -> Union[BaseSchema, Any]:
+        logger.info(
+            "{}.{} start extract value. Field attrs: schema={}, crop_rule={}, factory={}",
+            instance.__schema_name__,
+            self._schema.__name__,
+            self.crop_rule,
+            self.factory,
+        )
         markup = self._parse(markup)
         value = self._schema.from_crop_rule(markup, crop_rule=self.crop_rule)
+        logger.debug("{}.{} create schema: {}", instance.__schema_name__, name, value)
         return self._factory(value)
 
+    def extract(self, markup: Any, *, type_: Optional[Type] = None) -> None:
+        raise NotImplementedError("Method `extract` not allowed in Nested field")
+
 
 class NestedList(BaseNested):
     def __init__(
         self,
         schema: Type[BaseSchema],
         *,
         crop_rule: Callable[[str], List[str]],
@@ -55,10 +68,21 @@
         self.crop_rule = crop_rule
         self._schema = schema
         self.crop_rule = crop_rule
 
     def __call__(
         self, instance: BaseSchema, name: str, markup: str
     ) -> Union[List[BaseSchema], Any]:
+        logger.info(
+            "{}.{} start extract value. Field attrs: schema={}, crop_rule={}, factory={}",
+            instance.__schema_name__,
+            self._schema.__name__,
+            self.crop_rule,
+            self.factory,
+        )
         markup = self._parse(markup)
         value = self._schema.from_crop_rule_list(markup, crop_rule=self.crop_rule)
+        logger.debug("{}.{} create schemas: {}", instance.__schema_name__, name, value)
         return self._factory(value)
+
+    def extract(self, markup: Any, *, type_: Optional[Type] = None) -> None:
+        raise NotImplementedError("Method `extract` not allowed in NestedList field")
```

### Comparing `scrape_schema-0.1.4/scrape_schema/fields/parsel.py` & `scrape_schema-0.2.0/scrape_schema/fields/parsel.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.4/scrape_schema/fields/regex.py` & `scrape_schema-0.2.0/scrape_schema/fields/regex.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.4/scrape_schema/fields/slax.py` & `scrape_schema-0.2.0/scrape_schema/fields/slax.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.4/scrape_schema/fields/soup.py` & `scrape_schema-0.2.0/scrape_schema/fields/soup.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.4/.gitignore` & `scrape_schema-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.4/LICENSE` & `scrape_schema-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.4/README.md` & `scrape_schema-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -134,36 +134,40 @@
 lorem upsum dolor
 192.168.0.1
 """
 
 
 class Schema(BaseSchema):
     ipv4: ScField[str, ReMatch(r"(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})")]
-    max_digit: ScField[int, ReMatchList(r"(\d+)",
-                                          callback=int,                                      
-                                          factory=max)]
     failed_value: ScField[bool, ReMatchList(r"(ora)", default=False)]
     digits: ScField[List[int], ReMatchList(r"(\d+)")]
     digits_float: ScField[List[float], ReMatchList(r"(\d+)", 
                                                      callback=lambda s: f"{s}.5")]
     words_lower: ScField[List[str], ReMatchList(r"([a-z]+)")]
     words_upper: ScField[List[str], ReMatchList(r"([A-Z]+)")]
     
+    @property
+    def max_digit(self) -> int:
+        return max(self.digits)
+    
+    @property
+    def all_words(self) -> List[str]:
+        return self.words_lower + self.words_upper
+    
 if __name__ == '__main__':
     schema = Schema(TEXT)
-    pprint.pprint(schema.dict(), width=48, compact=True)
-    # {'digits': [10, 20, 192, 168, 0, 1],
-    #  'digits_float': [10.5, 20.5, 192.5, 168.5, 0.5,
-    #                   1.5],
+    pprint.pprint(schema.dict(), compact=True)
+    # {'all_words': ['banana', 'potato', 'foo', 'bar', 'lorem', 'upsum', 'dolor',
+    #           'BANANA', 'POTATO'],
+    #  'digits': [10, 20, 192, 168, 0, 1],
+    #  'digits_float': [10.5, 20.5, 192.5, 168.5, 0.5, 1.5],
     #  'failed_value': False,
-    #  'ip_v4': '192.168.0.1',
+    #  'ipv4': '192.168.0.1',
     #  'max_digit': 192,
-    #  'words_lower': ['banana', 'potato', 'foo',
-    #                  'bar', 'lorem', 'upsum',
-    #                  'dolor'],
+    #  'words_lower': ['banana', 'potato', 'foo', 'bar', 'lorem', 'upsum', 'dolor'],
     #  'words_upper': ['BANANA', 'POTATO']}
 ```
 
 _____
 # logging
 In this project, logging to the `DEBUG` level is enabled by default.
```

### Comparing `scrape_schema-0.1.4/pyproject.toml` & `scrape_schema-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,17 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Topic :: Internet",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Text Processing"
 ]
 dependencies = [
-'typing_extensions; python_version < "3.11"']
+  'colorama',
+  'typing_extensions; python_version < "3.11"'
+]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/vypivshiy/scrape-schema#readme"
 Issues = "https://github.com/vypivshiy/scrape-schema/issues"
 Source = "https://github.com/vypivshiy/scrape-schema"
 Examples = "https://github.com/vypivshiy/scrape-schema/examples"
@@ -53,14 +55,15 @@
 
 [tool.hatch.envs.docs.scripts]
 build = "mkdocs build --clean --strict"
 serve = "mkdocs serve --dev-addr localhost:8000"
 
 [tool.hatch.envs.default]
 dependencies = [
+  "colorama",
   "pytest",
   "selectolax",
   "bs4",
   "parsel",
   "pytest-cov"
 ]
 
@@ -101,10 +104,11 @@
 exclude = ["env", ".env", "venv", "tests/*", "__pycache__", "examples"]
 files = "scrape_schema/*.py,scrape_schema/fields/*.py,scrape_schema/callbacks/*.py"
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "error",
     'ignore::RuntimeWarning',
+    'ignore::DeprecationWarning'
 ]
```

### Comparing `scrape_schema-0.1.4/PKG-INFO` & `scrape_schema-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-schema
-Version: 0.1.4
+Version: 0.2.0
 Summary: A library for converting any text (xml, html, plain text, stdout, etc) to python datatypes
 Project-URL: Documentation, https://github.com/vypivshiy/scrape-schema#readme
 Project-URL: Issues, https://github.com/vypivshiy/scrape-schema/issues
 Project-URL: Source, https://github.com/vypivshiy/scrape-schema
 Project-URL: Examples, https://github.com/vypivshiy/scrape-schema/examples
 Author: vypivshiy
 License-Expression: MIT
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.8
+Requires-Dist: colorama
 Requires-Dist: typing-extensions; python_version < '3.11'
 Provides-Extra: all
 Requires-Dist: bs4; extra == 'all'
 Requires-Dist: parsel; extra == 'all'
 Requires-Dist: selectolax; extra == 'all'
 Provides-Extra: bs4
 Requires-Dist: bs4; extra == 'bs4'
@@ -191,36 +192,40 @@
 lorem upsum dolor
 192.168.0.1
 """
 
 
 class Schema(BaseSchema):
     ipv4: ScField[str, ReMatch(r"(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})")]
-    max_digit: ScField[int, ReMatchList(r"(\d+)",
-                                          callback=int,                                      
-                                          factory=max)]
     failed_value: ScField[bool, ReMatchList(r"(ora)", default=False)]
     digits: ScField[List[int], ReMatchList(r"(\d+)")]
     digits_float: ScField[List[float], ReMatchList(r"(\d+)", 
                                                      callback=lambda s: f"{s}.5")]
     words_lower: ScField[List[str], ReMatchList(r"([a-z]+)")]
     words_upper: ScField[List[str], ReMatchList(r"([A-Z]+)")]
     
+    @property
+    def max_digit(self) -> int:
+        return max(self.digits)
+    
+    @property
+    def all_words(self) -> List[str]:
+        return self.words_lower + self.words_upper
+    
 if __name__ == '__main__':
     schema = Schema(TEXT)
-    pprint.pprint(schema.dict(), width=48, compact=True)
-    # {'digits': [10, 20, 192, 168, 0, 1],
-    #  'digits_float': [10.5, 20.5, 192.5, 168.5, 0.5,
-    #                   1.5],
+    pprint.pprint(schema.dict(), compact=True)
+    # {'all_words': ['banana', 'potato', 'foo', 'bar', 'lorem', 'upsum', 'dolor',
+    #           'BANANA', 'POTATO'],
+    #  'digits': [10, 20, 192, 168, 0, 1],
+    #  'digits_float': [10.5, 20.5, 192.5, 168.5, 0.5, 1.5],
     #  'failed_value': False,
-    #  'ip_v4': '192.168.0.1',
+    #  'ipv4': '192.168.0.1',
     #  'max_digit': 192,
-    #  'words_lower': ['banana', 'potato', 'foo',
-    #                  'bar', 'lorem', 'upsum',
-    #                  'dolor'],
+    #  'words_lower': ['banana', 'potato', 'foo', 'bar', 'lorem', 'upsum', 'dolor'],
     #  'words_upper': ['BANANA', 'POTATO']}
 ```
 
 _____
 # logging
 In this project, logging to the `DEBUG` level is enabled by default.
```

