# Comparing `tmp/slicer_package_manager-0.7.1.tar.gz` & `tmp/slicer_package_manager-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slicer_package_manager-0.7.1.tar", last modified: Sat May 21 04:10:36 2022, max compression
+gzip compressed data, was "slicer_package_manager-0.8.0.tar", last modified: Thu May 11 02:54:22 2023, max compression
```

## Comparing `slicer_package_manager-0.7.1.tar` & `slicer_package_manager-0.8.0.tar`

### file list

```diff
@@ -1,162 +1,58 @@
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:36.244562 slicer_package_manager-0.7.1/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      148 2022-04-18 17:25:05.000000 slicer_package_manager-0.7.1/AUTHORS.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      600 2022-04-18 17:25:05.000000 slicer_package_manager-0.7.1/LICENSE
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      226 2022-04-18 17:25:05.000000 slicer_package_manager-0.7.1/MANIFEST.in
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1909 2022-05-21 04:10:36.244562 slicer_package_manager-0.7.1/PKG-INFO
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1109 2022-05-20 21:48:20.000000 slicer_package_manager-0.7.1/README.rst
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:36.228562 slicer_package_manager-0.7.1/docs/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1130 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/docs/Makefile
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:36.224562 slicer_package_manager-0.7.1/docs/_build/
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:36.228562 slicer_package_manager-0.7.1/docs/_build/doctrees/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3266 2022-05-20 21:16:55.000000 slicer_package_manager-0.7.1/docs/_build/doctrees/authors.doctree
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    48894 2022-05-20 21:16:55.000000 slicer_package_manager-0.7.1/docs/_build/doctrees/changes.doctree
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    90359 2022-05-20 21:16:56.000000 slicer_package_manager-0.7.1/docs/_build/doctrees/commands_shell.doctree
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    28539 2022-05-20 21:16:56.000000 slicer_package_manager-0.7.1/docs/_build/doctrees/concepts.doctree
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:36.232562 slicer_package_manager-0.7.1/docs/_build/doctrees/developer_guide/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    35919 2022-05-20 21:16:56.000000 slicer_package_manager-0.7.1/docs/_build/doctrees/developer_guide/develop.doctree
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2923 2022-05-20 21:16:56.000000 slicer_package_manager-0.7.1/docs/_build/doctrees/developer_guide/index.doctree
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    12231 2022-05-20 21:16:56.000000 slicer_package_manager-0.7.1/docs/_build/doctrees/developer_guide/install.doctree
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4727 2022-05-20 21:16:56.000000 slicer_package_manager-0.7.1/docs/_build/doctrees/developer_guide/overview.doctree
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    94651 2022-05-20 21:16:56.000000 slicer_package_manager-0.7.1/docs/_build/doctrees/developer_guide/slicer_package_manager.api.doctree
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    37896 2022-05-20 21:16:56.000000 slicer_package_manager-0.7.1/docs/_build/doctrees/developer_guide/slicer_package_manager.doctree
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    40345 2022-05-20 21:16:57.000000 slicer_package_manager-0.7.1/docs/_build/doctrees/developer_guide/slicer_package_manager.models.doctree
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)   152085 2022-05-20 21:16:57.000000 slicer_package_manager-0.7.1/docs/_build/doctrees/developer_guide/slicer_package_manager_client.doctree
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    87989 2022-05-20 21:16:57.000000 slicer_package_manager-0.7.1/docs/_build/doctrees/environment.pickle
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    26998 2022-05-20 21:16:57.000000 slicer_package_manager-0.7.1/docs/_build/doctrees/faq.doctree
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     7415 2022-05-20 21:16:57.000000 slicer_package_manager-0.7.1/docs/_build/doctrees/index.doctree
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    11662 2022-05-20 21:16:57.000000 slicer_package_manager-0.7.1/docs/_build/doctrees/installation.doctree
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    36677 2022-05-20 21:16:57.000000 slicer_package_manager-0.7.1/docs/_build/doctrees/make_a_release.doctree
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    17526 2022-05-20 21:16:57.000000 slicer_package_manager-0.7.1/docs/_build/doctrees/overview.doctree
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:36.232562 slicer_package_manager-0.7.1/docs/_build/html/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      230 2022-05-20 21:16:58.000000 slicer_package_manager-0.7.1/docs/_build/html/.buildinfo
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:36.232562 slicer_package_manager-0.7.1/docs/_build/html/_sources/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       28 2022-04-18 17:25:05.000000 slicer_package_manager-0.7.1/docs/_build/html/_sources/authors.rst.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       28 2022-04-18 17:25:05.000000 slicer_package_manager-0.7.1/docs/_build/html/_sources/changes.rst.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    13624 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/docs/_build/html/_sources/commands_shell.rst.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4774 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/docs/_build/html/_sources/concepts.rst.txt
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:36.232562 slicer_package_manager-0.7.1/docs/_build/html/_sources/developer_guide/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     5986 2022-05-20 21:01:47.000000 slicer_package_manager-0.7.1/docs/_build/html/_sources/developer_guide/develop.rst.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      172 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/docs/_build/html/_sources/developer_guide/index.rst.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2051 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/docs/_build/html/_sources/developer_guide/install.rst.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      430 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/docs/_build/html/_sources/developer_guide/overview.rst.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      378 2022-05-20 21:16:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_sources/developer_guide/slicer_package_manager.api.rst.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      618 2022-05-20 21:16:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_sources/developer_guide/slicer_package_manager.models.rst.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      636 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/docs/_build/html/_sources/developer_guide/slicer_package_manager.rst.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      455 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/docs/_build/html/_sources/developer_guide/slicer_package_manager_client.rst.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     5137 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/docs/_build/html/_sources/faq.rst.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      969 2022-05-20 20:58:17.000000 slicer_package_manager-0.7.1/docs/_build/html/_sources/index.rst.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1664 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/docs/_build/html/_sources/installation.rst.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     5300 2022-05-20 20:53:38.000000 slicer_package_manager-0.7.1/docs/_build/html/_sources/make_a_release.rst.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3359 2022-05-20 20:57:49.000000 slicer_package_manager-0.7.1/docs/_build/html/_sources/overview.rst.txt
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:36.236562 slicer_package_manager-0.7.1/docs/_build/html/_static/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    14692 2022-05-20 21:16:58.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/basic.css
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:36.236562 slicer_package_manager-0.7.1/docs/_build/html/_static/css/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3275 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/css/badge_only.css
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:36.240562 slicer_package_manager-0.7.1/docs/_build/html/_static/css/fonts/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    87624 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    67312 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    86288 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    66444 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)   165742 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)   444379 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)   165548 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    98024 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    77160 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)   323344 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)   193308 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)   309728 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)   184912 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)   328412 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)   195704 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)   309192 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)   182708 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)   129674 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/css/theme.css
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    10766 2022-05-19 14:25:53.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/doctools.js
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      422 2022-05-20 21:16:58.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/documentation_options.js
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      286 2022-05-19 14:25:53.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/file.png
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)   287630 2022-05-19 14:25:53.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/jquery-3.5.1.js
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    89476 2022-05-19 14:25:53.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/jquery.js
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:36.240562 slicer_package_manager-0.7.1/docs/_build/html/_static/js/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      934 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/js/badge_only.js
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4370 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2734 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/js/html5shiv.min.js
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     5023 2022-05-19 14:25:55.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/js/theme.js
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    10854 2022-05-20 21:16:58.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/language_data.js
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       90 2022-05-19 14:25:53.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/minus.png
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       90 2022-05-19 14:25:53.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/plus.png
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4846 2022-05-20 21:16:58.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/pygments.css
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    16634 2022-05-19 14:25:53.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/searchtools.js
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    68420 2022-05-19 14:25:53.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/underscore-1.13.1.js
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    19530 2022-05-19 14:25:53.000000 slicer_package_manager-0.7.1/docs/_build/html/_static/underscore.js
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     5167 2022-05-20 21:16:57.000000 slicer_package_manager-0.7.1/docs/_build/html/authors.html
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    22453 2022-05-20 21:16:57.000000 slicer_package_manager-0.7.1/docs/_build/html/changes.html
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    41056 2022-05-20 21:16:57.000000 slicer_package_manager-0.7.1/docs/_build/html/commands_shell.html
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    11190 2022-05-20 21:16:57.000000 slicer_package_manager-0.7.1/docs/_build/html/concepts.html
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:36.240562 slicer_package_manager-0.7.1/docs/_build/html/developer_guide/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    16260 2022-05-20 21:16:57.000000 slicer_package_manager-0.7.1/docs/_build/html/developer_guide/develop.html
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     9136 2022-05-20 21:16:57.000000 slicer_package_manager-0.7.1/docs/_build/html/developer_guide/index.html
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    10329 2022-05-20 21:16:57.000000 slicer_package_manager-0.7.1/docs/_build/html/developer_guide/install.html
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     6869 2022-05-20 21:16:57.000000 slicer_package_manager-0.7.1/docs/_build/html/developer_guide/overview.html
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    35631 2022-05-20 21:16:57.000000 slicer_package_manager-0.7.1/docs/_build/html/developer_guide/slicer_package_manager.api.html
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    22648 2022-05-20 21:16:57.000000 slicer_package_manager-0.7.1/docs/_build/html/developer_guide/slicer_package_manager.html
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    19967 2022-05-20 21:16:57.000000 slicer_package_manager-0.7.1/docs/_build/html/developer_guide/slicer_package_manager.models.html
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    54357 2022-05-20 21:16:57.000000 slicer_package_manager-0.7.1/docs/_build/html/developer_guide/slicer_package_manager_client.html
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    14768 2022-05-20 21:16:58.000000 slicer_package_manager-0.7.1/docs/_build/html/faq.html
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    23567 2022-05-20 21:16:58.000000 slicer_package_manager-0.7.1/docs/_build/html/genindex.html
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     6745 2022-05-20 21:16:58.000000 slicer_package_manager-0.7.1/docs/_build/html/index.html
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     7864 2022-05-20 21:16:58.000000 slicer_package_manager-0.7.1/docs/_build/html/installation.html
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    17128 2022-05-20 21:16:58.000000 slicer_package_manager-0.7.1/docs/_build/html/make_a_release.html
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1375 2022-05-20 21:16:58.000000 slicer_package_manager-0.7.1/docs/_build/html/objects.inv
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    13556 2022-05-20 21:16:58.000000 slicer_package_manager-0.7.1/docs/_build/html/overview.html
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     7206 2022-05-20 21:16:58.000000 slicer_package_manager-0.7.1/docs/_build/html/py-modindex.html
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4431 2022-05-20 21:16:58.000000 slicer_package_manager-0.7.1/docs/_build/html/search.html
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    17923 2022-05-20 21:16:58.000000 slicer_package_manager-0.7.1/docs/_build/html/searchindex.js
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       28 2022-04-18 17:25:05.000000 slicer_package_manager-0.7.1/docs/authors.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       28 2022-04-18 17:25:05.000000 slicer_package_manager-0.7.1/docs/changes.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    13624 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/docs/commands_shell.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4774 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/docs/concepts.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     5479 2022-05-20 21:35:19.000000 slicer_package_manager-0.7.1/docs/conf.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:36.244562 slicer_package_manager-0.7.1/docs/developer_guide/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     5751 2022-05-20 21:57:49.000000 slicer_package_manager-0.7.1/docs/developer_guide/develop.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      172 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/docs/developer_guide/index.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2051 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/docs/developer_guide/install.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      430 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/docs/developer_guide/overview.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      378 2022-05-20 21:16:55.000000 slicer_package_manager-0.7.1/docs/developer_guide/slicer_package_manager.api.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      618 2022-05-20 21:16:55.000000 slicer_package_manager-0.7.1/docs/developer_guide/slicer_package_manager.models.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      636 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/docs/developer_guide/slicer_package_manager.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      455 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/docs/developer_guide/slicer_package_manager_client.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     5137 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/docs/faq.rst
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:36.244562 slicer_package_manager-0.7.1/docs/images/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)  1515244 2022-04-18 17:25:05.000000 slicer_package_manager-0.7.1/docs/images/slicer_package_manager_models.JPG
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      969 2022-05-20 21:48:20.000000 slicer_package_manager-0.7.1/docs/index.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1664 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/docs/installation.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     5300 2022-05-20 21:48:20.000000 slicer_package_manager-0.7.1/docs/make_a_release.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3359 2022-05-20 21:48:20.000000 slicer_package_manager-0.7.1/docs/overview.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      238 2022-05-21 04:10:36.244562 slicer_package_manager-0.7.1/setup.cfg
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1410 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/setup.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:36.244562 slicer_package_manager-0.7.1/slicer_package_manager/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4303 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/slicer_package_manager/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      497 2022-05-21 04:10:36.244562 slicer_package_manager-0.7.1/slicer_package_manager/_version.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:36.244562 slicer_package_manager-0.7.1/slicer_package_manager/api/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/slicer_package_manager/api/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    44099 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/slicer_package_manager/api/app.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      302 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/slicer_package_manager/constants.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:36.244562 slicer_package_manager-0.7.1/slicer_package_manager/models/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/slicer_package_manager/models/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4854 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/slicer_package_manager/models/extension.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3548 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/slicer_package_manager/models/package.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     6785 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/slicer_package_manager/utilities.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:36.244562 slicer_package_manager-0.7.1/slicer_package_manager.egg-info/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1909 2022-05-21 04:10:35.000000 slicer_package_manager-0.7.1/slicer_package_manager.egg-info/PKG-INFO
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     5891 2022-05-21 04:10:36.000000 slicer_package_manager-0.7.1/slicer_package_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        1 2022-05-21 04:10:35.000000 slicer_package_manager-0.7.1/slicer_package_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       77 2022-05-21 04:10:36.000000 slicer_package_manager-0.7.1/slicer_package_manager.egg-info/entry_points.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        1 2022-05-20 22:01:54.000000 slicer_package_manager-0.7.1/slicer_package_manager.egg-info/not-zip-safe
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       16 2022-05-21 04:10:36.000000 slicer_package_manager-0.7.1/slicer_package_manager.egg-info/requires.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       29 2022-05-21 04:10:36.000000 slicer_package_manager-0.7.1/slicer_package_manager.egg-info/top_level.txt
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:36.244562 slicer_package_manager-0.7.1/tests/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    14029 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/tests/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      396 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/tests/conftest.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      183 2022-04-18 17:25:05.000000 slicer_package_manager-0.7.1/tests/test_load.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    41255 2022-05-20 20:46:19.000000 slicer_package_manager-0.7.1/tests/test_slicer_package_manager.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    68605 2022-05-20 21:48:20.000000 slicer_package_manager-0.7.1/versioneer.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:22.034357 slicer_package_manager-0.8.0/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      148 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/AUTHORS.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      600 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/LICENSE
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      226 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/MANIFEST.in
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1982 2023-05-11 02:54:22.034357 slicer_package_manager-0.8.0/PKG-INFO
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1109 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/README.rst
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:22.030357 slicer_package_manager-0.8.0/docs/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1130 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/Makefile
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       28 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/authors.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       28 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/changes.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    13624 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/commands_shell.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4774 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/concepts.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     5473 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/conf.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:22.030357 slicer_package_manager-0.8.0/docs/developer_guide/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     5732 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/developer_guide/develop.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      172 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/developer_guide/index.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2138 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/developer_guide/install.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      430 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/developer_guide/overview.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      378 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/developer_guide/slicer_package_manager.api.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      618 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/developer_guide/slicer_package_manager.models.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      636 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/developer_guide/slicer_package_manager.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      455 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/developer_guide/slicer_package_manager_client.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4756 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/faq.rst
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:22.030357 slicer_package_manager-0.8.0/docs/images/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)  1515244 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/images/slicer_package_manager_models.JPG
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      969 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/index.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1664 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/installation.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     5300 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/make_a_release.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3359 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/docs/overview.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2933 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/pyproject.toml
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      238 2023-05-11 02:54:22.034357 slicer_package_manager-0.8.0/setup.cfg
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1480 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:22.034357 slicer_package_manager-0.8.0/slicer_package_manager/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     7267 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/slicer_package_manager/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      497 2023-05-11 02:54:22.034357 slicer_package_manager-0.8.0/slicer_package_manager/_version.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:22.034357 slicer_package_manager-0.8.0/slicer_package_manager/api/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/slicer_package_manager/api/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    44559 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/slicer_package_manager/api/app.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      302 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/slicer_package_manager/constants.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:22.034357 slicer_package_manager-0.8.0/slicer_package_manager/models/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/slicer_package_manager/models/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4975 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/slicer_package_manager/models/extension.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3652 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/slicer_package_manager/models/package.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     7461 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/slicer_package_manager/utilities.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:22.034357 slicer_package_manager-0.8.0/slicer_package_manager.egg-info/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1982 2023-05-11 02:54:22.000000 slicer_package_manager-0.8.0/slicer_package_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1428 2023-05-11 02:54:22.000000 slicer_package_manager-0.8.0/slicer_package_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        1 2023-05-11 02:54:22.000000 slicer_package_manager-0.8.0/slicer_package_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       77 2023-05-11 02:54:22.000000 slicer_package_manager-0.8.0/slicer_package_manager.egg-info/entry_points.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        1 2023-05-11 02:54:21.000000 slicer_package_manager-0.8.0/slicer_package_manager.egg-info/not-zip-safe
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       49 2023-05-11 02:54:22.000000 slicer_package_manager-0.8.0/slicer_package_manager.egg-info/requires.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       29 2023-05-11 02:54:22.000000 slicer_package_manager-0.8.0/slicer_package_manager.egg-info/top_level.txt
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:22.034357 slicer_package_manager-0.8.0/tests/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    14270 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/tests/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      396 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/tests/conftest.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      259 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/tests/test_load.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    47108 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/tests/test_slicer_package_manager.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    68603 2023-05-11 02:51:26.000000 slicer_package_manager-0.8.0/versioneer.py
```

### Comparing `slicer_package_manager-0.7.1/LICENSE` & `slicer_package_manager-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slicer_package_manager-0.7.1/PKG-INFO` & `slicer_package_manager-0.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: slicer_package_manager
-Version: 0.7.1
+Version: 0.8.0
 Summary: Manage Slicer application and extension packages.
 Home-page: https://github.com/girder/slicer_package_manager
 Author: Jean-Christophe Fillion-Robin
 Author-email: slicer-packages-support@kitware.com
 License: Apache Software License 2.0
 Keywords: girder-plugin,slicer_package_manager
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ======================
 Slicer Package Manager
 ======================
