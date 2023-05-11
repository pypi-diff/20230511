# Comparing `tmp/newWhoisBobPkgs-1.0.0.8-py3-none-any.whl.zip` & `tmp/newWhoisBobPkgs-1.0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 13678 bytes, number of entries: 12
--rw-rw-r--  2.0 unx    13679 b- defN 22-Oct-31 02:34 bobwhois.py
+Zip file size: 13677 bytes, number of entries: 12
+-rw-rw-r--  2.0 unx    13679 b- defN 22-Oct-31 02:38 bobwhois.py
 -rw-rw-r--  2.0 unx     9072 b- defN 22-Aug-22 02:39 kisa.py
 -rw-rw-r--  2.0 unx       30 b- defN 22-Aug-22 02:39 kisaBobPkgs.py
 -rw-rw-r--  2.0 unx       31 b- defN 22-Oct-22 15:52 newWhoisBobPkgs.py
 -rw-rw-r--  2.0 unx       46 b- defN 22-Aug-22 02:39 test_bob8gook.py
 -rw-rw-r--  2.0 unx       30 b- defN 22-Aug-22 02:39 testbob8gook.py
 -rw-rw-r--  2.0 unx    13594 b- defN 22-Oct-22 15:44 whois.py
 -rw-rw-r--  2.0 unx       31 b- defN 22-Oct-22 15:52 whoisBobPkgs.py
--rw-rw-r--  2.0 unx      205 b- defN 22-Oct-31 02:35 newWhoisBobPkgs-1.0.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Oct-31 02:35 newWhoisBobPkgs-1.0.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       25 b- defN 22-Oct-31 02:35 newWhoisBobPkgs-1.0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      889 b- defN 22-Oct-31 02:35 newWhoisBobPkgs-1.0.0.8.dist-info/RECORD
-12 files, 37724 bytes uncompressed, 12200 bytes compressed:  67.7%
+-rw-rw-r--  2.0 unx      205 b- defN 22-Oct-31 02:38 newWhoisBobPkgs-1.0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Oct-31 02:38 newWhoisBobPkgs-1.0.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       25 b- defN 22-Oct-31 02:38 newWhoisBobPkgs-1.0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      889 b- defN 22-Oct-31 02:38 newWhoisBobPkgs-1.0.0.9.dist-info/RECORD
+12 files, 37724 bytes uncompressed, 12199 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: whois.py
 Comment: 
 
 Filename: whoisBobPkgs.py
 Comment: 
 
-Filename: newWhoisBobPkgs-1.0.0.8.dist-info/METADATA
+Filename: newWhoisBobPkgs-1.0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: newWhoisBobPkgs-1.0.0.8.dist-info/WHEEL
+Filename: newWhoisBobPkgs-1.0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: newWhoisBobPkgs-1.0.0.8.dist-info/top_level.txt
+Filename: newWhoisBobPkgs-1.0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: newWhoisBobPkgs-1.0.0.8.dist-info/RECORD
+Filename: newWhoisBobPkgs-1.0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bobwhois.py

```diff
@@ -12,18 +12,18 @@
 import threading
 from apscheduler.schedulers.background import BlockingScheduler
 
 
 whitelist_ip = ''
 whitelist_description = ''
 whitelist_country = ''
-#botEmail = "bob8gook_whois@webex.bot"
-botEmail = "bob8gook_test@webex.bot"
-#accessToken = "MGY3ZWI0N2ItZjI0ZC00MzQ2LWFlNjYtNDc0MWM3NDNlNGQ2ODI1MzQ4MzAtZmMz_PF84_22cb7792-d880-4ec5-b6a6-649d9411bb5e"
-accessToken = 'NDIzZjQwMjktMzEyMi00Zjg2LTk0ZWMtYTgzZWExMTRlMWY4MzA5NjZmYzEtM2E0_PF84_22cb7792-d880-4ec5-b6a6-649d9411bb5e'
+botEmail = "bob8gook_whois@webex.bot"
+#botEmail = "bob8gook_test@webex.bot"
+accessToken = "MGY3ZWI0N2ItZjI0ZC00MzQ2LWFlNjYtNDc0MWM3NDNlNGQ2ODI1MzQ4MzAtZmMz_PF84_22cb7792-d880-4ec5-b6a6-649d9411bb5e"
+#accessToken = 'NDIzZjQwMjktMzEyMi00Zjg2LTk0ZWMtYTgzZWExMTRlMWY4MzA5NjZmYzEtM2E0_PF84_22cb7792-d880-4ec5-b6a6-649d9411bb5e'
 headers = {"Authorization": "Bearer %s" % accessToken, "Content-Type": "application/json", 'Accept' : 'application/json'}
 
 now = datetime.datetime.now()
 now = now + datetime.timedelta(days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=9, weeks=0)
 
 fPath_working = os.getcwd()
```

## Comparing `newWhoisBobPkgs-1.0.0.8.dist-info/RECORD` & `newWhoisBobPkgs-1.0.0.9.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-bobwhois.py,sha256=-_7SAPZtyrI-aRBEoRkU3_IWSIV_7xlLR4xoijiU9w4,13679
+bobwhois.py,sha256=-KumbQVwvNXpIB3a738yJ2cHbH_9HygretoP2YJ6Nu4,13679
 kisa.py,sha256=T1acpCjxR_4ZORv8qh1FsWoR6Tqp9AhiKaOpe8K8cMs,9072
 kisaBobPkgs.py,sha256=rIZfeOARwpySPpRj_tnnoZHjcE4m5ioqFWTP8wVb8ZM,30
 newWhoisBobPkgs.py,sha256=guIuOR4ofGmQdmGegzptp-Kp5JTWXpEQATvcSVMQCtA,31
 test_bob8gook.py,sha256=rKYmL-vMQUEsRrzcOYH3ZK9LUPJhhAPgf8q4bL8-EZ4,46
 testbob8gook.py,sha256=rIZfeOARwpySPpRj_tnnoZHjcE4m5ioqFWTP8wVb8ZM,30
 whois.py,sha256=EAwi7BR_voiSTLmfyxAELvctxAo_SJWW4NghVCpwmbY,13594
 whoisBobPkgs.py,sha256=guIuOR4ofGmQdmGegzptp-Kp5JTWXpEQATvcSVMQCtA,31
-newWhoisBobPkgs-1.0.0.8.dist-info/METADATA,sha256=m7tpBlyC_jWCMNpPvPR_BLxit82vFHQEzg2ofOwTilI,205
-newWhoisBobPkgs-1.0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-newWhoisBobPkgs-1.0.0.8.dist-info/top_level.txt,sha256=qGY_9y5C1CwBFsJAFNz2etNSfMnvfBvklaUikbhLu8Y,25
-newWhoisBobPkgs-1.0.0.8.dist-info/RECORD,,
+newWhoisBobPkgs-1.0.0.9.dist-info/METADATA,sha256=gzhJCijcu30AZLmzl0lOT6WuAv9542R94AWfrIdbtnI,205
+newWhoisBobPkgs-1.0.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+newWhoisBobPkgs-1.0.0.9.dist-info/top_level.txt,sha256=qGY_9y5C1CwBFsJAFNz2etNSfMnvfBvklaUikbhLu8Y,25
+newWhoisBobPkgs-1.0.0.9.dist-info/RECORD,,
```

