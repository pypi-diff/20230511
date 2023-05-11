# Comparing `tmp/manim_course_utils-0.2.0.tar.gz` & `tmp/manim_course_utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim_course_utils-0.2.0.tar", max compression
+gzip compressed data, was "manim_course_utils-0.3.0.tar", max compression
```

## Comparing `manim_course_utils-0.2.0.tar` & `manim_course_utils-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       74 2023-05-11 16:01:10.723193 manim_course_utils-0.2.0/manim_course_utils/__init__.py
--rw-r--r--   0        0        0     2611 2023-05-11 16:00:10.102887 manim_course_utils-0.2.0/manim_course_utils/animation_description.py
--rw-r--r--   0        0        0     1722 2023-05-11 16:01:19.606091 manim_course_utils-0.2.0/manim_course_utils/mobject_description.py
--rw-r--r--   0        0        0      534 2023-05-11 16:20:30.323291 manim_course_utils-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      168 2023-05-11 16:15:04.015818 manim_course_utils-0.2.0/README.md
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 manim_course_utils-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       74 2023-05-11 16:01:10.723193 manim_course_utils-0.3.0/manim_course_utils/__init__.py
+-rw-r--r--   0        0        0     2611 2023-05-11 16:00:10.102887 manim_course_utils-0.3.0/manim_course_utils/animation_description.py
+-rw-r--r--   0        0        0     1722 2023-05-11 16:01:19.606091 manim_course_utils-0.3.0/manim_course_utils/mobject_description.py
+-rw-r--r--   0        0        0      658 2023-05-11 16:24:15.821706 manim_course_utils-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-05-11 16:15:04.015818 manim_course_utils-0.3.0/README.md
+-rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 manim_course_utils-0.3.0/PKG-INFO
```

### Comparing `manim_course_utils-0.2.0/manim_course_utils/animation_description.py` & `manim_course_utils-0.3.0/manim_course_utils/animation_description.py`

 * *Files identical despite different names*

### Comparing `manim_course_utils-0.2.0/manim_course_utils/mobject_description.py` & `manim_course_utils-0.3.0/manim_course_utils/mobject_description.py`

 * *Files identical despite different names*

### Comparing `manim_course_utils-0.2.0/pyproject.toml` & `manim_course_utils-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 [tool.poetry]
 name = "manim-course-utils"
-version = "0.2.0"
+version = "0.3.0"
 description = "Para el curso de ManimCE de MathLike"
+homepage = "https://github.com/MathLike/manim-course-utils"
+repository = "https://github.com/MathLike/manim-course-utils"
 authors = ["MathLike <benjamin.ubilla@uc.cl>"]
 readme = "README.md"
 packages = [{include = "manim_course_utils"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 manim = "^0.17.3"
```

