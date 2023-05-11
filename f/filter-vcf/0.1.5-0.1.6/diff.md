# Comparing `tmp/filter-vcf-0.1.5.tar.gz` & `tmp/filter-vcf-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filter-vcf-0.1.5.tar", last modified: Thu Apr 27 13:45:51 2023, max compression
+gzip compressed data, was "filter-vcf-0.1.6.tar", last modified: Thu May 11 16:57:49 2023, max compression
```

## Comparing `filter-vcf-0.1.5.tar` & `filter-vcf-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       13 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/PYPI.md
--rw-r--r--   0        0        0        0 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/filter_vcf/__init__.py
--rw-r--r--   0        0        0      675 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/filter_vcf/filter_vcf.py
--rw-r--r--   0        0        0     5829 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/filter_vcf/process.py
--rw-r--r--   0        0        0        0 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/filter_vcf/util/__init__.py
--rw-r--r--   0        0        0     1791 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/filter_vcf/util/addDepth.py
--rw-r--r--   0        0        0     3692 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/filter_vcf/util/checkArgs.py
--rw-r--r--   0        0        0     2435 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/filter_vcf/util/cleanAD.py
--rw-r--r--   0        0        0     4257 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/filter_vcf/util/cleanGT.py
--rw-r--r--   0        0        0     1753 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/filter_vcf/util/convertChrName.py
--rw-r--r--   0        0        0      631 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/filter_vcf/util/detectVcf.py
--rw-r--r--   0        0        0      814 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/filter_vcf/util/readVcf.py
--rw-r--r--   0        0        0      720 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/filter_vcf/util/removeNonRef.py
--rw-r--r--   0        0        0      779 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/filter_vcf/util/sortVcf.py
--rw-r--r--   0        0        0      781 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/filter_vcf/util/unique.py
--rw-r--r--   0        0        0     1485 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/filter_vcf/util/userFilter.py
--rw-r--r--   0        0        0      273 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/filter_vcf/util/writeVcf.py
--rw-r--r--   0        0        0      899 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       28 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/tests/resources/GRCh37.fa.gz
--rw-r--r--   0        0        0    62676 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/tests/resources/carisSample.lifted.modified.somatic.vcf.gz
--rw-r--r--   0        0        0     3490 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/tests/resources/decomp.vcf
--rw-r--r--   0        0        0     1443 2023-04-27 13:43:12.839239 filter-vcf-0.1.5/tests/resources/foundationSample.tcf.gz
--rw-r--r--   0        0        0   270284 2023-04-27 13:43:12.843239 filter-vcf-0.1.5/tests/resources/full.vcf
--rw-r--r--   0        0        0     1682 2023-04-27 13:43:12.843239 filter-vcf-0.1.5/tests/resources/presorted.vcf
--rw-r--r--   0        0        0    62601 2023-04-27 13:43:12.843239 filter-vcf-0.1.5/tests/resources/sample.nrm.vcf.gz
--rw-r--r--   0        0        0     1682 2023-04-27 13:43:12.843239 filter-vcf-0.1.5/tests/resources/unsorted.vcf
--rw-r--r--   0        0        0      514 2023-04-27 13:43:12.843239 filter-vcf-0.1.5/tests/resources/unsorted.vcf.gz
--rw-r--r--   0        0        0       40 2023-04-27 13:43:12.843239 filter-vcf-0.1.5/tests/resources/vcf.txt
--rw-r--r--   0        0        0    46946 2023-04-27 13:43:12.843239 filter-vcf-0.1.5/tests/test_process.py
--rw-r--r--   0        0        0      245 1970-01-01 00:00:00.000000 filter-vcf-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/PYPI.md
+-rw-r--r--   0        0        0        0 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/filter_vcf/__init__.py
+-rw-r--r--   0        0        0      675 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/filter_vcf/filter_vcf.py
+-rw-r--r--   0        0        0     5986 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/filter_vcf/process.py
+-rw-r--r--   0        0        0        0 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/filter_vcf/util/__init__.py
+-rw-r--r--   0        0        0     1791 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/filter_vcf/util/addDepth.py
+-rw-r--r--   0        0        0     3692 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/filter_vcf/util/checkArgs.py
+-rw-r--r--   0        0        0     2435 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/filter_vcf/util/cleanAD.py
+-rw-r--r--   0        0        0     4257 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/filter_vcf/util/cleanGT.py
+-rw-r--r--   0        0        0     1753 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/filter_vcf/util/convertChrName.py
+-rw-r--r--   0        0        0      631 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/filter_vcf/util/detectVcf.py
+-rw-r--r--   0        0        0      814 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/filter_vcf/util/readVcf.py
+-rw-r--r--   0        0        0      720 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/filter_vcf/util/removeNonRef.py
+-rw-r--r--   0        0        0      779 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/filter_vcf/util/sortVcf.py
+-rw-r--r--   0        0        0      781 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/filter_vcf/util/unique.py
+-rw-r--r--   0        0        0     1485 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/filter_vcf/util/userFilter.py
+-rw-r--r--   0        0        0      273 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/filter_vcf/util/writeVcf.py
+-rw-r--r--   0        0        0      899 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/tests/resources/GRCh37.fa.gz
+-rw-r--r--   0        0        0    62676 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/tests/resources/carisSample.lifted.modified.somatic.vcf.gz
+-rw-r--r--   0        0        0     3490 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/tests/resources/decomp.vcf
+-rw-r--r--   0        0        0     1443 2023-05-11 16:55:29.655348 filter-vcf-0.1.6/tests/resources/foundationSample.tcf.gz
+-rw-r--r--   0        0        0   270284 2023-05-11 16:55:29.659349 filter-vcf-0.1.6/tests/resources/full.vcf
+-rw-r--r--   0        0        0     1682 2023-05-11 16:55:29.659349 filter-vcf-0.1.6/tests/resources/presorted.vcf
+-rw-r--r--   0        0        0    62601 2023-05-11 16:55:29.659349 filter-vcf-0.1.6/tests/resources/sample.nrm.vcf.gz
+-rw-r--r--   0        0        0     1682 2023-05-11 16:55:29.659349 filter-vcf-0.1.6/tests/resources/unsorted.vcf
+-rw-r--r--   0        0        0      514 2023-05-11 16:55:29.659349 filter-vcf-0.1.6/tests/resources/unsorted.vcf.gz
+-rw-r--r--   0        0        0       40 2023-05-11 16:55:29.659349 filter-vcf-0.1.6/tests/resources/vcf.txt
+-rw-r--r--   0        0        0    47388 2023-05-11 16:55:29.659349 filter-vcf-0.1.6/tests/test_process.py
+-rw-r--r--   0        0        0      245 1970-01-01 00:00:00.000000 filter-vcf-0.1.6/PKG-INFO
```

### Comparing `filter-vcf-0.1.5/filter_vcf/filter_vcf.py` & `filter-vcf-0.1.6/filter_vcf/filter_vcf.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.5/filter_vcf/process.py` & `filter-vcf-0.1.6/filter_vcf/process.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,14 +123,16 @@
                 os.system(f"gzip {tmp_dir}/normalized.vcf")
                 os.rename(f"{tmp_dir}/normalized.vcf.gz", in_file)
                 working_vcf = read_vcf(in_file, log).to_string()
                 working_vcf = convert_chr_name(working_vcf, "chr", log)
 
             else:
                 write_vcf(working_vcf, in_file, True, log)
