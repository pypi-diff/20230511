# Comparing `tmp/pyPINTS-1.1.8.tar.gz` & `tmp/pyPINTS-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPINTS-1.1.8.tar", last modified: Sat Oct  8 04:22:43 2022, max compression
+gzip compressed data, was "pyPINTS-1.1.9.tar", last modified: Thu May 11 20:25:13 2023, max compression
```

## Comparing `pyPINTS-1.1.8.tar` & `pyPINTS-1.1.9.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 04:22:43.429348 pyPINTS-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-10-08 04:22:39.000000 pyPINTS-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-08 04:22:39.000000 pyPINTS-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8257 2022-10-08 04:22:43.429348 pyPINTS-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7975 2022-10-08 04:22:39.000000 pyPINTS-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 04:22:43.433348 pyPINTS-1.1.8/pints/
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-10-08 04:22:39.000000 pyPINTS-1.1.8/pints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-10-08 04:22:43.433348 pyPINTS-1.1.8/pints/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    79170 2022-10-08 04:22:39.000000 pyPINTS-1.1.8/pints/calling_engine.py
--rw-r--r--   0 runner    (1001) docker     (121)    11807 2022-10-08 04:22:39.000000 pyPINTS-1.1.8/pints/extension_engine.py
--rw-r--r--   0 runner    (1001) docker     (121)    32473 2022-10-08 04:22:39.000000 pyPINTS-1.1.8/pints/io_engine.py
--rw-r--r--   0 runner    (1001) docker     (121)    27792 2022-10-08 04:22:39.000000 pyPINTS-1.1.8/pints/stats_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 04:22:43.429348 pyPINTS-1.1.8/pyPINTS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8257 2022-10-08 04:22:43.000000 pyPINTS-1.1.8/pyPINTS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-10-08 04:22:43.000000 pyPINTS-1.1.8/pyPINTS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-08 04:22:43.000000 pyPINTS-1.1.8/pyPINTS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-10-08 04:22:43.000000 pyPINTS-1.1.8/pyPINTS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-08 04:22:43.000000 pyPINTS-1.1.8/pyPINTS.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 04:22:43.429348 pyPINTS-1.1.8/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     5074 2022-10-08 04:22:39.000000 pyPINTS-1.1.8/scripts/pints_boundary_extender
--rw-r--r--   0 runner    (1001) docker     (121)    15162 2022-10-08 04:22:39.000000 pyPINTS-1.1.8/scripts/pints_caller
--rw-r--r--   0 runner    (1001) docker     (121)     8076 2022-10-08 04:22:39.000000 pyPINTS-1.1.8/scripts/pints_normalizer
--rw-r--r--   0 runner    (1001) docker     (121)    11832 2022-10-08 04:22:39.000000 pyPINTS-1.1.8/scripts/pints_visualizer
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-10-08 04:22:43.433348 pyPINTS-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-10-08 04:22:39.000000 pyPINTS-1.1.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    70194 2022-10-08 04:22:39.000000 pyPINTS-1.1.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:25:13.410160 pyPINTS-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-11 20:25:05.000000 pyPINTS-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-11 20:25:05.000000 pyPINTS-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-11 20:25:13.410160 pyPINTS-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-05-11 20:25:05.000000 pyPINTS-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:25:13.410160 pyPINTS-1.1.9/pints/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-11 20:25:05.000000 pyPINTS-1.1.9/pints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-11 20:25:13.410160 pyPINTS-1.1.9/pints/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79299 2023-05-11 20:25:05.000000 pyPINTS-1.1.9/pints/calling_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11803 2023-05-11 20:25:05.000000 pyPINTS-1.1.9/pints/extension_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-05-11 20:25:05.000000 pyPINTS-1.1.9/pints/io_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-11 20:25:05.000000 pyPINTS-1.1.9/pints/qc_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27792 2023-05-11 20:25:05.000000 pyPINTS-1.1.9/pints/stats_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:25:13.410160 pyPINTS-1.1.9/pyPINTS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-11 20:25:13.000000 pyPINTS-1.1.9/pyPINTS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-11 20:25:13.000000 pyPINTS-1.1.9/pyPINTS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:25:13.000000 pyPINTS-1.1.9/pyPINTS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-11 20:25:13.000000 pyPINTS-1.1.9/pyPINTS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 20:25:13.000000 pyPINTS-1.1.9/pyPINTS.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:25:13.410160 pyPINTS-1.1.9/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-05-11 20:25:05.000000 pyPINTS-1.1.9/scripts/pints_boundary_extender
+-rw-r--r--   0 runner    (1001) docker     (123)    15276 2023-05-11 20:25:05.000000 pyPINTS-1.1.9/scripts/pints_caller
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-11 20:25:05.000000 pyPINTS-1.1.9/scripts/pints_normalizer
+-rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-05-11 20:25:05.000000 pyPINTS-1.1.9/scripts/pints_visualizer
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-11 20:25:13.410160 pyPINTS-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-11 20:25:05.000000 pyPINTS-1.1.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70194 2023-05-11 20:25:05.000000 pyPINTS-1.1.9/versioneer.py
```

### Comparing `pyPINTS-1.1.8/LICENSE` & `pyPINTS-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPINTS-1.1.8/PKG-INFO` & `pyPINTS-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPINTS
-Version: 1.1.8
+Version: 1.1.9
 Summary: Peak Identifier for Nascent Transcripts Starts (PINTS)
 Home-page: https://pints.yulab.org
 Author: Li Yao
 Author-email: regulatorygenome@gmail.com
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyPINTS-1.1.8/README.md` & `pyPINTS-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyPINTS-1.1.8/pints/__init__.py` & `pyPINTS-1.1.9/pints/__init__.py`

 * *Files identical despite different names*

### Comparing `pyPINTS-1.1.8/pints/calling_engine.py` & `pyPINTS-1.1.9/pints/calling_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # coding=utf-8
 
