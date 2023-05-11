# Comparing `tmp/pydan-6.9-py3-none-any.whl.zip` & `tmp/pydan-7.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,17 @@
-Zip file size: 22144 bytes, number of entries: 16
--rw-r-----  2.0 unx       47 b- defN 23-Feb-10 12:05 pydan/__init__.py
--rw-r-----  2.0 unx      972 b- defN 23-Mar-08 09:25 pydan/ansi.py
--rw-r-----  2.0 unx     2489 b- defN 23-Jan-08 14:55 pydan/api.py
--rw-r-----  2.0 unx    27870 b- defN 23-Mar-08 10:12 pydan/jdata.py
--rw-r-----  2.0 unx     4021 b- defN 23-Jan-08 14:55 pydan/log.py
--rw-r-----  2.0 unx    13087 b- defN 23-Jan-26 10:44 pydan/logsmart.py
--rw-r-----  2.0 unx     8662 b- defN 23-Jan-08 14:55 pydan/logsmartold.py
--rw-r-----  2.0 unx     1848 b- defN 23-Jan-08 14:55 pydan/muid.py
--rw-r-----  2.0 unx      567 b- defN 23-Jan-08 14:55 pydan/run.py
--rw-r-----  2.0 unx     3157 b- defN 23-Jan-08 14:55 pydan/script.py
--rw-r-----  2.0 unx      602 b- defN 23-Jan-08 14:55 pydan/utils.py
--rw-r-----  2.0 unx      345 b- defN 23-Jan-08 14:55 pydan/xdata.py
--rw-r-----  2.0 unx      314 b- defN 23-Mar-08 10:13 pydan-6.9.dist-info/METADATA
--rw-r-----  2.0 unx       92 b- defN 23-Mar-08 10:13 pydan-6.9.dist-info/WHEEL
--rw-r-----  2.0 unx        6 b- defN 23-Mar-08 10:13 pydan-6.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1133 b- defN 23-Mar-08 10:13 pydan-6.9.dist-info/RECORD
-16 files, 65212 bytes uncompressed, 20336 bytes compressed:  68.8%
+Zip file size: 22028 bytes, number of entries: 15
+-rw-rw----  2.0 unx      972 b- defN 23-Mar-21 07:36 pydan/ansi.py
+-rw-rw----  2.0 unx     2489 b- defN 23-Jan-17 07:57 pydan/api.py
+-rw-rw----  2.0 unx    28055 b- defN 23-May-11 11:36 pydan/jdata.py
+-rw-rw----  2.0 unx     4021 b- defN 23-Jan-17 07:57 pydan/log.py
+-rw-rw----  2.0 unx    13087 b- defN 23-Jan-25 12:37 pydan/logsmart.py
+-rw-rw----  2.0 unx     8662 b- defN 23-Jan-17 07:57 pydan/logsmartold.py
+-rw-rw----  2.0 unx     1848 b- defN 23-Jan-17 07:57 pydan/muid.py
+-rw-rw----  2.0 unx      567 b- defN 23-Jan-17 07:57 pydan/run.py
+-rw-rw----  2.0 unx     3157 b- defN 23-Jan-17 07:57 pydan/script.py
+-rw-rw----  2.0 unx      602 b- defN 23-Jan-17 07:57 pydan/utils.py
+-rw-rw----  2.0 unx      345 b- defN 23-Jan-17 07:57 pydan/xdata.py
+-rw-rw----  2.0 unx      314 b- defN 23-May-11 11:50 pydan-7.1.dist-info/METADATA
+-rw-rw----  2.0 unx       92 b- defN 23-May-11 11:50 pydan-7.1.dist-info/WHEEL
+-rw-rw----  2.0 unx        6 b- defN 23-May-11 11:50 pydan-7.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1061 b- defN 23-May-11 11:50 pydan-7.1.dist-info/RECORD
+15 files, 65278 bytes uncompressed, 20330 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -1,10 +1,7 @@
-Filename: pydan/__init__.py
-Comment: 
-
 Filename: pydan/ansi.py
 Comment: 
 
 Filename: pydan/api.py
 Comment: 
 
 Filename: pydan/jdata.py
@@ -30,20 +27,20 @@
 
 Filename: pydan/utils.py
 Comment: 
 
 Filename: pydan/xdata.py
 Comment: 
 
-Filename: pydan-6.9.dist-info/METADATA
+Filename: pydan-7.1.dist-info/METADATA
 Comment: 
 
-Filename: pydan-6.9.dist-info/WHEEL
+Filename: pydan-7.1.dist-info/WHEEL
 Comment: 
 
-Filename: pydan-6.9.dist-info/top_level.txt
+Filename: pydan-7.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pydan-6.9.dist-info/RECORD
+Filename: pydan-7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pydan/jdata.py

