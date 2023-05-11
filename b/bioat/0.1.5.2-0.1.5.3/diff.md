# Comparing `tmp/bioat-0.1.5.2.tar.gz` & `tmp/bioat-0.1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioat-0.1.5.2.tar", max compression
+gzip compressed data, was "bioat-0.1.5.3.tar", max compression
```

## Comparing `bioat-0.1.5.2.tar` & `bioat-0.1.5.3.tar`

### file list

```diff
@@ -1,23 +1,28 @@
--rw-r--r--   0        0        0     1080 2022-10-12 10:28:48.000000 bioat-0.1.5.2/LICENSE
--rw-r--r--   0        0        0      689 2023-04-10 17:11:40.000000 bioat-0.1.5.2/README.md
--rw-r--r--   0        0        0     1064 2023-04-08 13:49:15.966541 bioat-0.1.5.2/pyproject.toml
--rw-r--r--   0        0        0      471 2023-04-01 11:15:49.201131 bioat-0.1.5.2/src/bioat/__init__.py
--rw-r--r--   0        0        0      508 2023-04-02 12:41:49.000000 bioat-0.1.5.2/src/bioat/about.py
--rw-r--r--   0        0        0    13631 2023-04-10 17:00:33.000000 bioat-0.1.5.2/src/bioat/bam.py
--rw-r--r--   0        0        0     1413 2023-04-06 11:55:25.000000 bioat-0.1.5.2/src/bioat/cli.py
--rw-r--r--   0        0        0       63 2022-10-12 10:34:44.000000 bioat-0.1.5.2/src/bioat/exceptions.py
--rw-r--r--   0        0        0    11016 2023-03-13 04:00:08.114588 bioat-0.1.5.2/src/bioat/fastx.py
--rw-r--r--   0        0        0      818 2023-03-13 04:16:15.365909 bioat-0.1.5.2/src/bioat/genome.py
--rw-r--r--   0        0        0     5895 2023-04-10 17:00:56.000000 bioat-0.1.5.2/src/bioat/hic.py
--rw-r--r--   0        0        0        0 2023-04-01 12:21:31.028419 bioat-0.1.5.2/src/bioat/lib/__init__.py
--rw-r--r--   0        0        0      854 2023-04-08 13:49:32.058220 bioat-0.1.5.2/src/bioat/lib/_dev_tools.py
--rw-r--r--   0        0        0     5550 2023-04-11 16:07:38.982348 bioat-0.1.5.2/src/bioat/lib/libalignment.py
--rw-r--r--   0        0        0     2719 2023-04-11 14:34:02.889267 bioat-0.1.5.2/src/bioat/lib/libcolor.py
--rw-r--r--   0        0        0     7042 2023-04-11 11:27:23.563291 bioat-0.1.5.2/src/bioat/lib/libcrispr.py
--rw-r--r--   0        0        0     1442 2023-04-10 17:17:40.000000 bioat-0.1.5.2/src/bioat/logger.py
--rw-r--r--   0        0        0      668 2023-04-07 16:11:22.000000 bioat-0.1.5.2/src/bioat/mgi.py
--rw-r--r--   0        0        0     5629 2023-03-12 14:27:33.279607 bioat-0.1.5.2/src/bioat/system.py
--rw-r--r--   0        0        0     3245 2023-04-07 08:00:16.234706 bioat-0.1.5.2/src/bioat/table.py
--rw-r--r--   0        0        0    27616 2023-04-11 16:22:40.513555 bioat-0.1.5.2/src/bioat/targeted_deep_sequencing.py
--rw-r--r--   0        0        0      384 2023-04-10 17:03:51.000000 bioat-0.1.5.2/src/bioat/version.py
--rw-r--r--   0        0        0     1723 1970-01-01 00:00:00.000000 bioat-0.1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2022-10-12 10:28:48.000000 bioat-0.1.5.3/LICENSE
+-rw-r--r--   0        0        0      852 2023-05-09 16:09:06.000000 bioat-0.1.5.3/README.md
+-rw-r--r--   0        0        0     1112 2023-05-11 14:44:30.818057 bioat-0.1.5.3/pyproject.toml
+-rw-r--r--   0        0        0      471 2023-04-01 11:15:49.201131 bioat-0.1.5.3/src/bioat/__init__.py
+-rw-r--r--   0        0        0      508 2023-04-02 12:41:49.000000 bioat-0.1.5.3/src/bioat/about.py
+-rw-r--r--   0        0        0    13627 2023-05-08 15:34:47.326510 bioat-0.1.5.3/src/bioat/bam.py
+-rw-r--r--   0        0        0     1452 2023-05-11 14:31:32.618474 bioat-0.1.5.3/src/bioat/cli.py
+-rw-r--r--   0        0        0    14545 2023-04-19 14:58:31.765837 bioat-0.1.5.3/src/bioat/detect_seq.py
+-rw-r--r--   0        0        0       63 2022-10-12 10:34:44.000000 bioat-0.1.5.3/src/bioat/exceptions.py
+-rw-r--r--   0        0        0    11016 2023-03-13 04:00:08.114588 bioat-0.1.5.3/src/bioat/fastx.py
+-rw-r--r--   0        0        0      818 2023-03-13 04:16:15.365909 bioat-0.1.5.3/src/bioat/genome.py
+-rw-r--r--   0        0        0     5895 2023-04-10 17:00:56.000000 bioat-0.1.5.3/src/bioat/hic.py
+-rw-r--r--   0        0        0        0 2023-04-01 12:21:31.028419 bioat-0.1.5.3/src/bioat/lib/__init__.py
+-rw-r--r--   0        0        0      854 2023-04-08 13:49:32.058220 bioat-0.1.5.3/src/bioat/lib/_dev_tools.py
+-rw-r--r--   0        0        0     6274 2023-04-13 16:27:56.000000 bioat-0.1.5.3/src/bioat/lib/libalignment.py
+-rwxr-xr-x   0        0        0    77022 2023-05-11 14:29:19.339453 bioat-0.1.5.3/src/bioat/lib/libcircos.py
+-rw-r--r--   0        0        0     2719 2023-04-11 14:34:02.889267 bioat-0.1.5.3/src/bioat/lib/libcolor.py
+-rw-r--r--   0        0        0     6543 2023-04-13 15:00:50.900126 bioat-0.1.5.3/src/bioat/lib/libcrispr.py
+-rw-r--r--   0        0        0   155206 2023-04-19 14:58:47.513136 bioat-0.1.5.3/src/bioat/lib/libdetect_seq.py
+-rw-r--r--   0        0        0     1720 2023-04-25 18:24:40.767945 bioat-0.1.5.3/src/bioat/lib/libplot.py
+-rw-r--r--   0        0        0      509 2023-05-11 14:37:34.152762 bioat-0.1.5.3/src/bioat/lib/libsnakemake.py
+-rw-r--r--   0        0        0     1604 2023-04-17 08:05:06.992591 bioat-0.1.5.3/src/bioat/logger.py
+-rw-r--r--   0        0        0      668 2023-04-07 16:11:22.000000 bioat-0.1.5.3/src/bioat/mgi.py
+-rw-r--r--   0        0        0     5745 2023-05-07 15:13:15.000000 bioat-0.1.5.3/src/bioat/system.py
+-rw-r--r--   0        0        0     3245 2023-04-07 08:00:16.234706 bioat-0.1.5.3/src/bioat/table.py
+-rw-r--r--   0        0        0    27399 2023-04-13 16:49:11.000000 bioat-0.1.5.3/src/bioat/targeted_deep_sequencing.py
+-rw-r--r--   0        0        0      384 2023-04-11 17:08:03.000000 bioat-0.1.5.3/src/bioat/version.py
+-rw-r--r--   0        0        0     2018 1970-01-01 00:00:00.000000 bioat-0.1.5.3/PKG-INFO
```

### Comparing `bioat-0.1.5.2/LICENSE` & `bioat-0.1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.2/pyproject.toml` & `bioat-0.1.5.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [tool.poetry]
 name = "bioat"
