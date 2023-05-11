# Comparing `tmp/CNFgen-0.9.1.tar.gz` & `tmp/CNFgen-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CNFgen-0.9.1.tar", last modified: Mon Dec 12 21:10:28 2022, max compression
+gzip compressed data, was "CNFgen-0.9.2.tar", last modified: Thu May 11 14:51:01 2023, max compression
```

## Comparing `CNFgen-0.9.1.tar` & `CNFgen-0.9.2.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwx------   0 massimo   (1000) massimo   (1000)        0 2022-12-12 21:10:28.626401 CNFgen-0.9.1/
-drwx------   0 massimo   (1000) massimo   (1000)        0 2022-12-12 21:10:28.618401 CNFgen-0.9.1/CNFgen.egg-info/
--rw-------   0 massimo   (1000) massimo   (1000)     1254 2022-12-12 21:10:28.000000 CNFgen-0.9.1/CNFgen.egg-info/PKG-INFO
--rw-------   0 massimo   (1000) massimo   (1000)     2047 2022-12-12 21:10:28.000000 CNFgen-0.9.1/CNFgen.egg-info/SOURCES.txt
--rw-------   0 massimo   (1000) massimo   (1000)        1 2022-12-12 21:10:28.000000 CNFgen-0.9.1/CNFgen.egg-info/dependency_links.txt
--rw-------   0 massimo   (1000) massimo   (1000)      136 2022-12-12 21:10:28.000000 CNFgen-0.9.1/CNFgen.egg-info/entry_points.txt
--rw-------   0 massimo   (1000) massimo   (1000)       27 2022-12-12 21:10:28.000000 CNFgen-0.9.1/CNFgen.egg-info/requires.txt
--rw-------   0 massimo   (1000) massimo   (1000)        7 2022-12-12 21:10:28.000000 CNFgen-0.9.1/CNFgen.egg-info/top_level.txt
--rw-------   0 massimo   (1000) massimo   (1000)      954 2022-08-24 16:38:58.000000 CNFgen-0.9.1/CREDITS.org
--rw-------   0 massimo   (1000) massimo   (1000)    35128 2022-08-24 16:38:58.000000 CNFgen-0.9.1/LICENSE
--rw-------   0 massimo   (1000) massimo   (1000)      113 2022-08-24 16:38:58.000000 CNFgen-0.9.1/MANIFEST.in
--rw-------   0 massimo   (1000) massimo   (1000)     2553 2022-08-24 16:38:58.000000 CNFgen-0.9.1/Makefile
--rw-------   0 massimo   (1000) massimo   (1000)     1254 2022-12-12 21:10:28.626401 CNFgen-0.9.1/PKG-INFO
--rw-------   0 massimo   (1000) massimo   (1000)      944 2022-08-24 16:38:58.000000 CNFgen-0.9.1/PyPI.md
--rw-------   0 massimo   (1000) massimo   (1000)     3263 2022-08-24 16:38:58.000000 CNFgen-0.9.1/README.org
-drwx------   0 massimo   (1000) massimo   (1000)        0 2022-12-12 21:10:28.618401 CNFgen-0.9.1/cnfgen/
--rw-------   0 massimo   (1000) massimo   (1000)     3448 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/__init__.py
-drwx------   0 massimo   (1000) massimo   (1000)        0 2022-12-12 21:10:28.618401 CNFgen-0.9.1/cnfgen/clihelpers/
--rw-------   0 massimo   (1000) massimo   (1000)        0 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clihelpers/__init__.py
--rw-------   0 massimo   (1000) massimo   (1000)    11866 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clihelpers/counting_helpers.py
--rw-------   0 massimo   (1000) massimo   (1000)     1915 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clihelpers/cpls_helpers.py
--rw-------   0 massimo   (1000) massimo   (1000)     1732 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clihelpers/dimacs_helpers.py
--rw-------   0 massimo   (1000) massimo   (1000)      706 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clihelpers/formula_helpers.py
--rw-------   0 massimo   (1000) massimo   (1000)    14314 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clihelpers/graph_helpers.py
--rw-------   0 massimo   (1000) massimo   (1000)     5736 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clihelpers/ordering_helpers.py
--rw-------   0 massimo   (1000) massimo   (1000)     4353 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clihelpers/pebbling_helpers.py
--rw-------   0 massimo   (1000) massimo   (1000)    17206 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clihelpers/php_helpers.py
--rw-------   0 massimo   (1000) massimo   (1000)     1947 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clihelpers/pitfall_helpers.py
--rw-------   0 massimo   (1000) massimo   (1000)     6503 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clihelpers/simple_helpers.py
--rw-------   0 massimo   (1000) massimo   (1000)    16941 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clihelpers/transformation_helpers.py
-drwx------   0 massimo   (1000) massimo   (1000)        0 2022-12-12 21:10:28.622401 CNFgen-0.9.1/cnfgen/clitools/
--rw-------   0 massimo   (1000) massimo   (1000)     1117 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clitools/__init__.py
--rwx------   0 massimo   (1000) massimo   (1000)     9386 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clitools/cmdline.py
--rwx------   0 massimo   (1000) massimo   (1000)    19135 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clitools/cnfgen.py
--rw-------   0 massimo   (1000) massimo   (1000)     5472 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clitools/cnfshuffle.py
--rw-------   0 massimo   (1000) massimo   (1000)    14525 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clitools/graph_args.py
--rw-------   0 massimo   (1000) massimo   (1000)    14232 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clitools/graph_build.py
--rw-------   0 massimo   (1000) massimo   (1000)     5967 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clitools/graph_docs.py
--rwx------   0 massimo   (1000) massimo   (1000)     2972 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clitools/graph_fileinput.py
--rw-------   0 massimo   (1000) massimo   (1000)     6298 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clitools/kthlist2pebbling.py
--rw-------   0 massimo   (1000) massimo   (1000)     1769 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clitools/msg.py
--rw-------   0 massimo   (1000) massimo   (1000)    15414 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/clitools/pbgen.py
-drwx------   0 massimo   (1000) massimo   (1000)        0 2022-12-12 21:10:28.622401 CNFgen-0.9.1/cnfgen/families/
--rw-------   0 massimo   (1000) massimo   (1000)        0 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/families/__init__.py
--rw-------   0 massimo   (1000) massimo   (1000)     2336 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/families/cliquecoloring.py
--rwx------   0 massimo   (1000) massimo   (1000)     2949 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/families/coloring.py
--rw-------   0 massimo   (1000) massimo   (1000)     1777 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/families/counting.py
--rw-------   0 massimo   (1000) massimo   (1000)     3028 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/families/cpls.py
--rw-------   0 massimo   (1000) massimo   (1000)     3874 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/families/dominatingset.py
--rw-------   0 massimo   (1000) massimo   (1000)     2222 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/families/graphisomorphism.py
--rw-------   0 massimo   (1000) massimo   (1000)     4309 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/families/ordering.py
--rwx------   0 massimo   (1000) massimo   (1000)     7136 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/families/pebbling.py
--rw-------   0 massimo   (1000) massimo   (1000)    11935 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/families/pigeonhole.py
--rw-------   0 massimo   (1000) massimo   (1000)     5408 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/families/pitfall.py
--rw-------   0 massimo   (1000) massimo   (1000)     6300 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/families/ramsey.py
--rw-------   0 massimo   (1000) massimo   (1000)     3847 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/families/randomformulas.py
--rw-------   0 massimo   (1000) massimo   (1000)     6837 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/families/subgraph.py
--rw-------   0 massimo   (1000) massimo   (1000)     3207 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/families/subsetcardinality.py
--rw-------   0 massimo   (1000) massimo   (1000)     1651 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/families/tseitin.py
-drwx------   0 massimo   (1000) massimo   (1000)        0 2022-12-12 21:10:28.622401 CNFgen-0.9.1/cnfgen/formula/
--rw-------   0 massimo   (1000) massimo   (1000)        0 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/formula/__init__.py
--rw-------   0 massimo   (1000) massimo   (1000)     9755 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/formula/basecnf.py
--rw-------   0 massimo   (1000) massimo   (1000)    18010 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/formula/baseopb.py
--rwx------   0 massimo   (1000) massimo   (1000)     2425 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/formula/cnf.py
--rw-------   0 massimo   (1000) massimo   (1000)    13353 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/formula/cnfio.py
--rw-------   0 massimo   (1000) massimo   (1000)     7764 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/formula/linear.py
--rw-------   0 massimo   (1000) massimo   (1000)     2632 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/formula/opb.py
--rw-------   0 massimo   (1000) massimo   (1000)     4658 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/formula/opbio.py
--rw-------   0 massimo   (1000) massimo   (1000)    64230 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/formula/variables.py
--rwx------   0 massimo   (1000) massimo   (1000)    61042 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/graphs.py
--rw-------   0 massimo   (1000) massimo   (1000)     1189 2022-12-12 21:05:28.000000 CNFgen-0.9.1/cnfgen/info.py
--rw-------   0 massimo   (1000) massimo   (1000)     2378 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/localtypes.py
-drwx------   0 massimo   (1000) massimo   (1000)        0 2022-12-12 21:10:28.622401 CNFgen-0.9.1/cnfgen/transformations/
--rw-------   0 massimo   (1000) massimo   (1000)        0 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/transformations/__init__.py
--rw-------   0 massimo   (1000) massimo   (1000)     4446 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/transformations/shuffle.py
--rw-------   0 massimo   (1000) massimo   (1000)    12741 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/transformations/substitutions.py
-drwx------   0 massimo   (1000) massimo   (1000)        0 2022-12-12 21:10:28.626401 CNFgen-0.9.1/cnfgen/utils/
--rw-------   0 massimo   (1000) massimo   (1000)      105 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/utils/__init__.py
--rw-------   0 massimo   (1000) massimo   (1000)     6938 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/utils/latexoutput.py
--rw-------   0 massimo   (1000) massimo   (1000)     2853 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/utils/opb.py
--rw-------   0 massimo   (1000) massimo   (1000)     5820 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/utils/parsedimacs.py
--rw-------   0 massimo   (1000) massimo   (1000)    14980 2022-08-24 16:38:58.000000 CNFgen-0.9.1/cnfgen/utils/solver.py
--rw-------   0 massimo   (1000) massimo   (1000)       18 2022-12-12 21:10:28.000000 CNFgen-0.9.1/cnfgen/version.py
--rw-------   0 massimo   (1000) massimo   (1000)       27 2022-08-24 16:38:58.000000 CNFgen-0.9.1/requirements.txt
--rw-------   0 massimo   (1000) massimo   (1000)       38 2022-12-12 21:10:28.626401 CNFgen-0.9.1/setup.cfg
--rw-------   0 massimo   (1000) massimo   (1000)     1027 2022-08-24 16:38:58.000000 CNFgen-0.9.1/setup.py
+drwx------   0 massimo    (501) staff       (20)        0 2023-05-11 14:51:01.888768 CNFgen-0.9.2/
+drwx------   0 massimo    (501) staff       (20)        0 2023-05-11 14:51:01.861177 CNFgen-0.9.2/CNFgen.egg-info/
+-rw-------   0 massimo    (501) staff       (20)     1234 2023-05-11 14:51:01.000000 CNFgen-0.9.2/CNFgen.egg-info/PKG-INFO
+-rw-------   0 massimo    (501) staff       (20)     2077 2023-05-11 14:51:01.000000 CNFgen-0.9.2/CNFgen.egg-info/SOURCES.txt
+-rw-------   0 massimo    (501) staff       (20)        1 2023-05-11 14:51:01.000000 CNFgen-0.9.2/CNFgen.egg-info/dependency_links.txt
+-rw-------   0 massimo    (501) staff       (20)      135 2023-05-11 14:51:01.000000 CNFgen-0.9.2/CNFgen.egg-info/entry_points.txt
+-rw-------   0 massimo    (501) staff       (20)       27 2023-05-11 14:51:01.000000 CNFgen-0.9.2/CNFgen.egg-info/requires.txt
+-rw-------   0 massimo    (501) staff       (20)        7 2023-05-11 14:51:01.000000 CNFgen-0.9.2/CNFgen.egg-info/top_level.txt
+-rw-------   0 massimo    (501) staff       (20)      954 2022-08-15 11:20:27.000000 CNFgen-0.9.2/CREDITS.org
+-rw-------   0 massimo    (501) staff       (20)    35128 2022-08-15 11:20:27.000000 CNFgen-0.9.2/LICENSE
+-rw-------   0 massimo    (501) staff       (20)      113 2022-08-15 11:20:27.000000 CNFgen-0.9.2/MANIFEST.in
+-rw-------   0 massimo    (501) staff       (20)     2582 2023-01-15 11:21:57.000000 CNFgen-0.9.2/Makefile
+-rw-------   0 massimo    (501) staff       (20)     1234 2023-05-11 14:51:01.888252 CNFgen-0.9.2/PKG-INFO
+-rw-------   0 massimo    (501) staff       (20)      944 2022-08-15 11:20:27.000000 CNFgen-0.9.2/PyPI.md
+-rw-------   0 massimo    (501) staff       (20)     3263 2022-08-15 11:20:27.000000 CNFgen-0.9.2/README.org
+drwx------   0 massimo    (501) staff       (20)        0 2023-05-11 14:51:01.863429 CNFgen-0.9.2/cnfgen/
+-rw-------   0 massimo    (501) staff       (20)     3498 2023-03-30 20:33:37.000000 CNFgen-0.9.2/cnfgen/__init__.py
+drwx------   0 massimo    (501) staff       (20)        0 2023-05-11 14:51:01.867329 CNFgen-0.9.2/cnfgen/clihelpers/
+-rw-------   0 massimo    (501) staff       (20)        0 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clihelpers/__init__.py
+-rw-r--r--   0 massimo    (501) staff       (20)    12300 2023-04-26 01:25:24.000000 CNFgen-0.9.2/cnfgen/clihelpers/counting_helpers.py
+-rw-------   0 massimo    (501) staff       (20)     1915 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clihelpers/cpls_helpers.py
+-rw-------   0 massimo    (501) staff       (20)     1732 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clihelpers/dimacs_helpers.py
+-rw-------   0 massimo    (501) staff       (20)      706 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clihelpers/formula_helpers.py
+-rw-------   0 massimo    (501) staff       (20)    14314 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clihelpers/graph_helpers.py
+-rw-------   0 massimo    (501) staff       (20)     5736 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clihelpers/ordering_helpers.py
+-rw-------   0 massimo    (501) staff       (20)     4353 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clihelpers/pebbling_helpers.py
+-rw-------   0 massimo    (501) staff       (20)    17206 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clihelpers/php_helpers.py
+-rw-------   0 massimo    (501) staff       (20)     1947 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clihelpers/pitfall_helpers.py
+-rw-------   0 massimo    (501) staff       (20)     8535 2023-03-30 20:45:56.000000 CNFgen-0.9.2/cnfgen/clihelpers/simple_helpers.py
+-rw-------   0 massimo    (501) staff       (20)    16941 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clihelpers/transformation_helpers.py
+drwx------   0 massimo    (501) staff       (20)        0 2023-05-11 14:51:01.870698 CNFgen-0.9.2/cnfgen/clitools/
+-rw-------   0 massimo    (501) staff       (20)     1117 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clitools/__init__.py
+-rwx------   0 massimo    (501) staff       (20)     9386 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clitools/cmdline.py
+-rwx------   0 massimo    (501) staff       (20)    19172 2023-03-30 19:31:28.000000 CNFgen-0.9.2/cnfgen/clitools/cnfgen.py
+-rw-------   0 massimo    (501) staff       (20)     5472 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clitools/cnfshuffle.py
+-rw-------   0 massimo    (501) staff       (20)    14525 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clitools/graph_args.py
+-rw-------   0 massimo    (501) staff       (20)    14232 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clitools/graph_build.py
+-rw-------   0 massimo    (501) staff       (20)     5967 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clitools/graph_docs.py
+-rwx------   0 massimo    (501) staff       (20)     2972 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clitools/graph_fileinput.py
+-rw-------   0 massimo    (501) staff       (20)     6298 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clitools/kthlist2pebbling.py
+-rw-------   0 massimo    (501) staff       (20)     1769 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clitools/msg.py
+-rw-------   0 massimo    (501) staff       (20)    15414 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clitools/pbgen.py
+drwx------   0 massimo    (501) staff       (20)        0 2023-05-11 14:51:01.878539 CNFgen-0.9.2/cnfgen/families/
+-rw-------   0 massimo    (501) staff       (20)        0 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/__init__.py
+-rw-------   0 massimo    (501) staff       (20)     2336 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/cliquecoloring.py
+-rwx------   0 massimo    (501) staff       (20)     2949 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/coloring.py
+-rw-------   0 massimo    (501) staff       (20)     1777 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/counting.py
+-rw-------   0 massimo    (501) staff       (20)     3028 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/cpls.py
+-rw-------   0 massimo    (501) staff       (20)     3874 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/dominatingset.py
+-rw-------   0 massimo    (501) staff       (20)     2222 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/graphisomorphism.py
+-rw-------   0 massimo    (501) staff       (20)     4309 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/ordering.py
+-rwx------   0 massimo    (501) staff       (20)     7136 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/pebbling.py
+-rw-------   0 massimo    (501) staff       (20)    11935 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/pigeonhole.py
+-rw-------   0 massimo    (501) staff       (20)     5408 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/pitfall.py
+-rw-------   0 massimo    (501) staff       (20)     6300 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/ramsey.py
+-rw-------   0 massimo    (501) staff       (20)     4005 2023-03-30 20:22:27.000000 CNFgen-0.9.2/cnfgen/families/randomformulas.py
+-rw-r--r--   0 massimo    (501) staff       (20)     4318 2023-03-30 20:22:10.000000 CNFgen-0.9.2/cnfgen/families/randomkxor.py
+-rw-------   0 massimo    (501) staff       (20)     6837 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/subgraph.py
+-rw-------   0 massimo    (501) staff       (20)     3207 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/subsetcardinality.py
+-rw-------   0 massimo    (501) staff       (20)     1651 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/tseitin.py
+drwx------   0 massimo    (501) staff       (20)        0 2023-05-11 14:51:01.883733 CNFgen-0.9.2/cnfgen/formula/
+-rw-------   0 massimo    (501) staff       (20)        0 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/formula/__init__.py
+-rw-------   0 massimo    (501) staff       (20)     9755 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/formula/basecnf.py
+-rw-------   0 massimo    (501) staff       (20)    18010 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/formula/baseopb.py
+-rwx------   0 massimo    (501) staff       (20)     2425 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/formula/cnf.py
+-rw-------   0 massimo    (501) staff       (20)    13353 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/formula/cnfio.py
+-rw-------   0 massimo    (501) staff       (20)     8052 2023-03-30 19:47:51.000000 CNFgen-0.9.2/cnfgen/formula/linear.py
+-rw-------   0 massimo    (501) staff       (20)     2632 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/formula/opb.py
+-rw-------   0 massimo    (501) staff       (20)     4661 2023-03-30 16:53:11.000000 CNFgen-0.9.2/cnfgen/formula/opbio.py
+-rw-------   0 massimo    (501) staff       (20)    64230 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/formula/variables.py
+-rwx------   0 massimo    (501) staff       (20)    61042 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/graphs.py
+-rw-------   0 massimo    (501) staff       (20)     1189 2022-12-24 07:47:49.000000 CNFgen-0.9.2/cnfgen/info.py
+-rw-------   0 massimo    (501) staff       (20)     2378 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/localtypes.py
+drwx------   0 massimo    (501) staff       (20)        0 2023-05-11 14:51:01.885254 CNFgen-0.9.2/cnfgen/transformations/
+-rw-------   0 massimo    (501) staff       (20)        0 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/transformations/__init__.py
+-rw-------   0 massimo    (501) staff       (20)     4446 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/transformations/shuffle.py
+-rw-------   0 massimo    (501) staff       (20)    12741 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/transformations/substitutions.py
+drwx------   0 massimo    (501) staff       (20)        0 2023-05-11 14:51:01.887588 CNFgen-0.9.2/cnfgen/utils/
+-rw-------   0 massimo    (501) staff       (20)      105 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/utils/__init__.py
+-rw-------   0 massimo    (501) staff       (20)     6938 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/utils/latexoutput.py
+-rw-------   0 massimo    (501) staff       (20)     2853 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/utils/opb.py
+-rw-------   0 massimo    (501) staff       (20)     5808 2023-04-08 07:46:21.000000 CNFgen-0.9.2/cnfgen/utils/parsedimacs.py
+-rw-------   0 massimo    (501) staff       (20)    14980 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/utils/solver.py
+-rw-------   0 massimo    (501) staff       (20)       18 2023-05-11 14:51:01.000000 CNFgen-0.9.2/cnfgen/version.py
+-rw-------   0 massimo    (501) staff       (20)       32 2023-01-15 11:21:57.000000 CNFgen-0.9.2/requirements.txt
+-rw-------   0 massimo    (501) staff       (20)       38 2023-05-11 14:51:01.888920 CNFgen-0.9.2/setup.cfg
+-rw-------   0 massimo    (501) staff       (20)     1027 2022-08-15 11:20:27.000000 CNFgen-0.9.2/setup.py
```

### Comparing `CNFgen-0.9.1/CNFgen.egg-info/PKG-INFO` & `CNFgen-0.9.2/CNFgen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: CNFgen
-Version: 0.9.1
+Version: 0.9.2
 Summary: CNF formula generator
 Home-page: https://massimolauria.net/cnfgen
 Author: Massimo Lauria
 Author-email: massimo.lauria@uniroma1.it
 License: GPL-3
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CNFgen formula generator and tools
 
 This repository provides the command
