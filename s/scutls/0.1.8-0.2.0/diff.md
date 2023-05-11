# Comparing `tmp/scutls-0.1.8.tar.gz` & `tmp/scutls-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scutls-0.1.8.tar", max compression
+gzip compressed data, was "scutls-0.2.0.tar", max compression
```

## Comparing `scutls-0.1.8.tar` & `scutls-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0      583 2023-05-09 02:54:26.962623 scutls-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     6148 2022-06-21 02:55:28.045509 scutls-0.1.8/scutls/.DS_Store
--rw-r--r--   0        0        0       22 2023-01-06 05:03:16.476307 scutls-0.1.8/scutls/__init__.py
--rw-r--r--   0        0        0     5682 2023-05-09 02:41:06.226561 scutls-0.1.8/scutls/arguments.py
--rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.1.8/scutls/assets/genome_ensembl_107_54_54_54.json
--rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.1.8/scutls/assets/genome_ensembl_release_all.txt
--rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.1.8/scutls/assets/genome_ensembl_release_use.txt
--rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.1.8/scutls/assets/genome_ucsc.json
--rw-r--r--   0        0        0     3891 2023-05-09 02:52:35.471573 scutls-0.1.8/scutls/barcode.py
--rw-r--r--   0        0        0     1023 2023-05-09 02:41:24.391377 scutls-0.1.8/scutls/cli.py
--rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.1.8/scutls/download.py
--rw-r--r--   0        0        0     3603 2023-05-08 14:34:45.400997 scutls-0.1.8/scutls/fastq.py
--rw-r--r--   0        0        0     7624 2023-05-09 02:33:14.600203 scutls-0.1.8/scutls/util.py
--rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 scutls-0.1.8/setup.py
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 scutls-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-05-11 17:04:40.763821 scutls-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-11 17:04:56.253239 scutls-0.2.0/scutls/__init__.py
+-rw-r--r--   0        0        0     6256 2023-05-10 15:48:41.694697 scutls-0.2.0/scutls/arguments.py
+-rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.2.0/scutls/assets/genome_ensembl_107_54_54_54.json
+-rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.2.0/scutls/assets/genome_ensembl_release_all.txt
+-rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.2.0/scutls/assets/genome_ensembl_release_use.txt
+-rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.2.0/scutls/assets/genome_ucsc.json
+-rw-r--r--   0        0        0     4939 2023-05-10 22:02:20.277174 scutls-0.2.0/scutls/barcode.py
+-rw-r--r--   0        0        0     1074 2023-05-10 15:45:19.722039 scutls-0.2.0/scutls/cli.py
+-rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.2.0/scutls/download.py
+-rw-r--r--   0        0        0     3603 2023-05-08 14:34:45.400997 scutls-0.2.0/scutls/fastq.py
+-rw-r--r--   0        0        0     9127 2023-05-10 22:03:04.285591 scutls-0.2.0/scutls/util.py
+-rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 scutls-0.2.0/setup.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 scutls-0.2.0/PKG-INFO
```

### Comparing `scutls-0.1.8/pyproject.toml` & `scutls-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scutls"
-version = "0.1.8"
+version = "0.2.0"
 description = "Single-cell data processing utility tools"
 authors = ["Kai Hu <kai.hu@umassmed.edu>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 importlib-resources = "^5.8.0"
 wget = "^3.2"
```

### Comparing `scutls-0.1.8/scutls/arguments.py` & `scutls-0.2.0/scutls/arguments.py`

 * *Files 7% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     required = True, type = str, default = None
 )
 ## add mutually exclusive groups
 parser_fastq_group = parser_fastq.add_mutually_exclusive_group()
 parser_fastq_group.add_argument(
     "-u", "--unique",
     help = "keep unique records (by sequence ID) in fastq file",
-    required = False, default = False, action='store_true'
+    required = False, default = False, action = "store_true"
 )
 parser_fastq_group.add_argument(
     "-j", "--join",
     help = "append each read from --join fastq to corresponding line in --input fastq, not 'cat'; the read count and id must be the same in the two fastq files",
     required = False, type = str, default = None
 )
 ## set default values
@@ -124,27 +124,42 @@
 parser_barcode.add_argument(
     "-i", "--input",
     help = "input fastq, can end with .gz",
     required = True, type = str, default = None)
 parser_barcode.add_argument(
     "-o", "--output",
     help = "output fastq name, can end with .gz",
-    required = True, type = str, default = None
+    required = False, type = str, default = None
 )
 parser_barcode.add_argument(
     "-o2", "--output2",
     help = "output fastq name for non-hit reads, can end with .gz",
     required = False, type = str, default = None
 )
-parser_barcode.add_argument(
+
+
+## add mutually exclusive groups
+parser_barcode_group = parser_barcode.add_mutually_exclusive_group()
+parser_barcode_group.add_argument(
     "-c", "--contain",
     help = "barcode string to search against the fastq, seperate by comma if multiple. e.g. 'AACCC,GTCCC,CAAA'",
-    required = True, type = str, default = None
+    required = False, type = str, default = None
+)
+parser_barcode_group.add_argument(
+    "-l", "--locate",
+    help = "barcode string to search against the fastq, seperate by comma if multiple. e.g. 'AACCC,GTCCC,CAAA'",
+    required = False, type = str, default = None
 )
 parser_barcode.add_argument(
+    "-p", "--position",
+    help = "return which matched location, default to 0 meaning that the first matched location, use -1 for that last matched location",
+    required = False, type = int, default = 0
+)
+
+parser_barcode.add_argument(
     "-e", "--error",
     help = "allowed mismatchs (including INDELs) when searching for barcode string",
     required = False, type = int, default = 1
 )
 parser_barcode.add_argument(
     "-rcb", "--rc_barcode", 
     help = "reverse complement the barcode before searching",
```

### Comparing `scutls-0.1.8/scutls/assets/genome_ensembl_107_54_54_54.json` & `scutls-0.2.0/scutls/assets/genome_ensembl_107_54_54_54.json`

 * *Files identical despite different names*

### Comparing `scutls-0.1.8/scutls/assets/genome_ensembl_release_all.txt` & `scutls-0.2.0/scutls/assets/genome_ensembl_release_all.txt`

 * *Files identical despite different names*

### Comparing `scutls-0.1.8/scutls/assets/genome_ucsc.json` & `scutls-0.2.0/scutls/assets/genome_ucsc.json`

 * *Files identical despite different names*

### Comparing `scutls-0.1.8/scutls/barcode.py` & `scutls-0.2.0/scutls/barcode.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,100 +1,126 @@
 import argparse
 import functools
 from multiprocessing import Pool
 from Bio import SeqIO, bgzf
 from Bio.Seq import Seq
-from .util import fastq_chunk_interval, fastq_contain_barcode
+from .util import fastq_chunk_interval, fastq_contain_barcode, get_search_pattern, fastq_locate_barcode
 import os
+import regex
 
-def barcode(input = None, output = None, output2 = None, contain = None, error = 1, rc_barcode = False, nproc = 1):
+def barcode(input = None, output = None, output2 = None, contain = None, locate = None, pos = 0, error = 1, rc_barcode = False, nproc = 1):
     """barcode subcommand
     Paramters
     ---------
 
     input : str
         output file name, auto detects .gz
     output : str
         output file name, auto detects .gz, contains fastq that contains specified barcode via contain
     contain: str
         barcode to detect, if multiple barcode, separate with comma: "AATTCCC,AGGGCCC,CCGGCG"
         # optional for "contain" sub-command:
         error: int
-            allowed nucleotide mismatches (can be INDELs) when aligning, default to 1. 
+            allowed nucleotide mismatches (can be INDELs) when aligning, default to 1
         nproc: int
-            number of parallel jobs, default to 1.
+            number of parallel jobs, default to 1
         rc_barcode: bool
-            take reverse complement of the barcode when aligning, default to False.
-
+            take reverse complement of the barcode when aligning, default to False
+    locate: str
+        barcode to detect its location in reads
+        # shared arguments with "contain": error, nproc, rc_barcode
+        pos: int
+            which matched position to return, default to 0 meaning the first, use -1 to indicate the last.
+        
     """
 
     args = list(locals().keys())
 
     local = locals()
     if all(bool(local[key]) is not True for key in args): 
         print("scutls fastq: warning: use 'scutls contain -h' for usage")
     # use True since args can be either None or False
     # arguments.py defines requirments of each argument
 
     # check if input fastq contains specified barcode:
     if contain:
         # prepare search pattern
-        if not "," in contain:
-            if rc_barcode:
-                contain = str(Seq(contain).reverse_complement())
-            barcode_pattern = "(" + contain + "){e<=" + str(error) + "}"
-        else:
-            barcode_pattern = ""
-            barcodes = contain.split(",")
-            for barcode in barcodes:
-                if rc_barcode:
-                    contain = str(Seq(contain).reverse_complement())
-                barcode_pattern += "(" + barcode + "){e<=" + str(error) + "}(.*?)"
-    
+        barcode_pattern = get_search_pattern(pattern = contain, error = error, rc_barcode = rc_barcode)
+
         # multiprocessing
-        print("Saving to " + output + " ...")
+        if not output == None:
+            print("Saving to " + output + " ...")
+        else:
+            print("Processing ...")
         intervals = fastq_chunk_interval(input, nproc = nproc)
         p = Pool(nproc)
         res = p.map_async(
             functools.partial(
                 fastq_contain_barcode,
                 fastq = input,
                 barcode_pattern = barcode_pattern),
                 intervals.values()).get()
         fastq_hit, fastq_non_hit = [], []
         
         for x in range(len(res)):
             fastq_hit = fastq_hit + [hit for hit in res[x][0]]
             fastq_non_hit = fastq_non_hit + [non_hit for non_hit in res[x][1]]
 
-        if not os.path.dirname(output) == "":
-            os.makedirs(os.path.dirname(output), exist_ok=True)
-        if output.endswith(".gz"):
-            with bgzf.BgzfWriter(output, "wb") as outgz:
-                SeqIO.write(sequences = fastq_hit, handle = outgz, format="fastq")
+        if not output == None:
+            if not os.path.dirname(output) == "":
+                os.makedirs(os.path.dirname(output), exist_ok=True)
+            if output.endswith(".gz"):
+                with bgzf.BgzfWriter(output, "wb") as outgz:
+                    SeqIO.write(sequences = fastq_hit, handle = outgz, format="fastq")
+            else:
+                SeqIO.write(fastq_hit, output, "fastq")
         else:
-            SeqIO.write(fastq_hit, output, "fastq")
+            for record in fastq_hit:
+                print(record.seq, [x.start() for x in regex.finditer(barcode_pattern, str(record.seq))])
         
         if not output2 == None:
             print("Saving to " + output2 + " ...")
             if not os.path.dirname(output2) == "":
                 os.makedirs(os.path.dirname(output2), exist_ok=True)
             if output2.endswith(".gz"):
                 with bgzf.BgzfWriter(output2, "wb") as outgz:
                     SeqIO.write(sequences = fastq_non_hit, handle = outgz, format="fastq")
             else:
                 SeqIO.write(fastq_non_hit, output2, "fastq")
         
         print("Done!")
 
+    # check if input fastq contains specified barcode
+    if locate:
+        # prepare search pattern
+        barcode_pattern = get_search_pattern(pattern = locate, error = error, rc_barcode = rc_barcode)
+
+        # multiprocessing
+        intervals = fastq_chunk_interval(input, nproc = nproc)
+        p = Pool(nproc)
+        res_list = p.map_async(
+            functools.partial(
+                fastq_locate_barcode,
+                fastq = input,
+                barcode_pattern = barcode_pattern,
+                pos = pos),
+                intervals.values()).get()
+        for res in res_list:
+            for res_items in res:
+                print(res_items[0], res_items[1], res_items[2])
+
+
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('--input',  '-i', type   = str)
     parser.add_argument('--output', '-o', type   = str)
     parser.add_argument('--output2', '-o2', type = str)
-    parser.add_argument('--contain', '-c', action = str)
+    parser.add_argument('--contain', '-c', type = str)
+    parser.add_argument('--locate', '-l', type = str)
+    parser.add_argument('--position', '-p', type = int)
+    
     parser.add_argument('--error',   '-e', type   = int)
     parser.add_argument('--rc_barcode', '-rcb', default = False)
     parser.add_argument('--num_processor', '-nproc', default = 1)
     
 if __name__ == "__main__":
     main()
```

### Comparing `scutls-0.1.8/scutls/cli.py` & `scutls-0.2.0/scutls/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,11 +26,13 @@
 
 def run_barcode(args):
     barcode.barcode(
     input  = args.input,
     output = args.output,
     output2 = args.output2,
     contain = args.contain,
+    locate = args.locate,
+    pos = args.position,
     error   = args.error,
     rc_barcode = args.rc_barcode,
     nproc = args.num_processor # must use full name
     )
```

### Comparing `scutls-0.1.8/scutls/download.py` & `scutls-0.2.0/scutls/download.py`

 * *Files identical despite different names*

### Comparing `scutls-0.1.8/scutls/fastq.py` & `scutls-0.2.0/scutls/fastq.py`

 * *Files identical despite different names*

### Comparing `scutls-0.1.8/scutls/util.py` & `scutls-0.2.0/scutls/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import importlib_resources
 import json
 import gzip
 from mimetypes import guess_type
 from functools import partial
 import math
 from Bio import SeqIO
+from Bio.Seq import Seq
 import regex
 
 # helper function to perform sort
 def num_sort(test_string):
     return list(map(int, re.findall(r'\d+', test_string)))[0]
 
 # helper for extracting links to releases:
@@ -178,24 +179,59 @@
 def fastq_chunk_interval(fastq, nproc = 1):
     with _open(fastq) as f:
         n1 = sum(1 for record in SeqIO.parse(f, "fastq"))
     chunk_size = math.ceil(n1 / nproc)
     chunk_size = closest_number(chunk_size, 4)
     intervals = list(chunks(range(0, n1), chunk_size))
     intervals = {i: intervals[i] for i in range(0, len(intervals))}
-    
     return(intervals)
 
 # obtain fastq that contains specified barcode
 def fastq_contain_barcode(interval, fastq, barcode_pattern):
     fastq_hit, fastq_non_hit = [], []
     with _open(fastq) as f:
         for i, record in enumerate(SeqIO.parse(f, "fastq")):
             if i in interval:
                 if regex.search(barcode_pattern, str(record.seq)):
                     fastq_hit.append(record)
                 else:
                     fastq_non_hit.append(record)
     return([fastq_hit, fastq_non_hit])
 
+# obtain search pattern given string pattern and allowed mismatches (error)
+def get_search_pattern(pattern, error, rc_barcode):
+    if not "," in pattern:
+        if rc_barcode:
+            pattern = str(Seq(pattern).reverse_complement())
+        barcode_pattern = "(" + pattern + "){e<=" + str(error) + "}"
+    else:
+        barcode_pattern = ""
+        barcodes = pattern.split(",")
+        for barcode in barcodes:
+            if rc_barcode:
+                pattern = str(Seq(pattern).reverse_complement())
+            barcode_pattern += "(" + barcode + "){e<=" + str(error) + "}(.*?)"
+    return(barcode_pattern)
+
+# obtain fastq coordinates for specified barcode
+def fastq_locate_barcode(interval, fastq, barcode_pattern, pos = 0):
+    """
+    pos: which match to return: use 0 for the first match, use -1 for the last match.
+    The return value will be: record.id match_location_0_based len(record.seq)s
+    
+    """
+    res = []
+    with _open(fastq) as f:
+        for i, record in enumerate(SeqIO.parse(f, "fastq")):
+            if i in interval:
+                matches = regex.finditer(barcode_pattern, str(record.seq))
+                # tem = [match for match in matches]
+                pos_start = [match.start() for match in matches]
+        
+                if not len(pos_start) == 0:
+                    res.append([record.id, pos_start[pos], len(record.seq)])
+                else:
+                    res.append([record.id, "NA", len(record.seq)])
+    return(res)
+
 if __name__ == "__main__":
     update_ensembl_release()
```

### Comparing `scutls-0.1.8/setup.py` & `scutls-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'wget>=3.2,<4.0']
 
 entry_points = \
 {'console_scripts': ['scutls = scutls.arguments:main']}
 
 setup_kwargs = {
     'name': 'scutls',
-    'version': '0.1.8',
+    'version': '0.2.0',
     'description': 'Single-cell data processing utility tools',
     'long_description': 'None',
     'author': 'Kai Hu',
     'author_email': 'kai.hu@umassmed.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `scutls-0.1.8/PKG-INFO` & `scutls-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scutls
-Version: 0.1.8
+Version: 0.2.0
 Summary: Single-cell data processing utility tools
 Author: Kai Hu
 Author-email: kai.hu@umassmed.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

