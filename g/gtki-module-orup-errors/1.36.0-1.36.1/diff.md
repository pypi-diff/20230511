# Comparing `tmp/gtki_module_orup_errors-1.36.0-py3-none-any.whl.zip` & `tmp/gtki_module_orup_errors-1.36.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 12981 bytes, number of entries: 17
+Zip file size: 12994 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Oct-20 07:03 orup_errors/__init__.py
 -rw-rw-rw-  2.0 fat    16857 b- defN 23-May-11 06:51 orup_errors/all_errors.py
--rw-rw-rw-  2.0 fat     9323 b- defN 23-May-11 06:52 orup_errors/check_funcs.py
+-rw-rw-rw-  2.0 fat     9408 b- defN 23-May-11 07:28 orup_errors/check_funcs.py
 -rw-rw-rw-  2.0 fat     2473 b- defN 23-May-11 06:51 orup_errors/general_functions.py
 -rw-rw-rw-  2.0 fat     2340 b- defN 23-Mar-28 11:17 orup_errors/main.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Oct-20 07:03 orup_errors/tests/__init__.py
 -rw-rw-rw-  2.0 fat     1545 b- defN 21-Oct-20 07:03 orup_errors/tests/all_errors_test.py
 -rw-rw-rw-  2.0 fat      744 b- defN 21-Oct-20 07:03 orup_errors/tests/args_test.py
 -rw-rw-rw-  2.0 fat      288 b- defN 21-Dec-03 04:31 orup_errors/tests/check_funcs_test.py
 -rw-rw-rw-  2.0 fat     1385 b- defN 21-Oct-20 07:03 orup_errors/tests/draw_win_test.py
 -rw-rw-rw-  2.0 fat     1300 b- defN 21-Dec-03 04:20 orup_errors/tests/general_functions_test.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Oct-20 07:03 orup_errors/tests/orup_errors_operator_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-11 06:53 gtki_module_orup_errors-1.36.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      156 b- defN 23-May-11 06:53 gtki_module_orup_errors-1.36.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-11 06:53 gtki_module_orup_errors-1.36.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-May-11 06:53 gtki_module_orup_errors-1.36.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1524 b- defN 23-May-11 06:53 gtki_module_orup_errors-1.36.0.dist-info/RECORD
-17 files, 39130 bytes uncompressed, 10419 bytes compressed:  73.4%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-11 07:28 gtki_module_orup_errors-1.36.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      156 b- defN 23-May-11 07:28 gtki_module_orup_errors-1.36.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-11 07:28 gtki_module_orup_errors-1.36.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-May-11 07:28 gtki_module_orup_errors-1.36.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1524 b- defN 23-May-11 07:28 gtki_module_orup_errors-1.36.1.dist-info/RECORD
+17 files, 39215 bytes uncompressed, 10432 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: orup_errors/tests/general_functions_test.py
 Comment: 
 
 Filename: orup_errors/tests/orup_errors_operator_test.py
 Comment: 
 
-Filename: gtki_module_orup_errors-1.36.0.dist-info/LICENSE
+Filename: gtki_module_orup_errors-1.36.1.dist-info/LICENSE
 Comment: 
 
-Filename: gtki_module_orup_errors-1.36.0.dist-info/METADATA
+Filename: gtki_module_orup_errors-1.36.1.dist-info/METADATA
 Comment: 
 
-Filename: gtki_module_orup_errors-1.36.0.dist-info/WHEEL
+Filename: gtki_module_orup_errors-1.36.1.dist-info/WHEEL
 Comment: 
 
-Filename: gtki_module_orup_errors-1.36.0.dist-info/top_level.txt
+Filename: gtki_module_orup_errors-1.36.1.dist-info/top_level.txt
 Comment: 
 
-Filename: gtki_module_orup_errors-1.36.0.dist-info/RECORD
+Filename: gtki_module_orup_errors-1.36.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## orup_errors/check_funcs.py