@@ -38,9 +37,7 @@
 - Python Package at <https://pypi.org/project/CNFgen/>
 - Github repository <https://github.com/MassimoLauria/cnfgen>
 - Zenodo link (DOI) <https://zenodo.org/record/3548843>
 
 
 Copyright 2012-2020  © Massimo
 Lauria ([massimo.lauria@uniroma1.it](mailto:massimo.lauria@uniroma1.it))
-
-
```

### Comparing `CNFgen-0.9.1/CNFgen.egg-info/SOURCES.txt` & `CNFgen-0.9.2/CNFgen.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 cnfgen/families/graphisomorphism.py
 cnfgen/families/ordering.py
 cnfgen/families/pebbling.py
 cnfgen/families/pigeonhole.py
 cnfgen/families/pitfall.py
 cnfgen/families/ramsey.py
 cnfgen/families/randomformulas.py
+cnfgen/families/randomkxor.py
 cnfgen/families/subgraph.py
 cnfgen/families/subsetcardinality.py
 cnfgen/families/tseitin.py
 cnfgen/formula/__init__.py
 cnfgen/formula/basecnf.py
 cnfgen/formula/baseopb.py
 cnfgen/formula/cnf.py
```

### Comparing `CNFgen-0.9.1/CREDITS.org` & `CNFgen-0.9.2/CREDITS.org`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/LICENSE` & `CNFgen-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/Makefile` & `CNFgen-0.9.2/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 # The environment is based on the latest 3.8 python with is neither
 # a '-dev' nor an 'rc*' version. At least according to the list produced by
 #
 # $ pyenv install -l
 #
 DEV_DEPENDENCES:=yapf pytest pytest-datadir flake8 'python-lsp-server[all]'
 PKG_DEPENDENCES:=wheel twine keyring
-DOC_DEPENDENCES:=sphinx sphinx-autobuild numpydoc sphinx_rtd_theme
+DOC_DEPENDENCES:='sphinx<6' sphinx-autobuild numpydoc sphinx_rtd_theme sphinx-autodoc-typehints
 
 PYENV:= $(shell command -v pyenv 2> /dev/null)
 PYENV_PYVERSION:=$(shell pyenv install -l | grep '[[:space:]]3.10.[[:digit:]]*' | grep -v 'rc\|dev' | tail -1)
 
 docs: docs-install-tools $(VERSIONFILE)
 	. $(VIRTUALENV)/bin/activate && \
 	python setup.py install && \
```

