# Comparing `tmp/symlib-1.3.0.tar.gz` & `tmp/symlib-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symlib-1.3.0.tar", last modified: Sat May  6 00:43:31 2023, max compression
+gzip compressed data, was "symlib-1.3.1.tar", last modified: Thu May 11 04:10:28 2023, max compression
```

## Comparing `symlib-1.3.0.tar` & `symlib-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-06 00:43:31.923970 symlib-1.3.0/
--rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.3.0/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-05-06 00:43:31.923856 symlib-1.3.0/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.3.0/README.md
--rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.3.0/pyproject.toml
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-05-06 00:43:31.924003 symlib-1.3.0/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)      885 2023-05-06 00:43:24.000000 symlib-1.3.0/setup.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-06 00:43:31.923139 symlib-1.3.0/symlib/
--rw-r--r--   0 phil       (501) staff       (20)     1629 2023-04-18 17:25:19.000000 symlib-1.3.0/symlib/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.3.0/symlib/file_management.py
--rw-r--r--   0 phil       (501) staff       (20)    46482 2023-05-06 00:43:01.000000 symlib-1.3.0/symlib/lib.py
--rw-r--r--   0 phil       (501) staff       (20)    35330 2023-04-11 22:48:38.000000 symlib-1.3.0/symlib/star_tagging.py
--rw-r--r--   0 phil       (501) staff       (20)     8508 2023-05-06 00:43:01.000000 symlib-1.3.0/symlib/util.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-06 00:43:31.923700 symlib-1.3.0/symlib.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-05-06 00:43:31.000000 symlib-1.3.0/symlib.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      287 2023-05-06 00:43:31.000000 symlib-1.3.0/symlib.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-05-06 00:43:31.000000 symlib-1.3.0/symlib.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       41 2023-05-06 00:43:31.000000 symlib-1.3.0/symlib.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)        7 2023-05-06 00:43:31.000000 symlib-1.3.0/symlib.egg-info/top_level.txt
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-11 04:10:28.610875 symlib-1.3.1/
+-rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.3.1/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-05-11 04:10:28.610760 symlib-1.3.1/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.3.1/README.md
+-rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.3.1/pyproject.toml
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-05-11 04:10:28.610906 symlib-1.3.1/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)      885 2023-05-11 04:10:25.000000 symlib-1.3.1/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-11 04:10:28.609911 symlib-1.3.1/symlib/
+-rw-r--r--   0 phil       (501) staff       (20)     1629 2023-04-18 17:25:19.000000 symlib-1.3.1/symlib/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.3.1/symlib/file_management.py
+-rw-r--r--   0 phil       (501) staff       (20)    47959 2023-05-11 04:10:25.000000 symlib-1.3.1/symlib/lib.py
+-rw-r--r--   0 phil       (501) staff       (20)    35330 2023-04-11 22:48:38.000000 symlib-1.3.1/symlib/star_tagging.py
+-rw-r--r--   0 phil       (501) staff       (20)     8508 2023-05-06 00:43:01.000000 symlib-1.3.1/symlib/util.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-11 04:10:28.610585 symlib-1.3.1/symlib.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-05-11 04:10:28.000000 symlib-1.3.1/symlib.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      287 2023-05-11 04:10:28.000000 symlib-1.3.1/symlib.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-05-11 04:10:28.000000 symlib-1.3.1/symlib.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       41 2023-05-11 04:10:28.000000 symlib-1.3.1/symlib.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)        7 2023-05-11 04:10:28.000000 symlib-1.3.1/symlib.egg-info/top_level.txt
```

### Comparing `symlib-1.3.0/LICENSE` & `symlib-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `symlib-1.3.0/PKG-INFO` & `symlib-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.3.0
+Version: 1.3.1
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `symlib-1.3.0/setup.py` & `symlib-1.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import setuptools
-version = "1.3.0"
+version = "1.3.1"
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="symlib",
     version=version,