+                if args["filterContig"] == False:
+                    subprocess.run(f"tabix -p vcf {in_file}", shell=True, check=True)
                 subprocess.run(
                     f"vt normalize -n -r {ref_file} {in_file} -o {tmp_dir}/normalized.vcf",
                     shell=True,
                     check=True,
                 )
                 os.system(f"gzip {tmp_dir}/normalized.vcf")
                 os.rename(f"{tmp_dir}/normalized.vcf.gz", in_file)
@@ -143,7 +145,9 @@
             working_vcf = keep_unique_variants(working_vcf, log)
 
         if args["filters"] != "":
             working_vcf = perform_filter_vcf(working_vcf, args["filters"], log)
 
         log.info(f"Writing output to {args['output']}")
         write_vcf(working_vcf, args["output"], compression=True, log=log)
+
+        return args
```

### Comparing `filter-vcf-0.1.5/filter_vcf/util/addDepth.py` & `filter-vcf-0.1.6/filter_vcf/util/addDepth.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.5/filter_vcf/util/checkArgs.py` & `filter-vcf-0.1.6/filter_vcf/util/checkArgs.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.5/filter_vcf/util/cleanAD.py` & `filter-vcf-0.1.6/filter_vcf/util/cleanAD.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.5/filter_vcf/util/cleanGT.py` & `filter-vcf-0.1.6/filter_vcf/util/cleanGT.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.5/filter_vcf/util/convertChrName.py` & `filter-vcf-0.1.6/filter_vcf/util/convertChrName.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.5/filter_vcf/util/detectVcf.py` & `filter-vcf-0.1.6/filter_vcf/util/detectVcf.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.5/filter_vcf/util/readVcf.py` & `filter-vcf-0.1.6/filter_vcf/util/readVcf.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.5/filter_vcf/util/removeNonRef.py` & `filter-vcf-0.1.6/filter_vcf/util/removeNonRef.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.5/filter_vcf/util/sortVcf.py` & `filter-vcf-0.1.6/filter_vcf/util/sortVcf.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.5/filter_vcf/util/unique.py` & `filter-vcf-0.1.6/filter_vcf/util/unique.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.5/filter_vcf/util/userFilter.py` & `filter-vcf-0.1.6/filter_vcf/util/userFilter.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.5/pyproject.toml` & `filter-vcf-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "filter-vcf"
-version = "0.1.5"
+version = "0.1.6"
 description = "LifeOmic VCF filtering"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging==0.3.2",
     "vcfpy>=0.13.4",
