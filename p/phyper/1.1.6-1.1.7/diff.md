# Comparing `tmp/phyper-1.1.6-py3-none-any.whl.zip` & `tmp/phyper-1.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 29425 bytes, number of entries: 15
+Zip file size: 29421 bytes, number of entries: 15
 -rw-r--r--  2.0 unx      685 b- defN 23-Apr-20 10:38 phyper/__init__.py
 -rw-r--r--  2.0 unx      292 b- defN 23-Apr-20 12:42 phyper/chemometrics/__init__.py
 -rw-r--r--  2.0 unx     9507 b- defN 23-Apr-20 15:13 phyper/chemometrics/_gui.py
 -rw-r--r--  2.0 unx    13252 b- defN 23-Apr-20 10:38 phyper/chemometrics/analysis.py
--rw-r--r--  2.0 unx    50777 b- defN 23-May-11 11:45 phyper/chemometrics/dataset.py
+-rw-r--r--  2.0 unx    50776 b- defN 23-May-11 11:48 phyper/chemometrics/dataset.py
 -rw-r--r--  2.0 unx     2713 b- defN 23-Apr-20 10:38 phyper/chemometrics/preprocessing.py
 -rw-r--r--  2.0 unx     2298 b- defN 23-Apr-20 10:38 phyper/chemometrics/sampling.py
 -rw-r--r--  2.0 unx      121 b- defN 23-Apr-20 10:38 phyper/lab/__init__.py
 -rw-r--r--  2.0 unx      802 b- defN 23-Apr-20 10:38 phyper/lab/_misc.py
 -rw-r--r--  2.0 unx    15275 b- defN 23-Apr-20 13:35 phyper/lab/measurement.py
--rwxrwxrwx  2.0 unx     1075 b- defN 23-May-11 11:46 phyper-1.1.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     2268 b- defN 23-May-11 11:46 phyper-1.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-11 11:46 phyper-1.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-May-11 11:46 phyper-1.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1219 b- defN 23-May-11 11:46 phyper-1.1.6.dist-info/RECORD
-15 files, 100383 bytes uncompressed, 27415 bytes compressed:  72.7%
+-rwxrwxrwx  2.0 unx     1075 b- defN 23-May-11 11:49 phyper-1.1.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-11 11:49 phyper-1.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-11 11:49 phyper-1.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-11 11:49 phyper-1.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1219 b- defN 23-May-11 11:49 phyper-1.1.7.dist-info/RECORD
+15 files, 100382 bytes uncompressed, 27411 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: phyper/lab/_misc.py
 Comment: 
 
 Filename: phyper/lab/measurement.py
 Comment: 
 
-Filename: phyper-1.1.6.dist-info/LICENSE
+Filename: phyper-1.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: phyper-1.1.6.dist-info/METADATA
+Filename: phyper-1.1.7.dist-info/METADATA
 Comment: 
 
-Filename: phyper-1.1.6.dist-info/WHEEL
+Filename: phyper-1.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: phyper-1.1.6.dist-info/top_level.txt
+Filename: phyper-1.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: phyper-1.1.6.dist-info/RECORD
+Filename: phyper-1.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## phyper/chemometrics/dataset.py

```diff
@@ -916,15 +916,15 @@
             Mathematical method form the numpy library. e.g. np.divide
 
         Returns
         -------
         result: HyperSpectralDataset
             Result from numpy operation
         """
-        result = self.deepcopy()
+        result = deepcopy(self)
         HC = result.get_HC()
         if isinstance(other, HyperSpectralDataset):
             HC = np_func(HC, other.get_HC(), out=HC)
         elif isinstance(other, np.ndarray):
             HC = np_func(HC, other, out=HC)
         else:
             raise AttributeError(f'{np_func} on HyperSpectralDataset is not possible with {other.type}')
```

## Comparing `phyper-1.1.6.dist-info/LICENSE` & `phyper-1.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `phyper-1.1.6.dist-info/METADATA` & `phyper-1.1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phyper
-Version: 1.1.6
+Version: 1.1.7
 Summary: Package for managing (hyper)spectral datasets
 Home-page: https://gitlab.kuleuven.be/u0123403/pyper
 Author: Remi Van Belleghem
 Author-email: remi.vanbelleghem@kuleuven.be
 Maintainer: MeBios - KULeuven
 Maintainer-email: wouter.saeys@kuleuven.be
 License: UNKNOWN
```

## Comparing `phyper-1.1.6.dist-info/RECORD` & `phyper-1.1.7.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 phyper/__init__.py,sha256=4hYB58cealu01B6FLn3lhRnI0JAPY6Va107e65WXTcs,685
 phyper/chemometrics/__init__.py,sha256=5y7WaXHDvt1RbplvdekletkldO9cMdvYHRFzJkE1ziE,292
 phyper/chemometrics/_gui.py,sha256=YqamSYFGlfdLj7EYuLU1Ut3YXdGdexkj6sBJs85WAQA,9507
 phyper/chemometrics/analysis.py,sha256=903ZGNPjkmJL_z0CeeorcQkoiCMZLeOYK3_q18CmBnc,13252
-phyper/chemometrics/dataset.py,sha256=mR2T2zIzjJ3NoyFXO88dlA6UcqSSX96cCaQy2xb0a0E,50777
+phyper/chemometrics/dataset.py,sha256=1VtDz50nnNTGxEm44H2Ik2ER32SxpTHc0hEmloLcZ-o,50776
 phyper/chemometrics/preprocessing.py,sha256=lKoB64-a4IdM82pC1OAh9cCy-LXKLOcFbygVYnQCBcM,2713
 phyper/chemometrics/sampling.py,sha256=H-xl0PrAwRoaxwah8DqVSlRJ1gPl9Qm806Zh7MPuu2U,2298
 phyper/lab/__init__.py,sha256=p1f53MLglxawnDhRGT4O1NI5CpL2Rvski2XEyg9ErM8,121
 phyper/lab/_misc.py,sha256=irgAaObHkaIBESTdw-o0e0Eb-z2pUm9Kdc9ujZq8pg8,802
 phyper/lab/measurement.py,sha256=YCQX5YkgWDmwesoELt14JgdWcVYc2vq8cqnjIbxHfSM,15275
-phyper-1.1.6.dist-info/LICENSE,sha256=i-l_fDhG098wzA_kHlskLIwp3UKEjHzNP1PVuIu2wuQ,1075
-phyper-1.1.6.dist-info/METADATA,sha256=MLW_OI15ygg3fNJUyb0kGVCWf91XjP2Gim4Ba13Hknw,2268
-phyper-1.1.6.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-phyper-1.1.6.dist-info/top_level.txt,sha256=1CRpBqxQW0H4uxZ6GzjiIKUq4FJksW5pai8komowTII,7
-phyper-1.1.6.dist-info/RECORD,,
+phyper-1.1.7.dist-info/LICENSE,sha256=i-l_fDhG098wzA_kHlskLIwp3UKEjHzNP1PVuIu2wuQ,1075
+phyper-1.1.7.dist-info/METADATA,sha256=PhfwruaNnLNFSmwn9okAOLskh8B1JPQkxkcYa8c7yj0,2268
+phyper-1.1.7.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+phyper-1.1.7.dist-info/top_level.txt,sha256=1CRpBqxQW0H4uxZ6GzjiIKUq4FJksW5pai8komowTII,7
+phyper-1.1.7.dist-info/RECORD,,
```