### Comparing `CNFgen-0.9.1/PKG-INFO` & `CNFgen-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: CNFgen
-Version: 0.9.1
+Version: 0.9.2
 Summary: CNF formula generator
 Home-page: https://massimolauria.net/cnfgen
 Author: Massimo Lauria
 Author-email: massimo.lauria@uniroma1.it
 License: GPL-3
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CNFgen formula generator and tools
 
 This repository provides the command
@@ -38,9 +37,7 @@
 - Python Package at <https://pypi.org/project/CNFgen/>
 - Github repository <https://github.com/MassimoLauria/cnfgen>
 - Zenodo link (DOI) <https://zenodo.org/record/3548843>
 
 
 Copyright 2012-2020  © Massimo
 Lauria ([massimo.lauria@uniroma1.it](mailto:massimo.lauria@uniroma1.it))
-
-
```

### Comparing `CNFgen-0.9.1/PyPI.md` & `CNFgen-0.9.2/PyPI.md`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/README.org` & `CNFgen-0.9.2/README.org`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/__init__.py` & `CNFgen-0.9.2/cnfgen/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from cnfgen.families.pigeonhole import GraphPigeonholePrinciple
 from cnfgen.families.pigeonhole import BinaryPigeonholePrinciple
 from cnfgen.families.pigeonhole import RelativizedPigeonholePrinciple
 from cnfgen.families.ramsey import RamseyNumber
 from cnfgen.families.ramsey import PythagoreanTriples
 from cnfgen.families.ramsey import VanDerWaerden
 from cnfgen.families.randomformulas import RandomKCNF