-version = "0.1.5.2"
+version = "0.1.5.3"
 description = "Bioinformatic toolkit with python (It's still under development!)"
 license = "MIT"
 authors = ["Herman Zhao <hermanzhaozzzz@gmail.com>"]
 repository = "https://github.com/hermanzhaozzzz/BioinformaticAnalysisTools"
 homepage = "https://github.com/hermanzhaozzzz/BioinformaticAnalysisTools"
 # README file(s) are used as the package description
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 # Compatible Python versions
-python = "^3.9.6"
+python = ">=3.8.0,<3.11"
 pandas = "^1.5.3"
 numpy = "^1.24.1"
 tqdm = "^4.64.1"
 fire = "^0.5.0"
 cython = "^0.29.33"
 pysam = "^0.20.0"
-biopython = "^1.81"
+biopython = "^1.80"
 pandarallel = "^1.6.4"
 matplotlib = "^3.7.1"
 tabulate = "^0.9.0"
+scipy = "^1.8.0"
+statsmodels = "^0.13.5"
 
 [tool.poetry.scripts]
 bioat = "bioat.cli:main"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 pytest-cov = "^3.0"
```

### Comparing `bioat-0.1.5.2/src/bioat/bam.py` & `bioat-0.1.5.3/src/bioat/bam.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         pass
 
     def mpileup_to_table(
             self,
             mpileup: str,
             output: str = sys.stdout,
             threads: int = os.cpu_count() - 1,
-            mutation_number_threshold: int = None,
+            mutation_number_threshold: int = 0,
             temp_dir: str = f"/tmp/bioat_{''.join(random.sample(string.ascii_letters + string.digits, 16))}",
             remove_temp: bool = True,
             log_level: str = 'INFO'
     ):
         """Convert mpileup file to info file.
 
         :param mpileup: samtools mpileup format file
@@ -36,14 +36,15 @@
         :param log_level: 'CRITICAL', 'ERROR', 'WARNING', 'INFO', 'DEBUG', 'NOTSET'
         """
         set_logging_level(level=log_level)
         # set logger
         lib_name = __name__
         function_name = sys._getframe().f_code.co_name
         logger = logging.getLogger(f'{lib_name}.{function_name} ==> ')
+
         def _temp_split_bam(mpileup, threads, temp_dir):
             # creat temp file name and open file
             logger.debug("Making temp files...")
 
             input_file_basename = os.path.basename(mpileup)
 
             temp_filename_list = []
@@ -198,19 +199,19 @@
             so = bam_in.header['HD']['SO']
         except KeyError:
             so = None
 
         if so:
             if so != "queryname":
                 logger.fatal(f"the input BAM|SAM must be sorted by name and has header [SO:queryname]!\n"
-                              f"your header: [SO:{so}]\n")
+                             f"your header: [SO:{so}]\n")
                 exit(1)
         else:
             logger.warning(f"the input BAM|SAM must be sorted by name and has header [SO:queryname]!\n"
-                            "your bam file does not have a header\n")
+                           "your bam file does not have a header\n")
 
         write_mode = 'wb' if output_fmt.upper() == "BAM" else 'w'
         bam_out = pysam.AlignmentFile(output, write_mode, template=bam_in)
 
         # Iterate through reads.
         read1, read2 = None, None
```

### Comparing `bioat-0.1.5.2/src/bioat/cli.py` & `bioat-0.1.5.3/src/bioat/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,22 +26,23 @@
         """Print information about <bioat>.
         """
         return about
 
     def list(self):
         """Print commands and subcommands.
         """
+        out = ""
         for att in dir(self):
             if not att.startswith('_'):
-                print(f'{att}')
+                out += f'{att}\n'
 
                 for sub_att in dir(getattr(self, att)):
                     if not sub_att.startswith('_'):
-                        print(f'  ├── {sub_att}')
-
+                        out += f'  ├── {sub_att}\n'
+        return out
     @classmethod
     def version(self):
         """Print version information.
         """
         return __version__
```

### Comparing `bioat-0.1.5.2/src/bioat/fastx.py` & `bioat-0.1.5.3/src/bioat/fastx.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.2/src/bioat/genome.py` & `bioat-0.1.5.3/src/bioat/genome.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.2/src/bioat/hic.py` & `bioat-0.1.5.3/src/bioat/hic.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.2/src/bioat/lib/_dev_tools.py` & `bioat-0.1.5.3/src/bioat/lib/_dev_tools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.2/src/bioat/lib/libalignment.py` & `bioat-0.1.5.3/src/bioat/lib/libalignment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,36 @@
-from Bio.Align import Alignment
+from Bio.Align import Alignment, PairwiseAligner
 import sys
 import logging
 
 
