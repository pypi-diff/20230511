# Comparing `tmp/Xhpc-2.9.tar.gz` & `tmp/Xhpc-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Xhpc-2.9.tar", last modified: Tue Apr 25 22:13:14 2023, max compression
+gzip compressed data, was "Xhpc-2.9.1.tar", last modified: Thu May 11 00:30:06 2023, max compression
```

## Comparing `Xhpc-2.9.tar` & `Xhpc-2.9.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 franck     (501) staff       (20)        0 2023-04-25 22:13:14.506501 Xhpc-2.9/
--rw-r--r--   0 franck     (501) staff       (20)     1657 2022-04-20 13:12:04.000000 Xhpc-2.9/LICENCE
--rw-r--r--   0 franck     (501) staff       (20)    11323 2023-04-25 22:13:14.506162 Xhpc-2.9/PKG-INFO
--rwxr-xr-x   0 franck     (501) staff       (20)    10430 2022-05-04 09:21:13.000000 Xhpc-2.9/README.md
-drwxr-xr-x   0 franck     (501) staff       (20)        0 2023-04-25 22:13:14.496476 Xhpc-2.9/Xhpc/
--rw-r--r--   0 franck     (501) staff       (20)      358 2023-04-25 22:12:04.000000 Xhpc-2.9/Xhpc/__init__.py
--rw-r--r--   0 franck     (501) staff       (20)      652 2022-04-22 15:33:48.000000 Xhpc-2.9/Xhpc/assess.py
--rw-r--r--   0 franck     (501) staff       (20)     9681 2022-07-04 08:57:11.000000 Xhpc-2.9/Xhpc/cmd.py
--rw-r--r--   0 franck     (501) staff       (20)     8732 2022-07-05 15:04:42.000000 Xhpc-2.9/Xhpc/directives.py
--rw-r--r--   0 franck     (501) staff       (20)     3542 2022-04-28 14:03:34.000000 Xhpc-2.9/Xhpc/email.py
--rw-r--r--   0 franck     (501) staff       (20)     4461 2022-05-18 23:12:36.000000 Xhpc-2.9/Xhpc/env.py
--rw-r--r--   0 franck     (501) staff       (20)    15588 2022-07-07 13:28:11.000000 Xhpc-2.9/Xhpc/io_utils.py
--rw-r--r--   0 franck     (501) staff       (20)     6313 2022-10-11 09:00:05.000000 Xhpc-2.9/Xhpc/nodes.py
--rw-r--r--   0 franck     (501) staff       (20)     6010 2022-10-11 12:59:50.000000 Xhpc-2.9/Xhpc/preamble.py
--rw-r--r--   0 franck     (501) staff       (20)    12492 2022-07-20 10:29:54.000000 Xhpc-2.9/Xhpc/relocate.py
--rw-r--r--   0 franck     (501) staff       (20)     4849 2022-05-12 08:45:39.000000 Xhpc-2.9/Xhpc/scratches.py
-drwxr-xr-x   0 franck     (501) staff       (20)        0 2023-04-25 22:13:14.499651 Xhpc-2.9/Xhpc/scripts/
--rw-r--r--   0 franck     (501) staff       (20)      376 2022-04-20 13:03:44.000000 Xhpc-2.9/Xhpc/scripts/__init__.py
--rwxr-xr-x   0 franck     (501) staff       (20)     7518 2023-04-25 22:11:10.000000 Xhpc-2.9/Xhpc/scripts/_standalone_xhpc.py
-drwxr-xr-x   0 franck     (501) staff       (20)        0 2023-04-25 22:13:14.505434 Xhpc-2.9/Xhpc/test/
--rw-r--r--   0 franck     (501) staff       (20)        0 2022-04-01 16:31:50.000000 Xhpc-2.9/Xhpc/test/__init__.py
--rw-r--r--   0 franck     (501) staff       (20)     9370 2022-07-04 08:56:37.000000 Xhpc-2.9/Xhpc/test/test_cmd.py
--rw-r--r--   0 franck     (501) staff       (20)     4777 2022-05-06 07:35:32.000000 Xhpc-2.9/Xhpc/test/test_directives.py
--rw-r--r--   0 franck     (501) staff       (20)     5097 2022-04-28 17:14:35.000000 Xhpc-2.9/Xhpc/test/test_email.py
--rw-r--r--   0 franck     (501) staff       (20)     5007 2022-04-28 17:14:35.000000 Xhpc-2.9/Xhpc/test/test_env.py
--rw-r--r--   0 franck     (501) staff       (20)    12483 2022-07-04 08:58:42.000000 Xhpc-2.9/Xhpc/test/test_io_utils.py
--rw-r--r--   0 franck     (501) staff       (20)     1800 2022-07-04 08:59:55.000000 Xhpc-2.9/Xhpc/test/test_nodes.py
--rw-r--r--   0 franck     (501) staff       (20)     7634 2022-07-04 09:14:57.000000 Xhpc-2.9/Xhpc/test/test_preamble.py
--rw-r--r--   0 franck     (501) staff       (20)     7291 2022-07-04 09:19:47.000000 Xhpc-2.9/Xhpc/test/test_relocate.py
--rw-r--r--   0 franck     (501) staff       (20)     6276 2022-05-12 15:32:37.000000 Xhpc-2.9/Xhpc/test/test_scratches.py
--rwxr-xr-x   0 franck     (501) staff       (20)     5388 2022-10-11 09:04:21.000000 Xhpc-2.9/Xhpc/xhpc.py
-drwxr-xr-x   0 franck     (501) staff       (20)        0 2023-04-25 22:13:14.498710 Xhpc-2.9/Xhpc.egg-info/
--rw-r--r--   0 franck     (501) staff       (20)    11323 2023-04-25 22:13:14.000000 Xhpc-2.9/Xhpc.egg-info/PKG-INFO
--rw-r--r--   0 franck     (501) staff       (20)      691 2023-04-25 22:13:14.000000 Xhpc-2.9/Xhpc.egg-info/SOURCES.txt
--rw-r--r--   0 franck     (501) staff       (20)        1 2023-04-25 22:13:14.000000 Xhpc-2.9/Xhpc.egg-info/dependency_links.txt
--rw-r--r--   0 franck     (501) staff       (20)       71 2023-04-25 22:13:14.000000 Xhpc-2.9/Xhpc.egg-info/entry_points.txt
--rw-r--r--   0 franck     (501) staff       (20)       20 2023-04-25 22:13:14.000000 Xhpc-2.9/Xhpc.egg-info/requires.txt
--rw-r--r--   0 franck     (501) staff       (20)        5 2023-04-25 22:13:14.000000 Xhpc-2.9/Xhpc.egg-info/top_level.txt
--rw-r--r--   0 franck     (501) staff       (20)       38 2023-04-25 22:13:14.506573 Xhpc-2.9/setup.cfg
--rwxr-xr-x   0 franck     (501) staff       (20)     1970 2022-04-20 16:00:34.000000 Xhpc-2.9/setup.py
+drwxr-xr-x   0 franck     (501) staff       (20)        0 2023-05-11 00:30:06.723163 Xhpc-2.9.1/
+-rw-r--r--   0 franck     (501) staff       (20)     1657 2022-04-20 13:12:04.000000 Xhpc-2.9.1/LICENCE
+-rw-r--r--   0 franck     (501) staff       (20)    11325 2023-05-11 00:30:06.722718 Xhpc-2.9.1/PKG-INFO
+-rwxr-xr-x   0 franck     (501) staff       (20)    10430 2022-05-04 09:21:13.000000 Xhpc-2.9.1/README.md
+drwxr-xr-x   0 franck     (501) staff       (20)        0 2023-05-11 00:30:06.709911 Xhpc-2.9.1/Xhpc/
+-rw-r--r--   0 franck     (501) staff       (20)      360 2023-05-11 00:29:38.000000 Xhpc-2.9.1/Xhpc/__init__.py
+-rw-r--r--   0 franck     (501) staff       (20)      652 2022-04-22 15:33:48.000000 Xhpc-2.9.1/Xhpc/assess.py
+-rw-r--r--   0 franck     (501) staff       (20)     9681 2022-07-04 08:57:11.000000 Xhpc-2.9.1/Xhpc/cmd.py
+-rw-r--r--   0 franck     (501) staff       (20)     8732 2022-07-05 15:04:42.000000 Xhpc-2.9.1/Xhpc/directives.py
+-rw-r--r--   0 franck     (501) staff       (20)     3542 2022-04-28 14:03:34.000000 Xhpc-2.9.1/Xhpc/email.py
+-rw-r--r--   0 franck     (501) staff       (20)     4461 2022-05-18 23:12:36.000000 Xhpc-2.9.1/Xhpc/env.py
+-rw-r--r--   0 franck     (501) staff       (20)    15588 2022-07-07 13:28:11.000000 Xhpc-2.9.1/Xhpc/io_utils.py
+-rw-r--r--   0 franck     (501) staff       (20)     6313 2022-10-11 09:00:05.000000 Xhpc-2.9.1/Xhpc/nodes.py
+-rw-r--r--   0 franck     (501) staff       (20)     6010 2023-05-11 00:28:29.000000 Xhpc-2.9.1/Xhpc/preamble.py
+-rw-r--r--   0 franck     (501) staff       (20)    12492 2022-07-20 10:29:54.000000 Xhpc-2.9.1/Xhpc/relocate.py
+-rw-r--r--   0 franck     (501) staff       (20)     4849 2022-05-12 08:45:39.000000 Xhpc-2.9.1/Xhpc/scratches.py
+drwxr-xr-x   0 franck     (501) staff       (20)        0 2023-05-11 00:30:06.718875 Xhpc-2.9.1/Xhpc/scripts/
+-rw-r--r--   0 franck     (501) staff       (20)      376 2022-04-20 13:03:44.000000 Xhpc-2.9.1/Xhpc/scripts/__init__.py
+-rwxr-xr-x   0 franck     (501) staff       (20)     7518 2023-04-25 22:11:10.000000 Xhpc-2.9.1/Xhpc/scripts/_standalone_xhpc.py
+drwxr-xr-x   0 franck     (501) staff       (20)        0 2023-05-11 00:30:06.722276 Xhpc-2.9.1/Xhpc/test/
+-rw-r--r--   0 franck     (501) staff       (20)        0 2022-04-01 16:31:50.000000 Xhpc-2.9.1/Xhpc/test/__init__.py
+-rw-r--r--   0 franck     (501) staff       (20)     9370 2022-07-04 08:56:37.000000 Xhpc-2.9.1/Xhpc/test/test_cmd.py
+-rw-r--r--   0 franck     (501) staff       (20)     4777 2022-05-06 07:35:32.000000 Xhpc-2.9.1/Xhpc/test/test_directives.py
+-rw-r--r--   0 franck     (501) staff       (20)     5097 2022-04-28 17:14:35.000000 Xhpc-2.9.1/Xhpc/test/test_email.py
+-rw-r--r--   0 franck     (501) staff       (20)     5007 2022-04-28 17:14:35.000000 Xhpc-2.9.1/Xhpc/test/test_env.py
+-rw-r--r--   0 franck     (501) staff       (20)    12483 2022-07-04 08:58:42.000000 Xhpc-2.9.1/Xhpc/test/test_io_utils.py
+-rw-r--r--   0 franck     (501) staff       (20)     1800 2022-07-04 08:59:55.000000 Xhpc-2.9.1/Xhpc/test/test_nodes.py
+-rw-r--r--   0 franck     (501) staff       (20)     7634 2022-07-04 09:14:57.000000 Xhpc-2.9.1/Xhpc/test/test_preamble.py
+-rw-r--r--   0 franck     (501) staff       (20)     7291 2022-07-04 09:19:47.000000 Xhpc-2.9.1/Xhpc/test/test_relocate.py
+-rw-r--r--   0 franck     (501) staff       (20)     6276 2022-05-12 15:32:37.000000 Xhpc-2.9.1/Xhpc/test/test_scratches.py
+-rwxr-xr-x   0 franck     (501) staff       (20)     5388 2022-10-11 09:04:21.000000 Xhpc-2.9.1/Xhpc/xhpc.py
+drwxr-xr-x   0 franck     (501) staff       (20)        0 2023-05-11 00:30:06.718087 Xhpc-2.9.1/Xhpc.egg-info/
+-rw-r--r--   0 franck     (501) staff       (20)    11325 2023-05-11 00:30:06.000000 Xhpc-2.9.1/Xhpc.egg-info/PKG-INFO
+-rw-r--r--   0 franck     (501) staff       (20)      691 2023-05-11 00:30:06.000000 Xhpc-2.9.1/Xhpc.egg-info/SOURCES.txt
+-rw-r--r--   0 franck     (501) staff       (20)        1 2023-05-11 00:30:06.000000 Xhpc-2.9.1/Xhpc.egg-info/dependency_links.txt
+-rw-r--r--   0 franck     (501) staff       (20)       71 2023-05-11 00:30:06.000000 Xhpc-2.9.1/Xhpc.egg-info/entry_points.txt
+-rw-r--r--   0 franck     (501) staff       (20)       20 2023-05-11 00:30:06.000000 Xhpc-2.9.1/Xhpc.egg-info/requires.txt
+-rw-r--r--   0 franck     (501) staff       (20)        5 2023-05-11 00:30:06.000000 Xhpc-2.9.1/Xhpc.egg-info/top_level.txt
+-rw-r--r--   0 franck     (501) staff       (20)       38 2023-05-11 00:30:06.723264 Xhpc-2.9.1/setup.cfg
+-rwxr-xr-x   0 franck     (501) staff       (20)     1970 2022-04-20 16:00:34.000000 Xhpc-2.9.1/setup.py
```

### Comparing `Xhpc-2.9/LICENCE` & `Xhpc-2.9.1/LICENCE`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/PKG-INFO` & `Xhpc-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xhpc
-Version: 2.9
+Version: 2.9.1
 Summary: Xhpc is a command line tool allowing the conversion of a sh/bash script into a Slurm (or Torque) script with directives for use on a computercluster.
 Home-page: https://github.com/FranckLejzerowicz/Xhpc
 Author: Franck Lejzerowicz
 Author-email: franck.lejzerowicz@gmail.com
 Maintainer: Franck Lejzerowicz
 Maintainer-email: franck.lejzerowicz@gmail.com
 License: BSD
```

