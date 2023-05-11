# Comparing `tmp/ar_ex_sys_worker-1.6.11-py3-none-any.whl.zip` & `tmp/ar_ex_sys_worker-1.6.20-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 16123 bytes, number of entries: 11
+Zip file size: 16230 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:51 ar_external_sys_worker/__init__.py
--rw-rw-rw-  2.0 fat    27217 b- defN 23-Apr-25 11:47 ar_external_sys_worker/main.py
+-rw-rw-rw-  2.0 fat    27414 b- defN 23-Apr-28 12:31 ar_external_sys_worker/main.py
 -rw-rw-rw-  2.0 fat    19883 b- defN 23-Apr-25 07:19 ar_external_sys_worker/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:52 ar_external_sys_worker/tests/__init__.py
--rw-rw-rw-  2.0 fat    10365 b- defN 23-Apr-25 11:29 ar_external_sys_worker/tests/main_test.py
+-rw-rw-rw-  2.0 fat    11225 b- defN 23-Apr-28 12:19 ar_external_sys_worker/tests/main_test.py
 -rw-rw-rw-  2.0 fat     1107 b- defN 23-Apr-25 11:47 ar_external_sys_worker/tests/mixins_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-25 11:48 ar_ex_sys_worker-1.6.11.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      344 b- defN 23-Apr-25 11:48 ar_ex_sys_worker-1.6.11.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-25 11:48 ar_ex_sys_worker-1.6.11.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-25 11:48 ar_ex_sys_worker-1.6.11.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      994 b- defN 23-Apr-25 11:48 ar_ex_sys_worker-1.6.11.dist-info/RECORD
-11 files, 61116 bytes uncompressed, 14407 bytes compressed:  76.4%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-28 12:31 ar_ex_sys_worker-1.6.20.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      344 b- defN 23-Apr-28 12:31 ar_ex_sys_worker-1.6.20.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 12:31 ar_ex_sys_worker-1.6.20.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-28 12:31 ar_ex_sys_worker-1.6.20.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      994 b- defN 23-Apr-28 12:31 ar_ex_sys_worker-1.6.20.dist-info/RECORD
+11 files, 62173 bytes uncompressed, 14514 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: ar_external_sys_worker/tests/main_test.py
 Comment: 
 
 Filename: ar_external_sys_worker/tests/mixins_test.py
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.11.dist-info/LICENSE
+Filename: ar_ex_sys_worker-1.6.20.dist-info/LICENSE
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.11.dist-info/METADATA
+Filename: ar_ex_sys_worker-1.6.20.dist-info/METADATA
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.11.dist-info/WHEEL
+Filename: ar_ex_sys_worker-1.6.20.dist-info/WHEEL
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.11.dist-info/top_level.txt
+Filename: ar_ex_sys_worker-1.6.20.dist-info/top_level.txt
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.11.dist-info/RECORD
+Filename: ar_ex_sys_worker-1.6.20.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ar_external_sys_worker/main.py