```

### Comparing `symlib-1.3.0/symlib/__init__.py` & `symlib-1.3.1/symlib/__init__.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.0/symlib/file_management.py` & `symlib-1.3.1/symlib/file_management.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.0/symlib/lib.py` & `symlib-1.3.1/symlib/lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,18 @@
 """
 HISTORY_DTYPE = [("mpeak", "f4"), ("vpeak", "f4"), ("merger_snap", "i4"),
                  ("merger_ratio", "f4"),
                  ("start", "i4"), ("end", "i4"), ("is_real", "?"),
                  ("is_disappear", "?"), ("is_main_sub", "?"),
                  ("preprocess", "i4"), ("first_infall_snap", "i4"),
                  ("branch_idx", "i4"), ("false_selection", "?"),
-                 ("mpeak_pre", "f4")]
+                 ("mpeak_pre", "f4"), ("conv_snap_discrete", "i4"),
+                 ("conv_snap_eps", "i4"), ("conv_snap_relax", "i4"),
+                 ("conv_snap_relax_hydro", "i4"), ("disrupt_snap", "i4"),
+                 ("disrupt_snap_rs", "i4")]
 
 
 """ BRANCH_DTYPE is a numpy datatype representing the main branch of of halo's
 merger tree. This forms a component of HISTORY_DTYPE, which 
  - The main branch of a given halo within the depth-first merger tree can be 
    found with x[start:end].
  - is_real: false if a halo is definitely a numerical artefact (e.g. if it's
@@ -515,17 +518,46 @@
                                         h["first_infall_snap"][i])
 
         infall_snap = h["first_infall_snap"][i]
         mpeak_infall = np.max(s[i,:infall_snap+1]["mvir"])
         h["mpeak_pre"][i] = mpeak_infall
         h["false_selection"][i] = mpeak_infall < 300*param["mp"]
 
+    (snap_discrete, snap_eps,
+     snap_relax, snap_relax_hydro,
+     disrupt_snap, disrupt_snap_rs) = read_convergence_limits(dir_name)
+    if snap_discrete is not None:
+        h["conv_snap_discrete"] = snap_discrete
+        h["conv_snap_eps"] = snap_eps
+        h["conv_snap_relax"] = snap_relax
+        h["conv_snap_relax_hydro"] = snap_relax_hydro
+        h["disrupt_snap"] = disrupt_snap
+        h["disrupt_snap_rs"] = disrupt_snap_rs
+
     return h
 
-def read_cores(dir_name, include_false_selections=False, suffix="fid"):
+def read_convergence_limits(sim_dir):
+    file_name = path.join(sim_dir, "convergence_limits.dat")
+    if not path.exists(file_name): return None, None, None, None, None, None
+
+    try:
+        with open(file_name, "rb") as fp:
+            n_halo, = struct.unpack("q", fp.read(8))
+            snap_discrete = np.fromfile(fp, np.int32, n_halo)
+            snap_eps = np.fromfile(fp, np.int32, n_halo)
+            snap_relax = np.fromfile(fp, np.int32, n_halo)
+            snap_relax_hydro = np.fromfile(fp, np.int32, n_halo)
+            disrupt_snap = np.fromfile(fp, np.int32, n_halo)
+            disrupt_snap_rs = np.fromfile(fp, np.int32, n_halo)
+
+            return snap_discrete, snap_eps, snap_relax, snap_relax_hydro, disrupt_snap, disrupt_snap_rs
+    except:
+        return None, None, None, None, None, None
+
+def read_cores(dir_name, include_false_selections=False, suffix="fid3"):
     """ read_cores read the particle-tracked halo cores of the halo in the
     given directory. The returned array is a structured array of type
     CORE_DTYPE with shape (n_halos, n_snaps).
     """
     if suffix == "":
         file_name = path.join(dir_name, "halos", "cores.dat")
     else:
```

### Comparing `symlib-1.3.0/symlib/star_tagging.py` & `symlib-1.3.1/symlib/star_tagging.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.0/symlib/util.py` & `symlib-1.3.1/symlib/util.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.0/symlib.egg-info/PKG-INFO` & `symlib-1.3.1/symlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.3.0
+Version: 1.3.1
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