### Comparing `Xhpc-2.9/README.md` & `Xhpc-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc/assess.py` & `Xhpc-2.9.1/Xhpc/assess.py`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc/cmd.py` & `Xhpc-2.9.1/Xhpc/cmd.py`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc/directives.py` & `Xhpc-2.9.1/Xhpc/directives.py`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc/email.py` & `Xhpc-2.9.1/Xhpc/email.py`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc/env.py` & `Xhpc-2.9.1/Xhpc/env.py`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc/io_utils.py` & `Xhpc-2.9.1/Xhpc/io_utils.py`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc/nodes.py` & `Xhpc-2.9.1/Xhpc/nodes.py`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc/preamble.py` & `Xhpc-2.9.1/Xhpc/preamble.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     # if a conda environment is used
     if args['env']:
         # activate the env
         env = ['\n# active conda environment',
                'echo "Conda environment is %s"' % args['env']]
         if args['saga']:
             env.extend([
-                'module load Anaconda3/2019.03',
+                'module load Anaconda3/2022.10',
                 'export PS1=\\$',
                 'source ${EBROOTANACONDA3}/etc/profile.d/conda.sh',
                 'conda deactivate &>/dev/null'])
         env.append('conda activate %s' % args['env'])
         if args['saga']:
             env.append('module purge')
         args['preamble'].extend(env)
