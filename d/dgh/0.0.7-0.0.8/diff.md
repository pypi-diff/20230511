# Comparing `tmp/dgh-0.0.7.tar.gz` & `tmp/dgh-0.0.8.tar.gz`

## Comparing `dgh-0.0.7.tar` & `dgh-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 dgh-0.0.7/CHANGELOG.md
--rw-r--r--   0        0        0    10507 2020-02-02 00:00:00.000000 dgh-0.0.7/illustration.pdf
--rw-r--r--   0        0        0    13473 2020-02-02 00:00:00.000000 dgh-0.0.7/illustration.png
--rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 dgh-0.0.7/illustration.svg
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 dgh-0.0.7/illustration_wide.pdf
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 dgh-0.0.7/illustration_wide_tall.pdf
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 dgh-0.0.7/dgh/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 dgh-0.0.7/dgh/constants.py
--rw-r--r--   0        0        0     7106 2020-02-02 00:00:00.000000 dgh-0.0.7/dgh/dgh.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 dgh-0.0.7/dgh/fw.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 dgh-0.0.7/dgh/mappings.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 dgh-0.0.7/dgh/spaces.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dgh-0.0.7/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 dgh-0.0.7/LICENSE
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 dgh-0.0.7/README.md
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 dgh-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 dgh-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 dgh-0.0.8/CHANGELOG.md
+-rw-r--r--   0        0        0    10507 2020-02-02 00:00:00.000000 dgh-0.0.8/illustration.pdf
+-rw-r--r--   0        0        0    13473 2020-02-02 00:00:00.000000 dgh-0.0.8/illustration.png
+-rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 dgh-0.0.8/illustration.svg
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 dgh-0.0.8/illustration_wide.pdf
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 dgh-0.0.8/illustration_wide_tall.pdf
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 dgh-0.0.8/dgh/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 dgh-0.0.8/dgh/constants.py
+-rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 dgh-0.0.8/dgh/dgh.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 dgh-0.0.8/dgh/fw.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 dgh-0.0.8/dgh/mappings.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 dgh-0.0.8/dgh/spaces.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dgh-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 dgh-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 dgh-0.0.8/README.md
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dgh-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 dgh-0.0.8/PKG-INFO
```

### Comparing `dgh-0.0.7/CHANGELOG.md` & `dgh-0.0.8/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 # Changelog
 
 <!--next-version-placeholder-->
+## v0.0.8 (May 11 2023)
+
+### Feature
+
+- Added f, g to verbose output if returning them
+
+### Fix
+
+- Corrected (halved) ub in summary (verbose > 0)
+
+### Documentation
+
+- Corrected project homepage
+- Switched to url for the example illustration 
+
 ## v0.0.7 (May 10 2023)
 
 ### Feature
 
 - Simplified import structure
 - Added "summary" verbose level
```

### Comparing `dgh-0.0.7/illustration.pdf` & `dgh-0.0.8/illustration.pdf`

 * *Files identical despite different names*

### Comparing `dgh-0.0.7/illustration.png` & `dgh-0.0.8/illustration.png`

 * *Files identical despite different names*

### Comparing `dgh-0.0.7/illustration.svg` & `dgh-0.0.8/illustration.svg`

 * *Files identical despite different names*

### Comparing `dgh-0.0.7/illustration_wide.pdf` & `dgh-0.0.8/illustration_wide.pdf`

 * *Files identical despite different names*

### Comparing `dgh-0.0.7/illustration_wide_tall.pdf` & `dgh-0.0.8/illustration_wide_tall.pdf`

 * *Files identical despite different names*

### Comparing `dgh-0.0.7/dgh/dgh.py` & `dgh-0.0.8/dgh/dgh.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,19 +118,20 @@
     # Find minima from new restarts until run out of iteration budget.
     min_dis_R = np.inf
     fw_seq = []
     restart_idx = 0
     while iter_budget > 0:
         # Initialize new restart.
         S = center(n, m) if restart_idx == 0 and center_start else rnd_S(n, m, rnd)
+        restart_iter = 0
         fw_idx = 0
         c = first_c
+        solving_for_next_c = True
 
         # Run a sequence of FW solvers using solutions as subsequent warm starts.
-        solving_for_next_c = True
         while solving_for_next_c:
             # Set up next FW solver in the sequence if needed.
             try:
                 fw = fw_seq[fw_idx]
             except IndexError:
                 fw = make_frank_wolfe_solver(
                     X, Y, c, tol=tol, verbose=verbose)