```

### Comparing `slicer_package_manager-0.7.1/README.rst` & `slicer_package_manager-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `slicer_package_manager-0.7.1/docs/Makefile` & `slicer_package_manager-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `slicer_package_manager-0.7.1/docs/_build/html/_sources/commands_shell.rst.txt` & `slicer_package_manager-0.8.0/docs/commands_shell.rst`

 * *Files identical despite different names*

### Comparing `slicer_package_manager-0.7.1/docs/_build/html/_sources/concepts.rst.txt` & `slicer_package_manager-0.8.0/docs/concepts.rst`

 * *Files identical despite different names*

### Comparing `slicer_package_manager-0.7.1/docs/_build/html/_sources/developer_guide/develop.rst.txt` & `slicer_package_manager-0.8.0/docs/developer_guide/develop.rst`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Once Girder is started via ``girder-server``, the server will reload itself whenever a server
 source file is modified. If you are doing front-end development, it’s much faster to use a watch
 process to perform automatic fast rebuilds of your code whenever you make changes to source files.
 
 If you are front-end development of Slicer package manager plugin, use::
 
-    $ girder-install web --watch-plugin slicer_package_manager
+    $ girder build --watch-plugin slicer_package_manager
 
 
 Server side development
 -----------------------
 
 See the `Server Development documentation <https://girder.readthedocs.io/en/latest/development.html
 #server-development>`_ to know more about the good development practise in Girder
@@ -23,21 +23,20 @@
 See the `Client Development documentation <https://girder.readthedocs.io/en/latest/development.html
 #client-development>`_ to know more about the good development practise in Girder
 
 
 Python client development
 -------------------------
 
-The development of the **Slicer Package Manager Client** is in Python, it must work on both 2.7
-and 3.5 version of python, and follow flake8_ (the wrapper which verifies ``pep8``, ``pyflakes``
-and ``circular complexity``).
+The development of the **Slicer Package Manager Client** is in Python, and it uses ruff_  for code
+style validation.
 
 The python client use click_, a command line library for Python.
 
-.. _flake8: https://pypi.python.org/pypi/flake8
+.. _ruff: https://beta.ruff.rs/docs/
 .. _click: https://click.pocoo.org
 
 
 Testing
 -------
 
 Tests are the base of software development, they meant to check if what you've expected is really
@@ -96,17 +95,15 @@
 
 In the `CircleCI configuration file
 <https://github.com/girder/slicer_package_manager/blob/main/.circleci/config.yml>`_,
 there are several test going on:
 
 * :ref:`server_side_testing`
 
-    It will occurs each time a commit will be pushed on the repository (Source code at
-    `s_e_m_test.py <https://github.com/girder/slicer_package_manager/blob/main/plugin_tests/
-    s_e_m_test.py>`_).
+    It will occurs each time a commit will be pushed on the repository.
 
 * :ref:`python_client_testing`
 
     Both the python client API and the CLI are tested
 
 * Docker containers testing
```

### Comparing `slicer_package_manager-0.7.1/docs/_build/html/_sources/developer_guide/install.rst.txt` & `slicer_package_manager-0.8.0/docs/developer_guide/install.rst`

 * *Files 20% similar despite different names*

```diff
@@ -31,31 +31,37 @@
 
 Install from Git
 ----------------
 
 To easily develop the Slicer Package Manager, you will need to use some of Girder commands.
 So let's start by installing Girder::
 
-    $ git clone --branch 2.x-maintenance https://github.com/girder/girder.git
+    $ git clone https://github.com/girder/girder.git
     $ cd girder
+    $ pip install -e .
 
-To run the server, you must install some external Python package dependencies::
 
-    $ pip install -e .
+Then, let's install the Slicer Package Manager server plugin::
+
+    $ git clone https://github.com/girder/slicer_package_manager
+    $ cd slicer_package_manager
+    $ pip install -e .[test]
+
 
 This will provide you all the package needed to run the development environment. Then install
 the front-end web client development dependencies::
 
-    $ girder-install web --dev
+    $ girder build --dev
+
 
 Run
 ---
 
 To run the server, first make sure the Mongo daemon is running. To manually start it, run::
 
     $ mongod &
 
 Then to run Girder itself, just use the following command::
 
-    $ girder-server
+    $ girder-server --dev
 
 The application should be accessible on http://localhost:8080/ in your web browser.
```

### Comparing `slicer_package_manager-0.7.1/docs/_build/html/_sources/developer_guide/slicer_package_manager.models.rst.txt` & `slicer_package_manager-0.8.0/docs/developer_guide/slicer_package_manager.models.rst`

 * *Files identical despite different names*

### Comparing `slicer_package_manager-0.7.1/docs/_build/html/_sources/developer_guide/slicer_package_manager.rst.txt` & `slicer_package_manager-0.8.0/docs/developer_guide/slicer_package_manager.rst`

 * *Files identical despite different names*

### Comparing `slicer_package_manager-0.7.1/docs/_build/html/_sources/faq.rst.txt` & `slicer_package_manager-0.8.0/docs/faq.rst`

 * *Files 10% similar despite different names*

```diff
@@ -96,29 +96,19 @@
 *   Once you created the new release folder, enter inside it, then use the ``Copy picked resources here``
 
 *   You will just need to delete the draft sub-folder used to make the new stable release
 
 How to clean up the Draft release folder?
 -----------------------------------------
 
-Every day more than 300 extensions are supposed to be uploaded into the Slicer Package Manager. It's important to be
-able to clean up the old packages occasionally. Here's the process to do it:
+Since a large number of draft packages may be uploaded on a regular basis. Older draft packages may be removed
+applying this process:
 
-The command: ``slicer_package_manager_client draft list <APP_NAME> --offset <N>`` allows to list the oldest draft subfolders
+The command ``slicer_package_manager_client draft list <APP_NAME> --offset <N>`` allows to list the oldest draft subfolders
 related to old application revision. Using this command, you will be able to get a list of ``revision`` and then use the
 command ``slicer_package_manager_client draft delete <APP_NAME> <REVISION>`` in a loop to delete them all.
 
-There is also a bash script you can use easily to do that for you. In the directory
-``slicer_package_manager/python_client``, you will find the ``cleanNightly.sh`` script.
+.. note::
 
-To be able to run this script make sure to have the ``slicer_package_manager_client`` installed on your machine, if not
-check the :doc:`commands_shell` documentation.
+    The draft packages associated with the https://slicer-packages.kitware.com instance are automatically cleared
+    using the `clean-nightly-slicer-package-manager.sh <https://github.com/Slicer/DashboardScripts/blob/main/maintenance/metroplex/clean-nightly-slicer-package-manager.sh>`_  script.
 
-Then just enter::
-
-    $ ./cleanNightly.sh <API_URL> <API_KEY> <N>
-
-* API_URL: The URL of the distant machine, for instance http://192.168.xxx.xxx/api/v1
-
-* API_KEY: The token that allow you to use the client
-
-* N: Number of draft release you want to keep, all the oldest will be deleted
```

### Comparing `slicer_package_manager-0.7.1/docs/_build/html/_sources/index.rst.txt` & `slicer_package_manager-0.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `slicer_package_manager-0.7.1/docs/_build/html/_sources/installation.rst.txt` & `slicer_package_manager-0.8.0/docs/installation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 the server running the following commands::
 
     $ cd slicer_package_manager
     $ docker-compose up -d
 
 .. note::
 
-    The ``-d`` option is running the container in deamon mode. Remove it to display the logs
+    The ``-d`` option is running the container in daemon mode. Remove it to display the logs
     on the running containers.
 
     To rebuild the container after changing the source code use the ``--build`` option when
     you run the command.
 
 .. warning::
```

### Comparing `slicer_package_manager-0.7.1/docs/_build/html/_sources/make_a_release.rst.txt` & `slicer_package_manager-0.8.0/docs/make_a_release.rst`

 * *Files identical despite different names*

### Comparing `slicer_package_manager-0.7.1/docs/_build/html/_sources/overview.rst.txt` & `slicer_package_manager-0.8.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `slicer_package_manager-0.7.1/docs/conf.py` & `slicer_package_manager-0.8.0/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.doctest',
     'sphinx.ext.todo',
     'sphinx.ext.coverage',
-    'sphinx_issues'
+    'sphinx_issues',
 ]
 
 issues_github_path = 'girder/slicer_package_manager'
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
@@ -48,26 +48,26 @@
 # source_suffix = ['.rst', '.md']
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = u'Slicer Package Manager'
-copyright = u'2018, Kitware, Inc'
-author = u'Pierre Assemat'
+project = 'Slicer Package Manager'
+copyright = '2018, Kitware, Inc'
+author = 'Pierre Assemat'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = u'0.1.0'
+version = '0.1.0'
 # The full version, including alpha/beta/rc tags.
-release = u'0.1.0'
+release = '0.1.0'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
@@ -107,15 +107,15 @@
 #
 # This is required for the alabaster theme
 # refs: https://alabaster.readthedocs.io/en/latest/installation.html#sidebars
 html_sidebars = {
     '**': [
         'relations.html',  # needs 'show_related': True theme option to display
         'searchbox.html',
-    ]
+    ],
 }
 
 
 # -- Options for HTMLHelp output ------------------------------------------
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = 'SlicerPackageManagerdoc'
@@ -141,35 +141,35 @@
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'SlicerPackageManager.tex', u'Slicer Package Manager Documentation',
-     u'Pierre Assemat', 'manual'),
+    (master_doc, 'SlicerPackageManager.tex', 'Slicer Package Manager Documentation',
+     'Pierre Assemat', 'manual'),
 ]
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    (master_doc, 'slicerpackagemanager', u'Slicer Package Manager Documentation',
-     [author], 1)
+    (master_doc, 'slicerpackagemanager', 'Slicer Package Manager Documentation',
+     [author], 1),
 ]
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (master_doc, 'SlicerPackageManager',
-     u'Slicer Package Manager Documentation',
+     'Slicer Package Manager Documentation',
      author,
      'SlicerPackageManager',
      'One line description of project.',
      'Miscellaneous'),
 ]
```

### Comparing `slicer_package_manager-0.7.1/docs/images/slicer_package_manager_models.JPG` & `slicer_package_manager-0.8.0/docs/images/slicer_package_manager_models.JPG`

 * *Files identical despite different names*

### Comparing `slicer_package_manager-0.7.1/setup.py` & `slicer_package_manager-0.8.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-# -*- coding: utf-8 -*-
-
 import versioneer
 
 from setuptools import setup, find_packages
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 requirements = [
-    'girder>=3.0.0a1'
+    'girder>=3.0.0a1',
+    'girder-hashsum-download>=3.0.0a1',
 ]
 
 setup(
     author='Jean-Christophe Fillion-Robin',
     author_email='slicer-packages-support@kitware.com',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9'
+        'Programming Language :: Python :: 3.9',
     ],
     description='Manage Slicer application and extension packages.',
     install_requires=requirements,
     license='Apache Software License 2.0',
     long_description=readme,
     long_description_content_type='text/x-rst',
     include_package_data=True,
     keywords='girder-plugin, slicer_package_manager',
     name='slicer_package_manager',
     packages=find_packages(exclude=['test', 'test.*']),
-    python_require='>=3.7',
+    python_requires='>=3.6',
     url='https://github.com/girder/slicer_package_manager',
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     zip_safe=False,
     entry_points={
         'girder.plugin': [
-            'slicer_package_manager = slicer_package_manager:GirderPlugin'
-        ]
-    }
+            'slicer_package_manager = slicer_package_manager:GirderPlugin',
+        ],
+    },
 )
```

### Comparing `slicer_package_manager-0.7.1/slicer_package_manager/api/app.py` & `slicer_package_manager-0.8.0/slicer_package_manager/api/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from ..models.package import Package as PackageModel
 from .. import constants
 from .. import utilities
 
 
 class App(Resource):
     def __init__(self):
-        super(App, self).__init__()
+        super().__init__()
         self.resourceName = 'app'
         self._model = Folder()
 
         self.route('POST', (), self.initApp)
         self.route('GET', (), self.listApp)
         self.route('DELETE', (':app_id',), self.deleteApp)
         self.route('GET', (':app_id', 'downloadstats'), self.getDownloadStats)
