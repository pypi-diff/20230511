# Comparing `tmp/pawnlib-1.0.8-py3-none-any.whl.zip` & `tmp/pawnlib-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,34 +1,35 @@
-Zip file size: 109012 bytes, number of entries: 48
+Zip file size: 109685 bytes, number of entries: 49
 -rw-r--r--  2.0 unx     1188 b- defN 23-Jan-31 08:49 pawnlib/__init__.py
 -rw-r--r--  2.0 unx     1224 b- defN 23-Jan-31 08:49 pawnlib/__main__.py
--rw-r--r--  2.0 unx      296 b- defN 23-May-03 09:08 pawnlib/__version__.py
+-rw-r--r--  2.0 unx      296 b- defN 23-May-06 09:14 pawnlib/__version__.py
 -rw-r--r--  2.0 unx       19 b- defN 22-Jul-21 06:00 pawnlib/asyncio/__init__.py
 -rw-r--r--  2.0 unx     4261 b- defN 23-Feb-22 08:29 pawnlib/asyncio/run.py
 -rw-r--r--  2.0 unx       36 b- defN 22-Jul-28 01:54 pawnlib/builder/__init__.py
 -rw-r--r--  2.0 unx     5382 b- defN 23-Jan-31 06:30 pawnlib/builder/generator.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jul-28 04:35 pawnlib/builder/templates/__init__.py
 -rw-r--r--  2.0 unx     2343 b- defN 23-Feb-16 09:40 pawnlib/builder/templates/app_with_logging.tmpl
 -rw-r--r--  2.0 unx        0 b- defN 22-Jul-28 04:34 pawnlib/cli/__init__.py
 -rw-r--r--  2.0 unx     1328 b- defN 23-Jan-31 04:22 pawnlib/cli/aws.py
+-rw-r--r--  2.0 unx     1120 b- defN 23-May-06 07:13 pawnlib/cli/banner.py
 -rw-r--r--  2.0 unx     9975 b- defN 23-Apr-18 05:35 pawnlib/cli/http.py
 -rw-r--r--  2.0 unx     2910 b- defN 23-Apr-18 05:35 pawnlib/cli/icon.py
 -rw-r--r--  2.0 unx     1305 b- defN 22-Sep-22 06:43 pawnlib/cli/init.py
 -rw-r--r--  2.0 unx     5242 b- defN 23-Apr-18 05:35 pawnlib/cli/main_cli.py
 -rw-r--r--  2.0 unx     6605 b- defN 23-Jan-31 06:39 pawnlib/cli/proxy.py
 -rw-r--r--  2.0 unx     3269 b- defN 23-Apr-27 06:14 pawnlib/cli/wallet.py
 -rw-r--r--  2.0 unx     1380 b- defN 22-Aug-29 07:53 pawnlib/config/__fix_import.py
 -rw-r--r--  2.0 unx      121 b- defN 23-Feb-27 02:19 pawnlib/config/__init__.py
 -rw-r--r--  2.0 unx     4523 b- defN 22-Oct-21 09:48 pawnlib/config/configure.py
 -rw-r--r--  2.0 unx     4165 b- defN 23-Jan-31 05:50 pawnlib/config/console.py
 -rw-r--r--  2.0 unx    29835 b- defN 23-May-03 08:49 pawnlib/config/globalconfig.py
 -rw-r--r--  2.0 unx      432 b- defN 23-Apr-18 05:35 pawnlib/input/__init__.py
 -rw-r--r--  2.0 unx    21792 b- defN 23-Apr-19 03:05 pawnlib/input/prompt.py
 -rw-r--r--  2.0 unx      650 b- defN 23-Apr-19 01:22 pawnlib/output/__init__.py
--rw-r--r--  2.0 unx    38557 b- defN 23-May-02 06:42 pawnlib/output/color_print.py
+-rw-r--r--  2.0 unx    38730 b- defN 23-May-06 09:09 pawnlib/output/color_print.py
 -rw-r--r--  2.0 unx     6198 b- defN 23-Jan-31 06:29 pawnlib/output/file.py
 -rw-r--r--  2.0 unx      445 b- defN 23-Feb-17 09:14 pawnlib/resource/__init__.py
 -rw-r--r--  2.0 unx     6568 b- defN 23-Jan-31 04:59 pawnlib/resource/net.py
 -rw-r--r--  2.0 unx    11387 b- defN 22-Nov-22 01:36 pawnlib/resource/server.py
 -rw-r--r--  2.0 unx     2022 b- defN 23-Apr-26 02:59 pawnlib/typing/__init__.py
 -rw-r--r--  2.0 unx     9094 b- defN 23-Apr-26 05:18 pawnlib/typing/check.py
 -rw-r--r--  2.0 unx      823 b- defN 23-Apr-18 05:35 pawnlib/typing/constants.py