@@ -140,38 +141,40 @@
             S, used_iter = fw(S0=S, max_iter=iter_budget)
 
             # Terminate if no iterations were made, run out of iteration budget,
             # or next c will exceed floating point arithmetic limits.
             solving_for_next_c = 0 < used_iter < iter_budget and c < MAX_C
 
             # Move to the next minimization obtained by squaring c.
-            iter_budget -= used_iter
             fw_idx += 1
             with np.errstate(over='ignore'):
                 c **= 2
+            iter_budget -= used_iter
+            restart_iter += used_iter
 
         # Project the solution to the set of correspondences and find the
         # resulting distortion on the original scale.
         R = S_to_R(S, n, m)
         dis_R = dis(R, X, Y) * d_max
 
         # Update the best distortion achieved from all restarts.
         if dis_R < min_dis_R:
-            best_f, best_g = S_to_fg(S, n, m)
+            best_f, best_g = map(list, S_to_fg(S, n, m))
             min_dis_R = dis_R
 
         if verbose > 1:
-            print(f'finished restart {restart_idx}: ½dis(R)={dis_R/2:.4f}, '
-                  f'min ½dis(R)={min_dis_R/2:.4f}, remaining iter={iter_budget}')
+            fg_descr = f' (f={best_f}, g={best_g})' if return_fg else ''
+            print(f'restart {restart_idx} (used {restart_iter} iterations): '
+                  f'½dis(R)={dis_R/2:.4f}, min ½dis(R)={min_dis_R/2:.4f}{fg_descr}')
 
         restart_idx += 1
 
         # Terminate if achieved lower bound.
         if min_dis_R <= lb:
             break
 
     if verbose > 0:
-        print(f'proved dGH≤{min_dis_R} after {restart_idx} restarts')
+        print(f'proved dGH≤{min_dis_R/2} after {restart_idx} restarts')
 
     res = (min_dis_R/2, best_f, best_g) if return_fg else min_dis_R/2
 
     return res
```

### Comparing `dgh-0.0.7/dgh/fw.py` & `dgh-0.0.8/dgh/fw.py`

 * *Files identical despite different names*

### Comparing `dgh-0.0.7/dgh/mappings.py` & `dgh-0.0.8/dgh/mappings.py`

 * *Files identical despite different names*

### Comparing `dgh-0.0.7/dgh/spaces.py` & `dgh-0.0.8/dgh/spaces.py`

 * *Files identical despite different names*

### Comparing `dgh-0.0.7/LICENSE` & `dgh-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dgh-0.0.7/README.md` & `dgh-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Installing the package from Python Package Index:
 
 ```$ pip install dgh```
 
 Computing $d_\text{GH}(X, Y)$ where $X$ is the vertices of a tall narrow rectangle and $Y$ is the vertices of a small equilateral triangle together with a remote point from it (see illustration):
 
 <p align="center">
-    <img src="./illustration.png" alt="Illustration to the example" width="400"/>
+    <img src="https://github.com/vlad-oles/dgh/blob/main/illustration.png" alt="Illustration of the example" width="400"/>
 </p>
 
 ```
 import numpy as np
 import dgh
 
 # Set distance matrix for the rectangle.
```

### Comparing `dgh-0.0.7/PKG-INFO` & `dgh-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dgh
-Version: 0.0.7
+Version: 0.0.8
 Summary: Computing the Gromov–Hausdorff distance
-Project-URL: Homepage, https://github.com/pypa/dgh
-Project-URL: Bug Tracker, https://github.com/pypa/dgh/issues
+Project-URL: Homepage, https://github.com/vlad-oles/dgh
+Project-URL: Bug Tracker, https://github.com/vlad-oles/dgh/issues
 Author-email: Vladyslav Oles <vlad.oles@proton.me>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
@@ -23,15 +23,15 @@
 Installing the package from Python Package Index:
 
 ```$ pip install dgh```
 
 Computing $d_\text{GH}(X, Y)$ where $X$ is the vertices of a tall narrow rectangle and $Y$ is the vertices of a small equilateral triangle together with a remote point from it (see illustration):
 
 <p align="center">
-    <img src="./illustration.png" alt="Illustration to the example" width="400"/>
+    <img src="https://github.com/vlad-oles/dgh/blob/main/illustration.png" alt="Illustration of the example" width="400"/>
 </p>
 
 ```
 import numpy as np
 import dgh
 
 # Set distance matrix for the rectangle.
```