@@ -57,15 +57,15 @@
         .param('collection_id', 'The ID of the collection which contain the application',
                required=False)
         .param('collection_name', 'The Name of the collection which be created to contain'
                ' the application', required=False)
         .param('collection_description', 'Collection description.', required=False)
         .param('public', 'Whether the collection should be publicly visible.',
                required=False, dataType='boolean', default=True)
-        .errorResponse('Write permission denied on the application.', 403)
+        .errorResponse('Write permission denied on the application.', 403),
     )
     @access.user(scope=TokenScope.DATA_WRITE)
     def initApp(self, name, app_description, collection_id, collection_name,
                 collection_description, public):
         """
         Create the directory for start a new application. By default, without specifying
         a ``collection_id``, it will create a new collection name either ``collection_name``
@@ -144,28 +144,28 @@
             creator=creator)
         # Set a default template name for extensions in the application,
         # this can be changed in anytime.
         return self._model.setMetadata(
             app,
             {
                 'applicationPackageNameTemplate': constants.APPLICATION_PACKAGE_TEMPLATE_NAME,
-                'extensionPackageNameTemplate': constants.EXTENSION_PACKAGE_TEMPLATE_NAME
-            }
+                'extensionPackageNameTemplate': constants.EXTENSION_PACKAGE_TEMPLATE_NAME,
+            },
         )
 
     @autoDescribeRoute(
         Description('List existing application.')
         .responseClass('Folder', array=True)
         .param('app_id', 'The ID of the application.', required=False)
         .param('collection_id', 'The ID of the collection.', required=False)
         .param('name', 'The name of the application.', required=False)
         .param('text', 'Provide text search of the application.', required=False)
         .pagingParams(defaultSort='name')
         .errorResponse()
-        .errorResponse('Read permission denied on the application.', 403)
+        .errorResponse('Read permission denied on the application.', 403),
     )
     @access.public(scope=TokenScope.DATA_READ)
     def listApp(self, app_id, collection_id, name, text, limit, offset, sort):
         """
         List existing applications base on some optional parameters.
         For searching application which aren't in the default collection (Applications),
         the parameter ``collection_id`` need to be provided.
@@ -194,15 +194,15 @@
                 if top_folder_name:
                     top_folder_name = top_folder_name[0]
                 else:
                     return []
                 filters = {}
                 if text:
                     filters['$text'] = {
-                        '$search': text
+                        '$search': text,
                     }
                 if name:
                     filters['name'] = name
 
                 return list(self._model.childFolders(
                     parentType='Folder', parent=top_folder_name, user=user,
                     offset=offset, limit=limit, sort=sort, filters=filters))
@@ -211,36 +211,37 @@
     @access.user(scope=TokenScope.DATA_WRITE)
     @autoDescribeRoute(
         Description('Delete an Application by ID.')
         .modelParam('app_id', destName='app_folder', model=Folder, level=AccessType.ADMIN)
         .param('progress', 'Whether to record progress on this task.',
                required=False, dataType='boolean', default=False)
         .errorResponse('ID was invalid.')
-        .errorResponse('Admin access was denied for the application.', 403)
+        .errorResponse('Admin access was denied for the application.', 403),
     )
     def deleteApp(self, app_folder, progress):
         """
         Delete an application by ID.
 
         :param app_folder: Application folder loaded using ``app_id`` route parameter.
         :return: Confirmation message with the deleted application name
         """
-        return utilities.deleteFolder(app_folder, progress, self.getCurrentUser())
+        utilities.deleteFolder(app_folder, progress, self.getCurrentUser())
+        return {'message': 'Deleted application %s.' % app_folder['name']}
 
     @autoDescribeRoute(
         Description('Create a new release.')
         .responseClass('Folder')
         .notes("The application's revision is stored as metadata of the new release.")
         .param('name', "The release's name.")
         .param('app_id', "The application's ID which contain the release", paramType='path')
         .param('app_revision', "The application's revision which correspond to the release")
         .param('description', "The application's description.", required=False)
         .param('public', 'Whether the release should be publicly visible.',
                required=False, dataType='boolean', default=True)
-        .errorResponse()
+        .errorResponse(),
     )
     @access.user(scope=TokenScope.DATA_WRITE)
     def createNewRelease(self, name, app_id, app_revision, description, public):
         """
         Create a new release with the ``name`` within the application. The ``app_revision``
         will be used to automatically choose this release when uploading an application or
         extension package with a matching application revision metadata.
@@ -270,15 +271,15 @@
     @autoDescribeRoute(
         Description('Get all the releases from an application.')
         .responseClass('Folder')
         .param('app_id', "The application's ID.", paramType='path')
         .param('release_id_or_name', "The release's ID or name.", required=False)
         .pagingParams(defaultSort='created', defaultSortDir=SortDir.DESCENDING)
         .errorResponse('ID was invalid.')
-        .errorResponse('Read permission denied on the application.', 403)
+        .errorResponse('Read permission denied on the application.', 403),
     )
     @access.public(scope=TokenScope.DATA_READ)
     def getReleases(self, app_id, release_id_or_name, limit, offset, sort):
         """
         Get a list of all the stable release of an application. You can also search
         for a specific release if you provide the ``release_id_or_name`` parameter.
         If the ``release_id_or_name`` parameter doesn't correspond to any existing