```

### Comparing `Xhpc-2.9/Xhpc/relocate.py` & `Xhpc-2.9.1/Xhpc/relocate.py`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc/scratches.py` & `Xhpc-2.9.1/Xhpc/scratches.py`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc/scripts/_standalone_xhpc.py` & `Xhpc-2.9.1/Xhpc/scripts/_standalone_xhpc.py`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc/test/test_cmd.py` & `Xhpc-2.9.1/Xhpc/test/test_cmd.py`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc/test/test_directives.py` & `Xhpc-2.9.1/Xhpc/test/test_directives.py`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc/test/test_email.py` & `Xhpc-2.9.1/Xhpc/test/test_email.py`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc/test/test_env.py` & `Xhpc-2.9.1/Xhpc/test/test_env.py`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc/test/test_io_utils.py` & `Xhpc-2.9.1/Xhpc/test/test_io_utils.py`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc/test/test_nodes.py` & `Xhpc-2.9.1/Xhpc/test/test_nodes.py`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc/test/test_preamble.py` & `Xhpc-2.9.1/Xhpc/test/test_preamble.py`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc/test/test_relocate.py` & `Xhpc-2.9.1/Xhpc/test/test_relocate.py`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc/test/test_scratches.py` & `Xhpc-2.9.1/Xhpc/test/test_scratches.py`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc/xhpc.py` & `Xhpc-2.9.1/Xhpc/xhpc.py`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/Xhpc.egg-info/PKG-INFO` & `Xhpc-2.9.1/Xhpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xhpc
-Version: 2.9
+Version: 2.9.1
 Summary: Xhpc is a command line tool allowing the conversion of a sh/bash script into a Slurm (or Torque) script with directives for use on a computercluster.
 Home-page: https://github.com/FranckLejzerowicz/Xhpc
 Author: Franck Lejzerowicz
 Author-email: franck.lejzerowicz@gmail.com
 Maintainer: Franck Lejzerowicz
 Maintainer-email: franck.lejzerowicz@gmail.com
 License: BSD
```

### Comparing `Xhpc-2.9/Xhpc.egg-info/SOURCES.txt` & `Xhpc-2.9.1/Xhpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Xhpc-2.9/setup.py` & `Xhpc-2.9.1/setup.py`

 * *Files identical despite different names*

