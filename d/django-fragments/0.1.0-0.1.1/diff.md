# Comparing `tmp/django_fragments-0.1.0.tar.gz` & `tmp/django_fragments-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_fragments-0.1.0.tar", max compression
+gzip compressed data, was "django_fragments-0.1.1.tar", max compression
```

## Comparing `django_fragments-0.1.0.tar` & `django_fragments-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,18 @@
--rw-r--r--   0        0        0      633 2023-05-09 09:30:28.551190 django_fragments-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-07 21:19:46.006724 django_fragments-0.1.0/django_fragments/__init__.py
--rw-r--r--   0        0        0      163 2023-05-08 11:11:49.135944 django_fragments-0.1.0/django_fragments/apps.py
--rw-r--r--   0        0        0      292 2023-05-07 15:19:00.977243 django_fragments-0.1.0/django_fragments/templates/svg/heroicons_x_mark_mini.html
--rw-r--r--   0        0        0        0 2023-05-07 23:31:34.843055 django_fragments-0.1.0/django_fragments/templatetags/__init__.py
--rw-r--r--   0        0        0     5280 2023-05-09 09:01:43.072723 django_fragments-0.1.0/django_fragments/templatetags/fragments.py
--rw-r--r--   0        0        0     1759 2023-05-09 09:23:25.310001 django_fragments-0.1.0/django_fragments/templatetags/helpers.py
--rw-r--r--   0        0        0     1649 2023-05-09 09:14:25.380285 django_fragments-0.1.0/django_fragments/templatetags/og.py
--rw-r--r--   0        0        0       70 2023-05-08 02:09:45.909742 django_fragments-0.1.0/django_fragments/templatetags/utils/__init__.py
--rw-r--r--   0        0        0     2157 2023-05-08 02:17:55.382358 django_fragments-0.1.0/django_fragments/templatetags/utils/filter_attrs.py
--rw-r--r--   0        0        0     4146 2023-05-08 08:19:35.581999 django_fragments-0.1.0/django_fragments/templatetags/utils/wrap_svg.py
--rw-r--r--   0        0        0     2578 2023-05-09 09:23:49.310432 django_fragments-0.1.0/django_fragments/tests.py
--rw-r--r--   0        0        0     1319 2023-05-09 09:29:41.055088 django_fragments-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1425 1970-01-01 00:00:00.000000 django_fragments-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-05-09 09:45:58.288456 django_fragments-0.1.1/LICENSE
+-rw-r--r--   0        0        0      690 2023-05-09 09:47:26.935180 django_fragments-0.1.1/README.md
+-rw-r--r--   0        0        0       27 2023-05-10 21:50:52.993055 django_fragments-0.1.1/django_fragments/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-08 11:11:49.135944 django_fragments-0.1.1/django_fragments/apps.py
+-rw-r--r--   0        0        0      258 2023-05-10 22:57:17.273819 django_fragments-0.1.1/django_fragments/forms.py
+-rw-r--r--   0        0        0      292 2023-05-07 15:19:00.977243 django_fragments-0.1.1/django_fragments/templates/svg/heroicons_x_mark_mini.html
+-rw-r--r--   0        0        0      132 2023-05-10 22:28:42.950032 django_fragments-0.1.1/django_fragments/templates/test_snippet.html
+-rw-r--r--   0        0        0        0 2023-05-07 23:31:34.843055 django_fragments-0.1.1/django_fragments/templatetags/__init__.py
+-rw-r--r--   0        0        0     5104 2023-05-10 22:52:21.725007 django_fragments-0.1.1/django_fragments/templatetags/fragments.py
+-rw-r--r--   0        0        0     2039 2023-05-09 09:39:46.557198 django_fragments-0.1.1/django_fragments/templatetags/helpers.py
+-rw-r--r--   0        0        0     1649 2023-05-09 09:40:55.305731 django_fragments-0.1.1/django_fragments/templatetags/og.py
+-rw-r--r--   0        0        0       70 2023-05-08 02:09:45.909742 django_fragments-0.1.1/django_fragments/templatetags/utils/__init__.py
+-rw-r--r--   0        0        0     2157 2023-05-08 02:17:55.382358 django_fragments-0.1.1/django_fragments/templatetags/utils/filter_attrs.py
+-rw-r--r--   0        0        0     4146 2023-05-08 08:19:35.581999 django_fragments-0.1.1/django_fragments/templatetags/utils/wrap_svg.py
+-rw-r--r--   0        0        0     4919 2023-05-10 22:57:26.892872 django_fragments-0.1.1/django_fragments/tests.py
+-rw-r--r--   0        0        0      424 2023-05-10 23:01:29.088719 django_fragments-0.1.1/django_fragments/utils.py
+-rw-r--r--   0        0        0     1406 2023-05-10 23:01:21.957208 django_fragments-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1482 1970-01-01 00:00:00.000000 django_fragments-0.1.1/PKG-INFO
```

### Comparing `django_fragments-0.1.0/README.md` & `django_fragments-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # django-fragments
 
 ![Github CI](https://github.com/justmars/django-fragments/actions/workflows/main.yml/badge.svg)
 
 ## Purpose
 
-Used for partial template rendering of: `<input>`, `<svg>` tags for a Django [boilerplate](https://start-django.fly.dev)
+Used for partial template rendering of: `<input>`, `<svg>` tags. Originally for a Django [boilerplate](https://start-django.fly.dev), refactored out into an independent library.
 
 ## Setup
 
 After installation, e.g. `pip install django-fragments`
 
 ```py
 INSTALLED_APPS = [
```

### Comparing `django_fragments-0.1.0/django_fragments/templatetags/fragments.py` & `django_fragments-0.1.1/django_fragments/templatetags/fragments.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 def md(text: str, exts: list[str] = ["attr_list"]) -> SafeText:
     """Convert a text in markdown to its html equivalent using specific extensions."""
     return mark_safe(markdown(text, extensions=exts))
 
 
 @register.simple_tag
 def curr(lhs: str, reversible: str) -> SafeText:
-    """Set `aria-current` as an attribute by comparing a `lhs` path with reverse of `rhs`
-    path.
+    """Returns a string `aria-current` for use as an attribute when `lhs` path matches the
+    `reversible` value that will be passed to the `django.urls.reverse()`.
 
     Args:
         lhs (str): lhs stands for lefthand side, should be first positional element in the tag
         reversible (str): The value will be passed to the `django.urls.reverse()` without args, kwargs
 
     Returns:
         SafeText: The text "aria-current=page" if a match occurs, otherwise ""
@@ -44,15 +44,15 @@
     css: str | None = None,
     request: HttpRequest | None = None,
 ) -> SafeText:
     """HTML fragment: `<a>` tag for desktop/mobile navbar links.
 
     Checks if link represented by reverse name url `reversible` is the _current_ path via the request, if it is provided.
 
-    In the latter case, on match of the `request.path` to the `reversible`, add "aria-current=true"
+    In the latter case, on match of the `request.path` to the `reversible`, add `aria-current=true`
 
     Args:
         reversible (str): The value will be passed to the `django.urls.reverse()` function without keyword arguments
         text (str | None, optional): The text to incude within the anchor element, if any. Defaults to None.
         css (str | None, optional): If provided, will populate the `class` attribute of the anchor element. Defaults to None.
         request (HttpRequest | None, optional): The django http request object to ascertain the present path of the request. Defaults to None.
 
@@ -65,21 +65,14 @@
         url=reverse(reversible),
         css=css,
         aria=curr(request.path, reversible) if request else "",
     )
 
 
 @register.simple_tag
-def attrize(d: dict) -> SafeText:
-    """Unpack a dictionary as attributes, useful for adding attributes to
-    an existing tag."""
-    return mark_safe(" ".join([f'{k}="{v}"' for k, v in d.items()]))
-
-
-@register.simple_tag
 def icon(
     name: str,
     prefix: str = settings.FRAGMENTS.get("icons_prefix"),
     folder: Path = settings.FRAGMENTS.get("icons_path"),
     css: str | None = None,
     **kwargs,
 ) -> SafeText:
@@ -106,27 +99,25 @@
 def input(bound: Field, kls: str, label_kls: str | None = None) -> SafeText:
     """Can likely replace this with prospective Django 5.0's
     `django.forms.BoundField.as_field_group`"""
     return mark_safe(
         Template("""
             {% load fragments %}
             {% whitespaceless %}
-            <div class="{{kls}}">
-                <label for="{{bound.id_for_label}}"
-                    {% if label_kls %}class="{{label_kls}}"{% endif %}>
+            <div class="{{ kls }}
+                data-hidden="{{ bound.is_hidden}}"
+                data-widget="{{ bound.widget_type }}"
+            >
+                {{ bound.errors }}
+                <label for="{{ bound.id_for_label }}"
+                    {% if label_kls %}class="{{ label_kls }}"{% endif %}>
                     {{bound.label}}
                 </label>
-                {{bound}}
-                {% if bound.errors %}
-                    {{ bound.errors }}
-                {% else %}
-                    <p class="help">
-                    {{ bound.help_text }}
-                    </p>
-                {% endif %}
+                {{ bound }}
+                <p class="help">{{ bound.help_text }}</p>
             </div>
             {% endwhitespaceless %}
             """)  # noqa: E501
         .render(
             context=Context(
                 {
                     "bound": bound,
```

### Comparing `django_fragments-0.1.0/django_fragments/templatetags/helpers.py` & `django_fragments-0.1.1/django_fragments/templatetags/helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 import re
 
 from django import template
 from django.utils.functional import keep_lazy_text
+from django.utils.safestring import SafeText, mark_safe
 
 from .fragments import register
 
 
+@register.simple_tag
+def attrize(d: dict) -> SafeText:
+    """Unpack a dictionary as attributes, useful for adding attributes to
+    an existing tag."""
+    return mark_safe(" ".join([f'{k}="{v}"' for k, v in d.items()]))
+
+
 @keep_lazy_text
 def strip_whitespace(value):
     """
     See https://stackoverflow.com/a/72942459 answer by [Will Gordon](https://stackoverflow.com/users/6758654/will-gordon)
     Return the given HTML with any newlines, duplicate whitespace, or trailing spaces are removed.
     """  # noqa: E501
     # Process duplicate whitespace occurrences or
```

### Comparing `django_fragments-0.1.0/django_fragments/templatetags/og.py` & `django_fragments-0.1.1/django_fragments/templatetags/og.py`

 * *Files identical despite different names*

### Comparing `django_fragments-0.1.0/django_fragments/templatetags/utils/filter_attrs.py` & `django_fragments-0.1.1/django_fragments/templatetags/utils/filter_attrs.py`

 * *Files identical despite different names*

### Comparing `django_fragments-0.1.0/django_fragments/templatetags/utils/wrap_svg.py` & `django_fragments-0.1.1/django_fragments/templatetags/utils/wrap_svg.py`

 * *Files identical despite different names*

### Comparing `django_fragments-0.1.0/pyproject.toml` & `django_fragments-0.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "django-fragments"
 description = "Custom template tags for common html idioms in Django."
-version = "0.1.0"
+version = "0.1.1"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/django-fragments"
 documentation = "https://mv3.dev/django-fragments"
 classifiers = [
   "Programming Language :: Python :: 3.11",
@@ -29,21 +29,24 @@
 mkdocs = "^1.4"
 mkdocstrings = { extras = ["python"], version = "^0.20.0" }
 mkdocs-material = "^9.1"
 ipykernel = "^6.22.0"
 
 [tool.pytest.ini_options]
 minversion = "7.3"
-addopts = "-ra -q --ds=config.settings --doctest-modules --cov"
+addopts = "-ra -q -vv --ds=config.settings --doctest-modules --cov"
 filterwarnings = [
   "ignore::DeprecationWarning", # DeprecationWarning: pkg_resources is deprecated as an API
 ]
-testpaths = ["fragments", "fragments/tests.py"]
+testpaths = ["django_fragments", "django_fragments/tests.py"]
 
 [tool.ruff]
 ignore = ["F401", "F403"]
 fixable = ["F", "E", "W", "I001"]
 select = ["F", "E", "W", "I001"]
 
+[tool.ruff.per-file-ignores]
+"django_fragments/tests.py" = ["E501"]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django_fragments-0.1.0/PKG-INFO` & `django_fragments-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-fragments
-Version: 0.1.0
+Version: 0.1.1
 Summary: Custom template tags for common html idioms in Django.
 Home-page: https://mv3.dev
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
@@ -21,15 +21,15 @@
 
 # django-fragments
 
 ![Github CI](https://github.com/justmars/django-fragments/actions/workflows/main.yml/badge.svg)
 
 ## Purpose
 
-Used for partial template rendering of: `<input>`, `<svg>` tags for a Django [boilerplate](https://start-django.fly.dev)
+Used for partial template rendering of: `<input>`, `<svg>` tags. Originally for a Django [boilerplate](https://start-django.fly.dev), refactored out into an independent library.
 
 ## Setup
 
 After installation, e.g. `pip install django-fragments`
 
 ```py
 INSTALLED_APPS = [
```