@@ -300,15 +301,15 @@
                 user=user,
                 filters={'lowerName': release_id_or_name.lower()}))
             if not release_folder:
                 return None
             else:
                 return release_folder[0]
         filters = {
-            'name': {'$ne': constants.DRAFT_RELEASE_NAME}
+            'name': {'$ne': constants.DRAFT_RELEASE_NAME},
         }
         return list(self._model.childFolders(
             application,
             'Folder',
             user=user,
             limit=limit,
             offset=offset,
@@ -318,15 +319,15 @@
     @autoDescribeRoute(
         Description('Get all the draft releases from an application.')
         .responseClass('Folder')
         .param('app_id', "The application's ID.", paramType='path')
         .param('revision', 'The revision of a draft release', required=False)
         .pagingParams(defaultSort='created', defaultSortDir=SortDir.DESCENDING)
         .errorResponse('ID was invalid.')
-        .errorResponse('Read permission denied on the application.', 403)
+        .errorResponse('Read permission denied on the application.', 403),
     )
     @access.public(scope=TokenScope.DATA_READ)
     def getAllDraftReleases(self, app_id, revision, limit, offset, sort):
         """
         Get a list of all the draft release of an application. It's also
         possible to filter this list by the metadata ``revision``.
 
@@ -334,24 +335,24 @@
         :param revision: Revision of one of the draft release
         :return: List of all release within the application
         """
         user = self.getCurrentUser()
         application = self._model.load(app_id, user=user, level=AccessType.READ)
 
         filters = {
-            'name': constants.DRAFT_RELEASE_NAME
+            'name': constants.DRAFT_RELEASE_NAME,
         }
         release = list(self._model.childFolders(
             application,
             'Folder',
             user=user,
             filters=filters))
         if not release:
-            raise RestException('There is no %s release in this application.'
-                                % constants.DRAFT_RELEASE_NAME)
+            msg = f"There is no {constants.DRAFT_RELEASE_NAME} release in this application."
+            raise RestException(msg)
         release = release[0]
         draft_filters = {'meta.revision': {'$exists': True}}
         if revision:
             draft_filters = {'meta.revision': revision}
         return list(self._model.childFolders(
             release,
             'Folder',
@@ -365,15 +366,15 @@
     @autoDescribeRoute(
         Description('Delete a release by ID or name.')
         .modelParam('app_id', destName='app_folder', model=Folder, level=AccessType.ADMIN)
         .param('release_id_or_name', "The release's ID or name.", paramType='path')
         .param('progress', 'Whether to record progress on this task.',
                required=False, dataType='boolean', default=False)
         .errorResponse('ID was invalid.')
-        .errorResponse('Admin access was denied for the release.', 403)
+        .errorResponse('Admin access was denied for the release.', 403),
     )
     def deleteReleaseByIdOrName(self, app_folder, release_id_or_name, progress):
         """
         Delete a release by ID or name.
 
         :param app_folder: Application folder loaded using ``app_id`` route parameter.
         :param release_id_or_name: Could be either the release ID or the release name
@@ -393,30 +394,33 @@
             if not release_folder:
                 release_folder = list(self._model.childFolders(
                     app_folder,
                     'Folder',
                     user=user,
                     filters={'lowerName': constants.DRAFT_RELEASE_NAME.lower()}))
                 if not release_folder:
-                    raise RestException("Couldn't find release %s" % release_id_or_name)
+                    msg = f"Could not find the release '{release_id_or_name}'."
+                    raise RestException(msg)
                 revision_folder = list(self._model.childFolders(
                     release_folder[0],
                     'Folder',
                     user=user,
-                    filters={'lowerName': release_id_or_name.lower()}
+                    filters={'lowerName': release_id_or_name.lower()},
                 ))
                 if not revision_folder:
-                    raise RestException("Couldn't find release %s" % release_id_or_name)
+                    msg = f"Could not find the release '{release_id_or_name}'."
+                    raise RestException(msg)
                 release = revision_folder[0]
             else:
                 release = release_folder[0]
 
-        return utilities.deleteFolder(release, progress, self.getCurrentUser())
+        utilities.deleteFolder(release, progress, self.getCurrentUser())
+        return {'message': 'Deleted release %s.' % release['name']}
 
-    @autoDescribeRoute(  # noqa: C901
+    @autoDescribeRoute(
         Description('List or search available extensions.')
         .notes('If the "release_id" provided correspond to the "draft" release,'
                ' then you must provide the "app_revision" to use this parameters. '
                'If not, it will just be ignored.')
         .responseClass('Extension')
         .param('app_id', 'The ID of the application.', paramType='path')
         .param('extension_name', 'The name of the extension.', required=False)
@@ -426,15 +430,15 @@
                required=False, enum=['linux', 'win', 'macosx'])
         .param('arch', 'The os chip architecture.',
                required=False, enum=['i386', 'amd64'])
         .param('app_revision', 'The revision of the application.', required=False)
         .param('baseName', 'The baseName of the extension', required=False)
         .param('q', 'The search query.', required=False)
         .pagingParams(defaultSort='created', defaultSortDir=SortDir.DESCENDING)
-        .errorResponse()
+        .errorResponse(),
     )
     @access.public(scope=TokenScope.DATA_READ)
     def getExtensions(self, app_id, extension_name, release_id, extension_id, os, arch,
                       app_revision, baseName, q, limit, sort, offset=0):
         """
         Get a list of extension which is filtered by some optional parameters. If the ``release_id``
         provided correspond to the draft release, then you must provide the app_revision to use
@@ -454,15 +458,15 @@
         user = self.getCurrentUser()
         utilities.checkAccess(app_id, user)
         filters = {
             '$and': [
                 {'meta.app_id': {'$eq': app_id}},
                 {'meta.os': {'$exists': True}},
                 {'meta.arch': {'$exists': True}},
-                {'meta.app_revision': {'$exists': True}}]
+                {'meta.app_revision': {'$exists': True}}],
         }
         if extension_name:
             filters['lowerName'] = extension_name.lower()
         if ObjectId.is_valid(extension_id):
             filters['_id'] = ObjectId(extension_id)
         if os:
             filters['meta.os'] = os
@@ -473,15 +477,15 @@
         if baseName:
             # Provide a exact match base on baseName
             filters['meta.baseName'] = baseName
         if q:
             escaped_query = re.escape(q)
             filters['$or'] = [
                 {'meta.baseName': {'$regex': escaped_query, '$options': 'i'}},
-                {'meta.description': {'$regex': escaped_query, '$options': 'i'}}
+                {'meta.description': {'$regex': escaped_query, '$options': 'i'}},
             ]
         if ObjectId.is_valid(release_id):
             release = self._model.load(release_id, user=user, level=AccessType.READ)
             if release['name'] == constants.DRAFT_RELEASE_NAME:
                 if app_revision:
                     revisions = list(self._model.childFolders(
                         release,
@@ -537,15 +541,15 @@
                 filters['folderId'] = ObjectId(extensions_folder['_id'])
         return list(ExtensionModel().find(
             query=filters,
             limit=limit,
             offset=offset,
             sort=sort))
 
-    @autoDescribeRoute(  # noqa: 901
+    @autoDescribeRoute(
         Description('Create or Update an extension package.')
         .param('app_id', 'The ID of the App.', paramType='path')
         .param('os', 'The target operating system of the package.',
                enum=['linux', 'win', 'macosx'])
         .param('arch', 'The os chip architecture.', enum=['i386', 'amd64'])
         .param('baseName', 'The baseName of the package (ie installer baseName).')
         .param('repository_type', 'The type of the repository (svn, git).')
@@ -565,15 +569,15 @@
         .param('contributors', 'List of contributors of the extension.', required=False)
         .param('dependency', 'List of the required extensions to use this one.', required=False)
         .param('license', 'The license short description of the extension.', required=False)
         .param('development_status', 'Arbitrary description of the status of the extension '
                '(stable, active, etc).', required=False)
         .param('enabled', 'Boolean indicating if the extension should be automatically enabled '
                'after its installation.', required=False)
-        .errorResponse()
+        .errorResponse(),
     )
     @access.user(scope=TokenScope.DATA_WRITE)
     def createOrUpdateExtension(self, app_id, os, arch, baseName, repository_type, repository_url,
                                 revision, app_revision, description,
                                 icon_url, development_status, category, enabled, homepage,
                                 screenshots, contributors, dependency, license):
         """
@@ -625,15 +629,15 @@
             'baseName': baseName,
             'os': os,
             'arch': arch,
             'repository_type': repository_type,
             'repository_url': repository_url,
             'revision': revision,
             'app_revision': app_revision,
-            'description': description
+            'description': description,
         }
         if icon_url:
             params['icon_url'] = icon_url
         if development_status:
             params['development_status'] = development_status
         if category:
             params['category'] = category
@@ -651,55 +655,59 @@
             params['license'] = license
 
         name = application['meta']['extensionPackageNameTemplate'].format(**params)
         filters = {
             'meta.baseName': baseName,
             'meta.os': os,
             'meta.arch': arch,
-            'meta.app_revision': app_revision
+            'meta.app_revision': app_revision,
         }
         # Only one extensions should be in this list
         extensions = list(ExtensionModel().get(extensions_folder, filters=filters))
         if not len(extensions):
             # The extension doesn't exist yet:
             extension = ExtensionModel().createExtension(name, creator, extensions_folder, params)
         elif len(extensions) == 1:
             # The extension already exist
             extension = extensions[0]
             # Check the file inside the extension Item
             files = ExtensionModel().childFiles(extension)
             if not files.count():
                 # Extension empty
-                raise RestException("Extension existing without any binary file.")
+                msg = "Extension existing without any binary file."
+                raise RestException(msg)
 
             # Update the extension
             extension['name'] = name
             extension = ExtensionModel().setMetadata(extension, params)
         else:
-            raise RestException('Too many extensions found for the same name :"%s"' % name)
+            msg = f"Too many extensions found for the same name '{name}'."
+            raise RestException(msg)
 
         # Ready to upload the binary file
         return extension
 
     @autoDescribeRoute(
         Description('Delete an Extension by ID.')
         .param('app_id', 'The ID of the App.', paramType='path')
         .modelParam('ext_id', destName='ext_model', model=ExtensionModel, level=AccessType.WRITE)
         .errorResponse('ID was invalid.')
-        .errorResponse('Admin access was denied for the extension.', 403)
+        .errorResponse('Admin access was denied for the extension.', 403),
     )
     @access.user(scope=TokenScope.DATA_WRITE)
     def deleteExtension(self, app_id, ext_model):
         """
         Delete an extension by ID.
 
         :param app_id: Application ID
         :param ext_model: Extension model loaded using ``ext_id`` route parameter.
         :return: The deleted extension
         """
+        user = self.getCurrentUser()
+        utilities.checkAccess(app_id, user)
         ExtensionModel().remove(ext_model)
         return ext_model
 
     @autoDescribeRoute(
         Description('List or search available packages.')
         .notes('If the "release_id" provided correspond to the "draft" release,'
                ' then you must provide the "revision" to use this parameters. '
@@ -712,15 +720,15 @@
         .param('os', 'The target operating system of the package.',
                required=False, enum=['linux', 'win', 'macosx'])
         .param('arch', 'The os chip architecture.',
                required=False, enum=['i386', 'amd64'])
         .param('revision', 'The revision of the application.', required=False)
         .param('baseName', 'The baseName of the package', required=False)
         .pagingParams(defaultSort='created', defaultSortDir=SortDir.DESCENDING)
-        .errorResponse()
+        .errorResponse(),
     )
     @access.public(scope=TokenScope.DATA_READ)
     def getPackages(self, app_id, package_name, release_id_or_name, package_id, os, arch,
                     revision, baseName, limit, offset, sort):
         """
         Get a list of package which is filtered by some optional parameters. If the ``release_id``
         provided correspond to the draft release, then you must provide the revision to use
@@ -739,15 +747,15 @@
         user = self.getCurrentUser()
         filters = {
             '$and': [
                 {'meta.app_id': {'$eq': app_id}},
                 {'meta.os': {'$exists': True}},
                 {'meta.arch': {'$exists': True}},
                 {'meta.revision': {'$exists': True}},
-                {'meta.app_revision': {'$exists': False}}]
+                {'meta.app_revision': {'$exists': False}}],
         }
         if package_name:
             filters['lowerName'] = package_name.lower()
         if ObjectId.is_valid(package_id):
             filters['_id'] = ObjectId(package_id)
         if os:
             filters['meta.os'] = os
@@ -820,15 +828,15 @@
         .param('revision', 'The revision of the application')
         .param('version', 'The version of the application')
         .param('description', 'Text describing the package.', required=False)
         .param('pre_release', 'Boolean to specify if the package is a full release ready to be distributed.',
                dataType='boolean', required=False)
         .param('build_date', 'Build timestamp specified as a datetime string. Default set to current date and time.',
                required=False)
-        .errorResponse()
+        .errorResponse(),
     )
     @access.user(scope=TokenScope.DATA_WRITE)
     def createOrUpdatePackage(self, app_id, os, arch, baseName, repository_type, repository_url,
                               revision, version, description, pre_release, build_date):
         """
         Create or update a package item.
 
@@ -861,83 +869,88 @@
 
         if not build_date:
             build_date = datetime.datetime.utcnow()
         else:
             try:
                 build_date = parseTimestamp(build_date)
             except ValueError:
-                raise RestException('Parameter "build_date" is incorrectly formatted.')
+                msg = "Parameter 'build_date' is incorrectly formatted."
+                raise RestException(msg)
 
         params = {
             'app_id': app_id,
             'baseName': baseName,
             'os': os,
             'arch': arch,
             'repository_type': repository_type,
             'repository_url': repository_url,
             'revision': revision,
             'version': version,
             'pre_release': pre_release,
-            'build_date': build_date
+            'build_date': build_date,
         }
 
         name = application['meta']['applicationPackageNameTemplate'].format(**params)
         filters = {
             'meta.baseName': baseName,
             'meta.os': os,
             'meta.arch': arch,
-            'meta.revision': revision
+            'meta.revision': revision,
         }
         # Only one package should be in this list
         package = list(PackageModel().get(release_folder, filters=filters))
         if not len(package):
             # The package doesn't exist yet:
             package = PackageModel().createPackage(name, creator, release_folder, params,
                                                    description)
         elif len(package) == 1:
             # The package already exist
             package = package[0]
             # Check the file inside the application package
             files = PackageModel().childFiles(package)
             if not files.count():
                 # Package empty
-                raise RestException("Application Package existing without any binary file.")
+                msg = "Application Package existing without any binary file."
+                raise RestException(msg)
             # Update the package
             package['name'] = name
             package = PackageModel().setMetadata(package, params)
         else:
-            raise RestException('Too many packages found for the same name :"%s"' % name)
+            msg = f"Too many packages found for the same name '{name}'."
+            raise RestException(msg)
 
         # Ready to upload the binary file
         return package
 
     @autoDescribeRoute(
         Description('Delete a Package by ID.')
         .param('app_id', 'The ID of the App.', paramType='path')
         .modelParam('pkg_id', destName='pkg_model', model=PackageModel, level=AccessType.WRITE)
         .errorResponse('ID was invalid.')
-        .errorResponse('Admin access was denied for the package.', 403)
+        .errorResponse('Admin access was denied for the package.', 403),
     )
     @access.user(scope=TokenScope.DATA_WRITE)
     def deletePackage(self, app_id, pkg_model):
         """
         Delete an application package by ID.
 
         :param app_id: Application ID
         :param pkg_model: Package model loaded using ``pkg_id`` route parameter.
         :return: The deleted package
         """
+        user = self.getCurrentUser()
+        utilities.checkAccess(app_id, user)
         PackageModel().remove(pkg_model)
         return pkg_model
 
     @autoDescribeRoute(
         Description('Get download stats of application and extensions packages '
                     'within an application.')
         .param('app_id', 'The ID of the application.', paramType='path')
-        .errorResponse()
+        .errorResponse(),
     )
     @access.public(scope=TokenScope.DATA_READ)
     def getDownloadStats(self, app_id):
         """
         Get all the download count of all the application and extension packages
         from an application.
```

### Comparing `slicer_package_manager-0.7.1/slicer_package_manager/models/extension.py` & `slicer_package_manager-0.8.0/slicer_package_manager/models/extension.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import datetime
-import six
 
 from girder.models.folder import Folder
 from girder.models.item import Item
 from girder.models.model_base import ValidationException
 
 
 class Extension(Item):
     """
-    The ``Extension`` class derive from the ``Item`` model in Girder and it uses to embedded
+    The ``Extension`` class derives from the ``Item`` model in Girder and it embeds
     extension binary files.
     """
 
     def initialize(self):
-        super(Extension, self).initialize()
+        super().initialize()
         # To be able to upload within an Extension the name has to stay as 'item'.
         self.name = 'item'
 
     def get(self, release, limit=0, offset=0, sort=None, filters=None, **kwargs):
         """
         Get all the extensions available for a release.
 
@@ -42,81 +41,98 @@
         :param params: All the metadata to set on the new extension
         :return: The new extension item
         """
         item = self.createItem(
             name,
             creator,
             folder,
-            params.get('description')
+            params.get('description'),
         )
         return self.setMetadata(item, params)
 
     def validate(self, doc):
         """
         Validate the extension instance.
 
         :param doc: The extension instance
         :return: The extension instance once validated
         """
         # Call Item validate method
-        doc = super(Extension, self).validate(doc)
+        doc = super().validate(doc)
 
         if not isinstance(doc.get('created'), datetime.datetime):
-            raise ValidationException(
-                'Extension field "created" must be a datetime.')
+            msg = 'Extension field "created" must be a datetime.'
+            raise ValidationException(msg)
 
         # Validate the meta field
         if doc.get('meta'):
-            base_params = {'app_id', 'os', 'arch', 'revision', 'repository_type', 'repository_url',
-                           'app_revision', 'baseName', 'description'}
+            base_params = {
+                'app_id',
+                'os',
+                'arch',
+                'revision',
+                'repository_type',
+                'repository_url',
+                'app_revision',
+                'baseName',
+                'description',
+                'sha512',
+            }
             specs = []
             for meta in base_params:
                 specs.append({
                     'name': meta,
-                    'type': six.string_types,
-                    'exception_msg': 'Extension field "{}" must be a non-empty string.'
-                                     .format(meta)
+                    'type': (str,),
+                    'exception_msg': f'Extension field "{meta}" must be a non-empty string.',
                 })
             for spec in specs:
                 if doc['meta'].get(spec['name']) and not isinstance(
                    doc['meta'][spec['name']], spec['type']):
-                    raise ValidationException(spec['exception_msg'])
-            extraMeta = set(six.viewkeys(doc['meta'])) - base_params
+                    msg=spec['exception_msg']
+                    raise ValidationException(msg)
+            extraMeta = set(doc['meta'].keys()) - base_params
             if extraMeta:
-                extra_params = {'icon_url', 'development_status', 'category',
-                                'enabled', 'homepage', 'screenshots', 'contributors', 'dependency',
-                                'license'}
+                extra_params = {
+                    'icon_url',
+                    'development_status',
+                    'category',
+                    'enabled',
+                    'homepage',
+                    'screenshots',
+                    'contributors',
+                    'dependency',
+                    'license',
+                }
                 if extraMeta - extra_params:
-                    raise ValidationException('Extension has extra fields: %s.' %
-                                              ', '.join(sorted(extraMeta)))
+                    msg = f'Extension has extra fields: {", ".join(sorted(extraMeta))}.'
+                    raise ValidationException(msg)
                 specs = []
                 for meta in extra_params:
                     if meta == 'enabled':
                         specs.append({
                             'name': meta,
                             'type': bool,
-                            'exception_msg': 'Extension field "{}" must be a boolean.'
-                                             .format(meta)
+                            'exception_msg': f'Extension field "{meta}" must be a boolean.',
                         })
                     else:
                         specs.append({
                             'name': meta,
-                            'type': six.string_types,
-                            'exception_msg': 'Extension field "{}" must be a non-empty string.'
-                                             .format(meta)
+                            'type': (str,),
+                            'exception_msg': f'Extension field "{meta}" must be a non-empty string.',
                         })
                 for spec in specs:
                     if doc['meta'].get(spec['name']) and not isinstance(
                        doc['meta'][spec['name']], spec['type']):
-                        raise ValidationException(spec['exception_msg'])
+                        msg = spec['exception_msg']
+                        raise ValidationException(msg)
             duplicateQuery = {
                 'name': doc['name'],
                 'os': doc['meta']['os'],
                 'arch': doc['meta']['arch'],
-                'app_revision': doc['meta']['app_revision']
+                'app_revision': doc['meta']['app_revision'],
             }
             if '_id' in doc:
                 duplicateQuery['_id'] = {'$ne': doc['_id']}
             if self.findOne(duplicateQuery, fields=['_id']):
-                raise ValidationException(
-                    'An Extension with this name and characteristics already exists.')
+                msg = 'An Extension with this name and characteristics already exists.'
+                raise ValidationException(msg)
         return doc
```

### Comparing `slicer_package_manager-0.7.1/slicer_package_manager/models/package.py` & `slicer_package_manager-0.8.0/slicer_package_manager/models/package.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import datetime
-import six
 
 from girder.models.folder import Folder
 from girder.models.item import Item
 from girder.models.model_base import ValidationException
 
 
 class Package(Item):
     """
-    The ``Package`` class derive from the ``Item`` model in Girder and it uses to embedded
-    packages binary files.
+    The ``Package`` class derives from the ``Item`` model in Girder and it embeds
+    package binary files.
     """
 
     def initialize(self):
-        super(Package, self).initialize()
+        super().initialize()
         # To be able to upload within a Package the name has to stay as 'item'.
         self.name = 'item'
 
     def get(self, release, limit=0, offset=0, sort=None, filters=None, **kwargs):
         """
         Get all the application packages available for a release.
 
@@ -43,57 +42,66 @@
         :param description: A description for the application package.
         :return: The new application package item
         """
         item = self.createItem(
             name,
             creator,
             folder,
-            description
+            description,
         )
         return self.setMetadata(item, params)
 
     def validate(self, doc):
         """
         Validate the package instance.
 
         :param doc: The package instance
         :return: The package instance once validated
         """
         # Call Item validate method
-        doc = super(Package, self).validate(doc)
+        doc = super().validate(doc)
 
         if not isinstance(doc.get('created'), datetime.datetime):
-            raise ValidationException(
-                'Package field "created" must be a datetime.')
+            msg = 'Package field "created" must be a datetime.'
+            raise ValidationException(msg)
 
         # Validate the meta field
         if doc.get('meta'):
-            base_params = {'app_id', 'os', 'arch', 'repository_type', 'repository_url',
-                           'revision', 'baseName'}
+            base_params = {
+                'app_id',
+                'os',
+                'arch',
+                'repository_type',
+                'repository_url',
+                'revision',
+                'baseName',
+                'sha512',
+            }
             specs = []
             for meta in base_params:
                 specs.append({
                     'name': meta,
-                    'type': six.string_types,
-                    'exception_msg': 'Package field "%s" must be a non-empty string.' % meta
+                    'type': (str,),
+                    'exception_msg': f'Package field "{meta}" must be a non-empty string.',
                 })
             specs.append({
                 'name': 'build_date ',
                 'type': datetime.datetime,
-                'exception_msg': 'Package field "%s" must be a datetime.' % 'build_date'
+                'exception_msg': 'Package field "build_date" must be a datetime.',
             })
             for spec in specs:
                 if doc['meta'].get(spec['name']) and not isinstance(
                    doc['meta'][spec['name']], spec['type']):
-                    raise ValidationException(spec['exception_msg'])
+                    msg = spec['exception_msg']
+                    raise ValidationException(msg)
             duplicateQuery = {
                 'name': doc['name'],
                 'os': doc['meta']['os'],
                 'arch': doc['meta']['arch'],
-                'revision': doc['meta']['revision']
+                'revision': doc['meta']['revision'],
             }
             if '_id' in doc:
                 duplicateQuery['_id'] = {'$ne': doc['_id']}
             if self.findOne(duplicateQuery, fields=['_id']):
-                raise ValidationException(
-                    'A Package with this name and characteristics already exists.')
+                msg = 'A Package with this name and characteristics already exists.'
+                raise ValidationException(msg)
         return doc
```

### Comparing `slicer_package_manager-0.7.1/slicer_package_manager/utilities.py` & `slicer_package_manager-0.8.0/slicer_package_manager/utilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 from girder.constants import AccessType
 from girder.models.folder import Folder
+from girder.models.item import Item
 from girder.utility.progress import ProgressContext
 
 from . import constants
 
 
 def isSlicerPackages(item):
+    """Return True if the item represents either an application or an extension package."""
     if 'meta' in item and all(k in item['meta'] for k in ('os', 'arch', 'baseName', 'revision')):
         return True
     return False
 
 
+def isChildOfSlicerPackages(file_item):
+    """
+    Return True if the file is included in an item corresponding to either an application or
+    an extension package.
+    """
+    parent_item = Item().load(file_item['itemId'], force=True)
+    return isSlicerPackages(parent_item)
+
+
 def isApplicationFolder(folder):
     """
     Return True if folder an application folder.
 
     An application folder is expected to have the ``applicationPackageNameTemplate`` and
     ``extensionPackageNameTemplate`` metadata as well as parent folder named after
     :const:`constants.TOP_LEVEL_FOLDER_NAME`.
@@ -70,19 +81,18 @@
     :param app_revision: The revision of the application.
     :return: The created/existing release folder.
     """
     release_folder = None
     # Find the release by metadata revision
     releases = Folder().childFolders(application, 'Folder', user=user)
     for folder in releases:
-        if 'meta' in folder:
-            if 'revision' in folder['meta']:
-                if folder['meta']['revision'] == app_revision:
-                    release_folder = folder
-                    break
+        revision = folder.get('meta', {}).get('revision', '')
+        if revision == app_revision:
+            release_folder = folder
+            break
     if not release_folder:
         # Only the draft release in the list
         release_folder = list(Folder().childFolders(
             application,
             'Folder',
             user=user,
             filters={'name': constants.DRAFT_RELEASE_NAME}))
@@ -162,22 +172,31 @@
     if grantparent_folder['name'] == constants.DRAFT_RELEASE_NAME:
         return grantparent_folder
     else:
         return package_folder
 
 
 def deleteFolder(folder, progress, user):
+    """Recursively delete a folder by ID.
+
+    :param folder: The folder document to delete.
+    :type folder: dict
+    :param progress: A progress context to record progress on.
+    :type progress: girder.utility.progress.ProgressContext or None.
+    :param user: The user creating the progress.
+    :type user: dict
+    :return:
+    """
     with ProgressContext(progress, user=user,
                          title='Deleting folder %s' % folder['name'],
                          message='Calculating folder size...') as ctx:
         # Don't do the subtree count if we weren't asked for progress
         if progress:
             ctx.update(total=Folder().subtreeCount(folder))
         Folder().remove(folder, progress=ctx)
-    return folder
 
 
 def checkAccess(app_id, user):
     """
     Check user has access to the application.
 
     :param app_id: The ID of the application.
```

### Comparing `slicer_package_manager-0.7.1/slicer_package_manager.egg-info/PKG-INFO` & `slicer_package_manager-0.8.0/slicer_package_manager.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: slicer-package-manager
-Version: 0.7.1
+Version: 0.8.0
 Summary: Manage Slicer application and extension packages.
 Home-page: https://github.com/girder/slicer_package_manager
 Author: Jean-Christophe Fillion-Robin
 Author-email: slicer-packages-support@kitware.com
 License: Apache Software License 2.0
 Keywords: girder-plugin,slicer_package_manager
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ======================
 Slicer Package Manager
 ======================
```

### Comparing `slicer_package_manager-0.7.1/tests/__init__.py` & `slicer_package_manager-0.8.0/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 from shutil import copyfile
 
 from slicer_package_manager.constants import (
     APPLICATION_PACKAGE_TEMPLATE_NAME,
-    EXTENSION_PACKAGE_TEMPLATE_NAME
+    EXTENSION_PACKAGE_TEMPLATE_NAME,
 )
 
 
 FIXTURE_DIR = os.path.join(
     os.path.dirname(os.path.realpath(__file__)),
     'data',
     )
@@ -23,91 +23,91 @@
         'version': '0.1.0',
     },
 ]
 
 DRAFT_RELEASES = [
     {
         'revision': '0000',
-        'version': '0.2.0'
+        'version': '0.2.0',
     },
     {
         'revision': '0001',
-        'version': '0.3.0'
+        'version': '0.3.0',
     },
 ]
 
 RELEASE_EXTENSIONS = [
     {
         'filepath': 'extension0.tar.gz',
         'meta': {
             'os': 'linux',
             'arch': 'i386',
             'baseName': 'Ext0',
             'repository_type': 'git',
             'repository_url': 'http://slicer.com/extension/Ext',
             'revision': '35333',
             'app_revision': RELEASES[0]['revision'],
-            'description': 'Extension for Slicer 4'
-        }
-    }
+            'description': 'Extension for Slicer 4',
+        },
+    },
 ]
 
 DRAFT_EXTENSIONS = [
     {
         'filepath': 'extension1.tar.gz',
         'meta': {
             'os': 'win',
             'arch': 'i386',
             'baseName': 'Ext1',
             'repository_type': 'git',
             'repository_url': 'http://slicer.com/extension/Ext',
             'revision': '54342',
             'app_revision': DRAFT_RELEASES[0]['revision'],
-            'description': 'Extension for Slicer 4 new version'
-        }
+            'description': 'Extension for Slicer 4 new version',
+        },
     },
     {
         'filepath': 'extension2.tar.gz',
         'meta': {
             'os': 'linux',
             'arch': 'amd64',
             'baseName': 'Ext2',
             'repository_type': 'gitlab',
             'repository_url': 'http://slicer.com/extension/Ext',
             'revision': '542',
             'app_revision': DRAFT_RELEASES[1]['revision'],
-            'description': 'Extension for Slicer 4 new version'
-        }
+            'description': 'Extension for Slicer 4 new version',
+        },
     },
     {
         'filepath': 'extension3.tar.gz',
         'meta': {
             'os': 'macosx',
             'arch': 'amd64',
             'baseName': 'Ext2',
             'repository_type': 'gitlab',
             'repository_url': 'http://slicer.com/extension/Ext',
             'revision': '542',
             'app_revision': DRAFT_RELEASES[1]['revision'],
-            'description': 'Extension for Slicer 4 new version'
-        }
+            'description': 'Extension for Slicer 4 new version',
+        },
     },
     {
         'filepath': 'extension4.tar.gz',
         'meta': {
             'os': 'macosx',
             'arch': 'i386',
             'baseName': 'Ext2',
             'repository_type': 'gitlab',
             'repository_url': 'http://slicer.com/extension/Ext',
             'revision': '542',
             'app_revision': DRAFT_RELEASES[1]['revision'],
-            'description': 'Extension for Slicer 4 new version'
-        }
-    }
+            'description': 'Extension for Slicer 4 new version',
+        },
+    },
 ]
 
 EXTENSIONS = []
 EXTENSIONS.extend(RELEASE_EXTENSIONS)
 EXTENSIONS.extend(DRAFT_EXTENSIONS)
 
 for extension in EXTENSIONS:
@@ -121,139 +121,141 @@
             'os': 'macosx',
             'arch': 'amd64',
             'baseName': 'pkg0',
             'repository_type': 'gitlab',
             'repository_url': 'https://slicer4.com',
             'revision': RELEASES[0]['revision'],
             'version': RELEASES[0]['version'],
-        }
-    }
+        },
+    },
 ]
 
 DRAFT_PACKAGES = [
     {
         'filepath': 'pkg1.exe',
         'meta': {
             'os': 'win',
             'arch': 'i386',
             'baseName': 'pkg1',
             'repository_type': 'gitlab',
             'repository_url': 'https://slicer4.com',
             'revision': DRAFT_RELEASES[0]['revision'],
             'version': DRAFT_RELEASES[0]['version'],
-        }
+        },
     },
     {
         'filepath': 'pkg2.tar.gz',
         'meta': {
             'os': 'linux',
             'arch': 'amd64',
             'baseName': 'pkg2',
             'repository_type': 'git',
             'repository_url': 'git://slicer4.com',
             'revision': DRAFT_RELEASES[0]['revision'],
             'version': DRAFT_RELEASES[0]['version'],
-        }
-    }
+        },
+    },
 ]
 
 PACKAGES = []
 PACKAGES.extend(RELEASE_PACKAGES)
 PACKAGES.extend(DRAFT_PACKAGES)
 
 for package in PACKAGES:
     package['name'] = APPLICATION_PACKAGE_TEMPLATE_NAME.format(**package['meta'])
 
 expectedDownloadStats = {
     DRAFT_RELEASES[0]['revision']: {
         'applications': {
             'win': {
-                'i386': 1
+                'i386': 1,
             },
             'linux': {
-                'amd64': 1
-            }
+                'amd64': 1,
+            },
         },
         'extensions': {
             'Ext1': {
                 'win': {
-                    'i386': 1
-                }
-            }
-        }
+                    'i386': 1,
+                },
+            },
+        },
     },
     DRAFT_RELEASES[1]['revision']: {
         'extensions': {
             'Ext2': {
                 'linux': {
-                    'amd64': 1
+                    'amd64': 1,
                 },
                 'macosx': {
                     'amd64': 1,
-                    'i386': 1
-                }
-            }
-        }
+                    'i386': 1,
+                },
+            },
+        },
     },
     RELEASES[0]['revision']: {
         'applications': {
             'macosx': {
-                'amd64': 1
-            }
+                'amd64': 1,
+            },
         },
         'extensions': {
             'Ext0': {
                 'linux': {
-                    'i386': 1
-                }
-            }
-        }
-    }
+                    'i386': 1,
+                },
+            },
+        },
+    },
 }
 
 
 def computeContentChecksum(algo, content):
     """Compute digest of ``content`` using ``algo``.
 
     Supported hashing algorithms are SHA256, SHA512, and MD5.
 
     :raises ValueError: if algo is unknown.
     """
     import hashlib
 
     if algo not in ['SHA256', 'SHA512', 'MD5']:
-        raise ValueError("unsupported hashing algorithm %s" % algo)
+        msg = f"unsupported hashing algorithm {algo}"
+        raise ValueError(msg)
 
-    hash = hashlib.new(algo)
-    hash.update(content)
-    return hash.hexdigest()
+    digest = hashlib.new(algo)
+    digest.update(content)
+    return digest.hexdigest()
 
 
 def computeFileChecksum(algo, filePath):
     """Compute digest of ``filePath`` using ``algo``.
 
     Supported hashing algorithms are SHA256, SHA512, and MD5.
     It internally reads the file by chunk of 8192 bytes.
 
     :raises ValueError: if algo is unknown.
     :raises IOError: if filePath does not exist.
     """
     import hashlib
 
     if algo not in ['SHA256', 'SHA512', 'MD5']:
-        raise ValueError("unsupported hashing algorithm %s" % algo)
+        msg = f"unsupported hashing algorithm {algo}"
+        raise ValueError(msg)
 
     with open(filePath, 'rb') as content:
-        hash = hashlib.new(algo)
+        digest = hashlib.new(algo)
         while True:
             chunk = content.read(8192)
             if not chunk:
                 break
-            hash.update(chunk)
-        return hash.hexdigest()
+            digest.update(chunk)
+        return digest.hexdigest()
 
 
 class ExternalData:
 
     def __init__(self, objectStorePath):
         self._downloadPercent = 0
         self._objectStorePath = objectStorePath
@@ -272,30 +274,35 @@
         return "%3.1f %s" % (size, 'TB')
 
     @staticmethod
     def _extractAlgoAndDigest(checksum):
         """Given a checksum string formatted as ``<algo>:<digest>`` returns the tuple ``(algo, digest)``.
 
         ``<algo>`` is expected to be `SHA256`, `SHA512`, or `MD5`.
-        ``<digest>`` is expected to be the full length hexdecimal digest.
+        ``<digest>`` is expected to be the full length hexadecimal digest.
 
         :raises ValueError: if checksum is incorrectly formatted.
         """
         if checksum is None:
             return None, None
         if len(checksum.split(':')) != 2:
-            raise ValueError("invalid checksum '%s'. Expected format is '<algo>:<digest>'." % checksum)
+            msg = f"invalid checksum '{checksum}'. Expected format is '<algo>:<digest>'."
+            raise ValueError(msg)
         (algo, digest) = checksum.split(':')
         expected_algos = ['SHA256', 'SHA512', 'MD5']
         if algo not in expected_algos:
-            raise ValueError("invalid algo '%s'. Algo must be one of %s" % (algo, ", ".join(expected_algos)))
+            msg = f"Invalid algo '{algo}'. Algo must be one of {', '.join(expected_algos)}."
+            raise ValueError(msg)
         expected_digest_length = {'SHA256': 64, 'SHA512': 128, 'MD5': 32}
         if len(digest) != expected_digest_length[algo]:
-            raise ValueError("invalid digest length %d. Expected digest length for %s is %d" % (
-                len(digest), algo, expected_digest_length[algo]))
+            msg  = (
+                f"Invalid digest length {len(digest)}. "
+                f"Expected digest length for {algo} is {expected_digest_length[algo]}."
+            )
+            raise ValueError(msg)
         return algo, digest
 
     def _reportHook(self, blocksSoFar, blockSize, totalSize):
         # we clamp to 100% because the blockSize might be larger than the file itself
         percent = min(int((100. * blocksSoFar * blockSize) / totalSize), 100)
         if percent == 100 or (percent - self._downloadPercent >= 10):
             # we clamp to totalSize when blockSize is larger than totalSize
@@ -318,16 +325,17 @@
             import urllib.error
             import urllib.parse
             import urllib.request
             print('Requesting download %s from %s ...' % (name, uri))
             try:
                 urllib.request.urlretrieve(uri, filePath, self._reportHook)
                 print('Download finished')
-            except IOError as exc:
-                raise ValueError(f"Failed to download {uri} to {filePath}: %s" % exc)
+            except OSError as exc:
+                msg = f"Failed to download {uri} to {filePath}: {exc}"
+                raise ValueError(msg)
 
             if algo is not None:
                 print('Verifying checksum')
                 current_digest = computeFileChecksum(algo, filePath)
                 if current_digest != digest:
                     print(
                         'Checksum verification failed. Computed checksum %s different from expected checksum %s' % (
@@ -367,17 +375,20 @@
         errors = set()
         for _attemptsCount in range(maximumAttemptsCount):
             try:
                 return self._downloadFile(uri, fileName, checksum)
             except ValueError as exc:
                 errors.add(str(exc))
                 continue
-        raise RuntimeError('Download of %s failed for %d attempts\n  uri: %s\n  errors: %s' % (
-            fileName, maximumAttemptsCount, uri, ", ".join(errors)
-        ))
+        msg = (
+            f"Download of {fileName} failed for {maximumAttemptsCount} attempts\n"
+            f"  uri: {uri}\n"
+            f"  errors: {', '.join(map(str, errors))}"
+        )
+        raise RuntimeError(msg)
 
 
 def downloadExternals(key_files, dest_dir):
     """
     Download the data files identified by the key files from https://data.kitware.com.
 
     :param key_files: List of the data file with a “.sha512” extension appended to the file name.
@@ -392,33 +403,34 @@
             external = key_file + "." + ext
             if os.path.exists(external):
                 break
             else:
                 ext_not_found.append(ext)
                 external = None
         if external is None:
-            raise ValueError("{}.{} not found".format(key_file, ", ".join(ext_not_found)))
+            msg = f"{key_file}.{', '.join(ext_not_found)} not found"
+            raise ValueError(msg)
         with open(external) as content:
             hashsum = content.read().strip()
         externals[os.path.basename(key_file)] = (ext, hashsum)
 
     external_data_dir = os.environ.get(
         'GIRDER_TEST_DATA_PREFIX', os.path.join(os.path.dirname(__file__), ".external_data"))
 
     # Download files
     downloaded_files = []
     for fileName, value in externals.items():
         algo, checksum = value
         print("fileName [%s] algo [%s] checksum [%s]" % (fileName, algo, checksum))
         downloaded_files.append(
             ExternalData(external_data_dir).download(
-                uri="https://data.kitware.com/api/v1/file/hashsum/{}/{}/download".format(algo, checksum),
+                uri=f"https://data.kitware.com/api/v1/file/hashsum/{algo}/{checksum}/download",
                 fileName=fileName,
-                checksum="{}:{}".format(algo.upper(), checksum)
-            )
+                checksum=f"{algo.upper()}:{checksum}",
+            ),
         )
 
     # Copy download files to temporary directory
     for downloaded_file in downloaded_files:
         copyfile(downloaded_file, dest_dir.join(os.path.basename(downloaded_file)))
 
     return dest_dir
```

### Comparing `slicer_package_manager-0.7.1/tests/test_slicer_package_manager.py` & `slicer_package_manager-0.8.0/tests/test_slicer_package_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pytest
 
 from bson.objectid import ObjectId
 
 from girder.models.collection import Collection
 from girder.models.folder import Folder
 from girder.models.file import File
+from girder.models.item import Item
 from girder.models.user import User
 
 from pytest_girder.assertions import assertStatus, assertStatusOk
 from pytest_girder.utils import getResponseBody
 
 from slicer_package_manager import constants, utilities
 
@@ -24,296 +25,310 @@
     DRAFT_PACKAGES,
     DRAFT_RELEASES,
     EXTENSIONS,
     FIXTURE_DIR,
     PACKAGES,
     RELEASE_EXTENSIONS,
     RELEASE_PACKAGES,
-    RELEASES
+    RELEASES,
 )
 
 
 @pytest.fixture(name='user')
 def fixture_user():
-    yield User().createUser('usr0', 'passwd', 'tst', 'usr', 'u@u.com')
+    return User().createUser('usr0', 'passwd', 'tst', 'usr', 'u@u.com')
 
 
 @pytest.fixture(name='collection')
 def fixture_collection(user):
-    yield Collection().createCollection(
+    return Collection().createCollection(
         'testCollection',
         creator=user,
-        description='Contain applications'
+        description='Contain applications',
     )
 
 
 @pytest.fixture(name='packages_folder')
 def fixture_packages_folder(user, collection):
-    yield Folder().createFolder(
+    return Folder().createFolder(
         parent=collection,
         name=constants.TOP_LEVEL_FOLDER_NAME,
         parentType='Collection',
         public=True,
-        creator=user
+        creator=user,
     )
 
 
 @pytest.fixture(name='app_folder')
 def fixture_app_folder(user, packages_folder):
     folder = Folder().createFolder(
         parent=packages_folder,
         name='application',
         description='app description',
         parentType='Folder',
         public=True,
-        creator=user
+        creator=user,
     )
     folder = Folder().setMetadata(
         folder,
         {
             'applicationPackageNameTemplate': constants.APPLICATION_PACKAGE_TEMPLATE_NAME,
-            'extensionPackageNameTemplate': constants.EXTENSION_PACKAGE_TEMPLATE_NAME
-        }
+            'extensionPackageNameTemplate': constants.EXTENSION_PACKAGE_TEMPLATE_NAME,
+        },
     )
-    yield folder
+    return folder
 
 
 @pytest.fixture(name='draft_release_folder')
 def fixture_draft_release_folder(user, app_folder):
-    yield Folder().createFolder(
+    return Folder().createFolder(
         parent=app_folder,
         name=constants.DRAFT_RELEASE_NAME,
         description='Uploaded each night, always up-to-date',
         parentType='Folder',
         public=True,
-        creator=user
+        creator=user,
     )
 
 
 @pytest.fixture(name='draft_release_revision_folder')
 def fixture_draft_release_revision_folder(user, draft_release_folder):
     folder = Folder().createFolder(
         parent=draft_release_folder,
         name=DRAFT_RELEASES[0]['revision'],
         parentType='Folder',
         public=True,
-        creator=user
+        creator=user,
     )
     folder = Folder().setMetadata(folder, {'revision': DRAFT_RELEASES[0]['revision']})
-    yield folder
+    return folder
 
 
 @pytest.fixture(name='release_folder')
 def fixture_release_folder(user, app_folder):
     folder = Folder().createFolder(
         parent=app_folder,
         name='release1',
         description='release description',
         parentType='Folder',
         public=True,
-        creator=user
+        creator=user,
     )
     folder = Folder().setMetadata(folder, {'revision': RELEASES[0]['revision']})
-    yield folder
+    return folder
 
 
 @pytest.fixture(name='release_extensions')
 def fixture_release_extensions(server, user, app_folder, release_folder, tmpdir, fsAssetstore):
+    # Fix warnings related to fixtures not explicitly used.
+    assert fsAssetstore
+
     downloadExternals(
         [os.path.join(FIXTURE_DIR, extension['filepath']) for extension in RELEASE_EXTENSIONS],
-        tmpdir
+        tmpdir,
     )
 
     extensions = [_createOrUpdatePackage(
         server, 'extension', extension['meta'],
         filePath=tmpdir.join(extension['filepath']),
-        _user=user, _app=app_folder
+        _user=user, _app=app_folder,
     ) for extension in RELEASE_EXTENSIONS]
 
     for index, extension in enumerate(extensions):
         assert extension['name'] == RELEASE_EXTENSIONS[index]['name']
         isRelease = RELEASE_EXTENSIONS[index]['meta']['app_revision'] == release_folder['meta']['revision']
         assert isRelease
         extensions_folder = Folder().load(extension['folderId'], user=user)
         assert ObjectId(extensions_folder['parentId']) == release_folder['_id']
 
-    yield extensions
+    return extensions
 
 
 @pytest.fixture(name='draft_extensions')
 def fixture_draft_extensions(server, user, app_folder, release_folder, draft_release_folder, tmpdir, fsAssetstore):
+    # Fix warnings related to fixtures not explicitly used.
+    assert draft_release_folder
+    assert fsAssetstore
+
     downloadExternals(
         [os.path.join(FIXTURE_DIR, extension['filepath']) for extension in DRAFT_EXTENSIONS],
-        tmpdir
+        tmpdir,
     )
 
     extensions = [_createOrUpdatePackage(
         server, 'extension', extension['meta'],
         filePath=tmpdir.join(extension['filepath']),
-        _user=user, _app=app_folder
+        _user=user, _app=app_folder,
     ) for extension in DRAFT_EXTENSIONS]
 
     for index, extension in enumerate(extensions):
         assert extension['name'] == DRAFT_EXTENSIONS[index]['name']
         isRelease = DRAFT_EXTENSIONS[index]['meta']['app_revision'] == release_folder['meta']['revision']
         assert not isRelease
 
-    yield extensions
+    return extensions
 
 
 @pytest.fixture(name='extensions')
 def fixture_extensions(release_extensions, draft_extensions):
     extensions = []
     extensions.extend(release_extensions)
     extensions.extend(draft_extensions)
-    yield extensions
+    return extensions
 
 
 @pytest.fixture(name='release_packages')
 def fixture_release_packages(server, user, app_folder, release_folder, tmpdir, fsAssetstore):
+    # Fix warnings related to fixtures not explicitly used.
+    assert fsAssetstore
+
     downloadExternals(
         [os.path.join(FIXTURE_DIR, package['filepath']) for package in RELEASE_PACKAGES],
-        tmpdir
+        tmpdir,
     )
     packages = [_createOrUpdatePackage(
         server, 'package', package['meta'],
         filePath=tmpdir.join(package['filepath']),
-        _user=user, _app=app_folder
+        _user=user, _app=app_folder,
     ) for package in RELEASE_PACKAGES]
 
     for index, package in enumerate(packages):
         assert package['name'] == RELEASE_PACKAGES[index]['name']
         isRelease = RELEASE_PACKAGES[index]['meta']['revision'] == release_folder['meta']['revision']
         assert isRelease
         assert ObjectId(package['folderId']) == release_folder['_id']
         assert package['meta']['release'] == release_folder['name']
 
-    yield packages
+    return packages
 
 
 @pytest.fixture(name='draft_packages')
 def fixture_draft_packages(server, user, app_folder, release_folder, draft_release_folder, tmpdir, fsAssetstore):
+    # Fix warnings related to fixtures not explicitly used.
+    assert draft_release_folder
+    assert fsAssetstore
+
     downloadExternals(
         [os.path.join(FIXTURE_DIR, package['filepath']) for package in DRAFT_PACKAGES],
-        tmpdir
+        tmpdir,
     )
     packages = [_createOrUpdatePackage(
         server, 'package', package['meta'],
         filePath=tmpdir.join(package['filepath']),
-        _user=user, _app=app_folder
+        _user=user, _app=app_folder,
     ) for package in DRAFT_PACKAGES]
 
     for index, package in enumerate(packages):
         assert package['name'] == DRAFT_PACKAGES[index]['name']
         isRelease = DRAFT_PACKAGES[index]['meta']['revision'] == release_folder['meta']['revision']
         assert not isRelease
         assert 'release' not in package['meta']
 
-    yield packages
+    return packages
 
 
 @pytest.fixture(name='packages')
 def fixture_packages(release_packages, draft_packages):
     packages = []
     packages.extend(release_packages)
     packages.extend(draft_packages)
-    yield packages
+    return packages
 
 
 @pytest.mark.plugin('slicer_package_manager')
 def testInitApp(server, user, collection):
     _createApplicationCheck(
         server,
         'App_test',
         'Application without specifying any collection',
         collDescription='Automatic creation of the collection Applications',
-        _user=user
+        _user=user,
     )
     # Without any collection this should load the 'Applications' collection
     _createApplicationCheck(
         server,
         'App_test1',
         'Application without specifying any collection',
-        _user=user
+        _user=user,
     )
     # With a collection ID this should load the collection
     _createApplicationCheck(
         server,
         'App_test2',
         'Application with a collection ID',
         collId=collection['_id'],
-        _user=user
+        _user=user,
     )
     # With a collection name that match an existing collection name
     _createApplicationCheck(
         server,
         'App_test3',
         'Application with a collection name',
         collName=collection['name'],
-        _user=user
+        _user=user,
     )
     # With a collection name that does not exist yet
     _createApplicationCheck(
         server,
         'App_test4',
         'Application with a collection name',
         collName='Collection_for_app',
-        _user=user
+        _user=user,
     )
 
 
 @pytest.mark.plugin('slicer_package_manager')
 def testListApp(server, user, collection, app_folder):
     # Create applications in the 'Applications' collection
     app1 = _createApplicationCheck(
         server,
         'App_test1',
         'Application without specifying any collection',
         collDescription='Automatic creation of the collection Applications',
-        _user=user
+        _user=user,
     )
     app2 = _createApplicationCheck(
         server,
         'App_test2',
         'Application without specifying any collection',
         collDescription='Automatic creation of the collection Applications',
-        _user=user
+        _user=user,
     )
 
     # Get application with application ID
     resp = server.request(
         path='/app',
         method='GET',
         user=user,
-        params={'app_id': app_folder['_id']}
+        params={'app_id': app_folder['_id']},
     )
     assertStatusOk(resp)
     assert ObjectId(resp.json['_id']) == app_folder['_id']
     assert resp.json['name'] == app_folder['name']
     assert resp.json['description'] == app_folder['description']
     assert resp.json['meta']['applicationPackageNameTemplate'] == constants.APPLICATION_PACKAGE_TEMPLATE_NAME
     assert resp.json['meta']['extensionPackageNameTemplate'] == constants.EXTENSION_PACKAGE_TEMPLATE_NAME
     # List all applications from 'Applications' collection (Default)
     resp = server.request(
         path='/app',
         method='GET',
-        user=user
+        user=user,
     )
     assertStatusOk(resp)
     assert len(resp.json) == 2
     assert resp.json[0]['_id'] == app1['_id']
     assert resp.json[1]['_id'] == app2['_id']
     # Get application with exact name
     resp = server.request(
         path='/app',
         method='GET',
         user=user,
         params={
             'collection_id': collection['_id'],
-            'name': app_folder['name']}
+            'name': app_folder['name']},
     )
     assertStatusOk(resp)
     assert ObjectId(resp.json[0]['_id']) == app_folder['_id']
     assert resp.json[0]['name'] == app_folder['name']
     assert resp.json[0]['description'] == app_folder['description']
     assert resp.json[0]['meta']['applicationPackageNameTemplate'] == constants.APPLICATION_PACKAGE_TEMPLATE_NAME
     assert resp.json[0]['meta']['extensionPackageNameTemplate'] == constants.EXTENSION_PACKAGE_TEMPLATE_NAME
@@ -324,72 +339,72 @@
     # Create the application without any collection,
     # this should create the new 'Applications' collection
     app = _createApplicationCheck(
         server,
         'App_test',
         'Application without specifying any collection',
         collDescription='Automatic creation of the collection Applications',
-        _user=user
+        _user=user,
     )
     # Get the new application by ID
     resp = server.request(
         path='/app',
         method='GET',
         user=user,
-        params={'app_id': app['_id']}
+        params={'app_id': app['_id']},
     )
     assertStatusOk(resp)
     assert resp.json['_id'] == app['_id']
     assert resp.json['name'] == app['name']
     # Delete the application
     resp = server.request(
         path='/app/%s' % app['_id'],
         method='DELETE',
-        user=user
+        user=user,
     )
     assertStatusOk(resp)
-    assert resp.json['_id'] == app['_id']
+    assert resp.json['message'] == f"Deleted application {app['name']}."
     # Try to get the application should failed
     resp = server.request(
         path='/app',
         method='GET',
         user=user,
-        params={'app_id': app['_id']}
+        params={'app_id': app['_id']},
     )
     assertStatusOk(resp)
     assert resp.json is None
 
 
 @pytest.mark.plugin('slicer_package_manager')
 def testNewRelease(server, user, app_folder):
     _createReleaseCheck(
         server,
         name='V3.2.1',
         app_id=app_folder['_id'],
         app_revision='001',
         desc='This is a new release',
-        _user=user
+        _user=user,
     )
 
 
 @pytest.mark.plugin('slicer_package_manager')
 def testGetRelease(server, user, app_folder, release_folder, draft_release_folder):
     release1 = _createReleaseCheck(
         server,
         name='V3.2.1',
         app_id=app_folder['_id'],
         app_revision='002',
         desc='This is a new release',
-        _user=user
+        _user=user,
     )
 
     resp = server.request(
         path='/app/%s/release' % app_folder['_id'],
         method='GET',
-        user=user
+        user=user,
     )
     # Check if it has return all the stable releases
     assertStatusOk(resp)
     assert len(resp.json) == 2
     assert resp.json[0]['_id'] == release1['_id']
     assert ObjectId(resp.json[1]['_id']) == release_folder['_id']
 
@@ -429,39 +444,39 @@
 
 
 @pytest.mark.plugin('slicer_package_manager')
 def testGetAllDraftRelease(server, user, app_folder, draft_release_revision_folder):
     resp = server.request(
         path='/app/%s/draft' % app_folder['_id'],
         method='GET',
-        user=user
+        user=user,
     )
     # Check if it has return all the revision from the default release
     assertStatusOk(resp)
     assert len(resp.json) == 1
     assert ObjectId(resp.json[0]['_id']) == draft_release_revision_folder['_id']
     assert resp.json[0]['meta']['revision'] == draft_release_revision_folder['meta']['revision']
     # With the parameter 'revision'
     resp = server.request(
         path='/app/%s/draft' % app_folder['_id'],
         method='GET',
         user=user,
-        params={'revision': draft_release_revision_folder['meta']['revision']}
+        params={'revision': draft_release_revision_folder['meta']['revision']},
     )
     # Check if it has return the good revision from the draft folder
     assertStatusOk(resp)
     assert len(resp.json) == 1
     assert ObjectId(resp.json[0]['_id']) == draft_release_revision_folder['_id']
     assert resp.json[0]['meta']['revision'] == draft_release_revision_folder['meta']['revision']
     # With the parameter 'revision' set to a wrong value
     resp = server.request(
         path='/app/%s/draft' % app_folder['_id'],
         method='GET',
         user=user,
-        params={'revision': 'wrongRev'}
+        params={'revision': 'wrongRev'},
     )
     # Check if it has return the good revision from the draft folder
     assertStatusOk(resp)
     assert len(resp.json) == 0
 
 
 @pytest.mark.plugin('slicer_package_manager')
@@ -472,108 +487,112 @@
 @pytest.mark.plugin('slicer_package_manager')
 def testDeleteReleaseByName(server, user, app_folder):
     _deleteRelease(server, 'name', _user=user, _app=app_folder)
 
 
 @pytest.mark.plugin('slicer_package_manager')
 def testDeleteRevisionRelease(server, user, app_folder, packages, extensions):
+    # Fix warnings related to fixtures not explicitly used.
+    assert packages
+    assert extensions
+
     resp = server.request(
         path='/app/%s/draft' % app_folder['_id'],
         method='GET',
-        user=user
+        user=user,
     )
 
     # Check if it has return all the revision from the default release
     assertStatusOk(resp)
     assert len(resp.json) == 2
 
     # Delete by Name the revision release '0001' in the "draft" release
     resp = server.request(
         path='/app/%s/release/%s' %
              (app_folder['_id'], EXTENSIONS[3]['meta']['app_revision']),
         method='DELETE',
-        user=user
+        user=user,
     )
     assertStatusOk(resp)
 
     resp = server.request(
         path='/app/%s/draft' % app_folder['_id'],
         method='GET',
-        user=user
+        user=user,
     )
     # Check if it has return all the revision from the default release
     assertStatusOk(resp)
     assert len(resp.json) == 1
 
 
 @pytest.mark.plugin('slicer_package_manager')
 def testUpdateExtensions(server, user, app_folder, extensions):
     # Update the same extension
     newParams = EXTENSIONS[1]['meta'].copy()
     newParams.update({
         'revision': '0000',
         'repository_type': 'gitlab',
-        'description': 'Extension for Slicer 4 new version 2'
+        'description': 'Extension for Slicer 4 new version 2',
     })
     updatedExtension = _createOrUpdatePackage(server, 'extension', newParams, _user=user, _app=app_folder)
     # Check the same extension has different metadata
     assert updatedExtension['_id'] == extensions[1]['_id']
     assert updatedExtension['name'] == constants.EXTENSION_PACKAGE_TEMPLATE_NAME.format(**newParams)
     assert updatedExtension['meta'] != extensions[1]['meta']
 
 
 @pytest.mark.plugin('slicer_package_manager')
 def testGetExtensions(server, user, app_folder, release_folder, extensions):
     # Get all the extension of the application
     resp = server.request(
         path='/app/%s/extension' % app_folder['_id'],
         method='GET',
-        user=user
+        user=user,
     )
     assertStatusOk(resp)
     assert len(resp.json) == len(EXTENSIONS)
 
     # Get all the extension of the application for Linux
     resp = server.request(
         path='/app/%s/extension' % app_folder['_id'],
         method='GET',
         user=user,
         params={
-            'os': 'linux'
-        }
+            'os': 'linux',
+        },
     )
     assertStatusOk(resp)
     assert len(resp.json) == 2
     for ext in resp.json:
         assert ext['meta']['os'] == 'linux'
 
     # Get all the extension of the application for Linux and amd64 architecture
     resp = server.request(
         path='/app/%s/extension' % app_folder['_id'],
         method='GET',
         user=user,
         params={
             'os': 'linux',
-            'arch': 'amd64'
-        }
+            'arch': 'amd64',
+        },
     )
     assertStatusOk(resp)
     assert len(resp.json) == 1
     for ext in resp.json:
         assert ext['meta']['os'] == 'linux'
         assert ext['meta']['arch'] == 'amd64'
 
     # Get all the extension of the application which are in "release1"
     resp = server.request(
         path='/app/%s/extension' % app_folder['_id'],
         method='GET',
         user=user,
         params={
-            'release_id': release_folder['_id']
-        }
+            'release_id': release_folder['_id'],
+        },
     )
     assertStatusOk(resp)
     assert len(resp.json) == 1
 
     # Get all the extension of the application which are in the draft release
     draftRelease = list(Folder().childFolders(
         app_folder,
@@ -581,16 +600,16 @@
         user=user,
         filters={'name': constants.DRAFT_RELEASE_NAME}))
     resp = server.request(
         path='/app/%s/extension' % app_folder['_id'],
         method='GET',
         user=user,
         params={
-            'release_id': draftRelease[0]['_id']
-        }
+            'release_id': draftRelease[0]['_id'],
+        },
     )
     assertStatusOk(resp)
     assert len(resp.json) == 4
 
     # Get a specific extension by name
     resp = server.request(
         path='/app/%s/extension' % app_folder['_id'],
@@ -618,36 +637,36 @@
 def testDeleteExtensionPackages(server, user, app_folder, release_folder):
     # Create a new extension in the release "_release"
     extension = _createOrUpdatePackage(
         server,
         'extension',
         EXTENSIONS[0]['meta'],
         _user=user,
-        _app=app_folder
+        _app=app_folder,
     )
     assert extension['name'] == EXTENSIONS[0]['name']
     extensions_folder = Folder().load(extension['folderId'], user=user)
     assert ObjectId(extensions_folder['parentId']) == release_folder['_id']
     # Get, delete, and try to re-get the package
     _deletePackages(server, 'extension', extension, _user=user, _app=app_folder)
 
 
 @pytest.mark.external_data(
-    os.path.join(FIXTURE_DIR, PACKAGES[2]['filepath'])
+    os.path.join(FIXTURE_DIR, PACKAGES[2]['filepath']),
 )
 @pytest.mark.plugin('slicer_package_manager')
 def testUploadAndDownloadPackages(server, user, app_folder, packages, external_data):
     # Try to create the same application package should just get the same one
     package2 = _createOrUpdatePackage(
         server,
         'package',
         PACKAGES[2]['meta'],
         external_data.join(PACKAGES[2]['filepath']),
         _user=user,
-        _app=app_folder
+        _app=app_folder,
     )
     assert package2['name'] == packages[2]['name']
 
 
 @pytest.mark.plugin('slicer_package_manager')
 def testUpdatePackages(server, user, app_folder, packages):
     # Update the same package
@@ -665,53 +684,53 @@
 
 @pytest.mark.plugin('slicer_package_manager')
 def testGetPackages(server, user, app_folder, release_folder, packages):
     # Get all the package of the application
     resp = server.request(
         path='/app/%s/package' % app_folder['_id'],
         method='GET',
-        user=user
+        user=user,
     )
     assertStatusOk(resp)
     assert len(resp.json) == 3
 
     # Get all the package of the application for Linux
     resp = server.request(
         path='/app/%s/package' % app_folder['_id'],
         method='GET',
         user=user,
         params={
-            'os': 'linux'
-        }
+            'os': 'linux',
+        },
     )
     assertStatusOk(resp)
     assert len(resp.json) == 1
     assert resp.json[0]['meta']['os'] == 'linux'
 
     # Get all the package of the application for Linux and amd64 architecture
     resp = server.request(
         path='/app/%s/package' % app_folder['_id'],
         method='GET',
         user=user,
         params={
             'os': 'macosx',
-            'arch': 'i386'
-        }
+            'arch': 'i386',
+        },
     )
     assertStatusOk(resp)
     assert len(resp.json) == 0
 
     # Get all the package of the application which are in "release1"
     resp = server.request(
         path='/app/%s/package' % app_folder['_id'],
         method='GET',
         user=user,
         params={
-            'release_id_or_name': release_folder['_id']
-        }
+            'release_id_or_name': release_folder['_id'],
+        },
     )
     assertStatusOk(resp)
     assert len(resp.json) == 1
 
     # Get all the package of the application which are in the draft release
     draftRelease = list(Folder().childFolders(
         app_folder,
@@ -719,16 +738,16 @@
         user=user,
         filters={'name': constants.DRAFT_RELEASE_NAME}))
     resp = server.request(
         path='/app/%s/package' % app_folder['_id'],
         method='GET',
         user=user,
         params={
-            'release_id_or_name': draftRelease[0]['_id']
-        }
+            'release_id_or_name': draftRelease[0]['_id'],
+        },
     )
     assertStatusOk(resp)
     assert len(resp.json) == 2
 
     # Get a specific package by name
     resp = server.request(
         path='/app/%s/package' % app_folder['_id'],
@@ -755,31 +774,34 @@
 @pytest.mark.plugin('slicer_package_manager')
 def testDeleteApplicationPackages(server, user, app_folder, release_folder):
     package = _createOrUpdatePackage(
         server,
         'package',
         PACKAGES[0]['meta'],
         _user=user,
-        _app=app_folder
+        _app=app_folder,
     )
     assert package['name'] == PACKAGES[0]['name']
     assert ObjectId(package['folderId']) == release_folder['_id']
 
     # Get, delete, and try to re-get the package
     _deletePackages(server, 'package', package, _user=user, _app=app_folder)
 
 
 @pytest.mark.plugin('slicer_package_manager')
 def testDownloadStats(server, user, app_folder, draft_release_revision_folder, packages, extensions):
+    # Fix warnings related to fixtures not explicitly used.
+    assert packages
+
     # Get the downloadStats
     expectedStats = expectedDownloadStats
     resp = server.request(
         path='/app/%s/downloadstats' % app_folder['_id'],
         method='GET',
-        user=user
+        user=user,
     )
     assertStatusOk(resp)
     assert resp.json == expectedStats
 
     # Download multiple time an extension
     ext3_file = list(File().find({'itemId': ObjectId(extensions[3]['_id'])}))
     ext4_file = list(File().find({'itemId': ObjectId(extensions[4]['_id'])}))
@@ -787,66 +809,69 @@
     N = 5
     for _idx in range(N):
         _downloadFile(server, ext3_file[0]['_id'], _user=user)
         _downloadFile(server, ext4_file[0]['_id'], _user=user)
 
     expectedStats['0001']['extensions']['Ext2']['macosx'].update({
         'amd64': N + expectedStats['0001']['extensions']['Ext2']['macosx']['amd64'],
-        'i386': N + expectedStats['0001']['extensions']['Ext2']['macosx']['i386']
+        'i386': N + expectedStats['0001']['extensions']['Ext2']['macosx']['i386'],
     })
     resp = server.request(
         path='/app/%s/downloadstats' % app_folder['_id'],
         method='GET',
-        user=user
+        user=user,
     )
     assertStatusOk(resp)
     assert resp.json == expectedStats
 
     # The download stats aren't affected by deletion of extension or revision
     # in the default release
     # Delete extensions
     resp = server.request(
         path='/app/%(app_id)s/extension/%(ext_id)s' % {
             'app_id': app_folder['_id'],
             'ext_id': extensions[3]['_id']},
         method='DELETE',
-        user=user
+        user=user,
     )
     assertStatusOk(resp)
     resp = server.request(
         path='/app/%(app_id)s/extension/%(ext_id)s' % {
             'app_id': app_folder['_id'],
             'ext_id': extensions[4]['_id']},
         method='DELETE',
-        user=user
+        user=user,
     )
     assertStatusOk(resp)
 
     # Delete the revision '0000' in the "draft" release
     resp = server.request(
         path='/app/%(app_id)s/release/%(release_id)s' % {
             'app_id': app_folder['_id'],
             'release_id': draft_release_revision_folder['_id']},
         method='DELETE',
-        user=user
+        user=user,
     )
     assertStatusOk(resp)
 
     # Check if download Stats are the same
     resp = server.request(
         path='/app/%s/downloadstats' % app_folder['_id'],
         method='GET',
-        user=user
+        user=user,
     )
     assertStatusOk(resp)
     assert resp.json == expectedStats
 
 
 @pytest.mark.plugin('slicer_package_manager')
 def testGetReleaseFolder(server, user, release_folder, packages, extensions):
+    # Fix warnings related to fixtures not explicitly used.
+    assert server
+
     # Release package
     release_package = packages[0]
     assert utilities.getReleaseFolder(release_package)['_id'] == release_folder['_id']
 
     # Draft package
     draft_package = packages[1]
     assert utilities.getReleaseFolder(draft_package)['name'] == constants.DRAFT_RELEASE_NAME
@@ -860,82 +885,91 @@
     # Draft extension
     draft_extension = extensions[1]
     assert utilities.getReleaseFolder(draft_extension)['name'] == constants.DRAFT_RELEASE_NAME
 
 
 @pytest.mark.plugin('slicer_package_manager')
 def testIsApplicationFolder(server, app_folder, release_folder, draft_release_folder, draft_release_revision_folder):
+    # Fix warnings related to fixtures not explicitly used.
+    assert server
+
     assert utilities.isApplicationFolder(app_folder)
     assert not utilities.isApplicationFolder(release_folder)
     assert not utilities.isApplicationFolder(draft_release_folder)
     assert not utilities.isApplicationFolder(draft_release_revision_folder)
 
 
 @pytest.mark.plugin('slicer_package_manager')
 def testIsReleaseFolder(server, app_folder, release_folder, draft_release_folder, draft_release_revision_folder):
+    # Fix warnings related to fixtures not explicitly used.
+    assert server
+
     assert not utilities.isReleaseFolder(app_folder)
     assert utilities.isReleaseFolder(release_folder)
     assert not utilities.isReleaseFolder(draft_release_folder)
     assert utilities.isReleaseFolder(draft_release_revision_folder)
 
 
 @pytest.mark.plugin('slicer_package_manager')
 def testIsDraftReleaseFolder(server, app_folder, release_folder, draft_release_folder, draft_release_revision_folder):
+    # Fix warnings related to fixtures not explicitly used.
+    assert server
+
     assert not utilities.isDraftReleaseFolder(app_folder)
     assert not utilities.isDraftReleaseFolder(release_folder)
     assert not utilities.isDraftReleaseFolder(draft_release_folder)
     assert utilities.isDraftReleaseFolder(draft_release_revision_folder)
 
 
 @pytest.mark.parametrize(
-    "action,method,src_folder,dest_folder,items,release_before,release_after",
+    ('action', 'method', 'src_folder', 'dest_folder', 'items', 'release_before', 'release_after'),
     [
         (
             'copy',
             'POST',
             pytest.lazy_fixture('draft_release_revision_folder'),
             pytest.lazy_fixture('release_folder'),
             pytest.lazy_fixture('draft_packages'),
             None,
-            RELEASES[0]['name']
+            RELEASES[0]['name'],
         ),
         (
             'copy',
             'POST',
             pytest.lazy_fixture('release_folder'),
             pytest.lazy_fixture('draft_release_revision_folder'),
             pytest.lazy_fixture('release_packages'),
             RELEASES[0]['name'],
-            None
+            None,
         ),
         (
             'move',
             'PUT',
             pytest.lazy_fixture('draft_release_revision_folder'),
             pytest.lazy_fixture('release_folder'),
             pytest.lazy_fixture('draft_packages'),
             None,
-            RELEASES[0]['name']
+            RELEASES[0]['name'],
         ),
         (
             'move',
             'PUT',
             pytest.lazy_fixture('release_folder'),
             pytest.lazy_fixture('draft_release_revision_folder'),
             pytest.lazy_fixture('release_packages'),
             RELEASES[0]['name'],
-            None
+            None,
         ),
     ],
     ids=[
         'copy_package_from_draft_to_release',
         'copy_package_from_release_to_draft',
         'move_package_from_draft_to_release',
-        'move_package_from_release_to_draft'
-    ]
+        'move_package_from_release_to_draft',
+    ],
 )
 @pytest.mark.plugin('slicer_package_manager')
 def testApplicationPackageMetadataAutoUpdate(
         server, user, action, method, src_folder, dest_folder, items, release_before, release_after):
 
     item = items[0]
 
