# Comparing `tmp/python-escpos-3.0a8.tar.gz` & `tmp/python-escpos-3.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-escpos-3.0a8.tar", last modified: Tue May 12 17:36:43 2020, max compression
+gzip compressed data, was "python-escpos-3.0a9.tar", last modified: Thu May 11 21:40:14 2023, max compression
```

## Comparing `python-escpos-3.0a8.tar` & `python-escpos-3.0a9.tar`

### file list

```diff
@@ -1,202 +1,207 @@
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.245532 python-escpos-3.0a8/
--rw-r--r--   0 patrick   (1000) patrick   (1000)       20 2017-05-26 00:39:06.000000 python-escpos-3.0a8/.coveragerc
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.217532 python-escpos-3.0a8/.github/
--rw-r--r--   0 patrick   (1000) patrick   (1000)      586 2017-05-26 00:39:06.000000 python-escpos-3.0a8/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 patrick   (1000) patrick   (1000)      263 2017-05-26 00:39:06.000000 python-escpos-3.0a8/.github/PULL_REQUEST_TEMPLATE.md
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.221532 python-escpos-3.0a8/.github/workflows/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1465 2020-05-08 23:45:42.000000 python-escpos-3.0a8/.github/workflows/pythonpackage.yml
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      460 2020-05-10 23:15:24.000000 python-escpos-3.0a8/.gitignore
--rw-r--r--   0 patrick   (1000) patrick   (1000)      140 2018-05-15 21:12:34.000000 python-escpos-3.0a8/.gitmodules
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1172 2020-05-08 20:43:09.000000 python-escpos-3.0a8/.mailmap
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2613 2020-05-12 17:05:45.000000 python-escpos-3.0a8/.travis.yml
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.221532 python-escpos-3.0a8/.vscode/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      308 2020-05-10 23:14:35.000000 python-escpos-3.0a8/.vscode/settings.json
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      385 2020-05-08 23:45:42.000000 python-escpos-3.0a8/.vscode/tasks.json
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      585 2020-05-08 23:45:42.000000 python-escpos-3.0a8/AUTHORS
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    11104 2020-05-12 17:31:49.000000 python-escpos-3.0a8/CHANGELOG.rst
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3307 2020-05-10 23:11:05.000000 python-escpos-3.0a8/CONTRIBUTING.rst
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      342 2020-05-08 23:45:42.000000 python-escpos-3.0a8/INSTALL
--rw-r--r--   0 patrick   (1000) patrick   (1000)     1097 2017-05-26 00:39:06.000000 python-escpos-3.0a8/LICENSE
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      332 2020-05-08 23:45:42.000000 python-escpos-3.0a8/MANIFEST.in
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5942 2020-05-12 17:36:43.245532 python-escpos-3.0a8/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3671 2020-05-10 23:11:05.000000 python-escpos-3.0a8/README.rst
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.217532 python-escpos-3.0a8/capabilities-data/
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.221532 python-escpos-3.0a8/capabilities-data/dist/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    67837 2020-05-08 22:39:57.000000 python-escpos-3.0a8/capabilities-data/dist/capabilities.json
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      128 2020-05-10 23:13:40.000000 python-escpos-3.0a8/codecov.yml
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.221532 python-escpos-3.0a8/doc/
--rw-r--r--   0 patrick   (1000) patrick   (1000)        8 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/.gitignore
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6961 2020-05-12 16:39:03.000000 python-escpos-3.0a8/doc/Makefile
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.217532 python-escpos-3.0a8/doc/_build/
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.217532 python-escpos-3.0a8/doc/_build/html/
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.221532 python-escpos-3.0a8/doc/_build/html/_sources/
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.225532 python-escpos-3.0a8/doc/_build/html/_sources/api/
--rw-r--r--   0 patrick   (1000) patrick   (1000)      208 2017-01-29 21:25:39.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/capabilities.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      208 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/capabilities.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      172 2017-01-29 21:27:58.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/cli.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      172 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/cli.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      196 2017-01-29 21:27:58.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/codepages.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      196 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/codepages.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      185 2016-06-24 09:25:19.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/config.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      185 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/config.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      197 2016-06-24 09:25:19.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/constants.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      197 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/constants.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      187 2016-06-24 09:25:19.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/escpos.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      187 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/escpos.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      180 2016-06-24 09:25:19.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/exceptions.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      180 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/exceptions.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      195 2016-07-23 14:47:59.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/image.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      195 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/image.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      192 2017-01-29 21:27:58.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/katakana.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      192 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/katakana.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      206 2017-01-29 21:27:58.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/magicencode.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      206 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/magicencode.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      197 2016-06-24 09:25:19.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/printer.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      197 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_build/html/_sources/api/printer.txt
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.229532 python-escpos-3.0a8/doc/_build/html/_sources/dev/
--rw-r--r--   0 patrick   (1000) patrick   (1000)       32 2016-06-24 09:25:19.000000 python-escpos-3.0a8/doc/_build/html/_sources/dev/changelog.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)       32 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_build/html/_sources/dev/changelog.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)       35 2016-07-23 14:47:59.000000 python-escpos-3.0a8/doc/_build/html/_sources/dev/contributing.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)       35 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_build/html/_sources/dev/contributing.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      876 2017-01-29 21:29:35.000000 python-escpos-3.0a8/doc/_build/html/_sources/index.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      876 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_build/html/_sources/index.txt
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.229532 python-escpos-3.0a8/doc/_build/html/_sources/user/
--rw-r--r--   0 patrick   (1000) patrick   (1000)     1189 2016-08-02 14:32:46.000000 python-escpos-3.0a8/doc/_build/html/_sources/user/barcode.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)     1189 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_build/html/_sources/user/barcode.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)     1813 2016-07-23 14:47:59.000000 python-escpos-3.0a8/doc/_build/html/_sources/user/installation.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)     1813 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_build/html/_sources/user/installation.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      352 2017-01-25 22:35:38.000000 python-escpos-3.0a8/doc/_build/html/_sources/user/methods.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      352 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_build/html/_sources/user/methods.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)     2093 2017-01-25 23:22:37.000000 python-escpos-3.0a8/doc/_build/html/_sources/user/printers.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)     2093 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_build/html/_sources/user/printers.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)     1221 2017-01-06 14:52:20.000000 python-escpos-3.0a8/doc/_build/html/_sources/user/raspi.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)     1221 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_build/html/_sources/user/raspi.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      804 2016-06-24 09:25:19.000000 python-escpos-3.0a8/doc/_build/html/_sources/user/todo.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      804 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_build/html/_sources/user/todo.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)     8819 2019-06-15 22:31:21.000000 python-escpos-3.0a8/doc/_build/html/_sources/user/usage.rst.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)     8760 2017-08-04 14:49:21.000000 python-escpos-3.0a8/doc/_build/html/_sources/user/usage.txt
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.229532 python-escpos-3.0a8/doc/_build/html/_static/
--rw-r--r--   0 patrick   (1000) patrick   (1000)   165662 2016-06-24 09:25:19.000000 python-escpos-3.0a8/doc/_build/html/_static/pyescpos.ico
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.229532 python-escpos-3.0a8/doc/_build/latex/
--rw-r--r--   0 patrick   (1000) patrick   (1000)     2057 2016-03-01 14:30:08.000000 python-escpos-3.0a8/doc/_build/latex/Makefile
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.233532 python-escpos-3.0a8/doc/_build/spelling/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    17525 2020-05-11 21:38:37.000000 python-escpos-3.0a8/doc/_build/spelling/output.txt
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.233532 python-escpos-3.0a8/doc/_static/
--rw-r--r--   0 patrick   (1000) patrick   (1000)        0 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/_static/.gitignore
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.233532 python-escpos-3.0a8/doc/api/
--rw-r--r--   0 patrick   (1000) patrick   (1000)      208 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/api/capabilities.rst
--rw-r--r--   0 patrick   (1000) patrick   (1000)      172 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/api/cli.rst
--rw-r--r--   0 patrick   (1000) patrick   (1000)      196 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/api/codepages.rst
--rw-r--r--   0 patrick   (1000) patrick   (1000)      185 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/api/config.rst
--rw-r--r--   0 patrick   (1000) patrick   (1000)      197 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/api/constants.rst
--rw-r--r--   0 patrick   (1000) patrick   (1000)      187 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/api/escpos.rst
--rw-r--r--   0 patrick   (1000) patrick   (1000)      180 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/api/exceptions.rst
--rw-r--r--   0 patrick   (1000) patrick   (1000)      195 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/api/image.rst
--rw-r--r--   0 patrick   (1000) patrick   (1000)      192 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/api/katakana.rst
--rw-r--r--   0 patrick   (1000) patrick   (1000)      206 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/api/magicencode.rst
--rw-r--r--   0 patrick   (1000) patrick   (1000)      197 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/api/printer.rst
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9478 2020-05-12 16:39:03.000000 python-escpos-3.0a8/doc/conf.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.233532 python-escpos-3.0a8/doc/dev/
--rw-r--r--   0 patrick   (1000) patrick   (1000)       32 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/dev/changelog.rst
--rw-r--r--   0 patrick   (1000) patrick   (1000)       35 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/dev/contributing.rst
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.233532 python-escpos-3.0a8/doc/download/
--rw-r--r--   0 patrick   (1000) patrick   (1000)     2667 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/download/barcode.bin
--rwxr-xr-x   0 patrick   (1000) patrick   (1000)      467 2017-10-08 20:46:33.000000 python-escpos-3.0a8/doc/generate_authors.sh
--rw-r--r--   0 patrick   (1000) patrick   (1000)      876 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/index.rst
--rw-r--r--   0 patrick   (1000) patrick   (1000)     6715 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/make.bat
--rw-r--r--   0 patrick   (1000) patrick   (1000)   165662 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/pyescpos.ico
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      149 2020-05-12 16:39:03.000000 python-escpos-3.0a8/doc/requirements.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       45 2020-05-12 16:39:03.000000 python-escpos-3.0a8/doc/spelling_wordlist.txt
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.237532 python-escpos-3.0a8/doc/user/
--rw-r--r--   0 patrick   (1000) patrick   (1000)     1189 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/user/barcode.rst
--rw-r--r--   0 patrick   (1000) patrick   (1000)     1813 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/user/installation.rst
--rw-r--r--   0 patrick   (1000) patrick   (1000)      352 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/user/methods.rst
--rw-r--r--   0 patrick   (1000) patrick   (1000)     2093 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/user/printers.rst
--rw-r--r--   0 patrick   (1000) patrick   (1000)     1221 2017-05-26 00:39:06.000000 python-escpos-3.0a8/doc/user/raspi.rst
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      246 2020-05-08 23:45:42.000000 python-escpos-3.0a8/doc/user/todo.rst
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8760 2020-05-12 16:39:03.000000 python-escpos-3.0a8/doc/user/usage.rst
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.237532 python-escpos-3.0a8/examples/
--rw-r--r--   0 patrick   (1000) patrick   (1000)      256 2018-08-09 10:47:15.000000 python-escpos-3.0a8/examples/barcodes.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1341 2020-05-10 23:11:05.000000 python-escpos-3.0a8/examples/codepage_tables.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.217532 python-escpos-3.0a8/examples/graphics/
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.241532 python-escpos-3.0a8/examples/graphics/climacons/
--rw-r--r--   0 patrick   (1000) patrick   (1000)     5142 2017-08-04 14:49:21.000000 python-escpos-3.0a8/examples/graphics/climacons/clear-day.png
--rw-r--r--   0 patrick   (1000) patrick   (1000)    21442 2017-08-04 14:49:21.000000 python-escpos-3.0a8/examples/graphics/climacons/clear-night.png
--rw-r--r--   0 patrick   (1000) patrick   (1000)    22565 2017-08-04 14:49:21.000000 python-escpos-3.0a8/examples/graphics/climacons/cloudy.png
--rw-r--r--   0 patrick   (1000) patrick   (1000)    20413 2017-08-04 14:49:21.000000 python-escpos-3.0a8/examples/graphics/climacons/fog.png
--rw-r--r--   0 patrick   (1000) patrick   (1000)     6088 2017-08-04 14:49:21.000000 python-escpos-3.0a8/examples/graphics/climacons/partly-cloudy-day.png
--rw-r--r--   0 patrick   (1000) patrick   (1000)     5106 2017-08-04 14:49:21.000000 python-escpos-3.0a8/examples/graphics/climacons/partly-cloudy-night.png
--rw-r--r--   0 patrick   (1000) patrick   (1000)     4771 2017-08-04 14:49:21.000000 python-escpos-3.0a8/examples/graphics/climacons/rain.png
--rw-r--r--   0 patrick   (1000) patrick   (1000)      693 2017-08-04 14:49:21.000000 python-escpos-3.0a8/examples/graphics/climacons/readme.md
--rw-r--r--   0 patrick   (1000) patrick   (1000)     5091 2017-08-04 14:49:21.000000 python-escpos-3.0a8/examples/graphics/climacons/sleet.png
--rw-r--r--   0 patrick   (1000) patrick   (1000)     5045 2017-08-04 14:49:21.000000 python-escpos-3.0a8/examples/graphics/climacons/snow.png
--rw-r--r--   0 patrick   (1000) patrick   (1000)     3136 2017-08-04 14:49:21.000000 python-escpos-3.0a8/examples/graphics/climacons/wind.png
--rw-r--r--   0 patrick   (1000) patrick   (1000)      324 2018-08-09 10:47:15.000000 python-escpos-3.0a8/examples/qr_code.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      193 2020-05-10 23:11:05.000000 python-escpos-3.0a8/examples/software_barcode.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3639 2020-05-10 23:11:05.000000 python-escpos-3.0a8/examples/weather.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      111 2020-05-08 23:45:42.000000 python-escpos-3.0a8/readthedocs.yml
--rw-r--r--   0 patrick   (1000) patrick   (1000)        4 2016-06-24 09:25:19.000000 python-escpos-3.0a8/requirements.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1900 2020-05-12 17:36:43.249532 python-escpos-3.0a8/setup.cfg
--rwxrwxr-x   0 patrick   (1000) patrick   (1000)     1018 2020-05-10 23:13:51.000000 python-escpos-3.0a8/setup.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.217532 python-escpos-3.0a8/src/
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.241532 python-escpos-3.0a8/src/escpos/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      439 2020-05-10 23:11:05.000000 python-escpos-3.0a8/src/escpos/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    67837 2020-05-08 22:39:57.000000 python-escpos-3.0a8/src/escpos/capabilities.json
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4342 2020-05-12 16:39:03.000000 python-escpos-3.0a8/src/escpos/capabilities.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    17199 2020-05-12 16:39:03.000000 python-escpos-3.0a8/src/escpos/cli.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)      536 2018-08-09 10:47:15.000000 python-escpos-3.0a8/src/escpos/codepages.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3550 2020-05-12 16:39:03.000000 python-escpos-3.0a8/src/escpos/config.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    10686 2020-05-10 23:11:05.000000 python-escpos-3.0a8/src/escpos/constants.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    39019 2020-05-12 16:39:03.000000 python-escpos-3.0a8/src/escpos/escpos.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8165 2020-05-10 23:11:05.000000 python-escpos-3.0a8/src/escpos/exceptions.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3939 2020-05-10 23:11:05.000000 python-escpos-3.0a8/src/escpos/image.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2482 2020-05-10 23:11:05.000000 python-escpos-3.0a8/src/escpos/katakana.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    10814 2020-05-10 23:11:05.000000 python-escpos-3.0a8/src/escpos/magicencode.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    12026 2020-05-10 23:11:05.000000 python-escpos-3.0a8/src/escpos/printer.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)      117 2020-05-12 17:36:43.000000 python-escpos-3.0a8/src/escpos/version.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.241532 python-escpos-3.0a8/src/python_escpos.egg-info/
--rw-r--r--   0 patrick   (1000) patrick   (1000)     5942 2020-05-12 17:36:43.000000 python-escpos-3.0a8/src/python_escpos.egg-info/PKG-INFO
--rw-r--r--   0 patrick   (1000) patrick   (1000)     5157 2020-05-12 17:36:43.000000 python-escpos-3.0a8/src/python_escpos.egg-info/SOURCES.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)        1 2020-05-12 17:36:43.000000 python-escpos-3.0a8/src/python_escpos.egg-info/dependency_links.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)       51 2020-05-12 17:36:43.000000 python-escpos-3.0a8/src/python_escpos.egg-info/entry_points.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2020-05-09 00:44:47.000000 python-escpos-3.0a8/src/python_escpos.egg-info/not-zip-safe
--rw-r--r--   0 patrick   (1000) patrick   (1000)      145 2020-05-12 17:36:43.000000 python-escpos-3.0a8/src/python_escpos.egg-info/requires.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)        7 2020-05-12 17:36:43.000000 python-escpos-3.0a8/src/python_escpos.egg-info/top_level.txt
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.245532 python-escpos-3.0a8/test/
--rw-r--r--   0 patrick   (1000) patrick   (1000)       98 2018-05-15 20:05:11.000000 python-escpos-3.0a8/test/conftest.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2020-05-12 17:36:43.245532 python-escpos-3.0a8/test/resources/
--rw-r--r--   0 patrick   (1000) patrick   (1000)       65 2017-05-26 00:39:06.000000 python-escpos-3.0a8/test/resources/black_transparent.gif
--rw-r--r--   0 patrick   (1000) patrick   (1000)      167 2017-05-26 00:39:06.000000 python-escpos-3.0a8/test/resources/black_transparent.png
--rw-r--r--   0 patrick   (1000) patrick   (1000)       65 2017-05-26 00:39:06.000000 python-escpos-3.0a8/test/resources/black_white.gif
--rw-r--r--   0 patrick   (1000) patrick   (1000)      175 2017-05-26 00:39:06.000000 python-escpos-3.0a8/test/resources/black_white.jpg
--rw-r--r--   0 patrick   (1000) patrick   (1000)      156 2017-05-26 00:39:06.000000 python-escpos-3.0a8/test/resources/black_white.png
--rw-r--r--   0 patrick   (1000) patrick   (1000)       72 2017-05-26 00:39:06.000000 python-escpos-3.0a8/test/resources/canvas_black.gif
--rw-r--r--   0 patrick   (1000) patrick   (1000)      160 2017-05-26 00:39:06.000000 python-escpos-3.0a8/test/resources/canvas_black.jpg
--rw-r--r--   0 patrick   (1000) patrick   (1000)      239 2017-05-26 00:39:06.000000 python-escpos-3.0a8/test/resources/canvas_black.png
--rw-r--r--   0 patrick   (1000) patrick   (1000)       72 2017-05-26 00:39:06.000000 python-escpos-3.0a8/test/resources/canvas_white.gif
--rw-r--r--   0 patrick   (1000) patrick   (1000)      160 2017-05-26 00:39:06.000000 python-escpos-3.0a8/test/resources/canvas_white.jpg
--rw-r--r--   0 patrick   (1000) patrick   (1000)      239 2017-05-26 00:39:06.000000 python-escpos-3.0a8/test/resources/canvas_white.png
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      769 2020-05-12 16:39:03.000000 python-escpos-3.0a8/test/test_abstract_base_class.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2893 2020-05-10 23:11:05.000000 python-escpos-3.0a8/test/test_cli.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1350 2020-05-10 23:11:05.000000 python-escpos-3.0a8/test/test_function_barcode.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      373 2020-05-10 23:11:05.000000 python-escpos-3.0a8/test/test_function_cashdraw.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3925 2020-05-10 23:11:05.000000 python-escpos-3.0a8/test/test_function_check_barcode.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      304 2020-05-10 23:11:05.000000 python-escpos-3.0a8/test/test_function_cut.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)      205 2018-05-15 21:12:34.000000 python-escpos-3.0a8/test/test_function_dummy_clear.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5366 2020-05-10 23:11:05.000000 python-escpos-3.0a8/test/test_function_image.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      973 2020-05-10 23:11:05.000000 python-escpos-3.0a8/test/test_function_linedisplay.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      768 2020-05-10 23:11:05.000000 python-escpos-3.0a8/test/test_function_panel_button.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3164 2020-05-10 23:11:05.000000 python-escpos-3.0a8/test/test_function_qr_native.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      913 2020-05-10 23:11:05.000000 python-escpos-3.0a8/test/test_function_qr_non-native.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8791 2020-05-10 23:11:05.000000 python-escpos-3.0a8/test/test_function_set.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      314 2020-05-10 23:11:05.000000 python-escpos-3.0a8/test/test_function_softbarcode.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1474 2020-05-10 23:11:05.000000 python-escpos-3.0a8/test/test_function_text.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)      732 2017-05-26 00:39:06.000000 python-escpos-3.0a8/test/test_functions.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     2316 2017-05-26 00:39:06.000000 python-escpos-3.0a8/test/test_image.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      504 2020-05-10 23:11:05.000000 python-escpos-3.0a8/test/test_load_module.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3882 2020-05-10 23:11:05.000000 python-escpos-3.0a8/test/test_magicencode.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2158 2020-05-10 23:11:05.000000 python-escpos-3.0a8/test/test_printer_file.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     1025 2017-05-26 00:39:06.000000 python-escpos-3.0a8/test/test_profile.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      797 2020-05-10 23:11:05.000000 python-escpos-3.0a8/test/test_raise_arbitrary_error.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      634 2020-05-10 23:11:05.000000 python-escpos-3.0a8/test/test_with_statement.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      822 2020-05-12 16:39:03.000000 python-escpos-3.0a8/tox.ini
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.898643 python-escpos-3.0a9/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       20 2021-10-30 16:04:41.000000 python-escpos-3.0a9/.coveragerc
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.874643 python-escpos-3.0a9/.github/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      586 2021-10-30 16:04:41.000000 python-escpos-3.0a9/.github/ISSUE_TEMPLATE.md
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      101 2023-05-11 21:13:05.000000 python-escpos-3.0a9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      782 2021-10-30 16:04:41.000000 python-escpos-3.0a9/.github/dependabot.yml
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.878643 python-escpos-3.0a9/.github/workflows/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      229 2023-04-19 20:32:57.000000 python-escpos-3.0a9/.github/workflows/black.yml
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2364 2023-05-11 21:13:05.000000 python-escpos-3.0a9/.github/workflows/codeql-analysis.yml
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1042 2023-05-08 23:09:31.000000 python-escpos-3.0a9/.github/workflows/documentation.yml
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1486 2023-05-08 23:09:31.000000 python-escpos-3.0a9/.github/workflows/pythonpackage.yml
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      499 2023-05-08 23:09:31.000000 python-escpos-3.0a9/.gitignore
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      140 2021-10-30 16:04:41.000000 python-escpos-3.0a9/.gitmodules
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1460 2023-05-08 23:20:51.000000 python-escpos-3.0a9/.mailmap
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.878643 python-escpos-3.0a9/.vscode/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      378 2023-04-19 20:32:57.000000 python-escpos-3.0a9/.vscode/settings.json
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      385 2021-10-30 16:04:41.000000 python-escpos-3.0a9/.vscode/tasks.json
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      664 2023-05-11 20:49:56.000000 python-escpos-3.0a9/AUTHORS
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    11600 2023-05-11 21:38:29.000000 python-escpos-3.0a9/CHANGELOG.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3309 2021-10-30 16:04:41.000000 python-escpos-3.0a9/CONTRIBUTING.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      342 2021-10-30 16:04:41.000000 python-escpos-3.0a9/INSTALL
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1097 2021-10-30 16:04:41.000000 python-escpos-3.0a9/LICENSE
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      332 2021-10-30 16:04:41.000000 python-escpos-3.0a9/MANIFEST.in
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5113 2023-05-11 21:40:14.898643 python-escpos-3.0a9/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3659 2021-10-30 16:04:41.000000 python-escpos-3.0a9/README.rst
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.870643 python-escpos-3.0a9/capabilities-data/
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.878643 python-escpos-3.0a9/capabilities-data/dist/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    91160 2023-05-11 21:04:31.000000 python-escpos-3.0a9/capabilities-data/dist/capabilities.json
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      128 2021-10-30 16:04:41.000000 python-escpos-3.0a9/codecov.yml
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.878643 python-escpos-3.0a9/doc/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        8 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/.gitignore
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6962 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/Makefile
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.874643 python-escpos-3.0a9/doc/_build/
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.874643 python-escpos-3.0a9/doc/_build/html/
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.878643 python-escpos-3.0a9/doc/_build/html/_sources/
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.882643 python-escpos-3.0a9/doc/_build/html/_sources/api/
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      208 2017-01-29 21:25:39.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/capabilities.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      208 2017-05-26 00:39:06.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/capabilities.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      172 2017-01-29 21:27:58.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/cli.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      172 2017-05-26 00:39:06.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/cli.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      196 2017-01-29 21:27:58.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/codepages.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      196 2017-05-26 00:39:06.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/codepages.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      185 2016-06-24 09:25:19.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/config.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      185 2017-05-26 00:39:06.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/config.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      197 2016-06-24 09:25:19.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/constants.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      197 2017-05-26 00:39:06.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/constants.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      187 2016-06-24 09:25:19.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/escpos.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      187 2017-05-26 00:39:06.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/escpos.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      180 2016-06-24 09:25:19.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/exceptions.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      180 2017-05-26 00:39:06.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/exceptions.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      195 2016-07-23 14:47:59.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/image.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      195 2017-05-26 00:39:06.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/image.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      192 2017-01-29 21:27:58.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/katakana.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      192 2017-05-26 00:39:06.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/katakana.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      206 2017-01-29 21:27:58.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/magicencode.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      206 2017-05-26 00:39:06.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/magicencode.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      197 2016-06-24 09:25:19.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/printer.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      197 2017-05-26 00:39:06.000000 python-escpos-3.0a9/doc/_build/html/_sources/api/printer.txt
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.882643 python-escpos-3.0a9/doc/_build/html/_sources/dev/
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)       32 2016-06-24 09:25:19.000000 python-escpos-3.0a9/doc/_build/html/_sources/dev/changelog.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)       32 2017-05-26 00:39:06.000000 python-escpos-3.0a9/doc/_build/html/_sources/dev/changelog.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)       35 2016-07-23 14:47:59.000000 python-escpos-3.0a9/doc/_build/html/_sources/dev/contributing.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)       35 2017-05-26 00:39:06.000000 python-escpos-3.0a9/doc/_build/html/_sources/dev/contributing.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      876 2017-01-29 21:29:35.000000 python-escpos-3.0a9/doc/_build/html/_sources/index.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      876 2017-05-26 00:39:06.000000 python-escpos-3.0a9/doc/_build/html/_sources/index.txt
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.886643 python-escpos-3.0a9/doc/_build/html/_sources/user/
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)     1189 2016-08-02 14:32:46.000000 python-escpos-3.0a9/doc/_build/html/_sources/user/barcode.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)     1189 2017-05-26 00:39:06.000000 python-escpos-3.0a9/doc/_build/html/_sources/user/barcode.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)     1813 2016-07-23 14:47:59.000000 python-escpos-3.0a9/doc/_build/html/_sources/user/installation.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)     1813 2017-05-26 00:39:06.000000 python-escpos-3.0a9/doc/_build/html/_sources/user/installation.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      352 2017-01-25 22:35:38.000000 python-escpos-3.0a9/doc/_build/html/_sources/user/methods.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      352 2017-05-26 00:39:06.000000 python-escpos-3.0a9/doc/_build/html/_sources/user/methods.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)     2093 2017-01-25 23:22:37.000000 python-escpos-3.0a9/doc/_build/html/_sources/user/printers.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)     2093 2017-05-26 00:39:06.000000 python-escpos-3.0a9/doc/_build/html/_sources/user/printers.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)     1221 2017-01-06 14:52:20.000000 python-escpos-3.0a9/doc/_build/html/_sources/user/raspi.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)     1221 2017-05-26 00:39:06.000000 python-escpos-3.0a9/doc/_build/html/_sources/user/raspi.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      246 2020-05-08 23:45:42.000000 python-escpos-3.0a9/doc/_build/html/_sources/user/todo.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      804 2017-05-26 00:39:06.000000 python-escpos-3.0a9/doc/_build/html/_sources/user/todo.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)     9600 2020-10-04 12:26:29.000000 python-escpos-3.0a9/doc/_build/html/_sources/user/usage.rst.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)     8760 2017-08-04 14:49:21.000000 python-escpos-3.0a9/doc/_build/html/_sources/user/usage.txt
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.886643 python-escpos-3.0a9/doc/_build/html/_static/
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)   165662 2016-06-24 09:25:19.000000 python-escpos-3.0a9/doc/_build/html/_static/pyescpos.ico
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.886643 python-escpos-3.0a9/doc/_build/latex/
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)     2057 2016-03-01 14:30:08.000000 python-escpos-3.0a9/doc/_build/latex/Makefile
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.886643 python-escpos-3.0a9/doc/_build/spelling/
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)    17525 2020-05-11 21:38:37.000000 python-escpos-3.0a9/doc/_build/spelling/output.txt
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.886643 python-escpos-3.0a9/doc/_static/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/_static/.gitignore
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.886643 python-escpos-3.0a9/doc/api/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      208 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/api/capabilities.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      172 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/api/cli.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      196 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/api/codepages.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      185 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/api/config.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      197 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/api/constants.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      187 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/api/escpos.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      180 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/api/exceptions.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      195 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/api/image.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      192 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/api/katakana.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      206 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/api/magicencode.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      197 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/api/printer.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9489 2023-04-19 20:10:20.000000 python-escpos-3.0a9/doc/conf.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.886643 python-escpos-3.0a9/doc/dev/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       32 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/dev/changelog.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       35 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/dev/contributing.rst
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.886643 python-escpos-3.0a9/doc/download/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2667 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/download/barcode.bin
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      607 2020-09-28 17:40:15.000000 python-escpos-3.0a9/doc/generate_authors.sh
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      876 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/index.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6716 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/make.bat
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)   165662 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/pyescpos.ico
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      172 2023-05-11 21:13:05.000000 python-escpos-3.0a9/doc/requirements.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       45 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/spelling_wordlist.txt
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.890643 python-escpos-3.0a9/doc/user/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1189 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/user/barcode.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1813 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/user/installation.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      352 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/user/methods.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2892 2023-05-08 23:09:31.000000 python-escpos-3.0a9/doc/user/printers.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1221 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/user/raspi.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      246 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/user/todo.rst
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9602 2021-10-30 16:04:41.000000 python-escpos-3.0a9/doc/user/usage.rst
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.890643 python-escpos-3.0a9/examples/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      256 2021-10-30 16:26:19.000000 python-escpos-3.0a9/examples/barcodes.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1374 2021-10-30 16:26:19.000000 python-escpos-3.0a9/examples/codepage_tables.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.874643 python-escpos-3.0a9/examples/graphics/
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.890643 python-escpos-3.0a9/examples/graphics/climacons/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5142 2021-10-30 16:04:41.000000 python-escpos-3.0a9/examples/graphics/climacons/clear-day.png
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    21442 2021-10-30 16:04:41.000000 python-escpos-3.0a9/examples/graphics/climacons/clear-night.png
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    22565 2021-10-30 16:04:41.000000 python-escpos-3.0a9/examples/graphics/climacons/cloudy.png
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    20413 2021-10-30 16:04:41.000000 python-escpos-3.0a9/examples/graphics/climacons/fog.png
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6088 2021-10-30 16:04:41.000000 python-escpos-3.0a9/examples/graphics/climacons/partly-cloudy-day.png
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5106 2021-10-30 16:04:41.000000 python-escpos-3.0a9/examples/graphics/climacons/partly-cloudy-night.png
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4771 2021-10-30 16:04:41.000000 python-escpos-3.0a9/examples/graphics/climacons/rain.png
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      696 2021-10-30 16:04:41.000000 python-escpos-3.0a9/examples/graphics/climacons/readme.md
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5091 2021-10-30 16:04:41.000000 python-escpos-3.0a9/examples/graphics/climacons/sleet.png
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5045 2021-10-30 16:04:41.000000 python-escpos-3.0a9/examples/graphics/climacons/snow.png
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3136 2021-10-30 16:04:41.000000 python-escpos-3.0a9/examples/graphics/climacons/wind.png
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      324 2021-10-30 16:26:19.000000 python-escpos-3.0a9/examples/qr_code.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      193 2021-10-30 16:26:19.000000 python-escpos-3.0a9/examples/software_barcode.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3603 2023-04-19 20:10:20.000000 python-escpos-3.0a9/examples/weather.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       51 2021-10-30 16:31:54.000000 python-escpos-3.0a9/pyproject.toml
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      111 2021-10-30 16:04:41.000000 python-escpos-3.0a9/readthedocs.yml
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        4 2021-10-30 16:04:41.000000 python-escpos-3.0a9/requirements.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1928 2023-05-11 21:40:14.898643 python-escpos-3.0a9/setup.cfg
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)     1018 2020-05-10 23:13:51.000000 python-escpos-3.0a9/setup.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.874643 python-escpos-3.0a9/src/
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.894643 python-escpos-3.0a9/src/escpos/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      438 2021-10-30 16:26:19.000000 python-escpos-3.0a9/src/escpos/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    91160 2023-05-11 21:04:31.000000 python-escpos-3.0a9/src/escpos/capabilities.json
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4381 2021-10-30 16:26:19.000000 python-escpos-3.0a9/src/escpos/capabilities.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    17207 2021-10-30 16:26:19.000000 python-escpos-3.0a9/src/escpos/cli.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      536 2021-10-30 16:26:19.000000 python-escpos-3.0a9/src/escpos/codepages.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3566 2021-10-30 16:26:19.000000 python-escpos-3.0a9/src/escpos/config.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9998 2023-05-11 20:49:56.000000 python-escpos-3.0a9/src/escpos/constants.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    41467 2023-05-11 20:51:35.000000 python-escpos-3.0a9/src/escpos/escpos.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8231 2021-10-30 16:26:19.000000 python-escpos-3.0a9/src/escpos/exceptions.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3942 2021-10-30 16:26:19.000000 python-escpos-3.0a9/src/escpos/image.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2481 2021-10-30 16:35:12.000000 python-escpos-3.0a9/src/escpos/katakana.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    11026 2023-05-08 23:20:51.000000 python-escpos-3.0a9/src/escpos/magicencode.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    17942 2023-05-08 23:09:31.000000 python-escpos-3.0a9/src/escpos/printer.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      117 2023-05-11 21:40:14.000000 python-escpos-3.0a9/src/escpos/version.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.894643 python-escpos-3.0a9/src/python_escpos.egg-info/
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)     5113 2023-05-11 21:40:14.000000 python-escpos-3.0a9/src/python_escpos.egg-info/PKG-INFO
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)     5314 2023-05-11 21:40:14.000000 python-escpos-3.0a9/src/python_escpos.egg-info/SOURCES.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)        1 2023-05-11 21:40:14.000000 python-escpos-3.0a9/src/python_escpos.egg-info/dependency_links.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)       51 2023-05-11 21:40:14.000000 python-escpos-3.0a9/src/python_escpos.egg-info/entry_points.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)        1 2020-05-09 00:44:47.000000 python-escpos-3.0a9/src/python_escpos.egg-info/not-zip-safe
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)      129 2023-05-11 21:40:14.000000 python-escpos-3.0a9/src/python_escpos.egg-info/requires.txt
+-rwxrwxrwx   0 patrick   (1000) patrick   (1000)        7 2023-05-11 21:40:14.000000 python-escpos-3.0a9/src/python_escpos.egg-info/top_level.txt
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.894643 python-escpos-3.0a9/test/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       98 2021-10-30 16:04:41.000000 python-escpos-3.0a9/test/conftest.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-11 21:40:14.898643 python-escpos-3.0a9/test/resources/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       65 2021-10-30 16:04:41.000000 python-escpos-3.0a9/test/resources/black_transparent.gif
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      167 2021-10-30 16:04:41.000000 python-escpos-3.0a9/test/resources/black_transparent.png
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       65 2021-10-30 16:04:41.000000 python-escpos-3.0a9/test/resources/black_white.gif
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      175 2021-10-30 16:04:41.000000 python-escpos-3.0a9/test/resources/black_white.jpg
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      156 2021-10-30 16:04:41.000000 python-escpos-3.0a9/test/resources/black_white.png
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       72 2021-10-30 16:04:41.000000 python-escpos-3.0a9/test/resources/canvas_black.gif
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      160 2021-10-30 16:04:41.000000 python-escpos-3.0a9/test/resources/canvas_black.jpg
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      239 2021-10-30 16:04:41.000000 python-escpos-3.0a9/test/resources/canvas_black.png
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       72 2021-10-30 16:04:41.000000 python-escpos-3.0a9/test/resources/canvas_white.gif
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      160 2021-10-30 16:04:41.000000 python-escpos-3.0a9/test/resources/canvas_white.jpg
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      239 2021-10-30 16:04:41.000000 python-escpos-3.0a9/test/resources/canvas_white.png
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      767 2021-10-30 16:26:19.000000 python-escpos-3.0a9/test/test_abstract_base_class.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2835 2021-10-30 16:26:19.000000 python-escpos-3.0a9/test/test_cli.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1439 2021-10-30 16:26:19.000000 python-escpos-3.0a9/test/test_function_barcode.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      372 2021-10-30 16:26:19.000000 python-escpos-3.0a9/test/test_function_cashdraw.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4279 2021-10-30 16:26:19.000000 python-escpos-3.0a9/test/test_function_check_barcode.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      302 2021-10-30 16:26:19.000000 python-escpos-3.0a9/test/test_function_cut.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      205 2021-10-30 16:26:19.000000 python-escpos-3.0a9/test/test_function_dummy_clear.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5452 2021-10-30 16:26:19.000000 python-escpos-3.0a9/test/test_function_image.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      971 2021-10-30 16:26:19.000000 python-escpos-3.0a9/test/test_function_linedisplay.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      766 2021-10-30 16:26:19.000000 python-escpos-3.0a9/test/test_function_panel_button.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3222 2021-10-30 16:26:19.000000 python-escpos-3.0a9/test/test_function_qr_native.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      913 2021-10-30 16:26:19.000000 python-escpos-3.0a9/test/test_function_qr_non-native.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8900 2023-04-19 20:32:57.000000 python-escpos-3.0a9/test/test_function_set.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      569 2021-10-30 16:26:19.000000 python-escpos-3.0a9/test/test_function_softbarcode.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1480 2021-10-30 16:26:19.000000 python-escpos-3.0a9/test/test_function_text.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      732 2021-10-30 16:26:19.000000 python-escpos-3.0a9/test/test_functions.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2374 2021-10-30 16:26:19.000000 python-escpos-3.0a9/test/test_image.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      504 2021-10-30 16:26:19.000000 python-escpos-3.0a9/test/test_load_module.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3920 2023-04-19 20:10:20.000000 python-escpos-3.0a9/test/test_magicencode.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2158 2021-10-30 16:26:19.000000 python-escpos-3.0a9/test/test_printer_file.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      596 2021-10-30 16:26:20.000000 python-escpos-3.0a9/test/test_printer_network.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1015 2021-10-30 16:26:20.000000 python-escpos-3.0a9/test/test_profile.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      797 2021-10-30 16:04:41.000000 python-escpos-3.0a9/test/test_raise_arbitrary_error.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      630 2021-10-30 16:26:20.000000 python-escpos-3.0a9/test/test_with_statement.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      911 2023-04-19 20:32:57.000000 python-escpos-3.0a9/tox.ini
```

### Comparing `python-escpos-3.0a8/.github/ISSUE_TEMPLATE.md` & `python-escpos-3.0a9/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/.github/workflows/pythonpackage.yml` & `python-escpos-3.0a9/.github/workflows/pythonpackage.yml`

 * *Files 11% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.5, 3.6, 3.7, 3.8]
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
       with:
         submodules: 'recursive'
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v4.6.0
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install flake8 pytest tox tox-gh-actions
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
```