+from cnfgen.families.randomkxor import RandomKXOR
 from cnfgen.families.subgraph import SubgraphFormula
 from cnfgen.families.subgraph import CliqueFormula
 from cnfgen.families.subgraph import BinaryCliqueFormula
 from cnfgen.families.subgraph import RamseyWitnessFormula
 from cnfgen.families.subsetcardinality import SubsetCardinalityFormula
 from cnfgen.families.tseitin import TseitinFormula
 from cnfgen.families.pitfall import PitfallFormula
```

### Comparing `CNFgen-0.9.1/cnfgen/clihelpers/counting_helpers.py` & `CNFgen-0.9.2/cnfgen/clihelpers/counting_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """Implementation of counting/matching formulas helpers
 
-Copyright (C) 2012, 2013, 2014, 2015, 2016, 2019, 2020, 2021, 2022 Massimo Lauria <massimo.lauria@uniroma1.it>
+Copyright (C) 2012, 2013, 2014, 2015, 2016, 2019, 2020, 2021, 2022, 2023 Massimo Lauria <massimo.lauria@uniroma1.it>
 https://massimolauria.net/cnfgen/
 """
 
 from cnfgen.families.counting import CountingPrinciple
 from cnfgen.families.counting import PerfectMatchingPrinciple
 from cnfgen.families.tseitin import TseitinFormula
 from cnfgen.families.subsetcardinality import SubsetCardinalityFormula