```diff
@@ -73,14 +73,16 @@
     return check_type_incorrectness(type_name, types_list)
 
 
 def check_carrier_debtor(carrier_name: str, debtors_list: list, comment, *args,
                          **kwargs):
     aborted_contract = None
     actual_contract = None
+    banned = False
+    ban_reason = None
     for debtor_l in debtors_list: # Перебираем список договоров
         if debtor_l['name'] == carrier_name: # Нашли договор организации
             banned = debtor_l['banned']
             ban_reason = debtor_l['ban_reason']
             if (ban_reason and isinstance(ban_reason, str)
                     and 'приостановлен' in ban_reason.lower()):
                 # Если есть приостановленный договор - сразу запрет
@@ -104,18 +106,20 @@
     if aborted_contract and actual_contract:
         # Проверяем, если у орагнизации есть прекращенный договор без долго + актуальный, все ок
         return
     if banned:
         # Если же мы дошли сюда, и есть причина запрета - выводим ее
         return ban_reason
 
-def check_carrier_debtor(client_name: str, debtors_list: list, comment, *args,
+def check_client_debtor(client_name: str, debtors_list: list, comment, *args,
                          **kwargs):
     aborted_contract = None
     actual_contract = None
+    banned = False
+    ban_reason = None
     for debtor_l in debtors_list: # Перебираем список договоров
         if debtor_l['name'] == client_name: # Нашли договор организации
             banned = debtor_l['banned']
             ban_reason = debtor_l['ban_reason']
             if (ban_reason and isinstance(ban_reason, str)
                     and 'приостановлен' in ban_reason.lower()):
                 # Если есть приостановленный договор - сразу запрет
```

## Comparing `gtki_module_orup_errors-1.36.0.dist-info/LICENSE` & `gtki_module_orup_errors-1.36.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gtki_module_orup_errors-1.36.0.dist-info/RECORD` & `gtki_module_orup_errors-1.36.1.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 orup_errors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 orup_errors/all_errors.py,sha256=rU5KKPhSNn9JGTDybC_krJdhVdmNUzas_2tqDdhneYU,16857
-orup_errors/check_funcs.py,sha256=qjaDl3kAjowtZ5_3yUAVUjWCtWBnHwlDaw_fWHdzZdI,9323
+orup_errors/check_funcs.py,sha256=CXYr-YHObEABuNX_b3svPovRRRJolA4DG0uzMTHfZ1I,9408
 orup_errors/general_functions.py,sha256=4nvGzaj0MwcFeQlDhR1JUaZB1DNdo2nLnwbcMjNxjP8,2473
 orup_errors/main.py,sha256=0rAbiAqmCHK-T_hmEedmofODsCQPEaxR57b2AYb9wWI,2340
 orup_errors/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 orup_errors/tests/all_errors_test.py,sha256=Lxq5C6Ka5XaHPOVMCQdMSuZT3l07TaJuoGP5l4ZJU_0,1545
 orup_errors/tests/args_test.py,sha256=rz64Iv4D8nPuDlATAHuO_4wFRS20b71gYsIyotaw1pI,744
 orup_errors/tests/check_funcs_test.py,sha256=m5e0kAHg5AcEi2VfRLBEslCAKfFDs8ARWb8emZ_j1Pk,288
 orup_errors/tests/draw_win_test.py,sha256=dsrfPhbnArm08IukF_zypmUFYOw1wjHD_5qYHYjk-88,1385
 orup_errors/tests/general_functions_test.py,sha256=CHoOqcw6k2qLUfgHnGA4TTgACt25jIZNDkF0UnKRtlQ,1300
 orup_errors/tests/orup_errors_operator_test.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gtki_module_orup_errors-1.36.0.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-gtki_module_orup_errors-1.36.0.dist-info/METADATA,sha256=8o-DxcNoQCdJkfiMwEwpVZV6ZjvwejvefTuULwhgXc8,156
-gtki_module_orup_errors-1.36.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gtki_module_orup_errors-1.36.0.dist-info/top_level.txt,sha256=WzasBtx2xqnJAQK3vavyWJNr2nwUAPObo6jw7F1FFko,12
-gtki_module_orup_errors-1.36.0.dist-info/RECORD,,
+gtki_module_orup_errors-1.36.1.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+gtki_module_orup_errors-1.36.1.dist-info/METADATA,sha256=4khXv89qD-S95efW-HkB2fk4FDL51e3PdUnGx88sK3E,156
+gtki_module_orup_errors-1.36.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gtki_module_orup_errors-1.36.1.dist-info/top_level.txt,sha256=WzasBtx2xqnJAQK3vavyWJNr2nwUAPObo6jw7F1FFko,12
+gtki_module_orup_errors-1.36.1.dist-info/RECORD,,
```