### Comparing `python-escpos-3.0a8/AUTHORS` & `python-escpos-3.0a9/AUTHORS`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Ahmed Tahri
 akeonly
+Alejandro Hernández
 Alexander Bougakov
 Alex Debiasio
 Asuki Kono
 belono
+B. Howell
 Brian
 Christoph Heuel
 Cody (Quantified Code Bot)
 csoft2k
 Curtis // mashedkeyboard
 Davis Goglin
 Dean Rispin
+dependabot[bot]
 Dmytro Katyukha
 Gerard Marull-Paretas
 Hark
 Joel Lehtonen
 Justin Vieira
 kennedy
 Kristi
 ldos
 Lucy Linder
 Manuel F Martinez
+Mathieu Poussin
 Maximilian Wagenbach
 Michael Billington
 Michael Elsdörfer
 mrwunderbar666
 Nathan Bookham
 Omer Akram
 Patrick Kanzler
@@ -37,7 +41,8 @@
 Sam Cheng
 Sergio Pulgarin
 Stephan Sokolow
 Thijs Triemstra
 Thomas van den Berg
 Yaisel Hurtado
 ysuolmai
+白月秋见心
```

### Comparing `python-escpos-3.0a8/CHANGELOG.rst` & `python-escpos-3.0a9/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,32 @@
 *********
 Changelog
 *********
+2023-05-11 - Version 3.0a9 - "Pride Comes Before A Fall"
+--------------------------------------------------------
+This release is the 10th alpha release of the new version 3.0.
+After three years hiatus, a new release is in work in order to
+finally get a version 3.0 out.
+
+changes
+^^^^^^^
+- Include support for CUPS based printer interfaces
+- Move the build toolchain to GitHub
+
+contributors
+^^^^^^^^^^^^
+- belono
+- brendanhowell
+- AlexandroJaez
+- NullYing
+- kedare
+- Foaly
+- patkan
+- and others
+
 2020-05-12 - Version 3.0a8 - "Only Slightly Bent"
 -------------------------------------------------
 This release is the ninth alpha release of the new version 3.0.
 Please be aware that the API is subject to change until v3.0 is
 released.
 
 This release drops support for Python 2, requiring at least
```

### Comparing `python-escpos-3.0a8/CONTRIBUTING.rst` & `python-escpos-3.0a9/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 This project is open to any kind of contribution. You can help with improving the documentation, adding fixes to the
 code, providing test cases in code or as a description or just spreading the word. Please feel free to create an
 issue or pull request.
 In order to reduce the amount of work for everyone please try to adhere to good practice.
 
 The pull requests and issues will be prefilled with templates. Please fill in your information where applicable.
 
-This project uses `semantic versioning <http://semver.org/>`_ and tries to adhere to the proposed rules as
+This project uses `semantic versioning <https://semver.org/>`_ and tries to adhere to the proposed rules as
 well as possible.
 
 Author-list
 -----------
 
 This project keeps a list of authors. This can be auto-generated by calling `./doc/generate-authors.sh`.
 When contributing the first time, please include a commit with the output of this script in place.
@@ -58,12 +58,12 @@
 Try to write tests whenever possible. Our goal for the future is 100% coverage.
 We are currently using `nose` but might change in the future.
 You can copy the structure from other testcases. Please remember to adapt the docstrings.
 
 Further reading
 ^^^^^^^^^^^^^^^
 For further best practices and hints on contributing please see the
-`contribution-guide <http://www.contribution-guide.org/>`_. Should there be any contradictions between this guide
+`contribution-guide <https://www.contribution-guide.org/>`_. Should there be any contradictions between this guide
 and the linked one, please stick to this text.
 Aside from that feel free to create an issue or write an email if anything is unclear.
 
 Thank you for your contribution!
```

### Comparing `python-escpos-3.0a8/LICENSE` & `python-escpos-3.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/PKG-INFO` & `python-escpos-3.0a9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,141 +1,143 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: python-escpos
-Version: 3.0a8
+Version: 3.0a9
 Summary: Python library to manipulate ESC/POS Printers
 Home-page: https://github.com/python-escpos/python-escpos
 Author: Manuel F Martinez and others
 Author-email: dev@pkanzler.de
 Maintainer: Patrick Kanzler
 Maintainer-email: dev@pkanzler.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/python-escpos/python-escpos/issues
 Project-URL: Documentation, https://python-escpos.readthedocs.io/en/latest/
 Project-URL: Release Notes, https://github.com/python-escpos/python-escpos/releases
-Description: #############################################################
-        python-escpos - Python library to manipulate ESC/POS Printers
-        #############################################################
-        
-        .. image:: https://travis-ci.org/python-escpos/python-escpos.svg?branch=master
-            :target: https://travis-ci.org/python-escpos/python-escpos
-            :alt: Continous Integration
-        
-        .. image:: https://codecov.io/github/python-escpos/python-escpos/coverage.svg?branch=master
-            :target: https://codecov.io/github/python-escpos/python-escpos?branch=master
-            :alt: Code Coverage
-        
-        .. image:: https://readthedocs.org/projects/python-escpos/badge/?version=latest
-            :target: http://python-escpos.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        
-        Description
-        -----------
-        
-        Python ESC/POS is a library which lets the user have access to all those printers handled
-        by ESC/POS commands, as defined by Epson, from a Python application.
-        
-        The library tries to implement the functions provided by the ESC/POS-commandset and supports sending text, images,
-        barcodes and qr-codes to the printer.
-        
-        Text can be aligned/justified and fonts can be changed by size, type and weight.
-        
-        Also, this module handles some hardware functionalities like cutting paper, control characters, printer reset
-        and similar functions.
-        
-        Since supported commands differ from printer to printer the software tries to automatically apply the right
-        settings for the printer that you set. These settings are handled by
-        `escpos-printer-db <https://github.com/receipt-print-hq/escpos-printer-db>`_ which is also used in
-        `escpos-php <https://github.com/mike42/escpos-php>`_.
-        
-        Dependencies
-        ------------
-        
-        This library makes use of:
-        
-        * `pyusb <https://github.com/walac/pyusb>`_ for USB-printers
-        * `Pillow <https://github.com/python-pillow/Pillow>`_ for image printing
-        * `qrcode <https://github.com/lincolnloop/python-qrcode>`_ for the generation of QR-codes
-        * `pyserial <https://github.com/pyserial/pyserial>`_ for serial printers
-        * `python-barcode <https://github.com/WhyNotHugo/python-barcode>`_ for the generation of barcodes
-        
-        Documentation and Usage
-        -----------------------
-        
-        The basic usage is:
-        
-        .. code:: python
-        
-            from escpos.printer import Usb
-        
-            """ Seiko Epson Corp. Receipt Printer (EPSON TM-T88III) """
-            p = Usb(0x04b8, 0x0202, 0, profile="TM-T88III")
-            p.text("Hello World\n")
-            p.image("logo.gif")
-            p.barcode('1324354657687', 'EAN13', 64, 2, '', '')
-            p.cut()
-        
-        
-        Another example based on the Network printer class:
-        
-        .. code:: python
-        
-            from escpos.printer import Network
-            
-            kitchen = Network("192.168.1.100") #Printer IP Address
-            kitchen.text("Hello World\n")
-            kitchen.barcode('1324354657687', 'EAN13', 64, 2, '', '')
-            kitchen.cut()
-            
-        Another example based on the Serial printer class:
-        
-        .. code:: python
-        
-            from escpos.printer import Serial
-            
-            """ 9600 Baud, 8N1, Flow Control Enabled """
-            p = Serial(devfile='/dev/tty.usbserial',
-                       baudrate=9600,
-                       bytesize=8,
-                       parity='N',
-                       stopbits=1,
-                       timeout=1.00,
-                       dsrdtr=True)
-        
-            p.text("Hello World\n")
-            p.qr("You can readme from your smartphone")
-            p.cut()
-        
-        
-        The full project-documentation is available on `Read the Docs <https://python-escpos.readthedocs.io>`_.
-        
-        Contributing
-        ------------
-        
-        This project is open for any contribution! Please see `CONTRIBUTING.rst <http://python-escpos.readthedocs.io/en/latest/dev/contributing.html>`_ for more information.
-        
-        
-        Disclaimer
-        ----------
-        
-        None of the vendors cited in this project agree or endorse any of the patterns or implementations.
-        Its names are used only to maintain context.
-        
-        
-        
 Keywords: ESC/POS,thermoprinter,voucher printer,printing,receipt
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Office/Business :: Financial :: Point-Of-Sale
-Requires-Python: >=3.5
+Requires-Python: >=3.6
+License-File: LICENSE
+
+#############################################################
+python-escpos - Python library to manipulate ESC/POS Printers
+#############################################################
+
+.. image:: https://travis-ci.org/python-escpos/python-escpos.svg?branch=master
+    :target: https://travis-ci.org/python-escpos/python-escpos
+    :alt: Continous Integration
+
+.. image:: https://codecov.io/github/python-escpos/python-escpos/coverage.svg?branch=master
+    :target: https://codecov.io/github/python-escpos/python-escpos?branch=master
+    :alt: Code Coverage
+
+.. image:: https://readthedocs.org/projects/python-escpos/badge/?version=latest
+    :target: https://python-escpos.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+
+Description
+-----------
+
+Python ESC/POS is a library which lets the user have access to all those printers handled
+by ESC/POS commands, as defined by Epson, from a Python application.
+
+The library tries to implement the functions provided by the ESC/POS-commandset and supports sending text, images,
+barcodes and qr-codes to the printer.
+
+Text can be aligned/justified and fonts can be changed by size, type and weight.
+
+Also, this module handles some hardware functionalities like cutting paper, control characters, printer reset
+and similar functions.
+
+Since supported commands differ from printer to printer the software tries to automatically apply the right
+settings for the printer that you set. These settings are handled by
+`escpos-printer-db <https://github.com/receipt-print-hq/escpos-printer-db>`_ which is also used in
+`escpos-php <https://github.com/mike42/escpos-php>`_.
+
+Dependencies
+------------
+
+This library makes use of:
+
+* `pyusb <https://github.com/walac/pyusb>`_ for USB-printers
+* `Pillow <https://github.com/python-pillow/Pillow>`_ for image printing
+* `qrcode <https://github.com/lincolnloop/python-qrcode>`_ for the generation of QR-codes
+* `pyserial <https://github.com/pyserial/pyserial>`_ for serial printers
+* `python-barcode <https://github.com/WhyNotHugo/python-barcode>`_ for the generation of barcodes
+
+Documentation and Usage
+-----------------------
+
+The basic usage is:
+
+.. code:: python
+
+    from escpos.printer import Usb
+
+    """ Seiko Epson Corp. Receipt Printer (EPSON TM-T88III) """
+    p = Usb(0x04b8, 0x0202, 0, profile="TM-T88III")
+    p.text("Hello World\n")
+    p.image("logo.gif")
+    p.barcode('1324354657687', 'EAN13', 64, 2, '', '')
+    p.cut()
+
+
+Another example based on the Network printer class:
+
+.. code:: python
+
+    from escpos.printer import Network
+
+    kitchen = Network("192.168.1.100") #Printer IP Address
+    kitchen.text("Hello World\n")
+    kitchen.barcode('1324354657687', 'EAN13', 64, 2, '', '')
+    kitchen.cut()
+
+Another example based on the Serial printer class:
+
+.. code:: python
+
+    from escpos.printer import Serial
+
+    """ 9600 Baud, 8N1, Flow Control Enabled """
+    p = Serial(devfile='/dev/tty.usbserial',
+               baudrate=9600,
+               bytesize=8,
+               parity='N',
+               stopbits=1,
+               timeout=1.00,
+               dsrdtr=True)
+
+    p.text("Hello World\n")
+    p.qr("You can readme from your smartphone")
+    p.cut()
+
+
+The full project-documentation is available on `Read the Docs <https://python-escpos.readthedocs.io>`_.
+
+Contributing
+------------
+
+This project is open for any contribution! Please see `CONTRIBUTING.rst <https://python-escpos.readthedocs.io/en/latest/dev/contributing.html>`_ for more information.
+
+
+Disclaimer
+----------
+
+None of the vendors cited in this project agree or endorse any of the patterns or implementations.
+Its names are used only to maintain context.
+
+
```

### Comparing `python-escpos-3.0a8/README.rst` & `python-escpos-3.0a9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     :alt: Continous Integration
 
 .. image:: https://codecov.io/github/python-escpos/python-escpos/coverage.svg?branch=master
     :target: https://codecov.io/github/python-escpos/python-escpos?branch=master
     :alt: Code Coverage
 
 .. image:: https://readthedocs.org/projects/python-escpos/badge/?version=latest
-    :target: http://python-escpos.readthedocs.io/en/latest/?badge=latest
+    :target: https://python-escpos.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 
 Description
 -----------
 
 Python ESC/POS is a library which lets the user have access to all those printers handled
@@ -63,26 +63,26 @@
 
 
 Another example based on the Network printer class:
 
 .. code:: python
 
     from escpos.printer import Network
-    
+
     kitchen = Network("192.168.1.100") #Printer IP Address
     kitchen.text("Hello World\n")
     kitchen.barcode('1324354657687', 'EAN13', 64, 2, '', '')
     kitchen.cut()
-    
+
 Another example based on the Serial printer class:
 
 .. code:: python
 
     from escpos.printer import Serial
-    
+
     """ 9600 Baud, 8N1, Flow Control Enabled """
     p = Serial(devfile='/dev/tty.usbserial',
                baudrate=9600,
                bytesize=8,
                parity='N',
                stopbits=1,
                timeout=1.00,
@@ -94,17 +94,15 @@
 
 
 The full project-documentation is available on `Read the Docs <https://python-escpos.readthedocs.io>`_.
 
 Contributing
 ------------
 
-This project is open for any contribution! Please see `CONTRIBUTING.rst <http://python-escpos.readthedocs.io/en/latest/dev/contributing.html>`_ for more information.
+This project is open for any contribution! Please see `CONTRIBUTING.rst <https://python-escpos.readthedocs.io/en/latest/dev/contributing.html>`_ for more information.
 
 
 Disclaimer
 ----------
 
 None of the vendors cited in this project agree or endorse any of the patterns or implementations.
 Its names are used only to maintain context.
-
-
```

### Comparing `python-escpos-3.0a8/capabilities-data/dist/capabilities.json` & `python-escpos-3.0a9/capabilities-data/dist/capabilities.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.927627418093268%*

 * *Differences: {"'encodings'": "{'KATAKANA': OrderedDict([('data', ['▁▂▃▄▅▆▇█▏▎▍▌▋▊▉┼', '┴┬┤├¯─│▕┌┐└┘╭╮╰╯', ' "*

 * *                "｡｢｣､･ｦｧｨｩｪｫｬｭｮｯ', 'ｰｱｲｳｴｵｶｷｸｹｺｻｼｽｾｿ', 'ﾀﾁﾂﾃﾄﾅﾆﾇﾈﾉﾊﾋﾌﾍﾎﾏ', 'ﾐﾑﾒﾓﾔﾕﾖﾗﾘﾙﾚﾛﾜﾝﾞﾟ', "*

 * *                "'═╞╪╡◢◣◥◤♠♥♦♣●○╱╲', '╳円年月日時分秒〒市区町村人▓\\xa0']), ('name', 'Katakana (codepage "*

 * *                "1)')])}",*

 * * "'profiles'": "{'P822D': {'codePages': {'1': 'KATAKANA'}}, 'RP326': {'codePages': {'1': "*

 * *               "'KATAKANA'}}, 'TM-T88II': {'codePages': {'19': 'Unknown', '6': 'Unknown', '7': "*

 * *          […]*

```diff
@@ -286,14 +286,27 @@
             "python_encode": "iso8859_8"
         },
         "ISO_8859-9": {
             "iconv": "ISO_8859-9",
             "name": "ISO_8859-9",
             "python_encode": "iso8859_9"
         },
+        "KATAKANA": {
+            "data": [
+                "\u2581\u2582\u2583\u2584\u2585\u2586\u2587\u2588\u258f\u258e\u258d\u258c\u258b\u258a\u2589\u253c",
+                "\u2534\u252c\u2524\u251c\u00af\u2500\u2502\u2595\u250c\u2510\u2514\u2518\u256d\u256e\u2570\u256f",
+                " \uff61\uff62\uff63\uff64\uff65\uff66\uff67\uff68\uff69\uff6a\uff6b\uff6c\uff6d\uff6e\uff6f",
+                "\uff70\uff71\uff72\uff73\uff74\uff75\uff76\uff77\uff78\uff79\uff7a\uff7b\uff7c\uff7d\uff7e\uff7f",
+                "\uff80\uff81\uff82\uff83\uff84\uff85\uff86\uff87\uff88\uff89\uff8a\uff8b\uff8c\uff8d\uff8e\uff8f",
+                "\uff90\uff91\uff92\uff93\uff94\uff95\uff96\uff97\uff98\uff99\uff9a\uff9b\uff9c\uff9d\uff9e\uff9f",
+                "\u2550\u255e\u256a\u2561\u25e2\u25e3\u25e5\u25e4\u2660\u2665\u2666\u2663\u25cf\u25cb\u2571\u2572",
+                "\u2573\u5186\u5e74\u6708\u65e5\u6642\u5206\u79d2\u3012\u5e02\u533a\u753a\u6751\u4eba\u2593\u00a0"
+            ],
+            "name": "Katakana (codepage 1)"
+        },
         "OXHOO-EUROPEAN": {
             "data": [
                 "\u00c7\u00fc\u00e9\u00e2\u00e4\u00e0\u00e5\u00e7\u00ea\u00eb\u00e8\u00ef\u00ee\u00ec\u00c4\u00c5",
                 "\u00c9\u00e6\u00c6\u00f4\u00f6\u00f2\u00fb\u00f9\u00ff\u00d6\u00dc\u00f1\u00d1\u00aa\u00ba\u00bf",
                 "\u00e1\u00ed\u00f3\u00fa\u00a2\u00a3\u00a5\u20a7\u0192\u00a1\u00c3\u00e3\u00d5\u00f5\u00d8\u00f8",
                 "\u00b7\u00a8\u00b0`\u00b4\u00bd\u00bc\u00d7\u00f7\u2264\u2265\u00ab\u00bb\u2260\u221a\u00af",
                 "\u2320\u2321\u221e\u25e4\u21b5\u2191\u2193\u2192\u2190\u250c\u2510\u2514\u2518\u2022\u00ae\u00a9",
@@ -441,14 +454,126 @@
                     "pixels": 640
                 }
             },
             "name": "CT-S651",
             "notes": "Citizen CT-S651 profile. This is a two-color thermal printer, supporting paper sizes from 58mm up to 83mm\n",
             "vendor": "Citizen"
         },
+        "KR-306": {
+            "codePages": {
+                "0": "CP437",
+                "1": "KATAKANA",
+                "10": "Unknown",
+                "11": "CP1252",
+                "12": "CP866",
+                "13": "CP852",
+                "14": "CP858",
+                "15": "Unknown",
+                "16": "Unknown",
+                "17": "Unknown",
+                "18": "Unknown",
+                "19": "CP747",
+                "2": "CP850",
+                "20": "Unknown",
+                "21": "Unknown",
+                "22": "Unknown",
+                "23": "CP864",
+                "24": "Unknown",
+                "25": "Unknown",
+                "26": "Unknown",
+                "27": "CP1255",
+                "28": "CP437",
+                "29": "KATAKANA",
+                "3": "CP860",
+                "30": "CP437",
+                "31": "CP858",
+                "32": "CP852",
+                "33": "CP860",
+                "34": "CP861",
+                "35": "CP863",
+                "36": "CP865",
+                "37": "CP866",
+                "38": "CP855",
+                "39": "CP857",
+                "4": "CP863",
+                "40": "CP862",
+                "41": "CP864",
+                "42": "CP737",
+                "43": "CP851",
+                "44": "CP869",
+                "45": "CP928",
+                "46": "CP772",
+                "47": "CP774",
+                "48": "CP874",
+                "49": "CP1252",
+                "5": "CP865",
+                "50": "CP1250",
+                "51": "CP1251",
+                "52": "CP3840",
+                "53": "CP3841",
+                "54": "CP3843",
+                "55": "CP3844",
+                "56": "CP3845",
+                "57": "CP3846",
+                "58": "CP3847",
+                "59": "CP3848",
+                "6": "Unknown",
+                "60": "CP1001",
+                "61": "CP2001",
+                "62": "CP3001",
+                "63": "CP3002",
+                "64": "CP3011",
+                "65": "CP3012",
+                "66": "CP3021",
+                "67": "CP3041",
+                "68": "CP852",
+                "69": "Unknown",
+                "7": "Unknown",
+                "70": "CP1256",
+                "8": "Unknown",
+                "9": "Unknown"
+            },
+            "colors": {
+                "0": "black"
+            },
+            "features": {
+                "barcodeA": true,
+                "barcodeB": true,
+                "bitImageColumn": true,
+                "bitImageRaster": true,
+                "graphics": false,
+                "highDensity": true,
+                "paperFullCut": true,
+                "paperPartCut": true,
+                "pdf417Code": true,
+                "pulseBel": false,
+                "pulseStandard": true,
+                "qrCode": true,
+                "starCommands": false
+            },
+            "fonts": {
+                "0": {
+                    "columns": 48,
+                    "name": "Font A"
+                },
+                "1": {
+                    "columns": 64,
+                    "name": "Font B"
+                }
+            },
+            "media": {
+                "width": {
+                    "mm": 72,
+                    "pixels": 576
+                }
+            },
+            "name": "KR-306",
+            "notes": "Kefar KR-306 printer with 200mm/s speed\n",
+            "vendor": "Kefar"
+        },
         "NT-5890K": {
             "codePages": {
                 "0": "CP437",
                 "1": "CP932",
                 "10": "Unknown",
                 "16": "CP1252",
                 "17": "CP866",
@@ -667,15 +792,15 @@
             "name": "OCD-300 Customer Display",
             "notes": "This is a two-line, ESC/POS-aware customer display from Aures. It has some graphics support via vendor-provided tools, but is otherwise text-only.\n",
             "vendor": "Aures"
         },
         "P822D": {
             "codePages": {
                 "0": "CP437",
-                "1": "Unknown",
+                "1": "KATAKANA",
                 "10": "Unknown",
                 "16": "CP1252",
                 "17": "CP866",
                 "18": "CP852",
                 "19": "CP858",
                 "2": "CP850",
                 "20": "Unknown",
@@ -885,18 +1010,138 @@
                     "pixels": 384
                 }
             },
             "name": "POS5890 Series",
             "notes": "POS-5890 thermal printer series, also marketed under various other names.\n",
             "vendor": "Zjiang"
         },
+        "RP-F10-58mm": {
+            "codePages": {
+                "0": "CP437",
+                "1": "KATAKANA",
+                "13": "CP857",
+                "14": "CP737",
+                "16": "CP1252",
+                "17": "CP866",
+                "18": "CP852",
+                "19": "CP858",
+                "2": "CP850",
+                "255": "Unknown",
+                "3": "CP860",
+                "34": "CP855",
+                "37": "CP864",
+                "4": "CP863",
+                "45": "CP1250",
+                "46": "CP1251",
+                "47": "CP1253",
+                "48": "CP1254",
+                "5": "CP865"
+            },
+            "colors": {
+                "0": "black"
+            },
+            "features": {
+                "barcodeA": true,
+                "barcodeB": true,
+                "bitImageColumn": true,
+                "bitImageRaster": true,
+                "graphics": true,
+                "highDensity": true,
+                "paperFullCut": true,
+                "paperPartCut": true,
+                "pdf417Code": true,
+                "pulseBel": false,
+                "pulseStandard": true,
+                "qrCode": true,
+                "starCommands": false
+            },
+            "fonts": {
+                "0": {
+                    "columns": 36,
+                    "name": "Font A"
+                },
+                "1": {
+                    "columns": 54,
+                    "name": "Font B"
+                }
+            },
+            "media": {
+                "width": {
+                    "mm": 54,
+                    "pixels": 432
+                }
+            },
+            "name": "RP-F10",
+            "notes": "Seiko RP-F10 series with 58mm paper\n",
+            "vendor": "Seiko"
+        },
+        "RP-F10-80mm": {
+            "codePages": {
+                "0": "CP437",
+                "1": "KATAKANA",
+                "13": "CP857",
+                "14": "CP737",
+                "16": "CP1252",
+                "17": "CP866",
+                "18": "CP852",
+                "19": "CP858",
+                "2": "CP850",
+                "255": "Unknown",
+                "3": "CP860",
+                "34": "CP855",
+                "37": "CP864",
+                "4": "CP863",
+                "45": "CP1250",
+                "46": "CP1251",
+                "47": "CP1253",
+                "48": "CP1254",
+                "5": "CP865"
+            },
+            "colors": {
+                "0": "black"
+            },
+            "features": {
+                "barcodeA": true,
+                "barcodeB": true,
+                "bitImageColumn": true,
+                "bitImageRaster": true,
+                "graphics": true,
+                "highDensity": true,
+                "paperFullCut": true,
+                "paperPartCut": true,
+                "pdf417Code": true,
+                "pulseBel": false,
+                "pulseStandard": true,
+                "qrCode": true,
+                "starCommands": false
+            },
+            "fonts": {
+                "0": {
+                    "columns": 48,
+                    "name": "Font A"
+                },
+                "1": {
+                    "columns": 72,
+                    "name": "Font B"
+                }
+            },
+            "media": {
+                "width": {
+                    "mm": 72,
+                    "pixels": 576
+                }
+            },
+            "name": "RP-F10",
+            "notes": "Seiko RP-F10 series with 80mm paper\n",
+            "vendor": "Seiko"
+        },
         "RP326": {
             "codePages": {
                 "0": "CP437",
-                "1": "Unknown",
+                "1": "KATAKANA",
                 "10": "Unknown",
                 "15": "CP862",
                 "16": "CP1252",
                 "17": "CP1253",
                 "18": "CP852",
                 "19": "CP858",
                 "2": "CP850",
@@ -1119,14 +1364,63 @@
                     "pixels": 384
                 }
             },
             "name": "Sunmi V2",
             "notes": "Sunmi mini-POS Android device with a built-in Virtual Bluetooth thermal printer.\n",
             "vendor": "Sunmi"
         },
+        "T-1": {
+            "codePages": {
+                "0": "CP437",
+                "1": "KATAKANA",
+                "19": "CP858",
+                "2": "CP850",
+                "255": "Unknown",
+                "3": "CP860",
+                "4": "CP863",
+                "5": "CP865"
+            },
+            "colors": {
+                "0": "black"
+            },
+            "features": {
+                "barcodeA": true,
+                "barcodeB": true,
+                "bitImageColumn": true,
+                "bitImageRaster": true,
+                "graphics": true,
+                "highDensity": true,
+                "paperFullCut": true,
+                "paperPartCut": true,
+                "pdf417Code": true,
+                "pulseBel": false,
+                "pulseStandard": true,
+                "qrCode": true,
+                "starCommands": false
+            },
+            "fonts": {
+                "0": {
+                    "columns": 42,
+                    "name": "Font A"
+                },
+                "1": {
+                    "columns": 56,
+                    "name": "Font B"
+                }
+            },
+            "media": {
+                "width": {
+                    "mm": 80,
+                    "pixels": 504
+                }
+            },
+            "name": "T-1",
+            "notes": "Metapace T-1 Thermal Printer Rev. 1.00",
+            "vendor": "Metapace"
+        },
         "TEP-200M": {
             "codePages": {
                 "0": "CP437",
                 "1": "CP932",
                 "11": "CP851",
                 "12": "CP853",
                 "13": "CP857",
@@ -1222,14 +1516,238 @@
                     "pixels": "Unknown"
                 }
             },
             "name": "TEP200M Series",
             "notes": "",
             "vendor": "EPOS"
         },
+        "TH230": {
+            "codePages": {
+                "0": "CP437",
+                "1": "CP850",
+                "10": "CP737",
+                "11": "CP874",
+                "12": "CP857",
+                "16": "CP1254",
+                "17": "CP1250",
+                "18": "Unknown",
+                "19": "Unknown",
+                "2": "CP852",
+                "20": "Unknown",
+                "21": "Unknown",
+                "22": "CP864",
+                "23": "CP720",
+                "24": "CP1256",
+                "25": "Unknown",
+                "26": "KATAKANA",
+                "27": "CP775",
+                "28": "CP1257",
+                "29": "Unknown",
+                "3": "CP860",
+                "4": "CP863",
+                "5": "CP865",
+                "6": "CP858",
+                "7": "CP866",
+                "8": "CP1252",
+                "9": "CP862"
+            },
+            "colors": {
+                "0": "black"
+            },
+            "features": {
+                "barcodeA": true,
+                "barcodeB": true,
+                "bitImageColumn": true,
+                "bitImageRaster": true,
+                "graphics": true,
+                "highDensity": true,
+                "paperFullCut": true,
+                "paperPartCut": true,
+                "pdf417Code": false,
+                "pulseBel": false,
+                "pulseStandard": true,
+                "qrCode": false,
+                "starCommands": false
+            },
+            "fonts": {
+                "0": {
+                    "columns": 44,
+                    "name": "Font A"
+                },
+                "1": {
+                    "columns": 57,
+                    "name": "Font B"
+                }
+            },
+            "media": {
+                "width": {
+                    "mm": 72,
+                    "pixels": 576
+                }
+            },
+            "name": "TH230",
+            "notes": "Profile for TH230. Use bitImageColumn to print properly.\n",
+            "vendor": "Wincor Nixdorf"
+        },
+        "TH230Plus": {
+            "codePages": {
+                "0": "CP437",
+                "1": "CP850",
+                "10": "CP737",
+                "11": "CP874",
+                "12": "CP857",
+                "16": "CP1254",
+                "17": "CP1250",
+                "18": "Unknown",
+                "19": "Unknown",
+                "2": "CP852",
+                "20": "Unknown",
+                "21": "Unknown",
+                "22": "CP864",
+                "23": "CP720",
+                "24": "CP1256",
+                "25": "Unknown",
+                "26": "KATAKANA",
+                "27": "CP775",
+                "28": "CP1257",
+                "29": "Unknown",
+                "3": "CP860",
+                "4": "CP863",
+                "5": "CP865",
+                "6": "CP858",
+                "7": "CP866",
+                "8": "CP1252",
+                "9": "CP862"
+            },
+            "colors": {
+                "0": "black"
+            },
+            "features": {
+                "barcodeA": true,
+                "barcodeB": true,
+                "bitImageColumn": true,
+                "bitImageRaster": true,
+                "graphics": true,
+                "highDensity": true,
+                "paperFullCut": true,
+                "paperPartCut": true,
+                "pdf417Code": true,
+                "pulseBel": false,
+                "pulseStandard": true,
+                "qrCode": true,
+                "starCommands": false
+            },
+            "fonts": {
+                "0": {
+                    "columns": 44,
+                    "name": "Font A"
+                },
+                "1": {
+                    "columns": 57,
+                    "name": "Font B"
+                }
+            },
+            "media": {
+                "width": {
+                    "mm": 72,
+                    "pixels": 576
+                }
+            },
+            "name": "TH230+",
+            "notes": "Profile for TH230+. Use bitImageColumn to print properly. TH230+ supports native qr codes and PDF417 codes\n",
+            "vendor": "Wincor Nixdorf"
+        },
+        "TM-L90": {
+            "codePages": {
+                "0": "CP437",
+                "1": "CP932",
+                "11": "CP851",
+                "12": "CP853",
+                "13": "CP857",
+                "14": "CP737",
+                "15": "ISO_8859-7",
+                "16": "CP1252",
+                "17": "CP866",
+                "18": "CP852",
+                "19": "CP858",
+                "2": "CP850",
+                "20": "Unknown",
+                "21": "CP874",
+                "22": "Unknown",
+                "23": "Unknown",
+                "24": "Unknown",
+                "25": "Unknown",
+                "255": "Unknown",
+                "26": "Unknown",
+                "3": "CP860",
+                "30": "TCVN-3-1",
+                "31": "TCVN-3-2",
+                "32": "CP720",
+                "33": "CP775",
+                "34": "CP855",
+                "35": "CP861",
+                "36": "CP862",
+                "37": "CP864",
+                "38": "CP869",
+                "39": "ISO_8859-2",
+                "4": "CP863",
+                "40": "ISO_8859-15",
+                "41": "CP1098",
+                "42": "CP774",
+                "43": "CP772",
+                "44": "CP1125",
+                "45": "CP1250",
+                "46": "CP1251",
+                "47": "CP1253",
+                "48": "CP1254",
+                "49": "CP1255",
+                "5": "CP865",
+                "50": "CP1256",
+                "51": "CP1257",
+                "52": "CP1258",
+                "53": "RK1048"
+            },
+            "colors": {
+                "0": "black"
+            },
+            "features": {
+                "barcodeA": true,
+                "barcodeB": true,
+                "bitImageColumn": true,
+                "bitImageRaster": true,
+                "graphics": true,
+                "highDensity": true,
+                "paperFullCut": true,
+                "paperPartCut": true,
+                "pdf417Code": true,
+                "pulseBel": false,
+                "pulseStandard": true,
+                "qrCode": true,
+                "starCommands": false
+            },
+            "fonts": {
+                "0": {
+                    "columns": 48,
+                    "name": "Font A"
+                },
+                "1": {
+                    "columns": 64,
+                    "name": "Font B"
+                }
+            },
+            "media": {
+                "width": {
+                    "mm": 80,
+                    "pixels": 576
+                }
+            },
+            "name": "TM-L90",
+            "notes": "Epson TM-L90 profile. The standard 80mm paper width version was used here. The code page mapping is documented in the \"TM-L90 Technical Reference Guide\".\n",
+            "vendor": "Epson"
+        },
         "TM-P80": {
             "codePages": {
                 "0": "CP437",
                 "1": "CP932",
                 "11": "CP851",
                 "12": "CP853",
                 "13": "CP857",
@@ -1436,24 +1954,236 @@
                     "pixels": 546
                 }
             },
             "name": "TM-P80 (42 column mode)",
             "notes": "Portable printer (42-column mode)",
             "vendor": "Epson"
         },