@@ -138,15 +138,17 @@
  {0} first file.dot        --- Put odd charge just on first vertex on graph in 'file.dot'
 
 positional arguments:
   <charge>       --- It can be one of the following:
                      `first'  puts odd charge on first vertex;
                      `random' puts a random charge on vertices;
                      `randomodd' puts random odd  charge on vertices;
-                     `randomeven' puts random even charge on vertices.
+                     `randomeven' puts random even charge on vertices;
+                     `zero' puts charge 0 on every vertex;
+                     `one'  puts charge 1 on every vertex.
   <graph>        --- a simple undirected graph (see 'cnfgen --help-graph')
 
 optional arguments:
   --help, -h            show this help message and exit
 """
 
 
@@ -176,20 +178,22 @@
                               action='store',
                               default=4)
 
         longform = CLIParser()
         longform.add_argument(
             'charge',
             metavar='<charge>',
-            choices=['first', 'random', 'randomodd', 'randomeven'],
+            choices=['first', 'random', 'randomodd', 'randomeven','zero','one'],
             help="""charge on the vertices.
                                     `first'  puts odd charge on first vertex;
                                     `random' puts a random charge on vertices;
                                     `randomodd' puts random odd  charge on vertices;
-                                    `randomeven' puts random even charge on vertices.
+                                    `randomeven' puts random even charge on vertices;
+                                    `zero' puts charge 0 on every vertex;
+                                    `one'  puts charge 1 on every vertex.
                                      """)
         longform.add_argument(
             'G',
             metavar='<graph>',
             help='a simple undirected graph (see \'cnfgen --help-graph\')',
             action=ObtainSimpleGraph)
 
@@ -231,14 +235,22 @@
 
             pass
 
         elif args.charge == 'first':
 
             charge = [1] + [0] * (G.order() - 1)
 
+        elif args.charge == 'zero':
+
+            charge = [0] * G.order()
+
+        elif args.charge == 'one':
+
+            charge = [1] * G.order()
+
         else:  # random vector
             charge = [random.randint(0, 1) for _ in range(G.order() - 1)]
 
             parity = sum(charge) % 2
 
             if args.charge == 'random':
                 charge.append(random.randint(0, 1))
```

### Comparing `CNFgen-0.9.1/cnfgen/clihelpers/cpls_helpers.py` & `CNFgen-0.9.2/cnfgen/clihelpers/cpls_helpers.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/clihelpers/dimacs_helpers.py` & `CNFgen-0.9.2/cnfgen/clihelpers/dimacs_helpers.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/clihelpers/formula_helpers.py` & `CNFgen-0.9.2/cnfgen/clihelpers/formula_helpers.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/clihelpers/graph_helpers.py` & `CNFgen-0.9.2/cnfgen/clihelpers/graph_helpers.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/clihelpers/ordering_helpers.py` & `CNFgen-0.9.2/cnfgen/clihelpers/ordering_helpers.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/clihelpers/pebbling_helpers.py` & `CNFgen-0.9.2/cnfgen/clihelpers/pebbling_helpers.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/clihelpers/php_helpers.py` & `CNFgen-0.9.2/cnfgen/clihelpers/php_helpers.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/clihelpers/pitfall_helpers.py` & `CNFgen-0.9.2/cnfgen/clihelpers/pitfall_helpers.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/clihelpers/simple_helpers.py` & `CNFgen-0.9.2/cnfgen/clihelpers/simple_helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """Formula Helpers for simple and random formulas
 
