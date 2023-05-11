# Comparing `tmp/pter-3.6.1.tar.gz` & `tmp/pter-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pter-3.6.1.tar", last modified: Sat Mar 11 09:07:33 2023, max compression
+gzip compressed data, was "pter-3.7.0.tar", last modified: Thu May 11 17:29:24 2023, max compression
```

## Comparing `pter-3.6.1.tar` & `pter-3.7.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-03-11 09:07:33.443464 pter-3.6.1/
--rw-r--r--   0 robert    (1000) robert    (1000)    11590 2023-03-11 09:02:43.000000 pter-3.6.1/CHANGELOG.md
--rw-r--r--   0 robert    (1000) robert    (1000)     1097 2022-04-15 06:59:55.000000 pter-3.6.1/LICENSE
--rw-r--r--   0 robert    (1000) robert    (1000)      218 2022-02-19 08:34:12.000000 pter-3.6.1/MANIFEST.in
--rw-r--r--   0 robert    (1000) robert    (1000)     2900 2023-03-11 09:07:33.440131 pter-3.6.1/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)     2313 2022-07-24 08:17:34.000000 pter-3.6.1/README.md
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-03-11 09:07:33.430131 pter-3.6.1/doc/
--rw-r--r--   0 robert    (1000) robert    (1000)   365846 2022-02-19 08:34:12.000000 pter-3.6.1/doc/pter-demo.gif
--rw-r--r--   0 robert    (1000) robert    (1000)    45810 2023-03-06 14:38:19.000000 pter-3.6.1/doc/pter.rst
--rw-r--r--   0 robert    (1000) robert    (1000)    29201 2022-02-19 08:34:12.000000 pter-3.6.1/doc/qpter.png
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-03-11 09:07:33.433464 pter-3.6.1/extras/
--rw-r--r--   0 robert    (1000) robert    (1000)     8834 2022-02-19 08:34:12.000000 pter-3.6.1/extras/example.conf
--rw-r--r--   0 robert    (1000) robert    (1000)      196 2022-02-19 08:34:12.000000 pter-3.6.1/extras/pter.desktop
--rw-r--r--   0 robert    (1000) robert    (1000)      296 2022-02-19 08:34:12.000000 pter-3.6.1/extras/qpter.desktop
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-03-11 09:07:33.433464 pter-3.6.1/man/
--rw-r--r--   0 robert    (1000) robert    (1000)    52818 2023-03-11 09:07:32.000000 pter-3.6.1/man/pter.1
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-03-11 09:07:33.436798 pter-3.6.1/pter/
--rw-r--r--   0 robert    (1000) robert    (1000)        0 2022-02-19 08:34:12.000000 pter-3.6.1/pter/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)     5055 2023-03-06 14:04:12.000000 pter-3.6.1/pter/common.py
--rw-r--r--   0 robert    (1000) robert    (1000)     6640 2023-03-06 14:14:47.000000 pter-3.6.1/pter/configuration.py
--rw-r--r--   0 robert    (1000) robert    (1000)    88291 2023-03-11 09:01:22.000000 pter-3.6.1/pter/curses.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-03-11 09:07:33.436798 pter-3.6.1/pter/docs/
--rw-r--r--   0 robert    (1000) robert    (1000)    82898 2023-03-11 09:07:32.000000 pter-3.6.1/pter/docs/pter.html
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-03-11 09:07:33.440131 pter-3.6.1/pter/icons/
--rw-r--r--   0 robert    (1000) robert    (1000)     1083 2022-02-19 08:34:12.000000 pter-3.6.1/pter/icons/qpter_16x16.png
--rw-r--r--   0 robert    (1000) robert    (1000)     1598 2022-02-19 08:34:12.000000 pter-3.6.1/pter/icons/qpter_32x32.png
--rw-r--r--   0 robert    (1000) robert    (1000)     5399 2022-02-19 08:34:12.000000 pter-3.6.1/pter/key.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4358 2022-04-13 13:28:24.000000 pter-3.6.1/pter/main.py
--rw-r--r--   0 robert    (1000) robert    (1000)    75198 2022-10-29 11:46:33.000000 pter-3.6.1/pter/qtui.py
--rw-r--r--   0 robert    (1000) robert    (1000)    19345 2022-02-19 08:34:12.000000 pter-3.6.1/pter/searcher.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2261 2022-02-19 08:34:12.000000 pter-3.6.1/pter/source.py
--rw-r--r--   0 robert    (1000) robert    (1000)       31 2022-02-19 08:34:12.000000 pter-3.6.1/pter/tr.py
--rw-r--r--   0 robert    (1000) robert    (1000)    17758 2022-11-26 09:24:26.000000 pter-3.6.1/pter/utils.py
--rw-r--r--   0 robert    (1000) robert    (1000)       23 2023-03-11 09:01:29.000000 pter-3.6.1/pter/version.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-03-11 09:07:33.436798 pter-3.6.1/pter.egg-info/
--rw-r--r--   0 robert    (1000) robert    (1000)     2900 2023-03-11 09:07:33.000000 pter-3.6.1/pter.egg-info/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)      747 2023-03-11 09:07:33.000000 pter-3.6.1/pter.egg-info/SOURCES.txt
--rw-r--r--   0 robert    (1000) robert    (1000)        1 2023-03-11 09:07:33.000000 pter-3.6.1/pter.egg-info/dependency_links.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       76 2023-03-11 09:07:33.000000 pter-3.6.1/pter.egg-info/entry_points.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       49 2023-03-11 09:07:33.000000 pter-3.6.1/pter.egg-info/requires.txt
--rw-r--r--   0 robert    (1000) robert    (1000)        5 2023-03-11 09:07:33.000000 pter-3.6.1/pter.egg-info/top_level.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-03-11 09:07:33.443464 pter-3.6.1/setup.cfg
--rw-r--r--   0 robert    (1000) robert    (1000)     2773 2022-02-19 08:34:12.000000 pter-3.6.1/setup.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-03-11 09:07:33.440131 pter-3.6.1/tests/
--rw-r--r--   0 robert    (1000) robert    (1000)     1518 2022-02-19 08:34:12.000000 pter-3.6.1/tests/test_displaynames.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1684 2022-10-31 18:55:16.000000 pter-3.6.1/tests/test_priochange.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1221 2022-02-19 08:34:12.000000 pter-3.6.1/tests/test_pter.py
--rw-r--r--   0 robert    (1000) robert    (1000)     6496 2022-02-19 08:34:12.000000 pter-3.6.1/tests/test_rec.py
--rw-r--r--   0 robert    (1000) robert    (1000)    12855 2022-02-19 08:34:12.000000 pter-3.6.1/tests/test_searcher.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1618 2022-02-19 08:34:12.000000 pter-3.6.1/tests/test_sorting.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1475 2022-02-19 08:34:12.000000 pter-3.6.1/tests/test_taskid.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 17:29:24.486706 pter-3.7.0/
+-rw-r--r--   0 robert    (1000) robert    (1000)    11813 2023-05-11 17:23:02.000000 pter-3.7.0/CHANGELOG.md
+-rw-r--r--   0 robert    (1000) robert    (1000)     1097 2022-04-15 06:59:55.000000 pter-3.7.0/LICENSE
+-rw-r--r--   0 robert    (1000) robert    (1000)      218 2022-02-19 08:34:12.000000 pter-3.7.0/MANIFEST.in
+-rw-r--r--   0 robert    (1000) robert    (1000)     2900 2023-05-11 17:29:24.483373 pter-3.7.0/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)     2313 2022-07-24 08:17:34.000000 pter-3.7.0/README.md
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 17:29:24.480039 pter-3.7.0/doc/
+-rw-r--r--   0 robert    (1000) robert    (1000)   365846 2022-02-19 08:34:12.000000 pter-3.7.0/doc/pter-demo.gif
+-rw-r--r--   0 robert    (1000) robert    (1000)    45973 2023-05-11 17:27:09.000000 pter-3.7.0/doc/pter.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)    29201 2022-02-19 08:34:12.000000 pter-3.7.0/doc/qpter.png
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 17:29:24.483373 pter-3.7.0/extras/
+-rw-r--r--   0 robert    (1000) robert    (1000)     8834 2022-02-19 08:34:12.000000 pter-3.7.0/extras/example.conf
+-rw-r--r--   0 robert    (1000) robert    (1000)      196 2022-02-19 08:34:12.000000 pter-3.7.0/extras/pter.desktop
+-rw-r--r--   0 robert    (1000) robert    (1000)      296 2022-02-19 08:34:12.000000 pter-3.7.0/extras/qpter.desktop
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 17:29:24.483373 pter-3.7.0/man/
+-rw-r--r--   0 robert    (1000) robert    (1000)    53014 2023-05-11 17:29:24.000000 pter-3.7.0/man/pter.1
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 17:29:24.483373 pter-3.7.0/pter/
+-rw-r--r--   0 robert    (1000) robert    (1000)        0 2023-05-11 17:11:53.000000 pter-3.7.0/pter/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     5089 2023-05-11 17:11:53.000000 pter-3.7.0/pter/common.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     6686 2023-05-11 17:11:53.000000 pter-3.7.0/pter/configuration.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    89000 2023-05-11 17:11:53.000000 pter-3.7.0/pter/curses.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 17:29:24.483373 pter-3.7.0/pter/docs/
+-rw-r--r--   0 robert    (1000) robert    (1000)    83258 2023-05-11 17:29:24.000000 pter-3.7.0/pter/docs/pter.html
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 17:29:24.483373 pter-3.7.0/pter/icons/
+-rw-r--r--   0 robert    (1000) robert    (1000)     1083 2022-02-19 08:34:12.000000 pter-3.7.0/pter/icons/qpter_16x16.png
+-rw-r--r--   0 robert    (1000) robert    (1000)     1598 2022-02-19 08:34:12.000000 pter-3.7.0/pter/icons/qpter_32x32.png
+-rw-r--r--   0 robert    (1000) robert    (1000)     5399 2023-05-11 17:11:53.000000 pter-3.7.0/pter/key.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4358 2023-05-11 17:11:53.000000 pter-3.7.0/pter/main.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    75198 2023-05-11 17:11:53.000000 pter-3.7.0/pter/qtui.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    19345 2023-05-11 17:11:53.000000 pter-3.7.0/pter/searcher.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2261 2023-05-11 17:11:53.000000 pter-3.7.0/pter/source.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       31 2023-05-11 17:11:53.000000 pter-3.7.0/pter/tr.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    17809 2023-05-11 17:11:53.000000 pter-3.7.0/pter/utils.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       23 2023-05-11 17:27:33.000000 pter-3.7.0/pter/version.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 17:29:24.483373 pter-3.7.0/pter.egg-info/
+-rw-r--r--   0 robert    (1000) robert    (1000)     2900 2023-05-11 17:29:24.000000 pter-3.7.0/pter.egg-info/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)      747 2023-05-11 17:29:24.000000 pter-3.7.0/pter.egg-info/SOURCES.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)        1 2023-05-11 17:29:24.000000 pter-3.7.0/pter.egg-info/dependency_links.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       76 2023-05-11 17:29:24.000000 pter-3.7.0/pter.egg-info/entry_points.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       49 2023-05-11 17:29:24.000000 pter-3.7.0/pter.egg-info/requires.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)        5 2023-05-11 17:29:24.000000 pter-3.7.0/pter.egg-info/top_level.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-05-11 17:29:24.486706 pter-3.7.0/setup.cfg
+-rw-r--r--   0 robert    (1000) robert    (1000)     2773 2022-02-19 08:34:12.000000 pter-3.7.0/setup.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 17:29:24.483373 pter-3.7.0/tests/
+-rw-r--r--   0 robert    (1000) robert    (1000)     1518 2022-02-19 08:34:12.000000 pter-3.7.0/tests/test_displaynames.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1684 2022-10-31 18:55:16.000000 pter-3.7.0/tests/test_priochange.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1221 2022-02-19 08:34:12.000000 pter-3.7.0/tests/test_pter.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     6496 2022-02-19 08:34:12.000000 pter-3.7.0/tests/test_rec.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    12855 2022-02-19 08:34:12.000000 pter-3.7.0/tests/test_searcher.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1618 2022-02-19 08:34:12.000000 pter-3.7.0/tests/test_sorting.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1475 2022-02-19 08:34:12.000000 pter-3.7.0/tests/test_taskid.py
```

### Comparing `pter-3.6.1/CHANGELOG.md` & `pter-3.7.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Changelog
 
 This file contains the changes made between released versions.
 
 The format is based on [Keep a changelog](https://keepachangelog.com/) and the versioning tries to follow
 [Semantic Versioning](https://semver.org).
 
+
+## 3.7.0
+### Changed
+- When using templates, the initial cursor position will be after the creation date or at the start of the field
+
+### Added
+- When editing a task you can `Tab` through not-filled in keys, like `due:`
+
 ## 3.6.1
 ### Fixed
 - When scrolling past the end of list of tasks pter could crash (related to key sequences)
 
 
 ## 3.6.0
 ### Added
```

### Comparing `pter-3.6.1/LICENSE` & `pter-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pter-3.6.1/PKG-INFO` & `pter-3.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pter
-Version: 3.6.1
+Version: 3.7.0
 Summary: Console UI to manage your todo.txt file(s).
 Home-page: https://vonshednob.cc/pter
 Author: R
 Author-email: contact+pter@vonshednob.cc
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `pter-3.6.1/README.md` & `pter-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pter-3.6.1/doc/pter-demo.gif` & `pter-3.7.0/doc/pter-demo.gif`

 * *Files identical despite different names*

### Comparing `pter-3.6.1/doc/pter.rst` & `pter-3.7.0/doc/pter.rst`

 * *Files 1% similar despite different names*

```diff
@@ -360,14 +360,15 @@
  - ``del-left``, delete the character left of the cursor
  - ``del-right``, delete the character right of the cursor
  - ``del-to-bol``, delete all characters from the cursor to the beginning of the line
  - ``go-bol``, move the cursor to the beginning of the line
  - ``go-eol``, move the cursor to the end of the line
  - ``go-left``, move the cursor one character to the left
  - ``go-right``, move the cursor one charackter to the right
+ - ``goto-empty``, move the cursor to the next ``tag:value`` where the is no ``value``
  - ``submit-input``, accept the changes, leave the editor (applies the changes)
  - ``select-file``, when creating a new task, this allows you to select
    what todo.txt file to save the task in
  - ``comp-next``, next item in the completion list
  - ``comp-prev``, previous item in the completion list
  - ``comp-use``, use the selected item in the completion list
  - ``comp-close``, close the completion list
@@ -733,14 +734,15 @@
  - "Backspace", "^H": delete the character to the left of the cursor
  - "Del": delete the character under the cursor
  - "^U": delete from before the cursor to the start of the line
  - "Escape", "^C": cancel editing
  - "Enter", "Return": accept input and submit changes
  - "↓", "Tab", "^N": next item in the completion list
  - "↑", "^P": previous item in the completion list
+ - "Tab": jump to the next ``key:value`` field where there is not ``value``
  - "Enter": use the selected item of the completion list
  - "Esc", "^C": close the completion list
 
 
 qpter
 ------
```

### Comparing `pter-3.6.1/doc/qpter.png` & `pter-3.7.0/doc/qpter.png`

 * *Files identical despite different names*

### Comparing `pter-3.6.1/extras/example.conf` & `pter-3.7.0/extras/example.conf`

 * *Files identical despite different names*

### Comparing `pter-3.6.1/man/pter.1` & `pter-3.7.0/man/pter.1`

 * *Files 0% similar despite different names*

```diff
@@ -513,14 +513,16 @@
 .IP \(bu 2
 \fBgo\-eol\fP, move the cursor to the end of the line
 .IP \(bu 2
 \fBgo\-left\fP, move the cursor one character to the left
 .IP \(bu 2
 \fBgo\-right\fP, move the cursor one charackter to the right
 .IP \(bu 2
+\fBgoto\-empty\fP, move the cursor to the next \fBtag:value\fP where the is no \fBvalue\fP
+.IP \(bu 2
 \fBsubmit\-input\fP, accept the changes, leave the editor (applies the changes)
 .IP \(bu 2
 \fBselect\-file\fP, when creating a new task, this allows you to select
 what todo.txt file to save the task in
 .IP \(bu 2
 \fBcomp\-next\fP, next item in the completion list
 .IP \(bu 2
@@ -1126,14 +1128,16 @@
 .IP \(bu 2
 \(dqEnter\(dq, \(dqReturn\(dq: accept input and submit changes
 .IP \(bu 2
 \(dq↓\(dq, \(dqTab\(dq, \(dq^N\(dq: next item in the completion list
 .IP \(bu 2
 \(dq↑\(dq, \(dq^P\(dq: previous item in the completion list
 .IP \(bu 2
+\(dqTab\(dq: jump to the next \fBkey:value\fP field where there is not \fBvalue\fP
+.IP \(bu 2
 \(dqEnter\(dq: use the selected item of the completion list
 .IP \(bu 2
 \(dqEsc\(dq, \(dq^C\(dq: close the completion list
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .SS qpter
```

### Comparing `pter-3.6.1/pter/common.py` & `pter-3.7.0/pter/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 SETTING_USE_COMPLETION = 'use-completion'
 SETTING_PROTOCOLS = 'protocols'
 SETTING_DELEG_MARKER = 'delegation-marker'
 SETTING_DELEG_ACTION = 'delegation-action'
 SETTING_DELEG_TO = 'delegation-to'
 SETTING_DEFAULT_THRESHOLD = 'default-threshold'
 SETTING_EXT_EDITOR = 'editor'
+SETTING_TAB_CYCLES = 'tab-cycles'
 SETTING_ADD_CREATED = 'add-creation-date'
 SETTING_SEARCH_CASE_SENSITIVE = 'search-case-sensitive'
 SETTING_SAFE_SAVE = 'safe-save'
 SETTING_SCROLL_MARGIN = 'scroll-margin'
 SETTING_SHOW_NUMBERS = 'show-numbers'
 SETTING_USE_COLORS = 'use-colors'
 SETTING_TASK_FORMAT = 'task-format'
```

### Comparing `pter-3.6.1/pter/configuration.py` & `pter-3.7.0/pter/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
             common.SETTING_DEFAULT_THRESHOLD: '',
             common.SETTING_HUMAN_DATES: '',
             common.SETTING_DELEG_MARKER: '@delegated',
             common.SETTING_DELEG_ACTION: common.DELEGATE_ACTION_NONE,
             common.SETTING_DELEG_TO: 'to',
             common.SETTING_EXT_EDITOR: '',
             common.SETTING_ADD_CREATED: 'yes',
+            common.SETTING_TAB_CYCLES: 'yes',
             common.SETTING_TASK_FORMAT: common.DEFAULT_TASK_FORMAT,
             common.SETTING_CLEAR_CONTEXT: '',
             common.SETTING_PROTOCOLS: 'http,https,mailto,ftp,ftps',
             common.SETTING_CREATE_FROM_SEARCH: 'no',
             common.SETTING_AUTO_ID: 'no',
             common.SETTING_HIDE_SEQUENTIAL: 'yes',
             common.SETTING_RELATED_SHOW_SELF: 'yes',
```

### Comparing `pter-3.6.1/pter/curses.py` & `pter-3.7.0/pter/curses.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
                'toggle-tracking': 'Start/stop tracking',
                'show-help': 'Help',
                'open-manual': 'Read the manual',
                'go-left': 'Go one character to the left',
                'go-right': 'Go one character to the right',
                'go-bol': 'Go to start of line',
                'go-eol': 'Go to end of line',
+               'goto-empty': 'Goto the next empty key',
                'del-left': 'Delete to the left',
                'del-right': 'Delete to the right',
                'del-to-bol': 'Delete to start of line',
                'submit-input': 'Apply changes',
                'select-file': 'Select file',
                'delegate': 'Delegate task',
                'delete': 'Delete task',
@@ -671,14 +672,22 @@
             must_repaint = self.scroll()
         elif fnc == 'go-bol':
             self.cursor = 0
             must_repaint = self.scroll()
         elif fnc == 'go-eol':
             self.cursor = len(self.text)
             must_repaint = self.scroll()
+        elif fnc == 'goto-empty':
+            empty_field = utils.EMPTY_FIELD_RE.search(self.text, self.cursor)
+            if empty_field is None and self.app.tab_cycles:
+                empty_field = utils.EMPTY_FIELD_RE.search(self.text, 0)
+            if empty_field:
+                self.cursor = min(len(self.text), empty_field.end(1))
+                must_repaint = self.scroll()
+
         elif len(str(key)) == 1:
             self.text = self.text[:self.cursor] + str(key) + self.text[self.cursor:]
             self.cursor += 1
             must_repaint = True
         else:
             handled = False
 
@@ -884,28 +893,30 @@
     def __init__(self, parent):
         super().__init__(parent, None)
         self.title = 'New task'
 
         add_creation_date = self.app.conf.bool(common.SETTING_GROUP_GENERAL, common.SETTING_ADD_CREATED)
         create_from_search = self.app.conf.bool(common.SETTING_GROUP_GENERAL, common.SETTING_CREATE_FROM_SEARCH)
         self.auto_id = self.app.conf.bool(common.SETTING_GROUP_GENERAL, common.SETTING_AUTO_ID)
+        self.editor.cursor = 1
 
         initial = []
         if add_creation_date:
-            initial.append(datetime.datetime.now().strftime(Task.DATE_FMT))
+            create_date = datetime.datetime.now().strftime(Task.DATE_FMT)
+            initial.append(create_date)
+            self.editor.cursor += len(create_date)
         if create_from_search:
             initial.append(utils.create_from_search(self.app.search))
         if self.app.selected_template is not None:
             initial.append(self.app.selected_template)
 
         initial = ' '.join([part for part in initial if len(part) > 0])
         if len(initial) > 0 and not initial.endswith(' '):
             initial += ' '
         self.editor.text = initial
-        self.editor.cursor = len(initial)
         self.editor.scroll()
 
         self.task = Task(initial, todotxt=self.app.sources[0])
 
     def handle_key(self, key):
         fnc = self.app.editor_key_mapping.get(str(key), None)
 
@@ -1086,15 +1097,15 @@
         lines += [('', ''), (tr('Search'), '')]
         lines += [(name, key) for name, key in self.collect_name_fnc(search_fncs, self.app.key_mapping)]
         lines += [('', ''), (tr('Change Tasks'), '')]
         lines += [(name, key) for name, key in self.collect_name_fnc(edt_fncs, self.app.key_mapping)]
         lines += [('', ''), (tr('Other'), '')]
         lines += [(name, key) for name, key in self.collect_name_fnc(other_fncs, self.app.key_mapping)]
 
-        edt_nav_fncs = ['go-left', 'go-right', 'go-bol', 'go-eol']
+        edt_nav_fncs = ['go-left', 'go-right', 'go-bol', 'go-eol', 'goto-empty']
         edt_edt_fncs = ['del-left', 'del-right', 'del-to-bol']
         edt_meta_fncs = ['cancel', 'submit-input']
         edt_comp_fncs = ['comp-next', 'comp-prev', 'comp-use', 'comp-close']
         lines += [('', ''), ('', ''), (tr('TASK EDITING'), ''), ('', ''), (tr('General'), '')]
         lines += [(name, key) for name, key in self.collect_name_fnc(edt_meta_fncs, self.app.editor_key_mapping)]
         lines += [('', ''), (tr('Navigation'), '')]
         lines += [(name, key) for name, key in self.collect_name_fnc(edt_nav_fncs, self.app.editor_key_mapping)]
@@ -1252,14 +1263,16 @@
                                          common.SETTING_REUSE_RECURRING, 'n')
         self.scroll_margin = conf.number(common.SETTING_GROUP_GENERAL,
                                          common.SETTING_SCROLL_MARGIN)
         self.safe_save = conf.bool(common.SETTING_GROUP_GENERAL,
                                    common.SETTING_SAFE_SAVE, 'y')
         self.use_completion = conf.bool(common.SETTING_GROUP_GENERAL,
                                         common.SETTING_USE_COMPLETION, 'y')
+        self.tab_cycles = conf.bool(common.SETTING_GROUP_GENERAL,
+                                        common.SETTING_TAB_CYCLES, 'y')
         self.trash_file = conf.path(common.SETTING_GROUP_GENERAL,
                                     common.SETTING_TRASHFILE,
                                     common.DEFAULT_TRASHFILE);
         self.delete_is = conf.get(common.SETTING_GROUP_GENERAL,
                                   common.SETTING_DELETE_IS,
                                   common.DELETE_OPTION_DISABLED)
         if self.delete_is not in common.DELETE_OPTIONS:
@@ -1343,14 +1356,15 @@
             ('=',): 'prio-none',
             }
         self.editor_key_mapping = {
             '^C': 'cancel',
             '<escape>': 'cancel',
             '<left>': 'go-left',
             '<right>': 'go-right',
+            '<tab>': 'goto-empty',
             '^U': 'del-to-bol',
             '<backspace>': 'del-left',
             '<del>': 'del-right',
             '<home>': 'go-bol',
             '<end>': 'go-eol',
             '<f6>': 'select-file',
             '<return>': 'submit-input',
```

### Comparing `pter-3.6.1/pter/docs/pter.html` & `pter-3.7.0/pter/docs/pter.html`

 * *Files 0% similar despite different names*

#### Comparing `pter-3.6.1/pter/docs/pter.html` & `pter-3.7.0/pter/docs/pter.html`

```diff
@@ -1387,14 +1387,23 @@
                 <tt class="docutils literal">
                   <span class="pre">go-right</span>
                 </tt>
                 , move the cursor one charackter to the right
               </li>
               <li>
                 <tt class="docutils literal">
+                  <span class="pre">goto-empty</span>
+                </tt>
+                , move the cursor to the next
+                <tt class="docutils literal">tag:value</tt>
+                where the is no
+                <tt class="docutils literal">value</tt>
+              </li>
+              <li>
+                <tt class="docutils literal">
                   <span class="pre">submit-input</span>
                 </tt>
                 , accept the changes, leave the editor (applies the changes)
               </li>
               <li>
                 <tt class="docutils literal">
                   <span class="pre">select-file</span>
@@ -2198,14 +2207,20 @@
               <li>&quot;Backspace&quot;, &quot;^H&quot;: delete the character to the left of the cursor</li>
               <li>&quot;Del&quot;: delete the character under the cursor</li>
               <li>&quot;^U&quot;: delete from before the cursor to the start of the line</li>
               <li>&quot;Escape&quot;, &quot;^C&quot;: cancel editing</li>
               <li>&quot;Enter&quot;, &quot;Return&quot;: accept input and submit changes</li>
               <li>&quot;↓&quot;, &quot;Tab&quot;, &quot;^N&quot;: next item in the completion list</li>
               <li>&quot;↑&quot;, &quot;^P&quot;: previous item in the completion list</li>
+              <li>
+                &quot;Tab&quot;: jump to the next
+                <tt class="docutils literal">key:value</tt>
+                field where there is not
+                <tt class="docutils literal">value</tt>
+              </li>
               <li>&quot;Enter&quot;: use the selected item of the completion list</li>
               <li>&quot;Esc&quot;, &quot;^C&quot;: close the completion list</li>
             </ul>
           </blockquote>
         </div>
         <div class="section" id="qpter">
           <h2>qpter</h2>
```

### Comparing `pter-3.6.1/pter/icons/qpter_16x16.png` & `pter-3.7.0/pter/icons/qpter_16x16.png`

 * *Files identical despite different names*

### Comparing `pter-3.6.1/pter/icons/qpter_32x32.png` & `pter-3.7.0/pter/icons/qpter_32x32.png`

 * *Files identical despite different names*

### Comparing `pter-3.6.1/pter/key.py` & `pter-3.7.0/pter/key.py`

 * *Files identical despite different names*

### Comparing `pter-3.6.1/pter/main.py` & `pter-3.7.0/pter/main.py`

 * *Files identical despite different names*

### Comparing `pter-3.6.1/pter/qtui.py` & `pter-3.7.0/pter/qtui.py`

 * *Files identical despite different names*

### Comparing `pter-3.6.1/pter/searcher.py` & `pter-3.7.0/pter/searcher.py`

 * *Files identical despite different names*

### Comparing `pter-3.6.1/pter/source.py` & `pter-3.7.0/pter/source.py`

 * *Files identical despite different names*

### Comparing `pter-3.6.1/pter/utils.py` & `pter-3.7.0/pter/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from pter import common
 from pter.searcher import get_relative_date
 from pter.source import Source
 
 
 DATETIME_FMT = '%Y-%m-%d-%H-%M-%S'
 FORMAT_TOKEN_RE = re.compile('^([^a-z]*)([a-z][a-z-]*)(.*)$')
+EMPTY_FIELD_RE = re.compile('([a-z]+[:])(?:\s|$)')
 
 
 def duration_as_str(duration):
     seconds = int(duration.total_seconds())
     hours = seconds // 3600
     minutes = (seconds % 3600) // 60
```

### Comparing `pter-3.6.1/pter.egg-info/PKG-INFO` & `pter-3.7.0/pter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pter
-Version: 3.6.1
+Version: 3.7.0
 Summary: Console UI to manage your todo.txt file(s).
 Home-page: https://vonshednob.cc/pter
 Author: R
 Author-email: contact+pter@vonshednob.cc
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `pter-3.6.1/pter.egg-info/SOURCES.txt` & `pter-3.7.0/pter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pter-3.6.1/setup.py` & `pter-3.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `pter-3.6.1/tests/test_displaynames.py` & `pter-3.7.0/tests/test_displaynames.py`

 * *Files identical despite different names*

### Comparing `pter-3.6.1/tests/test_priochange.py` & `pter-3.7.0/tests/test_priochange.py`

 * *Files identical despite different names*

### Comparing `pter-3.6.1/tests/test_pter.py` & `pter-3.7.0/tests/test_pter.py`

 * *Files identical despite different names*

### Comparing `pter-3.6.1/tests/test_rec.py` & `pter-3.7.0/tests/test_rec.py`

 * *Files identical despite different names*

### Comparing `pter-3.6.1/tests/test_searcher.py` & `pter-3.7.0/tests/test_searcher.py`

 * *Files identical despite different names*

### Comparing `pter-3.6.1/tests/test_sorting.py` & `pter-3.7.0/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `pter-3.6.1/tests/test_taskid.py` & `pter-3.7.0/tests/test_taskid.py`

 * *Files identical despite different names*