+def instantiate_pairwise_aligner(
+        scoring_match,
+        penalty_mismatch,
+        penalty_gap_open,
+        penalty_gap_extension,
+        # penalty_query_left_gap
+        mode='global'
+):
+    # set logger
+    lib_name = __name__
+    function_name = sys._getframe().f_code.co_name
+    logger = logging.getLogger(f'{lib_name}.{function_name} ==> ')
+
+    aligner = PairwiseAligner()
+    aligner.match = scoring_match
+    aligner.mismatch = penalty_mismatch
+    aligner.open_gap_score = penalty_gap_open
+    aligner.extend_gap_score = penalty_gap_extension
+    aligner.query_left_gap_score = 0
+    aligner.query_right_gap_score = 0
+    aligner.mode = mode
+    logger.info(aligner)
+    return aligner
+
 def get_aligned_seq(alignment: Alignment, reverse: bool = False) -> dict:
     """Get_aligned_seq.
 
     :param alignment: Bio.Align.Alignment object
     :param reverse: return reversed seq info or not
     :return: dict, like this:
          {
```

### Comparing `bioat-0.1.5.2/src/bioat/lib/libcolor.py` & `bioat-0.1.5.3/src/bioat/lib/libcolor.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.2/src/bioat/lib/libcrispr.py` & `bioat-0.1.5.3/src/bioat/lib/libcrispr.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,220 +1,177 @@
 from __future__ import absolute_import
 import logging
 import sys
+
+import pandas as pd
 from Bio.Seq import Seq
 from Bio.Align import PairwiseAligner
 from bioat.lib.libalignment import get_alignment_info
 
 """TARGET_REGIONS_LIB.
 
 bioat targeted_deep_sequencing region_heatmap test_sorted.mpileup.info.tsv test.pdf --get_built_in_target_region
 
 INFO:root:You can use <key> in built-in <target_regions> to represent your target_region:
         <key>   <target_region>
-        EMX1    GAGTCCGAGCAGAAGAAGAA^GGG^
-        HEK3    GGCCCAGACTGAGCACGTGA^TGG^
-        HEK4    GGCACTGCGGCTGGAGGTGG^GGG^
+        EMX1    GAGTCCGAGCAGAAGAAGAA^NGG^
+        HEK3    GGCCCAGACTGAGCACGTGA^NGG^
+        HEK4    GGCACTGCGGCTGGAGGTGG^NGG^
         ...
 """
 TARGET_SEQ_LIB = {
-    "EMX1": "GAGTCCGAGCAGAAGAAGAA^GGG^",
-    "HEK3": "GGCCCAGACTGAGCACGTGA^TGG^",
-    "HEK4": "GGCACTGCGGCTGGAGGTGG^GGG^",
-    "RNF2": "GTCATCTTAGTCATTACCTG^AGG^",
-    "VEGFA": "GACCCCCTCCACCCCGCCTC^CGG^",
+    "EMX1": "GAGTCCGAGCAGAAGAAGAA^NGG^",
+    "HEK3": "GGCCCAGACTGAGCACGTGA^NGG^",
+    "HEK4": "GGCACTGCGGCTGGAGGTGG^NGG^",
+    "RNF2": "GTCATCTTAGTCATTACCTG^NGG^",
+    "VEGFA": "GACCCCCTCCACCCCGCCTC^NGG^",
     "CDKN2A": "^TTTA^GCCCCAATAATCCCCACATGTCA",
     "DYRK1A": "^TTTA^GAAGCACATCAAGGACATTCTAA",
     "ND4": "TGCTAGTAACCACGTTCTCCTGATCAAATATCACTCTCCTACTTACAGGA",
     "ND5.1": "TAGCATTAGCAGGAATACCTTTCCTCACAGGTTTCTACTCCAAAGA",
     "ND6": "TGACCCCCATGCCTCAGGATACTCCTCAATAGCCATCG",
 }
 
 
-def find_seq_PAM_index(query_seq):
-    """Find seq PAM index.
-
-    :param query_seq: e.g. query_seq = "AAAGAGAG"
-    :return: index list = [1,3,5], which means search NAG, NGG at the same time
-    """
-    pam_index_list = []
-
-    for index, base in enumerate(query_seq[:-2]):
-        if query_seq[index + 1:index + 3] == "AG":
-            pam_index_list.append((index, "NAG"))
-
-        elif query_seq[index + 1:index + 3] == "GG":
-            pam_index_list.append((index, "NGG"))
-
-    return (pam_index_list)
-
-
-def sign_value(x):
-    """
-    HELP
-        sign function
-    """
-    if x < 0:
-        return (-1)
-    elif x == 0:
-        return (0)
-    else:
-        return (1)
-
-
-def cmp_align_list(align_a, align_b):
+def cmp_align_list(aln_a: dict, aln_b: dict):
     """
     INPUT
         like [17, 3, 0, 73.0, 1, 22 'AAGAAGAAGACGAGTCTGCA', '||||||||||||||X|||XX', 'AAGAAGAAGACGAGCCTGAG']