-Copyright (C) 2012, 2013, 2014, 2015, 2016, 2019, 2020, 2021, 2022 Massimo Lauria <massimo.lauria@uniroma1.it>
+Copyright (C) 2012, 2013, 2014, 2015, 2016, 2019, 2020, 2021, 2022, 2023 Massimo Lauria <massimo.lauria@uniroma1.it>
 https://massimolauria.net/cnfgen/
 """
 
 from cnfgen.formula.cnf import CNF
 from cnfgen.families.randomformulas import RandomKCNF
+from cnfgen.families.randomkxor import RandomKXOR
 from cnfgen.clitools import nonnegative_int, positive_int
 from .formula_helpers import FormulaHelper
 
 import random
 
 
 class OR(FormulaHelper):
@@ -207,7 +208,62 @@
                               args.n,
                               args.m,
                               planted_assignments=[planted],
                               formula_class=formula_class)
         else:
             return RandomKCNF(args.k, args.n, args.m,
                               formula_class=formula_class)
+
+class RandXorHelper(FormulaHelper):
+    """Command line helper for random formulas
+    """
+    name = 'randkxor'
+    description = 'random k-XOR'
+
+    @staticmethod
+    def setup_command_line(parser):
+        """Setup the command line options for an and of literals
+
+        Arguments:
+        - `parser`: parser to load with options.
+        """
+        parser.usage = "usage:\n {0} [-h|--help] [-p|--plant] <k> <n> <m>".format(parser.prog)
+        parser.description = """ Sample <m> parity constraints over <n> variables, each of width <k>,
+uniformly at random. The sampling is done without repetition, meaning
+that whenever a xor is already in the formula, it is never
+picked again.
+
+positional arguments:
+  <k>                  width of the parities
+  <n>                  number of variables in the formula
+  <m>                  number of sampled xors
+
+optional arguments:
+  --plant, -p          plant a random satisfying assignment (default: no)
+  --help, -h           show this help message and exit
+"""
+        parser.add_argument('k', type=positive_int)
+        parser.add_argument('n', type=positive_int)
+        parser.add_argument('m', type=nonnegative_int)
+        parser.add_argument('--plant',
+                            '-p',
+                            action='store_true',
+                            default=False)
+
+    @staticmethod
+    def build_formula(args, formula_class):
+        """Build a conjunction
+
+        Arguments:
+        - `args`: command line options
+        """
+        n = args.n
+        if args.plant:
+            planted = [random.choice([-1,1])*v for v in range(1,n+1)]
+            return RandomKXOR(args.k,
+                              args.n,
+                              args.m,
+                              planted_assignments=[planted],
+                              formula_class=formula_class)
+        else:
+            return RandomKXOR(args.k, args.n, args.m,
+                              formula_class=formula_class)
```

### Comparing `CNFgen-0.9.1/cnfgen/clihelpers/transformation_helpers.py` & `CNFgen-0.9.2/cnfgen/clihelpers/transformation_helpers.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/clitools/__init__.py` & `CNFgen-0.9.2/cnfgen/clitools/__init__.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/clitools/cmdline.py` & `CNFgen-0.9.2/cnfgen/clitools/cmdline.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/clitools/cnfgen.py` & `CNFgen-0.9.2/cnfgen/clitools/cnfgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,15 @@
     pitfall             Pitfall formula
     ptn                 Bicoloring of N with no monochromatic
                         Pythagorean Triples
     ram                 ramsey number principle
     ramlb               unsat if G witnesses that r(k,s)>|V(G)|
                         (i.e. G has neither a k-clique nor an s-stable)
     randkcnf            random k-CNF
+    randkxor            random k-XOR
     rphp                relativized pigeonhole principle
     stone               stone formula (dense and sparse)
     subgraph            subgraph formula
     subsetcard          subset cardinality formulas
     tiling              tiling formula
     true                CNF formula with no clauses
     tseitin             tseitin formula
```

### Comparing `CNFgen-0.9.1/cnfgen/clitools/cnfshuffle.py` & `CNFgen-0.9.2/cnfgen/clitools/cnfshuffle.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/clitools/graph_args.py` & `CNFgen-0.9.2/cnfgen/clitools/graph_args.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/clitools/graph_build.py` & `CNFgen-0.9.2/cnfgen/clitools/graph_build.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/clitools/graph_docs.py` & `CNFgen-0.9.2/cnfgen/clitools/graph_docs.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/clitools/graph_fileinput.py` & `CNFgen-0.9.2/cnfgen/clitools/graph_fileinput.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/clitools/kthlist2pebbling.py` & `CNFgen-0.9.2/cnfgen/clitools/kthlist2pebbling.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/clitools/msg.py` & `CNFgen-0.9.2/cnfgen/clitools/msg.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/clitools/pbgen.py` & `CNFgen-0.9.2/cnfgen/clitools/pbgen.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/families/cliquecoloring.py` & `CNFgen-0.9.2/cnfgen/families/cliquecoloring.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/families/coloring.py` & `CNFgen-0.9.2/cnfgen/families/coloring.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/families/counting.py` & `CNFgen-0.9.2/cnfgen/families/counting.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/families/cpls.py` & `CNFgen-0.9.2/cnfgen/families/cpls.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/families/dominatingset.py` & `CNFgen-0.9.2/cnfgen/families/dominatingset.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/families/graphisomorphism.py` & `CNFgen-0.9.2/cnfgen/families/graphisomorphism.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/families/ordering.py` & `CNFgen-0.9.2/cnfgen/families/ordering.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/families/pebbling.py` & `CNFgen-0.9.2/cnfgen/families/pebbling.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/families/pigeonhole.py` & `CNFgen-0.9.2/cnfgen/families/pigeonhole.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/families/pitfall.py` & `CNFgen-0.9.2/cnfgen/families/pitfall.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/families/ramsey.py` & `CNFgen-0.9.2/cnfgen/families/ramsey.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/families/randomformulas.py` & `CNFgen-0.9.2/cnfgen/families/randomformulas.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 
 def clause_satisfied(cls, assignments):
     """Test whether a clause is satisfied by all assignments
 
 Test if clauses `cls` is satisfied by all assigment in the
 list assignments.
 """
-    if assignments is None:
-        return True
     for assignment in assignments:
         for lit in cls:
             if lit in assignment:
                 break
         else:
             return False
     return True
@@ -53,30 +51,36 @@
 
         if not clause_satisfied(cls, planted_assignments):
             continue
 
         sampled.add(tcls)
         clauses.append(cls)
 
-    if len(clauses) < m:
-        return sample_clauses_dense(k, n, m, planted_assignments)
-    return clauses
+    if len(clauses) == m:
+        return clauses
+
+    # dense sampling
+    fullset = list(all_clauses(k, n, planted_assignments))
+    if len(fullset) < m:
+        if len(planted_assignments)>0:
+            raise ValueError("Not enough clauses satisfying the planted assignment")
+        else:
+            raise ValueError("Too many clauses requested")
+    return random.sample(fullset, m)
 
 
 def all_clauses(k, n, planted_assignments):
     for domain in itertools.combinations(range(1, n+1), k):
         for polarity in itertools.product([-1, 1], repeat=k):
 
             cls = [p*v for p,v in zip(polarity,domain)]
             if clause_satisfied(cls, planted_assignments):
                 yield cls
 
 
-def sample_clauses_dense(k, n, m, planted_assignments):
-    return random.sample(list(all_clauses(k, n, planted_assignments)), m)
 
 
 def RandomKCNF(k, n, m, seed=None, planted_assignments=None, formula_class=CNF):
     """Build a random k-CNF
 
     Sample :math:`m` clauses over :math:`n` variables, each of width
     :math:`k`, uniformly at random. The sampling is done without