@@ -38,13 +39,13 @@
 -rw-r--r--  2.0 unx    12711 b- defN 23-Jan-31 06:35 pawnlib/typing/generator.py
 -rw-r--r--  2.0 unx      552 b- defN 23-Apr-18 05:35 pawnlib/utils/__init__.py
 -rw-r--r--  2.0 unx    50602 b- defN 23-May-02 08:39 pawnlib/utils/http.py
 -rw-r--r--  2.0 unx    25686 b- defN 23-Apr-28 06:32 pawnlib/utils/icx_signer.py
 -rw-r--r--  2.0 unx    12172 b- defN 23-Jan-31 05:22 pawnlib/utils/log.py
 -rw-r--r--  2.0 unx     7005 b- defN 23-May-03 07:27 pawnlib/utils/notify.py
 -rw-r--r--  2.0 unx    23248 b- defN 23-Apr-18 05:35 pawnlib/utils/operate_handler.py
--rw-r--r--  2.0 unx     5131 b- defN 23-May-03 09:08 pawnlib-1.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-03 09:08 pawnlib-1.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-May-03 09:08 pawnlib-1.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-May-03 09:08 pawnlib-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3917 b- defN 23-May-03 09:08 pawnlib-1.0.8.dist-info/RECORD
-48 files, 394381 bytes uncompressed, 102844 bytes compressed:  73.9%
+-rw-r--r--  2.0 unx     5131 b- defN 23-May-06 09:14 pawnlib-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-06 09:14 pawnlib-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-May-06 09:14 pawnlib-1.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-May-06 09:14 pawnlib-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3995 b- defN 23-May-06 09:14 pawnlib-1.0.9.dist-info/RECORD
+49 files, 395752 bytes uncompressed, 103399 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -27,14 +27,17 @@
 
 Filename: pawnlib/cli/__init__.py
 Comment: 
 
 Filename: pawnlib/cli/aws.py
 Comment: 
 
+Filename: pawnlib/cli/banner.py
+Comment: 
+
 Filename: pawnlib/cli/http.py
 Comment: 
 
 Filename: pawnlib/cli/icon.py
 Comment: 
 
 Filename: pawnlib/cli/init.py
@@ -123,23 +126,23 @@
 
 Filename: pawnlib/utils/notify.py
 Comment: 
 
 Filename: pawnlib/utils/operate_handler.py
 Comment: 
 
-Filename: pawnlib-1.0.8.dist-info/METADATA
+Filename: pawnlib-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: pawnlib-1.0.8.dist-info/WHEEL
+Filename: pawnlib-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: pawnlib-1.0.8.dist-info/entry_points.txt
+Filename: pawnlib-1.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: pawnlib-1.0.8.dist-info/top_level.txt
+Filename: pawnlib-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pawnlib-1.0.8.dist-info/RECORD
+Filename: pawnlib-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pawnlib/__version__.py

```diff
@@ -1,9 +1,9 @@
 ####
 __title__ = 'pawnlib'
 __description__ = 'pawnlib is a collection of libraries for IaC.'
 __url__ = 'https://github.com/jinwoo-j/pawnlib'
-__version__ = '1.0.8'
+__version__ = '1.0.9'
 __author__ = 'Jinwoo Jeong'
 __author_email__ = 'jinwoo@parametacorp.com'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2022 JINWOO'
```

## pawnlib/output/color_print.py

```diff
@@ -1098,11 +1098,13 @@
             filename = sys.exc_info()[-1].tb_filename
         except AttributeError:
             previous_frame = inspect.currentframe().f_back
             line_no = inspect.currentframe().f_back.f_lineno
             (filename, line_number,
              function_name, ln, index) = inspect.getframeinfo(previous_frame)
         # self.args = "<{0.__name__}> ({2} line {2}): \n {3}".format(type(self), filename, line_no, msg),
-        self.args = "{0}<{1.__name__}>{2} ({3} line {4}): \n {5}".format(bcolors.FAIL, type(self), bcolors.ENDC, filename, line_no, msg),
+        # self.args = "{0}<{1.__name__}>{2} ({3} line {4}): \n {5}".format(bcolors.FAIL, type(self), bcolors.ENDC, filename, line_no, msg),
+        # self.args = "<{0.__name__}>({1} line {2}): \n {3}".format(type(self), filename, line_no, msg),
+        self.args = "<{0.__name__}> {1}".format(type(self), msg),
         # ex_type, ex_value, traceback = sys.exc_info()
         raise Exception(self)
```