-        "TM-T88II": {
+        "TM-T20II": {
             "codePages": {
                 "0": "CP437",
                 "1": "CP932",
+                "11": "CP851",
+                "12": "CP853",
+                "13": "CP857",
+                "14": "CP737",
+                "15": "ISO_8859-7",
+                "16": "CP1252",
+                "17": "CP866",
+                "18": "CP852",
                 "19": "CP858",
                 "2": "CP850",
                 "255": "Unknown",
                 "3": "CP860",
+                "30": "TCVN-3-1",
+                "31": "TCVN-3-2",
+                "32": "CP720",
+                "33": "CP775",
+                "34": "CP855",
+                "35": "CP861",
+                "36": "CP862",
+                "37": "CP864",
+                "38": "CP869",
+                "39": "ISO_8859-2",
                 "4": "CP863",
-                "5": "CP865"
+                "40": "ISO_8859-15",
+                "41": "CP1098",
+                "44": "CP1125",
+                "45": "CP1250",
+                "46": "CP1251",
+                "47": "CP1253",
+                "48": "CP1254",
+                "49": "CP1255",
+                "5": "CP865",
+                "50": "CP1256",
+                "51": "CP1257",
+                "52": "CP1258",
+                "53": "RK1048"
+            },
+            "colors": {
+                "0": "black"
+            },
+            "features": {
+                "barcodeA": true,
+                "barcodeB": true,
+                "bitImageColumn": true,
+                "bitImageRaster": true,
+                "graphics": true,
+                "highDensity": true,
+                "paperFullCut": true,
+                "paperPartCut": true,
+                "pdf417Code": true,
+                "pulseBel": false,
+                "pulseStandard": true,
+                "qrCode": true,
+                "starCommands": false
+            },
+            "fonts": {
+                "0": {
+                    "columns": 48,
+                    "name": "Font A"
+                },
+                "1": {
+                    "columns": 64,
+                    "name": "Font B"
+                }
+            },
+            "media": {
+                "width": {
+                    "mm": 72,
+                    "pixels": 576
+                }
+            },
+            "name": "TM-T20II",
+            "notes": "Epson TM-T20II profile",
+            "vendor": "Epson"
+        },
+        "TM-T20II-42col": {
+            "codePages": {
+                "0": "CP437",
+                "1": "CP932",
+                "11": "CP851",
+                "12": "CP853",
+                "13": "CP857",
+                "14": "CP737",
+                "15": "ISO_8859-7",
+                "16": "CP1252",
+                "17": "CP866",
+                "18": "CP852",
+                "19": "CP858",
+                "2": "CP850",
+                "255": "Unknown",
+                "3": "CP860",
+                "30": "TCVN-3-1",
+                "31": "TCVN-3-2",
+                "32": "CP720",
+                "33": "CP775",
+                "34": "CP855",
+                "35": "CP861",
+                "36": "CP862",
+                "37": "CP864",
+                "38": "CP869",
+                "39": "ISO_8859-2",
+                "4": "CP863",
+                "40": "ISO_8859-15",
+                "41": "CP1098",
+                "44": "CP1125",
+                "45": "CP1250",
+                "46": "CP1251",
+                "47": "CP1253",
+                "48": "CP1254",
+                "49": "CP1255",
+                "5": "CP865",
+                "50": "CP1256",
+                "51": "CP1257",
+                "52": "CP1258",
+                "53": "RK1048"
+            },
+            "colors": {
+                "0": "black"
+            },
+            "features": {
+                "barcodeA": true,
+                "barcodeB": true,
+                "bitImageColumn": true,
+                "bitImageRaster": true,
+                "graphics": true,
+                "highDensity": true,
+                "paperFullCut": true,
+                "paperPartCut": true,
+                "pdf417Code": true,
+                "pulseBel": false,
+                "pulseStandard": true,
+                "qrCode": true,
+                "starCommands": false
+            },
+            "fonts": {
+                "0": {
+                    "columns": 42,
+                    "name": "Font A"
+                },
+                "1": {
+                    "columns": 60,
+                    "name": "Font B"
+                }
+            },
+            "media": {
+                "width": {
+                    "mm": 68.3,
+                    "pixels": 546
+                }
+            },
+            "name": "TM-T20II (42 column mode)",
+            "notes": "Epson TM-T20II profile (42 column mode)",
+            "vendor": "Epson"
+        },
+        "TM-T88II": {
+            "codePages": {
+                "0": "CP437",
+                "1": "CP932",
+                "11": "Unknown",
+                "12": "Unknown",
+                "13": "CP857",
+                "14": "CP737",
+                "15": "ISO_8859-7",
+                "16": "CP1252",
+                "17": "CP866",
+                "18": "CP852",
+                "19": "Unknown",
+                "2": "CP850",
+                "20": "Unknown",
+                "21": "CP874",
+                "22": "Unknown",
+                "23": "Unknown",
+                "24": "Unknown",
+                "25": "Unknown",
+                "254": "Unknown",
+                "255": "Unknown",
+                "26": "Unknown",
+                "3": "CP860",
+                "30": "TCVN-3-1",
+                "31": "TCVN-3-2",
+                "32": "Unknown",
+                "33": "CP775",
+                "34": "CP855",
+                "35": "CP861",
+                "36": "CP862",
+                "37": "CP864",
+                "38": "CP869",
+                "39": "ISO_8859-2",
+                "4": "CP863",
+                "40": "ISO_8859-15",
+                "41": "Unknown",
+                "42": "CP774",
+                "43": "CP772",
+                "44": "CP1125",
+                "45": "CP1250",
+                "46": "CP1251",
+                "47": "CP1253",
+                "48": "CP1254",
+                "49": "CP1255",
+                "5": "CP865",
+                "50": "CP1256",
+                "51": "CP1257",
+                "52": "CP1258",
+                "53": "RK1048",
+                "6": "Unknown",
+                "66": "Unknown",
+                "67": "Unknown",
+                "68": "Unknown",
+                "69": "Unknown",
+                "7": "Unknown",
+                "70": "Unknown",
+                "71": "Unknown",
+                "72": "Unknown",
+                "73": "Unknown",
+                "74": "Unknown",
+                "75": "Unknown",
+                "8": "Unknown",
+                "82": "Unknown"
             },
             "colors": {
                 "0": "black"
             },
             "features": {
                 "barcodeA": true,
                 "barcodeB": true,
@@ -1477,20 +2207,20 @@
                 "1": {
                     "columns": 56,
                     "name": "Font B"
                 }
             },
             "media": {
                 "width": {
-                    "mm": "Unknown",
-                    "pixels": "Unknown"
+                    "mm": 72,
+                    "pixels": 512
                 }
             },
             "name": "TM-T88II",
-            "notes": "Epson TM-T88II profile. This printer is discontinued by the Vendor, and has similar feature support to the TM-T88III. The code page mapping is documented in the \"TM-T88II/T88III Technical Reference Guide\".\n",
+            "notes": "Epson TM-T88II profile. The specs where taken from a TM-T88IIP machine (I assume the P just stands for parallel port). The standart 80mm paper width version was used here. There is also a custom 58mm factory option. If you are using the custom version change media width to 50.8mm and 360px accordingly. This printer is discontinued by the Vendor and has similar feature support to the TM-T88III. The code page mapping is documented in the \"TM-T88II/T88III Technical Reference Guide\".\n",
             "vendor": "Epson"
         },
         "TM-T88III": {
             "codePages": {
                 "0": "CP437",
                 "1": "CP932",
                 "16": "CP1252",
@@ -1529,16 +2259,16 @@
                 "1": {
                     "columns": 56,
                     "name": "Font B"
                 }
             },
             "media": {
                 "width": {
-                    "mm": "Unknown",
-                    "pixels": "Unknown"
+                    "mm": 80,
+                    "pixels": 512
                 }
             },
             "name": "TM-T88III",
             "notes": "Epson TM-T88III profile. This printer has similar feature support to the TM-T88II. The code page mapping is documented in the \"TM-T88II/T88III Technical Reference Guide\".\n",
             "vendor": "Epson"
         },
         "TM-T88IV": {
```

### Comparing `python-escpos-3.0a8/doc/Makefile` & `python-escpos-3.0a9/doc/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 SPHINXOPTS    =
 SPHINXBUILD   = sphinx-build
 PAPER         =
 BUILDDIR      = _build
 
 # User-friendly check for sphinx-build
 ifeq ($(shell which $(SPHINXBUILD) >/dev/null 2>&1; echo $$?), 1)
-$(error The '$(SPHINXBUILD)' command was not found. Make sure you have Sphinx installed, then set the SPHINXBUILD environment variable to point to the full path of the '$(SPHINXBUILD)' executable. Alternatively you can add the directory with the executable to your PATH. If you don't have Sphinx installed, grab it from http://sphinx-doc.org/)
+$(error The '$(SPHINXBUILD)' command was not found. Make sure you have Sphinx installed, then set the SPHINXBUILD environment variable to point to the full path of the '$(SPHINXBUILD)' executable. Alternatively you can add the directory with the executable to your PATH. If you don't have Sphinx installed, grab it from https://sphinx-doc.org/)
 endif
 
 # Internal variables.
 PAPEROPT_a4     = -D latex_paper_size=a4
 PAPEROPT_letter = -D latex_paper_size=letter
 ALLSPHINXOPTS   = -d $(BUILDDIR)/doctrees $(PAPEROPT_$(PAPER)) $(SPHINXOPTS) .
 # the i18n builder cannot share the environment and doctrees with the others
```

### Comparing `python-escpos-3.0a8/doc/_build/html/_sources/index.rst.txt` & `python-escpos-3.0a9/doc/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/doc/_build/html/_sources/index.txt` & `python-escpos-3.0a9/doc/_build/html/_sources/index.txt`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/doc/_build/html/_sources/user/barcode.rst.txt` & `python-escpos-3.0a9/doc/_build/html/_sources/user/barcode.rst.txt`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/doc/_build/html/_sources/user/barcode.txt` & `python-escpos-3.0a9/doc/_build/html/_sources/user/barcode.txt`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/doc/_build/html/_sources/user/installation.rst.txt` & `python-escpos-3.0a9/doc/_build/html/_sources/user/installation.rst.txt`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/doc/_build/html/_sources/user/installation.txt` & `python-escpos-3.0a9/doc/_build/html/_sources/user/installation.txt`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/doc/_build/html/_sources/user/printers.rst.txt` & `python-escpos-3.0a9/doc/_build/html/_sources/user/printers.rst.txt`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/doc/_build/html/_sources/user/printers.txt` & `python-escpos-3.0a9/doc/_build/html/_sources/user/printers.txt`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/doc/_build/html/_sources/user/raspi.rst.txt` & `python-escpos-3.0a9/doc/_build/html/_sources/user/raspi.rst.txt`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/doc/_build/html/_sources/user/raspi.txt` & `python-escpos-3.0a9/doc/_build/html/_sources/user/raspi.txt`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/doc/_build/html/_sources/user/todo.rst.txt` & `python-escpos-3.0a9/doc/_build/html/_sources/user/todo.txt`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/doc/_build/html/_sources/user/usage.rst.txt` & `python-escpos-3.0a9/doc/_build/html/_sources/user/usage.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,92 +40,89 @@
 The first command will yield the "Interface" number that must be handy
 to have and the second yields the "Output Endpoint" address.
 
 **USB Printer initialization**
 
 ::
 
-    p = printer.Usb(0x04b8,0x0202)
+    Epson = printer.Usb(0x04b8,0x0202)
 
 By default the "Interface" number is "0" and the "Output Endpoint"
 address is "0x01". If you have other values then you can define them on
 your instance. So, assuming that we have another printer where in\_ep is
 on 0x81 and out\_ep=0x02, then the printer definition should look like:
 
 **Generic USB Printer initialization**
 
 ::
 
-    p = printer.Usb(0x1a2b,0x1a2b,0,0x81,0x02)
+    Generic = printer.Usb(0x1a2b,0x1a2b,0,0x81,0x02)
 
 Network printer
 ^^^^^^^^^^^^^^^
 
 You only need the IP of your printer, either because it is getting its
 IP by DHCP or you set it manually.
 
 **Network Printer initialization**
 
 ::
 
-    p = printer.Network("192.168.1.99")
+    Epson = printer.Network("192.168.1.99")
 
 Serial printer
 ^^^^^^^^^^^^^^
 
 Most of the default values set by the DIP switches for the serial
 printers, have been set as default on the serial printer class, so the
 only thing you need to know is which serial port the printer is connected
 to.
 
 **Serial printer initialization**
 
 ::
 
-    p = printer.Serial("/dev/tty0")
-    
-    # on a Windows OS serial devices are typically accessible as COM
-    p = printer.Serial("COM1")
+    Epson = printer.Serial("/dev/tty0")
 
 Other printers
 ^^^^^^^^^^^^^^
 
 Some printers under `/dev` can't be used or initialized with any of the
 methods described above. Usually, those are printers used by printcap,
 however, if you know the device name, you could try to initialize by
 passing the device node name.
 
 ::
 
-    p = printer.File("/dev/usb/lp1")
+    Epson = printer.File("/dev/usb/lp1")
 
 The default is "/dev/usb/lp0", so if the printer is located on that
 node, then you don't necessary need to pass the node name.
 
 Define your instance
 --------------------
 
 The following example demonstrates how to initialize the Epson TM-TI88IV
 on a USB interface.
 
 ::
 
     from escpos import *
     """ Seiko Epson Corp. Receipt Printer M129 Definitions (EPSON TM-T88IV) """
-    p = printer.Usb(0x04b8,0x0202)
+    Epson = printer.Usb(0x04b8,0x0202)
     # Print text
-    p.text("Hello World\n")
+    Epson.text("Hello World\n")
     # Print image
-    p.image("logo.gif")
+    Epson.image("logo.gif")
     # Print QR Code
-    p.qr("You can readme from your smartphone")
+    Epson.qr("You can readme from your smartphone")
     # Print barcode
-    p.barcode('1324354657687','EAN13',64,2,'','')
+    Epson.barcode('1324354657687','EAN13',64,2,'','')
     # Cut paper
-    p.cut()
+    Epson.cut()
 
 Configuration File
 ------------------
 
 You can create a configuration file for python-escpos. This will
 allow you to use the CLI, and skip some setup when using the library
 programmatically.
```

### Comparing `python-escpos-3.0a8/doc/_build/html/_sources/user/usage.txt` & `python-escpos-3.0a9/doc/user/usage.rst`

 * *Files 5% similar despite different names*

```diff
@@ -40,89 +40,99 @@
 The first command will yield the "Interface" number that must be handy
 to have and the second yields the "Output Endpoint" address.
 
 **USB Printer initialization**
 
 ::
 
-    Epson = printer.Usb(0x04b8,0x0202)
+    p = printer.Usb(0x04b8,0x0202)
 
 By default the "Interface" number is "0" and the "Output Endpoint"
 address is "0x01". If you have other values then you can define them on
-your instance. So, assuming that we have another printer where in\_ep is
-on 0x81 and out\_ep=0x02, then the printer definition should look like:
+your instance. So, assuming that we have another printer, CT-S2000,
+manufactured by Citizen (with "Vendor ID" of 2730 and "Product ID" of 0fff)
+where in\_ep is on 0x81 and out\_ep=0x02, then the printer definition should
+look like:
 
 **Generic USB Printer initialization**
 
 ::
 
-    Generic = printer.Usb(0x1a2b,0x1a2b,0,0x81,0x02)
+    p = printer.Usb(0x2730, 0x0fff, 0, 0x81, 0x02)
 
 Network printer
 ^^^^^^^^^^^^^^^
 
 You only need the IP of your printer, either because it is getting its
 IP by DHCP or you set it manually.
 
 **Network Printer initialization**
 
 ::
 
-    Epson = printer.Network("192.168.1.99")
+    p = printer.Network("192.168.1.99")
 
 Serial printer
 ^^^^^^^^^^^^^^
 
 Most of the default values set by the DIP switches for the serial
 printers, have been set as default on the serial printer class, so the
 only thing you need to know is which serial port the printer is connected
 to.
 
 **Serial printer initialization**
 
 ::
 
-    Epson = printer.Serial("/dev/tty0")
+    p = printer.Serial("/dev/tty0")
+
+    # on a Windows OS serial devices are typically accessible as COM
+    p = printer.Serial("COM1")
 
 Other printers
 ^^^^^^^^^^^^^^
 
 Some printers under `/dev` can't be used or initialized with any of the
 methods described above. Usually, those are printers used by printcap,
 however, if you know the device name, you could try to initialize by
 passing the device node name.
 
 ::
 
-    Epson = printer.File("/dev/usb/lp1")
+    p = printer.File("/dev/usb/lp1")
 
 The default is "/dev/usb/lp0", so if the printer is located on that
 node, then you don't necessary need to pass the node name.
 
 Define your instance
 --------------------
 
 The following example demonstrates how to initialize the Epson TM-TI88IV
 on a USB interface.
 
 ::
 
     from escpos import *
     """ Seiko Epson Corp. Receipt Printer M129 Definitions (EPSON TM-T88IV) """
-    Epson = printer.Usb(0x04b8,0x0202)
+    p = printer.Usb(0x04b8,0x0202)
     # Print text
-    Epson.text("Hello World\n")
+    p.text("Hello World\n")
     # Print image
-    Epson.image("logo.gif")
+    p.image("logo.gif")
     # Print QR Code
-    Epson.qr("You can readme from your smartphone")
+    p.qr("You can readme from your smartphone")
     # Print barcode
-    Epson.barcode('1324354657687','EAN13',64,2,'','')
+    p.barcode('1324354657687','EAN13',64,2,'','')
     # Cut paper
-    Epson.cut()
+    p.cut()
+
+Standard python constraints on libraries apply. This means especially
+that you should not name the script in which you implement these lines
+should not be named ``escpos`` as this would collide with the name of
+the library.
 
 Configuration File
 ------------------
 
 You can create a configuration file for python-escpos. This will
 allow you to use the CLI, and skip some setup when using the library
 programmatically.
@@ -154,15 +164,15 @@
 
 
 The printer section
 ^^^^^^^^^^^^^^^^^^^
 
 The ``printer`` configuration section defines a default printer to create.
 
-The only required paramter is ``type``. The value of this has to be one of the
+The only required parameter is ``type``. The value of this has to be one of the
 printers defined in :doc:`/user/printers`.
 
 The rest of the given parameters will be passed on to the initialization of the printer class.
 Use these to overwrite the default values as specified in :doc:`/user/printers`.
 This implies that the parameters have to match the parameter-names of the respective printer class.
 
 An example file printer::
@@ -185,20 +195,20 @@
             idVendor: 0x1234
             idProduct: 0x5678
             in_ep: 0x66
             out_ep: 0x01
 
 Printing text right
 -------------------
-Python-escpos is designed to accept unicode. So make sure that you use ``u'strings'`` or import ``unicode_literals``
-from ``__future__`` if you are on Python 2. On Python 3 you should be fine.
+
+Python-escpos is designed to accept unicode.
 
 For normal usage you can simply pass your text to the printers ``text()``-function. It will automatically guess
 the right codepage and then send the encoded data to the printer. If this feature does not work, please try to
-isolate the error and then create an issue on the Github project page.
+isolate the error and then create an issue on the GitHub project page.
 
 If you want or need to you can manually set the codepage. For this please use the ``charcode()``-function. You can set
 any key-value that is in ``CHARCODE``. If something is wrong, an ``CharCodeError`` will be raised.
 After you have manually set the codepage the printer won't change it anymore. You can revert to normal behaviour
 by setting charcode to ``AUTO``.
 
 Advanced Usage: Print from binary blob
@@ -280,8 +290,22 @@
    # send code to printer
    p._raw(d.output)
 
 This way you could also store the code in a file and print it later.
 You could then for example print the code from another process than your main-program and thus reduce the waiting time.
 (Of course this will not make the printer print faster.)
 
+Troubleshooting
+---------------
+
+This section gathers various hints on troubleshooting.
+
+Print with STAR TSP100 family
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Printer of the STAR TSP100 family do not have a native ESC/POS mode, which
+is why you will not be able to directly print with this library to the printer.
+
+More information on this topic can be found in the online documentation of
+`Star Micronics <https://www.starmicronics.com/help-center/knowledge-base/configure-tsp100-series-printers-esc-pos-mode/>`_
+and the `discussion in the python-escpos project <https://github.com/python-escpos/python-escpos/issues/410>`_.
+
```

### Comparing `python-escpos-3.0a8/doc/_build/html/_static/pyescpos.ico` & `python-escpos-3.0a9/doc/_build/html/_static/pyescpos.ico`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/doc/_build/latex/Makefile` & `python-escpos-3.0a9/doc/_build/latex/Makefile`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/doc/_build/spelling/output.txt` & `python-escpos-3.0a9/doc/_build/spelling/output.txt`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/doc/conf.py` & `python-escpos-3.0a9/doc/conf.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,292 +10,301 @@
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 import sys
 import os
-on_rtd = os.getenv('READTHEDOCS') == 'True'
-if on_rtd:
-    import escpos
-else:
-    from setuptools_scm import get_version
+
+from importlib.metadata import version as imp_version
+
+on_rtd = os.getenv("READTHEDOCS") == "True"
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-sys.path.insert(0, os.path.abspath('../src'))
-root = os.path.relpath(os.path.join(os.path.dirname(__file__), '..'))
+sys.path.insert(0, os.path.abspath("../src"))
+root = os.path.relpath(os.path.join(os.path.dirname(__file__), ".."))
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
-#needs_sphinx = '1.0'
+# needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.doctest',
-    'sphinx.ext.todo',
-    'sphinx.ext.coverage',
-    'sphinx.ext.viewcode',
-    'sphinx.ext.todo',
-    'sphinx.ext.graphviz',
-    'sphinx.ext.inheritance_diagram',
-    'sphinxcontrib.spelling',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.doctest",
+    "sphinx.ext.todo",
+    "sphinx.ext.coverage",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.todo",
+    "sphinx.ext.graphviz",
+    "sphinx.ext.inheritance_diagram",
+    "sphinxcontrib.spelling",
 ]
 
 # supress warnings for external images
 suppress_warnings = [
-    'image.nonlocal_uri',
+    "image.nonlocal_uri",
 ]
 
 # enable todos
 todo_include_todos = True
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix of source filenames.
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
-#source_encoding = 'utf-8-sig'
+# source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'python-escpos'
-copyright = u'2016, Manuel F Martinez and others'
+project = "python-escpos"
+copyright = "2016, Manuel F Martinez and others"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
-if on_rtd:
-    # The full version, including alpha/beta/rc tags.
-    release = escpos.__version__
-else:
-    # locally setuptools_scm should work
-    release = get_version(root=root)
+release = imp_version("python-escpos")
 # The short X.Y version.
-version = '.'.join(release.split('.')[:2])  # The short X.Y version.
+version = ".".join(release.split(".")[:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
-#language = None
+# language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = ['_build']
+exclude_patterns = ["_build"]
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
-#default_role = None
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
-#keep_warnings = False
+# keep_warnings = False
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 if on_rtd:
-    html_theme = 'default'
+    html_theme = "default"
 else:
     try:
         import sphinx_rtd_theme
-        html_theme = 'sphinx_rtd_theme'
+
+        html_theme = "sphinx_rtd_theme"
         html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
     except ImportError:
         print("no sphinx_rtd_theme found, switching to nature")
-        html_theme = 'default'
+        html_theme = "default"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+# html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
+# html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-#html_title = None
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+# html_logo = None
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-html_favicon = 'pyescpos.ico'
+html_favicon = "pyescpos.ico"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
-#html_extra_path = []
+# html_extra_path = []
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
+# html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
+# html_sidebars = {}
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_domain_indices = True
+# html_domain_indices = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
+# html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-#html_show_sphinx = True
+# html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-#html_show_copyright = True
+# html_show_copyright = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = None
+# html_file_suffix = None
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'python-escposdoc'
+htmlhelp_basename = "python-escposdoc"
 
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
-# The paper size ('letterpaper' or 'a4paper').
-#'papersize': 'letterpaper',
-
-# The font size ('10pt', '11pt' or '12pt').
-#'pointsize': '10pt',
-
-# Additional stuff for the LaTeX preamble.
-#'preamble': '',
+    # The paper size ('letterpaper' or 'a4paper').
+    #'papersize': 'letterpaper',
+    # The font size ('10pt', '11pt' or '12pt').
+    #'pointsize': '10pt',
+    # Additional stuff for the LaTeX preamble.
+    #'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-  ('index', 'python-escpos.tex', u'python-escpos Documentation',
-   u'Manuel F Martinez and others', 'manual'),
+    (
+        "index",
+        "python-escpos.tex",
+        "python-escpos Documentation",
+        "Manuel F Martinez and others",
+        "manual",
+    ),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
-#latex_logo = None
+# latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
-#latex_use_parts = False
+# latex_use_parts = False
 
 # If true, show page references after internal links.
-#latex_show_pagerefs = False
+# latex_show_pagerefs = False
 
 # If true, show URL addresses after external links.
-#latex_show_urls = False
+# latex_show_urls = False
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_domain_indices = True
+# latex_domain_indices = True
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    ('index', 'python-escpos', u'python-escpos Documentation',
-     [u'Manuel F Martinez and others'], 1)
+    (
+        "index",
+        "python-escpos",
+        "python-escpos Documentation",
+        ["Manuel F Martinez and others"],
+        1,
+    )
 ]
 
 # If true, show URL addresses after external links.
-#man_show_urls = False
+# man_show_urls = False
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-  ('index', 'python-escpos', u'python-escpos Documentation',
-   u'Manuel F Martinez and others', 'python-escpos', 'One line description of project.',
-   'Miscellaneous'),
+    (
+        "index",
+        "python-escpos",
+        "python-escpos Documentation",
+        "Manuel F Martinez and others",
+        "python-escpos",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
 
 # Documents to append as an appendix to all manuals.
-#texinfo_appendices = []
+# texinfo_appendices = []
 
 # If false, no module index is generated.
-#texinfo_domain_indices = True
+# texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
-#texinfo_show_urls = 'footnote'
+# texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
-#texinfo_no_detailmenu = False
+# texinfo_no_detailmenu = False
 
 # spellchecker
 spelling_ignore_pypi_package_names = True
 spelling_ignore_wiki_words = True
 spelling_ignore_python_builtins = True
 spelling_ignore_importable_modules = True
```

### Comparing `python-escpos-3.0a8/doc/download/barcode.bin` & `python-escpos-3.0a9/doc/download/barcode.bin`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/doc/index.rst` & `python-escpos-3.0a9/doc/index.rst`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/doc/make.bat` & `python-escpos-3.0a9/doc/make.bat`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 	echo.
 	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
 	echo.installed, then set the SPHINXBUILD environment variable to point
 	echo.to the full path of the 'sphinx-build' executable. Alternatively you
 	echo.may add the Sphinx directory to PATH.
 	echo.
 	echo.If you don't have Sphinx installed, grab it from
-	echo.http://sphinx-doc.org/
+	echo.https://sphinx-doc.org/
 	exit /b 1
 )
 
 if "%1" == "html" (
 	%SPHINXBUILD% -b html %ALLSPHINXOPTS% %BUILDDIR%/html
 	if errorlevel 1 exit /b 1
 	echo.
```

### Comparing `python-escpos-3.0a8/doc/pyescpos.ico` & `python-escpos-3.0a9/doc/pyescpos.ico`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/doc/user/barcode.rst` & `python-escpos-3.0a9/doc/user/barcode.rst`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/doc/user/installation.rst` & `python-escpos-3.0a9/doc/user/installation.rst`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/doc/user/printers.rst` & `python-escpos-3.0a9/doc/user/printers.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ********
 Printers
 ********
-:Last Reviewed: 2017-01-25
+:Last Reviewed: 2022-11-25
 
-As of now there are 5 different type of printer implementations.
+As of now there are 7 different type of printer implementations.
 
 USB
 ---
 The USB-class uses pyusb and libusb to communicate with USB-based
 printers. Note that this driver is not suited for USB-to-Serial-adapters
 and similiar devices, but only for those implementing native USB.
 
@@ -71,7 +71,30 @@
 all of the "output" as raw ESC/POS in a string and returns that.
 
 .. autoclass:: escpos.printer.Dummy
       :members:
       :member-order: bysource
       :noindex:
 
+CUPS
+----
+This driver uses `pycups` in order to communicate with a CUPS server.
+Supports both local and remote CUPS printers and servers.
+The printer must be properly configured in CUPS administration.
+The connector generates a print job that is added to the CUPS queue.
+
+.. todo:: fix import in documentation
+
+LP
+----
+This driver uses the UNIX command `lp` in order to communicate with a CUPS server.
+Supports local and remote CUPS printers.
+The printer must be properly configured in CUPS administration.
+The connector spawns a new sub-process where the command lp is executed.
+
+No dependencies required, but somehow the print queue will affect some print job such as barcode.
+
+.. autoclass:: escpos.printer.LP
+      :members:
+      :special-members:
+      :member-order: bysource
+      :noindex:
```

### Comparing `python-escpos-3.0a8/doc/user/raspi.rst` & `python-escpos-3.0a9/doc/user/raspi.rst`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/doc/user/usage.rst` & `python-escpos-3.0a9/doc/_build/html/_sources/user/usage.rst.txt`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,19 @@
     # Print QR Code
     p.qr("You can readme from your smartphone")
     # Print barcode
     p.barcode('1324354657687','EAN13',64,2,'','')
     # Cut paper
     p.cut()
 
+Standard python constraints on libraries apply. This means especially
+that you should not name the script in which you implement these lines
+should not be named ``escpos`` as this would collide with the name of
+the library.
+
 Configuration File
 ------------------
 
 You can create a configuration file for python-escpos. This will
 allow you to use the CLI, and skip some setup when using the library
 programmatically.
 
@@ -285,8 +290,22 @@
    # send code to printer
    p._raw(d.output)
 
 This way you could also store the code in a file and print it later.
 You could then for example print the code from another process than your main-program and thus reduce the waiting time.
 (Of course this will not make the printer print faster.)
 
+Troubleshooting
+---------------
+
+This section gathers varios hint on troubleshooting.
+
+Print with STAR TSP100 family
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Printer of the STAR TSP100 family do not have a native ESC/POS mode, which
+is why you will not be able to directly print with this library to the printer.
+
+More information on this topic can be found in the online documentation of
+`Star Micronics <https://www.starmicronics.com/help-center/knowledge-base/configure-tsp100-series-printers-esc-pos-mode/>`_
+and the `discussion in the python-escpos project <https://github.com/python-escpos/python-escpos/issues/410>`_.
+
```

### Comparing `python-escpos-3.0a8/examples/codepage_tables.py` & `python-escpos-3.0a9/examples/codepage_tables.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,31 @@
 """
 
 
 import six
 import sys
 
 from escpos import printer
-from escpos.constants import CODEPAGE_CHANGE, ESC, CTL_LF, CTL_FF, CTL_CR, CTL_HT, CTL_VT
+from escpos.constants import (
+    CODEPAGE_CHANGE,
+    ESC,
+    CTL_LF,
+    CTL_FF,
+    CTL_CR,
+    CTL_HT,
+    CTL_VT,
+)
 
 
 def main():
     dummy = printer.Dummy()
 
-    dummy.hw('init')
+    dummy.hw("init")
 
-    for codepage in sys.argv[1:] or ['USA']:
+    for codepage in sys.argv[1:] or ["USA"]:
         dummy.set(height=2, width=2)
         dummy._raw(codepage + "\n\n\n")
         print_codepage(dummy, codepage)
         dummy._raw("\n\n")
 
     dummy.cut()
 
@@ -32,31 +40,31 @@
         printer._raw("after")
     else:
         printer.charcode(codepage)
 
     sep = ""
 
     # Table header
-    printer.set(font='b')
+    printer.set(font="b")
     printer._raw("  {}\n".format(sep.join(map(lambda s: hex(s)[2:], range(0, 16)))))
     printer.set()
 
     # The table
     for x in range(0, 16):
         # First column
-        printer.set(font='b')
+        printer.set(font="b")
         printer._raw("{} ".format(hex(x)[2:]))
         printer.set()
 
         for y in range(0, 16):
             byte = six.int2byte(x * 16 + y)
 
             if byte in (ESC, CTL_LF, CTL_FF, CTL_CR, CTL_HT, CTL_VT):
-                byte = ' '
+                byte = " "
 
             printer._raw(byte)
             printer._raw(sep)
-        printer._raw('\n')
+        printer._raw("\n")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `python-escpos-3.0a8/examples/graphics/climacons/clear-day.png` & `python-escpos-3.0a9/examples/graphics/climacons/clear-day.png`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/examples/graphics/climacons/clear-night.png` & `python-escpos-3.0a9/examples/graphics/climacons/clear-night.png`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/examples/graphics/climacons/cloudy.png` & `python-escpos-3.0a9/examples/graphics/climacons/cloudy.png`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/examples/graphics/climacons/fog.png` & `python-escpos-3.0a9/examples/graphics/climacons/fog.png`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/examples/graphics/climacons/partly-cloudy-day.png` & `python-escpos-3.0a9/examples/graphics/climacons/partly-cloudy-day.png`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/examples/graphics/climacons/partly-cloudy-night.png` & `python-escpos-3.0a9/examples/graphics/climacons/partly-cloudy-night.png`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/examples/graphics/climacons/rain.png` & `python-escpos-3.0a9/examples/graphics/climacons/rain.png`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/examples/graphics/climacons/readme.md` & `python-escpos-3.0a9/examples/graphics/climacons/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Climacons by Adam Whitcroft
 
-75 climatically categorised pictographs for web and UI design by [@adamwhitcroft](http://www.twitter.com/#!/adamwhitcroft).
+75 climatically categorised pictographs for web and UI design by [@adamwhitcroft](https://www.twitter.com/#!/adamwhitcroft).
 
-Visit the [Climacons](http://adamwhitcroft.com/climacons/) website for more information.
+Visit the [Climacons](https://adamwhitcroft.com/climacons/) website for more information.
 
 Visit [Adam Whitcroft on GitHub](https://github.com/AdamWhitcroft)
 
 ## License
-You are free to use any of the Climacons Icons (the "icons") in any personal or commercial work without obligation of payment (monetary or otherwise) or attribution, however a credit for the work would be appreciated. **Do not** redistribute or sell and **do not** claim creative credit. Intellectual property rights are not transferred with the download of the icons.
+You are free to use any of the Climacons Icons (the "icons") in any personal or commercial work without obligation of payment (monetary or otherwise) or attribution, however a credit for the work would be appreciated. **Do not** redistribute or sell and **do not** claim creative credit. Intellectual property rights are not transferred with the download of the icons.
```

### Comparing `python-escpos-3.0a8/examples/graphics/climacons/sleet.png` & `python-escpos-3.0a9/examples/graphics/climacons/sleet.png`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/examples/graphics/climacons/snow.png` & `python-escpos-3.0a9/examples/graphics/climacons/snow.png`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/examples/graphics/climacons/wind.png` & `python-escpos-3.0a9/examples/graphics/climacons/wind.png`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/examples/weather.py` & `python-escpos-3.0a9/examples/weather.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Weather forecast for Raspberry Pi w/Adafruit Mini Thermal Printer.
 # Retrieves data from DarkSky.net's API, prints current conditions and
 # forecasts for next two days.
 # Weather example using nice bitmaps.
 # Written by Adafruit Industries.  MIT license.
 # Adapted and enhanced for escpos library by MrWunderbar666
 
-# Icons taken from http://adamwhitcroft.com/climacons/
+# Icons taken from https://adamwhitcroft.com/climacons/
 # Check out his github: https://github.com/AdamWhitcroft/climacons
 
 
 from datetime import datetime
 import calendar
 import urllib
 import json
@@ -29,98 +29,100 @@
 # Adapt to your needs
 printer = Usb(0x0416, 0x5011, profile="POS-5890")
 
 # You can get your API Key on www.darksky.net and register a dev account.
 # Technically you can use any other weather service, of course :)
 API_KEY = "YOUR API KEY"
 
-LAT = "22.345490"       # Your Location
-LONG = "114.189945"     # Your Location
+LAT = "22.345490"  # Your Location
+LONG = "114.189945"  # Your Location
 
 
 def forecast_icon(idx):
-    icon = data['daily']['data'][idx]['icon']
+    icon = data["daily"]["data"][idx]["icon"]
     image = GRAPHICS_PATH + icon + ".png"
     return image
 
 
 # Dumps one forecast line to the printer
 def forecast(idx):
-    date = datetime.fromtimestamp(int(data['daily']['data'][idx]['time']))
+    date = datetime.fromtimestamp(int(data["daily"]["data"][idx]["time"]))
     day = calendar.day_name[date.weekday()]
-    lo = data['daily']['data'][idx]['temperatureMin']
-    hi = data['daily']['data'][idx]['temperatureMax']
-    cond = data['daily']['data'][idx]['summary']
+    lo = data["daily"]["data"][idx]["temperatureMin"]
+    hi = data["daily"]["data"][idx]["temperatureMax"]
+    cond = data["daily"]["data"][idx]["summary"]
     print(date)
     print(day)
     print(lo)
     print(hi)
     print(cond)
     time.sleep(1)
-    printer.set(
-        font='a',
-        height=2,
-        align='left',
-        bold=False,
-        double_height=False)
-    printer.text(day + ' \n ')
-    time.sleep(5)           # Sleep to prevent printer buffer overflow
-    printer.text('\n')
+    printer.set(font="a", height=2, align="left", bold=False, double_height=False)
+    printer.text(day + " \n ")
+    time.sleep(5)  # Sleep to prevent printer buffer overflow
+    printer.text("\n")
     printer.image(forecast_icon(idx))
-    printer.text('low ' + str(lo))
+    printer.text("low " + str(lo))
     printer.text(deg)
-    printer.text('\n')
-    printer.text(' high ' + str(hi))
+    printer.text("\n")
+    printer.text(" high " + str(hi))
     printer.text(deg)
-    printer.text('\n')
+    printer.text("\n")
     # take care of pesky unicode dash
-    printer.text(cond.replace(u'\u2013', '-').encode('utf-8'))
-    printer.text('\n \n')
+    printer.text(cond.replace("\u2013", "-").encode("utf-8"))
+    printer.text("\n \n")
 
 
 def icon():
-    icon = data['currently']['icon']
+    icon = data["currently"]["icon"]
     image = GRAPHICS_PATH + icon + ".png"
     return image
 
 
-deg = ' C'      # Degree symbol on thermal printer, need to find a better way to use a proper degree symbol
+deg = " C"  # Degree symbol on thermal printer, need to find a better way to use a proper degree symbol
 
 # if you want Fahrenheit change units= to 'us'
-url = "https://api.darksky.net/forecast/" + API_KEY + "/" + LAT + "," + LONG + \
-    "?exclude=[alerts,minutely,hourly,flags]&units=si"  # change last bit to 'us' for Fahrenheit
+url = (
+    "https://api.darksky.net/forecast/"
+    + API_KEY
+    + "/"
+    + LAT
+    + ","
+    + LONG
+    + "?exclude=[alerts,minutely,hourly,flags]&units=si"
+)  # change last bit to 'us' for Fahrenheit
 response = urllib.urlopen(url)
 data = json.loads(response.read())
 
 printer.print_and_feed(n=1)
 printer.control("LF")
-printer.set(font='a', height=2, align='center', bold=True, double_height=True)
+printer.set(font="a", height=2, align="center", bold=True, double_height=True)
 printer.text("Weather Forecast")
 printer.text("\n")
-printer.set(align='center')
+printer.set(align="center")
 
 
 # Print current conditions
-printer.set(font='a', height=2, align='center', bold=True, double_height=False)
-printer.text('Current conditions: \n')
+printer.set(font="a", height=2, align="center", bold=True, double_height=False)
+printer.text("Current conditions: \n")
 printer.image(icon())
 printer.text("\n")
 
-printer.set(font='a', height=2, align='left', bold=False, double_height=False)
-temp = data['currently']['temperature']
-cond = data['currently']['summary']
+printer.set(font="a", height=2, align="left", bold=False, double_height=False)
+temp = data["currently"]["temperature"]
+cond = data["currently"]["summary"]
 printer.text(temp)
-printer.text(' ')
+printer.text(" ")
 printer.text(deg)
-printer.text(' ')
-printer.text('\n')
-printer.text('Sky: ' + cond)
-printer.text('\n')
-printer.text('\n')
+printer.text(" ")
+printer.text("\n")
+printer.text("Sky: " + cond)
+printer.text("\n")
+printer.text("\n")
 
 # Print forecast
-printer.set(font='a', height=2, align='center', bold=True, double_height=False)
-printer.text('Forecast: \n')
+printer.set(font="a", height=2, align="center", bold=True, double_height=False)
+printer.text("Forecast: \n")
 forecast(0)
 forecast(1)
 printer.cut()
 printer.control("LF")
```

### Comparing `python-escpos-3.0a8/setup.cfg` & `python-escpos-3.0a9/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -14,28 +14,29 @@
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.5
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Office/Business :: Financial :: Point-Of-Sale
 project_urls = 
 	Bug Tracker = https://github.com/python-escpos/python-escpos/issues
 	Documentation = https://python-escpos.readthedocs.io/en/latest/
 	Release Notes = https://github.com/python-escpos/python-escpos/releases
 
 [options]
-python_requires = >=3.5
+python_requires = >=3.6
 zip_safe = false
 include_package_data = true
 install_requires = 
 	pyusb>=1.0.0
 	Pillow>=2.0
 	qrcode>=4.0
 	pyserial
@@ -43,28 +44,27 @@
 	setuptools
 	six
 	appdirs
 	PyYAML
 	argparse
 	argcomplete
 	future
-	viivakoodi>=0.8
 setup_requires = setuptools_scm
 tests_require = 
 	jaconv
 	tox
 	pytest!=3.2.0,!=3.3.0
 	pytest-cov
 	pytest-mock
 	nose
 	scripttest
 	mock
 	hypothesis>4
 	flake8
-	sphinxcontrib-spelling>=5
+	sphinxcontrib-spelling>=7.2.0
 
 [nosetests]
 verbosity = 3
 with-doctest = 1
 
 [flake8]
 exclude = .git,.tox,.github,.eggs,__pycache__,doc/conf.py,build,dist,capabilities-data,test,src/escpos/constants.py
```

### Comparing `python-escpos-3.0a8/setup.py` & `python-escpos-3.0a9/setup.py`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/src/escpos/capabilities.json` & `python-escpos-3.0a9/src/escpos/capabilities.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.927627418093268%*

 * *Differences: {"'encodings'": "{'KATAKANA': OrderedDict([('data', ['▁▂▃▄▅▆▇█▏▎▍▌▋▊▉┼', '┴┬┤├¯─│▕┌┐└┘╭╮╰╯', ' "*

 * *                "｡｢｣､･ｦｧｨｩｪｫｬｭｮｯ', 'ｰｱｲｳｴｵｶｷｸｹｺｻｼｽｾｿ', 'ﾀﾁﾂﾃﾄﾅﾆﾇﾈﾉﾊﾋﾌﾍﾎﾏ', 'ﾐﾑﾒﾓﾔﾕﾖﾗﾘﾙﾚﾛﾜﾝﾞﾟ', "*

 * *                "'═╞╪╡◢◣◥◤♠♥♦♣●○╱╲', '╳円年月日時分秒〒市区町村人▓\\xa0']), ('name', 'Katakana (codepage "*

 * *                "1)')])}",*

 * * "'profiles'": "{'P822D': {'codePages': {'1': 'KATAKANA'}}, 'RP326': {'codePages': {'1': "*

 * *               "'KATAKANA'}}, 'TM-T88II': {'codePages': {'19': 'Unknown', '6': 'Unknown', '7': "*

 * *          […]*

```diff
@@ -286,14 +286,27 @@
             "python_encode": "iso8859_8"
         },
         "ISO_8859-9": {
             "iconv": "ISO_8859-9",
             "name": "ISO_8859-9",
             "python_encode": "iso8859_9"
         },
+        "KATAKANA": {
+            "data": [
+                "\u2581\u2582\u2583\u2584\u2585\u2586\u2587\u2588\u258f\u258e\u258d\u258c\u258b\u258a\u2589\u253c",
+                "\u2534\u252c\u2524\u251c\u00af\u2500\u2502\u2595\u250c\u2510\u2514\u2518\u256d\u256e\u2570\u256f",
+                " \uff61\uff62\uff63\uff64\uff65\uff66\uff67\uff68\uff69\uff6a\uff6b\uff6c\uff6d\uff6e\uff6f",
+                "\uff70\uff71\uff72\uff73\uff74\uff75\uff76\uff77\uff78\uff79\uff7a\uff7b\uff7c\uff7d\uff7e\uff7f",
+                "\uff80\uff81\uff82\uff83\uff84\uff85\uff86\uff87\uff88\uff89\uff8a\uff8b\uff8c\uff8d\uff8e\uff8f",
+                "\uff90\uff91\uff92\uff93\uff94\uff95\uff96\uff97\uff98\uff99\uff9a\uff9b\uff9c\uff9d\uff9e\uff9f",
+                "\u2550\u255e\u256a\u2561\u25e2\u25e3\u25e5\u25e4\u2660\u2665\u2666\u2663\u25cf\u25cb\u2571\u2572",
+                "\u2573\u5186\u5e74\u6708\u65e5\u6642\u5206\u79d2\u3012\u5e02\u533a\u753a\u6751\u4eba\u2593\u00a0"
+            ],
+            "name": "Katakana (codepage 1)"
+        },
         "OXHOO-EUROPEAN": {
             "data": [
                 "\u00c7\u00fc\u00e9\u00e2\u00e4\u00e0\u00e5\u00e7\u00ea\u00eb\u00e8\u00ef\u00ee\u00ec\u00c4\u00c5",
                 "\u00c9\u00e6\u00c6\u00f4\u00f6\u00f2\u00fb\u00f9\u00ff\u00d6\u00dc\u00f1\u00d1\u00aa\u00ba\u00bf",
                 "\u00e1\u00ed\u00f3\u00fa\u00a2\u00a3\u00a5\u20a7\u0192\u00a1\u00c3\u00e3\u00d5\u00f5\u00d8\u00f8",
                 "\u00b7\u00a8\u00b0`\u00b4\u00bd\u00bc\u00d7\u00f7\u2264\u2265\u00ab\u00bb\u2260\u221a\u00af",
                 "\u2320\u2321\u221e\u25e4\u21b5\u2191\u2193\u2192\u2190\u250c\u2510\u2514\u2518\u2022\u00ae\u00a9",
@@ -441,14 +454,126 @@
                     "pixels": 640
                 }
             },
             "name": "CT-S651",
             "notes": "Citizen CT-S651 profile. This is a two-color thermal printer, supporting paper sizes from 58mm up to 83mm\n",
             "vendor": "Citizen"
         },
+        "KR-306": {
+            "codePages": {
+                "0": "CP437",
+                "1": "KATAKANA",
+                "10": "Unknown",
+                "11": "CP1252",
+                "12": "CP866",
+                "13": "CP852",
+                "14": "CP858",
+                "15": "Unknown",
+                "16": "Unknown",
+                "17": "Unknown",
+                "18": "Unknown",
+                "19": "CP747",
+                "2": "CP850",
+                "20": "Unknown",
+                "21": "Unknown",
+                "22": "Unknown",
+                "23": "CP864",
+                "24": "Unknown",
+                "25": "Unknown",
+                "26": "Unknown",
+                "27": "CP1255",
+                "28": "CP437",
+                "29": "KATAKANA",
+                "3": "CP860",
+                "30": "CP437",
+                "31": "CP858",
+                "32": "CP852",
+                "33": "CP860",
+                "34": "CP861",
+                "35": "CP863",
+                "36": "CP865",
+                "37": "CP866",
+                "38": "CP855",
+                "39": "CP857",
+                "4": "CP863",
+                "40": "CP862",
+                "41": "CP864",
+                "42": "CP737",
+                "43": "CP851",
+                "44": "CP869",
+                "45": "CP928",
+                "46": "CP772",
+                "47": "CP774",
+                "48": "CP874",
+                "49": "CP1252",
+                "5": "CP865",
+                "50": "CP1250",
+                "51": "CP1251",
+                "52": "CP3840",
+                "53": "CP3841",
+                "54": "CP3843",
+                "55": "CP3844",
+                "56": "CP3845",
+                "57": "CP3846",
+                "58": "CP3847",
+                "59": "CP3848",
+                "6": "Unknown",
+                "60": "CP1001",
+                "61": "CP2001",
+                "62": "CP3001",
+                "63": "CP3002",
+                "64": "CP3011",
+                "65": "CP3012",
+                "66": "CP3021",
+                "67": "CP3041",
+                "68": "CP852",
+                "69": "Unknown",
+                "7": "Unknown",
+                "70": "CP1256",
+                "8": "Unknown",
+                "9": "Unknown"
+            },
+            "colors": {
+                "0": "black"
+            },
+            "features": {
+                "barcodeA": true,
+                "barcodeB": true,
+                "bitImageColumn": true,
+                "bitImageRaster": true,
+                "graphics": false,
+                "highDensity": true,
+                "paperFullCut": true,
+                "paperPartCut": true,
+                "pdf417Code": true,
+                "pulseBel": false,
+                "pulseStandard": true,
+                "qrCode": true,
+                "starCommands": false
+            },
+            "fonts": {
+                "0": {
+                    "columns": 48,
+                    "name": "Font A"
+                },
+                "1": {
+                    "columns": 64,
+                    "name": "Font B"
+                }
+            },
+            "media": {
+                "width": {
+                    "mm": 72,
+                    "pixels": 576
+                }
+            },
+            "name": "KR-306",
+            "notes": "Kefar KR-306 printer with 200mm/s speed\n",
+            "vendor": "Kefar"
+        },
         "NT-5890K": {
             "codePages": {
                 "0": "CP437",
                 "1": "CP932",
                 "10": "Unknown",
                 "16": "CP1252",
                 "17": "CP866",
@@ -667,15 +792,15 @@
             "name": "OCD-300 Customer Display",
             "notes": "This is a two-line, ESC/POS-aware customer display from Aures. It has some graphics support via vendor-provided tools, but is otherwise text-only.\n",
             "vendor": "Aures"
         },
         "P822D": {
             "codePages": {
                 "0": "CP437",
-                "1": "Unknown",
+                "1": "KATAKANA",
                 "10": "Unknown",
                 "16": "CP1252",
                 "17": "CP866",
                 "18": "CP852",
                 "19": "CP858",
                 "2": "CP850",
                 "20": "Unknown",
@@ -885,18 +1010,138 @@
                     "pixels": 384
                 }
             },
             "name": "POS5890 Series",
             "notes": "POS-5890 thermal printer series, also marketed under various other names.\n",
             "vendor": "Zjiang"
         },
+        "RP-F10-58mm": {
+            "codePages": {
+                "0": "CP437",
+                "1": "KATAKANA",
+                "13": "CP857",
+                "14": "CP737",
+                "16": "CP1252",
+                "17": "CP866",
+                "18": "CP852",
+                "19": "CP858",
+                "2": "CP850",
+                "255": "Unknown",
+                "3": "CP860",
+                "34": "CP855",
+                "37": "CP864",
+                "4": "CP863",
+                "45": "CP1250",
+                "46": "CP1251",
+                "47": "CP1253",
+                "48": "CP1254",
+                "5": "CP865"
+            },
+            "colors": {
+                "0": "black"
+            },
+            "features": {
+                "barcodeA": true,
+                "barcodeB": true,
+                "bitImageColumn": true,
+                "bitImageRaster": true,
+                "graphics": true,
+                "highDensity": true,
+                "paperFullCut": true,
+                "paperPartCut": true,
+                "pdf417Code": true,
+                "pulseBel": false,
+                "pulseStandard": true,
+                "qrCode": true,
+                "starCommands": false
+            },
+            "fonts": {
+                "0": {
+                    "columns": 36,
+                    "name": "Font A"
+                },
+                "1": {
+                    "columns": 54,
+                    "name": "Font B"
+                }
+            },
+            "media": {
+                "width": {
+                    "mm": 54,
+                    "pixels": 432
+                }
+            },
+            "name": "RP-F10",
+            "notes": "Seiko RP-F10 series with 58mm paper\n",
+            "vendor": "Seiko"
+        },
+        "RP-F10-80mm": {
+            "codePages": {
+                "0": "CP437",
+                "1": "KATAKANA",
+                "13": "CP857",
+                "14": "CP737",
+                "16": "CP1252",
+                "17": "CP866",
+                "18": "CP852",
+                "19": "CP858",
+                "2": "CP850",
+                "255": "Unknown",
+                "3": "CP860",
+                "34": "CP855",
+                "37": "CP864",
+                "4": "CP863",
+                "45": "CP1250",
+                "46": "CP1251",
+                "47": "CP1253",
+                "48": "CP1254",
+                "5": "CP865"
+            },
+            "colors": {
+                "0": "black"
+            },
+            "features": {
+                "barcodeA": true,
+                "barcodeB": true,
+                "bitImageColumn": true,
+                "bitImageRaster": true,
+                "graphics": true,
+                "highDensity": true,
+                "paperFullCut": true,
+                "paperPartCut": true,
+                "pdf417Code": true,
+                "pulseBel": false,
+                "pulseStandard": true,
+                "qrCode": true,
+                "starCommands": false
+            },
+            "fonts": {
+                "0": {
+                    "columns": 48,
+                    "name": "Font A"
+                },
+                "1": {
+                    "columns": 72,
+                    "name": "Font B"
+                }
+            },
+            "media": {
+                "width": {
+                    "mm": 72,
+                    "pixels": 576
+                }
+            },
+            "name": "RP-F10",
+            "notes": "Seiko RP-F10 series with 80mm paper\n",
+            "vendor": "Seiko"
+        },
         "RP326": {
             "codePages": {
                 "0": "CP437",
-                "1": "Unknown",
+                "1": "KATAKANA",
                 "10": "Unknown",
                 "15": "CP862",
                 "16": "CP1252",
                 "17": "CP1253",
                 "18": "CP852",
                 "19": "CP858",
                 "2": "CP850",
@@ -1119,14 +1364,63 @@
                     "pixels": 384
                 }
             },
             "name": "Sunmi V2",
             "notes": "Sunmi mini-POS Android device with a built-in Virtual Bluetooth thermal printer.\n",
             "vendor": "Sunmi"
         },
+        "T-1": {
+            "codePages": {
+                "0": "CP437",
+                "1": "KATAKANA",
+                "19": "CP858",
+                "2": "CP850",
+                "255": "Unknown",
+                "3": "CP860",
+                "4": "CP863",
+                "5": "CP865"
+            },
+            "colors": {
+                "0": "black"
+            },
+            "features": {
+                "barcodeA": true,
+                "barcodeB": true,
+                "bitImageColumn": true,
+                "bitImageRaster": true,
+                "graphics": true,
+                "highDensity": true,
+                "paperFullCut": true,
+                "paperPartCut": true,
+                "pdf417Code": true,
+                "pulseBel": false,
+                "pulseStandard": true,
+                "qrCode": true,
+                "starCommands": false
+            },
+            "fonts": {
+                "0": {
+                    "columns": 42,
+                    "name": "Font A"
+                },
+                "1": {
+                    "columns": 56,
+                    "name": "Font B"
+                }
+            },
+            "media": {
+                "width": {
+                    "mm": 80,
+                    "pixels": 504
+                }
+            },
+            "name": "T-1",
+            "notes": "Metapace T-1 Thermal Printer Rev. 1.00",
+            "vendor": "Metapace"
+        },
         "TEP-200M": {
             "codePages": {
                 "0": "CP437",
                 "1": "CP932",
                 "11": "CP851",
                 "12": "CP853",
                 "13": "CP857",
@@ -1222,14 +1516,238 @@
                     "pixels": "Unknown"
                 }
             },
             "name": "TEP200M Series",
             "notes": "",
             "vendor": "EPOS"
         },
+        "TH230": {
+            "codePages": {
+                "0": "CP437",
+                "1": "CP850",
+                "10": "CP737",
+                "11": "CP874",
+                "12": "CP857",
+                "16": "CP1254",
+                "17": "CP1250",
+                "18": "Unknown",
+                "19": "Unknown",
+                "2": "CP852",
+                "20": "Unknown",
+                "21": "Unknown",
+                "22": "CP864",
+                "23": "CP720",
+                "24": "CP1256",
+                "25": "Unknown",
+                "26": "KATAKANA",
+                "27": "CP775",
+                "28": "CP1257",
+                "29": "Unknown",
+                "3": "CP860",
+                "4": "CP863",
+                "5": "CP865",
+                "6": "CP858",
+                "7": "CP866",
+                "8": "CP1252",
+                "9": "CP862"
+            },
+            "colors": {
+                "0": "black"
+            },
+            "features": {
+                "barcodeA": true,
+                "barcodeB": true,
+                "bitImageColumn": true,
+                "bitImageRaster": true,
+                "graphics": true,
+                "highDensity": true,
+                "paperFullCut": true,
+                "paperPartCut": true,
+                "pdf417Code": false,
+                "pulseBel": false,
+                "pulseStandard": true,
+                "qrCode": false,
+                "starCommands": false
+            },
+            "fonts": {
+                "0": {
+                    "columns": 44,
+                    "name": "Font A"
+                },
+                "1": {
+                    "columns": 57,
+                    "name": "Font B"
+                }
+            },
+            "media": {
+                "width": {
+                    "mm": 72,
+                    "pixels": 576
+                }
+            },
+            "name": "TH230",
+            "notes": "Profile for TH230. Use bitImageColumn to print properly.\n",
+            "vendor": "Wincor Nixdorf"
+        },
+        "TH230Plus": {
+            "codePages": {
+                "0": "CP437",
+                "1": "CP850",
+                "10": "CP737",
+                "11": "CP874",
+                "12": "CP857",
+                "16": "CP1254",
+                "17": "CP1250",
+                "18": "Unknown",
+                "19": "Unknown",
+                "2": "CP852",
+                "20": "Unknown",
+                "21": "Unknown",
+                "22": "CP864",
+                "23": "CP720",
+                "24": "CP1256",
+                "25": "Unknown",
+                "26": "KATAKANA",
+                "27": "CP775",
+                "28": "CP1257",
+                "29": "Unknown",
+                "3": "CP860",
+                "4": "CP863",
+                "5": "CP865",
+                "6": "CP858",
+                "7": "CP866",
+                "8": "CP1252",
+                "9": "CP862"
+            },
+            "colors": {
+                "0": "black"
+            },
+            "features": {
+                "barcodeA": true,
+                "barcodeB": true,
+                "bitImageColumn": true,
+                "bitImageRaster": true,
+                "graphics": true,
+                "highDensity": true,
+                "paperFullCut": true,
+                "paperPartCut": true,
+                "pdf417Code": true,
+                "pulseBel": false,
+                "pulseStandard": true,
+                "qrCode": true,
+                "starCommands": false
+            },
+            "fonts": {
+                "0": {
+                    "columns": 44,
+                    "name": "Font A"
+                },
+                "1": {
+                    "columns": 57,
+                    "name": "Font B"
+                }
+            },
+            "media": {
+                "width": {
+                    "mm": 72,
+                    "pixels": 576
+                }
+            },
+            "name": "TH230+",
+            "notes": "Profile for TH230+. Use bitImageColumn to print properly. TH230+ supports native qr codes and PDF417 codes\n",
+            "vendor": "Wincor Nixdorf"
+        },
+        "TM-L90": {
+            "codePages": {
+                "0": "CP437",
+                "1": "CP932",
+                "11": "CP851",
+                "12": "CP853",
+                "13": "CP857",
+                "14": "CP737",
+                "15": "ISO_8859-7",
+                "16": "CP1252",
+                "17": "CP866",
+                "18": "CP852",
+                "19": "CP858",
+                "2": "CP850",
+                "20": "Unknown",
+                "21": "CP874",
+                "22": "Unknown",
+                "23": "Unknown",
+                "24": "Unknown",
+                "25": "Unknown",
+                "255": "Unknown",
+                "26": "Unknown",
+                "3": "CP860",
+                "30": "TCVN-3-1",
+                "31": "TCVN-3-2",
+                "32": "CP720",
+                "33": "CP775",
+                "34": "CP855",
+                "35": "CP861",
+                "36": "CP862",
+                "37": "CP864",
+                "38": "CP869",
+                "39": "ISO_8859-2",
+                "4": "CP863",
+                "40": "ISO_8859-15",
+                "41": "CP1098",
+                "42": "CP774",
+                "43": "CP772",
+                "44": "CP1125",
+                "45": "CP1250",
+                "46": "CP1251",
+                "47": "CP1253",
+                "48": "CP1254",
+                "49": "CP1255",
+                "5": "CP865",
+                "50": "CP1256",
+                "51": "CP1257",
+                "52": "CP1258",
+                "53": "RK1048"
+            },
+            "colors": {
+                "0": "black"
+            },
+            "features": {
+                "barcodeA": true,
+                "barcodeB": true,
+                "bitImageColumn": true,
+                "bitImageRaster": true,
+                "graphics": true,
+                "highDensity": true,
+                "paperFullCut": true,
+                "paperPartCut": true,
+                "pdf417Code": true,
+                "pulseBel": false,
+                "pulseStandard": true,
+                "qrCode": true,
+                "starCommands": false
+            },
+            "fonts": {
+                "0": {
+                    "columns": 48,
+                    "name": "Font A"
+                },
+                "1": {
+                    "columns": 64,
+                    "name": "Font B"
+                }
+            },
+            "media": {
+                "width": {
+                    "mm": 80,
+                    "pixels": 576
+                }
+            },
+            "name": "TM-L90",
+            "notes": "Epson TM-L90 profile. The standard 80mm paper width version was used here. The code page mapping is documented in the \"TM-L90 Technical Reference Guide\".\n",
+            "vendor": "Epson"
+        },
         "TM-P80": {
             "codePages": {
                 "0": "CP437",
                 "1": "CP932",
                 "11": "CP851",
                 "12": "CP853",
                 "13": "CP857",
@@ -1436,24 +1954,236 @@
                     "pixels": 546
                 }
             },
             "name": "TM-P80 (42 column mode)",
             "notes": "Portable printer (42-column mode)",
             "vendor": "Epson"
         },
-        "TM-T88II": {
+        "TM-T20II": {
             "codePages": {
                 "0": "CP437",
                 "1": "CP932",
+                "11": "CP851",
+                "12": "CP853",
+                "13": "CP857",
+                "14": "CP737",
+                "15": "ISO_8859-7",
+                "16": "CP1252",
+                "17": "CP866",
+                "18": "CP852",
                 "19": "CP858",
                 "2": "CP850",
                 "255": "Unknown",
                 "3": "CP860",
+                "30": "TCVN-3-1",
+                "31": "TCVN-3-2",
+                "32": "CP720",
+                "33": "CP775",
+                "34": "CP855",
+                "35": "CP861",
+                "36": "CP862",
+                "37": "CP864",
+                "38": "CP869",
+                "39": "ISO_8859-2",
                 "4": "CP863",
-                "5": "CP865"
+                "40": "ISO_8859-15",
+                "41": "CP1098",
+                "44": "CP1125",
+                "45": "CP1250",
+                "46": "CP1251",
+                "47": "CP1253",
+                "48": "CP1254",
+                "49": "CP1255",
+                "5": "CP865",
+                "50": "CP1256",
+                "51": "CP1257",
+                "52": "CP1258",
+                "53": "RK1048"
+            },
+            "colors": {
+                "0": "black"
+            },
+            "features": {
+                "barcodeA": true,
+                "barcodeB": true,
+                "bitImageColumn": true,
+                "bitImageRaster": true,
+                "graphics": true,
+                "highDensity": true,
+                "paperFullCut": true,
+                "paperPartCut": true,
+                "pdf417Code": true,
+                "pulseBel": false,
+                "pulseStandard": true,
+                "qrCode": true,
+                "starCommands": false
+            },
+            "fonts": {
+                "0": {
+                    "columns": 48,
+                    "name": "Font A"
+                },
+                "1": {
+                    "columns": 64,
+                    "name": "Font B"
+                }
+            },
+            "media": {
+                "width": {
+                    "mm": 72,
+                    "pixels": 576
+                }
+            },
+            "name": "TM-T20II",
+            "notes": "Epson TM-T20II profile",
+            "vendor": "Epson"
+        },
+        "TM-T20II-42col": {
+            "codePages": {
+                "0": "CP437",
+                "1": "CP932",
+                "11": "CP851",
+                "12": "CP853",
+                "13": "CP857",
+                "14": "CP737",
+                "15": "ISO_8859-7",
+                "16": "CP1252",
+                "17": "CP866",
+                "18": "CP852",
+                "19": "CP858",
+                "2": "CP850",
+                "255": "Unknown",
+                "3": "CP860",
+                "30": "TCVN-3-1",
+                "31": "TCVN-3-2",
+                "32": "CP720",
+                "33": "CP775",
+                "34": "CP855",
+                "35": "CP861",
+                "36": "CP862",
+                "37": "CP864",
+                "38": "CP869",
+                "39": "ISO_8859-2",
+                "4": "CP863",
+                "40": "ISO_8859-15",
+                "41": "CP1098",
+                "44": "CP1125",
+                "45": "CP1250",
+                "46": "CP1251",
+                "47": "CP1253",
+                "48": "CP1254",
+                "49": "CP1255",
+                "5": "CP865",
+                "50": "CP1256",
+                "51": "CP1257",
+                "52": "CP1258",
+                "53": "RK1048"
+            },
+            "colors": {
+                "0": "black"
+            },
+            "features": {
+                "barcodeA": true,
+                "barcodeB": true,
+                "bitImageColumn": true,
+                "bitImageRaster": true,
+                "graphics": true,
+                "highDensity": true,
+                "paperFullCut": true,
+                "paperPartCut": true,
+                "pdf417Code": true,
+                "pulseBel": false,
+                "pulseStandard": true,
+                "qrCode": true,
+                "starCommands": false
+            },
+            "fonts": {
+                "0": {
+                    "columns": 42,
+                    "name": "Font A"
+                },
+                "1": {
+                    "columns": 60,
+                    "name": "Font B"
+                }
+            },
+            "media": {
+                "width": {
+                    "mm": 68.3,
+                    "pixels": 546
+                }
+            },
+            "name": "TM-T20II (42 column mode)",
+            "notes": "Epson TM-T20II profile (42 column mode)",
+            "vendor": "Epson"
+        },
+        "TM-T88II": {
+            "codePages": {
+                "0": "CP437",
+                "1": "CP932",
+                "11": "Unknown",
+                "12": "Unknown",
+                "13": "CP857",
+                "14": "CP737",
+                "15": "ISO_8859-7",
+                "16": "CP1252",
+                "17": "CP866",
+                "18": "CP852",
+                "19": "Unknown",
+                "2": "CP850",
+                "20": "Unknown",
+                "21": "CP874",
+                "22": "Unknown",
+                "23": "Unknown",
+                "24": "Unknown",
+                "25": "Unknown",
+                "254": "Unknown",
+                "255": "Unknown",
+                "26": "Unknown",
+                "3": "CP860",
+                "30": "TCVN-3-1",
+                "31": "TCVN-3-2",
+                "32": "Unknown",
+                "33": "CP775",
+                "34": "CP855",
+                "35": "CP861",
+                "36": "CP862",
+                "37": "CP864",
+                "38": "CP869",
+                "39": "ISO_8859-2",
+                "4": "CP863",
+                "40": "ISO_8859-15",
+                "41": "Unknown",
+                "42": "CP774",
+                "43": "CP772",
+                "44": "CP1125",
+                "45": "CP1250",
+                "46": "CP1251",
+                "47": "CP1253",
+                "48": "CP1254",
+                "49": "CP1255",
+                "5": "CP865",
+                "50": "CP1256",
+                "51": "CP1257",
+                "52": "CP1258",
+                "53": "RK1048",
+                "6": "Unknown",
+                "66": "Unknown",
+                "67": "Unknown",
+                "68": "Unknown",
+                "69": "Unknown",
+                "7": "Unknown",
+                "70": "Unknown",
+                "71": "Unknown",
+                "72": "Unknown",
+                "73": "Unknown",
+                "74": "Unknown",
+                "75": "Unknown",
+                "8": "Unknown",
+                "82": "Unknown"
             },
             "colors": {
                 "0": "black"
             },
             "features": {
                 "barcodeA": true,
                 "barcodeB": true,
@@ -1477,20 +2207,20 @@
                 "1": {
                     "columns": 56,
                     "name": "Font B"
                 }
             },
             "media": {
                 "width": {
-                    "mm": "Unknown",
-                    "pixels": "Unknown"
+                    "mm": 72,
+                    "pixels": 512
                 }
             },
             "name": "TM-T88II",
-            "notes": "Epson TM-T88II profile. This printer is discontinued by the Vendor, and has similar feature support to the TM-T88III. The code page mapping is documented in the \"TM-T88II/T88III Technical Reference Guide\".\n",
+            "notes": "Epson TM-T88II profile. The specs where taken from a TM-T88IIP machine (I assume the P just stands for parallel port). The standart 80mm paper width version was used here. There is also a custom 58mm factory option. If you are using the custom version change media width to 50.8mm and 360px accordingly. This printer is discontinued by the Vendor and has similar feature support to the TM-T88III. The code page mapping is documented in the \"TM-T88II/T88III Technical Reference Guide\".\n",
             "vendor": "Epson"
         },
         "TM-T88III": {
             "codePages": {
                 "0": "CP437",
                 "1": "CP932",
                 "16": "CP1252",
@@ -1529,16 +2259,16 @@
                 "1": {
                     "columns": 56,
                     "name": "Font B"
                 }
             },
             "media": {
                 "width": {
-                    "mm": "Unknown",
-                    "pixels": "Unknown"
+                    "mm": 80,
+                    "pixels": 512
                 }
             },
             "name": "TM-T88III",
             "notes": "Epson TM-T88III profile. This printer has similar feature support to the TM-T88II. The code page mapping is documented in the \"TM-T88II/T88III Technical Reference Guide\".\n",
             "vendor": "Epson"
         },
         "TM-T88IV": {
```

### Comparing `python-escpos-3.0a8/src/escpos/capabilities.py` & `python-escpos-3.0a9/src/escpos/capabilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,138 +7,142 @@
 
 import six
 import yaml
 
 from tempfile import gettempdir
 import platform
 
+from typing import Any, Dict
+
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
-pickle_dir = environ.get('ESCPOS_CAPABILITIES_PICKLE_DIR', gettempdir())
-pickle_path = path.join(pickle_dir, '{v}.capabilities.pickle'.format(v=platform.python_version()))
+pickle_dir = environ.get("ESCPOS_CAPABILITIES_PICKLE_DIR", gettempdir())
+pickle_path = path.join(
+    pickle_dir, "{v}.capabilities.pickle".format(v=platform.python_version())
+)
 # get a temporary file from pkg_resources if no file is specified in env
-capabilities_path = environ.get('ESCPOS_CAPABILITIES_FILE',
-                                pkg_resources.resource_filename(__name__, 'capabilities.json'))
+capabilities_path = environ.get(
+    "ESCPOS_CAPABILITIES_FILE",
+    pkg_resources.resource_filename(__name__, "capabilities.json"),
+)
 
 # Load external printer database
 t0 = time.time()
-logger.debug('Using capabilities from file: %s', capabilities_path)
+logger.debug("Using capabilities from file: %s", capabilities_path)
 if path.exists(pickle_path):
     if path.getmtime(capabilities_path) > path.getmtime(pickle_path):
-        logger.debug('Found a more recent capabilities file')
+        logger.debug("Found a more recent capabilities file")
         full_load = True
     else:
         full_load = False
-        logger.debug('Loading capabilities from pickle in %s', pickle_path)
-        with open(pickle_path, 'rb') as cf:
+        logger.debug("Loading capabilities from pickle in %s", pickle_path)
+        with open(pickle_path, "rb") as cf:
             CAPABILITIES = pickle.load(cf)
 else:
-    logger.debug('Capabilities pickle file not found: %s', pickle_path)
+    logger.debug("Capabilities pickle file not found: %s", pickle_path)
     full_load = True
 
 if full_load:
-    logger.debug('Loading and pickling capabilities')
-    with open(capabilities_path) as cp, open(pickle_path, 'wb') as pp:
+    logger.debug("Loading and pickling capabilities")
+    with open(capabilities_path) as cp, open(pickle_path, "wb") as pp:
         CAPABILITIES = yaml.safe_load(cp)
         pickle.dump(CAPABILITIES, pp, protocol=2)
 
-logger.debug('Finished loading capabilities took %.2fs', time.time() - t0)
+logger.debug("Finished loading capabilities took %.2fs", time.time() - t0)
 
 
-PROFILES = CAPABILITIES['profiles']
+PROFILES: Dict[str, Any] = CAPABILITIES["profiles"]
 
 
 class NotSupported(Exception):
     """Raised if a requested feature is not supported by the
     printer profile.
     """
+
     pass
 
 
-BARCODE_B = 'barcodeB'
+BARCODE_B = "barcodeB"
 
 
 class BaseProfile(object):
     """This represents a printer profile.
 
     A printer profile knows about the number of columns, supported
     features, colors and more.
     """
 
-    profile_data = {}
+    profile_data: Dict[str, Any] = {}
 
     def __getattr__(self, name):
         return self.profile_data[name]
 
-    def get_font(self, font):
+    def get_font(self, font) -> int:
         """Return the escpos index for `font`. Makes sure that
         the requested `font` is valid.
         """
-        font = {'a': 0, 'b': 1}.get(font, font)
+        font = {"a": 0, "b": 1}.get(font, font)
         if not six.text_type(font) in self.fonts:
             raise NotSupported(
-                '"{}" is not a valid font in the current profile'.format(font))
+                '"{}" is not a valid font in the current profile'.format(font)
+            )
         return font
 
     def get_columns(self, font):
-        """ Return the number of columns for the given font.
-        """
+        """Return the number of columns for the given font."""
         font = self.get_font(font)
-        return self.fonts[six.text_type(font)]['columns']
+        return self.fonts[six.text_type(font)]["columns"]
 
     def supports(self, feature):
-        """Return true/false for the given feature.
-        """
+        """Return true/false for the given feature."""
         return self.features.get(feature)
 
     def get_code_pages(self):
-        """Return the support code pages as a ``{name: index}`` dict.
-        """
+        """Return the support code pages as a ``{name: index}`` dict."""
         return {v: k for k, v in self.codePages.items()}
 
 
-def get_profile(name=None, **kwargs):
+def get_profile(name: str = None, **kwargs):
     """Get the profile by name; if no name is given, return the
     default profile.
     """
     if isinstance(name, Profile):
         return name
 
-    clazz = get_profile_class(name or 'default')
+    clazz = get_profile_class(name or "default")
     return clazz(**kwargs)
 
 
 CLASS_CACHE = {}
 
 
-def get_profile_class(name):
+def get_profile_class(name: str):
     """For the given profile name, load the data from the external
     database, then generate dynamically a class.
     """
     if name not in CLASS_CACHE:
         profile_data = PROFILES[name]
         profile_name = clean(name)
-        class_name = '{}{}Profile'.format(
-            profile_name[0].upper(), profile_name[1:])
-        new_class = type(class_name, (BaseProfile,), {'profile_data': profile_data})
+        class_name = "{}{}Profile".format(profile_name[0].upper(), profile_name[1:])
+        new_class = type(class_name, (BaseProfile,), {"profile_data": profile_data})
         CLASS_CACHE[name] = new_class
 
     return CLASS_CACHE[name]
 
 
 def clean(s):
     # Remove invalid characters
-    s = re.sub('[^0-9a-zA-Z_]', '', s)
+    s = re.sub("[^0-9a-zA-Z_]", "", s)
     # Remove leading characters until we find a letter or underscore
-    s = re.sub('^[^a-zA-Z_]+', '', s)
+    s = re.sub("^[^a-zA-Z_]+", "", s)
     return str(s)
 
 
-class Profile(get_profile_class('default')):
+class Profile(get_profile_class("default")):
     """
     For users, who want to provide their profile
     """
 
     def __init__(self, columns=None, features=None):
         super(Profile, self).__init__()
```

### Comparing `python-escpos-3.0a8/src/escpos/codepages.py` & `python-escpos-3.0a9/src/escpos/codepages.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
         # TODO resolve the encoding alias
         return encoding.upper()
 
     def get_encoding(self, encoding):
         return self.data[encoding]
 
 
-CodePages = CodePageManager(CAPABILITIES['encodings'])
+CodePages = CodePageManager(CAPABILITIES["encodings"])
```

### Comparing `python-escpos-3.0a8/src/escpos/config.py` & `python-escpos-3.0a9/src/escpos/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,105 +10,107 @@
 import yaml
 
 from . import printer
 from . import exceptions
 
 
 class Config(object):
-    """  Configuration handler class.
+    """Configuration handler class.
 
     This class loads configuration from a default or specificed directory. It
     can create your defined printer and return it to you.
     """
-    _app_name = 'python-escpos'
-    _config_file = 'config.yaml'
+
+    _app_name = "python-escpos"
+    _config_file = "config.yaml"
 
     def __init__(self):
-        """ Initialize configuration.
+        """Initialize configuration.
 
         Remember to add anything that needs to be reset between configurations
         to self._reset_config
         """
         self._has_loaded = False
         self._printer = None
 
         self._printer_name = None
         self._printer_config = None
 
     def _reset_config(self):
-        """ Clear the loaded configuration.
+        """Clear the loaded configuration.
 
         If we are loading a changed config, we don't want to have leftover
         data.
         """
         self._has_loaded = False
         self._printer = None
 
         self._printer_name = None
         self._printer_config = None
 
     def load(self, config_path=None):
-        """ Load and parse the configuration file using pyyaml
+        """Load and parse the configuration file using pyyaml
 
         :param config_path: An optional file path, file handle, or byte string
             for the configuration file.
 
         """
 
         self._reset_config()
 
         if not config_path:
             config_path = os.path.join(
-                appdirs.user_config_dir(self._app_name),
-                self._config_file
+                appdirs.user_config_dir(self._app_name), self._config_file
             )
 
         try:
             # First check if it's file like. If it is, pyyaml can load it.
             # I'm checking type instead of catching exceptions to keep the
             # exception handling simple
-            if hasattr(config_path, 'read'):
+            if hasattr(config_path, "read"):
                 config = yaml.safe_load(config_path)
             else:
                 # If it isn't, it's a path. We have to open it first, otherwise
                 # pyyaml will try to read it as yaml
-                with open(config_path, 'rb') as config_file:
+                with open(config_path, "rb") as config_file:
                     config = yaml.safe_load(config_file)
         except EnvironmentError:
-            raise exceptions.ConfigNotFoundError('Couldn\'t read config at {config_path}'.format(
-                config_path=str(config_path),
-            ))
+            raise exceptions.ConfigNotFoundError(
+                "Couldn't read config at {config_path}".format(
+                    config_path=str(config_path),
+                )
+            )
         except yaml.YAMLError:
-            raise exceptions.ConfigSyntaxError('Error parsing YAML')
+            raise exceptions.ConfigSyntaxError("Error parsing YAML")
 
-        if 'printer' in config:
-            self._printer_config = config['printer']
-            self._printer_name = self._printer_config.pop('type').title()
+        if "printer" in config:
+            self._printer_config = config["printer"]
+            self._printer_name = self._printer_config.pop("type").title()
 
             if not self._printer_name or not hasattr(printer, self._printer_name):
                 raise exceptions.ConfigSyntaxError(
                     'Printer type "{printer_name}" is invalid'.format(
                         printer_name=self._printer_name,
                     )
                 )
 
         self._has_loaded = True
 
     def printer(self):
-        """ Returns a printer that was defined in the config, or throws an
+        """Returns a printer that was defined in the config, or throws an
         exception.
 
         This method loads the default config if one hasn't beeen already loaded.
 
         """
         if not self._has_loaded:
             self.load()
 
         if not self._printer_name:
-            raise exceptions.ConfigSectionMissingError('printer')
+            raise exceptions.ConfigSectionMissingError("printer")
 
         if not self._printer:
             # We could catch init errors and make them a ConfigSyntaxError,
             # but I'll just let them pass
             self._printer = getattr(printer, self._printer_name)(**self._printer_config)
 
         return self._printer
```

### Comparing `python-escpos-3.0a8/src/escpos/constants.py` & `python-escpos-3.0a9/src/escpos/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,241 +11,259 @@
 :license: MIT
 """
 
 
 import six
 
 # Control characters
-# as labelled in http://www.novopos.ch/client/EPSON/TM-T20/TM-T20_eng_qr.pdf
-NUL = b'\x00'
-EOT = b'\x04'
-ENQ = b'\x05'
-DLE = b'\x10'
-DC4 = b'\x14'
-CAN = b'\x18'
-ESC = b'\x1b'
-FS  = b'\x1c'
-GS  = b'\x1d'
+# as labelled in https://www.novopos.ch/client/EPSON/TM-T20/TM-T20_eng_qr.pdf
+NUL = b"\x00"
+EOT = b"\x04"
+ENQ = b"\x05"
+DLE = b"\x10"
+DC4 = b"\x14"
+CAN = b"\x18"
+ESC = b"\x1b"
+FS = b"\x1c"
+GS = b"\x1d"
 
 # Feed control sequences
-CTL_LF = b'\n'              # Print and line feed
-CTL_FF = b'\f'              # Form feed
-CTL_CR = b'\r'              # Carriage return
-CTL_HT = b'\t'              # Horizontal tab
-CTL_SET_HT = ESC + b'\x44'  # Set horizontal tab positions
-CTL_VT = b'\v'              # Vertical tab
+CTL_LF = b"\n"  # Print and line feed
+CTL_FF = b"\f"  # Form feed
+CTL_CR = b"\r"  # Carriage return
+CTL_HT = b"\t"  # Horizontal tab
+CTL_SET_HT = ESC + b"\x44"  # Set horizontal tab positions
+CTL_VT = b"\v"  # Vertical tab
 
 # Printer hardware
-HW_INIT   = ESC + b'@'             # Clear data in buffer and reset modes
-HW_SELECT = ESC + b'=\x01'         # Printer select
+HW_INIT = ESC + b"@"  # Clear data in buffer and reset modes
+HW_SELECT = ESC + b"=\x01"  # Printer select
 
-HW_RESET  = ESC + b'\x3f\x0a\x00'   # Reset printer hardware
-                                    # (TODO: Where is this specified?)
+HW_RESET = ESC + b"\x3f\x0a\x00"  # Reset printer hardware
+# (TODO: Where is this specified?)
 
 # Cash Drawer (ESC p <pin> <on time: 2*ms> <off time: 2*ms>)
-_CASH_DRAWER = lambda m, t1='', t2='': ESC + b'p' + m + six.int2byte(t1) + six.int2byte(t2)
-CD_KICK_DEC_SEQUENCE = lambda esc, p, m, t1=50, t2=50: six.int2byte(esc) + six.int2byte(p) + six.int2byte(m) + six.int2byte(t1) + six.int2byte(t2)
-CD_KICK_2 = _CASH_DRAWER(b'\x00', 50, 50)  # Sends a pulse to pin 2 []
-CD_KICK_5 = _CASH_DRAWER(b'\x01', 50, 50)  # Sends a pulse to pin 5 []
+_CASH_DRAWER = (
+    lambda m, t1="", t2="": ESC + b"p" + m + six.int2byte(t1) + six.int2byte(t2)
+)
+CD_KICK_DEC_SEQUENCE = (
+    lambda esc, p, m, t1=50, t2=50: six.int2byte(esc)
+    + six.int2byte(p)
+    + six.int2byte(m)
+    + six.int2byte(t1)
+    + six.int2byte(t2)
+)
+CD_KICK_2 = _CASH_DRAWER(b"\x00", 50, 50)  # Sends a pulse to pin 2 []
+CD_KICK_5 = _CASH_DRAWER(b"\x01", 50, 50)  # Sends a pulse to pin 5 []
 
 # Paper Cutter
-_CUT_PAPER = lambda m: GS + b'V' + m
-PAPER_FULL_CUT = _CUT_PAPER(b'\x00')  # Full cut paper
-PAPER_PART_CUT = _CUT_PAPER(b'\x01')  # Partial cut paper
+_CUT_PAPER = lambda m: GS + b"V" + m
+PAPER_FULL_CUT = _CUT_PAPER(b"\x00")  # Full cut paper
+PAPER_PART_CUT = _CUT_PAPER(b"\x01")  # Partial cut paper
 
-# Beep
-BEEP = b'\x07'
+# Beep (please note that the actual beep sequence may differ between devices)
+BEEP = b"\x07"
 
 # Panel buttons (e.g. the FEED button)
-_PANEL_BUTTON = lambda n: ESC + b'c5' + six.int2byte(n)
+_PANEL_BUTTON = lambda n: ESC + b"c5" + six.int2byte(n)
 PANEL_BUTTON_ON = _PANEL_BUTTON(0)  # enable all panel buttons
 PANEL_BUTTON_OFF = _PANEL_BUTTON(1)  # disable all panel buttons
 
 # Line display printing
-LINE_DISPLAY_OPEN = ESC + b'\x3d\x02'
-LINE_DISPLAY_CLEAR = ESC + b'\x40'
-LINE_DISPLAY_CLOSE = ESC + b'\x3d\x01'
+LINE_DISPLAY_OPEN = ESC + b"\x3d\x02"
+LINE_DISPLAY_CLEAR = ESC + b"\x40"
+LINE_DISPLAY_CLOSE = ESC + b"\x3d\x01"
 
 # Sheet modes
-SHEET_SLIP_MODE = ESC + b'\x63\x30\x04'  # slip paper
-SHEET_ROLL_MODE = ESC + b'\x63\x30\x01'  # paper roll
+SHEET_SLIP_MODE = ESC + b"\x63\x30\x04"  # slip paper
+SHEET_ROLL_MODE = ESC + b"\x63\x30\x01"  # paper roll
+
+# Slip specific codes
+SLIP_EJECT = ESC + b"\x4b\xc0"  # Eject the slip or cheque
+SLIP_SELECT = FS  # Select the slip station as default station
+SLIP_SET_WAIT_TIME = (
+    ESC + b"\x1b\x66"
+)  # Set timeout waiting for a slip/cheque to be inserted
+SLIP_PRINT_AND_EJECT = (
+    b"\x0c"  # Print the buffer and eject (after waiting for the paper to be inserted)
+)
 
 # Text format
 # TODO: Acquire the "ESC/POS Application Programming Guide for Paper Roll
 #       Printers" and tidy up this stuff too.
-TXT_SIZE       = GS + b'!'
+TXT_SIZE = GS + b"!"
 
-TXT_NORMAL     = ESC + b'!\x00'     # Normal text
+TXT_NORMAL = ESC + b"!\x00"  # Normal text
 
 
 TXT_STYLE = {
-    'bold': {
-        False: ESC + b'\x45\x00',               # Bold font OFF
-        True: ESC + b'\x45\x01'                 # Bold font ON
-    },
-    'underline': {
-        0: ESC + b'\x2d\x00',                   # Underline font OFF
-        1: ESC + b'\x2d\x01',                   # Underline font 1-dot ON
-        2: ESC + b'\x2d\x02'                    # Underline font 2-dot ON
-    },
-    'size': {
-        'normal': TXT_NORMAL + ESC + b'!\x00',  # Normal text
-        '2h': TXT_NORMAL + ESC + b'!\x10',      # Double height text
-        '2w': TXT_NORMAL + ESC + b'!\x20',      # Double width text
-        '2x': TXT_NORMAL + ESC + b'!\x30'       # Quad area text
-    },
-    'font': {
-        'a': ESC + b'\x4d\x00',                 # Font type A
-        'b': ESC + b'\x4d\x00'                  # Font type B
-    },
-    'align': {
-        'left': ESC + b'\x61\x00',              # Left justification
-        'center': ESC + b'\x61\x01',            # Centering
-        'right': ESC + b'\x61\x02'              # Right justification
-    },
-    'invert': {
-        True: GS  + b'\x42\x01',                # Inverse Printing ON
-        False: GS  + b'\x42\x00'                # Inverse Printing OFF
-    },
-    'color': {
-        'black': ESC + b'\x72\x00',             # Default Color
-        'red': ESC + b'\x72\x01'                # Alternative Color, Usually Red
-    },
-    'flip': {
-        True: ESC + b'\x7b\x01',                # Flip ON
-        False: ESC + b'\x7b\x00'                # Flip OFF
-    },
-    'density': {
-        0: GS + b'\x7c\x00',                    # Printing Density -50%
-        1: GS + b'\x7c\x01',                    # Printing Density -37.5%
-        2: GS + b'\x7c\x02',                    # Printing Density -25%
-        3: GS + b'\x7c\x03',                    # Printing Density -12.5%
-        4: GS + b'\x7c\x04',                    # Printing Density  0%
-        5: GS + b'\x7c\x08',                    # Printing Density +50%
-        6: GS + b'\x7c\x07',                    # Printing Density +37.5%
-        7: GS + b'\x7c\x06',                    # Printing Density +25%
-        8: GS + b'\x7c\x05'                     # Printing Density +12.5%
-    },
-    'smooth': {
-        True: GS + b'\x62\x01',                 # Smooth ON
-        False: GS + b'\x62\x00'                 # Smooth OFF
+    "bold": {
+        False: ESC + b"\x45\x00",  # Bold font OFF
+        True: ESC + b"\x45\x01",  # Bold font ON
+    },
+    "underline": {
+        0: ESC + b"\x2d\x00",  # Underline font OFF
+        1: ESC + b"\x2d\x01",  # Underline font 1-dot ON
+        2: ESC + b"\x2d\x02",  # Underline font 2-dot ON
+    },
+    "size": {
+        "normal": TXT_NORMAL + ESC + b"!\x00",  # Normal text
+        "2h": TXT_NORMAL + ESC + b"!\x10",  # Double height text
+        "2w": TXT_NORMAL + ESC + b"!\x20",  # Double width text
+        "2x": TXT_NORMAL + ESC + b"!\x30",  # Quad area text
+    },
+    "font": {
+        "a": ESC + b"\x4d\x00",  # Font type A
+        "b": ESC + b"\x4d\x00",  # Font type B
+    },
+    "align": {
+        "left": ESC + b"\x61\x00",  # Left justification
+        "center": ESC + b"\x61\x01",  # Centering
+        "right": ESC + b"\x61\x02",  # Right justification
+    },
+    "invert": {
+        True: GS + b"\x42\x01",  # Inverse Printing ON
+        False: GS + b"\x42\x00",  # Inverse Printing OFF
+    },
+    "color": {
+        "black": ESC + b"\x72\x00",  # Default Color
+        "red": ESC + b"\x72\x01",  # Alternative Color, Usually Red
+    },
+    "flip": {True: ESC + b"\x7b\x01", False: ESC + b"\x7b\x00"},  # Flip ON  # Flip OFF
+    "density": {
+        0: GS + b"\x7c\x00",  # Printing Density -50%
+        1: GS + b"\x7c\x01",  # Printing Density -37.5%
+        2: GS + b"\x7c\x02",  # Printing Density -25%
+        3: GS + b"\x7c\x03",  # Printing Density -12.5%
+        4: GS + b"\x7c\x04",  # Printing Density  0%
+        5: GS + b"\x7c\x08",  # Printing Density +50%
+        6: GS + b"\x7c\x07",  # Printing Density +37.5%
+        7: GS + b"\x7c\x06",  # Printing Density +25%
+        8: GS + b"\x7c\x05",  # Printing Density +12.5%
+    },
+    "smooth": {
+        True: GS + b"\x62\x01",  # Smooth ON
+        False: GS + b"\x62\x00",  # Smooth OFF
     },
-    'height': {                                 # Custom text height
+    "height": {  # Custom text height
         1: 0x00,
         2: 0x01,
         3: 0x02,
         4: 0x03,
         5: 0x04,
         6: 0x05,
         7: 0x06,
-        8: 0x07
+        8: 0x07,
     },
-    'width': {                                  # Custom text width
+    "width": {  # Custom text width
         1: 0x00,
         2: 0x10,
         3: 0x20,
         4: 0x30,
         5: 0x40,
         6: 0x50,
         7: 0x60,
-        8: 0x70
-    }
+        8: 0x70,
+    },
 }
 
 # Fonts
-SET_FONT = lambda n: ESC + b'\x4d' + n
-TXT_FONT_A     = SET_FONT(b'\x00')  # Font type A
-TXT_FONT_B     = SET_FONT(b'\x01')  # Font type B
+SET_FONT = lambda n: ESC + b"\x4d" + n
+TXT_FONT_A = SET_FONT(b"\x00")  # Font type A
+TXT_FONT_B = SET_FONT(b"\x01")  # Font type B
 
 # Spacing
-LINESPACING_RESET = ESC + b'2'
+LINESPACING_RESET = ESC + b"2"
 LINESPACING_FUNCS = {
-  60: ESC + b'A',  # line_spacing/60 of an inch, 0 <= line_spacing <= 85
-  360: ESC + b'+', # line_spacing/360 of an inch, 0 <= line_spacing <= 255
-  180: ESC + b'3', # line_spacing/180 of an inch, 0 <= line_spacing <= 255
+    60: ESC + b"A",  # line_spacing/60 of an inch, 0 <= line_spacing <= 85
+    360: ESC + b"+",  # line_spacing/360 of an inch, 0 <= line_spacing <= 255
+    180: ESC + b"3",  # line_spacing/180 of an inch, 0 <= line_spacing <= 255
 }
 
 # Prefix to change the codepage. You need to attach a byte to indicate
 # the codepage to use. We use escpos-printer-db as the data source.
-CODEPAGE_CHANGE = ESC + b'\x74'
+CODEPAGE_CHANGE = ESC + b"\x74"
 
 # Barcode format
-_SET_BARCODE_TXT_POS = lambda n: GS + b'H' + n
-BARCODE_TXT_OFF = _SET_BARCODE_TXT_POS(b'\x00')  # HRI barcode chars OFF
-BARCODE_TXT_ABV = _SET_BARCODE_TXT_POS(b'\x01')  # HRI barcode chars above
-BARCODE_TXT_BLW = _SET_BARCODE_TXT_POS(b'\x02')  # HRI barcode chars below
-BARCODE_TXT_BTH = _SET_BARCODE_TXT_POS(b'\x03')  # HRI both above and below
-
-_SET_HRI_FONT = lambda n: GS + b'f' + n
-BARCODE_FONT_A = _SET_HRI_FONT(b'\x00')  # Font type A for HRI barcode chars
-BARCODE_FONT_B = _SET_HRI_FONT(b'\x01')  # Font type B for HRI barcode chars
+_SET_BARCODE_TXT_POS = lambda n: GS + b"H" + n
+BARCODE_TXT_OFF = _SET_BARCODE_TXT_POS(b"\x00")  # HRI barcode chars OFF
+BARCODE_TXT_ABV = _SET_BARCODE_TXT_POS(b"\x01")  # HRI barcode chars above
+BARCODE_TXT_BLW = _SET_BARCODE_TXT_POS(b"\x02")  # HRI barcode chars below
+BARCODE_TXT_BTH = _SET_BARCODE_TXT_POS(b"\x03")  # HRI both above and below
+
+_SET_HRI_FONT = lambda n: GS + b"f" + n
+BARCODE_FONT_A = _SET_HRI_FONT(b"\x00")  # Font type A for HRI barcode chars
+BARCODE_FONT_B = _SET_HRI_FONT(b"\x01")  # Font type B for HRI barcode chars
 
-BARCODE_HEIGHT = GS + b'h'  # Barcode Height [1-255]
-BARCODE_WIDTH  = GS + b'w'  # Barcode Width  [2-6]
+BARCODE_HEIGHT = GS + b"h"  # Barcode Height [1-255]
+BARCODE_WIDTH = GS + b"w"  # Barcode Width  [2-6]
 
 # NOTE: This isn't actually an ESC/POS command. It's the common prefix to the
 #      two "print bar code" commands:
 #      -  Type A: "GS k <type as integer> <data> NUL"
 #      -  TYPE B: "GS k <type as letter> <data length> <data>"
 #      The latter command supports more barcode types
-_SET_BARCODE_TYPE = lambda m: GS + b'k' + six.int2byte(m)
+_SET_BARCODE_TYPE = lambda m: GS + b"k" + six.int2byte(m)
 
 # Barcodes for printing function type A
 BARCODE_TYPE_A = {
-    'UPC-A':   _SET_BARCODE_TYPE(0),
-    'UPC-E':   _SET_BARCODE_TYPE(1),
-    'EAN13':   _SET_BARCODE_TYPE(2),
-    'EAN8':    _SET_BARCODE_TYPE(3),
-    'CODE39':  _SET_BARCODE_TYPE(4),
-    'ITF':     _SET_BARCODE_TYPE(5),
-    'NW7':     _SET_BARCODE_TYPE(6),
-    'CODABAR': _SET_BARCODE_TYPE(6),  # Same as NW7
+    "UPC-A": _SET_BARCODE_TYPE(0),
+    "UPC-E": _SET_BARCODE_TYPE(1),
+    "EAN13": _SET_BARCODE_TYPE(2),
+    "EAN8": _SET_BARCODE_TYPE(3),
+    "CODE39": _SET_BARCODE_TYPE(4),
+    "ITF": _SET_BARCODE_TYPE(5),
+    "NW7": _SET_BARCODE_TYPE(6),
+    "CODABAR": _SET_BARCODE_TYPE(6),  # Same as NW7
 }
 
 # Barcodes for printing function type B
 # The first 8 are the same barcodes as type A
 BARCODE_TYPE_B = {
-    'UPC-A':                       _SET_BARCODE_TYPE(65),
-    'UPC-E':                       _SET_BARCODE_TYPE(66),
-    'EAN13':                       _SET_BARCODE_TYPE(67),
-    'EAN8':                        _SET_BARCODE_TYPE(68),
-    'CODE39':                      _SET_BARCODE_TYPE(69),
-    'ITF':                         _SET_BARCODE_TYPE(70),
-    'NW7':                         _SET_BARCODE_TYPE(71),
-    'CODABAR':                     _SET_BARCODE_TYPE(71),  # Same as NW7
-    'CODE93':                      _SET_BARCODE_TYPE(72),
-    'CODE128':                     _SET_BARCODE_TYPE(73),
-    'GS1-128':                     _SET_BARCODE_TYPE(74),
-    'GS1 DATABAR OMNIDIRECTIONAL': _SET_BARCODE_TYPE(75),
-    'GS1 DATABAR TRUNCATED':       _SET_BARCODE_TYPE(76),
-    'GS1 DATABAR LIMITED':         _SET_BARCODE_TYPE(77),
-    'GS1 DATABAR EXPANDED':        _SET_BARCODE_TYPE(78),
+    "UPC-A": _SET_BARCODE_TYPE(65),
+    "UPC-E": _SET_BARCODE_TYPE(66),
+    "EAN13": _SET_BARCODE_TYPE(67),
+    "EAN8": _SET_BARCODE_TYPE(68),
+    "CODE39": _SET_BARCODE_TYPE(69),
+    "ITF": _SET_BARCODE_TYPE(70),
+    "NW7": _SET_BARCODE_TYPE(71),
+    "CODABAR": _SET_BARCODE_TYPE(71),  # Same as NW7
+    "CODE93": _SET_BARCODE_TYPE(72),
+    "CODE128": _SET_BARCODE_TYPE(73),
+    "GS1-128": _SET_BARCODE_TYPE(74),
+    "GS1 DATABAR OMNIDIRECTIONAL": _SET_BARCODE_TYPE(75),
+    "GS1 DATABAR TRUNCATED": _SET_BARCODE_TYPE(76),
+    "GS1 DATABAR LIMITED": _SET_BARCODE_TYPE(77),
+    "GS1 DATABAR EXPANDED": _SET_BARCODE_TYPE(78),
 }
 
 BARCODE_FORMATS = {
-    'UPC-A':                       ([(11, 12)], "^[0-9]{11,12}$"),
-    'UPC-E':                       ([(7, 8), (11, 12)], "^([0-9]{7,8}|[0-9]{11,12})$"),
-    'EAN13':                       ([(12, 13)], "^[0-9]{12,13}$"),
-    'EAN8':                        ([(7, 8)], "^[0-9]{7,8}$"),
-    'CODE39':                      ([(1, 255)], "^([0-9A-Z \$\%\+\-\.\/]+|\*[0-9A-Z \$\%\+\-\.\/]+\*)$"),
-    'ITF':                         ([(2, 255)], "^([0-9]{2})+$"),
-    'NW7':                         ([(1, 255)], "^[A-Da-d][0-9\$\+\-\.\/\:]+[A-Da-d]$"),
-    'CODABAR':                     ([(1, 255)], "^[A-Da-d][0-9\$\+\-\.\/\:]+[A-Da-d]$"),  # Same as NW7
-    'CODE93':                      ([(1, 255)], "^[\\x00-\\x7F]+$"),
-    'CODE128':                     ([(2, 255)], "^\{[A-C][\\x00-\\x7F]+$"),
-    'GS1-128':                     ([(2, 255)], "^\{[A-C][\\x00-\\x7F]+$"), # same as CODE128
-    'GS1 DATABAR OMNIDIRECTIONAL': ([(13,13)], "^[0-9]{13}$"),
-    'GS1 DATABAR TRUNCATED':       ([(13,13)], "^[0-9]{13}$"), # same as GS1 omnidirectional
-    'GS1 DATABAR LIMITED':         ([(13,13)], "^[01][0-9]{12}$"),
-    'GS1 DATABAR EXPANDED':        ([(2,255)], "^\([0-9][A-Za-z0-9 \!\"\%\&\'\(\)\*\+\,\-\.\/\:\;\<\=\>\?\_\{]+$"),
+    "UPC-A": ([(11, 12)], "^[0-9]{11,12}$"),
+    "UPC-E": ([(7, 8), (11, 12)], "^([0-9]{7,8}|[0-9]{11,12})$"),
+    "EAN13": ([(12, 13)], "^[0-9]{12,13}$"),
+    "EAN8": ([(7, 8)], "^[0-9]{7,8}$"),
+    "CODE39": ([(1, 255)], "^([0-9A-Z \$\%\+\-\.\/]+|\*[0-9A-Z \$\%\+\-\.\/]+\*)$"),
+    "ITF": ([(2, 255)], "^([0-9]{2})+$"),
+    "NW7": ([(1, 255)], "^[A-Da-d][0-9\$\+\-\.\/\:]+[A-Da-d]$"),
+    "CODABAR": ([(1, 255)], "^[A-Da-d][0-9\$\+\-\.\/\:]+[A-Da-d]$"),  # Same as NW7
+    "CODE93": ([(1, 255)], "^[\\x00-\\x7F]+$"),
+    "CODE128": ([(2, 255)], "^\{[A-C][\\x00-\\x7F]+$"),
+    "GS1-128": ([(2, 255)], "^\{[A-C][\\x00-\\x7F]+$"),  # same as CODE128
+    "GS1 DATABAR OMNIDIRECTIONAL": ([(13, 13)], "^[0-9]{13}$"),
+    "GS1 DATABAR TRUNCATED": ([(13, 13)], "^[0-9]{13}$"),  # same as GS1 omnidirectional
+    "GS1 DATABAR LIMITED": ([(13, 13)], "^[01][0-9]{12}$"),
+    "GS1 DATABAR EXPANDED": (
+        [(2, 255)],
+        "^\([0-9][A-Za-z0-9 \!\"\%\&'\(\)\*\+\,\-\.\/\:\;\<\=\>\?\_\{]+$",
+    ),
 }
 
 BARCODE_TYPES = {
-    'A': BARCODE_TYPE_A,
-    'B': BARCODE_TYPE_B,
+    "A": BARCODE_TYPE_A,
+    "B": BARCODE_TYPE_B,
 }
 
 # QRCode error correction levels
 QR_ECLEVEL_L = 0
 QR_ECLEVEL_M = 1
 QR_ECLEVEL_Q = 2
 QR_ECLEVEL_H = 3
@@ -254,21 +272,21 @@
 QR_MODEL_1 = 1
 QR_MODEL_2 = 2
 QR_MICRO = 3
 
 # Image format
 # NOTE: _PRINT_RASTER_IMG is the obsolete ESC/POS "print raster bit image"
 #       command. The constants include a fragment of the data's header.
-_PRINT_RASTER_IMG = lambda data: GS + b'v0' + data
-S_RASTER_N  = _PRINT_RASTER_IMG(b'\x00')  # Set raster image normal size
-S_RASTER_2W = _PRINT_RASTER_IMG(b'\x01')  # Set raster image double width
-S_RASTER_2H = _PRINT_RASTER_IMG(b'\x02')  # Set raster image double height
-S_RASTER_Q  = _PRINT_RASTER_IMG(b'\x03')  # Set raster image quadruple
+_PRINT_RASTER_IMG = lambda data: GS + b"v0" + data
+S_RASTER_N = _PRINT_RASTER_IMG(b"\x00")  # Set raster image normal size
+S_RASTER_2W = _PRINT_RASTER_IMG(b"\x01")  # Set raster image double width
+S_RASTER_2H = _PRINT_RASTER_IMG(b"\x02")  # Set raster image double height
+S_RASTER_Q = _PRINT_RASTER_IMG(b"\x03")  # Set raster image quadruple
 
 # Status Command
 RT_STATUS = DLE + EOT
-RT_STATUS_ONLINE = RT_STATUS +  b'\x01'
-RT_STATUS_PAPER = RT_STATUS +  b'\x04'
+RT_STATUS_ONLINE = RT_STATUS + b"\x01"
+RT_STATUS_PAPER = RT_STATUS + b"\x04"
 RT_MASK_ONLINE = 8
 RT_MASK_PAPER = 18
 RT_MASK_LOWPAPER = 30
-RT_MASK_NOPAPER = 114
+RT_MASK_NOPAPER = 114
```

### Comparing `python-escpos-3.0a8/src/escpos/escpos.py` & `python-escpos-3.0a9/src/escpos/escpos.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,25 +18,64 @@
 from re import match as re_match
 
 import barcode
 from barcode.writer import ImageWriter
 
 import os
 
-from .constants import ESC, GS, NUL, QR_ECLEVEL_L, QR_ECLEVEL_M, QR_ECLEVEL_H, QR_ECLEVEL_Q
-from .constants import QR_MODEL_1, QR_MODEL_2, QR_MICRO, BARCODE_TYPES, BARCODE_HEIGHT, BARCODE_WIDTH
+from .constants import (
+    ESC,
+    GS,
+    NUL,
+    QR_ECLEVEL_L,
+    QR_ECLEVEL_M,
+    QR_ECLEVEL_H,
+    QR_ECLEVEL_Q,
+    SHEET_ROLL_MODE,
+    SHEET_SLIP_MODE,
+    SLIP_PRINT_AND_EJECT,
+    SLIP_SELECT,
+    SLIP_EJECT,
+)
+from .constants import (
+    QR_MODEL_1,
+    QR_MODEL_2,
+    QR_MICRO,
+    BARCODE_TYPES,
+    BARCODE_HEIGHT,
+    BARCODE_WIDTH,
+)
 from .constants import BARCODE_FONT_A, BARCODE_FONT_B, BARCODE_FORMATS
-from .constants import BARCODE_TXT_OFF, BARCODE_TXT_BTH, BARCODE_TXT_ABV, BARCODE_TXT_BLW
+from .constants import (
+    BARCODE_TXT_OFF,
+    BARCODE_TXT_BTH,
+    BARCODE_TXT_ABV,
+    BARCODE_TXT_BLW,
+)
 from .constants import TXT_SIZE, TXT_NORMAL
 from .constants import SET_FONT
 from .constants import LINESPACING_FUNCS, LINESPACING_RESET
 from .constants import LINE_DISPLAY_OPEN, LINE_DISPLAY_CLEAR, LINE_DISPLAY_CLOSE
-from .constants import CD_KICK_DEC_SEQUENCE, CD_KICK_5, CD_KICK_2, PAPER_FULL_CUT, PAPER_PART_CUT
+from .constants import (
+    CD_KICK_DEC_SEQUENCE,
+    CD_KICK_5,
+    CD_KICK_2,
+    PAPER_FULL_CUT,
+    PAPER_PART_CUT,
+)
 from .constants import HW_RESET, HW_SELECT, HW_INIT
-from .constants import CTL_VT, CTL_CR, CTL_FF, CTL_LF, CTL_SET_HT, PANEL_BUTTON_OFF, PANEL_BUTTON_ON
+from .constants import (
+    CTL_VT,
+    CTL_CR,
+    CTL_FF,
+    CTL_LF,
+    CTL_SET_HT,
+    PANEL_BUTTON_OFF,
+    PANEL_BUTTON_ON,
+)
 from .constants import TXT_STYLE
 from .constants import RT_STATUS_ONLINE, RT_MASK_ONLINE
 from .constants import RT_STATUS_PAPER, RT_MASK_PAPER, RT_MASK_LOWPAPER, RT_MASK_NOPAPER
 
 from .exceptions import BarcodeTypeError, BarcodeSizeError, TabPosError
 from .exceptions import CashDrawerError, SetVariableError, BarcodeCodeError
 from .exceptions import ImageWidthError
@@ -46,52 +85,60 @@
 from abc import ABCMeta, abstractmethod  # abstract base class support
 from escpos.image import EscposImage
 from escpos.capabilities import get_profile, BARCODE_B
 
 
 @six.add_metaclass(ABCMeta)
 class Escpos(object):
-    """ ESC/POS Printer object
+    """ESC/POS Printer object
 
     This class is the abstract base class for an esc/pos-printer. The printer implementations are children of this
     class.
     """
+
     device = None
 
     def __init__(self, profile=None, magic_encode_args=None, **kwargs):
-        """ Initialize ESCPOS Printer
+        """Initialize ESCPOS Printer
 
         :param profile: Printer profile"""
         self.profile = get_profile(profile)
         self.magic = MagicEncode(self, **(magic_encode_args or {}))
 
     def __del__(self):
-        """ call self.close upon deletion """
+        """call self.close upon deletion"""
         self.close()
 
     @abstractmethod
     def _raw(self, msg):
-        """ Sends raw data to the printer
+        """Sends raw data to the printer
 
         This function has to be individually implemented by the implementations.
 
         :param msg: message string to be sent to the printer
         :type msg: bytes
         """
         pass
 
     def _read(self):
-        """ Returns a NotImplementedError if the instance of the class doesn't override this method.
+        """Returns a NotImplementedError if the instance of the class doesn't override this method.
         :raises NotImplementedError
         """
         raise NotImplementedError()
 
-    def image(self, img_source, high_density_vertical=True, high_density_horizontal=True, impl="bitImageRaster",
-              fragment_height=960, center=False):
-        """ Print an image
+    def image(
+        self,
+        img_source,
+        high_density_vertical=True,
+        high_density_horizontal=True,
+        impl="bitImageRaster",
+        fragment_height=960,
+        center=False,
+    ):
+        """Print an image
 
         You can select whether the printer should print in high density or not. The default value is high density.
         When printing in low density, the image will be stretched.
 
         Esc/Pos supplies several commands for printing. This function supports three of them. Please try to vary the
         implementations if you have any problems. For example the printer `IT80-002` will have trouble aligning
         images that are not printed in Column-mode.
@@ -112,85 +159,113 @@
         :param fragment_height: Images larger than this will be split into multiple fragments *default:* 960
         :param center: Center image horizontally *default:* False
 
         """
         im = EscposImage(img_source)
 
         try:
-            if self.profile.profile_data['media']['width']['pixels'] == "Unknown":
-                print("The media.width.pixel field of the printer profile is not set. " +
-                      "The center flag will have no effect.")
+            if self.profile.profile_data["media"]["width"]["pixels"] == "Unknown":
+                print(
+                    "The media.width.pixel field of the printer profile is not set. "
+                    + "The center flag will have no effect."
+                )
 
-            max_width = int(self.profile.profile_data['media']['width']['pixels'])
+            max_width = int(self.profile.profile_data["media"]["width"]["pixels"])
 
             if im.width > max_width:
-                raise ImageWidthError('{} > {}'.format(im.width, max_width))
+                raise ImageWidthError("{} > {}".format(im.width, max_width))
 
             if center:
                 im.center(max_width)
         except KeyError:
             # If the printer's pixel width is not known, print anyways...
             pass
         except ValueError:
             # If the max_width cannot be converted to an int, print anyways...
             pass
 
         if im.height > fragment_height:
             fragments = im.split(fragment_height)
             for fragment in fragments:
-                self.image(fragment,
-                           high_density_vertical=high_density_vertical,
-                           high_density_horizontal=high_density_horizontal,
-                           impl=impl,
-                           fragment_height=fragment_height)
+                self.image(
+                    fragment,
+                    high_density_vertical=high_density_vertical,
+                    high_density_horizontal=high_density_horizontal,
+                    impl=impl,
+                    fragment_height=fragment_height,
+                )
             return
 
         if impl == "bitImageRaster":
             # GS v 0, raster format bit image
-            density_byte = (0 if high_density_horizontal else 1) + (0 if high_density_vertical else 2)
-            header = GS + b"v0" + six.int2byte(density_byte) + self._int_low_high(im.width_bytes, 2) +\
-                self._int_low_high(im.height, 2)
+            density_byte = (0 if high_density_horizontal else 1) + (
+                0 if high_density_vertical else 2
+            )
+            header = (
+                GS
+                + b"v0"
+                + six.int2byte(density_byte)
+                + self._int_low_high(im.width_bytes, 2)
+                + self._int_low_high(im.height, 2)
+            )
             self._raw(header + im.to_raster_format())
 
         if impl == "graphics":
             # GS ( L raster format graphics
-            img_header = self._int_low_high(im.width, 2) + self._int_low_high(im.height, 2)
-            tone = b'0'
-            colors = b'1'
+            img_header = self._int_low_high(im.width, 2) + self._int_low_high(
+                im.height, 2
+            )
+            tone = b"0"
+            colors = b"1"
             ym = six.int2byte(1 if high_density_vertical else 2)
             xm = six.int2byte(1 if high_density_horizontal else 2)
             header = tone + xm + ym + colors + img_header
             raster_data = im.to_raster_format()
-            self._image_send_graphics_data(b'0', b'p', header + raster_data)
-            self._image_send_graphics_data(b'0', b'2', b'')
+            self._image_send_graphics_data(b"0", b"p", header + raster_data)
+            self._image_send_graphics_data(b"0", b"2", b"")
 
         if impl == "bitImageColumn":
             # ESC *, column format bit image
-            density_byte = (1 if high_density_horizontal else 0) + (32 if high_density_vertical else 0)
-            header = ESC + b"*" + six.int2byte(density_byte) + self._int_low_high(im.width, 2)
+            density_byte = (1 if high_density_horizontal else 0) + (
+                32 if high_density_vertical else 0
+            )
+            header = (
+                ESC
+                + b"*"
+                + six.int2byte(density_byte)
+                + self._int_low_high(im.width, 2)
+            )
             outp = [ESC + b"3" + six.int2byte(16)]  # Adjust line-feed size
             for blob in im.to_column_format(high_density_vertical):
                 outp.append(header + blob + b"\n")
             outp.append(ESC + b"2")  # Reset line-feed size
-            self._raw(b''.join(outp))
+            self._raw(b"".join(outp))
 
     def _image_send_graphics_data(self, m, fn, data):
         """
         Wrapper for GS ( L, to calculate and send correct data length.
 
         :param m: Modifier//variant for function. Usually '0'
         :param fn: Function number to use, as byte
         :param data: Data to send
         """
         header = self._int_low_high(len(data) + 2, 2)
-        self._raw(GS + b'(L' + header + m + fn + data)
+        self._raw(GS + b"(L" + header + m + fn + data)
 
-    def qr(self, content, ec=QR_ECLEVEL_L, size=3, model=QR_MODEL_2,
-           native=False, center=False, impl="bitImageRaster"):
-        """ Print QR Code for the provided string
+    def qr(
+        self,
+        content,
+        ec=QR_ECLEVEL_L,
+        size=3,
+        model=QR_MODEL_2,
+        native=False,
+        center=False,
+        impl="bitImageRaster",
+    ):
+        """Print QR Code for the provided string
 
         :param content: The content of the code. Numeric data will be more efficiently compacted.
         :param ec: Error-correction level to use. One of QR_ECLEVEL_L (default), QR_ECLEVEL_M, QR_ECLEVEL_Q or
             QR_ECLEVEL_H.
             Higher error correction results in a less compact code.
         :param size: Pixel size to use. Must be 1-16 (default 3)
         :param model: QR code model to use. Must be one of QR_MODEL_1, QR_MODEL_2 (default) or QR_MICRO (not supported
@@ -202,89 +277,103 @@
         """
         # Basic validation
         if ec not in [QR_ECLEVEL_L, QR_ECLEVEL_M, QR_ECLEVEL_H, QR_ECLEVEL_Q]:
             raise ValueError("Invalid error correction level")
         if not 1 <= size <= 16:
             raise ValueError("Invalid block size (must be 1-16)")
         if model not in [QR_MODEL_1, QR_MODEL_2, QR_MICRO]:
-            raise ValueError("Invalid QR model (must be one of QR_MODEL_1, QR_MODEL_2, QR_MICRO)")
+            raise ValueError(
+                "Invalid QR model (must be one of QR_MODEL_1, QR_MODEL_2, QR_MICRO)"
+            )
         if content == "":
             # Handle edge case by printing nothing.
             return
         if not native:
             # Map ESC/POS error correction levels to python 'qrcode' library constant and render to an image
             if model != QR_MODEL_2:
-                raise ValueError("Invalid QR model for qrlib rendering (must be QR_MODEL_2)")
+                raise ValueError(
+                    "Invalid QR model for qrlib rendering (must be QR_MODEL_2)"
+                )
             python_qr_ec = {
                 QR_ECLEVEL_H: qrcode.constants.ERROR_CORRECT_H,
                 QR_ECLEVEL_L: qrcode.constants.ERROR_CORRECT_L,
                 QR_ECLEVEL_M: qrcode.constants.ERROR_CORRECT_M,
-                QR_ECLEVEL_Q: qrcode.constants.ERROR_CORRECT_Q
+                QR_ECLEVEL_Q: qrcode.constants.ERROR_CORRECT_Q,
             }
-            qr_code = qrcode.QRCode(version=None, box_size=size, border=1, error_correction=python_qr_ec[ec])
+            qr_code = qrcode.QRCode(
+                version=None, box_size=size, border=1, error_correction=python_qr_ec[ec]
+            )
             qr_code.add_data(content)
             qr_code.make(fit=True)
             qr_img = qr_code.make_image()
             im = qr_img._img.convert("RGB")
 
             # Convert the RGB image in printable image
-            self.text('\n')
+            self.text("\n")
             self.image(im, center=center, impl=impl)
-            self.text('\n')
-            self.text('\n')
+            self.text("\n")
+            self.text("\n")
             return
 
         if center:
-            raise NotImplementedError("Centering not implemented for native QR rendering")
+            raise NotImplementedError(
+                "Centering not implemented for native QR rendering"
+            )
 
         # Native 2D code printing
-        cn = b'1'  # Code type for QR code
+        cn = b"1"  # Code type for QR code
         # Select model: 1, 2 or micro.
-        self._send_2d_code_data(six.int2byte(65), cn, six.int2byte(48 + model) + six.int2byte(0))
+        self._send_2d_code_data(
+            six.int2byte(65), cn, six.int2byte(48 + model) + six.int2byte(0)
+        )
         # Set dot size.
         self._send_2d_code_data(six.int2byte(67), cn, six.int2byte(size))
         # Set error correction level: L, M, Q, or H
         self._send_2d_code_data(six.int2byte(69), cn, six.int2byte(48 + ec))
         # Send content & print
-        self._send_2d_code_data(six.int2byte(80), cn, content.encode('utf-8'), b'0')
-        self._send_2d_code_data(six.int2byte(81), cn, b'', b'0')
+        self._send_2d_code_data(six.int2byte(80), cn, content.encode("utf-8"), b"0")
+        self._send_2d_code_data(six.int2byte(81), cn, b"", b"0")
 
-    def _send_2d_code_data(self, fn, cn, data, m=b''):
-        """ Wrapper for GS ( k, to calculate and send correct data length.
+    def _send_2d_code_data(self, fn, cn, data, m=b""):
+        """Wrapper for GS ( k, to calculate and send correct data length.
 
         :param fn: Function to use.
         :param cn: Output code type. Affects available data.
         :param data: Data to send.
         :param m: Modifier/variant for function. Often '0' where used.
         """
         if len(m) > 1 or len(cn) != 1 or len(fn) != 1:
             raise ValueError("cn and fn must be one byte each.")
         header = self._int_low_high(len(data) + len(m) + 2, 2)
-        self._raw(GS + b'(k' + header + cn + fn + m + data)
+        self._raw(GS + b"(k" + header + cn + fn + m + data)
 
     @staticmethod
     def _int_low_high(inp_number, out_bytes):
-        """ Generate multiple bytes for a number: In lower and higher parts, or more parts as needed.
+        """Generate multiple bytes for a number: In lower and higher parts, or more parts as needed.
 
         :param inp_number: Input number
         :param out_bytes: The number of bytes to output (1 - 4).
         """
-        max_input = (256 << (out_bytes * 8) - 1)
+        max_input = 256 << (out_bytes * 8) - 1
         if not 1 <= out_bytes <= 4:
             raise ValueError("Can only output 1-4 bytes")
         if not 0 <= inp_number <= max_input:
-            raise ValueError("Number too large. Can only output up to {0} in {1} bytes".format(max_input, out_bytes))
-        outp = b''
+            raise ValueError(
+                "Number too large. Can only output up to {0} in {1} bytes".format(
+                    max_input, out_bytes
+                )
+            )
+        outp = b""
         for _ in range(0, out_bytes):
             outp += six.int2byte(inp_number % 256)
             inp_number //= 256
         return outp
 
     def charcode(self, code="AUTO"):
-        """ Set Character Code Table
+        """Set Character Code Table
 
         Sets the control sequence from ``CHARCODE`` in :py:mod:`escpos.constants` as active. It will be sent with
         the next text sequence. If you set the variable code to ``AUTO`` it will try to automatically guess the
         right codepage. (This is the standard behaviour.)
 
         :param code: Name of CharCode
         :raises: :py:exc:`~escpos.exceptions.CharCodeError`
@@ -314,19 +403,31 @@
         :param code: alphanumeric data to be printed as bar code, see :py:meth:`.barcode()`
         :return: bool
         """
         if bc not in BARCODE_FORMATS:
             return False
 
         bounds, regex = BARCODE_FORMATS[bc]
-        return any(bound[0] <= len(code) <= bound[1] for bound in bounds) and re_match(regex, code)
-
-    def barcode(self, code, bc, height=64, width=3, pos="BELOW", font="A",
-                align_ct=True, function_type=None, check=True):
-        """ Print Barcode
+        return any(bound[0] <= len(code) <= bound[1] for bound in bounds) and re_match(
+            regex, code
+        )
+
+    def barcode(
+        self,
+        code,
+        bc,
+        height=64,
+        width=3,
+        pos="BELOW",
+        font="A",
+        align_ct=True,
+        function_type=None,
+        check=True,
+    ):
+        """Print Barcode
 
         This method allows to print barcodes. The rendering of the barcode is done by the printer and therefore has to
         be supported by the unit. By default, this method will check whether your barcode text is correct, that is
         the characters and lengths are supported by ESCPOS. Call the method with `check=False` to disable the check, but
         note that uncorrect barcodes may lead to unexpected printer behaviour.
         There are two forms of the barcode function. Type A is default but has fewer barcodes,
         while type B has some more to choose from.
@@ -403,46 +504,54 @@
 
         :raises: :py:exc:`~escpos.exceptions.BarcodeSizeError`,
                  :py:exc:`~escpos.exceptions.BarcodeTypeError`,
                  :py:exc:`~escpos.exceptions.BarcodeCodeError`
         """
         if function_type is None:
             # Choose the function type automatically.
-            if bc in BARCODE_TYPES['A']:
-                function_type = 'A'
+            if bc in BARCODE_TYPES["A"]:
+                function_type = "A"
             else:
-                if bc in BARCODE_TYPES['B']:
+                if bc in BARCODE_TYPES["B"]:
                     if not self.profile.supports(BARCODE_B):
-                        raise BarcodeTypeError((
-                            "Barcode type '{bc} not supported for "
-                            "the current printer profile").format(bc=bc))
-                    function_type = 'B'
+                        raise BarcodeTypeError(
+                            (
+                                "Barcode type '{bc} not supported for "
+                                "the current printer profile"
+                            ).format(bc=bc)
+                        )
+                    function_type = "B"
                 else:
-                    raise BarcodeTypeError((
-                        "Barcode type '{bc} is not valid").format(bc=bc))
+                    raise BarcodeTypeError(
+                        ("Barcode type '{bc} is not valid").format(bc=bc)
+                    )
 
         bc_types = BARCODE_TYPES[function_type.upper()]
         if bc.upper() not in bc_types.keys():
-            raise BarcodeTypeError((
-                "Barcode '{bc}' not valid for barcode function type "
-                "{function_type}").format(
+            raise BarcodeTypeError(
+                (
+                    "Barcode '{bc}' not valid for barcode function type "
+                    "{function_type}"
+                ).format(
                     bc=bc,
                     function_type=function_type,
-                ))
+                )
+            )
 
         if check and not self.check_barcode(bc, code):
-            raise BarcodeCodeError((
-                "Barcode '{code}' not in a valid format for type '{bc}'").format(
-                code=code,
-                bc=bc,
-            ))
+            raise BarcodeCodeError(
+                ("Barcode '{code}' not in a valid format for type '{bc}'").format(
+                    code=code,
+                    bc=bc,
+                )
+            )
 
         # Align Bar Code()
         if align_ct:
-            self._raw(TXT_STYLE['align']['center'])
+            self._raw(TXT_STYLE["align"]["center"])
         # Height
         if 1 <= height <= 255:
             self._raw(BARCODE_HEIGHT + six.int2byte(height))
         else:
             raise BarcodeSizeError("height = {height}".format(height=height))
         # Width
         if 2 <= width <= 6:
@@ -474,92 +583,113 @@
             self._raw(code.encode())
         else:
             raise BarcodeCodeError()
 
         if function_type.upper() == "A":
             self._raw(NUL)
 
-    def soft_barcode(self, barcode_type, data, impl='bitImageColumn',
-                     module_height=5, module_width=0.2, text_distance=1,
-                     center=True):
-
+    def soft_barcode(
+        self,
+        barcode_type,
+        data,
+        impl="bitImageColumn",
+        module_height=5,
+        module_width=0.2,
+        text_distance=1,
+        center=True,
+    ):
         image_writer = ImageWriter()
 
         # Check if barcode type exists
         if barcode_type not in barcode.PROVIDED_BARCODES:
             raise BarcodeTypeError(
-                'Barcode type {} not supported by software barcode renderer'
-                .format(barcode_type))
+                "Barcode type {} not supported by software barcode renderer".format(
+                    barcode_type
+                )
+            )
 
-        # Render the barcode to a fake file
+        # Render the barcode
         barcode_class = barcode.get_barcode_class(barcode_type)
         my_code = barcode_class(data, writer=image_writer)
-
-        with open(os.devnull, "wb") as nullfile:
-            my_code.write(nullfile, {
-                'module_height': module_height,
-                'module_width': module_width,
-                'text_distance': text_distance
-            })
+        my_code.render(
+            writer_options={
+                "module_height": module_height,
+                "module_width": module_width,
+                "text_distance": text_distance,
+            }
+        )
 
         # Retrieve the Pillow image and print it
         image = my_code.writer._image
         self.image(image, impl=impl, center=center)
 
     def text(self, txt):
-        """ Print alpha-numeric text
+        """Print alpha-numeric text
 
         The text has to be encoded in the currently selected codepage.
         The input text has to be encoded in unicode.
 
         :param txt: text to be printed
         :raises: :py:exc:`~escpos.exceptions.TextError`
         """
         txt = six.text_type(txt)
         self.magic.write(txt)
 
-    def textln(self, txt=''):
+    def textln(self, txt=""):
         """Print alpha-numeric text with a newline
 
         The text has to be encoded in the currently selected codepage.
         The input text has to be encoded in unicode.
 
         :param txt: text to be printed with a newline
         :raises: :py:exc:`~escpos.exceptions.TextError`
         """
-        self.text('{}\n'.format(txt))
+        self.text("{}\n".format(txt))
 
     def ln(self, count=1):
         """Print a newline or more
 
         :param count: number of newlines to print
         :raises: :py:exc:`ValueError` if count < 0
         """
         if count < 0:
-            raise ValueError('Count cannot be lesser than 0')
+            raise ValueError("Count cannot be lesser than 0")
         if count > 0:
-            self.text('\n' * count)
+            self.text("\n" * count)
 
-    def block_text(self, txt, font=None, columns=None):
-        """ Text is printed wrapped to specified columns
+    def block_text(self, txt, font="0", columns=None):
+        """Text is printed wrapped to specified columns
 
         Text has to be encoded in unicode.
 
         :param txt: text to be printed
         :param font: font to be used, can be :code:`a` or :code:`b`
         :param columns: amount of columns
         :return: None
         """
         col_count = self.profile.get_columns(font) if columns is None else columns
         self.text(textwrap.fill(txt, col_count))
 
-    def set(self, align='left', font='a', bold=False, underline=0, width=1,
-            height=1, density=9, invert=False, smooth=False, flip=False,
-            double_width=False, double_height=False, custom_size=False):
-        """ Set text properties by sending them to the printer
+    def set(
+        self,
+        align="left",
+        font="a",
+        bold=False,
+        underline=0,
+        width=1,
+        height=1,
+        density=9,
+        invert=False,
+        smooth=False,
+        flip=False,
+        double_width=False,
+        double_height=False,
+        custom_size=False,
+    ):
+        """Set text properties by sending them to the printer
 
         :param align: horizontal position for text, possible values are:
 
             * 'center'
             * 'left'
             * 'right'
 
@@ -592,45 +722,49 @@
         :type align: str
         :type width: int
         :type height: int
         :type density: int
         """
 
         if custom_size:
-            if 1 <= width <= 8 and 1 <= height <= 8 and isinstance(width, int) and\
-              isinstance(height, int):
-                size_byte = TXT_STYLE['width'][width] + TXT_STYLE['height'][height]
+            if (
+                1 <= width <= 8
+                and 1 <= height <= 8
+                and isinstance(width, int)
+                and isinstance(height, int)
+            ):
+                size_byte = TXT_STYLE["width"][width] + TXT_STYLE["height"][height]
                 self._raw(TXT_SIZE + six.int2byte(size_byte))
             else:
                 raise SetVariableError()
         else:
             self._raw(TXT_NORMAL)
             if double_width and double_height:
-                self._raw(TXT_STYLE['size']['2x'])
+                self._raw(TXT_STYLE["size"]["2x"])
             elif double_width:
-                self._raw(TXT_STYLE['size']['2w'])
+                self._raw(TXT_STYLE["size"]["2w"])
             elif double_height:
-                self._raw(TXT_STYLE['size']['2h'])
+                self._raw(TXT_STYLE["size"]["2h"])
             else:
-                self._raw(TXT_STYLE['size']['normal'])
+                self._raw(TXT_STYLE["size"]["normal"])
 
-        self._raw(TXT_STYLE['flip'][flip])
-        self._raw(TXT_STYLE['smooth'][smooth])
-        self._raw(TXT_STYLE['bold'][bold])
-        self._raw(TXT_STYLE['underline'][underline])
+        self._raw(TXT_STYLE["flip"][flip])
+        self._raw(TXT_STYLE["smooth"][smooth])
+        self._raw(TXT_STYLE["bold"][bold])
+        self._raw(TXT_STYLE["underline"][underline])
         self._raw(SET_FONT(six.int2byte(self.profile.get_font(font))))
-        self._raw(TXT_STYLE['align'][align])
+        self._raw(TXT_STYLE["align"][align])
 
         if density != 9:
-            self._raw(TXT_STYLE['density'][density])
+            self._raw(TXT_STYLE["density"][density])
 
-        self._raw(TXT_STYLE['invert'][invert])
+        self._raw(TXT_STYLE["invert"][invert])
 
     def line_spacing(self, spacing=None, divisor=180):
-        """ Set line character spacing.
+        """Set line character spacing.
 
         If no spacing is given, we reset it to the default.
 
         There are different commands for setting the line spacing, using
         a different denominator:
 
         '+'' line_spacing/360 of an inch, 0 <= line_spacing <= 255
@@ -642,59 +776,60 @@
         """
         if spacing is None:
             self._raw(LINESPACING_RESET)
             return
 
         if divisor not in LINESPACING_FUNCS:
             raise ValueError("divisor must be either 360, 180 or 60")
-        if (divisor in [360, 180]
-                and (not(0 <= spacing <= 255))):
-            raise ValueError("spacing must be a int between 0 and 255 when divisor is 360 or 180")
-        if divisor == 60 and (not(0 <= spacing <= 85)):
-            raise ValueError("spacing must be a int between 0 and 85 when divisor is 60")
+        if divisor in [360, 180] and (not (0 <= spacing <= 255)):
+            raise ValueError(
+                "spacing must be a int between 0 and 255 when divisor is 360 or 180"
+            )
+        if divisor == 60 and (not (0 <= spacing <= 85)):
+            raise ValueError(
+                "spacing must be a int between 0 and 85 when divisor is 60"
+            )
 
         self._raw(LINESPACING_FUNCS[divisor] + six.int2byte(spacing))
 
-    def cut(self, mode='FULL', feed=True):
-        """ Cut paper.
+    def cut(self, mode="FULL", feed=True):
+        """Cut paper.
 
         Without any arguments the paper will be cut completely. With 'mode=PART' a partial cut will
         be attempted. Note however, that not all models can do a partial cut. See the documentation of
         your printer for details.
 
-        .. todo:: Check this function on TM-T88II.
-
         :param mode: set to 'PART' for a partial cut. default: 'FULL'
         :param feed: print and feed before cutting. default: true
         :raises ValueError: if mode not in ('FULL', 'PART')
         """
 
         if not feed:
-            self._raw(GS + b'V' + six.int2byte(66) + b'\x00')
+            self._raw(GS + b"V" + six.int2byte(66) + b"\x00")
             return
 
         self.print_and_feed(6)
 
         mode = mode.upper()
-        if mode not in ('FULL', 'PART'):
+        if mode not in ("FULL", "PART"):
             raise ValueError("Mode must be one of ('FULL', 'PART')")
 
         if mode == "PART":
-            if self.profile.supports('paperPartCut'):
+            if self.profile.supports("paperPartCut"):
                 self._raw(PAPER_PART_CUT)
-            elif self.profile.supports('paperFullCut'):
+            elif self.profile.supports("paperFullCut"):
                 self._raw(PAPER_FULL_CUT)
         elif mode == "FULL":
-            if self.profile.supports('paperFullCut'):
+            if self.profile.supports("paperFullCut"):
                 self._raw(PAPER_FULL_CUT)
-            elif self.profile.supports('paperPartCut'):
+            elif self.profile.supports("paperPartCut"):
                 self._raw(PAPER_PART_CUT)
 
     def cashdraw(self, pin):
-        """ Send pulse to kick the cash drawer
+        """Send pulse to kick the cash drawer
 
         Kick cash drawer on pin 2 or pin 5 according to default parameter.
         For non default parameter send a decimal sequence i.e. [27,112,48] or [27,112,0,25,255]
 
         :param pin: pin number, 2 or 5 or list of decimals
         :raises: :py:exc:`~escpos.exceptions.CashDrawerError`
         """
@@ -705,30 +840,30 @@
         else:
             try:
                 self._raw(CD_KICK_DEC_SEQUENCE(*pin))
             except TypeError as err:
                 raise CashDrawerError(err)
 
     def linedisplay_select(self, select_display=False):
-        """ Selects the line display or the printer
+        """Selects the line display or the printer
 
         This method is used for line displays that are daisy-chained between your computer and printer.
         If you set `select_display` to true, only the display is selected and if you set it to false,
         only the printer is selected.
 
         :param select_display: whether the display should be selected or the printer
         :type select_display: bool
         """
         if select_display:
             self._raw(LINE_DISPLAY_OPEN)
         else:
             self._raw(LINE_DISPLAY_CLOSE)
 
     def linedisplay_clear(self):
-        """ Clears the line display and resets the cursor
+        """Clears the line display and resets the cursor
 
         This method is used for line displays that are daisy-chained between your computer and printer.
         """
         self._raw(LINE_DISPLAY_CLEAR)
 
     def linedisplay(self, text):
         """
@@ -741,15 +876,15 @@
         """
         self.linedisplay_select(select_display=True)
         self.linedisplay_clear()
         self.text(text)
         self.linedisplay_select(select_display=False)
 
     def hw(self, hw):
-        """ Hardware operations
+        """Hardware operations
 
         :param hw: hardware action, may be:
 
             * INIT
             * SELECT
             * RESET
         """
@@ -759,29 +894,29 @@
             self._raw(HW_SELECT)
         elif hw.upper() == "RESET":
             self._raw(HW_RESET)
         else:  # DEFAULT: DOES NOTHING
             pass
 
     def print_and_feed(self, n=1):
-        """ Print data in print buffer and feed *n* lines
+        """Print data in print buffer and feed *n* lines
 
-            if n not in range (0, 255) then ValueError will be raised
+        if n not in range (0, 255) then ValueError will be raised
 
-            :param n: number of n to feed. 0 <= n <= 255. default: 1
-            :raises ValueError: if not 0 <= n <= 255
+        :param n: number of n to feed. 0 <= n <= 255. default: 1
+        :raises ValueError: if not 0 <= n <= 255
         """
         if 0 <= n <= 255:
             # ESC d n
             self._raw(ESC + b"d" + six.int2byte(n))
         else:
             raise ValueError("n must be betwen 0 and 255")
 
     def control(self, ctl, count=5, tab_size=8):
-        """ Feed control sequences
+        """Feed control sequences
 
         :param ctl: string for the following control sequences:
 
             * LF *for Line Feed*
             * FF *for Form Feed*
             * CR *for Carriage Return*
             * HT *for Horizontal Tab*
@@ -795,29 +930,29 @@
         if ctl.upper() == "LF":
             self._raw(CTL_LF)
         elif ctl.upper() == "FF":
             self._raw(CTL_FF)
         elif ctl.upper() == "CR":
             self._raw(CTL_CR)
         elif ctl.upper() == "HT":
-            if not (0 <= count <= 32 and
-                    1 <= tab_size <= 255 and
-                    count * tab_size < 256):
+            if not (
+                0 <= count <= 32 and 1 <= tab_size <= 255 and count * tab_size < 256
+            ):
                 raise TabPosError()
             else:
                 # Set tab positions
                 self._raw(CTL_SET_HT)
                 for iterator in range(1, count):
                     self._raw(six.int2byte(iterator * tab_size))
                 self._raw(NUL)
         elif ctl.upper() == "VT":
             self._raw(CTL_VT)
 
     def panel_buttons(self, enable=True):
-        """ Controls the panel buttons on the printer (e.g. FEED)
+        """Controls the panel buttons on the printer (e.g. FEED)
 
         When enable is set to False the panel buttons on the printer will be disabled. Calling the method with
         enable=True or without argument will enable the panel buttons.
 
         If panel buttons are enabled, the function of the panel button, such as feeding, will be executed upon pressing
         the button. If the panel buttons are disabled, pressing them will not have any effect.
 
@@ -870,21 +1005,56 @@
 
         :returns: 2: Paper is adequate. 1: Paper ending. 0: No paper.
         :rtype: int
         """
         status = self.query_status(RT_STATUS_PAPER)
         if len(status) == 0:
             return 2
-        if (status[0] & RT_MASK_NOPAPER == RT_MASK_NOPAPER):
+        if status[0] & RT_MASK_NOPAPER == RT_MASK_NOPAPER:
             return 0
-        if (status[0] & RT_MASK_LOWPAPER == RT_MASK_LOWPAPER):
+        if status[0] & RT_MASK_LOWPAPER == RT_MASK_LOWPAPER:
             return 1
-        if (status[0] & RT_MASK_PAPER == RT_MASK_PAPER):
+        if status[0] & RT_MASK_PAPER == RT_MASK_PAPER:
             return 2
 
+    def target(self, type="ROLL"):
+        """Select where to print to
+
+        Print to the thermal printer by default (ROLL) or
+        print to the slip dot matrix printer if supported (SLIP)
+        """
+        if type.upper() == "ROLL":
+            self._raw(SHEET_ROLL_MODE)
+        elif type.upper() == "SLIP":
+            self._raw(SHEET_SLIP_MODE)
+        else:
+            raise ValueError("Unsupported target")
+
+    def eject_slip(self):
+        """Eject the slip/cheque"""
+        self._raw(SLIP_EJECT)
+
+    def print_and_eject_slip(self):
+        """Print and eject
+
+        Prints data from the buffer to the slip station and if the paper
+        sensor is covered, reverses the slip out the front of the printer
+        far enough to be accessible to the operator.
+        The impact station opens the platen in all cases.
+        """
+        self._raw(SLIP_PRINT_AND_EJECT)
+
+    def use_slip_only(self):
+        """Selects the Slip Station for all functions.
+
+        The receipt station is the default setting after the printer
+        is initialized or the Clear Printer (0x10) command is received
+        """
+        self._raw(SLIP_SELECT)
+
 
 class EscposIO(object):
     """ESC/POS Printer IO object
 
     Allows the class to be used together with the `with`-statement. You have to define a printer instance
     and assign it to the EscposIO class.
     This example explains the usage:
@@ -911,15 +1081,15 @@
         """
         self.printer = printer
         self.params = kwargs
         self.autocut = autocut
         self.autoclose = autoclose
 
     def set(self, **kwargs):
-        """ Set the printer-parameters
+        """Set the printer-parameters
 
         Controls which parameters will be passed to :py:meth:`Escpos.set() <escpos.escpos.Escpos.set()>`.
         For more information on the parameters see the :py:meth:`set() <escpos.escpos.Escpos.set()>`-methods
         documentation. These parameters can also be passed with this class' constructor or the
         :py:meth:`~escpos.escpos.EscposIO.writelines()`-method.
 
         :param kwargs: keyword-parameters that will be passed to :py:meth:`Escpos.set() <escpos.escpos.Escpos.set()>`
@@ -927,32 +1097,33 @@
         self.params.update(kwargs)
 
     def writelines(self, text, **kwargs):
         params = dict(self.params)
         params.update(kwargs)
 
         if isinstance(text, six.text_type):
-            lines = text.split('\n')
+            lines = text.split("\n")
         elif isinstance(text, list) or isinstance(text, tuple):
             lines = text
         else:
-            lines = ["{0}".format(text), ]
+            lines = [
+                "{0}".format(text),
+            ]
 
         # TODO check unicode handling
         # TODO flush? or on print? (this should prob rather be handled by the _raw-method)
         for line in lines:
             self.printer.set(**params)
             if isinstance(text, six.text_type):
-                self.printer.text(u"{0}\n".format(line))
+                self.printer.text("{0}\n".format(line))
             else:
                 self.printer.text("{0}\n".format(line))
 
     def close(self):
-        """ called upon closing the `with`-statement
-        """
+        """called upon closing the `with`-statement"""
         self.printer.close()
 
     def __enter__(self, **kwargs):
         return self
 
     def __exit__(self, type, value, traceback):
         """
```

### Comparing `python-escpos-3.0a8/src/escpos/exceptions.py` & `python-escpos-3.0a9/src/escpos/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,231 +23,253 @@
 :organization: Bashlinux and `python-escpos <https://github.com/python-escpos>`_
 :copyright: Copyright (c) 2012-2017 Bashlinux and python-escpos
 :license: MIT
 """
 
 
 class Error(Exception):
-    """ Base class for ESC/POS errors """
+    """Base class for ESC/POS errors"""
+
     def __init__(self, msg, status=None):
         Exception.__init__(self)
         self.msg = msg
         self.resultcode = 1
         if status is not None:
             self.resultcode = status
 
     def __str__(self):
         return self.msg
 
 
 class BarcodeTypeError(Error):
-    """ No Barcode type defined.
+    """No Barcode type defined.
 
     This exception indicates that no known barcode-type has been entered. The barcode-type has to be
     one of those specified in :py:meth:`escpos.escpos.Escpos.barcode`.
     The returned error code is `10`.
     """
+
     def __init__(self, msg=""):
         Error.__init__(self, msg)
         self.msg = msg
         self.resultcode = 10
 
     def __str__(self):
         return "No Barcode type is defined ({msg})".format(msg=self.msg)
 
 
 class BarcodeSizeError(Error):
-    """ Barcode size is out of range.
+    """Barcode size is out of range.
 
     This exception indicates that the values for the barcode size are out of range.
     The size of the barcode has to be in the range that is specified in :py:meth:`escpos.escpos.Escpos.barcode`.
     The resulting returncode is `20`.
     """
+
     def __init__(self, msg=""):
         Error.__init__(self, msg)
         self.msg = msg
         self.resultcode = 20
 
     def __str__(self):
         return "Barcode size is out of range ({msg})".format(msg=self.msg)
 
 
 class BarcodeCodeError(Error):
-    """ No Barcode code was supplied, or it is incorrect.
+    """No Barcode code was supplied, or it is incorrect.
 
     No data for the barcode has been supplied in :py:meth:`escpos.escpos.Escpos.barcode` or the the `check` parameter
     was True and the check failed.
     The returncode for this exception is `30`.
     """
+
     def __init__(self, msg=""):
         Error.__init__(self, msg)
         self.msg = msg
         self.resultcode = 30
 
     def __str__(self):
         return "No Barcode code was supplied ({msg})".format(msg=self.msg)
 
 
 class ImageSizeError(Error):
-    """ Image height is longer than 255px and can't be printed.
+    """Image height is longer than 255px and can't be printed.
 
     The returncode for this exception is `40`.
     """
+
     def __init__(self, msg=""):
         Error.__init__(self, msg)
         self.msg = msg
         self.resultcode = 40
 
     def __str__(self):
-        return "Image height is longer than 255px and can't be printed ({msg})".format(msg=self.msg)
+        return "Image height is longer than 255px and can't be printed ({msg})".format(
+            msg=self.msg
+        )
 
 
 class ImageWidthError(Error):
-    """ Image width is too large.
+    """Image width is too large.
 
     The return code for this exception is `41`.
     """
+
     def __init__(self, msg=""):
         Error.__init__(self, msg)
         self.msg = msg
         self.resultcode = 41
 
     def __str__(self):
         return "Image width is too large ({msg})".format(msg=self.msg)
 
 
 class TextError(Error):
-    """ Text string must be supplied to the `text()` method.
+    """Text string must be supplied to the `text()` method.
 
     This exception is raised when an empty string is passed to :py:meth:`escpos.escpos.Escpos.text`.
     The returncode for this exception is `50`.
     """
+
     def __init__(self, msg=""):
         Error.__init__(self, msg)
         self.msg = msg
         self.resultcode = 50
 
     def __str__(self):
-        return "Text string must be supplied to the text() method ({msg})".format(msg=self.msg)
+        return "Text string must be supplied to the text() method ({msg})".format(
+            msg=self.msg
+        )
 
 
 class CashDrawerError(Error):
-    """ Valid pin must be set in order to send pulse.
+    """Valid pin must be set in order to send pulse.
 
     A valid pin number has to be passed onto the method :py:meth:`escpos.escpos.Escpos.cashdraw`.
     The returncode for this exception is `60`.
     """
+
     def __init__(self, msg=""):
         Error.__init__(self, msg)
         self.msg = msg
         self.resultcode = 60
 
     def __str__(self):
         return "Valid pin must be set to send pulse ({msg})".format(msg=self.msg)
 
 
 class TabPosError(Error):
-    """ Valid tab positions must be set by using from 1 to 32 tabs, and between 1 and 255 tab size values.
+    """Valid tab positions must be set by using from 1 to 32 tabs, and between 1 and 255 tab size values.
     Both values multiplied must not exceed 255, since it is the maximum tab value.
 
     This exception is raised by :py:meth:`escpos.escpos.Escpos.control`.
     The returncode for this exception is `70`.
     """
+
     def __init__(self, msg=""):
         Error.__init__(self, msg)
         self.msg = msg
         self.resultcode = 70
 
     def __str__(self):
-        return "Valid tab positions must be in the range 0 to 16 ({msg})".format(msg=self.msg)
+        return "Valid tab positions must be in the range 0 to 16 ({msg})".format(
+            msg=self.msg
+        )
 
 
 class CharCodeError(Error):
-    """ Valid char code must be set.
+    """Valid char code must be set.
 
     The supplied charcode-name in :py:meth:`escpos.escpos.Escpos.charcode` is unknown.
     Ths returncode for this exception is `80`.
     """
+
     def __init__(self, msg=""):
         Error.__init__(self, msg)
         self.msg = msg
         self.resultcode = 80
 
     def __str__(self):
         return "Valid char code must be set ({msg})".format(msg=self.msg)
 
 
 class USBNotFoundError(Error):
-    """ Device wasn't found (probably not plugged in)
+    """Device wasn't found (probably not plugged in)
 
     The USB device seems to be not plugged in.
     Ths returncode for this exception is `90`.
     """
+
     def __init__(self, msg=""):
         Error.__init__(self, msg)
         self.msg = msg
         self.resultcode = 90
 
     def __str__(self):
         return "USB device not found ({msg})".format(msg=self.msg)
 
 
 class SetVariableError(Error):
-    """ A set method variable was out of range
+    """A set method variable was out of range
 
     Check set variables against minimum and maximum values
     Ths returncode for this exception is `100`.
     """
+
     def __init__(self, msg=""):
         Error.__init__(self, msg)
         self.msg = msg
         self.resultcode = 100
 
     def __str__(self):
         return "Set variable out of range ({msg})".format(msg=self.msg)
 
 
 # Configuration errors
 
+
 class ConfigNotFoundError(Error):
-    """ The configuration file was not found
+    """The configuration file was not found
 
     The default or passed configuration file could not be read
     Ths returncode for this exception is `200`.
     """
+
     def __init__(self, msg=""):
         Error.__init__(self, msg)
         self.msg = msg
         self.resultcode = 200
 
     def __str__(self):
         return "Configuration not found ({msg})".format(msg=self.msg)
 
 
 class ConfigSyntaxError(Error):
-    """ The configuration file is invalid
+    """The configuration file is invalid
 
     The syntax is incorrect
     Ths returncode for this exception is `210`.
     """
+
     def __init__(self, msg=""):
         Error.__init__(self, msg)
         self.msg = msg
         self.resultcode = 210
 
     def __str__(self):
         return "Configuration syntax is invalid ({msg})".format(msg=self.msg)
 
 
 class ConfigSectionMissingError(Error):
-    """ The configuration file is missing a section
+    """The configuration file is missing a section
 
     The part of the config asked for doesn't exist in the loaded configuration
     Ths returncode for this exception is `220`.
     """
+
     def __init__(self, msg=""):
         Error.__init__(self, msg)
         self.msg = msg
         self.resultcode = 220
 
     def __str__(self):
         return "Configuration section is missing ({msg})".format(msg=self.msg)
```

### Comparing `python-escpos-3.0a8/src/escpos/image.py` & `python-escpos-3.0a9/src/escpos/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             img_original = Image.open(img_source)
 
         # store image for eventual further processing (splitting)
         self.img_original = img_original
 
         # Convert to white RGB background, paste over white background
         # to strip alpha.
-        img_original = img_original.convert('RGBA')
+        img_original = img_original.convert("RGBA")
         im = Image.new("RGB", img_original.size, (255, 255, 255))
         im.paste(img_original, mask=img_original.split()[3])
         # Convert down to greyscale
         im = im.convert("L")
         # Invert: Only works on 'L' images
         im = ImageOps.invert(im)
         # Pure black and white
@@ -81,15 +81,15 @@
         width_pixels, height_pixels = im.size
         top = 0
         left = 0
         while left < width_pixels:
             box = (left, top, left + line_height, top + height_pixels)
             im_slice = im.transform((line_height, height_pixels), Image.EXTENT, box)
             im_bytes = im_slice.tobytes()
-            yield(im_bytes)
+            yield (im_bytes)
             left += line_height
 
     def to_raster_format(self):
         """
         Convert image to raster-format binary
         """
         return self._im.tobytes()
@@ -97,15 +97,15 @@
     def split(self, fragment_height):
         """
         Split an image into multiple fragments after fragment_height pixels
 
         :param fragment_height: height of fragment
         :return: list of PIL objects
         """
-        passes = int(math.ceil(self.height/fragment_height))
+        passes = int(math.ceil(self.height / fragment_height))
         fragments = []
         for n in range(0, passes):
             left = 0
             right = self.width
             upper = n * fragment_height
             lower = min((n + 1) * fragment_height, self.height)
             box = (left, upper, right, lower)
```

### Comparing `python-escpos-3.0a8/src/escpos/magicencode.py` & `python-escpos-3.0a9/src/escpos/magicencode.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 
 from builtins import bytes
 from .constants import CODEPAGE_CHANGE
 from .exceptions import Error
 from .codepages import CodePages
 import six
+import re
 
 
 class Encoder(object):
     """Takes a list of available code spaces. Picks the right one for a
     given character.
 
     Note: To determine the code page, it needs to do the conversion, and
@@ -51,60 +52,66 @@
         canonical encoding name; and also validate that the encoding
         is supported.
 
         TODO: Support encoding aliases: pc437 instead of cp437.
         """
         encoding = CodePages.get_encoding_name(encoding)
         if encoding not in self.codepages:
-            raise ValueError((
-                'Encoding "{}" cannot be used for the current profile. '
-                'Valid encodings are: {}'
-                ).format(encoding, ','.join(self.codepages.keys())))
+            raise ValueError(
+                (
+                    'Encoding "{}" cannot be used for the current profile. '
+                    "Valid encodings are: {}"
+                ).format(encoding, ",".join(self.codepages.keys()))
+            )
         return encoding
 
     @staticmethod
     def _get_codepage_char_list(encoding):
         """Get codepage character list
 
         Gets characters 128-255 for a given code page, as an array.
 
         :param encoding: The name of the encoding. This must appear in the CodePage list
         """
         codepage = CodePages.get_encoding(encoding)
-        if 'data' in codepage:
-            encodable_chars = list("".join(codepage['data']))
-            assert(len(encodable_chars) == 128)
+        if "data" in codepage:
+            encodable_chars = list("".join(codepage["data"]))
+            assert len(encodable_chars) == 128
             return encodable_chars
-        elif 'python_encode' in codepage:
-            encodable_chars = [u" "] * 128
+        elif "python_encode" in codepage:
+            encodable_chars = [" "] * 128
             for i in range(0, 128):
                 codepoint = i + 128
                 try:
-                    encodable_chars[i] = bytes([codepoint]).decode(codepage['python_encode'])
+                    encodable_chars[i] = bytes([codepoint]).decode(
+                        codepage["python_encode"]
+                    )
                 except UnicodeDecodeError:
                     # Non-encodable character, just skip it
                     pass
             return encodable_chars
         raise LookupError("Can't find a known encoding for {}".format(encoding))
 
     def _get_codepage_char_map(self, encoding):
-        """ Get codepage character map
+        """Get codepage character map
 
         Process an encoding and return a map of UTF-characters to code points
         in this encoding.
 
         This is generated once only, and returned from a cache.
 
         :param encoding: The name of the encoding.
         """
         # Skip things that were loaded previously
         if encoding in self.available_characters:
             return self.available_characters[encoding]
         codepage_char_list = self._get_codepage_char_list(encoding)
-        codepage_char_map = dict((utf8, i + 128) for (i, utf8) in enumerate(codepage_char_list))
+        codepage_char_map = dict(
+            (utf8, i + 128) for (i, utf8) in enumerate(codepage_char_list)
+        )
         self.available_characters[encoding] = codepage_char_map
         return codepage_char_map
 
     def can_encode(self, encoding, char):
         """Determine if a character is encodeable in the given code page.
 
         :param encoding: The name of the encoding.
@@ -119,42 +126,41 @@
         # Decide whether this character is encodeable in this code page
         is_ascii = ord(char) < 128
         is_encodable = char in available_map
         return is_ascii or is_encodable
 
     @staticmethod
     def _encode_char(char, charmap, defaultchar):
-        """ Encode a single character with the given encoding map
+        """Encode a single character with the given encoding map
 
         :param char: char to encode
         :param charmap: dictionary for mapping characters in this code page
         """
         if ord(char) < 128:
             return ord(char)
         if char in charmap:
             return charmap[char]
         return ord(defaultchar)
 
-    def encode(self, text, encoding, defaultchar='?'):
-        """ Encode text under the given encoding
+    def encode(self, text, encoding, defaultchar="?"):
+        """Encode text under the given encoding
 
         :param text: Text to encode
         :param encoding: Encoding name to use (must be defined in capabilities)
         :param defaultchar: Fallback for non-encodable characters
         """
         codepage_char_map = self._get_codepage_char_map(encoding)
-        output_bytes = bytes([self._encode_char(char, codepage_char_map, defaultchar) for char in text])
+        output_bytes = bytes(
+            [self._encode_char(char, codepage_char_map, defaultchar) for char in text]
+        )
         return output_bytes
 
     def __encoding_sort_func(self, item):
         key, index = item
-        return (
-            key in self.used_encodings,
-            index
-        )
+        return (key in self.used_encodings, index)
 
     def find_suitable_encoding(self, char):
         """The order of our search is a specific one:
 
         1. code pages that we already tried before; there is a good
            chance they might work again, reducing the search space,
            and by re-using already used encodings we might also
@@ -164,27 +170,25 @@
 
         2. code pages in lower ESCPOS slots first. Presumably, they
            are more likely to be supported, so if a printer profile
            is missing or incomplete, we might increase our change
            that the code page we pick for this character is actually
            supported.
         """
-        sorted_encodings = sorted(
-            self.codepages.items(),
-            key=self.__encoding_sort_func)
+        sorted_encodings = sorted(self.codepages.items(), key=self.__encoding_sort_func)
 
         for encoding, _ in sorted_encodings:
             if self.can_encode(encoding, char):
                 # This encoding worked; at it to the set of used ones.
                 self.used_encodings.add(encoding)
                 return encoding
 
 
 def split_writable_text(encoder, text, encoding):
-    """Splits off as many characters from the begnning of text as
+    """Splits off as many characters from the beginning of text as
     are writable with "encoding". Returns a 2-tuple (writable, rest).
     """
     if not encoding:
         return None, text
 
     for idx, char in enumerate(text):
         if encoder.can_encode(encoding, char):
@@ -201,29 +205,31 @@
     This will consider the printers supported codepages, according
     to the printer profile, and if a character cannot be encoded
     with the current profile, it will attempt to find a suitable one.
 
     If the printer does not support a suitable code page, it can
     insert an error character.
     """
-    def __init__(self, driver, encoding=None, disabled=False,
-                 defaultsymbol='?', encoder=None):
+
+    def __init__(
+        self, driver, encoding=None, disabled=False, defaultsymbol="?", encoder=None
+    ):
         """
 
         :param driver:
         :param encoding: If you know the current encoding of the printer
         when initializing this class, set it here. If the current
         encoding is unknown, the first character emitted will be a
         codepage switch.
         :param disabled:
         :param defaultsymbol:
         :param encoder:
         """
         if disabled and not encoding:
-            raise Error('If you disable magic encode, you need to define an encoding!')
+            raise Error("If you disable magic encode, you need to define an encoding!")
 
         self.driver = driver
         self.encoder = encoder or Encoder(driver.profile.get_code_pages())
 
         self.encoding = self.encoder.get_encoding_name(encoding) if encoding else None
         self.defaultsymbol = defaultsymbol
         self.disabled = disabled
@@ -237,21 +243,24 @@
         if not encoding:
             self.disabled = False
         else:
             self.write_with_encoding(encoding, None)
             self.disabled = True
 
     def write(self, text):
-        """Write the text, automatically switching encodings.
-        """
+        """Write the text, automatically switching encodings."""
 
         if self.disabled:
             self.write_with_encoding(self.encoding, text)
             return
 
+        if re.findall(r"[\u4e00-\u9fa5]", text):
+            self.driver._raw(text.encode("GB18030"))
+            return
+
         # See how far we can go into the text with the current encoding
         to_write, text = split_writable_text(self.encoder, text, self.encoding)
         if to_write:
             self.write_with_encoding(self.encoding, to_write)
 
         while text:
             # See if any of the code pages that the printer profile
@@ -264,29 +273,30 @@
 
             # Write as much text as possible with the encoding found.
             to_write, text = split_writable_text(self.encoder, text, encoding)
             if to_write:
                 self.write_with_encoding(encoding, to_write)
 
     def _handle_character_failed(self, char):
-        """Called when no codepage was found to render a character.
-        """
+        """Called when no codepage was found to render a character."""
         # Writing the default symbol via write() allows us to avoid
         # unnecesary codepage switches.
         self.write(self.defaultsymbol)
 
     def write_with_encoding(self, encoding, text):
         if text is not None and type(text) is not six.text_type:
-            raise Error("The supplied text has to be unicode, but is of type {type}.".format(
-                type=type(text)
-            ))
+            raise Error(
+                "The supplied text has to be unicode, but is of type {type}.".format(
+                    type=type(text)
+                )
+            )
 
         # We always know the current code page; if the new codepage
         # is different, emit a change command.
         if encoding != self.encoding:
             self.encoding = encoding
             self.driver._raw(
-                CODEPAGE_CHANGE +
-                six.int2byte(self.encoder.get_sequence(encoding)))
+                CODEPAGE_CHANGE + six.int2byte(self.encoder.get_sequence(encoding))
+            )
 
         if text:
             self.driver._raw(self.encoder.encode(text, encoding))
```

### Comparing `python-escpos-3.0a8/src/escpos/printer.py` & `python-escpos-3.0a9/src/escpos/printer.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,37 +5,67 @@
 :author: `Manuel F Martinez <manpaz@bashlinux.com>`_ and others
 :organization: Bashlinux and `python-escpos <https://github.com/python-escpos>`_
 :copyright: Copyright (c) 2012-2017 Bashlinux and python-escpos
 :license: MIT
 """
 
 
-import serial
+import os
 import socket
+import subprocess
+import sys
+
+import serial
 import usb.core
 import usb.util
 
 from .escpos import Escpos
 from .exceptions import USBNotFoundError
 
+_WIN32PRINT = False
+try:
+    import win32print
+
+    _WIN32PRINT = True
+except ImportError:
+    pass
+
+_CUPSPRINT = False
+try:
+    import cups
+    import tempfile
+
+    _CUPSPRINT = True
+except ImportError:
+    pass
+
 
 class Usb(Escpos):
-    """ USB printer
+    """USB printer
 
     This class describes a printer that natively speaks USB.
 
     inheritance:
 
     .. inheritance-diagram:: escpos.printer.Usb
         :parts: 1
 
     """
 
-    def __init__(self, idVendor, idProduct, usb_args=None, timeout=0, in_ep=0x82, out_ep=0x01,
-                 *args, **kwargs):  # noqa: N803
+    def __init__(
+        self,
+        idVendor,
+        idProduct,
+        usb_args=None,
+        timeout=0,
+        in_ep=0x82,
+        out_ep=0x01,
+        *args,
+        **kwargs
+    ):  # noqa: N803
         """
         :param idVendor: Vendor ID
         :param idProduct: Product ID
         :param usb_args: Optional USB arguments (e.g. custom_match)
         :param timeout: Is the time limit of the USB operation. Default without timeout.
         :param in_ep: Input end point
         :param out_ep: Output end point
@@ -43,21 +73,21 @@
         Escpos.__init__(self, *args, **kwargs)
         self.timeout = timeout
         self.in_ep = in_ep
         self.out_ep = out_ep
 
         usb_args = usb_args or {}
         if idVendor:
-            usb_args['idVendor'] = idVendor
+            usb_args["idVendor"] = idVendor
         if idProduct:
-            usb_args['idProduct'] = idProduct
+            usb_args["idProduct"] = idProduct
         self.open(usb_args)
 
     def open(self, usb_args):
-        """ Search device on USB tree and set it as escpos device.
+        """Search device on USB tree and set it as escpos device.
 
         :param usb_args: USB arguments
         """
         self.device = usb.core.find(**usb_args)
         if self.device is None:
             raise USBNotFoundError("Device not found or cable not plugged in.")
 
@@ -88,47 +118,57 @@
         try:
             self.device.set_configuration()
             self.device.reset()
         except usb.core.USBError as e:
             print("Could not set configuration: {0}".format(str(e)))
 
     def _raw(self, msg):
-        """ Print any command sent in raw format
+        """Print any command sent in raw format
 
         :param msg: arbitrary code to be printed
         :type msg: bytes
         """
         self.device.write(self.out_ep, msg, self.timeout)
 
     def _read(self):
-        """ Reads a data buffer and returns it to the caller. """
+        """Reads a data buffer and returns it to the caller."""
         return self.device.read(self.in_ep, 16)
 
     def close(self):
-        """ Release USB interface """
+        """Release USB interface"""
         if self.device:
             usb.util.dispose_resources(self.device)
         self.device = None
 
 
 class Serial(Escpos):
-    """ Serial printer
+    """Serial printer
 
     This class describes a printer that is connected by serial interface.
 
     inheritance:
 
     .. inheritance-diagram:: escpos.printer.Serial
         :parts: 1
 
     """
 
-    def __init__(self, devfile="/dev/ttyS0", baudrate=9600, bytesize=8, timeout=1,
-                 parity=serial.PARITY_NONE, stopbits=serial.STOPBITS_ONE,
-                 xonxoff=False, dsrdtr=True, *args, **kwargs):
+    def __init__(
+        self,
+        devfile="/dev/ttyS0",
+        baudrate=9600,
+        bytesize=8,
+        timeout=1,
+        parity=serial.PARITY_NONE,
+        stopbits=serial.STOPBITS_ONE,
+        xonxoff=False,
+        dsrdtr=True,
+        *args,
+        **kwargs
+    ):
         """
 
         :param devfile:  Device file under dev filesystem
         :param baudrate: Baud rate for serial transmission
         :param bytesize: Serial buffer size
         :param timeout:  Read/Write timeout
         :param parity:   Parity checking
@@ -145,48 +185,54 @@
         self.stopbits = stopbits
         self.xonxoff = xonxoff
         self.dsrdtr = dsrdtr
 
         self.open()
 
     def open(self):
-        """ Setup serial port and set is as escpos device """
+        """Setup serial port and set is as escpos device"""
         if self.device is not None and self.device.is_open:
             self.close()
-        self.device = serial.Serial(port=self.devfile, baudrate=self.baudrate,
-                                    bytesize=self.bytesize, parity=self.parity,
-                                    stopbits=self.stopbits, timeout=self.timeout,
-                                    xonxoff=self.xonxoff, dsrdtr=self.dsrdtr)
+        self.device = serial.Serial(
+            port=self.devfile,
+            baudrate=self.baudrate,
+            bytesize=self.bytesize,
+            parity=self.parity,
+            stopbits=self.stopbits,
+            timeout=self.timeout,
+            xonxoff=self.xonxoff,
+            dsrdtr=self.dsrdtr,
+        )
 
         if self.device is not None:
             print("Serial printer enabled")
         else:
             print("Unable to open serial printer on: {0}".format(str(self.devfile)))
 
     def _raw(self, msg):
-        """ Print any command sent in raw format
+        """Print any command sent in raw format
 
         :param msg: arbitrary code to be printed
         :type msg: bytes
         """
         self.device.write(msg)
 
     def _read(self):
-        """ Reads a data buffer and returns it to the caller. """
+        """Reads a data buffer and returns it to the caller."""
         return self.device.read(16)
 
     def close(self):
-        """ Close Serial interface """
+        """Close Serial interface"""
         if self.device is not None and self.device.is_open:
             self.device.flush()
             self.device.close()
 
 
 class Network(Escpos):
-    """ Network printer
+    """Network printer
 
     This class is used to attach to a networked printer. You can also use this in order to attach to a printer that
     is forwarded with ``socat``.
 
     If you have a local printer on parallel port ``/dev/usb/lp0`` then you could start ``socat`` with:
 
     .. code-block:: none
@@ -214,44 +260,47 @@
         Escpos.__init__(self, *args, **kwargs)
         self.host = host
         self.port = port
         self.timeout = timeout
         self.open()
 
     def open(self):
-        """ Open TCP socket with ``socket``-library and set it as escpos device """
+        """Open TCP socket with ``socket``-library and set it as escpos device"""
         self.device = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.device.settimeout(self.timeout)
         self.device.connect((self.host, self.port))
 
         if self.device is None:
             print("Could not open socket for {0}".format(self.host))
 
     def _raw(self, msg):
-        """ Print any command sent in raw format
+        """Print any command sent in raw format
 
         :param msg: arbitrary code to be printed
         :type msg: bytes
         """
         self.device.sendall(msg)
 
     def _read(self):
-        """ Read data from the TCP socket """
+        """Read data from the TCP socket"""
 
         return self.device.recv(16)
 
     def close(self):
-        """ Close TCP connection """
+        """Close TCP connection"""
         if self.device is not None:
-            self.device.shutdown(socket.SHUT_RDWR)
+            try:
+                self.device.shutdown(socket.SHUT_RDWR)
+            except socket.error:
+                pass
             self.device.close()
 
 
 class File(Escpos):
-    """ Generic file printer
+    """Generic file printer
 
     This class is used for parallel port printer or other printers that are directly attached to the filesystem.
     Note that you should stay away from using USB-to-Parallel-Adapter since they are unreliable
     and produce arbitrary errors.
 
     inheritance:
 
@@ -268,123 +317,286 @@
         """
         Escpos.__init__(self, *args, **kwargs)
         self.devfile = devfile
         self.auto_flush = auto_flush
         self.open()
 
     def open(self):
-        """ Open system file """
+        """Open system file"""
         self.device = open(self.devfile, "wb")
 
         if self.device is None:
             print("Could not open the specified file {0}".format(self.devfile))
 
     def flush(self):
-        """ Flush printing content """
+        """Flush printing content"""
         self.device.flush()
 
     def _raw(self, msg):
-        """ Print any command sent in raw format
+        """Print any command sent in raw format
 
         :param msg: arbitrary code to be printed
         :type msg: bytes
         """
         self.device.write(msg)
         if self.auto_flush:
             self.flush()
 
     def close(self):
-        """ Close system file """
+        """Close system file"""
         if self.device is not None:
             self.device.flush()
             self.device.close()
 
 
 class Dummy(Escpos):
-    """ Dummy printer
+    """Dummy printer
 
     This class is used for saving commands to a variable, for use in situations where
     there is no need to send commands to an actual printer. This includes
     generating print jobs for later use, or testing output.
 
     inheritance:
 
     .. inheritance-diagram:: escpos.printer.Dummy
         :parts: 1
 
     """
 
     def __init__(self, *args, **kwargs):
-        """
-        """
+        """ """
         Escpos.__init__(self, *args, **kwargs)
         self._output_list = []
 
     def _raw(self, msg):
-        """ Print any command sent in raw format
+        """Print any command sent in raw format
 
         :param msg: arbitrary code to be printed
         :type msg: bytes
         """
         self._output_list.append(msg)
 
     @property
     def output(self):
-        """ Get the data that was sent to this printer """
-        return b''.join(self._output_list)
+        """Get the data that was sent to this printer"""
+        return b"".join(self._output_list)
 
     def clear(self):
-        """ Clear the buffer of the printer
+        """Clear the buffer of the printer
 
         This method can be called if you send the contents to a physical printer
         and want to use the Dummy printer for new output.
         """
         del self._output_list[:]
 
     def close(self):
         pass
 
 
-_WIN32PRINT = False
-try:
-    import win32print
-
-    _WIN32PRINT = True
-except ImportError:
-    pass
-
 if _WIN32PRINT:
+
     class Win32Raw(Escpos):
         def __init__(self, printer_name=None, *args, **kwargs):
             Escpos.__init__(self, *args, **kwargs)
             if printer_name is not None:
                 self.printer_name = printer_name
             else:
                 self.printer_name = win32print.GetDefaultPrinter()
             self.hPrinter = None
+            self.open()
 
         def open(self, job_name="python-escpos"):
             if self.printer_name is None:
                 raise Exception("Printer not found")
             self.hPrinter = win32print.OpenPrinter(self.printer_name)
-            self.current_job = win32print.StartDocPrinter(self.hPrinter, 1, (job_name, None, "RAW"))
+            self.current_job = win32print.StartDocPrinter(
+                self.hPrinter, 1, (job_name, None, "RAW")
+            )
             win32print.StartPagePrinter(self.hPrinter)
 
         def close(self):
             if not self.hPrinter:
                 return
             win32print.EndPagePrinter(self.hPrinter)
             win32print.EndDocPrinter(self.hPrinter)
             win32print.ClosePrinter(self.hPrinter)
             self.hPrinter = None
 
         def _raw(self, msg):
-            """ Print any command sent in raw format
+            """Print any command sent in raw format
 
             :param msg: arbitrary code to be printed
             :type msg: bytes
             """
             if self.printer_name is None:
                 raise Exception("Printer not found")
             if self.hPrinter is None:
                 raise Exception("Printer job not opened")
             win32print.WritePrinter(self.hPrinter, msg)
+
+
+if _CUPSPRINT:
+
+    class CupsPrinter(Escpos):
+        """Simple CUPS printer connector.
+
+        .. note::
+                Requires _pycups_ which in turn needs the cups development library package:
+                - Ubuntu/Debian: _libcups2-dev_
+                - OpenSuse/Fedora: _cups-devel_
+        """
+
+        def __init__(self, printer_name=None, *args, **kwargs):
+            """CupsPrinter class constructor.
+
+            :param printer_name: CUPS printer name (Optional)
+            :type printer_name: str
+            :param host: CUPS server host/ip (Optional)
+            :type host: str
+            :param port: CUPS server port (Optional)
+            :type port: int
+            """
+            Escpos.__init__(self, *args, **kwargs)
+            host, port = args or (
+                kwargs.get("host", cups.getServer()),
+                kwargs.get("port", cups.getPort()),
+            )
+            cups.setServer(host)
+            cups.setPort(port)
+            self.conn = cups.Connection()
+            self.tmpfile = None
+            self.printer_name = printer_name
+            self.job_name = ""
+            self.pending_job = False
+            self.open()
+
+        @property
+        def printers(self):
+            """Available CUPS printers."""
+            return self.conn.getPrinters()
+
+        def open(self, job_name="python-escpos"):
+            """Setup a new print job and target printer.
+
+            A call to this method is required to send new jobs to
+            the same CUPS connection.
+
+            Defaults to default CUPS printer.
+            Creates a new temporary file buffer.
+            """
+            self.job_name = job_name
+            if self.printer_name not in self.printers:
+                self.printer_name = self.conn.getDefault()
+            self.tmpfile = tempfile.NamedTemporaryFile(delete=True)
+
+        def _raw(self, msg):
+            """Append any command sent in raw format to temporary file
+
+            :param msg: arbitrary code to be printed
+            :type msg: bytes
+            """
+            self.pending_job = True
+            try:
+                self.tmpfile.write(msg)
+            except ValueError:
+                self.pending_job = False
+                raise ValueError("Printer job not opened")
+
+        def send(self):
+            """Send the print job to the printer."""
+            if self.pending_job:
+                # Rewind tempfile
+                self.tmpfile.seek(0)
+                # Print temporary file via CUPS printer.
+                self.conn.printFile(
+                    self.printer_name,
+                    self.tmpfile.name,
+                    self.job_name,
+                    {"document-format": cups.CUPS_FORMAT_RAW},
+                )
+            self._clear()
+
+        def _clear(self):
+            """Finish the print job.
+
+            Remove temporary file.
+            """
+            self.tmpfile.close()
+            self.pending_job = False
+
+        def _read(self):
+            """Return a single-item array with the accepting state of the print queue.
+
+            states: idle = [3], printing a job = [4], stopped = [5]
+            """
+            printer = self.printers.get(self.printer_name, {})
+            state = printer.get("printer-state")
+            if not state:
+                return []
+            return [state]
+
+        def close(self):
+            """Close CUPS connection.
+
+            Send pending job to the printer if needed.
+            """
+            if self.pending_job:
+                self.send()
+            if self.conn:
+                print("Closing CUPS connection to printer {}".format(self.printer_name))
+                self.conn = None
+
+
+if not sys.platform.startswith("win"):
+
+    class LP(Escpos):
+        """Simple UNIX lp command raw printing.
+
+        Thanks to `Oyami-Srk comment <https://github.com/python-escpos/python-escpos/pull/348#issuecomment-549558316>`_.
+        """
+
+        def __init__(self, printer_name: str, *args, **kwargs):
+            """LP class constructor.
+
+            :param printer_name: CUPS printer name (Optional)
+            :type printer_name: str
+            :param auto_flush: Automatic flush after every _raw() (Optional)
+            :type auto_flush: bool
+            """
+            Escpos.__init__(self, *args, **kwargs)
+            self.printer_name = printer_name
+            self.auto_flush = kwargs.get("auto_flush", True)
+            self.open()
+
+        def open(self):
+            """Invoke _lp_ in a new subprocess and wait for commands."""
+            self.lp = subprocess.Popen(
+                ["lp", "-d", self.printer_name, "-o", "raw"],
+                stdin=subprocess.PIPE,
+                stdout=open(os.devnull, "w"),
+            )
+
+        def close(self):
+            """Stop the subprocess."""
+            self.lp.terminate()
+
+        def flush(self):
+            """End line and wait for new commands"""
+            if self.lp.stdin.writable():
+                self.lp.stdin.write(b"\n")
+            if self.lp.stdin.closed is False:
+                self.lp.stdin.close()
+            self.lp.wait()
+            self.open()
+
+        def _raw(self, msg):
+            """Write raw command(s) to the printer.
+
+            :param msg: arbitrary code to be printed
+            :type msg: bytes
+            """
+            if self.lp.stdin.writable():
+                self.lp.stdin.write(msg)
+            else:
+                raise Exception("Not a valid pipe for lp process")
+            if self.auto_flush:
+                self.flush()
```

### Comparing `python-escpos-3.0a8/src/python_escpos.egg-info/PKG-INFO` & `python-escpos-3.0a9/src/python_escpos.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,141 +1,143 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: python-escpos
-Version: 3.0a8
+Version: 3.0a9
 Summary: Python library to manipulate ESC/POS Printers
 Home-page: https://github.com/python-escpos/python-escpos
 Author: Manuel F Martinez and others
 Author-email: dev@pkanzler.de
 Maintainer: Patrick Kanzler
 Maintainer-email: dev@pkanzler.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/python-escpos/python-escpos/issues
 Project-URL: Documentation, https://python-escpos.readthedocs.io/en/latest/
 Project-URL: Release Notes, https://github.com/python-escpos/python-escpos/releases
-Description: #############################################################
-        python-escpos - Python library to manipulate ESC/POS Printers
-        #############################################################
-        
-        .. image:: https://travis-ci.org/python-escpos/python-escpos.svg?branch=master
-            :target: https://travis-ci.org/python-escpos/python-escpos
-            :alt: Continous Integration
-        
-        .. image:: https://codecov.io/github/python-escpos/python-escpos/coverage.svg?branch=master
-            :target: https://codecov.io/github/python-escpos/python-escpos?branch=master
-            :alt: Code Coverage
-        
-        .. image:: https://readthedocs.org/projects/python-escpos/badge/?version=latest
-            :target: http://python-escpos.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        
-        Description
-        -----------
-        
-        Python ESC/POS is a library which lets the user have access to all those printers handled
-        by ESC/POS commands, as defined by Epson, from a Python application.
-        
-        The library tries to implement the functions provided by the ESC/POS-commandset and supports sending text, images,
-        barcodes and qr-codes to the printer.
-        
-        Text can be aligned/justified and fonts can be changed by size, type and weight.
-        
-        Also, this module handles some hardware functionalities like cutting paper, control characters, printer reset
-        and similar functions.
-        
-        Since supported commands differ from printer to printer the software tries to automatically apply the right
-        settings for the printer that you set. These settings are handled by
-        `escpos-printer-db <https://github.com/receipt-print-hq/escpos-printer-db>`_ which is also used in
-        `escpos-php <https://github.com/mike42/escpos-php>`_.
-        
-        Dependencies
-        ------------
-        
-        This library makes use of:
-        
-        * `pyusb <https://github.com/walac/pyusb>`_ for USB-printers
-        * `Pillow <https://github.com/python-pillow/Pillow>`_ for image printing
-        * `qrcode <https://github.com/lincolnloop/python-qrcode>`_ for the generation of QR-codes
-        * `pyserial <https://github.com/pyserial/pyserial>`_ for serial printers
-        * `python-barcode <https://github.com/WhyNotHugo/python-barcode>`_ for the generation of barcodes
-        
-        Documentation and Usage
-        -----------------------
-        
-        The basic usage is:
-        
-        .. code:: python
-        
-            from escpos.printer import Usb
-        
-            """ Seiko Epson Corp. Receipt Printer (EPSON TM-T88III) """
-            p = Usb(0x04b8, 0x0202, 0, profile="TM-T88III")
-            p.text("Hello World\n")
-            p.image("logo.gif")
-            p.barcode('1324354657687', 'EAN13', 64, 2, '', '')
-            p.cut()
-        
-        
-        Another example based on the Network printer class:
-        
-        .. code:: python
-        
-            from escpos.printer import Network
-            
-            kitchen = Network("192.168.1.100") #Printer IP Address
-            kitchen.text("Hello World\n")
-            kitchen.barcode('1324354657687', 'EAN13', 64, 2, '', '')
-            kitchen.cut()
-            
-        Another example based on the Serial printer class:
-        
-        .. code:: python
-        
-            from escpos.printer import Serial
-            
-            """ 9600 Baud, 8N1, Flow Control Enabled """
-            p = Serial(devfile='/dev/tty.usbserial',
-                       baudrate=9600,
-                       bytesize=8,
-                       parity='N',
-                       stopbits=1,
-                       timeout=1.00,
-                       dsrdtr=True)
-        
-            p.text("Hello World\n")
-            p.qr("You can readme from your smartphone")
-            p.cut()
-        
-        
-        The full project-documentation is available on `Read the Docs <https://python-escpos.readthedocs.io>`_.
-        
-        Contributing
-        ------------
-        
-        This project is open for any contribution! Please see `CONTRIBUTING.rst <http://python-escpos.readthedocs.io/en/latest/dev/contributing.html>`_ for more information.
-        
-        
-        Disclaimer
-        ----------
-        
-        None of the vendors cited in this project agree or endorse any of the patterns or implementations.
-        Its names are used only to maintain context.
-        
-        
-        
 Keywords: ESC/POS,thermoprinter,voucher printer,printing,receipt
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Office/Business :: Financial :: Point-Of-Sale
-Requires-Python: >=3.5
+Requires-Python: >=3.6
+License-File: LICENSE
+
+#############################################################
+python-escpos - Python library to manipulate ESC/POS Printers
+#############################################################
+
+.. image:: https://travis-ci.org/python-escpos/python-escpos.svg?branch=master
+    :target: https://travis-ci.org/python-escpos/python-escpos
+    :alt: Continous Integration
+
+.. image:: https://codecov.io/github/python-escpos/python-escpos/coverage.svg?branch=master
+    :target: https://codecov.io/github/python-escpos/python-escpos?branch=master
+    :alt: Code Coverage
+
+.. image:: https://readthedocs.org/projects/python-escpos/badge/?version=latest
+    :target: https://python-escpos.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+
+Description
+-----------
+
+Python ESC/POS is a library which lets the user have access to all those printers handled
+by ESC/POS commands, as defined by Epson, from a Python application.
+
+The library tries to implement the functions provided by the ESC/POS-commandset and supports sending text, images,
+barcodes and qr-codes to the printer.
+
+Text can be aligned/justified and fonts can be changed by size, type and weight.
+
+Also, this module handles some hardware functionalities like cutting paper, control characters, printer reset
+and similar functions.
+
+Since supported commands differ from printer to printer the software tries to automatically apply the right
+settings for the printer that you set. These settings are handled by
+`escpos-printer-db <https://github.com/receipt-print-hq/escpos-printer-db>`_ which is also used in
+`escpos-php <https://github.com/mike42/escpos-php>`_.
+
+Dependencies
+------------
+
+This library makes use of:
+
+* `pyusb <https://github.com/walac/pyusb>`_ for USB-printers
+* `Pillow <https://github.com/python-pillow/Pillow>`_ for image printing
+* `qrcode <https://github.com/lincolnloop/python-qrcode>`_ for the generation of QR-codes
+* `pyserial <https://github.com/pyserial/pyserial>`_ for serial printers
+* `python-barcode <https://github.com/WhyNotHugo/python-barcode>`_ for the generation of barcodes
+
+Documentation and Usage
+-----------------------
+
+The basic usage is:
+
+.. code:: python
+
+    from escpos.printer import Usb
+
+    """ Seiko Epson Corp. Receipt Printer (EPSON TM-T88III) """
+    p = Usb(0x04b8, 0x0202, 0, profile="TM-T88III")
+    p.text("Hello World\n")
+    p.image("logo.gif")
+    p.barcode('1324354657687', 'EAN13', 64, 2, '', '')
+    p.cut()
+
+
+Another example based on the Network printer class:
+
+.. code:: python
+
+    from escpos.printer import Network
+
+    kitchen = Network("192.168.1.100") #Printer IP Address
+    kitchen.text("Hello World\n")
+    kitchen.barcode('1324354657687', 'EAN13', 64, 2, '', '')
+    kitchen.cut()
+
+Another example based on the Serial printer class:
+
+.. code:: python
+
+    from escpos.printer import Serial
+
+    """ 9600 Baud, 8N1, Flow Control Enabled """
+    p = Serial(devfile='/dev/tty.usbserial',
+               baudrate=9600,
+               bytesize=8,
+               parity='N',
+               stopbits=1,
+               timeout=1.00,
+               dsrdtr=True)
+
+    p.text("Hello World\n")
+    p.qr("You can readme from your smartphone")
+    p.cut()
+
+
+The full project-documentation is available on `Read the Docs <https://python-escpos.readthedocs.io>`_.
+
+Contributing
+------------
+
+This project is open for any contribution! Please see `CONTRIBUTING.rst <https://python-escpos.readthedocs.io/en/latest/dev/contributing.html>`_ for more information.
+
+
+Disclaimer
+----------
+
+None of the vendors cited in this project agree or endorse any of the patterns or implementations.
+Its names are used only to maintain context.
+
+
```

### Comparing `python-escpos-3.0a8/src/python_escpos.egg-info/SOURCES.txt` & `python-escpos-3.0a9/src/python_escpos.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 .coveragerc
 .gitignore
 .gitmodules
 .mailmap
-.travis.yml
 AUTHORS
 CHANGELOG.rst
 CONTRIBUTING.rst
 INSTALL
 LICENSE
 MANIFEST.in
 README.rst
 codecov.yml
+pyproject.toml
 readthedocs.yml
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 .github/ISSUE_TEMPLATE.md
 .github/PULL_REQUEST_TEMPLATE.md
+.github/dependabot.yml
+.github/workflows/black.yml
+.github/workflows/codeql-analysis.yml
+.github/workflows/documentation.yml
 .github/workflows/pythonpackage.yml
 .vscode/settings.json
 .vscode/tasks.json
 capabilities-data/dist/capabilities.json
 doc/.gitignore
 doc/Makefile
 doc/conf.py
@@ -152,14 +156,15 @@
 test/test_function_softbarcode.py
 test/test_function_text.py
 test/test_functions.py
 test/test_image.py
 test/test_load_module.py
 test/test_magicencode.py
 test/test_printer_file.py
+test/test_printer_network.py
 test/test_profile.py
 test/test_raise_arbitrary_error.py
 test/test_with_statement.py
 test/resources/black_transparent.gif
 test/resources/black_transparent.png
 test/resources/black_white.gif
 test/resources/black_white.jpg
```

### Comparing `python-escpos-3.0a8/test/test_abstract_base_class.py` & `python-escpos-3.0a9/test/test_abstract_base_class.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,10 +17,10 @@
 @raises(TypeError)
 def test_abstract_base_class_raises():
     """test whether the abstract base class raises an exception for ESC/POS"""
     escpos.Escpos()  # This call should raise TypeError because of abstractmethod _raw()
 
 
 def test_abstract_base_class():
-    """ test whether Escpos has the metaclass ABCMeta """
+    """test whether Escpos has the metaclass ABCMeta"""
     assert issubclass(escpos.Escpos, object)
     assert type(escpos.Escpos) is ABCMeta
```

### Comparing `python-escpos-3.0a8/test/test_function_barcode.py` & `python-escpos-3.0a9/test/test_function_barcode.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,46 +2,55 @@
 
 import escpos.printer as printer
 from escpos.capabilities import Profile, BARCODE_B
 from escpos.exceptions import BarcodeTypeError, BarcodeCodeError
 import pytest
 
 
-@pytest.mark.parametrize("bctype,data,expected", [
-    ('EAN13', '4006381333931',
-        b'\x1ba\x01\x1dh@\x1dw\x03\x1df\x00\x1dH\x02\x1dk\x024006381333931\x00')
-])
+@pytest.mark.parametrize(
+    "bctype,data,expected",
+    [
+        (
+            "EAN13",
+            "4006381333931",
+            b"\x1ba\x01\x1dh@\x1dw\x03\x1df\x00\x1dH\x02\x1dk\x024006381333931\x00",
+        )
+    ],
+)
 def test_barcode(bctype, data, expected):
-    """should generate different barcode types correctly.
-    """
+    """should generate different barcode types correctly."""
     instance = printer.Dummy()
     instance.barcode(data, bctype)
     assert instance.output == expected
 
 
-@pytest.mark.parametrize("bctype,supports_b", [
-    ('invalid', True),
-    ('CODE128', False),
-])
+@pytest.mark.parametrize(
+    "bctype,supports_b",
+    [
+        ("invalid", True),
+        ("CODE128", False),
+    ],
+)
 def test_lacks_support(bctype, supports_b):
-    """should raise an error if the barcode type is not supported.
-    """
+    """should raise an error if the barcode type is not supported."""
     profile = Profile(features={BARCODE_B: supports_b})
     instance = printer.Dummy(profile=profile)
     with pytest.raises(BarcodeTypeError):
-        instance.barcode('test', bctype)
+        instance.barcode("test", bctype)
 
-    assert instance.output == b''
+    assert instance.output == b""
 
 
-@pytest.mark.parametrize("bctype,data", [
-    ('EAN13', 'AA'),
-    ('CODE128', '{D2354AA'),
-])
+@pytest.mark.parametrize(
+    "bctype,data",
+    [
+        ("EAN13", "AA"),
+        ("CODE128", "{D2354AA"),
+    ],
+)
 def test_code_check(bctype, data):
-    """should raise an error if the barcode code is invalid.
-    """
+    """should raise an error if the barcode code is invalid."""
     instance = printer.Dummy()
     with pytest.raises(BarcodeCodeError):
         instance.barcode(data, bctype)
 
-    assert instance.output == b''
+    assert instance.output == b""
```

### Comparing `python-escpos-3.0a8/test/test_function_image.py` & `python-escpos-3.0a9/test/test_function_image.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,143 +18,158 @@
 
 # Raster format print
 def test_bit_image_black():
     """
     Test printing solid black bit image (raster)
     """
     instance = printer.Dummy()
-    instance.image('test/resources/canvas_black.png', impl="bitImageRaster")
-    assert(instance.output == b'\x1dv0\x00\x01\x00\x01\x00\x80')
+    instance.image("test/resources/canvas_black.png", impl="bitImageRaster")
+    assert instance.output == b"\x1dv0\x00\x01\x00\x01\x00\x80"
     # Same thing w/ object created on the fly, rather than a filename
     instance = printer.Dummy()
     im = Image.new("RGB", (1, 1), (0, 0, 0))
     instance.image(im, impl="bitImageRaster")
-    assert(instance.output == b'\x1dv0\x00\x01\x00\x01\x00\x80')
+    assert instance.output == b"\x1dv0\x00\x01\x00\x01\x00\x80"
 
 
 def test_bit_image_white():
     """
     Test printing solid white bit image (raster)
     """
     instance = printer.Dummy()
-    instance.image('test/resources/canvas_white.png', impl="bitImageRaster")
-    assert(instance.output == b'\x1dv0\x00\x01\x00\x01\x00\x00')
+    instance.image("test/resources/canvas_white.png", impl="bitImageRaster")
+    assert instance.output == b"\x1dv0\x00\x01\x00\x01\x00\x00"
 
 
 def test_bit_image_both():
     """
     Test printing black/white bit image (raster)
     """
     instance = printer.Dummy()
-    instance.image('test/resources/black_white.png', impl="bitImageRaster")
-    assert(instance.output == b'\x1dv0\x00\x01\x00\x02\x00\xc0\x00')
+    instance.image("test/resources/black_white.png", impl="bitImageRaster")
+    assert instance.output == b"\x1dv0\x00\x01\x00\x02\x00\xc0\x00"
 
 
 def test_bit_image_transparent():
     """
     Test printing black/transparent bit image (raster)
     """
     instance = printer.Dummy()
-    instance.image('test/resources/black_transparent.png', impl="bitImageRaster")
-    assert(instance.output == b'\x1dv0\x00\x01\x00\x02\x00\xc0\x00')
+    instance.image("test/resources/black_transparent.png", impl="bitImageRaster")
+    assert instance.output == b"\x1dv0\x00\x01\x00\x02\x00\xc0\x00"
 
 
 # Column format print
 def test_bit_image_colfmt_black():
     """
     Test printing solid black bit image (column format)
     """
     instance = printer.Dummy()
-    instance.image('test/resources/canvas_black.png', impl="bitImageColumn")
-    assert(instance.output == b'\x1b3\x10\x1b*!\x01\x00\x80\x00\x00\x0a\x1b2')
+    instance.image("test/resources/canvas_black.png", impl="bitImageColumn")
+    assert instance.output == b"\x1b3\x10\x1b*!\x01\x00\x80\x00\x00\x0a\x1b2"
 
 
 def test_bit_image_colfmt_white():
     """
     Test printing solid white bit image (column format)
     """
     instance = printer.Dummy()
-    instance.image('test/resources/canvas_white.png', impl="bitImageColumn")
-    assert(instance.output == b'\x1b3\x10\x1b*!\x01\x00\x00\x00\x00\x0a\x1b2')
+    instance.image("test/resources/canvas_white.png", impl="bitImageColumn")
+    assert instance.output == b"\x1b3\x10\x1b*!\x01\x00\x00\x00\x00\x0a\x1b2"
 
 
 def test_bit_image_colfmt_both():
     """
     Test printing black/white bit image (column format)
     """
     instance = printer.Dummy()
-    instance.image('test/resources/black_white.png', impl="bitImageColumn")
-    assert(instance.output == b'\x1b3\x10\x1b*!\x02\x00\x80\x00\x00\x80\x00\x00\x0a\x1b2')
+    instance.image("test/resources/black_white.png", impl="bitImageColumn")
+    assert (
+        instance.output == b"\x1b3\x10\x1b*!\x02\x00\x80\x00\x00\x80\x00\x00\x0a\x1b2"
+    )
 
 
 def test_bit_image_colfmt_transparent():
     """
     Test printing black/transparent bit image (column format)
     """
     instance = printer.Dummy()
-    instance.image('test/resources/black_transparent.png', impl="bitImageColumn")
-    assert(instance.output == b'\x1b3\x10\x1b*!\x02\x00\x80\x00\x00\x80\x00\x00\x0a\x1b2')
+    instance.image("test/resources/black_transparent.png", impl="bitImageColumn")
+    assert (
+        instance.output == b"\x1b3\x10\x1b*!\x02\x00\x80\x00\x00\x80\x00\x00\x0a\x1b2"
+    )
 
 
 # Graphics print
 def test_graphics_black():
     """
     Test printing solid black graphics
     """
     instance = printer.Dummy()
-    instance.image('test/resources/canvas_black.png', impl="graphics")
-    assert(instance.output == b'\x1d(L\x0b\x000p0\x01\x011\x01\x00\x01\x00\x80\x1d(L\x02\x0002')
+    instance.image("test/resources/canvas_black.png", impl="graphics")
+    assert (
+        instance.output
+        == b"\x1d(L\x0b\x000p0\x01\x011\x01\x00\x01\x00\x80\x1d(L\x02\x0002"
+    )
 
 
 def test_graphics_white():
     """
     Test printing solid white graphics
     """
     instance = printer.Dummy()
-    instance.image('test/resources/canvas_white.png', impl="graphics")
-    assert(instance.output == b'\x1d(L\x0b\x000p0\x01\x011\x01\x00\x01\x00\x00\x1d(L\x02\x0002')
+    instance.image("test/resources/canvas_white.png", impl="graphics")
+    assert (
+        instance.output
+        == b"\x1d(L\x0b\x000p0\x01\x011\x01\x00\x01\x00\x00\x1d(L\x02\x0002"
+    )
 
 
 def test_graphics_both():
     """
     Test printing black/white graphics
     """
     instance = printer.Dummy()
-    instance.image('test/resources/black_white.png', impl="graphics")
-    assert(instance.output == b'\x1d(L\x0c\x000p0\x01\x011\x02\x00\x02\x00\xc0\x00\x1d(L\x02\x0002')
+    instance.image("test/resources/black_white.png", impl="graphics")
+    assert (
+        instance.output
+        == b"\x1d(L\x0c\x000p0\x01\x011\x02\x00\x02\x00\xc0\x00\x1d(L\x02\x0002"
+    )
 
 
 def test_graphics_transparent():
     """
     Test printing black/transparent graphics
     """
     instance = printer.Dummy()
-    instance.image('test/resources/black_transparent.png', impl="graphics")
-    assert(instance.output == b'\x1d(L\x0c\x000p0\x01\x011\x02\x00\x02\x00\xc0\x00\x1d(L\x02\x0002')
+    instance.image("test/resources/black_transparent.png", impl="graphics")
+    assert (
+        instance.output
+        == b"\x1d(L\x0c\x000p0\x01\x011\x02\x00\x02\x00\xc0\x00\x1d(L\x02\x0002"
+    )
 
 
 def test_large_graphics():
     """
     Test whether 'large' graphics that induce a fragmentation are handled correctly.
     """
     instance = printer.Dummy()
-    instance.image('test/resources/black_white.png', impl="bitImageRaster", fragment_height=1)
-    assert(instance.output == b'\x1dv0\x00\x01\x00\x01\x00\xc0\x1dv0\x00\x01\x00\x01\x00\x00')
+    instance.image(
+        "test/resources/black_white.png", impl="bitImageRaster", fragment_height=1
+    )
+    assert (
+        instance.output
+        == b"\x1dv0\x00\x01\x00\x01\x00\xc0\x1dv0\x00\x01\x00\x01\x00\x00"
+    )
 
 
 @pytest.fixture
 def dummy_with_width():
     instance = printer.Dummy()
-    instance.profile.profile_data = {
-        'media': {
-            'width': {
-                'pixels': 384
-            }
-        }
-    }
+    instance.profile.profile_data = {"media": {"width": {"pixels": 384}}}
     return instance
 
 
 def test_width_too_large(dummy_with_width):
     """
     Test printing an image that is too large in width.
     """
```

### Comparing `python-escpos-3.0a8/test/test_function_linedisplay.py` & `python-escpos-3.0a9/test/test_function_linedisplay.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 import escpos.printer as printer
 
 
 def test_function_linedisplay_select_on():
     """test the linedisplay_select function (activate)"""
     instance = printer.Dummy()
     instance.linedisplay_select(select_display=True)
-    assert(instance.output == b'\x1B\x3D\x02')
+    assert instance.output == b"\x1B\x3D\x02"
+
 
 def test_function_linedisplay_select_off():
     """test the linedisplay_select function (deactivate)"""
     instance = printer.Dummy()
     instance.linedisplay_select(select_display=False)
-    assert(instance.output == b'\x1B\x3D\x01')
+    assert instance.output == b"\x1B\x3D\x01"
+
 
 def test_function_linedisplay_clear():
     """test the linedisplay_clear function"""
     instance = printer.Dummy()
     instance.linedisplay_clear()
-    assert(instance.output == b'\x1B\x40')
-
+    assert instance.output == b"\x1B\x40"
```

### Comparing `python-escpos-3.0a8/test/test_function_panel_button.py` & `python-escpos-3.0a9/test/test_function_panel_button.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import escpos.printer as printer
 
 
 def test_function_panel_button_on():
     """test the panel button function (enabling) by comparing output"""
     instance = printer.Dummy()
     instance.panel_buttons()
-    assert(instance.output == b'\x1B\x63\x35\x00')
+    assert instance.output == b"\x1B\x63\x35\x00"
 
 
 def test_function_panel_button_off():
     """test the panel button function (disabling) by comparing output"""
     instance = printer.Dummy()
     instance.panel_buttons(False)
-    assert(instance.output == b'\x1B\x63\x35\x01')
+    assert instance.output == b"\x1B\x63\x35\x01"
```

### Comparing `python-escpos-3.0a8/test/test_function_qr_native.py` & `python-escpos-3.0a9/test/test_function_qr_native.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,50 +15,59 @@
 from escpos.constants import QR_ECLEVEL_H, QR_MODEL_1
 
 
 def test_defaults():
     """Test QR code with defaults"""
     instance = printer.Dummy()
     instance.qr("1234", native=True)
-    expected = b'\x1d(k\x04\x001A2\x00\x1d(k\x03\x001C\x03\x1d(k\x03\x001E0\x1d' \
-        b'(k\x07\x001P01234\x1d(k\x03\x001Q0'
-    assert(instance.output == expected)
+    expected = (
+        b"\x1d(k\x04\x001A2\x00\x1d(k\x03\x001C\x03\x1d(k\x03\x001E0\x1d"
+        b"(k\x07\x001P01234\x1d(k\x03\x001Q0"
+    )
+    assert instance.output == expected
+
 
 def test_empty():
     """Test QR printing blank code"""
     instance = printer.Dummy()
     instance.qr("", native=True)
-    assert(instance.output == b'')
+    assert instance.output == b""
 
 
 def test_ec():
     """Test QR error correction setting"""
     instance = printer.Dummy()
     instance.qr("1234", native=True, ec=QR_ECLEVEL_H)
-    expected = b'\x1d(k\x04\x001A2\x00\x1d(k\x03\x001C\x03\x1d(k\x03\x001E3\x1d' \
-        b'(k\x07\x001P01234\x1d(k\x03\x001Q0'
-    assert(instance.output == expected)
+    expected = (
+        b"\x1d(k\x04\x001A2\x00\x1d(k\x03\x001C\x03\x1d(k\x03\x001E3\x1d"
+        b"(k\x07\x001P01234\x1d(k\x03\x001Q0"
+    )
+    assert instance.output == expected
 
 
 def test_size():
     """Test QR box size"""
     instance = printer.Dummy()
     instance.qr("1234", native=True, size=7)
-    expected = b'\x1d(k\x04\x001A2\x00\x1d(k\x03\x001C\x07\x1d(k\x03\x001E0\x1d' \
-        b'(k\x07\x001P01234\x1d(k\x03\x001Q0'
-    assert(instance.output == expected)
+    expected = (
+        b"\x1d(k\x04\x001A2\x00\x1d(k\x03\x001C\x07\x1d(k\x03\x001E0\x1d"
+        b"(k\x07\x001P01234\x1d(k\x03\x001Q0"
+    )
+    assert instance.output == expected
 
 
 def test_model():
     """Test QR model"""
     instance = printer.Dummy()
     instance.qr("1234", native=True, model=QR_MODEL_1)
-    expected = b'\x1d(k\x04\x001A1\x00\x1d(k\x03\x001C\x03\x1d(k\x03\x001E0\x1d' \
-        b'(k\x07\x001P01234\x1d(k\x03\x001Q0'
-    assert(instance.output == expected)
+    expected = (
+        b"\x1d(k\x04\x001A1\x00\x1d(k\x03\x001C\x03\x1d(k\x03\x001E0\x1d"
+        b"(k\x07\x001P01234\x1d(k\x03\x001Q0"
+    )
+    assert instance.output == expected
 
 
 @raises(ValueError)
 def test_invalid_ec():
     """Test invalid QR error correction"""
     instance = printer.Dummy()
     instance.qr("1234", native=True, ec=-1)
@@ -80,20 +89,22 @@
 
 @pytest.mark.skip("this test has to be debugged")
 def test_image():
     """Test QR as image"""
     instance = printer.Dummy()
     instance.qr("1", native=False, size=1)
     print(instance.output)
-    expected = b'\x1bt\x00\n' \
-        b'\x1dv0\x00\x03\x00\x17\x00\x00\x00\x00\x7f]\xfcA\x19\x04]it]et' \
-        b']ItA=\x04\x7fU\xfc\x00\x0c\x00y~t4\x7f =\xa84j\xd9\xf0\x05\xd4\x90\x00' \
-        b'i(\x7f<\xa8A \xd8]\'\xc4]y\xf8]E\x80Ar\x94\x7fR@\x00\x00\x00' \
-        b'\n\n'
-    assert(instance.output == expected)
+    expected = (
+        b"\x1bt\x00\n"
+        b"\x1dv0\x00\x03\x00\x17\x00\x00\x00\x00\x7f]\xfcA\x19\x04]it]et"
+        b"]ItA=\x04\x7fU\xfc\x00\x0c\x00y~t4\x7f =\xa84j\xd9\xf0\x05\xd4\x90\x00"
+        b"i(\x7f<\xa8A \xd8]'\xc4]y\xf8]E\x80Ar\x94\x7fR@\x00\x00\x00"
+        b"\n\n"
+    )
+    assert instance.output == expected
 
 
 @raises(ValueError)
 def test_image_invalid_model():
     """Test unsupported QR model as image"""
     instance = printer.Dummy()
     instance.qr("1234", native=False, model=QR_MODEL_1)
```

### Comparing `python-escpos-3.0a8/test/test_function_qr_non-native.py` & `python-escpos-3.0a9/test/test_function_qr_non-native.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import pytest
 import mock
 
 from escpos.printer import Dummy
 from PIL import Image
 
 
-@mock.patch('escpos.printer.Dummy.image', spec=Dummy)
+@mock.patch("escpos.printer.Dummy.image", spec=Dummy)
 def test_type_of_object_passed_to_image_function(img_function):
     """
     Test the type of object that is passed to the image function during non-native qr-printing.
 
     The type should be PIL.Image
     """
     d = Dummy()
```

### Comparing `python-escpos-3.0a8/test/test_function_set.py` & `python-escpos-3.0a9/test/test_function_set.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,276 +1,297 @@
-
 import six
 
 import escpos.printer as printer
 from escpos.constants import TXT_NORMAL, TXT_STYLE, SET_FONT
 from escpos.constants import TXT_SIZE
 
 
 # Default test, please copy and paste this block to test set method calls
 
+
 def test_default_values():
     instance = printer.Dummy()
     instance.set()
 
     expected_sequence = (
-        TXT_NORMAL, TXT_STYLE['size']['normal'],  # Normal text size
-        TXT_STYLE['flip'][False],  # Flip OFF
-        TXT_STYLE['smooth'][False],  # Smooth OFF
-        TXT_STYLE['bold'][False],  # Bold OFF
-        TXT_STYLE['underline'][0],  # Underline OFF
-        SET_FONT(b'\x00'),  # Default font
-        TXT_STYLE['align']['left'],  # Align left
-        TXT_STYLE['invert'][False]  # Inverted OFF
+        TXT_NORMAL,
+        TXT_STYLE["size"]["normal"],  # Normal text size
+        TXT_STYLE["flip"][False],  # Flip OFF
+        TXT_STYLE["smooth"][False],  # Smooth OFF
+        TXT_STYLE["bold"][False],  # Bold OFF
+        TXT_STYLE["underline"][0],  # Underline OFF
+        SET_FONT(b"\x00"),  # Default font
+        TXT_STYLE["align"]["left"],  # Align left
+        TXT_STYLE["invert"][False],  # Inverted OFF
     )
 
-    assert(instance.output == b''.join(expected_sequence))
+    assert instance.output == b"".join(expected_sequence)
+
 
 # Size tests
 
+
 def test_set_size_2h():
     instance = printer.Dummy()
     instance.set(double_height=True)
 
     expected_sequence = (
-        TXT_NORMAL, TXT_STYLE['size']['2h'],  # Double height text size
-        TXT_STYLE['flip'][False],  # Flip OFF
-        TXT_STYLE['smooth'][False],  # Smooth OFF
-        TXT_STYLE['bold'][False],  # Bold OFF
-        TXT_STYLE['underline'][0],  # Underline OFF
-        SET_FONT(b'\x00'),  # Default font
-        TXT_STYLE['align']['left'],  # Align left
-        TXT_STYLE['invert'][False]  # Inverted OFF
+        TXT_NORMAL,
+        TXT_STYLE["size"]["2h"],  # Double height text size
+        TXT_STYLE["flip"][False],  # Flip OFF
+        TXT_STYLE["smooth"][False],  # Smooth OFF
+        TXT_STYLE["bold"][False],  # Bold OFF
+        TXT_STYLE["underline"][0],  # Underline OFF
+        SET_FONT(b"\x00"),  # Default font
+        TXT_STYLE["align"]["left"],  # Align left
+        TXT_STYLE["invert"][False],  # Inverted OFF
     )
 
-    assert (instance.output == b''.join(expected_sequence))
+    assert instance.output == b"".join(expected_sequence)
 
 
 def test_set_size_2w():
     instance = printer.Dummy()
     instance.set(double_width=True)
 
     expected_sequence = (
-        TXT_NORMAL, TXT_STYLE['size']['2w'],  # Double width text size
-        TXT_STYLE['flip'][False],  # Flip OFF
-        TXT_STYLE['smooth'][False],  # Smooth OFF
-        TXT_STYLE['bold'][False],  # Bold OFF
-        TXT_STYLE['underline'][0],  # Underline OFF
-        SET_FONT(b'\x00'),  # Default font
-        TXT_STYLE['align']['left'],  # Align left
-        TXT_STYLE['invert'][False]  # Inverted OFF
+        TXT_NORMAL,
+        TXT_STYLE["size"]["2w"],  # Double width text size
+        TXT_STYLE["flip"][False],  # Flip OFF
+        TXT_STYLE["smooth"][False],  # Smooth OFF
+        TXT_STYLE["bold"][False],  # Bold OFF
+        TXT_STYLE["underline"][0],  # Underline OFF
+        SET_FONT(b"\x00"),  # Default font
+        TXT_STYLE["align"]["left"],  # Align left
+        TXT_STYLE["invert"][False],  # Inverted OFF
     )
 
-    assert (instance.output == b''.join(expected_sequence))
+    assert instance.output == b"".join(expected_sequence)
 
 
 def test_set_size_2x():
     instance = printer.Dummy()
     instance.set(double_height=True, double_width=True)
 
     expected_sequence = (
-        TXT_NORMAL, TXT_STYLE['size']['2x'],  # Double text size
-        TXT_STYLE['flip'][False],  # Flip OFF
-        TXT_STYLE['smooth'][False],  # Smooth OFF
-        TXT_STYLE['bold'][False],  # Bold OFF
-        TXT_STYLE['underline'][0],  # Underline OFF
-        SET_FONT(b'\x00'),  # Default font
-        TXT_STYLE['align']['left'],  # Align left
-        TXT_STYLE['invert'][False]  # Inverted OFF
+        TXT_NORMAL,
+        TXT_STYLE["size"]["2x"],  # Double text size
+        TXT_STYLE["flip"][False],  # Flip OFF
+        TXT_STYLE["smooth"][False],  # Smooth OFF
+        TXT_STYLE["bold"][False],  # Bold OFF
+        TXT_STYLE["underline"][0],  # Underline OFF
+        SET_FONT(b"\x00"),  # Default font
+        TXT_STYLE["align"]["left"],  # Align left
+        TXT_STYLE["invert"][False],  # Inverted OFF
     )
 
-    assert (instance.output == b''.join(expected_sequence))
+    assert instance.output == b"".join(expected_sequence)
 
 
 def test_set_size_custom():
     instance = printer.Dummy()
     instance.set(custom_size=True, width=8, height=7)
 
     expected_sequence = (
         TXT_SIZE,  # Custom text size, no normal reset
-        six.int2byte(TXT_STYLE['width'][8] + TXT_STYLE['height'][7]),
-        TXT_STYLE['flip'][False],  # Flip OFF
-        TXT_STYLE['smooth'][False],  # Smooth OFF
-        TXT_STYLE['bold'][False],  # Bold OFF
-        TXT_STYLE['underline'][0],  # Underline OFF
-        SET_FONT(b'\x00'),  # Default font
-        TXT_STYLE['align']['left'],  # Align left
-        TXT_STYLE['invert'][False]  # Inverted OFF
+        six.int2byte(TXT_STYLE["width"][8] + TXT_STYLE["height"][7]),
+        TXT_STYLE["flip"][False],  # Flip OFF
+        TXT_STYLE["smooth"][False],  # Smooth OFF
+        TXT_STYLE["bold"][False],  # Bold OFF
+        TXT_STYLE["underline"][0],  # Underline OFF
+        SET_FONT(b"\x00"),  # Default font
+        TXT_STYLE["align"]["left"],  # Align left
+        TXT_STYLE["invert"][False],  # Inverted OFF
     )
 
-    assert (instance.output == b''.join(expected_sequence))
+    assert instance.output == b"".join(expected_sequence)
+
 
 # Flip
 
+
 def test_set_flip():
     instance = printer.Dummy()
     instance.set(flip=True)
 
     expected_sequence = (
-        TXT_NORMAL, TXT_STYLE['size']['normal'],  # Normal text size
-        TXT_STYLE['flip'][True],  # Flip ON
-        TXT_STYLE['smooth'][False],  # Smooth OFF
-        TXT_STYLE['bold'][False],  # Bold OFF
-        TXT_STYLE['underline'][0],  # Underline OFF
-        SET_FONT(b'\x00'),  # Default font
-        TXT_STYLE['align']['left'],  # Align left
-        TXT_STYLE['invert'][False]  # Inverted OFF
+        TXT_NORMAL,
+        TXT_STYLE["size"]["normal"],  # Normal text size
+        TXT_STYLE["flip"][True],  # Flip ON
+        TXT_STYLE["smooth"][False],  # Smooth OFF
+        TXT_STYLE["bold"][False],  # Bold OFF
+        TXT_STYLE["underline"][0],  # Underline OFF
+        SET_FONT(b"\x00"),  # Default font
+        TXT_STYLE["align"]["left"],  # Align left
+        TXT_STYLE["invert"][False],  # Inverted OFF
     )
 
-    assert (instance.output == b''.join(expected_sequence))
+    assert instance.output == b"".join(expected_sequence)
+
 
 # Smooth
 
+
 def test_smooth():
     instance = printer.Dummy()
     instance.set(smooth=True)
 
     expected_sequence = (
-        TXT_NORMAL, TXT_STYLE['size']['normal'],  # Normal text size
-        TXT_STYLE['flip'][False],  # Flip OFF
-        TXT_STYLE['smooth'][True],  # Smooth ON
-        TXT_STYLE['bold'][False],  # Bold OFF
-        TXT_STYLE['underline'][0],  # Underline OFF
-        SET_FONT(b'\x00'),  # Default font
-        TXT_STYLE['align']['left'],  # Align left
-        TXT_STYLE['invert'][False]  # Inverted OFF
+        TXT_NORMAL,
+        TXT_STYLE["size"]["normal"],  # Normal text size
+        TXT_STYLE["flip"][False],  # Flip OFF
+        TXT_STYLE["smooth"][True],  # Smooth ON
+        TXT_STYLE["bold"][False],  # Bold OFF
+        TXT_STYLE["underline"][0],  # Underline OFF
+        SET_FONT(b"\x00"),  # Default font
+        TXT_STYLE["align"]["left"],  # Align left
+        TXT_STYLE["invert"][False],  # Inverted OFF
     )
 
-    assert(instance.output == b''.join(expected_sequence))
+    assert instance.output == b"".join(expected_sequence)
 
 
 # Type
 
 
 def test_set_bold():
     instance = printer.Dummy()
     instance.set(bold=True)
 
     expected_sequence = (
-        TXT_NORMAL, TXT_STYLE['size']['normal'],  # Normal text size
-        TXT_STYLE['flip'][False],  # Flip OFF
-        TXT_STYLE['smooth'][False],  # Smooth OFF
-        TXT_STYLE['bold'][True],  # Bold ON
-        TXT_STYLE['underline'][0],  # Underline OFF
-        SET_FONT(b'\x00'),  # Default font
-        TXT_STYLE['align']['left'],  # Align left
-        TXT_STYLE['invert'][False]  # Inverted OFF
+        TXT_NORMAL,
+        TXT_STYLE["size"]["normal"],  # Normal text size
+        TXT_STYLE["flip"][False],  # Flip OFF
+        TXT_STYLE["smooth"][False],  # Smooth OFF
+        TXT_STYLE["bold"][True],  # Bold ON
+        TXT_STYLE["underline"][0],  # Underline OFF
+        SET_FONT(b"\x00"),  # Default font
+        TXT_STYLE["align"]["left"],  # Align left
+        TXT_STYLE["invert"][False],  # Inverted OFF
     )
 
-    assert (instance.output == b''.join(expected_sequence))
+    assert instance.output == b"".join(expected_sequence)
 
 
 def test_set_underline():
     instance = printer.Dummy()
     instance.set(underline=1)
 
     expected_sequence = (
-        TXT_NORMAL, TXT_STYLE['size']['normal'],  # Normal text size
-        TXT_STYLE['flip'][False],  # Flip OFF
-        TXT_STYLE['smooth'][False],  # Smooth OFF
-        TXT_STYLE['bold'][False],  # Bold OFF
-        TXT_STYLE['underline'][1],  # Underline ON, type 1
-        SET_FONT(b'\x00'),  # Default font
-        TXT_STYLE['align']['left'],  # Align left
-        TXT_STYLE['invert'][False]  # Inverted OFF
+        TXT_NORMAL,
+        TXT_STYLE["size"]["normal"],  # Normal text size
+        TXT_STYLE["flip"][False],  # Flip OFF
+        TXT_STYLE["smooth"][False],  # Smooth OFF
+        TXT_STYLE["bold"][False],  # Bold OFF
+        TXT_STYLE["underline"][1],  # Underline ON, type 1
+        SET_FONT(b"\x00"),  # Default font
+        TXT_STYLE["align"]["left"],  # Align left
+        TXT_STYLE["invert"][False],  # Inverted OFF
     )
 
-    assert (instance.output == b''.join(expected_sequence))
+    assert instance.output == b"".join(expected_sequence)
 
 
 def test_set_underline2():
     instance = printer.Dummy()
     instance.set(underline=2)
 
     expected_sequence = (
-        TXT_NORMAL, TXT_STYLE['size']['normal'],  # Normal text size
-        TXT_STYLE['flip'][False],  # Flip OFF
-        TXT_STYLE['smooth'][False],  # Smooth OFF
-        TXT_STYLE['bold'][False],  # Bold OFF
-        TXT_STYLE['underline'][2],  # Underline ON, type 2
-        SET_FONT(b'\x00'),  # Default font
-        TXT_STYLE['align']['left'],  # Align left
-        TXT_STYLE['invert'][False]  # Inverted OFF
+        TXT_NORMAL,
+        TXT_STYLE["size"]["normal"],  # Normal text size
+        TXT_STYLE["flip"][False],  # Flip OFF
+        TXT_STYLE["smooth"][False],  # Smooth OFF
+        TXT_STYLE["bold"][False],  # Bold OFF
+        TXT_STYLE["underline"][2],  # Underline ON, type 2
+        SET_FONT(b"\x00"),  # Default font
+        TXT_STYLE["align"]["left"],  # Align left
+        TXT_STYLE["invert"][False],  # Inverted OFF
     )
 
-    assert (instance.output == b''.join(expected_sequence))
+    assert instance.output == b"".join(expected_sequence)
 
 
 # Align
 
+
 def test_align_center():
     instance = printer.Dummy()
-    instance.set(align='center')
+    instance.set(align="center")
 
     expected_sequence = (
-        TXT_NORMAL, TXT_STYLE['size']['normal'],  # Normal text size
-        TXT_STYLE['flip'][False],  # Flip OFF
-        TXT_STYLE['smooth'][False],  # Smooth OFF
-        TXT_STYLE['bold'][False],  # Bold OFF
-        TXT_STYLE['underline'][0],  # Underline OFF
-        SET_FONT(b'\x00'),  # Default font
-        TXT_STYLE['align']['center'],  # Align center
-        TXT_STYLE['invert'][False]  # Inverted OFF
+        TXT_NORMAL,
+        TXT_STYLE["size"]["normal"],  # Normal text size
+        TXT_STYLE["flip"][False],  # Flip OFF
+        TXT_STYLE["smooth"][False],  # Smooth OFF
+        TXT_STYLE["bold"][False],  # Bold OFF
+        TXT_STYLE["underline"][0],  # Underline OFF
+        SET_FONT(b"\x00"),  # Default font
+        TXT_STYLE["align"]["center"],  # Align center
+        TXT_STYLE["invert"][False],  # Inverted OFF
     )
 
-    assert(instance.output == b''.join(expected_sequence))
+    assert instance.output == b"".join(expected_sequence)
 
 
 def test_align_right():
     instance = printer.Dummy()
-    instance.set(align='right')
+    instance.set(align="right")
 
     expected_sequence = (
-        TXT_NORMAL, TXT_STYLE['size']['normal'],  # Normal text size
-        TXT_STYLE['flip'][False],  # Flip OFF
-        TXT_STYLE['smooth'][False],  # Smooth OFF
-        TXT_STYLE['bold'][False],  # Bold OFF
-        TXT_STYLE['underline'][0],  # Underline OFF
-        SET_FONT(b'\x00'),  # Default font
-        TXT_STYLE['align']['right'],  # Align right
-        TXT_STYLE['invert'][False]  # Inverted OFF
+        TXT_NORMAL,
+        TXT_STYLE["size"]["normal"],  # Normal text size
+        TXT_STYLE["flip"][False],  # Flip OFF
+        TXT_STYLE["smooth"][False],  # Smooth OFF
+        TXT_STYLE["bold"][False],  # Bold OFF
+        TXT_STYLE["underline"][0],  # Underline OFF
+        SET_FONT(b"\x00"),  # Default font
+        TXT_STYLE["align"]["right"],  # Align right
+        TXT_STYLE["invert"][False],  # Inverted OFF
     )
 
-    assert(instance.output == b''.join(expected_sequence))
+    assert instance.output == b"".join(expected_sequence)
 
 
 # Densities
 
-def test_densities():
 
+def test_densities():
     for density in range(8):
         instance = printer.Dummy()
         instance.set(density=density)
 
         expected_sequence = (
-            TXT_NORMAL, TXT_STYLE['size']['normal'],  # Normal text size
-            TXT_STYLE['flip'][False],  # Flip OFF
-            TXT_STYLE['smooth'][False],  # Smooth OFF
-            TXT_STYLE['bold'][False],  # Bold OFF
-            TXT_STYLE['underline'][0],  # Underline OFF
-            SET_FONT(b'\x00'),  # Default font
-            TXT_STYLE['align']['left'],  # Align left
-            TXT_STYLE['density'][density],  # Custom density from 0 to 8
-            TXT_STYLE['invert'][False]  # Inverted OFF
+            TXT_NORMAL,
+            TXT_STYLE["size"]["normal"],  # Normal text size
+            TXT_STYLE["flip"][False],  # Flip OFF
+            TXT_STYLE["smooth"][False],  # Smooth OFF
+            TXT_STYLE["bold"][False],  # Bold OFF
+            TXT_STYLE["underline"][0],  # Underline OFF
+            SET_FONT(b"\x00"),  # Default font
+            TXT_STYLE["align"]["left"],  # Align left
+            TXT_STYLE["density"][density],  # Custom density from 0 to 8
+            TXT_STYLE["invert"][False],  # Inverted OFF
         )
 
-        assert(instance.output == b''.join(expected_sequence))
+        assert instance.output == b"".join(expected_sequence)
 
 
 # Invert
 
+
 def test_invert():
     instance = printer.Dummy()
     instance.set(invert=True)
 
     expected_sequence = (
-        TXT_NORMAL, TXT_STYLE['size']['normal'],  # Normal text size
-        TXT_STYLE['flip'][False],  # Flip OFF
-        TXT_STYLE['smooth'][False],  # Smooth OFF
-        TXT_STYLE['bold'][False],  # Bold OFF
-        TXT_STYLE['underline'][0],  # Underline OFF
-        SET_FONT(b'\x00'),  # Default font
-        TXT_STYLE['align']['left'],  # Align left
-        TXT_STYLE['invert'][True]  # Inverted ON
+        TXT_NORMAL,
+        TXT_STYLE["size"]["normal"],  # Normal text size
+        TXT_STYLE["flip"][False],  # Flip OFF
+        TXT_STYLE["smooth"][False],  # Smooth OFF
+        TXT_STYLE["bold"][False],  # Bold OFF
+        TXT_STYLE["underline"][0],  # Underline OFF
+        SET_FONT(b"\x00"),  # Default font
+        TXT_STYLE["align"]["left"],  # Align left
+        TXT_STYLE["invert"][True],  # Inverted ON
     )
 
-    assert(instance.output == b''.join(expected_sequence))
+    assert instance.output == b"".join(expected_sequence)
```

### Comparing `python-escpos-3.0a8/test/test_function_text.py` & `python-escpos-3.0a9/test/test_function_text.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,50 +12,51 @@
 import mock
 from hypothesis import given, assume
 import hypothesis.strategies as st
 from escpos.printer import Dummy
 
 
 def get_printer():
-    return Dummy(magic_encode_args={'disabled': True, 'encoding': 'CP437'})
+    return Dummy(magic_encode_args={"disabled": True, "encoding": "CP437"})
 
 
 @given(text=st.text())
 def test_text(text):
-    """Test that text() calls the MagicEncode object.
-    """
+    """Test that text() calls the MagicEncode object."""
     instance = get_printer()
     instance.magic.write = mock.Mock()
     instance.text(text)
     instance.magic.write.assert_called_with(text)
 
 
 def test_block_text():
     printer = get_printer()
     printer.block_text(
-        "All the presidents men were eating falafel for breakfast.", font='a')
-    assert printer.output == \
-        b'All the presidents men were eating falafel\nfor breakfast.'
+        "All the presidents men were eating falafel for breakfast.", font="a"
+    )
+    assert (
+        printer.output == b"All the presidents men were eating falafel\nfor breakfast."
+    )
 
 
 def test_textln():
     printer = get_printer()
-    printer.textln('hello, world')
-    assert printer.output == b'hello, world\n'
+    printer.textln("hello, world")
+    assert printer.output == b"hello, world\n"
 
 
 def test_textln_empty():
     printer = get_printer()
     printer.textln()
-    assert printer.output == b'\n'
+    assert printer.output == b"\n"
 
 
 def test_ln():
     printer = get_printer()
     printer.ln()
-    assert printer.output == b'\n'
+    assert printer.output == b"\n"
 
 
 def test_multiple_ln():
     printer = get_printer()
     printer.ln(3)
-    assert printer.output == b'\n\n\n'
+    assert printer.output == b"\n\n\n"
```

### Comparing `python-escpos-3.0a8/test/test_functions.py` & `python-escpos-3.0a9/test/test_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from nose.tools import assert_raises
 from escpos.printer import Dummy
 
 
 def test_line_spacing_code_gen():
     printer = Dummy()
     printer.line_spacing(10)
-    assert printer.output == b'\x1b3\n'
+    assert printer.output == b"\x1b3\n"
 
 
 def test_line_spacing_rest():
     printer = Dummy()
     printer.line_spacing()
-    assert printer.output == b'\x1b2'
+    assert printer.output == b"\x1b2"
 
 
 def test_line_spacing_error_handling():
     printer = Dummy()
     with assert_raises(ValueError):
         printer.line_spacing(99, divisor=44)
     with assert_raises(ValueError):
```

### Comparing `python-escpos-3.0a8/test/test_image.py` & `python-escpos-3.0a9/test/test_image.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,61 +11,71 @@
 from escpos.image import EscposImage
 
 
 def test_image_black():
     """
     Test rendering solid black image
     """
-    for img_format in ['png', 'jpg', 'gif']:
-        _load_and_check_img('canvas_black.' + img_format, 1, 1, b'\x80', [b'\x80'])
+    for img_format in ["png", "jpg", "gif"]:
+        _load_and_check_img("canvas_black." + img_format, 1, 1, b"\x80", [b"\x80"])
 
 
 def test_image_black_transparent():
     """
     Test rendering black/transparent image
     """
-    for img_format in ['png', 'gif']:
-        _load_and_check_img('black_transparent.' + img_format, 2, 2, b'\xc0\x00', [b'\x80\x80'])
+    for img_format in ["png", "gif"]:
+        _load_and_check_img(
+            "black_transparent." + img_format, 2, 2, b"\xc0\x00", [b"\x80\x80"]
+        )
 
 
 def test_image_black_white():
     """
     Test rendering black/white image
     """
-    for img_format in ['png', 'jpg', 'gif']:
-        _load_and_check_img('black_white.' + img_format, 2, 2, b'\xc0\x00', [b'\x80\x80'])
+    for img_format in ["png", "jpg", "gif"]:
+        _load_and_check_img(
+            "black_white." + img_format, 2, 2, b"\xc0\x00", [b"\x80\x80"]
+        )
 
 
 def test_image_white():
     """
     Test rendering solid white image
     """
-    for img_format in ['png', 'jpg', 'gif']:
-        _load_and_check_img('canvas_white.' + img_format, 1, 1, b'\x00', [b'\x00'])
+    for img_format in ["png", "jpg", "gif"]:
+        _load_and_check_img("canvas_white." + img_format, 1, 1, b"\x00", [b"\x00"])
 
 
 def test_split():
     """
     test whether the split-function works as expected
     """
-    im = EscposImage('test/resources/black_white.png')
+    im = EscposImage("test/resources/black_white.png")
     (upper_part, lower_part) = im.split(1)
     upper_part = EscposImage(upper_part)
     lower_part = EscposImage(lower_part)
-    assert(upper_part.width == lower_part.width == 2)
-    assert(upper_part.height == lower_part.height == 1)
-    assert(upper_part.to_raster_format() == b'\xc0')
-    assert(lower_part.to_raster_format() == b'\x00')
+    assert upper_part.width == lower_part.width == 2
+    assert upper_part.height == lower_part.height == 1
+    assert upper_part.to_raster_format() == b"\xc0"
+    assert lower_part.to_raster_format() == b"\x00"
 
 
-def _load_and_check_img(filename, width_expected, height_expected, raster_format_expected, column_format_expected):
+def _load_and_check_img(
+    filename,
+    width_expected,
+    height_expected,
+    raster_format_expected,
+    column_format_expected,
+):
     """
     Load an image, and test whether raster & column formatted output, sizes, etc match expectations.
     """
-    im = EscposImage('test/resources/' + filename)
-    assert(im.width == width_expected)
-    assert(im.height == height_expected)
-    assert(im.to_raster_format() == raster_format_expected)
-    i = 0 
+    im = EscposImage("test/resources/" + filename)
+    assert im.width == width_expected
+    assert im.height == height_expected
+    assert im.to_raster_format() == raster_format_expected
+    i = 0
     for row in im.to_column_format(False):
-        assert(row == column_format_expected[i])
+        assert row == column_format_expected[i]
         i += 1
```

### Comparing `python-escpos-3.0a8/test/test_magicencode.py` & `python-escpos-3.0a9/test/test_magicencode.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 
 class TestEncoder:
     """
     Tests the single encoders.
     """
 
     def test_can_encode(self):
-        assert not Encoder({'CP437': 1}).can_encode('CP437', u'€')
-        assert Encoder({'CP437': 1}).can_encode('CP437', u'á')
-        assert not Encoder({'foobar': 1}).can_encode('foobar', 'a')
+        assert not Encoder({"CP437": 1}).can_encode("CP437", "€")
+        assert Encoder({"CP437": 1}).can_encode("CP437", "á")
+        assert not Encoder({"foobar": 1}).can_encode("foobar", "a")
 
     def test_find_suitable_encoding(self):
-        assert not Encoder({'CP437': 1}).find_suitable_encoding(u'€')
-        assert Encoder({'CP858': 1}).find_suitable_encoding(u'€') == 'CP858'
+        assert not Encoder({"CP437": 1}).find_suitable_encoding("€")
+        assert Encoder({"CP858": 1}).find_suitable_encoding("€") == "CP858"
 
     @raises(ValueError)
     def test_get_encoding(self):
-        Encoder({}).get_encoding_name('latin1')
+        Encoder({}).get_encoding_name("latin1")
 
 
 class TestMagicEncode:
     """
     Tests the magic encode functionality.
     """
 
@@ -53,58 +53,58 @@
 
             :param driver:
             """
             with pytest.raises(Error):
                 MagicEncode(driver, disabled=True)
 
     class TestWriteWithEncoding:
-
         def test_init_from_none(self, driver):
             encode = MagicEncode(driver, encoding=None)
-            encode.write_with_encoding('CP858', '€ ist teuro.')
-            assert driver.output == b'\x1bt\x13\xd5 ist teuro.'
+            encode.write_with_encoding("CP858", "€ ist teuro.")
+            assert driver.output == b"\x1bt\x13\xd5 ist teuro."
 
         def test_change_from_another(self, driver):
-            encode = MagicEncode(driver, encoding='CP437')
-            encode.write_with_encoding('CP858', '€ ist teuro.')
-            assert driver.output == b'\x1bt\x13\xd5 ist teuro.'
+            encode = MagicEncode(driver, encoding="CP437")
+            encode.write_with_encoding("CP858", "€ ist teuro.")
+            assert driver.output == b"\x1bt\x13\xd5 ist teuro."
 
         def test_no_change(self, driver):
-            encode = MagicEncode(driver, encoding='CP858')
-            encode.write_with_encoding('CP858', '€ ist teuro.')
-            assert driver.output == b'\xd5 ist teuro.'
+            encode = MagicEncode(driver, encoding="CP858")
+            encode.write_with_encoding("CP858", "€ ist teuro.")
+            assert driver.output == b"\xd5 ist teuro."
 
     class TestWrite:
-
         def test_write(self, driver):
             encode = MagicEncode(driver)
-            encode.write('€ ist teuro.')
-            assert driver.output == b'\x1bt\x0f\xa4 ist teuro.'
+            encode.write("€ ist teuro.")
+            assert driver.output == b"\x1bt\x0f\xa4 ist teuro."
 
         def test_write_disabled(self, driver):
-            encode = MagicEncode(driver, encoding='CP437', disabled=True)
-            encode.write('€ ist teuro.')
-            assert driver.output == b'? ist teuro.'
+            encode = MagicEncode(driver, encoding="CP437", disabled=True)
+            encode.write("€ ist teuro.")
+            assert driver.output == b"? ist teuro."
 
         def test_write_no_codepage(self, driver):
             encode = MagicEncode(
-                driver, defaultsymbol="_", encoder=Encoder({'CP437': 1}),
-                encoding='CP437')
-            encode.write(u'€ ist teuro.')
-            assert driver.output == b'_ ist teuro.'
+                driver,
+                defaultsymbol="_",
+                encoder=Encoder({"CP437": 1}),
+                encoding="CP437",
+            )
+            encode.write("€ ist teuro.")
+            assert driver.output == b"_ ist teuro."
 
     class TestForceEncoding:
-
         def test(self, driver):
             encode = MagicEncode(driver)
-            encode.force_encoding('CP437')
-            assert driver.output == b'\x1bt\x00'
+            encode.force_encoding("CP437")
+            assert driver.output == b"\x1bt\x00"
 
-            encode.write('€ ist teuro.')
-            assert driver.output == b'\x1bt\x00? ist teuro.'
+            encode.write("€ ist teuro.")
+            assert driver.output == b"\x1bt\x00? ist teuro."
 
 
 try:
     import jaconv
 except ImportError:
     jaconv = None
 
@@ -115,9 +115,9 @@
     @example("カタカナ")
     @example("あいうえお")
     @example("ﾊﾝｶｸｶﾀｶﾅ")
     def test_accept(self, text):
         encode_katakana(text)
 
     def test_result(self):
-        assert encode_katakana('カタカナ') == b'\xb6\xc0\xb6\xc5'
-        assert encode_katakana("あいうえお") == b'\xb1\xb2\xb3\xb4\xb5'
+        assert encode_katakana("カタカナ") == b"\xb6\xc0\xb6\xc5"
+        assert encode_katakana("あいうえお") == b"\xb1\xb2\xb3\xb4\xb5"
```

### Comparing `python-escpos-3.0a8/test/test_printer_file.py` & `python-escpos-3.0a9/test/test_printer_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,37 +14,37 @@
 import pytest
 from hypothesis import given, settings
 from hypothesis.strategies import text
 
 import escpos.printer as printer
 
 if six.PY3:
-    mock_open_call = 'builtins.open'
+    mock_open_call = "builtins.open"
 else:
-    mock_open_call = '__builtin__.open'
+    mock_open_call = "__builtin__.open"
 
 
 @pytest.mark.skip("this test is broken and has to be fixed or discarded")
 @given(path=text())
 def test_load_file_printer(mocker, path):
     """test the loading of the file-printer"""
-    mock_escpos = mocker.patch('escpos.escpos.Escpos.__init__')
+    mock_escpos = mocker.patch("escpos.escpos.Escpos.__init__")
     mock_open = mocker.patch(mock_open_call)
     printer.File(devfile=path)
     assert mock_escpos.called
     mock_open.assert_called_with(path, "wb")
 
 
 @pytest.mark.skip("this test is broken and has to be fixed or discarded")
 @given(txt=text())
 def test_auto_flush(mocker, txt):
     """test auto_flush in file-printer"""
-    mock_escpos = mocker.patch('escpos.escpos.Escpos.__init__')
+    mock_escpos = mocker.patch("escpos.escpos.Escpos.__init__")
     mock_open = mocker.patch(mock_open_call)
-    mock_device = mocker.patch.object(printer.File, 'device')
+    mock_device = mocker.patch.object(printer.File, "device")
 
     p = printer.File(auto_flush=False)
     # inject the mocked device-object
     p.device = mock_device
     p._raw(txt)
     assert not mock_device.flush.called
     mock_device.reset_mock()
@@ -56,15 +56,15 @@
 
 
 @pytest.mark.skip("this test is broken and has to be fixed or discarded")
 @given(txt=text())
 def test_flush_on_close(mocker, txt):
     """test flush on close in file-printer"""
     mock_open = mocker.patch(mock_open_call)
-    mock_device = mocker.patch.object(printer.File, 'device')
+    mock_device = mocker.patch.object(printer.File, "device")
 
     p = printer.File(auto_flush=False)
     # inject the mocked device-object
     p.device = mock_device
     p._raw(txt)
     assert not mock_device.flush.called
     p.close()
```

### Comparing `python-escpos-3.0a8/test/test_profile.py` & `python-escpos-3.0a9/test/test_profile.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 import pytest
 from escpos.capabilities import get_profile, NotSupported, BARCODE_B, Profile
 
 
 @pytest.fixture
 def profile():
-    return get_profile('default')
+    return get_profile("default")
 
 
 class TestBaseProfile:
-    """Test the `BaseProfile` class.
-    """
+    """Test the `BaseProfile` class."""
 
     def test_get_font(self, profile):
         with pytest.raises(NotSupported):
-            assert profile.get_font('3')
+            assert profile.get_font("3")
         assert profile.get_font(1) == 1
-        assert profile.get_font('a') == 0
+        assert profile.get_font("a") == 0
 
     def test_supports(self, profile):
-        assert not profile.supports('asdf asdf')
+        assert not profile.supports("asdf asdf")
         assert profile.supports(BARCODE_B)
 
     def test_get_columns(self, profile):
-        assert profile.get_columns('a') > 5
+        assert profile.get_columns("a") > 5
         with pytest.raises(NotSupported):
-            assert profile.get_columns('asdfasdf')
+            assert profile.get_columns("asdfasdf")
 
 
 class TestCustomProfile:
-    """Test custom profile options with the `Profile` class.
-    """
+    """Test custom profile options with the `Profile` class."""
 
     def test_columns(self):
-        assert Profile(columns=10).get_columns('sdfasdf') == 10
+        assert Profile(columns=10).get_columns("sdfasdf") == 10
 
     def test_features(self):
-        assert Profile(features={'foo': True}).supports('foo')
+        assert Profile(features={"foo": True}).supports("foo")
```

### Comparing `python-escpos-3.0a8/test/test_raise_arbitrary_error.py` & `python-escpos-3.0a9/test/test_raise_arbitrary_error.py`

 * *Files identical despite different names*

### Comparing `python-escpos-3.0a8/tox.ini` & `python-escpos-3.0a9/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 [tox]
-envlist = py35, py36, py37, py38, docs, flake8
+envlist = py37, py38, py39, py310, py311, docs, flake8
 
 [gh-actions]
 python =
     2.7: py27
     3.6: py36
     3.7: py37
     3.8: py38
+    3.9: py39
+    3.10: py310
+    3.11: py311
 
 [testenv]
 deps = nose
        jaconv
        coverage
        scripttest
        mock
        pytest!=3.2.0,!=3.3.0
        pytest-cov
        pytest-mock
        hypothesis>4
        python-barcode
 commands = pytest --cov escpos
-passenv = ESCPOS_CAPABILITIES_PICKLE_DIR ESCPOS_CAPABILITIES_FILE CI TRAVIS TRAVIS_* APPVEYOR APPVEYOR_* CODECOV_*
+passenv = ESCPOS_CAPABILITIES_PICKLE_DIR, ESCPOS_CAPABILITIES_FILE, CI, TRAVIS, TRAVIS_*, APPVEYOR, APPVEYOR_*, CODECOV_*
 
 [testenv:docs]
 basepython = python
 changedir = doc
-deps = sphinx>=1.5.1
+deps = sphinx>=3.0.0
        setuptools_scm
        python-barcode
-       sphinxcontrib-spelling>=5
+       sphinxcontrib-spelling>=7.2.0
+       sphinx_rtd_theme
 commands = sphinx-build -W -b html -d {envtmpdir}/doctrees .  {envtmpdir}/html
 
 [testenv:flake8]
 basepython = python
 # TODO add flake8-future
 # TODO add flake8-docstrings
 deps = flake8
```