```diff
@@ -336,22 +336,23 @@
         return date
 
 
 class SignallActWorker(mixins.SignallMixin, ActsWorker,
                        mixins.SignallPhotoEncoderMixin,
                        mixins.SignallGetCarriersPO):
     def __init__(self, sql_shell, trash_cats_list, time_start, acts_limit=5,
-                 login=None, password=None, auto_auth=True):
+                 login=None, password=None, auto_auth=True, mutex=None):
         super().__init__(sql_shell=sql_shell, trash_cats=trash_cats_list,
                          time_start=time_start, acts_limit=acts_limit,
                          login=login, password=password, auto_auth=auto_auth)
         self.get_carriers_po_link = self.get_full_endpoint(
             self.link_get_po_links)
         self.act_id_from_response = 'act_id'
-        self.mutex = allocate_lock()
+        if mutex:
+            self.mutex = mutex
 
     def format_file_before_logging(self, data):
         data = json.loads(data)
         data.pop('photos')
         print(data)
         return str(data).replace("'", '"')
 
@@ -448,39 +449,45 @@
             'platform_type': act['pol_object'],
             "act_number": {'number': act['act_number'],
                            'package': act['package_name']},
         }
         act_json = json.dumps(data)
         return act_json
 
+
 class SignAllActsWorkerToken(mixins.TokenAuth, SignallActWorker,
                              mixins.TokenDBAuth, mixins.SignallActDBDeletter):
     def __init__(self, sql_shell, trash_cats_list, time_start, platform_id,
-                 acts_limit=5, gravity_ip=None, gravity_port=8080, test=False):
+                 acts_limit=5, gravity_ip=None, gravity_port=8080, test=False,
+                 mutex=None):
         super().__init__(sql_shell, trash_cats_list, time_start, acts_limit,
-                         auto_auth=False)
+                         auto_auth=False, mutex=mutex)
         self.platform_id = platform_id
         self.gravity_ip = gravity_ip
         if not self.gravity_ip:
             s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
             s.connect(("8.8.8.8", 80))
             self.gravity_ip = s.getsockname()[0]
         self.gravity_port = gravity_port
         platform_info = self.get_platform_info()[0]
         self.inn, self.kpp = platform_info['inn'], platform_info['kpp']
         if test:
             self.link_host = 'https://signalltestdev.qodex.tech'
 
     def resend_unget_acts(self):
+        print("Resending acts")
+        self.mutex.acquire()
         unsend_acts = self.get_unget_by_signall_acts()
         if not unsend_acts:
+            self.mutex.release()
             return
         for act in unsend_acts:
             self.delete_act_from_send_reports(act['local_id'])
         self.send_unsend_acts(limit=len(unsend_acts))
+        self.mutex.release()
 
     @wsqluse.wsqluse.getTableDictStripper
     def get_platform_info(self):
         return self.sql_shell.get_table_dict(
             command=f"SELECT inn, kpp FROM duo_pol_owners "
                     f"WHERE id={self.platform_id}")
```

## ar_external_sys_worker/tests/main_test.py

```diff
@@ -1,9 +1,10 @@
 import datetime
 import os
+import time
 import unittest
 import threading
 import wsqluse.wsqluse
 import timeit
 import calendar
 from ar_external_sys_worker import main
 
@@ -209,15 +210,34 @@
                                   login="api", password="qwer1234")
         for car_num in car_nums:
             print('\n')
             print(car_num)
             res = inst.get_route_info('В292МР702', '05.12.2022')
             print(res)
 
-    def test_signall_worker_token(self):
+    def test_mutex(self):
+        print("first_go")
+        inst = main.SignAllActsWorkerToken(self.sql_shell,
+                                           ['ТКО', 'Прочее', 'ПО', 'Хвосты'],
+                                           '2023.04.24',
+                                           1,
+                                           gravity_ip='172.16.9.20',
+                                           test=True)
+        inst.set_signall_test()
+        #inst.link_host = 'https://signalltestdev.qodex.tech'
+        inst.auth()
+        threading.Thread(target=inst.send_unsend_acts).start()
+        time.sleep(2)
+        print("second_go")
+        threading.Thread(target=inst.send_unsend_acts).start()
+        time.sleep(2)
+        print("third_go")
+        threading.Thread(target=inst.send_unsend_acts).start()
+
+    def signall_worker_token(self):
         inst = main.SignAllActsWorkerToken(self.sql_shell,
                                            ['ТКО', 'Прочее', 'ПО', 'Хвосты'],
                                            '2023.04.24',
                                            1,
                                            gravity_ip='172.16.9.20',
                                            test=True)
         inst.set_signall_test()
```

## Comparing `ar_ex_sys_worker-1.6.11.dist-info/LICENSE` & `ar_ex_sys_worker-1.6.20.dist-info/LICENSE`

 * *Files identical despite different names*