## Comparing `pawnlib-1.0.8.dist-info/METADATA` & `pawnlib-1.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pawnlib
-Version: 1.0.8
+Version: 1.0.9
 Summary: pawnlib is a collection of libraries for IaC.
 Home-page: https://github.com/jinwoo-j/pawnlib
 Author: Jinwoo Jeong
 Author-email: jinwoo@parametacorp.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `pawnlib-1.0.8.dist-info/RECORD` & `pawnlib-1.0.9.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 pawnlib/__init__.py,sha256=FXDHsJ3zZkGKwHLxXvy0z-DLH9UwQvGh7SoLiigPptw,1188
 pawnlib/__main__.py,sha256=wmMMh9f5l39HY6p_IfARRZwRDcK1rnfENZdCb9tzJYg,1224
-pawnlib/__version__.py,sha256=KKyqaBPpxxUK_fhj3GAWyiZUZv8sYxFwMpNVj3hSgNA,296
+pawnlib/__version__.py,sha256=eIX4planfhXfyH-_Au4_tKSS_IsEzJBXHbnw7771f9c,296
 pawnlib/asyncio/__init__.py,sha256=ToWEND0eBP0YeJw4xZaBPLgQ-BGSeIvIApyysQMCsgo,19
 pawnlib/asyncio/run.py,sha256=WnZ8JWa5hnntds4wItvPtYy7HbJ7fLMvHbP04uXi05o,4261
 pawnlib/builder/__init__.py,sha256=2uuVV8xTTPsD8SCN1PDLhAcKOKISEZLQCQgOeritMrE,36
 pawnlib/builder/generator.py,sha256=4nsaQvZpzaLpIYLovIqmofBmyItj6nApae9zFdmvIuQ,5382
 pawnlib/builder/templates/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pawnlib/builder/templates/app_with_logging.tmpl,sha256=UpxeQgys681Q1B-mADpEpRaG47RccWwwsdKigHL-ECU,2343
 pawnlib/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pawnlib/cli/aws.py,sha256=7vM9CDAe6qqXyqLRpwktw_qWfLEs4hOHp9D2f1eKF3g,1328
+pawnlib/cli/banner.py,sha256=qbFsQc8K_6et4ljOCWp7s32I2N6nVIM0GR7wnOZ02U0,1120
 pawnlib/cli/http.py,sha256=GZPmoZve3vj2LkWwWUL3QIPv_PFIS-sN27cAR2Ka5-A,9975
 pawnlib/cli/icon.py,sha256=xaLVmfeOsqvT0JoJa6oquugqBp88tbTAOWJ5gLtkiCg,2910
 pawnlib/cli/init.py,sha256=GuRT6zIDWIegLvYznQEG4Dc3oOaHSD5QE8WItSVwj5w,1305
 pawnlib/cli/main_cli.py,sha256=BiVY0xtYEoZ3uhH-_gdH9rQ7tPaTHLh7-pTgi6izlMo,5242
 pawnlib/cli/proxy.py,sha256=iR0zwjMibFeHTn3x7N4vqM-Yzx5u0ETFM3D1ZmbdbFw,6605
 pawnlib/cli/wallet.py,sha256=mHIBMkdRzc8y3UaitnJyKCqc5IKUnlKStG7Gea1_wN8,3269
 pawnlib/config/__fix_import.py,sha256=RcDVfb9fdwYrba68s18UpHdUXD1xalA5NhLzbq-33z4,1380
 pawnlib/config/__init__.py,sha256=Z25cxP0bILcaUfpjx0kJubGH_8s3cOn_wBc8ixLXhCw,121
 pawnlib/config/configure.py,sha256=ARDGd3oanqDhhfW_oyXkw9stJ5ZlOMO0tSZA2gwuG_I,4523
 pawnlib/config/console.py,sha256=QKBEN-dn8qNbv5H_rz_-GYu6EX--L58mvZ8MG9hPh5A,4165
 pawnlib/config/globalconfig.py,sha256=uBIoeytI9Bd45kb-6DDPwSrxFouOBxS7LgBrj_gvpxQ,29835
 pawnlib/input/__init__.py,sha256=uagiBVVJrEfeBCmFL1rJK-cFcML8uTyoUMF1vwYy7eQ,432
 pawnlib/input/prompt.py,sha256=yDmEw7Y6o-5BcozxAFYYlfAykXn8luk53YtAjw8IyGg,21792
 pawnlib/output/__init__.py,sha256=oV_KTI_jcFfV3v9Y6tfx0abpu5rOL9J0_pmUFLSoXVE,650
-pawnlib/output/color_print.py,sha256=Qlx0D2r1APkG-_t5u4A-UEXICWKbisc8FqcFRP_fJt0,38557
+pawnlib/output/color_print.py,sha256=WhYVej33f8JBjOn1Y8EuuEjoY7yaPTT2Wq1TnpxzILY,38730
 pawnlib/output/file.py,sha256=V2_kYLQo5EG-PTeQa-HtYFhWagCGoV5PTkPUh8K0vUI,6198
 pawnlib/resource/__init__.py,sha256=s2u4U2LZF5ntbo65WivN9d74R_Hlh-DQTgmL8Zd_RzY,445
 pawnlib/resource/net.py,sha256=W8TwyXkXzhiTEqgZi-0l_alljzOw7bo4OC7iNkvb5wE,6568
 pawnlib/resource/server.py,sha256=T3_qcSL3TCxJ5AT9d3kBw_EQARYTpooxVjDdF-5Lo7w,11387
 pawnlib/typing/__init__.py,sha256=IVCs20A-AFyHGejhzctvphouVEnNIdWY4WCx7PWdSSA,2022
 pawnlib/typing/check.py,sha256=GTYRaQ1ubMYTEiKa1463SWub_oitBjSFFltnOCDdRvg,9094
 pawnlib/typing/constants.py,sha256=9mbzRKWZw9p2ByzWairAT1zZv-qgd_7WVOEIVwUbX_0,823
@@ -37,12 +38,12 @@
 pawnlib/typing/generator.py,sha256=tAzkL5hJt0le958oYkVjTMbRGmlOwP3gE7mZaD-yXJY,12711
 pawnlib/utils/__init__.py,sha256=nO-vGtRB4UIImOLlJO-gN7SWoXYLcXqfc3LLyoCEAxM,552
 pawnlib/utils/http.py,sha256=_E-9sEJFqBWF-GdPlAa3PTYY4ey6VJN5iafw1DmKr90,50602
 pawnlib/utils/icx_signer.py,sha256=PyMnhItB4QzICgReWzgk3wDIUab5pFg9H-FhjVbs5F4,25686
 pawnlib/utils/log.py,sha256=zYClSlvFJt9ZxZpApWvFZ7EcFRFtwUIyCyrtmUdfiLI,12172
 pawnlib/utils/notify.py,sha256=z2SV7K20I2NTy5eCkLPeI7tCa00E1rTeLhHSeG7DefI,7005
 pawnlib/utils/operate_handler.py,sha256=LMf41828PACtmmxnkR_zz0VD7s8F--Cqcdl9Efk4hV0,23248
-pawnlib-1.0.8.dist-info/METADATA,sha256=Ycd0MIvlddkXskGhIFSd5inCpdWSvPyp3KCeEs79mJM,5131
-pawnlib-1.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pawnlib-1.0.8.dist-info/entry_points.txt,sha256=gfwAzqk-lzSb_VFiXmGg4Xn-8TUu_TMcM3QBjdyEAAE,52
-pawnlib-1.0.8.dist-info/top_level.txt,sha256=a6t_hQ3MagyRwwliF91xPgBk12g6a7O84C4GiY3fKQE,8
-pawnlib-1.0.8.dist-info/RECORD,,
+pawnlib-1.0.9.dist-info/METADATA,sha256=yhqrHgKYnku70zBPcJ_rBiCs8JWDHhH6nU3zR0-oHRk,5131
+pawnlib-1.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pawnlib-1.0.9.dist-info/entry_points.txt,sha256=gfwAzqk-lzSb_VFiXmGg4Xn-8TUu_TMcM3QBjdyEAAE,52
+pawnlib-1.0.9.dist-info/top_level.txt,sha256=a6t_hQ3MagyRwwliF91xPgBk12g6a7O84C4GiY3fKQE,8
+pawnlib-1.0.9.dist-info/RECORD,,
```