@@ -945,88 +979,190 @@
     resp = server.request(
         path='/resource/%s' % action,
         method=method,
         user=user,
         params={
             'resources': json.dumps({'item': [item['_id']]}),
             'parentType': 'folder',
-            'parentId': dest_folder['_id']
-        }
+            'parentId': dest_folder['_id'],
+        },
     )
     assertStatusOk(resp)
 
     resp = server.request(
         path='/item',
         method='GET',
         user=user,
         params={
             'folderId': dest_folder['_id'],
-            'name': item['name']
-        }
+            'name': item['name'],
+        },
     )
     assertStatusOk(resp)
     item_after = resp.json[0]
 
     for key in ['name', 'size']:
         assert item_after[key] == item[key]
 
     for key in ['app_id', 'arch', 'baseName', 'os', 'revision']:
         assert item_after['meta'][key] == item['meta'][key]
 
     assert ObjectId(item_after['folderId']) == dest_folder['_id']
     assert item_after['meta'].get('release', None) == release_after
 
 
+@pytest.mark.plugin('slicer_package_manager')
+def testApplicationPackageMetadataChecksumUpdate_1(server, user, packages):
+    """Replace existing file and verify checksum is updated."""
+    item = Item().load(packages[0]['_id'], force=True)
+    file = list(Item().childFiles(item))[0]
+
+    # Replace file
+    updated_contents = "you've changed!"
+    _replaceFile(server, file["_id"], updated_contents, user)
+
+    # Confirm item checksum was updated
+    item_after = Item().load(item['_id'], force=True)
+    expected_checksum = computeContentChecksum("SHA512", updated_contents.encode("utf8"))
+    assert item_after["meta"]["sha512"] == expected_checksum
+
+
+@pytest.mark.plugin('slicer_package_manager')
+def testApplicationPackageMetadataChecksumUpdate_2(server, user, packages, tmpdir):
+    """Upload an additional file and verify checksum remains the same."""
+    item = Item().load(packages[1]['_id'], force=True)
+    assert Item().childFiles(item).count() == 1
+    item_first_file_sha512 = item["meta"]["sha512"]
+
+    # Upload additional file
+    filePath = tmpdir / "additional.tar.gz"
+    with open(filePath, "w") as content:
+        content.write("new file contents")
+    additional_file_sha512 = computeFileChecksum("SHA512", filePath)
+    assert item_first_file_sha512 != additional_file_sha512
+    with open(filePath) as content:
+        server.uploadFile(filePath, content.read(), user, item, parentType="item")
+
+    # Check the additional file was uploaded
+    item_after = Item().load(item['_id'], force=True)
+    assert Item().childFiles(item_after).count() == 2
+
+    # Confirm item checksum is unchanged
+    assert item_first_file_sha512 == item_after["meta"]["sha512"]
+
+
+@pytest.mark.plugin('slicer_package_manager')
+def testApplicationPackageMetadataChecksumUpdate_3(server, user, packages, tmpdir):
+    """Upload an additional file, remove the first one and verify the checksum matches
+    the one of the additional file.
+    """
+    item = Item().load(packages[2]['_id'], force=True)
+    assert Item().childFiles(item).count() == 1
+    item_first_file_sha512 = item["meta"]["sha512"]
+    item_first_file_id = list(Item().childFiles(item))[0]["_id"]
+
+    # Upload additional file
+    filePath = tmpdir / "additional.tar.gz"
+    with open(filePath, "w") as content:
+        content.write("new file contents")
+    additional_file_sha512 = computeFileChecksum("SHA512", filePath)
+    assert item_first_file_sha512 != additional_file_sha512
+    with open(filePath) as content:
+        server.uploadFile(filePath, content.read(), user, item, parentType="item")
+
+    # Check the additional file was uploaded
+    item_after = Item().load(item['_id'], force=True)
+    assert Item().childFiles(item_after).count() == 2
+
+    # Remove the first file
+    resp = server.request(
+        path='/file/%s' % item_first_file_id,
+        method='DELETE',
+        user=user,
+    )
+    assertStatusOk(resp)
+    item_after = Item().load(item['_id'], force=True)
+    assert Item().childFiles(item_after).count() == 1
+
+    # Confirm the item checksum was updated
+    assert item_after["meta"]["sha512"] != item_first_file_sha512
+    assert item_after["meta"]["sha512"] == additional_file_sha512
+
+
+@pytest.mark.plugin('slicer_package_manager')
+def testApplicationPackageMetadataChecksumUpdate_4(server, user, packages):
+    """Delete the last file and verify the checksum is set to an empty string."""
+    item = Item().load(packages[0]['_id'], force=True)
+    assert Item().childFiles(item).count() == 1
+    item_file_id = list(Item().childFiles(item))[0]["_id"]
+
+    # Remove the file
+    resp = server.request(
+        path='/file/%s' % item_file_id,
+        method='DELETE',
+        user=user,
+    )
+    assertStatusOk(resp)
+    item_after = Item().load(item['_id'], force=True)
+    assert Item().childFiles(item_after).count() == 0
+
+    # Confirm the item checksum was updated
+    assert not item_after["meta"]["sha512"]
+
+
 @pytest.mark.parametrize(
-    'build_date,expected_build_date,status_code', [
+    ('build_date', 'expected_build_date', 'status_code'), [
         (None, None, 200),
         ('2021-06-21 22:00:26', '2021-06-21T22:00:26+00:00', 200),
         ('2021-06-21T22:00:26+0000', '2021-06-21T22:00:26+00:00', 200),
         ('2021-06-21T22:00:26+00:00', '2021-06-21T22:00:26+00:00', 200),
         ('2021-06-21 11:37:36 -0400', '2021-06-21T15:37:36+00:00', 200),
         ('2021-06-23 02:54:11-04:00', '2021-06-23T06:54:11+00:00', 200),
-        ('abcdef', None, 400)
+        ('abcdef', None, 400),
     ],
     ids=[
         'default',
         'no-timezone',
         'timezone-without-colon',
         'timezone-with-colon',
         'git-date-iso-local',
         'date-rfc-3339-seconds',
-        'invalid'
-    ]
+        'invalid',
+    ],
 )
 @pytest.mark.plugin('slicer_package_manager')
 def testMetadataBuildDate(build_date, expected_build_date, status_code, server, user, app_folder, draft_release_folder):