@@ -116,22 +120,25 @@
     non_negative_int(n, 'n')
     non_negative_int(m, 'm')
     non_negative_int(k, 'k')
 
     if seed is not None:
         random.seed(seed)
 
+    if planted_assignments is None:
+        planted_assignments = []
+
     if k > n:
         raise ValueError("clauses width is {}, and we only have {} variables".format(k,n))
 
     descr = "Random {}-CNF over {} variables and {} clauses".format(k, n, m)
     F = formula_class(description=descr)
 
     F.update_variable_number(n)
     try:
         for clause in sample_clauses(k, n, m, planted_assignments):
             F.add_clause(clause, check=False)
     except ValueError:
         raise ValueError(
-            "There are fewer clauses available than the number requested")
+            "The number of clauses available is less than m")
 
     return F
```

### Comparing `CNFgen-0.9.1/cnfgen/families/subgraph.py` & `CNFgen-0.9.2/cnfgen/families/subgraph.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/families/subsetcardinality.py` & `CNFgen-0.9.2/cnfgen/families/subsetcardinality.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/families/tseitin.py` & `CNFgen-0.9.2/cnfgen/families/tseitin.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/formula/basecnf.py` & `CNFgen-0.9.2/cnfgen/formula/basecnf.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/formula/baseopb.py` & `CNFgen-0.9.2/cnfgen/formula/baseopb.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/formula/cnf.py` & `CNFgen-0.9.2/cnfgen/formula/cnf.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/formula/cnfio.py` & `CNFgen-0.9.2/cnfgen/formula/cnfio.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/formula/linear.py` & `CNFgen-0.9.2/cnfgen/formula/linear.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 This CNF formula type supports
 - linear equations mod 2
 - integer  linear inequalities on literals (no coefficients)
   for example 'atmost k'
 
 
