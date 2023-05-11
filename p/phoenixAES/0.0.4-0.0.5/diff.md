# Comparing `tmp/phoenixAES-0.0.4.tar.gz` & `tmp/phoenixAES-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phoenixAES-0.0.4.tar", last modified: Sat Oct  2 22:15:11 2021, max compression
+gzip compressed data, was "phoenixAES-0.0.5.tar", last modified: Thu May 11 10:44:21 2023, max compression
```

## Comparing `phoenixAES-0.0.4.tar` & `phoenixAES-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2021-10-02 22:15:11.968635 phoenixAES-0.0.4/
--rw-r--r--   0 phil      (1000) phil      (1000)    35141 2016-04-17 22:36:16.000000 phoenixAES-0.0.4/LICENSE
--rw-r--r--   0 phil      (1000) phil      (1000)     4042 2021-10-02 22:15:11.968635 phoenixAES-0.0.4/PKG-INFO
--rw-r--r--   0 phil      (1000) phil      (1000)     3376 2018-11-14 02:13:03.000000 phoenixAES-0.0.4/README.md
-drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2021-10-02 22:15:11.968635 phoenixAES-0.0.4/phoenixAES/
--rw-r--r--   0 phil      (1000) phil      (1000)    31845 2021-10-02 21:37:34.000000 phoenixAES-0.0.4/phoenixAES/__init__.py
-drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2021-10-02 22:15:11.968635 phoenixAES-0.0.4/phoenixAES.egg-info/
--rw-r--r--   0 phil      (1000) phil      (1000)     4042 2021-10-02 22:15:11.000000 phoenixAES-0.0.4/phoenixAES.egg-info/PKG-INFO
--rw-r--r--   0 phil      (1000) phil      (1000)      185 2021-10-02 22:15:11.000000 phoenixAES-0.0.4/phoenixAES.egg-info/SOURCES.txt
--rw-r--r--   0 phil      (1000) phil      (1000)        1 2021-10-02 22:15:11.000000 phoenixAES-0.0.4/phoenixAES.egg-info/dependency_links.txt
--rw-r--r--   0 phil      (1000) phil      (1000)       11 2021-10-02 22:15:11.000000 phoenixAES-0.0.4/phoenixAES.egg-info/top_level.txt
--rw-r--r--   0 phil      (1000) phil      (1000)       38 2021-10-02 22:15:11.968635 phoenixAES-0.0.4/setup.cfg
--rw-r--r--   0 phil      (1000) phil      (1000)      836 2021-10-02 22:10:14.000000 phoenixAES-0.0.4/setup.py
+drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2023-05-11 10:44:21.701822 phoenixAES-0.0.5/
+-rw-r--r--   0 phil      (1000) phil      (1000)    35141 2016-04-17 22:36:16.000000 phoenixAES-0.0.5/LICENSE
+-rw-r--r--   0 phil      (1000) phil      (1000)     4229 2023-05-11 10:44:21.701822 phoenixAES-0.0.5/PKG-INFO
+-rw-r--r--   0 phil      (1000) phil      (1000)     3600 2022-11-16 13:26:03.000000 phoenixAES-0.0.5/README.md
+drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2023-05-11 10:44:21.701822 phoenixAES-0.0.5/phoenixAES/
+-rw-r--r--   0 phil      (1000) phil      (1000)    32185 2022-04-05 21:54:35.000000 phoenixAES-0.0.5/phoenixAES/__init__.py
+drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2023-05-11 10:44:21.701822 phoenixAES-0.0.5/phoenixAES.egg-info/
+-rw-r--r--   0 phil      (1000) phil      (1000)     4229 2023-05-11 10:44:21.000000 phoenixAES-0.0.5/phoenixAES.egg-info/PKG-INFO
+-rw-r--r--   0 phil      (1000) phil      (1000)      185 2023-05-11 10:44:21.000000 phoenixAES-0.0.5/phoenixAES.egg-info/SOURCES.txt
+-rw-r--r--   0 phil      (1000) phil      (1000)        1 2023-05-11 10:44:21.000000 phoenixAES-0.0.5/phoenixAES.egg-info/dependency_links.txt
+-rw-r--r--   0 phil      (1000) phil      (1000)       11 2023-05-11 10:44:21.000000 phoenixAES-0.0.5/phoenixAES.egg-info/top_level.txt
+-rw-r--r--   0 phil      (1000) phil      (1000)       38 2023-05-11 10:44:21.701822 phoenixAES-0.0.5/setup.cfg
+-rw-r--r--   0 phil      (1000) phil      (1000)      836 2023-05-11 10:43:47.000000 phoenixAES-0.0.5/setup.py
```

### Comparing `phoenixAES-0.0.4/LICENSE` & `phoenixAES-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `phoenixAES-0.0.4/PKG-INFO` & `phoenixAES-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: phoenixAES
-Version: 0.0.4
+Version: 0.0.5
 Summary: tool to perform differential fault analysis attacks (DFA) against AES
 Home-page: https://github.com/SideChannelMarvels/JeanGrey
 Author: Philippe Teuwen
 Author-email: phil@teuwen.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Security :: Cryptography
 Description-Content-Type: text/markdown
@@ -19,19 +17,20 @@
 ## phoenixAES: a tool to perform differential fault analysis attacks (DFA) against AES
 
 Currently phoenixAES contains the following ciphers and fault models:
 
   * simple DFA R9:  
     AES 128 encryption or decryption  
     At least 4*2 faults in round 9 (between the last two MixCols)  
-    Ref: https://eprint.iacr.org/2003/010  
+    Ref: *[G. Piret and J.-J. Quisquater. A Differential Fault Attack Technique against SPN Structures, with Application to the AES and Khazad, CHES 2003 (pdf)](https://link.springer.com/content/pdf/10.1007/978-3-540-45238-6_7.pdf)*  
     Current implementation discards automatically unexploitable outputs but may fail if more than one fault occur on the same column so be careful to record only outputs from single faulted implementations.
   * simple DFA R8:  
     AES 128 encryption or decryption  
-    2 single faults in round 8
+    2 single faults in round 8  
+    Ref: same paper as above  
     It simply converts the ciphertexts as if they were faulted in round 9 so the previous attack can be applied
 
 See https://blog.quarkslab.com/differential-fault-analysis-on-white-box-aes-implementations.html for more background.
 
 ## Installation
 
 There is no dependencies, it requires only Python 3.
@@ -103,9 +102,7 @@
 
 After ~50 ms:
 
 ```
 Last round key #N found:
 D014F9A8C9EE2589E13F0CC8B6630CA6
 ```
-
-
```

