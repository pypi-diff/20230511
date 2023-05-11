# Comparing `tmp/django-async-orm-0.1.8.tar.gz` & `tmp/django-async-orm-0.1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-async-orm-0.1.8.tar", max compression
+gzip compressed data, was "django-async-orm-0.1.8.1.tar", max compression
```

## Comparing `django-async-orm-0.1.8.tar` & `django-async-orm-0.1.8.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1066 2021-05-23 07:16:12.859441 django-async-orm-0.1.8/LICENSE
--rw-r--r--   0        0        0     4704 2021-05-27 18:50:28.537742 django-async-orm-0.1.8/README.md
--rw-r--r--   0        0        0        0 2021-05-23 07:07:34.301758 django-async-orm-0.1.8/django_async_orm/__init__.py
--rw-r--r--   0        0        0      340 2021-05-24 06:36:34.837623 django-async-orm-0.1.8/django_async_orm/apps.py
--rw-r--r--   0        0        0      355 2021-05-24 07:01:52.476066 django-async-orm-0.1.8/django_async_orm/iter.py
--rw-r--r--   0        0        0      174 2021-05-23 09:54:11.642083 django-async-orm-0.1.8/django_async_orm/manager.py
--rw-r--r--   0        0        0     6578 2021-05-27 20:37:47.469044 django-async-orm-0.1.8/django_async_orm/query.py
--rw-r--r--   0        0        0      934 2021-05-29 10:24:53.070567 django-async-orm-0.1.8/django_async_orm/utils.py
--rw-r--r--   0        0        0      684 2021-05-23 11:24:51.726987 django-async-orm-0.1.8/django_async_orm/wrappers.py
--rw-r--r--   0        0        0      993 2021-05-29 10:25:12.770440 django-async-orm-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5457 2021-05-29 10:25:18.819343 django-async-orm-0.1.8/setup.py
--rw-r--r--   0        0        0     5681 2021-05-29 10:25:18.819760 django-async-orm-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2021-05-23 07:16:12.859441 django-async-orm-0.1.8.1/LICENSE
+-rw-r--r--   0        0        0     4812 2021-11-20 10:12:51.526399 django-async-orm-0.1.8.1/README.md
+-rw-r--r--   0        0        0    53248 2021-11-17 16:06:55.586986 django-async-orm-0.1.8.1/django_async_orm/.coverage
+-rw-r--r--   0        0        0        0 2021-11-23 18:35:24.325180 django-async-orm-0.1.8.1/django_async_orm/__init__.py
+-rw-r--r--   0        0        0      340 2021-11-17 19:06:59.905320 django-async-orm-0.1.8.1/django_async_orm/apps.py
+-rw-r--r--   0        0        0      355 2021-05-24 07:01:52.476066 django-async-orm-0.1.8.1/django_async_orm/iter.py
+-rw-r--r--   0        0        0      174 2021-05-23 09:54:11.642083 django-async-orm-0.1.8.1/django_async_orm/manager.py
+-rw-r--r--   0        0        0     6578 2021-05-27 20:37:47.469044 django-async-orm-0.1.8.1/django_async_orm/query.py
+-rw-r--r--   0        0        0      934 2021-05-29 10:24:53.070567 django-async-orm-0.1.8.1/django_async_orm/utils.py
+-rw-r--r--   0        0        0      684 2021-05-23 11:24:51.726987 django-async-orm-0.1.8.1/django_async_orm/wrappers.py
+-rw-r--r--   0        0        0     1034 2021-11-23 19:52:48.436577 django-async-orm-0.1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     5569 2021-11-23 19:52:50.950183 django-async-orm-0.1.8.1/setup.py
+-rw-r--r--   0        0        0     5835 2021-11-23 19:52:50.950932 django-async-orm-0.1.8.1/PKG-INFO
```

### Comparing `django-async-orm-0.1.8/LICENSE` & `django-async-orm-0.1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-async-orm-0.1.8/README.md` & `django-async-orm-0.1.8.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -112,15 +112,17 @@
 | `Model.objects.async_defer`              | ✅ |  |
 | `Model.objects.async_only`               | ✅ |  |
 | `Model.objects.async_using`              | ✅ |  |
 | `Model.objects.async_resolve_expression` | ✅ |  |
 | `Model.objects.async_ordered`            | ✅ |  |
 | `__aiter__`                              | ✅ |  |
 | `__repr__`                               | ✅ |  |
