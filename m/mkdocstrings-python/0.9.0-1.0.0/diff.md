# Comparing `tmp/mkdocstrings-python-0.9.0.tar.gz` & `tmp/mkdocstrings_python-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocstrings-python-0.9.0.tar", last modified: Mon Apr  3 14:20:24 2023, max compression
+gzip compressed data, was "mkdocstrings_python-1.0.0.tar", last modified: Thu May 11 10:08:32 2023, max compression
```

## Comparing `mkdocstrings-python-0.9.0.tar` & `mkdocstrings_python-1.0.0.tar`

### file list

```diff
@@ -1,71 +1,64 @@
--rw-r--r--   0        0        0      754 2023-04-01 14:36:13.301342 mkdocstrings-python-0.9.0/LICENSE
--rw-r--r--   0        0        0     3758 2023-04-01 14:36:13.404674 mkdocstrings-python-0.9.0/README.md
--rw-r--r--   0        0        0     2318 2023-04-01 14:36:13.404674 mkdocstrings-python-0.9.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-01 14:36:13.198010 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/py.typed
--rw-r--r--   0        0        0      326 2023-04-01 14:36:34.291024 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/__init__.py
--rw-r--r--   0        0        0    17401 2023-04-03 14:17:32.034907 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/handler.py
--rw-r--r--   0        0        0     6336 2023-04-01 15:17:37.426937 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/rendering.py
--rw-r--r--   0        0        0     2532 2022-04-29 13:33:38.953329 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html
--rw-r--r--   0        0        0     5053 2023-04-01 15:33:24.336417 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/children.html
--rw-r--r--   0        0        0     4186 2022-04-29 17:28:38.933216 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/class.html
--rw-r--r--   0        0        0      269 2022-02-13 13:38:05.822420 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/admonition.html
--rw-r--r--   0        0        0     2465 2022-04-29 23:09:02.903315 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html
--rw-r--r--   0        0        0      400 2022-03-01 18:29:05.585970 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/examples.html
--rw-r--r--   0        0        0     2475 2022-04-29 23:09:07.859915 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html
--rw-r--r--   0        0        0     3134 2022-04-29 23:09:10.543213 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html
--rw-r--r--   0        0        0     2132 2022-04-29 23:09:12.233190 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html
--rw-r--r--   0        0        0     3111 2022-04-29 23:09:14.279830 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html
--rw-r--r--   0        0        0     3081 2022-04-29 23:09:16.163138 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html
--rw-r--r--   0        0        0     2115 2022-04-29 23:09:18.059779 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html
--rw-r--r--   0        0        0     3051 2022-04-29 23:09:20.759743 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html
--rw-r--r--   0        0        0     1740 2023-03-03 13:20:57.896481 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html
--rw-r--r--   0        0        0      590 2022-04-29 22:21:21.405388 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/expression.html
--rw-r--r--   0        0        0     2532 2022-04-29 17:28:35.633273 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/function.html
--rw-r--r--   0        0        0      245 2022-05-08 08:40:49.298304 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/labels.html
--rw-r--r--   0        0        0     1852 2022-04-29 17:36:56.831573 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/module.html
--rw-r--r--   0        0        0     2055 2022-11-13 16:53:10.704878 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/signature.html
--rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/attribute.html
--rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/children.html
--rw-r--r--   0        0        0       33 2021-11-03 19:53:40.146116 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/class.html
--rw-r--r--   0        0        0       48 2022-02-01 20:48:46.512716 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/admonition.html
--rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/attributes.html
--rw-r--r--   0        0        0       46 2021-11-03 19:54:24.832142 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/examples.html
--rw-r--r--   0        0        0       54 2021-11-03 19:54:24.832142 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/other_parameters.html
--rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/parameters.html
--rw-r--r--   0        0        0       44 2021-11-22 18:41:47.281610 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/raises.html
--rw-r--r--   0        0        0       46 2021-11-22 18:41:51.551545 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/receives.html
--rw-r--r--   0        0        0       45 2021-11-03 19:54:24.832142 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/returns.html
--rw-r--r--   0        0        0       43 2021-11-22 18:41:56.598136 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/warns.html
--rw-r--r--   0        0        0       44 2021-11-03 19:54:24.832142 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/yields.html
--rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring.html
--rw-r--r--   0        0        0       38 2021-11-08 00:26:56.388000 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/expression.html
--rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/function.html
--rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/labels.html
--rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/module.html
--rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/signature.html
--rw-r--r--   0        0        0      703 2022-03-03 18:21:59.514950 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/style.css
--rw-r--r--   0        0        0      224 2021-10-30 13:54:10.019274 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/mkdocs/exceptions.html
--rw-r--r--   0        0        0      277 2021-10-30 13:54:10.202605 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/mkdocs/keyword_args.html
--rw-r--r--   0        0        0      293 2021-10-30 13:54:10.019274 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/mkdocs/parameters.html
--rw-r--r--   0        0        0      200 2021-10-30 13:54:10.092606 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/mkdocs/return.html
--rw-r--r--   0        0        0      137 2021-10-30 13:54:10.199272 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/mkdocs/style.css
--rw-r--r--   0        0        0      196 2021-10-30 13:54:10.202605 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/mkdocs/yield.html
--rw-r--r--   0        0        0      545 2021-10-30 13:54:09.842609 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/exceptions.html
--rw-r--r--   0        0        0      601 2021-11-06 17:58:09.459000 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/other_parameters.html
--rw-r--r--   0        0        0      618 2021-11-06 17:59:12.206399 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/parameters.html
--rw-r--r--   0        0        0      494 2021-11-06 17:58:14.115000 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/returns.html
--rw-r--r--   0        0        0      600 2021-10-30 13:54:09.942608 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/style.css
--rw-r--r--   0        0        0      490 2021-11-06 17:58:20.568000 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/yields.html
--rw-r--r--   0        0        0       37 2022-02-07 16:51:30.472324 mkdocstrings-python-0.9.0/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      194 2022-02-07 16:51:30.472324 mkdocstrings-python-0.9.0/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      295 2022-02-07 16:51:30.472324 mkdocstrings-python-0.9.0/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0      689 2022-02-08 11:16:01.880696 mkdocstrings-python-0.9.0/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2022-02-08 11:16:01.880696 mkdocstrings-python-0.9.0/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2022-02-08 11:16:01.880696 mkdocstrings-python-0.9.0/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        9 2022-02-08 11:16:01.397369 mkdocstrings-python-0.9.0/tests/.pytest_cache/v/randomly_seed
--rw-r--r--   0        0        0      174 2023-04-01 14:36:13.194677 mkdocstrings-python-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0     3042 2023-04-01 15:31:03.805108 mkdocstrings-python-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0     3222 2023-04-01 15:27:04.848491 mkdocstrings-python-0.9.0/tests/test_handler.py
--rw-r--r--   0        0        0     1515 2023-04-01 15:25:49.732868 mkdocstrings-python-0.9.0/tests/test_rendering.py
--rw-r--r--   0        0        0     1332 2023-04-01 15:22:56.275453 mkdocstrings-python-0.9.0/tests/test_themes.py
--rw-r--r--   0        0        0     5203 1970-01-01 00:00:00.000000 mkdocstrings-python-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-05-11 08:57:22.621862 mkdocstrings_python-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4243 2023-05-11 08:57:25.185137 mkdocstrings_python-1.0.0/README.md
+-rw-r--r--   0        0        0     2606 2023-05-11 10:08:32.951065 mkdocstrings_python-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-11 08:57:22.365201 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/py.typed
+-rw-r--r--   0        0        0      326 2023-05-01 15:54:09.233042 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/__init__.py
+-rw-r--r--   0        0        0    17985 2023-05-11 09:46:36.018635 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/handler.py
+-rw-r--r--   0        0        0     7542 2023-05-11 09:40:34.155577 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/rendering.py
+-rw-r--r--   0        0        0     2532 2022-04-29 13:33:38.953329 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html
+-rw-r--r--   0        0        0     5053 2023-05-01 15:54:09.233042 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/children.html
+-rw-r--r--   0        0        0     4078 2023-05-11 09:36:36.899109 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/class.html
+-rw-r--r--   0        0        0     1740 2023-03-03 13:20:57.896481 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html
+-rw-r--r--   0        0        0      274 2023-05-01 15:54:09.233042 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/admonition.html
+-rw-r--r--   0        0        0     2465 2022-04-29 23:09:02.903315 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html
+-rw-r--r--   0        0        0      400 2022-03-01 18:29:05.585970 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/examples.html
+-rw-r--r--   0        0        0     2475 2022-04-29 23:09:07.859915 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html
+-rw-r--r--   0        0        0     3134 2022-04-29 23:09:10.543213 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html
+-rw-r--r--   0        0        0     2132 2022-04-29 23:09:12.233190 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html
+-rw-r--r--   0        0        0     3111 2022-04-29 23:09:14.279830 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html
+-rw-r--r--   0        0        0     3081 2022-04-29 23:09:16.163138 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html
+-rw-r--r--   0        0        0     2115 2022-04-29 23:09:18.059779 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html
+-rw-r--r--   0        0        0     3051 2022-04-29 23:09:20.759743 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html
+-rw-r--r--   0        0        0      674 2023-05-11 09:36:36.899109 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/expression.html
+-rw-r--r--   0        0        0     2436 2023-05-11 09:36:36.899109 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/function.html
+-rw-r--r--   0        0        0      245 2022-05-08 08:40:49.298304 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/labels.html
+-rw-r--r--   0        0        0     1852 2022-04-29 17:36:56.831573 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/module.html
+-rw-r--r--   0        0        0     2698 2023-05-11 09:36:36.899109 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/signature.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/attribute.html
+-rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/children.html
+-rw-r--r--   0        0        0       33 2021-11-03 19:53:40.146116 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/class.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring.html
+-rw-r--r--   0        0        0       48 2022-02-01 20:48:46.512716 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring/admonition.html
+-rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring/attributes.html
+-rw-r--r--   0        0        0       46 2021-11-03 19:54:24.832142 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring/examples.html
+-rw-r--r--   0        0        0       54 2021-11-03 19:54:24.832142 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring/other_parameters.html
+-rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring/parameters.html
+-rw-r--r--   0        0        0       44 2021-11-22 18:41:47.281610 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring/raises.html
+-rw-r--r--   0        0        0       46 2021-11-22 18:41:51.551545 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring/receives.html
+-rw-r--r--   0        0        0       45 2021-11-03 19:54:24.832142 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring/returns.html
+-rw-r--r--   0        0        0       43 2021-11-22 18:41:56.598136 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring/warns.html
+-rw-r--r--   0        0        0       44 2021-11-03 19:54:24.832142 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/docstring/yields.html
+-rw-r--r--   0        0        0       38 2021-11-08 00:26:56.388000 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/expression.html
+-rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/function.html
+-rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/labels.html
+-rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/module.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/signature.html
+-rw-r--r--   0        0        0      703 2022-03-03 18:21:59.514950 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/style.css
+-rw-r--r--   0        0        0      224 2021-10-30 13:54:10.019274 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/mkdocs/exceptions.html
+-rw-r--r--   0        0        0      277 2021-10-30 13:54:10.202605 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/mkdocs/keyword_args.html
+-rw-r--r--   0        0        0      293 2021-10-30 13:54:10.019274 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/mkdocs/parameters.html
+-rw-r--r--   0        0        0      200 2021-10-30 13:54:10.092606 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/mkdocs/return.html
+-rw-r--r--   0        0        0      137 2021-10-30 13:54:10.199272 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/mkdocs/style.css
+-rw-r--r--   0        0        0      196 2021-10-30 13:54:10.202605 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/mkdocs/yield.html
+-rw-r--r--   0        0        0      545 2021-10-30 13:54:09.842609 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/readthedocs/exceptions.html
+-rw-r--r--   0        0        0      601 2021-11-06 17:58:09.459000 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/readthedocs/other_parameters.html
+-rw-r--r--   0        0        0      618 2021-11-06 17:59:12.206399 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/readthedocs/parameters.html
+-rw-r--r--   0        0        0      494 2021-11-06 17:58:14.115000 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/readthedocs/returns.html
+-rw-r--r--   0        0        0      600 2021-10-30 13:54:09.942608 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/readthedocs/style.css
+-rw-r--r--   0        0        0      490 2021-11-06 17:58:20.568000 mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/readthedocs/yields.html
+-rw-r--r--   0        0        0      174 2023-05-11 08:57:22.358534 mkdocstrings_python-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     3042 2023-05-11 08:57:25.185137 mkdocstrings_python-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     3222 2023-05-01 15:54:09.233042 mkdocstrings_python-1.0.0/tests/test_handler.py
+-rw-r--r--   0        0        0     1975 2023-05-11 09:36:36.899109 mkdocstrings_python-1.0.0/tests/test_rendering.py
+-rw-r--r--   0        0        0     1332 2023-05-01 15:54:09.233042 mkdocstrings_python-1.0.0/tests/test_themes.py
+-rw-r--r--   0        0        0     5749 1970-01-01 00:00:00.000000 mkdocstrings_python-1.0.0/PKG-INFO
```

### Comparing `mkdocstrings-python-0.9.0/LICENSE` & `mkdocstrings_python-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/README.md` & `mkdocstrings_python-1.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,21 @@
   </a>
 </p>
 
 ---
 
 <p align="center"><img src="logo.png"></p>
 