-Copyright (C) 2021, 2022 Massimo Lauria <lauria.massimo@gmail.com>
+Copyright (C) 2021, 2022, 2023 Massimo Lauria <lauria.massimo@gmail.com>
 https://github.com/MassimoLauria/cnfgen.git
 """
 
 from functools import reduce
 from operator import mul
 from itertools import combinations
 from itertools import product
@@ -58,14 +58,22 @@
         >>> C.add_parity([-1,2],1)
         >>> list(C)
         [[-1, 2], [1, -2]]
         >>> C=CNFLinear()
         >>> C.add_parity([-1,2],0)
         >>> list(C)
         [[-1, -2], [1, 2]]
+        >>> C=CNFLinear()
+        >>> C.add_parity([1,2,3],1)
+        >>> list(C)
+        [[1, 2, 3], [1, -2, -3], [-1, 2, -3], [-1, -2, 3]]
+        >>> C=CNFLinear()
+        >>> C.add_parity([1,2,3],0)
+        >>> list(C)
+        [[1, 2, -3], [1, -2, 3], [-1, 2, 3], [-1, -2, -3]]
         """
         if isgenerator(lits):
             lits = list(lits)
         if check:
             self._check_and_update(lits)
 
         desired_sign = 1 if constant == 1 else -1
```

### Comparing `CNFgen-0.9.1/cnfgen/formula/opb.py` & `CNFgen-0.9.2/cnfgen/formula/opb.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/formula/opbio.py` & `CNFgen-0.9.2/cnfgen/formula/opbio.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,17 +86,17 @@
         --------
         >>> c=OPBio()
         >>> c.cardinality_geq([1,3,-2,4],3)
         >>> c.cardinality_eq([1,3,-2,4],3)
         >>> c.add_constraint([(2,3),(2,-1),(1,-2),">=",2])
         >>> print(c.to_latex())
         \\begin{align}
-        & {x_1} + {x_3} + {\\overline{x}_2} + {x_4} \geq 3 \\\\
+        & {x_1} + {x_3} + {\\overline{x}_2} + {x_4} \\geq 3 \\\\
         & {x_1} + {x_3} + {\\overline{x}_2} + {x_4} = 3 \\\\
-        & 2{x_3} + 2{\\overline{x}_1} + {\overline{x}_2} \geq 2
+        & 2{x_3} + 2{\\overline{x}_1} + {\\overline{x}_2} \\geq 2
         \\end{align}
 
         References
         ----------
         .. [1] http://www.latex-project.org/
         """
         return to_latex_string(self)
```

### Comparing `CNFgen-0.9.1/cnfgen/formula/variables.py` & `CNFgen-0.9.2/cnfgen/formula/variables.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/graphs.py` & `CNFgen-0.9.2/cnfgen/graphs.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/info.py` & `CNFgen-0.9.2/cnfgen/info.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/localtypes.py` & `CNFgen-0.9.2/cnfgen/localtypes.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/transformations/shuffle.py` & `CNFgen-0.9.2/cnfgen/transformations/shuffle.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/transformations/substitutions.py` & `CNFgen-0.9.2/cnfgen/transformations/substitutions.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/utils/latexoutput.py` & `CNFgen-0.9.2/cnfgen/utils/latexoutput.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/utils/opb.py` & `CNFgen-0.9.2/cnfgen/utils/opb.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/cnfgen/utils/parsedimacs.py` & `CNFgen-0.9.2/cnfgen/utils/parsedimacs.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,16 +168,15 @@
     fileorname: file object or string (or stdin if None)
         destination file given either as object or as filename"""
     if fileorname is None:
         inputfile = sys.stdin
         name = '<stdin>'
     elif isinstance(fileorname, str):
         with open(fileorname, 'r', encoding='utf-8') as filehandle:
-            from_dimacs_file(cnfclass, filehandle)
-            return
+            return from_dimacs_file(cnfclass, filehandle)
     else:
         inputfile = fileorname
         try:
             name = fileorname.name
         except AttributeError:
             name = '<unknown>'
```

### Comparing `CNFgen-0.9.1/cnfgen/utils/solver.py` & `CNFgen-0.9.2/cnfgen/utils/solver.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.1/setup.py` & `CNFgen-0.9.2/setup.py`

 * *Files identical despite different names*