```diff
@@ -572,18 +572,27 @@
 			print(" (no vars)", end="")
 		out=data
 	else:
 		if __debug:
 			print(" (vars found)", end="")
 		# Hay variables
 		for sk in vars:
-			if sk not in varlist and "unkempty" not in flags:
-				print(f" ({sk} not in varlist)", end="")
-				continue
-			val=varlist.get(sk)
+			#if sk not in varlist and "unkempty" not in flags:
+			#	print(f" ({sk} not in varlist)", end="")
+			#	continue
+			#val=varlist.get(sk)
+			#val={"a":"claro","b":"si","c":42}
+			val=varlist
+			for skitem in sk.split("."):
+				if type(val)==dict and skitem in val:
+					val=val[skitem]
+				else:
+					val=None
+					break
+
 			if val is None and "unkempty" in flags: val=''
 			if __debug:
 				print(f" (replace '{sk}' for '{val}')", end="")
 			#if val is None:
 			#	if (unknownempty): val=""
 			#	else:
 			#		if (unknownnull):
@@ -934,16 +943,16 @@
 				if os.path.isfile(f):
 					with open(f, 'r') as s: subdata=ruamel.yaml.load(s, Loader=ruamel.yaml.Loader)
 					data.update(subdata)
 		data.pop("yaml-include")
 
 
 	# reemplazamos links de variables creadas con !var
-	dataflat=flatten(data)
-	data2=replacevars(data, dataflat, lsep="$$", rsep="$$")
+	#dataflat=flatten(data)
+	data2=replacevars(data, data, lsep="$$", rsep="$$")
 
 	return data2
 
 def yamlupdate(filename,var,val,node=None):
 	yaml=ruamel.yaml.YAML()
 	yaml.width=4096
 	f=open(filename,"r")
```

## Comparing `pydan-6.9.dist-info/RECORD` & `pydan-7.1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-pydan/__init__.py,sha256=2DUkW0FQkiC_0BBSZ93FhhXjoO27WrYwvoB4Ecl70KY,47
 pydan/ansi.py,sha256=M0d_v7JqvvqsZ4qXXC4gmKcgToqkvw-1ilKO7wm5Jdc,972
 pydan/api.py,sha256=NKt8MJ9Dk4wJQ087og2oRSv2FyjXs-b_d1nawHH51Og,2489
-pydan/jdata.py,sha256=N7GB6q3_R49gKS-fyLU7KWr5heLdR0xiE4WxY1Q8zeM,27870
+pydan/jdata.py,sha256=KirKzOHxJ0TFJEcEJIWnFkjKdGABRboYU2zxWl3dDDU,28055
 pydan/log.py,sha256=fcW6yWPDh9MeOCleF774Km5wE7pdi_14Dh6blEcAqDU,4021
 pydan/logsmart.py,sha256=xa-G_UxaAmoRIAlXzrC7Y3ZQa5YcyZyUUBLqDU27euo,13087
 pydan/logsmartold.py,sha256=_UrQieT1UyfM1rWwhgk6LyDv1JK8DBiXhYXPSXXHEFQ,8662
 pydan/muid.py,sha256=_sS1MewHare9BdHBZ_CVM1v0t8u54ig--3wbvg2PM08,1848
 pydan/run.py,sha256=NoYP_g3ZDTzBHx5i7ryol4WBP9GoW0HFhSejAOurUfQ,567
 pydan/script.py,sha256=qt4dZu5O3qQO6ro3veMsssx6SUJ0-6nKHJhrVKWYe2U,3157
 pydan/utils.py,sha256=8bW37mLyDM1VSrgqPi0DMRklIcCi1Mc1uUwSjmEbjOo,602
 pydan/xdata.py,sha256=sQEUViuC5KISYDxT8ywvdE2eUugnkuXGzr9kjBm-inU,345
-pydan-6.9.dist-info/METADATA,sha256=6EgvI9DgIEVYMbiMOqyhVyz8pWgBXzHDkNaw1Jtz9GY,314
-pydan-6.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pydan-6.9.dist-info/top_level.txt,sha256=TyPXGC1F7Xf881KyfV9TLr7g5fEddc6JF63CTG-PfAo,6
-pydan-6.9.dist-info/RECORD,,
+pydan-7.1.dist-info/METADATA,sha256=GBFWdaiQLTvIGjXhFWJ41DxaYFpp3rgb-We0L1yNQO0,314
+pydan-7.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pydan-7.1.dist-info/top_level.txt,sha256=TyPXGC1F7Xf881KyfV9TLr7g5fEddc6JF63CTG-PfAo,6
+pydan-7.1.dist-info/RECORD,,
```