+    # Fix warnings related to fixtures not explicitly used.
+    assert draft_release_folder
+
     newParams = PACKAGES[0]['meta'].copy()
     if build_date is not None:
         newParams['build_date'] = build_date
     package = _createOrUpdatePackage(
         server,
         'package',
         newParams,
         _user=user,
         _app=app_folder,
-        status_code=status_code
+        status_code=status_code,
     )
     if status_code != 200:
         return
     assert package['name'] == PACKAGES[0]['name']
     assert package['meta'].get('build_date')
     if expected_build_date is not None:
         assert package['meta'].get('build_date') == expected_build_date
 
 
 def _createApplicationCheck(server, appName, appDescription, collId=None,
                             collName=None, collDescription='', _user=None):
     params = {
         'name': appName,
         'app_description': appDescription,
-        'collection_description': collDescription
+        'collection_description': collDescription,
     }
     if not (collId or collName):
         collName = 'Applications'
         params.update({'collection_name': collName})
     elif collId:
         if not ObjectId.is_valid(collId):
             raise Exception("The ObjectId %s is not valid" % collId)
@@ -1036,15 +1172,15 @@
     else:
         params.update({'collection_name': collName})
 
     resp = server.request(
         path='/app',
         method='POST',
         user=_user,
-        params=params
+        params=params,
     )
     # Check if it has created the application
     assertStatusOk(resp)
     assert resp.json['name'] == appName
     assert resp.json['description'] == appDescription
     assert resp.json['meta']['applicationPackageNameTemplate'] == constants.APPLICATION_PACKAGE_TEMPLATE_NAME
     assert resp.json['meta']['extensionPackageNameTemplate'] == constants.EXTENSION_PACKAGE_TEMPLATE_NAME