### Comparing `phoenixAES-0.0.4/README.md` & `phoenixAES-0.0.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 ## phoenixAES: a tool to perform differential fault analysis attacks (DFA) against AES
 
 Currently phoenixAES contains the following ciphers and fault models:
 
   * simple DFA R9:  
     AES 128 encryption or decryption  
     At least 4*2 faults in round 9 (between the last two MixCols)  
-    Ref: https://eprint.iacr.org/2003/010  
+    Ref: *[G. Piret and J.-J. Quisquater. A Differential Fault Attack Technique against SPN Structures, with Application to the AES and Khazad, CHES 2003 (pdf)](https://link.springer.com/content/pdf/10.1007/978-3-540-45238-6_7.pdf)*  
     Current implementation discards automatically unexploitable outputs but may fail if more than one fault occur on the same column so be careful to record only outputs from single faulted implementations.
   * simple DFA R8:  
     AES 128 encryption or decryption  
-    2 single faults in round 8
+    2 single faults in round 8  
+    Ref: same paper as above  
     It simply converts the ciphertexts as if they were faulted in round 9 so the previous attack can be applied
 
 See https://blog.quarkslab.com/differential-fault-analysis-on-white-box-aes-implementations.html for more background.
 
 ## Installation
 
 There is no dependencies, it requires only Python 3.
```

### Comparing `phoenixAES-0.0.4/phoenixAES/__init__.py` & `phoenixAES-0.0.5/phoenixAES/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -493,18 +493,18 @@
         return ''.join(["%02X" % x if x is not None else ".." for x in key])
     else:
         return None
 
 def _absorb(index, o, candidates, goldenrefbytes, encrypt, verbose):
     Diff=[x^g for x, g, y in zip (o, goldenrefbytes, _AesFaultMaps[encrypt][index]) if y]
     Keys=[  k for    k, y in zip (        range(16), _AesFaultMaps[encrypt][index]) if y]
-    Cands  = _get_cands(Diff, Keys, [[14, 9,  13, 11], [2, 3, 1, 1]][encrypt], encrypt, verbose)
-    Cands += _get_cands(Diff, Keys, [[11, 14, 9,  13], [3, 1, 1, 2]][encrypt], encrypt, verbose)
-    Cands += _get_cands(Diff, Keys, [[13, 11, 14, 9] , [1, 1, 2, 3]][encrypt], encrypt, verbose)
-    Cands += _get_cands(Diff, Keys, [[9,  13, 11, 14], [1, 2, 3, 1]][encrypt], encrypt, verbose)
+    Cands  = _get_cands(Diff, Keys, goldenrefbytes, [[14, 9,  13, 11], [2, 3, 1, 1]][encrypt], encrypt, verbose)
+    Cands += _get_cands(Diff, Keys, goldenrefbytes, [[11, 14, 9,  13], [3, 1, 1, 2]][encrypt], encrypt, verbose)
+    Cands += _get_cands(Diff, Keys, goldenrefbytes, [[13, 11, 14, 9] , [1, 1, 2, 3]][encrypt], encrypt, verbose)
+    Cands += _get_cands(Diff, Keys, goldenrefbytes, [[9,  13, 11, 14], [1, 2, 3, 1]][encrypt], encrypt, verbose)
     if not candidates[index]:
         candidates[index] = Cands
     else:
         # merge self.candidates[index] and Cands
         new_candidates=[]
         for lc0,lc1,lc2,lc3 in Cands:
             for loc0,loc1,loc2,loc3 in candidates[index]:
@@ -512,22 +512,23 @@
                     new_candidates.append(((lc0 & loc0), (lc1 & loc1), (lc2 & loc2), (lc3 & loc3)))
         # candidates[index]=new_candidates
         if new_candidates != []:
             candidates[index]=new_candidates
         else:
             candidates[index] += Cands
 
-def _get_cands(Diff, Keys, tmult, encrypt, verbose):
+def _get_cands(Diff, Keys, Gold, tmult, encrypt, verbose):
     candi = [_get_compat(di, ti, encrypt) for di,ti in zip(Diff, tmult)]
     z = set(candi[0]).intersection(*candi[1:])
     candi = [[t for t in enumerate(ci) if t[1] in z] for ci in candi]
     cands = [[set([j for j,x in ci if x==zi]) for ci in candi] for zi in z]
     if verbose > 2:
         for kc0,kc1,kc2,kc3 in cands:
-            print ("K%x:" % Keys[0], ["%02X" % x for x in kc0], "K%x:" % Keys[1], ["%02X" % x for x in kc1],"K%x:" % Keys[2], ["%02X" % x for x in kc2],"K%x:" % Keys[3], ["%02X" % x for x in kc3])
+#            print ("K%x:" % Keys[0], ["%02X" % x for x in kc0], "K%x:" % Keys[1], ["%02X" % x for x in kc1],"K%x:" % Keys[2], ["%02X" % x for x in kc2],"K%x:" % Keys[3], ["%02X" % x for x in kc3])
+            print ("K%x:" % Keys[0], ["%02X" % (x ^ Gold[Keys[0]]) for x in kc0], "K%x:" % Keys[1], ["%02X" % (x ^ Gold[Keys[1]]) for x in kc1],"K%x:" % Keys[2], ["%02X" % (x ^ Gold[Keys[2]]) for x in kc2],"K%x:" % Keys[3], ["%02X" % (x ^ Gold[Keys[3]]) for x in kc3])
     return cands
 
 def _get_compat(diff, tmult, encrypt):
     ibox = [_AesSBox, _AesInvSBox][encrypt]
     itab = [0]*256
     for i,mi in enumerate(_AesMult[tmult]):
         itab[mi] = i
```

### Comparing `phoenixAES-0.0.4/phoenixAES.egg-info/PKG-INFO` & `phoenixAES-0.0.5/phoenixAES.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: phoenixAES
-Version: 0.0.4
+Version: 0.0.5
 Summary: tool to perform differential fault analysis attacks (DFA) against AES
 Home-page: https://github.com/SideChannelMarvels/JeanGrey
 Author: Philippe Teuwen
 Author-email: phil@teuwen.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Security :: Cryptography
 Description-Content-Type: text/markdown
@@ -19,19 +17,20 @@
 ## phoenixAES: a tool to perform differential fault analysis attacks (DFA) against AES
 
 Currently phoenixAES contains the following ciphers and fault models:
 
   * simple DFA R9:  
     AES 128 encryption or decryption  
     At least 4*2 faults in round 9 (between the last two MixCols)  
-    Ref: https://eprint.iacr.org/2003/010  
+    Ref: *[G. Piret and J.-J. Quisquater. A Differential Fault Attack Technique against SPN Structures, with Application to the AES and Khazad, CHES 2003 (pdf)](https://link.springer.com/content/pdf/10.1007/978-3-540-45238-6_7.pdf)*  
     Current implementation discards automatically unexploitable outputs but may fail if more than one fault occur on the same column so be careful to record only outputs from single faulted implementations.
   * simple DFA R8:  
     AES 128 encryption or decryption  
-    2 single faults in round 8
+    2 single faults in round 8  
+    Ref: same paper as above  
     It simply converts the ciphertexts as if they were faulted in round 9 so the previous attack can be applied
 
 See https://blog.quarkslab.com/differential-fault-analysis-on-white-box-aes-implementations.html for more background.
 
 ## Installation
 
 There is no dependencies, it requires only Python 3.
@@ -103,9 +102,7 @@
 
 After ~50 ms:
 
 ```
 Last round key #N found:
 D014F9A8C9EE2589E13F0CC8B6630CA6
 ```
-
-
```

### Comparing `phoenixAES-0.0.4/setup.py` & `phoenixAES-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="phoenixAES",
-    version="0.0.4",
+    version="0.0.5",
     author="Philippe Teuwen",
     author_email="phil@teuwen.org",
     description="tool to perform differential fault analysis attacks (DFA) against AES",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SideChannelMarvels/JeanGrey",
     packages=setuptools.find_packages(),
```