-
+        {
+            'match_count': 26,
+            'mismatch_count': 3,
+            'gap_count': 4,
+            'aln_score': 96.0,
+            'ref_aln_start': 0,
+            'ref_aln_end': 32,
+            'alignment': {
+                'reference_seq': 'GGCACTGCGGCTGGAAAAAAAAAAAAAAA--GT',
+                'aln_info':      '--..|.|||||||||||||||||||||||--||',
+                'target_seq':    '--GGCAGCGGCTGGAAAAAAAAAAAAAAAAGGT'
+            }
+        }
     HELP
         compare function for align_list
     """
-    align_alphabet = {"-": 0, "X": 1, "|": 2}
-    sort_index_list = [3, 2, 1, 0]
-    sort_rev_state_list = [True, False, False, True]
 
-    for order_index, align_index in enumerate(sort_index_list):
-        if (align_a[align_index] - align_b[align_index]) == 0:
-            continue
+    # sort reason score -> gap -> mismatch -> match
+    def sign_value(x):
+        """
+        HELP
+            sign function
+        """
+        if x > 0:
+            return 1
+        elif x < 0:
+            return -1
         else:
-            if sort_rev_state_list[order_index]:
-                return (-1 *
-                        sign_value(align_a[align_index] - align_b[align_index]))
-            else:
-                return (
-                    sign_value(
-                        align_a[align_index] -
-                        align_b[align_index]))
-
-    for index, char_a in enumerate(align_a[7]):
-        if index <= (len(align_b[7]) - 1):
-            value_a = align_alphabet[char_a]
-            value_b = align_alphabet[align_b[7][index]]
-
-            if value_a > value_b:
-                return 1
-            elif value_a < value_b:
-                return -1
+            return 0
 
-    return 0
-
-
-def run_sgRNA_alignment(align_ref_seq, align_sgRNA, aligner, extend_len=3):
-    """
-    INPUT
-        <ref_seq>
-
-        <align_sgRNA>
-            sgRNA seq without PAM
-
-        <possible_sgRNA_region>
-
-    RETURN
-        <final_align_res_list>
-    """
-    align_sgRNA_rev = align_sgRNA[::-1]
-
-    # find all PAM
-    PAM_info_list = find_seq_PAM_index(align_ref_seq)
-    if len(PAM_info_list) == 0:
-        return ([])
-
-    # forward alignment
-    final_align_res_list = []
-
-    for PAM_start_idx, PAM_type in PAM_info_list:
+    align_alphabet_score = {"-": 0, ".": 1, "|": 2}
+    sort_keys = ['alignment_score', 'gap_count', 'mismatch_count', 'match_count']
+    sort_rev_state_list = [True, False, False, True]
 
-        # filter 5' end PAM
-        if (PAM_start_idx - extend_len) < len(align_sgRNA):
+    for idx, key in enumerate(sort_keys):
+        if aln_a[key] - aln_b[key] == 0:
             continue
-
-        # select PAM and sgRNA in the possible region
-        region_seq_start = PAM_start_idx - len(align_sgRNA) - extend_len
-        region_seq_end = PAM_start_idx + 3
-
-        # alignment part
-        region_seq = align_ref_seq[region_seq_start: PAM_start_idx]
-        alignments = aligner.align(region_seq[::-1], align_sgRNA_rev)
-
-        # parse alignment
-        # if contain multiple alignment result with the same score, keep the best one;
-        # sort reason score -> gap -> mismatch -> match
-        align_res_list = []
-        for alignment in alignments:
-            align_analysis_res = get_alignment_info(alignment, reverse=True)
-            align_info_list = [x[::-1] for x in str(alignment).strip().split("\n")]
-            align_analysis_res += align_info_list
-            align_analysis_res += [PAM_start_idx, PAM_type]
-            align_res_list.append(align_analysis_res)
-
-        if len(align_res_list) == 1:
-            final_align_res_list.append(align_res_list[0])
-
         else:
-            align_res_list.sort(cmp=cmp_align_list)
-            final_align_res_list.append(align_res_list[0])
+            if sort_rev_state_list[idx]:
+                return -1 * sign_value(aln_a[key] - aln_b[key])
+            else:
+                return sign_value(aln_a[key] - aln_b[key])
 
-    # sort final alignment
-    final_align_res_list.sort(cmp=cmp_align_list)
+    aln_info_a = aln_a['alignment']['aln_info']
+    aln_info_b = aln_b['alignment']['aln_info']
 
-    return (final_align_res_list)
+    for idx, char_a in enumerate(aln_info_a):
+        if idx <= (len(aln_info_b) - 1):
+            value_a = align_alphabet_score[char_a]
+            value_b = align_alphabet_score[aln_info_a[idx]]
+            return sign_value(value_a - value_b)
+        else:
+            pass
 
 
-def run_no_PAM_sgRNA_alignment_no_chop(
+def run_target_seq_align(
         ref_seq: Seq,
         target_seq: Seq,
-        aligner: PairwiseAligner
+        aligner: PairwiseAligner,
+        PAM: dict = None
 ) -> list:
     """global alignment for target_seq
 
     :param ref_seq: a Seq object from BioPython, reference sequence for the targeted deep sequencing
     :param target_seq: a Seq object from BioPython, target region sequence for the editing window, usually the sgRNA
         sequencing without PAM
     :param aligner: an obj from BioPython pairwise alignment