+The Python handler uses [Griffe](https://mkdocstrings.github.io/griffe)
+to collect documentation from Python source code.
+The word "griffe" can sometimes be used instead of "signature" in French.
+Griffe is able to visit the Abstract Syntax Tree (AST) of the source code to extract useful information.
+It is also able to execute the code (by importing it) and introspect objects in memory
+when source code is not available. Finally, it can parse docstrings following different styles.
+
 ## Installation
 
 You can install this handler as a *mkdocstrings* extra:
 
 ```toml title="pyproject.toml"
 # PEP 621 dependencies declaration
 # adapt to your dependencies manager
```

#### html2text {}

```diff
@@ -1,39 +1,46 @@
                        ****** mkdocstrings-python ******
                       A Python handler for mkdocstrings.
              [ci] [documentation] [pypi_version] [gitpod] [gitter]
 ---
                                   [logo.png]
-## Installation You can install this handler as a *mkdocstrings* extra: ```toml
-title="pyproject.toml" # PEP 621 dependencies declaration # adapt to your
-dependencies manager [project] dependencies = [ "mkdocstrings[python]>=0.18", ]
-``` You can also explicitly depend on the handler: ```toml
-title="pyproject.toml" # PEP 621 dependencies declaration # adapt to your
-dependencies manager [project] dependencies = [ "mkdocstrings-python", ] ``` ##
-Preview  ![mkdocstrings_python_gif](https://user-images.githubusercontent.com/
-3999221/77157838-7184db80-6aa2-11ea-9f9a-fe77405202de.gif) ## Features - **Data
-collection from source code**: collection of the object-tree and the docstrings
-is done thanks to [Griffe](https://github.com/mkdocstrings/griffe). - **Support
-for type annotations:** Griffe collects your type annotations and
-*mkdocstrings* uses them to display parameter types or return types. It is even
-able to automatically add cross-references to other objects from your API, from
-the standard library or third-party libraries! See [how to load inventories]
-(https://mkdocstrings.github.io/usage/#cross-references-to-other-projects-
-inventories) to enable it. - **Recursive documentation of Python objects:**
-just use the module dotted-path as an identifier, and you get the full module
-docs. You don't need to inject documentation for each class, function, etc. -
-**Support for documented attributes:** attributes (variables) followed by a
-docstring (triple-quoted string) will be recognized by Griffe in modules,
-classes and even in `__init__` methods. - **Multiple docstring-styles support:
-** common support for Google-style, Numpydoc-style, and Sphinx-style
-docstrings. See [Griffe's documentation](https://mkdocstrings.github.io/griffe/
-docstrings/) on docstrings support. - **Admonition support in Google
-docstrings:** blocks like `Note:` or `Warning:` will be transformed to their
-[admonition](https://squidfunk.github.io/mkdocs-material/reference/admonitions/
-) equivalent. *We do not support nested admonitions in docstrings!* - **Every
-object has a TOC entry:** we render a heading for each object, meaning *MkDocs*
-picks them into the Table of Contents, which is nicely displayed by the
-Material theme. Thanks to *mkdocstrings* cross-reference ability, you can
-reference other objects within your docstrings, with the classic Markdown
-syntax: `[this object][package.module.object]` or directly with `
-[package.module.object][]` - **Source code display:** *mkdocstrings* can add a
-collapsible div containing the highlighted source code of the Python object.
+The Python handler uses [Griffe](https://mkdocstrings.github.io/griffe) to
+collect documentation from Python source code. The word "griffe" can sometimes
+be used instead of "signature" in French. Griffe is able to visit the Abstract
+Syntax Tree (AST) of the source code to extract useful information. It is also
+able to execute the code (by importing it) and introspect objects in memory
+when source code is not available. Finally, it can parse docstrings following
+different styles. ## Installation You can install this handler as a
+*mkdocstrings* extra: ```toml title="pyproject.toml" # PEP 621 dependencies
+declaration # adapt to your dependencies manager [project] dependencies =
+[ "mkdocstrings[python]>=0.18", ] ``` You can also explicitly depend on the
+handler: ```toml title="pyproject.toml" # PEP 621 dependencies declaration #
+adapt to your dependencies manager [project] dependencies = [ "mkdocstrings-
+python", ] ``` ## Preview  ![mkdocstrings_python_gif](https://user-
+images.githubusercontent.com/3999221/77157838-7184db80-6aa2-11ea-9f9a-
+fe77405202de.gif) ## Features - **Data collection from source code**:
+collection of the object-tree and the docstrings is done thanks to [Griffe]
+(https://github.com/mkdocstrings/griffe). - **Support for type annotations:**
+Griffe collects your type annotations and *mkdocstrings* uses them to display
+parameter types or return types. It is even able to automatically add cross-
+references to other objects from your API, from the standard library or third-
+party libraries! See [how to load inventories](https://mkdocstrings.github.io/
+usage/#cross-references-to-other-projects-inventories) to enable it. -
+**Recursive documentation of Python objects:** just use the module dotted-path
+as an identifier, and you get the full module docs. You don't need to inject
+documentation for each class, function, etc. - **Support for documented
+attributes:** attributes (variables) followed by a docstring (triple-quoted
+string) will be recognized by Griffe in modules, classes and even in `__init__`
+methods. - **Multiple docstring-styles support:** common support for Google-
+style, Numpydoc-style, and Sphinx-style docstrings. See [Griffe's
+documentation](https://mkdocstrings.github.io/griffe/docstrings/) on docstrings
+support. - **Admonition support in Google docstrings:** blocks like `Note:` or
+`Warning:` will be transformed to their [admonition](https://
+squidfunk.github.io/mkdocs-material/reference/admonitions/) equivalent. *We do
+not support nested admonitions in docstrings!* - **Every object has a TOC
+entry:** we render a heading for each object, meaning *MkDocs* picks them into
+the Table of Contents, which is nicely displayed by the Material theme. Thanks
+to *mkdocstrings* cross-reference ability, you can reference other objects
+within your docstrings, with the classic Markdown syntax: `[this object]
+[package.module.object]` or directly with `[package.module.object][]` -
+**Source code display:** *mkdocstrings* can add a collapsible div containing
+the highlighted source code of the Python object.
```

### Comparing `mkdocstrings-python-0.9.0/pyproject.toml` & `mkdocstrings_python-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [build-system]
 requires = [
-    "pdm-pep517",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
 
 [project]
 name = "mkdocstrings-python"
 description = "A Python handler for mkdocstrings."
 authors = [
     { name = "Timothée Mazzucotelli", email = "pawamoy@pm.me" },
 ]
-license = "ISC"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = []
 dynamic = []
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -32,49 +31,65 @@
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
     "mkdocstrings>=0.20",
     "griffe>=0.24",
 ]
-version = "0.9.0"
+version = "1.0.0"
+
+[project.license]
+text = "ISC"
 
 [project.urls]
 Homepage = "https://mkdocstrings.github.io/python"
 Documentation = "https://mkdocstrings.github.io/python"
 Changelog = "https://mkdocstrings.github.io/python/changelog"
 Repository = "https://github.com/mkdocstrings/python"
 Issues = "https://github.com/mkdocstrings/python/issues"
 Discussions = "https://github.com/mkdocstrings/python/discussions"
 Gitter = "https://gitter.im/python/community"
 Funding = "https://github.com/sponsors/mkdocstrings"
 
+[tool.pdm]
+plugins = [
+    "pdm-multirun",
+]
+
 [tool.pdm.version]
 source = "scm"
 
 [tool.pdm.build]
 package-dir = "src"
 includes = [
     "src/mkdocstrings_handlers",
 ]
 editable-backend = "editables"
 
 [tool.pdm.dev-dependencies]
 duty = [
-    "duty>=0.8",
+    "duty>=0.10",
+]
+ci-quality = [
+    "mkdocstrings-python[duty,docs,quality,typing,security]",
+]
+ci-tests = [
+    "mkdocstrings-python[duty,docs,tests]",
 ]
 docs = [
+    "black>=23.1",
+    "markdown-callouts>=0.2",
+    "markdown-exec>=0.5",
     "mkdocs>=1.3",
     "mkdocs-coverage>=0.2",
     "mkdocs-gen-files>=0.3",
+    "mkdocs-git-committers-plugin-2>=1.1",
     "mkdocs-literate-nav>=0.4",
     "mkdocs-material>=7.3",
-    "mkdocs-section-index>=0.3",
-    "markdown-callouts>=0.2",
-    "markdown-exec>=0.5",
+    "mkdocs-minify-plugin>=0.6.4",
     "toml>=0.10",
 ]
 maintain = [
     "black>=23.1",
     "blacken-docs>=1.13",
     "git-changelog>=1.0",
 ]
@@ -86,12 +101,13 @@
     "pytest-cov>=3.0",
     "pytest-randomly>=3.10",
     "pytest-xdist>=2.4",
 ]
 typing = [
     "mypy>=0.911",
     "types-markdown>=3.3",
+    "types-pyyaml>=6.0",
     "types-toml>=0.10",
 ]
 security = [
     "safety>=2",
 ]
```

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/handler.py` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
         "show_root_full_path": True,
         "show_root_members_full_path": False,
         "show_object_full_path": False,
         "show_category_heading": False,
         "show_if_no_docstring": False,
         "show_signature": True,
         "show_signature_annotations": False,
+        "signature_crossrefs": False,
         "separate_signature": False,
         "line_length": 60,
         "merge_init_into_class": False,
         "show_docstring_attributes": True,
         "show_docstring_description": True,
         "show_docstring_examples": True,
         "show_docstring_other_parameters": True,
@@ -105,16 +106,31 @@
         "members_order": rendering.Order.alphabetical.value,
         "docstring_section_style": "table",
         "members": None,
         "filters": ["!^_[^_]"],
         "annotations_path": "brief",
         "preload_modules": None,
         "load_external_modules": False,
+        "allow_inspection": True,
     }
     """
+    Attributes: General options:
+        allow_inspection (bool): Whether to allow inspecting modules when visiting them is not possible. Default: `True`.
+        show_bases (bool): Show the base classes of a class. Default: `True`.
+        show_source (bool): Show the source code of this object. Default: `True`.
+        preload_modules (list[str] | None): Pre-load modules that are
+            not specified directly in autodoc instructions (`::: identifier`).
+            It is useful when you want to render documentation for a particular member of an object,
+            and this member is imported from another package than its parent.
+
+            For an imported member to be rendered, you need to add it to the `__all__` attribute
+            of the importing module.
+
+            The modules must be listed as an array of strings. Default: `None`.
+
     Attributes: Headings options:
         heading_level (int): The initial heading level to use. Default: `2`.
         show_root_heading (bool): Show the heading of the object at the root of the documentation tree
             (i.e. the object referenced by the identifier after `:::`). Default: `False`.
         show_root_toc_entry (bool): If the root heading is not shown, at least add a ToC entry for it. Default: `True`.
         show_root_full_path (bool): Show the full Python path for the root object heading. Default: `True`.
         show_root_members_full_path (bool): Show the full Python path of the root members. Default: `False`.
@@ -132,15 +148,14 @@
         group_by_category (bool): Group the object's children by categories: attributes, classes, functions, and modules. Default: `True`.
         show_submodules (bool): When rendering a module, show its submodules recursively. Default: `False`.
 
     Attributes: Docstrings options:
         docstring_style (str): The docstring style to use: `google`, `numpy`, `sphinx`, or `None`. Default: `"google"`.
         docstring_options (dict): The options for the docstring parser. See parsers under [`griffe.docstrings`][].
         docstring_section_style (str): The style used to render docstring sections. Options: `table`, `list`, `spacy`. Default: `"table"`.
-        line_length (int): Maximum line length when formatting code/signatures. Default: `60`.
         merge_init_into_class (bool): Whether to merge the `__init__` method into the class' signature and docstring. Default: `False`.
         show_if_no_docstring (bool): Show the object heading even if it has no docstring or children with docstrings. Default: `False`.
         show_docstring_attributes (bool): Whether to display the "Attributes" section in the object's docstring. Default: `True`.
         show_docstring_description (bool): Whether to display the textual block (including admonitions) in the object's docstring. Default: `True`.
         show_docstring_examples (bool): Whether to display the "Examples" section in the object's docstring. Default: `True`.
         show_docstring_other_parameters (bool): Whether to display the "Other Parameters" section in the object's docstring. Default: `True`.
         show_docstring_parameters (bool): Whether to display the "Parameters" section in the object's docstring. Default: `True`.
@@ -148,32 +163,20 @@
         show_docstring_receives (bool): Whether to display the "Receives" section in the object's docstring. Default: `True`.
         show_docstring_returns (bool): Whether to display the "Returns" section in the object's docstring. Default: `True`.
         show_docstring_warns (bool): Whether to display the "Warns" section in the object's docstring. Default: `True`.
         show_docstring_yields (bool): Whether to display the "Yields" section in the object's docstring. Default: `True`.
 
     Attributes: Signatures/annotations options:
         annotations_path (str): The verbosity for annotations path: `brief` (recommended), or `source` (as written in the source). Default: `"brief"`.
+        line_length (int): Maximum line length when formatting code/signatures. Default: `60`.
         show_signature (bool): Show methods and functions signatures. Default: `True`.
         show_signature_annotations (bool): Show the type annotations in methods and functions signatures. Default: `False`.
+        signature_crossrefs (bool): Whether to render cross-references for type annotations in signatures. Default: `False`.
         separate_signature (bool): Whether to put the whole signature in a code block below the heading.
             If Black is installed, the signature is also formatted using it. Default: `False`.
-
-    Attributes: Additional options:
-        show_bases (bool): Show the base classes of a class. Default: `True`.
-        show_source (bool): Show the source code of this object. Default: `True`.
-        preload_modules (list[str] | None): Pre-load modules that are
-            not specified directly in autodoc instructions (`::: identifier`).
-            It is useful when you want to render documentation for a particular member of an object,
-            and this member is imported from another package than its parent.
-
-            For an imported member to be rendered, you need to add it to the `__all__` attribute
-            of the importing module.
-
-            The modules must be listed as an array of strings. Default: `None`.
-
     """
 
     def __init__(
         self,
         *args: Any,
         config_file_path: str | None = None,
         paths: list[str] | None = None,
@@ -253,14 +256,15 @@
             loader = GriffeLoader(
                 extensions=load_extensions(final_config.get("extensions", [])),
                 search_paths=self._paths,
                 docstring_parser=parser,
                 docstring_options=parser_options,
                 modules_collection=self._modules_collection,
                 lines_collection=self._lines_collection,
+                allow_inspection=final_config["allow_inspection"],
             )
             try:
                 for pre_loaded_module in final_config.get("preload_modules") or []:
                     if pre_loaded_module not in self._modules_collection:
                         loader.load_module(pre_loaded_module)
                 loader.load_module(module_name)
             except ImportError as error:
@@ -308,14 +312,17 @@
             ) from error
 
         if final_config["filters"]:
             final_config["filters"] = [
                 (re.compile(filtr.lstrip("!")), filtr.startswith("!")) for filtr in final_config["filters"]
             ]
 
+        # TODO: goal reached: remove once `signature_crossrefs` feature becomes public
+        final_config["signature_crossrefs"] = False
+
         return template.render(
             **{"config": final_config, data.kind.value: data, "heading_level": heading_level, "root": True},
         )
 
     def update_env(self, md: Markdown, config: dict) -> None:  # noqa: D102 (ignore missing docstring)
         super().update_env(md, config)
         self.env.trim_blocks = True
@@ -323,20 +330,21 @@
         self.env.keep_trailing_newline = False
         self.env.filters["crossref"] = rendering.do_crossref
         self.env.filters["multi_crossref"] = rendering.do_multi_crossref
         self.env.filters["order_members"] = rendering.do_order_members
         self.env.filters["format_code"] = rendering.do_format_code
         self.env.filters["format_signature"] = rendering.do_format_signature
         self.env.filters["filter_objects"] = rendering.do_filter_objects
+        self.env.filters["stash_crossref"] = lambda ref, length: ref
 
-    def get_anchors(self, data: CollectorItem) -> list[str]:  # noqa: D102 (ignore missing docstring)
+    def get_anchors(self, data: CollectorItem) -> set[str]:  # noqa: D102 (ignore missing docstring)
         try:
-            return list({data.path, data.canonical_path, *data.aliases})
+            return {data.path, data.canonical_path, *data.aliases}
         except AliasResolutionError:
-            return [data.path]
+            return {data.path}
 
 
 def get_handler(
     theme: str,
     custom_templates: str | None = None,
     config_file_path: str | None = None,
     paths: list[str] | None = None,
```

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/rendering.py` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/rendering.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 
 import enum
 import re
 import sys
 from functools import lru_cache
 from typing import TYPE_CHECKING, Any, Callable, Match, Pattern, Sequence
 
+from jinja2 import pass_context
 from markupsafe import Markup
 from mkdocstrings.loggers import get_logger
 
 if TYPE_CHECKING:
-    from griffe.dataclasses import Alias, Object
+    from griffe.dataclasses import Alias, Function, Object
+    from jinja2.runtime import Context
     from mkdocstrings.handlers.base import CollectorItem
 
 logger = get_logger(__name__)
 
 
 class Order(enum.Enum):
     """Enumeration for the possible members ordering."""
@@ -56,31 +58,57 @@
     code = code.strip()
     if len(code) < line_length:
         return code
     formatter = _get_black_formatter()
     return formatter(code, line_length)
 
 
-def do_format_signature(signature: str, line_length: int) -> str:
+def _format_signature(name: Markup, signature: str, line_length: int) -> str:
+    name = str(name).strip()  # type: ignore[assignment]
+    signature = signature.strip()
+    if len(name + signature) < line_length:
+        return name + signature
+
+    # Black cannot format names with dots, so we replace
+    # the whole name with a string of equal length
+    name_length = len(name)
+    formatter = _get_black_formatter()
+    formatable = f"def {'x' * name_length}{signature}: pass"
+    formatted = formatter(formatable, line_length)
+
+    # We put back the original name
+    # and remove starting `def ` and trailing `: pass`
+    return name + formatted[4:-5].strip()[name_length:-1]
+
+
+@pass_context
+def do_format_signature(
+    context: Context,
+    callable_path: Markup,
+    function: Function,
+    line_length: int,
+    *,
+    crossrefs: bool = False,  # noqa: ARG001
+) -> str:
     """Format a signature using Black.
 
     Parameters:
-        signature: The signature to format.
+        callable_path: The path of the callable we render the signature of.
         line_length: The line length to give to Black.
+        crossrefs: Whether to cross-reference types in the signature.
 
     Returns:
         The same code, formatted.
     """
-    code = signature.strip()
-    if len(code) < line_length:
-        return code
-    formatter = _get_black_formatter()
-    formatted = formatter(f"def {code}: pass", line_length)
-    # remove starting `def ` and trailing `: pass`
-    return formatted[4:-5].strip()[:-1]
+    env = context.environment
+    template = env.get_template("signature.html")
+    signature = template.render(context.parent, function=function)
+    signature = _format_signature(callable_path, signature, line_length)
+    signature = str(env.filters["highlight"](signature, language="python", inline=False))
+    return signature
 
 
 def do_order_members(
     members: Sequence[Object | Alias],
     order: Order,
     members_list: list[str] | None,
 ) -> Sequence[Object | Alias]:
@@ -181,32 +209,42 @@
             When given and empty, return an empty list.
             When given and not empty, ignore filters and docstrings presence/absence.
         keep_no_docstrings: Whether to keep objects with no/empty docstrings (recursive check).
 
     Returns:
         A list of objects.
     """
-    if members_list is not None:
-        if not members_list:
-            return []
-        return [obj for obj in objects_dictionary.values() if obj.name in set(members_list)]
+    # no members
+    if members_list is False or members_list == []:
+        return []
+
     objects = list(objects_dictionary.values())
+
+    # all members
+    if members_list is True:
+        return objects
+
+    # list of members
+    if members_list is not None:
+        return [obj for obj in objects if obj.name in set(members_list)]
+
+    # none, use filters and docstrings
     if filters:
         objects = [obj for obj in objects if _keep_object(obj.name, filters)]
     if keep_no_docstrings:
         return objects
     return [obj for obj in objects if obj.has_docstrings]
 
 
 @lru_cache(maxsize=1)
 def _get_black_formatter() -> Callable[[str, int], str]:
     try:
         from black import Mode, format_str
     except ModuleNotFoundError:
-        logger.warning("Formatting signatures requires Black to be installed.")
+        logger.info("Formatting signatures requires Black to be installed.")
         return lambda text, _: text
 
     def formatter(code: str, line_length: int) -> str:
         mode = Mode(line_length=line_length)
         return format_str(code, mode=mode)
 
     return formatter
```

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/children.html` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/children.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/class.html` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/class.html`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,16 @@
       {% endwith %}
 
     {% endfilter %}
 
     {% if config.separate_signature and config.merge_init_into_class %}
       {% if "__init__" in class.members %}
         {% with function = class.members["__init__"] %}
-          {% filter highlight(language="python", inline=False) %}
-            {% filter format_signature(config.line_length) %}
-              {% if show_full_path %}{{ class.path }}{% else %}{{ class.name }}{% endif %}
-              {% include "signature.html" with context %}
-            {% endfilter %}
+          {% filter format_signature(function, config.line_length, crossrefs=config.signature_crossrefs) %}
+            {% if show_full_path %}{{ class.path }}{% else %}{{ class.name }}{% endif %}
           {% endfilter %}
         {% endwith %}
       {% endif %}
     {% endif %}
 
   {% else %}
     {% if config.show_root_toc_entry %}
```

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/expression.html` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/expression.html`

 * *Files 12% similar despite different names*

```diff
@@ -3,10 +3,12 @@
   {%- for expression in original_expression -%}
     {%- include "expression.html" with context -%}
   {%- endfor -%}
 {%- elif original_expression is string -%}
   {{ original_expression }}
 {%- else -%}
   {%- with annotation = original_expression|attr(config.annotations_path) -%}
-    <span data-autorefs-optional{% if annotation != original_expression.full %}-hover{% endif %}="{{ original_expression.full }}">{{ annotation }}</span>
+    {%- filter stash_crossref(length=annotation|length) -%}
+      <span data-autorefs-optional{% if annotation != original_expression.full %}-hover{% endif %}="{{ original_expression.full }}">{{ annotation }}</span>
+    {%- endfilter -%}
   {%- endwith -%}
 {%- endif -%}
```

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/function.html` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/function.html`

 * *Files 10% similar despite different names*

```diff
@@ -33,19 +33,16 @@
       {% with labels = function.labels %}
         {% include "labels.html" with context %}
       {% endwith %}
 
     {% endfilter %}
 
     {% if config.separate_signature %}
-      {% filter highlight(language="python", inline=False) %}
-        {% filter format_signature(config.line_length) %}
-          {% if show_full_path %}{{ function.path }}{% else %}{{ function.name }}{% endif %}
-          {% include "signature.html" with context %}
-        {% endfilter %}
+      {% filter format_signature(function, config.line_length, crossrefs=config.signature_crossrefs) %}
+        {% if show_full_path %}{{ function.path }}{% else %}{{ function.name }}{% endif %}
       {% endfilter %}
     {% endif %}
 
   {% else %}
     {% if config.show_root_toc_entry %}
       {% filter heading(heading_level,
           role="function",
```

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/module.html` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/module.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/signature.html` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/_base/signature.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 {%- if config.show_signature -%}
   {{ log.debug("Rendering signature") }}
   {%- with -%}
 
-    {%- set ns = namespace(has_pos_only=False, render_pos_only_separator=True, render_kw_only_separator=True, equal="=") -%}
+    {%- set ns = namespace(
+          has_pos_only=False,
+          render_pos_only_separator=True,
+          render_kw_only_separator=True,
+          annotation="",
+          equal="=",
+        )
+    -%}
 
     {%- if config.show_signature_annotations -%}
       {%- set ns.equal = " = " -%}
     {%- endif -%}
 
     (
       {%- for parameter in function.parameters -%}
@@ -20,29 +27,40 @@
             {%- if parameter.kind.value == "keyword-only" -%}
               {%- if ns.render_kw_only_separator -%}
                 {%- set ns.render_kw_only_separator = False %}*, {% endif -%}
             {%- endif -%}
           {%- endif -%}
 
           {%- if config.show_signature_annotations and parameter.annotation is not none -%}
-            {%- set annotation = ": " + parameter.annotation|safe -%}
+            {%- if config.separate_signature and config.signature_crossrefs -%}
+              {%- with expression = parameter.annotation -%}
+                {%- set ns.annotation -%}: {% include "expression.html" with context %}{%- endset -%}
+              {%- endwith -%}
+            {%- else -%}
+              {%- set ns.annotation = ": " + parameter.annotation|safe -%}
+            {%- endif -%}
           {%- endif -%}
 
           {%- if parameter.default is not none and parameter.kind.value != "variadic positional" and parameter.kind.value != "variadic keyword" -%}
             {%- set default = ns.equal + parameter.default|safe -%}
           {%- endif -%}
 
           {%- if parameter.kind.value == "variadic positional" -%}
             {%- set ns.render_kw_only_separator = False -%}
           {%- endif -%}
 
           {% if parameter.kind.value == "variadic positional" %}*{% elif parameter.kind.value == "variadic keyword" %}**{% endif -%}
-          {{ parameter.name }}{{ annotation }}{{ default }}
+          {{ parameter.name }}{{ ns.annotation }}{{ default }}
           {%- if not loop.last %}, {% endif -%}
 
         {%- endif -%}
       {%- endfor -%}
     )
-    {%- if config.show_signature_annotations and function.annotation %} -> {{ function.annotation|safe }}{%- endif -%}
+    {%- if config.show_signature_annotations and function.annotation %} -> {% if config.separate_signature and config.signature_crossrefs -%}
+        {%- with expression = function.annotation %}{% include "expression.html" with context %}{%- endwith -%}
+      {%- else -%}
+        {{ function.annotation|safe }}
+      {%- endif -%}
+    {%- endif -%}
 
   {%- endwith -%}
 {%- endif -%}
```

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/style.css` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/material/style.css`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/exceptions.html` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/readthedocs/exceptions.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/other_parameters.html` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/readthedocs/other_parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/parameters.html` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/readthedocs/parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/style.css` & `mkdocstrings_python-1.0.0/src/mkdocstrings_handlers/python/templates/readthedocs/style.css`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/tests/conftest.py` & `mkdocstrings_python-1.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/tests/test_handler.py` & `mkdocstrings_python-1.0.0/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/tests/test_rendering.py` & `mkdocstrings_python-1.0.0/tests/test_rendering.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,52 @@
 """Tests for the `rendering` module."""
 
 from __future__ import annotations
 
 import re
 from dataclasses import dataclass
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 import pytest
 
 from mkdocstrings_handlers.python import rendering
 
+if TYPE_CHECKING:
+    from markupsafe import Markup
 
-def test_format_code_and_signature() -> None:
-    """Assert code and signatures can be Black-formatted."""
-    assert rendering.do_format_code("print('Hello')", 100)
-    assert rendering.do_format_code('print("Hello")', 100)
-    assert rendering.do_format_signature("(param: str = 'hello') -> 'Class'", 100)
-    assert rendering.do_format_signature('(param: str = "hello") -> "Class"', 100)
+
+@pytest.mark.parametrize(
+    "code",
+    [
+        "print('Hello')",
+        "aaaaa(bbbbb, ccccc=1) + ddddd.eeeee[ffff] or {ggggg: hhhhh, iiiii: jjjjj}",
+    ],
+)
+def test_format_code(code: str) -> None:
+    """Assert code can be Black-formatted.
+
+    Parameters:
+        code: Code to format.
+    """
+    for length in (5, 100):
+        assert rendering.do_format_code(code, length)
+
+
+@pytest.mark.parametrize(
+    ("name", "signature"),
+    [("Class.method", "(param: str = 'hello') -> 'OtherClass'")],
+)
+def test_format_signature(name: Markup, signature: str) -> None:
+    """Assert signatures can be Black-formatted.
+
+    Parameters:
+        signature: Signature to format.
+    """
+    for length in (5, 100):
+        assert rendering._format_signature(name, signature, length)
 
 
 @dataclass
 class _FakeObject:
     name: str
```

### Comparing `mkdocstrings-python-0.9.0/tests/test_themes.py` & `mkdocstrings_python-1.0.0/tests/test_themes.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.9.0/PKG-INFO` & `mkdocstrings_python-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: mkdocstrings-python
-Version: 0.9.0
+Version: 1.0.0
 Summary: A Python handler for mkdocstrings.
+Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
 License: ISC
-Author-email: Timothée Mazzucotelli <pawamoy@pm.me>
-Requires-Python: >=3.7
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
+Project-URL: Homepage, https://mkdocstrings.github.io/python
+Project-URL: Documentation, https://mkdocstrings.github.io/python
 Project-URL: Changelog, https://mkdocstrings.github.io/python/changelog
+Project-URL: Repository, https://github.com/mkdocstrings/python
+Project-URL: Issues, https://github.com/mkdocstrings/python/issues
 Project-URL: Discussions, https://github.com/mkdocstrings/python/discussions
-Project-URL: Documentation, https://mkdocstrings.github.io/python
-Project-URL: Funding, https://github.com/sponsors/mkdocstrings
 Project-URL: Gitter, https://gitter.im/python/community
-Project-URL: Homepage, https://mkdocstrings.github.io/python
-Project-URL: Issues, https://github.com/mkdocstrings/python/issues
-Project-URL: Repository, https://github.com/mkdocstrings/python
+Project-URL: Funding, https://github.com/sponsors/mkdocstrings
+Requires-Python: >=3.7
+Requires-Dist: mkdocstrings>=0.20
+Requires-Dist: griffe>=0.24
 Description-Content-Type: text/markdown
 
 <h1 align="center">mkdocstrings-python</h1>
 
 <p align="center">A Python handler for <a href="https://github.com/mkdocstrings/mkdocstrings"><i>mkdocstrings</i></a>.</p>
 
 <p align="center">
@@ -52,14 +54,21 @@
   </a>
 </p>
 
 ---
 
 <p align="center"><img src="logo.png"></p>
 
+The Python handler uses [Griffe](https://mkdocstrings.github.io/griffe)
+to collect documentation from Python source code.
+The word "griffe" can sometimes be used instead of "signature" in French.
+Griffe is able to visit the Abstract Syntax Tree (AST) of the source code to extract useful information.
+It is also able to execute the code (by importing it) and introspect objects in memory
+when source code is not available. Finally, it can parse docstrings following different styles.
+
 ## Installation
 
 You can install this handler as a *mkdocstrings* extra:
 
 ```toml title="pyproject.toml"
 # PEP 621 dependencies declaration
 # adapt to your dependencies manager
@@ -111,8 +120,7 @@
 - **Every object has a TOC entry:** we render a heading for each object, meaning *MkDocs* picks them into the Table
   of Contents, which is nicely displayed by the Material theme. Thanks to *mkdocstrings* cross-reference ability,
   you can reference other objects within your docstrings, with the classic Markdown syntax:
   `[this object][package.module.object]` or directly with `[package.module.object][]`
 
 - **Source code display:** *mkdocstrings* can add a collapsible div containing the highlighted source code
   of the Python object.
-
```

#### html2text {}

```diff
@@ -1,59 +1,67 @@
-Metadata-Version: 2.1 Name: mkdocstrings-python Version: 0.9.0 Summary: A
-Python handler for mkdocstrings. License: ISC Author-email: TimothÃ©e
-Mazzucotelli
-pm.me> Requires-Python: >=3.7 Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers Classifier: Programming Language ::
-Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Metadata-Version: 2.1 Name: mkdocstrings-python Version: 1.0.0 Summary: A
+Python handler for mkdocstrings. Author-Email: TimothÃ©e Mazzucotelli
+pm.me> License: ISC Classifier: Development Status :: 4 - Beta Classifier:
+Intended Audience :: Developers Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Topic ::
+3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
 Documentation Classifier: Topic :: Software Development Classifier: Topic ::
 Software Development :: Documentation Classifier: Topic :: Utilities
-Classifier: Typing :: Typed Project-URL: Changelog, https://
-mkdocstrings.github.io/python/changelog Project-URL: Discussions, https://
-github.com/mkdocstrings/python/discussions Project-URL: Documentation, https://
-mkdocstrings.github.io/python Project-URL: Funding, https://github.com/
-sponsors/mkdocstrings Project-URL: Gitter, https://gitter.im/python/community
-Project-URL: Homepage, https://mkdocstrings.github.io/python Project-URL:
-Issues, https://github.com/mkdocstrings/python/issues Project-URL: Repository,
-https://github.com/mkdocstrings/python Description-Content-Type: text/markdown
+Classifier: Typing :: Typed Project-URL: Homepage, https://
+mkdocstrings.github.io/python Project-URL: Documentation, https://
+mkdocstrings.github.io/python Project-URL: Changelog, https://
+mkdocstrings.github.io/python/changelog Project-URL: Repository, https://
+github.com/mkdocstrings/python Project-URL: Issues, https://github.com/
+mkdocstrings/python/issues Project-URL: Discussions, https://github.com/
+mkdocstrings/python/discussions Project-URL: Gitter, https://gitter.im/python/
+community Project-URL: Funding, https://github.com/sponsors/mkdocstrings
+Requires-Python: >=3.7 Requires-Dist: mkdocstrings>=0.20 Requires-Dist:
+griffe>=0.24 Description-Content-Type: text/markdown
                        ****** mkdocstrings-python ******
                       A Python handler for mkdocstrings.
              [ci] [documentation] [pypi_version] [gitpod] [gitter]
 ---
                                   [logo.png]
-## Installation You can install this handler as a *mkdocstrings* extra: ```toml
-title="pyproject.toml" # PEP 621 dependencies declaration # adapt to your
-dependencies manager [project] dependencies = [ "mkdocstrings[python]>=0.18", ]
-``` You can also explicitly depend on the handler: ```toml
-title="pyproject.toml" # PEP 621 dependencies declaration # adapt to your
-dependencies manager [project] dependencies = [ "mkdocstrings-python", ] ``` ##
-Preview  ![mkdocstrings_python_gif](https://user-images.githubusercontent.com/
-3999221/77157838-7184db80-6aa2-11ea-9f9a-fe77405202de.gif) ## Features - **Data
-collection from source code**: collection of the object-tree and the docstrings
-is done thanks to [Griffe](https://github.com/mkdocstrings/griffe). - **Support
-for type annotations:** Griffe collects your type annotations and
-*mkdocstrings* uses them to display parameter types or return types. It is even
-able to automatically add cross-references to other objects from your API, from
-the standard library or third-party libraries! See [how to load inventories]
-(https://mkdocstrings.github.io/usage/#cross-references-to-other-projects-
-inventories) to enable it. - **Recursive documentation of Python objects:**
-just use the module dotted-path as an identifier, and you get the full module
-docs. You don't need to inject documentation for each class, function, etc. -
-**Support for documented attributes:** attributes (variables) followed by a
-docstring (triple-quoted string) will be recognized by Griffe in modules,
-classes and even in `__init__` methods. - **Multiple docstring-styles support:
-** common support for Google-style, Numpydoc-style, and Sphinx-style
-docstrings. See [Griffe's documentation](https://mkdocstrings.github.io/griffe/
-docstrings/) on docstrings support. - **Admonition support in Google
-docstrings:** blocks like `Note:` or `Warning:` will be transformed to their
-[admonition](https://squidfunk.github.io/mkdocs-material/reference/admonitions/
-) equivalent. *We do not support nested admonitions in docstrings!* - **Every
-object has a TOC entry:** we render a heading for each object, meaning *MkDocs*
-picks them into the Table of Contents, which is nicely displayed by the
-Material theme. Thanks to *mkdocstrings* cross-reference ability, you can
-reference other objects within your docstrings, with the classic Markdown
-syntax: `[this object][package.module.object]` or directly with `
-[package.module.object][]` - **Source code display:** *mkdocstrings* can add a
-collapsible div containing the highlighted source code of the Python object.
+The Python handler uses [Griffe](https://mkdocstrings.github.io/griffe) to
+collect documentation from Python source code. The word "griffe" can sometimes
+be used instead of "signature" in French. Griffe is able to visit the Abstract
+Syntax Tree (AST) of the source code to extract useful information. It is also
+able to execute the code (by importing it) and introspect objects in memory
+when source code is not available. Finally, it can parse docstrings following
+different styles. ## Installation You can install this handler as a
+*mkdocstrings* extra: ```toml title="pyproject.toml" # PEP 621 dependencies
+declaration # adapt to your dependencies manager [project] dependencies =
+[ "mkdocstrings[python]>=0.18", ] ``` You can also explicitly depend on the
+handler: ```toml title="pyproject.toml" # PEP 621 dependencies declaration #
+adapt to your dependencies manager [project] dependencies = [ "mkdocstrings-
+python", ] ``` ## Preview  ![mkdocstrings_python_gif](https://user-
+images.githubusercontent.com/3999221/77157838-7184db80-6aa2-11ea-9f9a-
+fe77405202de.gif) ## Features - **Data collection from source code**:
+collection of the object-tree and the docstrings is done thanks to [Griffe]
+(https://github.com/mkdocstrings/griffe). - **Support for type annotations:**
+Griffe collects your type annotations and *mkdocstrings* uses them to display
+parameter types or return types. It is even able to automatically add cross-
+references to other objects from your API, from the standard library or third-
+party libraries! See [how to load inventories](https://mkdocstrings.github.io/
+usage/#cross-references-to-other-projects-inventories) to enable it. -
+**Recursive documentation of Python objects:** just use the module dotted-path
+as an identifier, and you get the full module docs. You don't need to inject
+documentation for each class, function, etc. - **Support for documented
+attributes:** attributes (variables) followed by a docstring (triple-quoted
+string) will be recognized by Griffe in modules, classes and even in `__init__`
+methods. - **Multiple docstring-styles support:** common support for Google-
+style, Numpydoc-style, and Sphinx-style docstrings. See [Griffe's
+documentation](https://mkdocstrings.github.io/griffe/docstrings/) on docstrings
+support. - **Admonition support in Google docstrings:** blocks like `Note:` or
+`Warning:` will be transformed to their [admonition](https://
+squidfunk.github.io/mkdocs-material/reference/admonitions/) equivalent. *We do
+not support nested admonitions in docstrings!* - **Every object has a TOC
+entry:** we render a heading for each object, meaning *MkDocs* picks them into
+the Table of Contents, which is nicely displayed by the Material theme. Thanks
+to *mkdocstrings* cross-reference ability, you can reference other objects
+within your docstrings, with the classic Markdown syntax: `[this object]
+[package.module.object]` or directly with `[package.module.object][]` -
+**Source code display:** *mkdocstrings* can add a collapsible div containing
+the highlighted source code of the Python object.
```

