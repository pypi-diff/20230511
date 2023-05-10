# Comparing `tmp/django_fragments-0.1.1.tar.gz` & `tmp/django_fragments-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_fragments-0.1.1.tar", max compression
+gzip compressed data, was "django_fragments-0.1.2.tar", max compression
```

## Comparing `django_fragments-0.1.1.tar` & `django_fragments-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1491 2023-05-09 09:45:58.288456 django_fragments-0.1.1/LICENSE
--rw-r--r--   0        0        0      690 2023-05-09 09:47:26.935180 django_fragments-0.1.1/README.md
--rw-r--r--   0        0        0       27 2023-05-10 21:50:52.993055 django_fragments-0.1.1/django_fragments/__init__.py
--rw-r--r--   0        0        0      163 2023-05-08 11:11:49.135944 django_fragments-0.1.1/django_fragments/apps.py
--rw-r--r--   0        0        0      258 2023-05-10 22:57:17.273819 django_fragments-0.1.1/django_fragments/forms.py
--rw-r--r--   0        0        0      292 2023-05-07 15:19:00.977243 django_fragments-0.1.1/django_fragments/templates/svg/heroicons_x_mark_mini.html
--rw-r--r--   0        0        0      132 2023-05-10 22:28:42.950032 django_fragments-0.1.1/django_fragments/templates/test_snippet.html
--rw-r--r--   0        0        0        0 2023-05-07 23:31:34.843055 django_fragments-0.1.1/django_fragments/templatetags/__init__.py
--rw-r--r--   0        0        0     5104 2023-05-10 22:52:21.725007 django_fragments-0.1.1/django_fragments/templatetags/fragments.py
--rw-r--r--   0        0        0     2039 2023-05-09 09:39:46.557198 django_fragments-0.1.1/django_fragments/templatetags/helpers.py
--rw-r--r--   0        0        0     1649 2023-05-09 09:40:55.305731 django_fragments-0.1.1/django_fragments/templatetags/og.py
--rw-r--r--   0        0        0       70 2023-05-08 02:09:45.909742 django_fragments-0.1.1/django_fragments/templatetags/utils/__init__.py
--rw-r--r--   0        0        0     2157 2023-05-08 02:17:55.382358 django_fragments-0.1.1/django_fragments/templatetags/utils/filter_attrs.py
--rw-r--r--   0        0        0     4146 2023-05-08 08:19:35.581999 django_fragments-0.1.1/django_fragments/templatetags/utils/wrap_svg.py
--rw-r--r--   0        0        0     4919 2023-05-10 22:57:26.892872 django_fragments-0.1.1/django_fragments/tests.py
--rw-r--r--   0        0        0      424 2023-05-10 23:01:29.088719 django_fragments-0.1.1/django_fragments/utils.py
--rw-r--r--   0        0        0     1406 2023-05-10 23:01:21.957208 django_fragments-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1482 1970-01-01 00:00:00.000000 django_fragments-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-05-09 09:45:58.288456 django_fragments-0.1.2/LICENSE
+-rw-r--r--   0        0        0      690 2023-05-09 09:47:26.935180 django_fragments-0.1.2/README.md
+-rw-r--r--   0        0        0       27 2023-05-10 21:50:52.993055 django_fragments-0.1.2/django_fragments/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-08 11:11:49.135944 django_fragments-0.1.2/django_fragments/apps.py
+-rw-r--r--   0        0        0      258 2023-05-10 22:57:17.273819 django_fragments-0.1.2/django_fragments/forms.py
+-rw-r--r--   0        0        0      292 2023-05-07 15:19:00.977243 django_fragments-0.1.2/django_fragments/templates/svg/heroicons_x_mark_mini.html
+-rw-r--r--   0        0        0      132 2023-05-10 23:33:49.851109 django_fragments-0.1.2/django_fragments/templates/test_snippet.html
+-rw-r--r--   0        0        0        0 2023-05-07 23:31:34.843055 django_fragments-0.1.2/django_fragments/templatetags/__init__.py
+-rw-r--r--   0        0        0     5104 2023-05-10 23:39:18.905343 django_fragments-0.1.2/django_fragments/templatetags/fragments.py
+-rw-r--r--   0        0        0     2039 2023-05-09 09:39:46.557198 django_fragments-0.1.2/django_fragments/templatetags/helpers.py
+-rw-r--r--   0        0        0     1649 2023-05-09 09:40:55.305731 django_fragments-0.1.2/django_fragments/templatetags/og.py
+-rw-r--r--   0        0        0       70 2023-05-08 02:09:45.909742 django_fragments-0.1.2/django_fragments/templatetags/utils/__init__.py
+-rw-r--r--   0        0        0     2157 2023-05-08 02:17:55.382358 django_fragments-0.1.2/django_fragments/templatetags/utils/filter_attrs.py
+-rw-r--r--   0        0        0     4146 2023-05-08 08:19:35.581999 django_fragments-0.1.2/django_fragments/templatetags/utils/wrap_svg.py
+-rw-r--r--   0        0        0     4978 2023-05-10 23:39:48.860675 django_fragments-0.1.2/django_fragments/tests.py
+-rw-r--r--   0        0        0      424 2023-05-10 23:01:29.088719 django_fragments-0.1.2/django_fragments/utils.py
+-rw-r--r--   0        0        0     1406 2023-05-10 23:40:08.516052 django_fragments-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1482 1970-01-01 00:00:00.000000 django_fragments-0.1.2/PKG-INFO
```

### Comparing `django_fragments-0.1.1/LICENSE` & `django_fragments-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_fragments-0.1.1/README.md` & `django_fragments-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django_fragments-0.1.1/django_fragments/templatetags/fragments.py` & `django_fragments-0.1.2/django_fragments/templatetags/fragments.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -103,21 +103,21 @@
         Template("""
             {% load fragments %}
             {% whitespaceless %}
             <div class="{{ kls }}
                 data-hidden="{{ bound.is_hidden}}"
                 data-widget="{{ bound.widget_type }}"
             >
-                {{ bound.errors }}
                 <label for="{{ bound.id_for_label }}"
                     {% if label_kls %}class="{{ label_kls }}"{% endif %}>
                     {{bound.label}}
                 </label>
                 {{ bound }}
                 <p class="help">{{ bound.help_text }}</p>
+                {{ bound.errors }}
             </div>
             {% endwhitespaceless %}
             """)  # noqa: E501
         .render(
             context=Context(
                 {
                     "bound": bound,
```

### Comparing `django_fragments-0.1.1/django_fragments/templatetags/helpers.py` & `django_fragments-0.1.2/django_fragments/templatetags/helpers.py`

 * *Files identical despite different names*

### Comparing `django_fragments-0.1.1/django_fragments/templatetags/og.py` & `django_fragments-0.1.2/django_fragments/templatetags/og.py`

 * *Files identical despite different names*

### Comparing `django_fragments-0.1.1/django_fragments/templatetags/utils/filter_attrs.py` & `django_fragments-0.1.2/django_fragments/templatetags/utils/filter_attrs.py`

 * *Files identical despite different names*

### Comparing `django_fragments-0.1.1/django_fragments/templatetags/utils/wrap_svg.py` & `django_fragments-0.1.2/django_fragments/templatetags/utils/wrap_svg.py`

 * *Files identical despite different names*

### Comparing `django_fragments-0.1.1/django_fragments/tests.py` & `django_fragments-0.1.2/django_fragments/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,49 +73,49 @@
 def test_whitespace(template, html):
     assert Template(template).render(context=Context()) == html
 
 
 @pytest.mark.parametrize(
     "data, html",
     [
-        (  # unbound form
+        (  # unbound form, no values
             None,
             (
                 '<div class="fieldWrapper data-hidden="False"'
                 ' data-widget="email"><label for="id_email">Email</label><input'
                 ' type="email" name="email" required id="id_email"><p'
                 ' class="help">Testable form</p></div><div class="fieldWrapper'
                 ' data-hidden="False" data-widget="textarea"><label'
                 ' for="id_message">Message</label><textarea name="message" cols="40"'
                 ' rows="3" required id="id_message"></textarea><p'
                 ' class="help"></p></div>'
             ),
         ),
-        (  # bound valid form
+        (  # bound valid form, no error message list
             {"message": "Hi there", "email": "foo@example.com"},
             (
                 '<div class="fieldWrapper data-hidden="False"'
                 ' data-widget="email"><label for="id_email">Email</label><input'
                 ' type="email" name="email" value="foo@example.com" required'
                 ' id="id_email"><p class="help">Testable form</p></div><div'
                 ' class="fieldWrapper data-hidden="False" data-widget="textarea"><label'
                 ' for="id_message">Message</label><textarea name="message" cols="40"'
                 ' rows="3" required id="id_message">Hi there</textarea><p'
                 ' class="help"></p></div>'
             ),
         ),
-        (  # bound invalid form
+        (  # bound invalid form, with error message list
             {"message": "Hi there", "email": "foo"},
             (
-                '<div class="fieldWrapper data-hidden="False" data-widget="email"><ul'
-                ' class="errorlist"><li>Enter a valid email address.</li></ul><label'
-                ' for="id_email">Email</label><input type="email" name="email"'
-                ' value="foo" required id="id_email"><p class="help">Testable'
-                ' form</p></div><div class="fieldWrapper data-hidden="False"'
-                ' data-widget="textarea"><label'
+                '<div class="fieldWrapper data-hidden="False"'
+                ' data-widget="email"><label for="id_email">Email</label><input'
+                ' type="email" name="email" value="foo" required id="id_email"><p'
+                ' class="help">Testable form</p><ul class="errorlist"><li>Enter a valid'
+                ' email address.</li></ul></div><div class="fieldWrapper'
+                ' data-hidden="False" data-widget="textarea"><label'
                 ' for="id_message">Message</label><textarea name="message" cols="40"'
                 ' rows="3" required id="id_message">Hi there</textarea><p'
                 ' class="help"></p></div>'
             ),
         ),
     ],
 )
```

### Comparing `django_fragments-0.1.1/pyproject.toml` & `django_fragments-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "django-fragments"
 description = "Custom template tags for common html idioms in Django."
-version = "0.1.1"
+version = "0.1.2"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/django-fragments"
 documentation = "https://mv3.dev/django-fragments"
 classifiers = [
   "Programming Language :: Python :: 3.11",
```

### Comparing `django_fragments-0.1.1/PKG-INFO` & `django_fragments-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-fragments
-Version: 0.1.1
+Version: 0.1.2
 Summary: Custom template tags for common html idioms in Django.
 Home-page: https://mv3.dev
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
```