+    :param PAM: a dict like {'PAM': 'AGG', 'position': 20, 'weight': 1.0},
+        position is the insertion site of target_seq,
+        weight is the priority, PAM alignment score will multiply by this weight.
     :return: a list: list contains some dict, each one is an alignment result.
     [
         {
             'match_count': 26,
             'mismatch_count': 3,
             'gap_count': 4,
-            'alignment_score': 96.0,
-            'ref_align_start_index': 0,
-            'ref_align_end_index': 32,
+            'aln_score': 96.0,
+            'ref_aln_start': 0,
+            'ref_aln_end': 32,
             'alignment': {
-                'aligned_reference_seq': 'GGCACTGCGGCTGGAAAAAAAAAAAAAAA--GT',
-                'aligned_seq_info':      '--..|.|||||||||||||||||||||||--||',
-                'aligned_target_seq':    '--GGCAGCGGCTGGAAAAAAAAAAAAAAAAGGT'
-            },
-            'PAM_start_index': None,
-            'PAM_type': None
+                'reference_seq': 'GGCACTGCGGCTGGAAAAAAAAAAAAAAA--GT',
+                'aln_info':      '--..|.|||||||||||||||||||||||--||',
+                'target_seq':    '--GGCAGCGGCTGGAAAAAAAAAAAAAAAAGGT'
+            }
         },
         ...
     ]
 
     """
     # set logger
     lib_name = __name__
     function_name = sys._getframe().f_code.co_name
     logger = logging.getLogger(f'{lib_name}.{function_name} ==> ')
 
+    if PAM:
+        # considering PAM
+        # DNA info https://www.bioinformatics.org/sms/iupac.html
+        alignments_pam = aligner.align(ref_seq, Seq(PAM['PAM']))
+        # use pam to find aim sequence on ref and then use target_seq to align them and give it a higher priority
+        dt_PAMs = {}
+
+        for idx, alignment in enumerate(alignments_pam):
+            alignment_analysis_result = get_alignment_info(alignment, reverse=False)
+            logger.debug(f'alignment_analysis_result for PAM:\n{alignment_analysis_result}')
+            ref_aln_start = alignment_analysis_result['ref_aln_start']
+            ref_aln_end = alignment_analysis_result['ref_aln_end']
+            aln_score = alignment_analysis_result['aln_score'] * PAM['weight']
+            dt_PAMs[f'{ref_aln_start}_{ref_aln_end}'] = dict(aln_score=aln_score * PAM['weight'])
+
+        logger.debug(f'find PAMs on reference: {dt_PAMs}')
+
+        # add PAM left or right or any position
+        target_seq = target_seq[:PAM['position']] + Seq(PAM['PAM']) + target_seq[PAM['position']:]
+        logger.info(f'find PAM on target_seq, target_seq is updated to: {str(target_seq)}')
+
     # alignment part
     alignments = aligner.align(ref_seq, target_seq)
     # parse alignment
-    # if contain multiple alignment result with the same score, keep the best one;
-    # sort reason score -> gap -> mismatch -> match
     alignment_results = []
 
     for alignment in alignments:
-        # logging.debug(type(align))  # Bio.Align.Alignment object
         alignment_analysis_result = get_alignment_info(alignment, reverse=False)
         logger.debug(f'alignment_analysis_result:\n{alignment_analysis_result}')
         alignment_results.append(alignment_analysis_result)
 
-        if len(alignment_results) == 1:
-            logger.debug(f'find 1 alignment result:\n{alignment_results}')
-        return alignment_results
-
+    if len(alignment_results) == 1:
+        logger.debug(f'find 1 alignment result:\n{alignment_results}')
+        return alignment_results[0]
     else:
-        alignment_results.sort(cmp=cmp_align_list)
-        logger.debug(f'find more than 1 alignment results:\n{alignment_results}')
-        return alignment_results
+        logger.debug(f'find {len(alignment_results)} alignment results:\n{alignment_results}')
+        df = pd.DataFrame(alignment_results)
+        # if contain multiple alignment result with the same score, keep the best one;
+        # sort reason score -> gap -> mismatch -> match
+        df.sort_values(
+            by=['aln_score', 'gap_count', 'mismatch_count', 'match_count'],
+            ascending=[False, True, True, False],
+            inplace=True
+        )
+        return df.iloc[0, :].to_dict()
```

### Comparing `bioat-0.1.5.2/src/bioat/mgi.py` & `bioat-0.1.5.3/src/bioat/mgi.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.2/src/bioat/system.py` & `bioat-0.1.5.3/src/bioat/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-# import os
-# import time
-#
-#
+from __future__ import absolute_import
+# from bioat.api.internet_speed import main as speedtest
+
+
 class System():
     def __init__(self):
+        # self.test_internet_speed = speedtest()
         pass
-#
+
 #     def __convert_size(self, size, mode='b') -> float:
 #         """将单位为Byte的数字转为其它单位
 #
 #         :param size: int, 单位为Byte的数字
 #         :param mode: str, 单位，b、k、m、g、t或者B、K、M、G、T
 #         :return:
 #         """
```

### Comparing `bioat-0.1.5.2/src/bioat/table.py` & `bioat-0.1.5.3/src/bioat/table.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.2/src/bioat/targeted_deep_sequencing.py` & `bioat-0.1.5.3/src/bioat/targeted_deep_sequencing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,24 @@
+from __future__ import absolute_import
 from bioat.logger import set_logging_level
-from bioat.lib.libcrispr import (
-    TARGET_SEQ_LIB,
-    run_no_PAM_sgRNA_alignment_no_chop,
-    run_sgRNA_alignment
-)
-from bioat.lib.libcolor import (
-    convert_hex_to_rgb,
-    convert_rgb_to_hex,
-    map_color,
-    make_color_list
-)
-
-from Bio.Align import PairwiseAligner
+from bioat.lib.libcrispr import TARGET_SEQ_LIB, run_target_seq_align
+from bioat.lib.libcolor import map_color, make_color_list
+from bioat.lib.libalignment import instantiate_pairwise_aligner
 from Bio.Seq import Seq
-
+from tabulate import tabulate
 from matplotlib.collections import PatchCollection
 from matplotlib.patches import Rectangle
 from matplotlib import pyplot as plt
-from tabulate import tabulate
+import matplotlib
 import numpy as np
 import pandas as pd
-import matplotlib
+
 import logging
 import sys
 