-| `Model.objects.async_iterator            | ❌ |  |
+| `__len__`                                | ❌ |  |
+| `__getitem__`                            | ❌ |  |
+| `Model.objects.async_iterator`           | ❌ |  |
 
 
 ### Model:
 
 | methods                    | supported  | comments |
 |----------------------------|------------|----------|
 | `Model.async_save`                      | ❌ |  |
```

### Comparing `django-async-orm-0.1.8/django_async_orm/query.py` & `django-async-orm-0.1.8.1/django_async_orm/query.py`

 * *Files identical despite different names*

### Comparing `django-async-orm-0.1.8/django_async_orm/utils.py` & `django-async-orm-0.1.8.1/django_async_orm/utils.py`

 * *Files identical despite different names*

### Comparing `django-async-orm-0.1.8/django_async_orm/wrappers.py` & `django-async-orm-0.1.8.1/django_async_orm/wrappers.py`

 * *Files identical despite different names*

### Comparing `django-async-orm-0.1.8/pyproject.toml` & `django-async-orm-0.1.8.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "django-async-orm"
-version = "0.1.8"
+version = "0.1.8.1"
 description = "Bringing async capabilities to django ORM"
 authors = ["SkanderBM <skander.bmahmoud@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rednaks/django-async-orm"
 repository = "https://github.com/rednaks/django-async-orm"
 keywords = ["django", "async", "orm"]
 classifiers = [
+    "Development Status :: 3 - Alpha",
     "Framework :: Django",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Documentation",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
```

### Comparing `django-async-orm-0.1.8/setup.py` & `django-async-orm-0.1.8.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['django_async_orm']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'django-async-orm',
-    'version': '0.1.8',
+    'version': '0.1.8.1',
     'description': 'Bringing async capabilities to django ORM',
-    'long_description': '## Disclaimer: Don\'t use this module in production it\'s still in active development.\n\n# Django Async Orm\nDjango module that brings async to django ORM.\n\n# Installing\n```\npython -m pip install django-async-orm\n``` \n\nthen add `django_async_orm` to your `INSTALLED_APPS` list:\n\n```python\nINSTALLED_APPS = [\n    ...,\n    \'django_async_orm\'\n]\n```\n# Usage\n\nDjango Async Orm will patch all your existing models to add `async_*` prefixed methods.\nTo be\n\nexample:\n\n```python\nclass MyModel(models.Model):\n    name = models.CharField(max_length=250)\n\n```\n\nyou can use it as follow:\n\n```python\nasync def get_model():\n    return await  MyModel.objects.async_get(name="something")\n```\n\nyou can also iterate over a query set with `async for`:\n\n```python\nasync def all_models():\n    all_result_set = await MyModel.objects.async_all()\n    async for obj in all_result_set:\n        print(obj)\n```\n\nSome wrappers are also available for template rendering, form validation and login/logout\n\n\n#### Async login\n```python\nfrom django_async_orm.wrappers import async_login\n\nasync def my_async_view(request):\n    await async_login(request)\n    ...\n```\n\n#### Form validation\n```python\n\nfrom django_async_orm.wrappers import async_form_is_valid\nasync def a_view(request):\n    form = MyForm(request.POST)\n    is_valid_form = await async_form_is_valid(form)\n    if is_valid_form:\n        ...\n    \n```\n\n\n# Django ORM support:\n\nThis is an on going projects, not all model methods are ported.\n\n### Manager:\n\n| methods                    | supported  | comments |\n|----------------------------|------------|----------|\n| `Model.objects.async_get`                | ✅ |  |\n| `Model.objects.async_create`             | ✅ |  |\n| `Model.objects.async_bulk_create`        | ✅ |  |\n| `Model.objects.async_bulk_update`        | ✅ |  |\n| `Model.objects.async_get_or_create`      | ✅ |  |\n| `Model.objects.async_update_or_create`   | ✅ |  |\n| `Model.objects.async_earliest`           | ✅ |  |\n| `Model.objects.async_latest`             | ✅ |  |\n| `Model.objects.async_first`              | ✅ |  |\n| `Model.objects.async_last`               | ✅ |  |\n| `Model.objects.async_in_bulk`            | ✅ |  |\n| `Model.objects.async_delete`             | ✅ |  |\n| `Model.objects.async_update`             | ✅ |  |\n| `Model.objects.async_exists`             | ✅ |  |\n| `Model.objects.async_explain`            | ✅ |  |\n| `Model.objects.async_raw`                | ✅ |  |\n| `Model.objects.async_all`                | ✅ |  |\n| `Model.objects.async_filter`             | ✅ |  |\n| `Model.objects.async_exclude`            | ✅ |  |\n| `Model.objects.async_complex_filter`     | ✅ |  |\n| `Model.objects.async_union`              | ✅ |  |\n| `Model.objects.async_intersection`       | ✅ |  |\n| `Model.objects.async_difference`         | ✅ |  |\n| `Model.objects.async_select_for_update`  | ✅ |  |\n| `Model.objects.async_prefetch_related`   | ✅ |  |\n| `Model.objects.async_annotate`           | ✅ |  |\n| `Model.objects.async_order_by`           | ✅ |  |\n| `Model.objects.async_distinct`           | ✅ |  |\n| `Model.objects.async_difference`         | ✅ |  |\n| `Model.objects.async_extra`              | ✅ |  |\n| `Model.objects.async_reverse`            | ✅ |  |\n| `Model.objects.async_defer`              | ✅ |  |\n| `Model.objects.async_only`               | ✅ |  |\n| `Model.objects.async_using`              | ✅ |  |\n| `Model.objects.async_resolve_expression` | ✅ |  |\n| `Model.objects.async_ordered`            | ✅ |  |\n| `__aiter__`                              | ✅ |  |\n| `__repr__`                               | ✅ |  |\n| `Model.objects.async_iterator            | ❌ |  |\n\n\n### Model:\n\n| methods                    | supported  | comments |\n|----------------------------|------------|----------|\n| `Model.async_save`                      | ❌ |  |\n| `Model.async_update`                    | ❌ |  |\n| `Model.async_delete`                    | ❌ |  |\n| `...`                                   | ❌ |  |\n\n\n### User Model / Manager\n| methods                    | supported  | comments |\n|----------------------------|------------|----------|\n| `UserModel.is_authenticated`            | ✅ |  |\n| `UserModel.is_super_user`               | ✅ |  |\n| `UserModel.objects.async_create_user`   | ❌ |  |\n| `...`                                   | ❌ |  |\n\n\n### Foreign object lazy loading:\nNot supported ❌\n\n\n### Wrappers:\n| methods                    | supported  | comments |\n|----------------------------|------------|----------|\n| `wrappers.async_render`            | ✅  |  |\n| `wrappers.async_login`            | ✅  |  |\n| `wrappers.async_logout`            | ✅  |  |\n\n\n\n',
+    'long_description': '## Disclaimer: Don\'t use this module in production it\'s still in active development.\n\n# Django Async Orm\nDjango module that brings async to django ORM.\n\n# Installing\n```\npython -m pip install django-async-orm\n``` \n\nthen add `django_async_orm` to your `INSTALLED_APPS` list:\n\n```python\nINSTALLED_APPS = [\n    ...,\n    \'django_async_orm\'\n]\n```\n# Usage\n\nDjango Async Orm will patch all your existing models to add `async_*` prefixed methods.\nTo be\n\nexample:\n\n```python\nclass MyModel(models.Model):\n    name = models.CharField(max_length=250)\n\n```\n\nyou can use it as follow:\n\n```python\nasync def get_model():\n    return await  MyModel.objects.async_get(name="something")\n```\n\nyou can also iterate over a query set with `async for`:\n\n```python\nasync def all_models():\n    all_result_set = await MyModel.objects.async_all()\n    async for obj in all_result_set:\n        print(obj)\n```\n\nSome wrappers are also available for template rendering, form validation and login/logout\n\n\n#### Async login\n```python\nfrom django_async_orm.wrappers import async_login\n\nasync def my_async_view(request):\n    await async_login(request)\n    ...\n```\n\n#### Form validation\n```python\n\nfrom django_async_orm.wrappers import async_form_is_valid\nasync def a_view(request):\n    form = MyForm(request.POST)\n    is_valid_form = await async_form_is_valid(form)\n    if is_valid_form:\n        ...\n    \n```\n\n\n# Django ORM support:\n\nThis is an on going projects, not all model methods are ported.\n\n### Manager:\n\n| methods                    | supported  | comments |\n|----------------------------|------------|----------|\n| `Model.objects.async_get`                | ✅ |  |\n| `Model.objects.async_create`             | ✅ |  |\n| `Model.objects.async_bulk_create`        | ✅ |  |\n| `Model.objects.async_bulk_update`        | ✅ |  |\n| `Model.objects.async_get_or_create`      | ✅ |  |\n| `Model.objects.async_update_or_create`   | ✅ |  |\n| `Model.objects.async_earliest`           | ✅ |  |\n| `Model.objects.async_latest`             | ✅ |  |\n| `Model.objects.async_first`              | ✅ |  |\n| `Model.objects.async_last`               | ✅ |  |\n| `Model.objects.async_in_bulk`            | ✅ |  |\n| `Model.objects.async_delete`             | ✅ |  |\n| `Model.objects.async_update`             | ✅ |  |\n| `Model.objects.async_exists`             | ✅ |  |\n| `Model.objects.async_explain`            | ✅ |  |\n| `Model.objects.async_raw`                | ✅ |  |\n| `Model.objects.async_all`                | ✅ |  |\n| `Model.objects.async_filter`             | ✅ |  |\n| `Model.objects.async_exclude`            | ✅ |  |\n| `Model.objects.async_complex_filter`     | ✅ |  |\n| `Model.objects.async_union`              | ✅ |  |\n| `Model.objects.async_intersection`       | ✅ |  |\n| `Model.objects.async_difference`         | ✅ |  |\n| `Model.objects.async_select_for_update`  | ✅ |  |\n| `Model.objects.async_prefetch_related`   | ✅ |  |\n| `Model.objects.async_annotate`           | ✅ |  |\n| `Model.objects.async_order_by`           | ✅ |  |\n| `Model.objects.async_distinct`           | ✅ |  |\n| `Model.objects.async_difference`         | ✅ |  |\n| `Model.objects.async_extra`              | ✅ |  |\n| `Model.objects.async_reverse`            | ✅ |  |\n| `Model.objects.async_defer`              | ✅ |  |\n| `Model.objects.async_only`               | ✅ |  |\n| `Model.objects.async_using`              | ✅ |  |\n| `Model.objects.async_resolve_expression` | ✅ |  |\n| `Model.objects.async_ordered`            | ✅ |  |\n| `__aiter__`                              | ✅ |  |\n| `__repr__`                               | ✅ |  |\n| `__len__`                                | ❌ |  |\n| `__getitem__`                            | ❌ |  |\n| `Model.objects.async_iterator`           | ❌ |  |\n\n\n### Model:\n\n| methods                    | supported  | comments |\n|----------------------------|------------|----------|\n| `Model.async_save`                      | ❌ |  |\n| `Model.async_update`                    | ❌ |  |\n| `Model.async_delete`                    | ❌ |  |\n| `...`                                   | ❌ |  |\n\n\n### User Model / Manager\n| methods                    | supported  | comments |\n|----------------------------|------------|----------|\n| `UserModel.is_authenticated`            | ✅ |  |\n| `UserModel.is_super_user`               | ✅ |  |\n| `UserModel.objects.async_create_user`   | ❌ |  |\n| `...`                                   | ❌ |  |\n\n\n### Foreign object lazy loading:\nNot supported ❌\n\n\n### Wrappers:\n| methods                    | supported  | comments |\n|----------------------------|------------|----------|\n| `wrappers.async_render`            | ✅  |  |\n| `wrappers.async_login`            | ✅  |  |\n| `wrappers.async_logout`            | ✅  |  |\n\n\n\n',
     'author': 'SkanderBM',
     'author_email': 'skander.bmahmoud@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/rednaks/django-async-orm',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `django-async-orm-0.1.8/PKG-INFO` & `django-async-orm-0.1.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: django-async-orm
-Version: 0.1.8
+Version: 0.1.8.1
 Summary: Bringing async capabilities to django ORM
 Home-page: https://github.com/rednaks/django-async-orm
 License: MIT
 Keywords: django,async,orm
 Author: SkanderBM
 Author-email: skander.bmahmoud@gmail.com
 Requires-Python: >=3.6,<4.0
+Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -136,15 +137,17 @@
 | `Model.objects.async_defer`              | ✅ |  |
 | `Model.objects.async_only`               | ✅ |  |
 | `Model.objects.async_using`              | ✅ |  |
 | `Model.objects.async_resolve_expression` | ✅ |  |
 | `Model.objects.async_ordered`            | ✅ |  |
 | `__aiter__`                              | ✅ |  |
 | `__repr__`                               | ✅ |  |
-| `Model.objects.async_iterator            | ❌ |  |
+| `__len__`                                | ❌ |  |
+| `__getitem__`                            | ❌ |  |
+| `Model.objects.async_iterator`           | ❌ |  |
 
 
 ### Model:
 
 | methods                    | supported  | comments |
 |----------------------------|------------|----------|
 | `Model.async_save`                      | ❌ |  |
```