```

### Comparing `filter-vcf-0.1.5/tests/resources/carisSample.lifted.modified.somatic.vcf.gz` & `filter-vcf-0.1.6/tests/resources/carisSample.lifted.modified.somatic.vcf.gz`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.5/tests/resources/decomp.vcf` & `filter-vcf-0.1.6/tests/resources/decomp.vcf`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.5/tests/resources/foundationSample.tcf.gz` & `filter-vcf-0.1.6/tests/resources/foundationSample.tcf.gz`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.5/tests/resources/full.vcf` & `filter-vcf-0.1.6/tests/resources/full.vcf`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.5/tests/resources/presorted.vcf` & `filter-vcf-0.1.6/tests/resources/presorted.vcf`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.5/tests/resources/sample.nrm.vcf.gz` & `filter-vcf-0.1.6/tests/resources/sample.nrm.vcf.gz`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.5/tests/resources/unsorted.vcf` & `filter-vcf-0.1.6/tests/resources/unsorted.vcf`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.5/tests/resources/unsorted.vcf.gz` & `filter-vcf-0.1.6/tests/resources/unsorted.vcf.gz`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.5/tests/test_process.py` & `filter-vcf-0.1.6/tests/test_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -861,16 +861,28 @@
         "normalize": False,
         "unique": True,
         "filterContig": False,
         "depth": True,
         "filters": "PASS",
     }
 
-    normalize_vcf(arguments)
+    args = normalize_vcf(arguments)
 
     assert (
         os.path.exists(
             f"{BASE_PATH}/resources/carisSample.lifted.modified.somatic.filtered.nrm.vcf.gz"
         )
         == True
     )
     os.remove(f"{BASE_PATH}/resources/carisSample.lifted.modified.somatic.filtered.nrm.vcf.gz")
+
+    assert args == {
+        "reference": f"{BASE_PATH}/resources/GRCh37.fa.gz",
+        "input": f"{BASE_PATH}/resources/carisSample.lifted.modified.somatic.vcf.gz",
+        "output": f"{BASE_PATH}/resources/carisSample.lifted.modified.somatic.filtered.nrm.vcf.gz",
+        "decompose": False,
+        "normalize": False,
+        "unique": True,
+        "filterContig": False,
+        "depth": True,
+        "filters": "PASS",
+    }
```