-matplotlib.use('Agg')
-np.set_printoptions(suppress=True)
-
 
 class TargetedDeepSequencing:
     def __init__(self):
         pass
 
     def region_heatmap(
             self,
@@ -48,14 +36,15 @@
             min_color: tuple = (250, 239, 230),
             max_color: tuple = (154, 104, 57),
             min_ratio: float = 0.001,
             max_ratio: float = 0.99,
             region_extend_length: int = 25,
             local_alignment_scoring_matrix: tuple = (5, -4, -24, -8),
             local_alignment_min_score: int = 15,
+            PAM_priority_weight: float = 1.0,
             get_built_in_target_seq: bool = False,
             log_level: str = 'INFO'
     ):
         """Plot region mutation info using table generated by `bioat bam mpileup_to_table`.
 
         :param input_table: Path of table generated by `bioat bam mpileup_to_table`.
                 This table should contain base mutation information from a short genome region (no more than 1k nt).
@@ -80,14 +69,16 @@
         :param max_color: max color to plot heatmap with RGB format
         :param min_ratio: mutation ratio of box lower than min_ratio will show as white
         :param max_ratio: mutation ratio of box higher than min_ratio will show as ??
         :param region_extend_length: expand how many bps for the two side of this region
         :param local_alignment_scoring_matrix: set <align_match_score>  <align_mismatch_score>
                                                 <align_gap_open_score> <align_gap_extension_score>
         :param local_alignment_min_score: If alignment score lower than this, consider as no appropriate alignment
+        :param PAM_priority_weight: PAM alignment score will multiply by this weight.
+
         :param get_built_in_target_seq: specify to True to return built-in target_seq sequence.
         :param log_level: 'CRITICAL', 'ERROR', 'WARNING', 'INFO', 'DEBUG', 'NOTSET'
 
         --- demo ---\n
         samtools mpileup test_sorted.bam --reference HK4-AOut-1.ref.upper.fa | gzip > test_sorted.mpileup.gz\n
         bioat bam mpileup_to_table test_sorted.mpileup.gz > test_sorted.mpileup.info.tsv\n
         bioat targeted_deep_sequencing region_heatmap \
@@ -123,25 +114,15 @@
             else:
                 logger.error("<target_seq> should be set as:"
                              "DNA sequence / <key> in <get_built_in_target_seq> / None,"
                              f"but your <target_seq> is {target_seq}")
                 exit(1)
 
         # set alignment
-        align_match, align_mismatch, align_gap_open, align_gap_extension = local_alignment_scoring_matrix
-
-        aligner = PairwiseAligner()
-        aligner.match = align_match
-        aligner.mismatch = align_mismatch
-        aligner.open_gap_score = align_gap_open
-        aligner.extend_gap_score = align_gap_extension
-        aligner.query_left_gap_score = 0
-        aligner.query_right_gap_score = 0
-        aligner.mode = "global"
-        logger.info(aligner)
+        aligner = instantiate_pairwise_aligner(*local_alignment_scoring_matrix)
 
         # load mpileup.info.tsv
         if input_table_header:
             df_bases = pd.read_csv(input_table, sep="\t")
         else:
             df_bases = pd.read_csv(input_table, sep="\t", header=None)
 
@@ -159,54 +140,61 @@
         logger.debug(f'Seq object for ref_seq:\n{ref_seq}')
         ref_seq_rc = ref_seq.reverse_complement()
         logger.debug(f'Seq object for ref_seq_rc (reverse_complement):\n{ref_seq_rc}')
 
         # target_seq
         if target_seq is None:
             target_seq = ref_seq
-            PAM_seq = None
+            PAM = None
         elif '^' in target_seq:
             if target_seq.find('^') == 0:
-                _, PAM_seq, target_seq = target_seq.strip().split('^')
+                _, PAM, target_seq = target_seq.strip().split('^')
                 target_seq = Seq(target_seq.upper())
-                PAM_seq = 'left_' + PAM_seq
+                PAM = {'PAM': PAM, 'position': 0, 'weight': PAM_priority_weight}
             else:
-                target_seq, PAM_seq, _ = target_seq.strip().split('^')
+                target_seq, PAM, _ = target_seq.strip().split('^')
                 target_seq = Seq(target_seq.upper())
-                PAM_seq = 'right_' + PAM_seq
+                PAM = {'PAM': PAM, 'position': len(target_seq), 'weight': PAM_priority_weight}
         else:
             logger.debug(f'no PAM sequence is defined from target_seq = {target_seq}')
             target_seq = Seq(target_seq)
-            PAM_seq = None
+            PAM = None
 
-        logger.info(f'parse target_seq: target_seq={target_seq}, PAM_seq={PAM_seq}')
+        logger.info(f'parse target_seq: target_seq={target_seq}, PAM={PAM}')
 
         # fwd alignment & rev alignment
         # 为了判断target_seq (sgRNA) 是设计在fwd还是rev链上
-        final_align_forward = run_no_PAM_sgRNA_alignment_no_chop(ref_seq, target_seq, aligner)
-        logger.debug(f'final_align_forward:\n{final_align_forward}')
-        final_align_reverse = run_no_PAM_sgRNA_alignment_no_chop(ref_seq_rc, target_seq, aligner)
-        logger.debug(f'final_align_reverse:\n{final_align_reverse}')
-
-        fwd = final_align_forward[0]
-        rev = final_align_reverse[0]
+        if not PAM:
+            logger.info('use PAMless mode to align')
+            fwd = run_target_seq_align(ref_seq, target_seq, aligner)
+            logger.debug(f'final_align_forward:\n{fwd}')
+            rev = run_target_seq_align(ref_seq_rc, target_seq, aligner)
+            logger.debug(f'final_align_reverse:\n{rev}')
+        else:
+            logger.info('use PAM mode to align')
+            # TODO
+            fwd = run_target_seq_align(ref_seq, target_seq, aligner, PAM=PAM)
+            logger.debug(f'final_align_forward:\n{fwd}')
+            rev = run_target_seq_align(ref_seq_rc, target_seq, aligner, PAM=PAM)
+            logger.debug(f'final_align_reverse:\n{rev}')
 
         # get fwd alignment info
         reference_seq = fwd['alignment']['reference_seq'][fwd['ref_aln_start']: fwd['ref_aln_end'] + 1]
         align_info = fwd['alignment']['aln_info'][fwd['ref_aln_start']: fwd['ref_aln_end'] + 1]
         target_seq = fwd['alignment']['target_seq'][fwd['ref_aln_start']: fwd['ref_aln_end'] + 1]
         aln_score = fwd['aln_score']
         logger.info(
             f"Forward best alignment:\n"
             f"reference  : {reference_seq}\n"
             f"align_info : {align_info}\n"
             f"target_seq : {target_seq}\n"
             f"align_score: {aln_score}"
         )
         # get rev alignment info
+        print(rev)
         reference_seq_rev = rev['alignment']['reference_seq'][rev['ref_aln_start']: rev['ref_aln_end'] + 1]
         align_info_rev = rev['alignment']['aln_info'][rev['ref_aln_start']: rev['ref_aln_end'] + 1]
         target_seq_rev = rev['alignment']['target_seq'][rev['ref_aln_start']: rev['ref_aln_end'] + 1]
         aln_score_rev = rev['aln_score']
         logger.info(
             f"Reverse best alignment:\n"
             f"reference  : {reference_seq_rev}\n"
@@ -252,33 +240,39 @@
         ref_gap_count = 0
         ref_del_str = ""
 
         aln_start = aln['ref_aln_start']
         aln_end = aln['ref_aln_end']
 
         # update target_seq_aln
-        logger.debug(f'target_seq_aln = {target_seq_aln}')
-        logger.debug("update target_seq_aln: show ''.join(target_seq_aln)")
+        logger.debug(f'target_seq_aln (before update) = {target_seq_aln}')
+        logger.debug(f'target_seq_aln_insert (before update) = {target_seq_aln_insert}')
+
         for idx, ref_base in enumerate(reference_seq):
 
             # reference  : GCCTCTGGAGAGGGAGGAGGG
             # align_info : |.|.|||..|..|||||.||-
             # target_seq : GGCACTGCGGCTGGAGGTGG-
             if ref_base != "-":
                 ref_gap_count += 0
                 ref_del_str = ""
                 target_seq_aln[aln_start + idx - ref_gap_count] = ref_del_str + target_seq[idx]
             else:
                 ref_gap_count += 1
                 ref_del_str += target_seq[idx]  # for continuous gap
                 target_seq_aln_insert[aln_start + idx] = target_seq[idx]
-            logger.debug(f"{''.join(target_seq_aln)}")
+        logger.debug(
+            "update target_seq_aln: show ''.join(target_seq_aln)\n"
+            f"target_seq_aln = {''.join(target_seq_aln)}\n"
+            f"target_seq     = {target_seq}"
+        )
         logger.debug("update target_seq_aln: Done")
-        logger.debug(f'target_seq_aln = {target_seq_aln}')
-        logger.debug(f'target_seq_aln_insert = {target_seq_aln_insert}')
+        logger.debug(f'target_seq_aln (after update) = {target_seq_aln}')
+        logger.debug(f'target_seq_aln_insert (after update) = {target_seq_aln_insert}')
+
         # if reverse alignment
         if aln_direction == "Reverse Alignment":
             # illustrate reverse alignment as forward alignment
             target_seq_aln = target_seq_aln[::-1]
             target_seq_aln_insert = target_seq_aln_insert[::-1]
             logger.debug("use reverse alignment")
             logger.debug(f'target_seq_aln = {target_seq_aln}')
@@ -306,14 +300,17 @@
         plot_region = (possible_target_region_start, possible_target_region_end)
         df_bases_select = df_bases.iloc[plot_region[0]: plot_region[1], :]
         logger.debug('df_bases_select:\n' + tabulate(df_bases_select, headers='keys', tablefmt='psql'))
 
         # make plot
         # set color
         # show indel
+        matplotlib.use('Agg')
+        np.set_printoptions(suppress=True)
+
         indel_plot_state = show_indel
         index_plot_state = show_index
         box_border_plot_state = box_border
 
         # set panel size
         panel_box_width = 0.4
         panel_box_heigth = 0.4
@@ -341,63 +338,56 @@
         total_box_count = plot_region[1] - plot_region[0]
 
         # calculate base info and fix zero
         base_sum_count = df_bases_select.loc[:, ["A", "G", "C", "T"]].sum(axis=1).astype(int)
         logger.debug(f'base_sum_count =\n{base_sum_count.values}')
         total_sum_count = df_bases_select[["A", "G", "C", "T", "del_count", "insert_count"]].sum(axis=1).astype(int)
         logger.debug(f'total_sum_count =\n{total_sum_count.values}')
-        # print(base_sum_count[base_sum_count == 7997])
-        # idx = base_sum_count[base_sum_count == 7997].index
-        # base_sum_count[base_sum_count == 7997] = 1
-        # print(base_sum_count[idx])
-
         # fix 0 -> ["A.ratio", list(df_bases_select["A"] / base_sum_count)]
         base_sum_count[base_sum_count == 0] = 1
         total_sum_count[total_sum_count == 0] = 1
 
         # make plot size
-        logger.debug(f'aln = {aln}')
-        # print(aln['alignment']['target_seq'][plot_region[0]: plot_region[1]])
-        # print(target_seq_aln[plot_region[0]: plot_region[1]])
-        # exit()
+        logger.debug(f'aln =\n{aln}')
+
         if indel_plot_state:
             panel_height_coef = [.5, .9, .9] + [.5] * 6 + [.5] * 6
             panel_space_coef = [1.] * 3 + [.3] * 3 + [1., .3, 1.] + [.3] * 3 + [1., .3]
             plot_data_list = [
-                ["Index", df_bases_select.chr_index],
+                ["Ref_index", df_bases_select.chr_index],
                 ["Target_seq", target_seq_aln[plot_region[0]: plot_region[1]]],
                 ["Ref_seq", df_bases_select.ref_base],
                 ["A", np.array(df_bases_select["A"])],
                 ["G", np.array(df_bases_select["G"])],
                 ["C", np.array(df_bases_select["C"])],
                 ["T", np.array(df_bases_select["T"])],
                 ["Del", np.array(df_bases_select["del_count"])],
                 ["Ins", np.array(df_bases_select["insert_count"])],
-                ["A.ratio", list(df_bases_select["A"] / base_sum_count)],
-                ["G.ratio", list(df_bases_select["G"] / base_sum_count)],
-                ["C.ratio", list(df_bases_select["C"] / base_sum_count)],
-                ["T.ratio", list(df_bases_select["T"] / base_sum_count)],
-                ["Del.ratio", list(df_bases_select["del_count"] / total_sum_count)],
-                ["Ins.ratio", list(df_bases_select["insert_count"] / total_sum_count)]
+                ["A %", list(df_bases_select["A"] / base_sum_count)],
+                ["G %", list(df_bases_select["G"] / base_sum_count)],
+                ["C %", list(df_bases_select["C"] / base_sum_count)],
+                ["T %", list(df_bases_select["T"] / base_sum_count)],
+                ["Del %", list(df_bases_select["del_count"] / total_sum_count)],
+                ["Ins %", list(df_bases_select["insert_count"] / total_sum_count)]
             ]
         else:
             panel_height_coef = [.5, .9, .9] + [.5] * 4 + [.5] * 4
             panel_space_coef = [1.] * 3 + [0.3] * 3 + [1.] + [0.3] * 3
             plot_data_list = [
-                ["Index", df_bases_select.chr_index],
+                ["Ref_index", df_bases_select.chr_index],
                 ["Target_seq", target_seq_aln[plot_region[0]: plot_region[1]]],
                 ["Ref_seq", df_bases_select.ref_base],
                 ["A", np.array(df_bases_select["A"])],
                 ["G", np.array(df_bases_select["G"])],
                 ["C", np.array(df_bases_select["C"])],
                 ["T", np.array(df_bases_select["T"])],
-                ["A.ratio", list(df_bases_select["A"] / base_sum_count)],
-                ["G.ratio", list(df_bases_select["G"] / base_sum_count)],
-                ["C.ratio", list(df_bases_select["C"] / base_sum_count)],
-                ["T.ratio", list(df_bases_select["T"] / base_sum_count)]
+                ["A %", list(df_bases_select["A"] / base_sum_count)],
+                ["G %", list(df_bases_select["G"] / base_sum_count)],
+                ["C %", list(df_bases_select["C"] / base_sum_count)],
+                ["T %", list(df_bases_select["T"] / base_sum_count)]
             ]
 
         # get box and space info
         box_height_list = np.array(panel_height_coef) * panel_box_heigth
         panel_space_list = np.array(panel_space_coef) * panel_space
         logger.debug(f'box_height_list = {box_height_list}')
         logger.debug(f'panel_space_list = {panel_space_list}')
@@ -407,22 +397,17 @@
                        (total_box_count - 1) * panel_box_space + panel_box_width * 2
         figure_height = sum(box_height_list) + sum(panel_space_list)
 
         logger.debug(f'figure_width = {figure_width}')
         logger.debug(f'figure_height = {figure_height}')
 
         # make all box_x
-        box_x_vec = np.arange(
-            0,
-            figure_width +
-            panel_box_width,
-            panel_box_width +
-            panel_box_space)
+        box_x_vec = np.arange(0, figure_width + panel_box_width, panel_box_width + panel_box_space)
         box_x_vec = box_x_vec[:(len(ref_seq) + 1)]
-        logger.debug(f'box_x_vec =\n{box_x_vec}')
+        # logger.debug(f'box_x_vec (x for each column) =\n{box_x_vec}')
 
         # make box border
         if box_border_plot_state:
             box_edgecolor = "#AAAAAA"
             box_linestyle = "-"
             box_linewidth = 2
             logger.debug(f'box_border_plot_state = {box_border_plot_state}')
@@ -440,14 +425,16 @@
 
         # make box_y initialize
         current_y = 0
 
         logger.debug('start to plot')
         fig = plt.figure(figsize=(figure_width * 1.1, figure_height * 1.1))
         logger.debug(f'set new figure, figsize = ({figure_width * 1.1}, {figure_height * 1.1})')
+
+        plt.set_loglevel("info")
         # will show matplotlib debug log with logging
         ax = fig.add_subplot(111, aspect="equal")
         # will show matplotlib debug log with logging
         plt.xlim([0, figure_width])
         plt.ylim([-figure_height, 0])
         plt.axis("off")
         logger.debug(f'plt.xlim([0, {figure_width}])')
@@ -463,15 +450,15 @@
             # panel name
             panel_name = plot_data_list[panel_index][0]
             panel_name_x = box_x_vec[0]
             panel_name_y = current_y - box_height_list[panel_index] * 0.5
             text_list.append((panel_name_x, panel_name_y, panel_name, 10))
 
             # plot panel box
-            if panel_name == "Index":
+            if panel_name == "Ref_index":
                 # don't draw box, only add text
                 for index, box_value in enumerate(
                         plot_data_list[panel_index][1]):
                     box_x = box_x_vec[index + 1]
                     text_list.append(
                         (
                             box_x + panel_box_width * 0.5, current_y - box_height_list[panel_index] * 0.5,
@@ -538,15 +525,15 @@
             elif panel_name in ["A", "G", "C", "T", "Del", "Ins"]:
                 if panel_name in ["Del", "Ins"]:
                     box_ratio = plot_data_list[panel_index][1] / total_sum_count
                 else:
                     box_ratio = plot_data_list[panel_index][1] / base_sum_count
 
                 box_color_list = map_color(box_ratio, color_break, color_list)
-                logger.debug(f'box_color_list = {box_color_list}')
+                logger.debug(f'get box_color_list for {panel_name}')
 
                 for index, box_value in enumerate(plot_data_list[panel_index][1]):
                     box_color = box_color_list[index]
                     box_x = box_x_vec[index + 1]
 
                     patches.append(
                         Rectangle(
@@ -604,27 +591,22 @@
                     )
 
                 # make next panel_y
                 if panel_index < len(panel_space_list):
                     current_y = current_y - (box_height_list[panel_index] + panel_space_list[panel_index])
 
         # plot box
-        logger.debug(f'plot patches = {patches}')
+        logger.debug(f'plot rectangles')
         ax.add_collection(PatchCollection(patches, match_original=True))
-        logger.debug(f'plot text:\n{text_list}')
-        # add text
+
+        logger.debug(f'plot text on each rectangle')
         for text_x, text_y, text_info, text_fontsize in text_list:
             plt.text(
-                x=text_x,
-                y=text_y,
-                s=text_info,
-                horizontalalignment='center',
-                verticalalignment='center',
-                fontsize=text_fontsize,
-                fontname="Arial"
+                x=text_x, y=text_y, s=text_info, horizontalalignment='center', verticalalignment='center',
+                fontsize=text_fontsize, fontname="Arial"
             )
         # output plot
         fig.savefig(fname=output_fig, bbox_inches='tight', dpi=output_fig_dpi, format=output_fig_fmt)
 
     # def region_heatmap_merge(self):
     #     pass
```

### Comparing `bioat-0.1.5.2/PKG-INFO` & `bioat-0.1.5.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 Metadata-Version: 2.1
 Name: bioat
-Version: 0.1.5.2
+Version: 0.1.5.3
 Summary: Bioinformatic toolkit with python (It's still under development!)
 Home-page: https://github.com/hermanzhaozzzz/BioinformaticAnalysisTools
 License: MIT
 Author: Herman Zhao
 Author-email: hermanzhaozzzz@gmail.com
-Requires-Python: >=3.9.6,<4.0.0
+Requires-Python: >=3.8.0,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: biopython (>=1.81,<2.0)
+Requires-Dist: biopython (>=1.80,<2.0)
 Requires-Dist: cython (>=0.29.33,<0.30.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: pandarallel (>=1.6.4,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pysam (>=0.20.0,<0.21.0)
+Requires-Dist: scipy (>=1.8.0,<2.0.0)
+Requires-Dist: statsmodels (>=0.13.5,<0.14.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Project-URL: Repository, https://github.com/hermanzhaozzzz/BioinformaticAnalysisTools
 Description-Content-Type: text/markdown
 
 # BioinformaticAnalysisTools
+## about author
+
+> author: [赵华男 | ZHAO Hua-nan](https://scholar.google.com/citations?user=ojSVoWQAAAAJ&hl=en)
+>
+> email: hermanzhaozzzz@gmail.com
+>
+> [Zhihu](https://www.zhihu.com/people/hymanzhaozzzz) | [BLOG](http://zhaohuanan.cc)
 
 ## Introduction
 A python command line toolkit for Bioinformatics and data science!
 
-\<under development\>
-
-- Author: Hua-nan ZHAO @Tsinghua University
-- E-Mail: hermanzhaozzzz@gmail.com
+**\<under development\>**
 
 ## Installation
 ```shell
 # supported platform: Linux / MacOS (intel & arm64) / WSL on Windows
 pip install --upgrade bioat
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

