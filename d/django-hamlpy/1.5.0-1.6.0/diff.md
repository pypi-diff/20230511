# Comparing `tmp/django_hamlpy-1.5.0.tar.gz` & `tmp/django_hamlpy-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_hamlpy-1.5.0.tar", max compression
+gzip compressed data, was "django_hamlpy-1.6.0.tar", max compression
```

## Comparing `django_hamlpy-1.5.0.tar` & `django_hamlpy-1.6.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1074 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/LICENSE
--rw-r--r--   0        0        0     9394 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/README.md
--rwxr-xr-x   0        0        0       37 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/__init__.py
--rw-r--r--   0        0        0      234 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/apps.py
--rwxr-xr-x   0        0        0     4458 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/compiler.py
--rw-r--r--   0        0        0     7368 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/hamlpy_watcher.py
--rw-r--r--   0        0        0      611 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/jinja.py
--rw-r--r--   0        0        0        0 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/parser/__init__.py
--rw-r--r--   0        0        0     6658 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/parser/attributes.py
--rw-r--r--   0        0        0     4876 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/parser/core.py
--rw-r--r--   0        0        0     6292 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/parser/elements.py
--rw-r--r--   0        0        0     5193 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/parser/filters.py
--rw-r--r--   0        0        0    16717 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/parser/nodes.py
--rw-r--r--   0        0        0     1331 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/parser/utils.py
--rw-r--r--   0        0        0       73 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/template/__init__.py
--rw-r--r--   0        0        0     2455 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/template/loaders.py
--rw-r--r--   0        0        0      797 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/template/templatize.py
--rw-r--r--   0        0        0      793 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/template/utils.py
--rw-r--r--   0        0        0      103 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/test/__init__.py
--rw-r--r--   0        0        0      595 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/test/settings.py
--rw-r--r--   0        0        0      294 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/test/templates/allIfTypesTest.hamlpy
--rw-r--r--   0        0        0      459 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/test/templates/allIfTypesTest.html
--rw-r--r--   0        0        0      200 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/test/templates/classIdMixtures.hamlpy
--rw-r--r--   0        0        0      211 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/test/templates/classIdMixtures.html
--rw-r--r--   0        0        0       43 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/test/templates/djangoBase.hamlpy
--rw-r--r--   0        0        0      108 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/test/templates/djangoBase.html
--rw-r--r--   0        0        0      260 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/test/templates/djangoCombo.hamlpy
--rw-r--r--   0        0        0      368 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/test/templates/djangoCombo.html
--rw-r--r--   0        0        0     1154 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/test/templates/filterMultilineIgnore.hamlpy
--rw-r--r--   0        0        0     1542 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/test/templates/filterMultilineIgnore.html
--rw-r--r--   0        0        0      415 2023-03-03 14:07:06.766250 django_hamlpy-1.5.0/hamlpy/test/templates/filters.hamlpy
--rw-r--r--   0        0        0      697 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/filters.html
--rw-r--r--   0        0        0       93 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/filtersMarkdown.hamlpy
--rw-r--r--   0        0        0      114 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/filtersMarkdown.html
--rw-r--r--   0        0        0       85 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/filtersPygments.hamlpy
--rw-r--r--   0        0        0      491 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/filtersPygments.html
--rw-r--r--   0        0        0      168 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/hamlComments.hamlpy
--rw-r--r--   0        0        0       79 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/hamlComments.html
--rw-r--r--   0        0        0      107 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/implicitDivs.hamlpy
--rw-r--r--   0        0        0      194 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/implicitDivs.html
--rw-r--r--   0        0        0      172 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/multiLineDict.hamlpy
--rw-r--r--   0        0        0      160 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/multiLineDict.html
--rw-r--r--   0        0        0       54 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/nestedComments.hamlpy
--rw-r--r--   0        0        0       93 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/nestedComments.html
--rw-r--r--   0        0        0      215 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/nestedDjangoTags.hamlpy
--rw-r--r--   0        0        0      362 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/nestedDjangoTags.html
--rw-r--r--   0        0        0       47 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/nestedIfElseBlocks.hamlpy
--rw-r--r--   0        0        0       90 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/nestedIfElseBlocks.html
--rw-r--r--   0        0        0      529 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/nukeInnerWhiteSpace.hamlpy
--rw-r--r--   0        0        0      545 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/nukeInnerWhiteSpace.html
--rw-r--r--   0        0        0     1085 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/nukeOuterWhiteSpace.hamlpy
--rw-r--r--   0        0        0     1495 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/nukeOuterWhiteSpace.html
--rw-r--r--   0        0        0      142 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/selfClosingDjango.hamlpy
--rw-r--r--   0        0        0      217 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/selfClosingDjango.html
--rw-r--r--   0        0        0       63 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/selfClosingTags.hamlpy
--rw-r--r--   0        0        0       82 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/selfClosingTags.html
--rw-r--r--   0        0        0       67 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/simple.hamlpy
--rw-r--r--   0        0        0      104 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/simple.html
--rw-r--r--   0        0        0     1012 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/whitespacePreservation.hamlpy
--rw-r--r--   0        0        0     1150 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/templates/whitespacePreservation.html
--rw-r--r--   0        0        0    11450 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/test_attributes.py
--rwxr-xr-x   0        0        0    15477 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/test_compiler.py
--rw-r--r--   0        0        0     6173 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/test_elements.py
--rw-r--r--   0        0        0      912 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/test_jinja.py
--rw-r--r--   0        0        0     2388 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/test_loader.py
--rw-r--r--   0        0        0     4853 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/test_nodes.py
--rw-r--r--   0        0        0     4020 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/test_parser.py
--rw-r--r--   0        0        0     3800 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/test_templates.py
--rw-r--r--   0        0        0      960 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/test_templatize.py
--rw-r--r--   0        0        0      692 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/test_views.py
--rw-r--r--   0        0        0     3420 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/test/test_watcher.py
--rw-r--r--   0        0        0        0 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/views/__init__.py
--rw-r--r--   0        0        0      999 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/hamlpy/views/generic/__init__.py
--rw-r--r--   0        0        0     1625 2023-03-03 14:07:06.770250 django_hamlpy-1.5.0/pyproject.toml
--rw-r--r--   0        0        0    10322 1970-01-01 00:00:00.000000 django_hamlpy-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/LICENSE
+-rw-r--r--   0        0        0     9394 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/README.md
+-rwxr-xr-x   0        0        0       37 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/hamlpy/__init__.py
+-rw-r--r--   0        0        0      234 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/hamlpy/apps.py
+-rwxr-xr-x   0        0        0     4541 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/hamlpy/compiler.py
+-rw-r--r--   0        0        0     7368 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/hamlpy/hamlpy_watcher.py
+-rw-r--r--   0        0        0      611 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/hamlpy/jinja.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/hamlpy/parser/__init__.py
+-rw-r--r--   0        0        0     6658 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/hamlpy/parser/attributes.py
+-rw-r--r--   0        0        0     4876 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/hamlpy/parser/core.py
+-rw-r--r--   0        0        0     6365 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/hamlpy/parser/elements.py
+-rw-r--r--   0        0        0     5193 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/hamlpy/parser/filters.py
+-rw-r--r--   0        0        0    16910 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/hamlpy/parser/nodes.py
+-rw-r--r--   0        0        0     1331 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/hamlpy/parser/utils.py
+-rw-r--r--   0        0        0       73 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/hamlpy/template/__init__.py
+-rw-r--r--   0        0        0     2455 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/hamlpy/template/loaders.py
+-rw-r--r--   0        0        0      797 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/hamlpy/template/templatize.py
+-rw-r--r--   0        0        0      793 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/hamlpy/template/utils.py
+-rw-r--r--   0        0        0      103 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/hamlpy/test/__init__.py
+-rw-r--r--   0        0        0      595 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/hamlpy/test/settings.py
+-rw-r--r--   0        0        0      294 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/hamlpy/test/templates/allIfTypesTest.hamlpy
+-rw-r--r--   0        0        0      459 2023-05-11 15:21:28.119488 django_hamlpy-1.6.0/hamlpy/test/templates/allIfTypesTest.html
+-rw-r--r--   0        0        0      200 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/classIdMixtures.hamlpy
+-rw-r--r--   0        0        0      211 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/classIdMixtures.html
+-rw-r--r--   0        0        0       43 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/djangoBase.hamlpy
+-rw-r--r--   0        0        0      108 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/djangoBase.html
+-rw-r--r--   0        0        0      260 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/djangoCombo.hamlpy
+-rw-r--r--   0        0        0      368 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/djangoCombo.html
+-rw-r--r--   0        0        0     1154 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/filterMultilineIgnore.hamlpy
+-rw-r--r--   0        0        0     1542 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/filterMultilineIgnore.html
+-rw-r--r--   0        0        0      415 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/filters.hamlpy
+-rw-r--r--   0        0        0      697 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/filters.html
+-rw-r--r--   0        0        0       93 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/filtersMarkdown.hamlpy
+-rw-r--r--   0        0        0      114 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/filtersMarkdown.html
+-rw-r--r--   0        0        0       85 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/filtersPygments.hamlpy
+-rw-r--r--   0        0        0      491 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/filtersPygments.html
+-rw-r--r--   0        0        0      168 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/hamlComments.hamlpy
+-rw-r--r--   0        0        0       79 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/hamlComments.html
+-rw-r--r--   0        0        0      107 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/implicitDivs.hamlpy
+-rw-r--r--   0        0        0      194 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/implicitDivs.html
+-rw-r--r--   0        0        0      172 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/multiLineDict.hamlpy
+-rw-r--r--   0        0        0      160 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/multiLineDict.html
+-rw-r--r--   0        0        0       54 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/nestedComments.hamlpy
+-rw-r--r--   0        0        0       93 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/nestedComments.html
+-rw-r--r--   0        0        0      215 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/nestedDjangoTags.hamlpy
+-rw-r--r--   0        0        0      362 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/nestedDjangoTags.html
+-rw-r--r--   0        0        0       47 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/nestedIfElseBlocks.hamlpy
+-rw-r--r--   0        0        0       90 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/nestedIfElseBlocks.html
+-rw-r--r--   0        0        0      529 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/nukeInnerWhiteSpace.hamlpy
+-rw-r--r--   0        0        0      545 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/nukeInnerWhiteSpace.html
+-rw-r--r--   0        0        0     1085 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/nukeOuterWhiteSpace.hamlpy
+-rw-r--r--   0        0        0     1495 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/nukeOuterWhiteSpace.html
+-rw-r--r--   0        0        0      142 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/selfClosingDjango.hamlpy
+-rw-r--r--   0        0        0      217 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/selfClosingDjango.html
+-rw-r--r--   0        0        0       63 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/selfClosingTags.hamlpy
+-rw-r--r--   0        0        0       82 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/selfClosingTags.html
+-rw-r--r--   0        0        0       67 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/simple.hamlpy
+-rw-r--r--   0        0        0      104 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/simple.html
+-rw-r--r--   0        0        0     1012 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/whitespacePreservation.hamlpy
+-rw-r--r--   0        0        0     1150 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/templates/whitespacePreservation.html
+-rw-r--r--   0        0        0    11450 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/test_attributes.py
+-rwxr-xr-x   0        0        0    15824 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/test_compiler.py
+-rw-r--r--   0        0        0     6401 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/test_elements.py
+-rw-r--r--   0        0        0      912 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/test_jinja.py
+-rw-r--r--   0        0        0     2388 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/test_loader.py
+-rw-r--r--   0        0        0     4853 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/test_nodes.py
+-rw-r--r--   0        0        0     4020 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/test_parser.py
+-rw-r--r--   0        0        0     3800 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/test_templates.py
+-rw-r--r--   0        0        0      960 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/test_templatize.py
+-rw-r--r--   0        0        0      692 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/test_views.py
+-rw-r--r--   0        0        0     3420 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/test/test_watcher.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/views/__init__.py
+-rw-r--r--   0        0        0      999 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/hamlpy/views/generic/__init__.py
+-rw-r--r--   0        0        0     1605 2023-05-11 15:21:28.123489 django_hamlpy-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0    10222 1970-01-01 00:00:00.000000 django_hamlpy-1.6.0/PKG-INFO
```

### Comparing `django_hamlpy-1.5.0/LICENSE` & `django_hamlpy-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/README.md` & `django_hamlpy-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/compiler.py` & `django_hamlpy-1.6.0/hamlpy/compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         self.escape_attrs = False  # escape HTML-sensitive characters in attribute values
         self.cdata = False  # wrap CSS, Javascript etc content in CDATA section
 
         # implementation specific options
         self.django_inline_style = False  # support both #{...} and ={...}
         self.tag_config = "django"  # Django vs Jinja2 tags
         self.custom_self_closing_tags = {}  # additional self-closing tags