-#  PINTS: Peak Identifier for Nascent Transcripts Sequencing
+#  PINTS: Peak Identifier for Nascent Transcripts Starts
 #  Copyright (c) 2019-2022. Li Yao at the Yu Lab.
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
@@ -318,28 +318,30 @@
     """
     selected_window = chromosome_coverage[coord_start:coord_end]
     window_value = np.sum(selected_window)
     if coord_end - coord_start < small_window_threshold \
             or window_value == 0:
         return 1., window_value, 0, 0, (0, 0, 0)
     flanking = np.asarray(flanking, dtype=int) // 2
+    chr_len = len(chromosome_coverage)
     mus = []
     variances = []
     pis = []
     ler_counts = []
     for f in flanking:
         qsl = coord_start - f
         qel = coord_start - 1
         qsl = qsl if qsl >= 0 else 0
         qsr = coord_end + 1
         qer = coord_end + f
         bg, x = iqr_obj.remove_peaks_in_local_env(stat_tester=stat_tester, bed_handler=sp_bed_handler,
-                                                  chromosome=chromosome_name, query_start_left=qsl,
-                                                  query_end_left=qel, query_start_right=qsr,
-                                                  query_end_right=qer, small_window_threshold=small_window_threshold,
+                                                  chromosome=chromosome_name, query_start_left=max(qsl, 0),
+                                                  query_end_left=max(qel, 0), query_start_right=min(qsr, chr_len),
+                                                  query_end_right=min(qer, chr_len),
+                                                  small_window_threshold=small_window_threshold,
                                                   peak_in_bg_threshold=peak_in_bg_threshold,
                                                   coverage_info=chromosome_coverage,
                                                   fdr_target=fdr_target, cache=cache,
                                                   disable_ler=disable_ler, enable_eler=enable_eler,
                                                   peak_threshold=top_peak_mu)
 
         mu_, var_, pi_, _, _ = stat_tester.fit(bg)
```

### Comparing `pyPINTS-1.1.8/pints/extension_engine.py` & `pyPINTS-1.1.9/pints/extension_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # coding=utf-8
 
-#  PINTS: Peak Identifier for Nascent Transcripts Sequencing
+#  PINTS: Peak Identifier for Nascent Transcripts Starts
 #  Copyright (c) 2019-2022. Li Yao at the Yu Lab.
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
```

### Comparing `pyPINTS-1.1.8/pints/io_engine.py` & `pyPINTS-1.1.9/pints/io_engine.py`

 * *Files identical despite different names*

### Comparing `pyPINTS-1.1.8/pints/stats_engine.py` & `pyPINTS-1.1.9/pints/stats_engine.py`

 * *Files identical despite different names*

### Comparing `pyPINTS-1.1.8/pyPINTS.egg-info/PKG-INFO` & `pyPINTS-1.1.9/pyPINTS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPINTS
-Version: 1.1.8
+Version: 1.1.9
 Summary: Peak Identifier for Nascent Transcripts Starts (PINTS)
 Home-page: https://pints.yulab.org
 Author: Li Yao
 Author-email: regulatorygenome@gmail.com
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyPINTS-1.1.8/scripts/pints_boundary_extender` & `pyPINTS-1.1.9/scripts/pints_boundary_extender`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,16 @@
                     handlers=[
                         logging.StreamHandler()
                     ])
 logger = logging.getLogger("PINTS - BoundaryExtender")
 
 
 if __name__ == "__main__":
-    parser = argparse.ArgumentParser(description="Element boundary refinement")
+    parser = argparse.ArgumentParser(description="Element boundary refinement",
+                                     formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     group = parser.add_mutually_exclusive_group(required=True)
     group.add_argument("--bam-files", action="store", dest="bam_files", nargs="*",
                        type=str, required=False,
                        help="input bam file, if you want to use bigwig files, please use --bw-pl and --bw-mn")
     group.add_argument("--bw-pl", action="store", dest="bw_pl", nargs="*",
                        type=str, required=False,
                        help="Bigwig for plus strand. If you want to use bigwig instead of BAM, "
```

### Comparing `pyPINTS-1.1.8/scripts/pints_caller` & `pyPINTS-1.1.9/scripts/pints_caller`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,16 @@
                     handlers=[
                         logging.StreamHandler()
                     ])
 logger = logging.getLogger("PINTS - Caller")
 
 
 if __name__ == "__main__":
-    parser = argparse.ArgumentParser(description="Peak Identifier for Nascent Transcripts Starts")
+    parser = argparse.ArgumentParser(description="Peak Identifier for Nascent Transcripts Starts",
+                                     formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     group = parser.add_argument_group("Input/Output")
     group.add_argument("--bam-file", action="store", dest="bam_file", nargs="*",
                        type=str, required=False,
                        help="input bam file, if you want to use bigwig files, please use --bw-pl and --bw-mn")
     group.add_argument("--save-to", action="store", dest="save_to",
                        type=str, required=False, default=".",
                        help="save peaks to this path (a folder), by default, current folder")
@@ -121,15 +122,15 @@
                        help="BPs to be extended from annotated TSSs, these extended regions will be used to minimize "
                             "overlaps between called peaks.")
     group.add_argument("--focused-chrom", action="store", dest="focused_chrom", default="chr1", type=str,
                        required=False,
                        help="If --annotation-gtf is specified, you use this parameter to change which chromosome the "
                             "tool should learn the values from.")
     group.add_argument("--alpha", "--donor-tolerance", action="store", dest="donor_tolerance",
-                       type=float, required=False, default=0.3, 
+                       type=float, required=False, default=0.3,
                        help="The stringency for PINTS to cluster nearby TSSs into a peak. 0 is the least stringent; "
                             "1 is the most stringent.")
     group.add_argument("--ce-trigger", action="store", dest="ce_trigger",
                        type=int, required=False, default=3, help="Trigger for receptor tolerance checking")
 
     group = parser.add_argument_group("Peak properties")
     group.add_argument("--top-peak-threshold", action="store", dest="top_peak_threshold",
@@ -171,15 +172,15 @@
                             "(shorter than --small-peak-threshold)")
 
     group = parser.add_argument_group("Other")
     group.add_argument("--epig-annotation", action="store", dest="epig_annotation", type=str, required=False,
                        help="Refine peak calls with compiled epigenomic annotation from the PINTS web server."
                             " Values should be the name of the biosample, for example, K562.")
     group.add_argument("--relaxed-fdr-target", action="store", dest="relaxed_fdr_target", default=0.2,
-                       type=float, required=False, help="Relaxed FDR cutoff for TREs overlap with ")
+                       type=float, required=False, help="Relaxed FDR cutoff for TREs overlap with epigenomic annotations")
     group.add_argument("--chromosome-start-with", action="store", dest="chromosome_startswith",
                        type=str, required=False, default="chr",
                        help="Only keep reads mapped to chromosomes with this prefix")
     group.add_argument("--dont-output-chrom-size", action="store_false", dest="output_chrom_size",
                        required=False, default=True,
                        help="Don't write chromosome dict to local folder (not recommended)")
     group.add_argument("--dont-check-updates", action="store_false", dest="check_updates",
```

### Comparing `pyPINTS-1.1.8/scripts/pints_normalizer` & `pyPINTS-1.1.9/scripts/pints_normalizer`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     for bam in bam_files:
         logger.info("Working on %s" % bam)
         bam_to_bigwig(bam, exp_type=exp_type, output_dir=output_dir, normalization_factor=1, rpm=True, rc=rc, **kwargs)
         bam_to_bigwig(bam, exp_type=exp_type, output_dir=output_dir, normalization_factor=1, rpm=True, rc=rc, **kwargs)
 
 
 if __name__ == "__main__":
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument("-m", "--method", help="Normalization method, acceptable values: RPM or Spikein")
     parser.add_argument("-b", "--bam", nargs="+", required=True)
     parser.add_argument("-f", "--fasta-spike-in")
     parser.add_argument("-e", "--exp-type")
     parser.add_argument("-o", "--output-dir")
     parser.add_argument("-c", "--cell-numbers", nargs="+", required=False, type=int)
     parser.add_argument("-r", "--reverse-complement", action="store_true", dest="seq_reverse_complement",
```

### Comparing `pyPINTS-1.1.8/scripts/pints_visualizer` & `pyPINTS-1.1.9/scripts/pints_visualizer`

 * *Files 6% similar despite different names*

```diff
@@ -143,19 +143,19 @@
     mn_ranges, mn_csize, mn_sum = _strand_atom(mn_dict, normalization_factor=normalization_factor,
                                                strand_sign="-")
     logger.info("Done: Generating signal tracks for reverse strand")
 
     if rpm_normalization:
         logger.info("%d reads passed filter" % (pl_sum + mn_sum))
         rpm_scale = 1000 * 1000 / (pl_sum + mn_sum)
-        logger.info("RPM normalizing (forward strand)")
+        logger.info("RPM normalizing (forward strand) with scale factor {:.3f}".format(rpm_scale))
         pl_ranges[3] = (np.asarray(pl_ranges[3]) * rpm_scale).tolist()
         logger.info("Done: RPM normalizing (forward strand)")
 
-        logger.info("RPM normalizing (reverse strand)")
+        logger.info("RPM normalizing (reverse strand) with scale factor {:.3f}".format(rpm_scale))
         # mn_ranges.Score *= rpm_scale
         mn_ranges[3] = (np.asarray(mn_ranges[3]) * rpm_scale).tolist()
         logger.info("Done: RPM normalizing (reverse strand)")
 
     logger.info("Generating bigwig file for forward strand")
     pl_fn = os.path.join(output_pref + "_pl.bw")
     if len(pl_ranges[0]) > 0:
@@ -237,15 +237,15 @@
                 try:
                     os.remove(hf)
                 except:
                     pass
 
 
 if __name__ == "__main__":
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument("-b", "--bam", action="store", required=True)
     parser.add_argument("-e", "--exp-type", action="store", default=None, dest="bam_parser",
                         help="Type of experiment, acceptable values are: CoPRO/GROcap/GROseq/PROcap/PROseq, or if you "
                              "know the position of RNA ends which you\'re interested on the reads, you can specify "
                              "R_5, R_3, R1_5, R1_3, R2_5 or R2_3")
     parser.add_argument("-r", "--reverse-complement", action="store_true", dest="seq_reverse_complement",
                         required=False, default=False,
```

### Comparing `pyPINTS-1.1.8/setup.py` & `pyPINTS-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyPINTS-1.1.8/versioneer.py` & `pyPINTS-1.1.9/versioneer.py`

 * *Files identical despite different names*