@@ -1068,16 +1204,16 @@
     resp = server.request(
         path='/app/%s/release' % app_id,
         method='POST',
         user=_user,
         params={
             'name': name,
             'app_revision': app_revision,
-            'description': desc
-        }
+            'description': desc,
+        },
     )
     # Check if it has created the new release
     assertStatusOk(resp)
     assert resp.json['name'] == name
     assert resp.json['description'] == desc
     assert resp.json['meta']['revision'] == app_revision
     return resp.json
@@ -1087,15 +1223,15 @@
     # Create the release
     release = _createReleaseCheck(
         server,
         name='V3.2.1',
         app_id=_app['_id'],
         app_revision='001',
         desc='This is a new release',
-        _user=_user
+        _user=_user,
     )
     # Get the new release by name
     resp = server.request(
         path='/app/%s/release' % _app['_id'],
         params={'release_id_or_name': release[identifier]},
         method='GET',
         user=_user,
@@ -1105,18 +1241,18 @@
     assert resp.json['name'] == release['name']
     # Delete the release by name
     resp = server.request(
         path='/app/%(app_id)s/release/%(id_or_name)s' % {
             'app_id': _app['_id'],
             'id_or_name': release[identifier]},
         method='DELETE',
-        user=_user
+        user=_user,
     )
     assertStatusOk(resp)
-    assert resp.json['_id'] == release['_id']
+    assert resp.json['message'] == f"Deleted release {release['name']}."
     # Try to get the release should failed
     resp = server.request(
         path='/app/%s/release' % _app['_id'],
         params={'release_id_or_name': release[identifier]},
         method='GET',
         user=_user,
     )
@@ -1169,24 +1305,49 @@
 #         assert 'itemId' in uploadedFile
 #         assert uploadedFile['assetstoreId'] == str(self.assetstore['_id'])
 #         assert uploadedFile['name'] == filePath
 #         assert uploadedFile['size'] == size
 #     return uploadedFile
 
 
-def _downloadFile(server, id, _user=None):
+def _downloadFile(server, _id, _user=None):
     resp = server.request(
-        path='/file/%s/download' % id,
+        path="/file/%s/download" % _id,
         method='GET',
         user=_user,
         isJson=False)
     assertStatusOk(resp)
     return getResponseBody(resp, text=False)
 
 
+def _replaceFile(server, _id, contents, _user):
+
+    upload = server.request(
+        path='/file/%s/contents' % _id,
+        method='PUT',
+        user=_user,
+        params={
+            'size': len(contents),
+        })
+    assertStatusOk(upload)
+
+    resp = server.request(
+        path='/file/chunk',
+        method='POST',
+        user=_user,
+        body=contents,
+        params={
+            'uploadId': upload.json['_id'],
+            'offset': 0,
+        },
+        type='text/plain')
+    assertStatusOk(resp)
+    return getResponseBody(resp, text=False)
+
+
 def _createOrUpdatePackage(server, packageType, params, filePath=None, _user=None, _app=None, status_code=200):
     resp = server.request(
         path='/app/%s/%s' % (_app['_id'], packageType),
         method='POST',
         user=_user,
         params=params)
     assertStatus(resp, status_code)
@@ -1194,17 +1355,18 @@
     if status_code != 200:
         return None
 
     def _filtered(metadata):
         return {k: v for (k, v) in metadata.items() if k not in (
             'app_id',
             'build_date',
+            'sha512',
         )}
 
-    # assert every other field (besides unique ones) are identical
+    # assert every other fields (besides unique or computed ones) are identical
     assert _filtered(resp.json['meta']) == _filtered(params)
 
     if filePath:
         # Upload a package file
         item = resp.json
         with open(filePath, 'rb') as content:
             uploadedFile = server.uploadFile(
@@ -1215,45 +1377,49 @@
         local_checksum = computeFileChecksum('SHA512', filePath)
         assert downloaded_checksum == local_checksum
 
     resp = server.request(
         path='/app/%s/%s' % (_app['_id'], packageType),
         method='GET',
         user=_user,
-        params={'%s_id' % packageType: resp.json['_id']}
+        params={'%s_id' % packageType: resp.json['_id']},
     )
     assertStatusOk(resp)
 
     assert len(resp.json) == 1
 
+    if filePath:
+        item = resp.json[0]
+        assert item['meta']['sha512'] == local_checksum
+
     return resp.json[0]
 
 
 def _deletePackages(server, packageType, pkg, _user=None, _app=None):
     # Get all the  application package, this should only be the new one
     resp = server.request(
         path='/app/%s/%s' % (_app['_id'], packageType),
         method='GET',
-        user=_user
+        user=_user,
     )
     assertStatusOk(resp)
     assert len(resp.json) == 1
     assert resp.json[0]['_id'] == pkg['_id']
     # Delete the package
     resp = server.request(
         path='/app/%(app_id)s/%(type)s/%(pkg_id)s' % {
             'app_id': _app['_id'],
             'type': packageType,
             'pkg_id': pkg['_id']},
         method='DELETE',
-        user=_user
+        user=_user,
     )
     assertStatusOk(resp)
     assert resp.json['_id'] == pkg['_id']
     # Try to get the package shouldn't success
     resp = server.request(
         path='/app/%s/%s' % (_app['_id'], packageType),
         method='GET',
-        user=_user
+        user=_user,
     )
     assertStatusOk(resp)
     assert len(resp.json) == 0
```

### Comparing `slicer_package_manager-0.7.1/versioneer.py` & `slicer_package_manager-0.8.0/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 
 * Source trees which contain multiple subprojects, such as
   [Buildbot](https://github.com/buildbot/buildbot), which contains both
   "main" and "slave" subprojects, each with their own `setup.py`,
   `setup.cfg`, and `tox.ini`. Projects like these produce multiple PyPI
   distributions (and upload multiple independently-installable tarballs).
 * Source trees whose main purpose is to contain a C library, but which also
-  provide bindings to Python (and perhaps other langauges) in subdirectories.
+  provide bindings to Python (and perhaps other languages) in subdirectories.
 
 Versioneer will look for `.git` in parent directories, and most operations
 should get the right version string. However `pip` and `setuptools` have bugs
 and implementation details which frequently cause `pip install .` from a
 subproject directory to fail to find a correct version string (so it usually
 defaults to `0+unknown`).
 
@@ -684,15 +684,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%%s'"
                                %% describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -1076,15 +1076,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%s'"
                                % describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
```