+        self.endblock_names = False  # include block name on endblock closing tags
         self.debug_tree = False
 
         for k, v in kwargs.items():
             setattr(self, k, v)
 
         if self.django_inline_style:  # pragma: no cover
             warnings.warn("Support for ={..} style variables is deprecated", DeprecationWarning)
```

### Comparing `django_hamlpy-1.5.0/hamlpy/hamlpy_watcher.py` & `django_hamlpy-1.6.0/hamlpy/hamlpy_watcher.py`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/jinja.py` & `django_hamlpy-1.6.0/hamlpy/jinja.py`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/parser/attributes.py` & `django_hamlpy-1.6.0/hamlpy/parser/attributes.py`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/parser/core.py` & `django_hamlpy-1.6.0/hamlpy/parser/core.py`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/parser/elements.py` & `django_hamlpy-1.6.0/hamlpy/parser/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,15 @@
         "embed",
         "keygen",
         "param",
         "wbr",
     )
 
     DEFAULT_TAG = "div"
+    ESCAPED = {'"': "&quot;", "'": "&#39;"}
 
     def __init__(
         self,
         tag,
         _id,
         classes,
         attributes,
@@ -186,26 +187,26 @@
             rendered.append("class=%s" % attr_wrap(" ".join(self.classes)))
 
         if self.id:
             rendered.append("id=%s" % attr_wrap(self.id))
 
         return " ".join(rendered)
 
-    @staticmethod
-    def _escape_attribute_quotes(v, attr_wrapper):
+    @classmethod
+    def _escape_attribute_quotes(cls, v, attr_wrapper):
         """
-        Escapes quotes with a backslash, except those inside a Django tag
+        Escapes quotes, except those inside a Django tag
         """
         escaped = []
         inside_tag = False
         for i, _ in enumerate(v):
             if v[i : i + 2] == "{%":
                 inside_tag = True
             elif v[i : i + 2] == "%}":
                 inside_tag = False
 
             if v[i] == attr_wrapper and not inside_tag:
-                escaped.append("\\")
-
-            escaped.append(v[i])
+                escaped.append(cls.ESCAPED[attr_wrapper])
+            else:
+                escaped.append(v[i])
 
         return "".join(escaped)
```

### Comparing `django_hamlpy-1.5.0/hamlpy/parser/filters.py` & `django_hamlpy-1.6.0/hamlpy/parser/filters.py`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/parser/nodes.py` & `django_hamlpy-1.6.0/hamlpy/parser/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -466,14 +466,18 @@
 
     def _render(self):
         self.before = "%s{%% %s %%}" % (self.indent, self.tag_statement)
 
         closing_tag = self.compiler.self_closing_tags.get(self.tag_name)
 
         if closing_tag:
+            if self.tag_name == "block" and self.compiler.options.endblock_names:
+                block_name = self.tag_statement.split(" ")[1]
+                closing_tag += " " + block_name
+
             self.before += self.render_newlines()
             self.after = "%s{%% %s %%}%s" % (self.indent, closing_tag, self.render_newlines())
         else:
             if self.children:
                 self.before += self.render_newlines()
             else:
                 self.after = self.render_newlines()
```

### Comparing `django_hamlpy-1.5.0/hamlpy/parser/utils.py` & `django_hamlpy-1.6.0/hamlpy/parser/utils.py`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/template/loaders.py` & `django_hamlpy-1.6.0/hamlpy/template/loaders.py`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/template/templatize.py` & `django_hamlpy-1.6.0/hamlpy/template/templatize.py`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/template/utils.py` & `django_hamlpy-1.6.0/hamlpy/template/utils.py`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/test/settings.py` & `django_hamlpy-1.6.0/hamlpy/test/settings.py`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/test/templates/filterMultilineIgnore.hamlpy` & `django_hamlpy-1.6.0/hamlpy/test/templates/filterMultilineIgnore.hamlpy`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/test/templates/filterMultilineIgnore.html` & `django_hamlpy-1.6.0/hamlpy/test/templates/filterMultilineIgnore.html`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/test/templates/filters.html` & `django_hamlpy-1.6.0/hamlpy/test/templates/filters.html`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/test/templates/nukeInnerWhiteSpace.hamlpy` & `django_hamlpy-1.6.0/hamlpy/test/templates/nukeInnerWhiteSpace.hamlpy`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/test/templates/nukeInnerWhiteSpace.html` & `django_hamlpy-1.6.0/hamlpy/test/templates/nukeInnerWhiteSpace.html`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/test/templates/nukeOuterWhiteSpace.hamlpy` & `django_hamlpy-1.6.0/hamlpy/test/templates/nukeOuterWhiteSpace.hamlpy`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/test/templates/nukeOuterWhiteSpace.html` & `django_hamlpy-1.6.0/hamlpy/test/templates/nukeOuterWhiteSpace.html`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/test/templates/whitespacePreservation.hamlpy` & `django_hamlpy-1.6.0/hamlpy/test/templates/whitespacePreservation.hamlpy`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/test/templates/whitespacePreservation.html` & `django_hamlpy-1.6.0/hamlpy/test/templates/whitespacePreservation.html`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/test/test_attributes.py` & `django_hamlpy-1.6.0/hamlpy/test/test_attributes.py`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/test/test_compiler.py` & `django_hamlpy-1.6.0/hamlpy/test/test_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,25 @@
         # with
         self._test("- with thing1 as another\n  stuff", "{% with thing1 as another %}\n  stuff\n{% endwith %}")
         self._test(
             "- with context\n  hello\n- with other_context\n  goodbye",
             "{% with context %}\n  hello\n{% endwith %}\n{% with other_context %}\n  goodbye\n{% endwith %}",
         )
 
+        # block
+        self._test(
+            "-block title\n   %p hello\n",
+            "{% block title %}\n   <p>hello</p>\n{% endblock %}",
+        )
+        self._test(
+            "-block title\n   %p hello\n",
+            "{% block title %}\n   <p>hello</p>\n{% endblock title %}",
+            options={"endblock_names": True},
+        )
+
         # trans
         self._test('- trans "Hello"\n', '{% trans "Hello" %}')
 
         # blocktrans
         self._test(
             "- blocktrans with amount=num_cookies\n" "  There are #{ amount } cookies",
             "{% blocktrans with amount=num_cookies %}\n" "  There are {{ amount }} cookies\n" "{% endblocktrans %}",
```

### Comparing `django_hamlpy-1.5.0/hamlpy/test/test_elements.py` & `django_hamlpy-1.6.0/hamlpy/test/test_elements.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,16 +39,21 @@
         self.assertEqual(element.inline_content, "")
         self.assertEqual(stream.text[stream.ptr :], "")
 
     def test_escape_attribute_quotes(self):
         s1 = Element._escape_attribute_quotes("""{% url 'blah' %}""", attr_wrapper="'")
         assert s1 == """{% url 'blah' %}"""
 
-        s2 = Element._escape_attribute_quotes("""blah's blah''s {% url 'blah' %} blah's blah''s""", attr_wrapper="'")
-        assert s2 == r"blah\'s blah\'\'s {% url 'blah' %} blah\'s blah\'\'s"
+        s2 = Element._escape_attribute_quotes(
+            """'foo'="bar" {% url 'blah' "blah" %} blah's blah''s""", attr_wrapper="'"
+        )
+        assert s2 == """&#39;foo&#39;="bar" {% url 'blah' "blah" %} blah&#39;s blah&#39;&#39;s"""
+
+        s3 = Element._escape_attribute_quotes("""'foo'="bar" {% url 'blah' "blah" %}""", attr_wrapper='"')
+        assert s3 == """'foo'=&quot;bar&quot; {% url 'blah' "blah" %}"""
 
     def test_parses_tag(self):
         element = self._read_element("%span.class")
         assert element.tag == "span"
 
         # can have namespace and hypens
         element = self._read_element("%ng-tags:ng-repeat.class")
```

### Comparing `django_hamlpy-1.5.0/hamlpy/test/test_jinja.py` & `django_hamlpy-1.6.0/hamlpy/test/test_jinja.py`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/test/test_loader.py` & `django_hamlpy-1.6.0/hamlpy/test/test_loader.py`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/test/test_nodes.py` & `django_hamlpy-1.6.0/hamlpy/test/test_nodes.py`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/test/test_parser.py` & `django_hamlpy-1.6.0/hamlpy/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/test/test_templates.py` & `django_hamlpy-1.6.0/hamlpy/test/test_templates.py`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/test/test_templatize.py` & `django_hamlpy-1.6.0/hamlpy/test/test_templatize.py`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/test/test_views.py` & `django_hamlpy-1.6.0/hamlpy/test/test_views.py`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/test/test_watcher.py` & `django_hamlpy-1.6.0/hamlpy/test/test_watcher.py`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/hamlpy/views/generic/__init__.py` & `django_hamlpy-1.6.0/hamlpy/views/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `django_hamlpy-1.5.0/pyproject.toml` & `django_hamlpy-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-hamlpy"
-version = "1.5.0"
+version = "1.6.0"
 description = "HAML like syntax for Django templates"
 authors = ["Nyaruka <code@nyaruka.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers=[
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
@@ -17,24 +17,23 @@
     { include = "hamlpy" },
 ]
 
 [tool.poetry.urls]
 repository = "http://github.com/nyaruka/django-hamlpy"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.9"
 django = ">=3.2,<5.0"
 regex = ">=2020.1.1"
 
 [tool.poetry.dev-dependencies]
 Markdown = "^3.4.1"
 pytest = "^6.1.2"
 pytest-cov = "^4.0.0"
 Pygments = "^2.14.0"
-codecov = "^2.1.12"
 Jinja2 = "^3.1.2"
 black = "^23.1.0"
 isort = "^5.11.0"
 
 [tool.poetry.scripts]
 hamlpy-watcher = "hamlpy.hamlpy_watcher:watch_folder"
```

### Comparing `django_hamlpy-1.5.0/PKG-INFO` & `django_hamlpy-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: django-hamlpy
-Version: 1.5.0
+Version: 1.6.0
 Summary: HAML like syntax for Django templates
 License: MIT
 Author: Nyaruka
 Author-email: code@nyaruka.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django (>=3.2,<5.0)
 Requires-Dist: regex (>=2020.1.1)
 Project-URL: repository, http://github.com/nyaruka/django-hamlpy
 Description-Content-Type: text/markdown
```

