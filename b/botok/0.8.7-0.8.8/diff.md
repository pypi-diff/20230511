# Comparing `tmp/botok-0.8.7.tar.gz` & `tmp/botok-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/botok-0.8.7.tar", last modified: Mon Jun 21 18:15:39 2021, max compression
+gzip compressed data, was "botok-0.8.8.tar", last modified: Tue Oct 12 07:59:52 2021, max compression
```

## Comparing `botok-0.8.7.tar` & `botok-0.8.8.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-21 18:15:39.000000 botok-0.8.7/
--rw-r--r--   0 root         (0) root         (0)    11356 2021-06-21 18:15:31.000000 botok-0.8.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7045 2021-06-21 18:15:39.000000 botok-0.8.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6162 2021-06-21 18:15:31.000000 botok-0.8.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-21 18:15:39.000000 botok-0.8.7/botok/
--rw-r--r--   0 root         (0) root         (0)     1489 2021-06-21 18:15:31.000000 botok-0.8.7/botok/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-21 18:15:39.000000 botok-0.8.7/botok/chunks/
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-21 18:15:31.000000 botok-0.8.7/botok/chunks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15219 2021-06-21 18:15:31.000000 botok-0.8.7/botok/chunks/chunkframework.py
--rw-r--r--   0 root         (0) root         (0)     8729 2021-06-21 18:15:31.000000 botok-0.8.7/botok/chunks/chunkframeworkbase.py
--rw-r--r--   0 root         (0) root         (0)     4504 2021-06-21 18:15:31.000000 botok-0.8.7/botok/chunks/chunks.py
--rw-r--r--   0 root         (0) root         (0)     4398 2021-06-21 18:15:31.000000 botok-0.8.7/botok/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-21 18:15:39.000000 botok-0.8.7/botok/modifytokens/
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-21 18:15:31.000000 botok-0.8.7/botok/modifytokens/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4785 2021-06-21 18:15:31.000000 botok-0.8.7/botok/modifytokens/adjusttokens.py
--rw-r--r--   0 root         (0) root         (0)     1048 2021-06-21 18:15:31.000000 botok-0.8.7/botok/modifytokens/cqlmatcher.py
--rw-r--r--   0 root         (0) root         (0)     1842 2021-06-21 18:15:31.000000 botok-0.8.7/botok/modifytokens/mergedagdra.py
--rw-r--r--   0 root         (0) root         (0)     1470 2021-06-21 18:15:31.000000 botok-0.8.7/botok/modifytokens/mergingmatcher.py
--rw-r--r--   0 root         (0) root         (0)      882 2021-06-21 18:15:31.000000 botok-0.8.7/botok/modifytokens/replacingmatcher.py
--rw-r--r--   0 root         (0) root         (0)     1400 2021-06-21 18:15:31.000000 botok-0.8.7/botok/modifytokens/splitaffixed.py
--rw-r--r--   0 root         (0) root         (0)     1563 2021-06-21 18:15:31.000000 botok-0.8.7/botok/modifytokens/splittingmatcher.py
--rw-r--r--   0 root         (0) root         (0)     3189 2021-06-21 18:15:31.000000 botok-0.8.7/botok/modifytokens/tokenmerge.py
--rw-r--r--   0 root         (0) root         (0)     4414 2021-06-21 18:15:31.000000 botok-0.8.7/botok/modifytokens/tokensplit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-21 18:15:39.000000 botok-0.8.7/botok/resources/
--rw-r--r--   0 root         (0) root         (0)     1786 2021-06-21 18:15:31.000000 botok-0.8.7/botok/resources/README.md
--rw-r--r--   0 root         (0) root         (0)    16855 2021-06-21 18:15:31.000000 botok-0.8.7/botok/resources/SylComponents.json
--rw-r--r--   0 root         (0) root         (0)    16138 2021-06-21 18:15:31.000000 botok-0.8.7/botok/resources/bo_uni_table.csv
--rw-r--r--   0 root         (0) root         (0)     1597 2021-06-21 18:15:31.000000 botok-0.8.7/botok/resources/particles.tsv
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-21 18:15:39.000000 botok-0.8.7/botok/text/
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-21 18:15:31.000000 botok-0.8.7/botok/text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1087 2021-06-21 18:15:31.000000 botok-0.8.7/botok/text/format.py
--rw-r--r--   0 root         (0) root         (0)     2503 2021-06-21 18:15:31.000000 botok-0.8.7/botok/text/modify.py
--rw-r--r--   0 root         (0) root         (0)     3477 2021-06-21 18:15:31.000000 botok-0.8.7/botok/text/pipelinebase.py
--rw-r--r--   0 root         (0) root         (0)      301 2021-06-21 18:15:31.000000 botok-0.8.7/botok/text/preprocess.py
--rw-r--r--   0 root         (0) root         (0)     5473 2021-06-21 18:15:31.000000 botok-0.8.7/botok/text/text.py
--rw-r--r--   0 root         (0) root         (0)     1288 2021-06-21 18:15:31.000000 botok-0.8.7/botok/text/tokenize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-21 18:15:39.000000 botok-0.8.7/botok/textunits/
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-21 18:15:31.000000 botok-0.8.7/botok/textunits/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4714 2021-06-21 18:15:31.000000 botok-0.8.7/botok/textunits/bostring.py
--rw-r--r--   0 root         (0) root         (0)     1849 2021-06-21 18:15:31.000000 botok-0.8.7/botok/textunits/bosyl.py
--rw-r--r--   0 root         (0) root         (0)     2420 2021-06-21 18:15:31.000000 botok-0.8.7/botok/textunits/charcategories.py
--rw-r--r--   0 root         (0) root         (0)     7883 2021-06-21 18:15:31.000000 botok-0.8.7/botok/textunits/sylcomponents.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-21 18:15:39.000000 botok-0.8.7/botok/third_party/
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-21 18:15:31.000000 botok-0.8.7/botok/third_party/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2435 2021-06-21 18:15:31.000000 botok-0.8.7/botok/third_party/cqlparser.py
--rw-r--r--   0 root         (0) root         (0)     1414 2021-06-21 18:15:31.000000 botok-0.8.7/botok/third_party/has_skrt_syl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-21 18:15:39.000000 botok-0.8.7/botok/third_party/pynpl/
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-21 18:15:31.000000 botok-0.8.7/botok/third_party/pynpl/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8956 2021-06-21 18:15:31.000000 botok-0.8.7/botok/third_party/pynpl/cql.py
--rw-r--r--   0 root         (0) root         (0)     3796 2021-06-21 18:15:31.000000 botok-0.8.7/botok/third_party/pynpl/fsa.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-21 18:15:39.000000 botok-0.8.7/botok/tokenizers/
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-21 18:15:31.000000 botok-0.8.7/botok/tokenizers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      255 2021-06-21 18:15:31.000000 botok-0.8.7/botok/tokenizers/chunktokenizer.py
--rw-r--r--   0 root         (0) root         (0)     1081 2021-06-21 18:15:31.000000 botok-0.8.7/botok/tokenizers/paragraphtokenizer.py
--rw-r--r--   0 root         (0) root         (0)     7517 2021-06-21 18:15:31.000000 botok-0.8.7/botok/tokenizers/sentencetokenizer.py
--rw-r--r--   0 root         (0) root         (0)     4890 2021-06-21 18:15:31.000000 botok-0.8.7/botok/tokenizers/token.py
--rw-r--r--   0 root         (0) root         (0)    10554 2021-06-21 18:15:31.000000 botok-0.8.7/botok/tokenizers/tokenize.py
--rw-r--r--   0 root         (0) root         (0)     5191 2021-06-21 18:15:31.000000 botok-0.8.7/botok/tokenizers/wordtokenizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-21 18:15:39.000000 botok-0.8.7/botok/tries/
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-21 18:15:31.000000 botok-0.8.7/botok/tries/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4985 2021-06-21 18:15:31.000000 botok-0.8.7/botok/tries/basictrie.py
--rw-r--r--   0 root         (0) root         (0)     7499 2021-06-21 18:15:31.000000 botok-0.8.7/botok/tries/trie.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-21 18:15:39.000000 botok-0.8.7/botok/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-21 18:15:31.000000 botok-0.8.7/botok/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1136 2021-06-21 18:15:31.000000 botok-0.8.7/botok/utils/expose_data.py
--rw-r--r--   0 root         (0) root         (0)      143 2021-06-21 18:15:31.000000 botok-0.8.7/botok/utils/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1536 2021-06-21 18:15:31.000000 botok-0.8.7/botok/vars.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-21 18:15:39.000000 botok-0.8.7/botok.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7045 2021-06-21 18:15:39.000000 botok-0.8.7/botok.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1764 2021-06-21 18:15:39.000000 botok-0.8.7/botok.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-06-21 18:15:39.000000 botok-0.8.7/botok.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2021-06-21 18:15:39.000000 botok-0.8.7/botok.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2021-06-21 18:15:39.000000 botok-0.8.7/botok.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      246 2021-06-21 18:15:39.000000 botok-0.8.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2138 2021-06-21 18:15:31.000000 botok-0.8.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-21 18:15:39.000000 botok-0.8.7/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-21 18:15:31.000000 botok-0.8.7/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      373 2021-06-21 18:15:31.000000 botok-0.8.7/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     7168 2021-06-21 18:15:31.000000 botok-0.8.7/tests/test_bugs.py
--rw-r--r--   0 root         (0) root         (0)     1855 2021-06-21 18:15:31.000000 botok-0.8.7/tests/test_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 07:59:52.775587 botok-0.8.8/
+-rw-r--r--   0 root         (0) root         (0)    11356 2021-10-12 07:59:50.000000 botok-0.8.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7045 2021-10-12 07:59:52.775587 botok-0.8.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6162 2021-10-12 07:59:50.000000 botok-0.8.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 07:59:52.767587 botok-0.8.8/botok/
+-rw-r--r--   0 root         (0) root         (0)     1489 2021-10-12 07:59:50.000000 botok-0.8.8/botok/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 07:59:52.771587 botok-0.8.8/botok/chunks/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-10-12 07:59:50.000000 botok-0.8.8/botok/chunks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15219 2021-10-12 07:59:50.000000 botok-0.8.8/botok/chunks/chunkframework.py
+-rw-r--r--   0 root         (0) root         (0)     8729 2021-10-12 07:59:50.000000 botok-0.8.8/botok/chunks/chunkframeworkbase.py
+-rw-r--r--   0 root         (0) root         (0)     4504 2021-10-12 07:59:50.000000 botok-0.8.8/botok/chunks/chunks.py
+-rw-r--r--   0 root         (0) root         (0)     4398 2021-10-12 07:59:50.000000 botok-0.8.8/botok/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 07:59:52.771587 botok-0.8.8/botok/modifytokens/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-10-12 07:59:50.000000 botok-0.8.8/botok/modifytokens/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4785 2021-10-12 07:59:50.000000 botok-0.8.8/botok/modifytokens/adjusttokens.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2021-10-12 07:59:50.000000 botok-0.8.8/botok/modifytokens/cqlmatcher.py
+-rw-r--r--   0 root         (0) root         (0)     1842 2021-10-12 07:59:50.000000 botok-0.8.8/botok/modifytokens/mergedagdra.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2021-10-12 07:59:50.000000 botok-0.8.8/botok/modifytokens/mergingmatcher.py
+-rw-r--r--   0 root         (0) root         (0)      882 2021-10-12 07:59:50.000000 botok-0.8.8/botok/modifytokens/replacingmatcher.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2021-10-12 07:59:50.000000 botok-0.8.8/botok/modifytokens/splitaffixed.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2021-10-12 07:59:50.000000 botok-0.8.8/botok/modifytokens/splittingmatcher.py
+-rw-r--r--   0 root         (0) root         (0)     3189 2021-10-12 07:59:50.000000 botok-0.8.8/botok/modifytokens/tokenmerge.py
+-rw-r--r--   0 root         (0) root         (0)     4414 2021-10-12 07:59:50.000000 botok-0.8.8/botok/modifytokens/tokensplit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 07:59:52.771587 botok-0.8.8/botok/resources/
+-rw-r--r--   0 root         (0) root         (0)     1786 2021-10-12 07:59:50.000000 botok-0.8.8/botok/resources/README.md
+-rw-r--r--   0 root         (0) root         (0)    16855 2021-10-12 07:59:50.000000 botok-0.8.8/botok/resources/SylComponents.json
+-rw-r--r--   0 root         (0) root         (0)    16138 2021-10-12 07:59:50.000000 botok-0.8.8/botok/resources/bo_uni_table.csv
+-rw-r--r--   0 root         (0) root         (0)     1597 2021-10-12 07:59:50.000000 botok-0.8.8/botok/resources/particles.tsv
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 07:59:52.771587 botok-0.8.8/botok/text/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-10-12 07:59:50.000000 botok-0.8.8/botok/text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2021-10-12 07:59:50.000000 botok-0.8.8/botok/text/format.py
+-rw-r--r--   0 root         (0) root         (0)     2503 2021-10-12 07:59:50.000000 botok-0.8.8/botok/text/modify.py
+-rw-r--r--   0 root         (0) root         (0)     3477 2021-10-12 07:59:50.000000 botok-0.8.8/botok/text/pipelinebase.py
+-rw-r--r--   0 root         (0) root         (0)      301 2021-10-12 07:59:50.000000 botok-0.8.8/botok/text/preprocess.py
+-rw-r--r--   0 root         (0) root         (0)     5473 2021-10-12 07:59:50.000000 botok-0.8.8/botok/text/text.py
+-rw-r--r--   0 root         (0) root         (0)     1288 2021-10-12 07:59:50.000000 botok-0.8.8/botok/text/tokenize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 07:59:52.775587 botok-0.8.8/botok/textunits/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-10-12 07:59:50.000000 botok-0.8.8/botok/textunits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4714 2021-10-12 07:59:50.000000 botok-0.8.8/botok/textunits/bostring.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2021-10-12 07:59:50.000000 botok-0.8.8/botok/textunits/bosyl.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2021-10-12 07:59:50.000000 botok-0.8.8/botok/textunits/charcategories.py
+-rw-r--r--   0 root         (0) root         (0)     7883 2021-10-12 07:59:50.000000 botok-0.8.8/botok/textunits/sylcomponents.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 07:59:52.775587 botok-0.8.8/botok/third_party/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-10-12 07:59:50.000000 botok-0.8.8/botok/third_party/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2435 2021-10-12 07:59:50.000000 botok-0.8.8/botok/third_party/cqlparser.py
+-rw-r--r--   0 root         (0) root         (0)     1414 2021-10-12 07:59:50.000000 botok-0.8.8/botok/third_party/has_skrt_syl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 07:59:52.775587 botok-0.8.8/botok/third_party/pynpl/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-10-12 07:59:50.000000 botok-0.8.8/botok/third_party/pynpl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8956 2021-10-12 07:59:50.000000 botok-0.8.8/botok/third_party/pynpl/cql.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2021-10-12 07:59:50.000000 botok-0.8.8/botok/third_party/pynpl/fsa.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 07:59:52.775587 botok-0.8.8/botok/tokenizers/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-10-12 07:59:50.000000 botok-0.8.8/botok/tokenizers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      255 2021-10-12 07:59:50.000000 botok-0.8.8/botok/tokenizers/chunktokenizer.py
+-rw-r--r--   0 root         (0) root         (0)     1081 2021-10-12 07:59:50.000000 botok-0.8.8/botok/tokenizers/paragraphtokenizer.py
+-rw-r--r--   0 root         (0) root         (0)     8955 2021-10-12 07:59:50.000000 botok-0.8.8/botok/tokenizers/sentencetokenizer.py
+-rw-r--r--   0 root         (0) root         (0)     4890 2021-10-12 07:59:50.000000 botok-0.8.8/botok/tokenizers/token.py
+-rw-r--r--   0 root         (0) root         (0)    10554 2021-10-12 07:59:50.000000 botok-0.8.8/botok/tokenizers/tokenize.py
+-rw-r--r--   0 root         (0) root         (0)     5191 2021-10-12 07:59:50.000000 botok-0.8.8/botok/tokenizers/wordtokenizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 07:59:52.775587 botok-0.8.8/botok/tries/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-10-12 07:59:50.000000 botok-0.8.8/botok/tries/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4985 2021-10-12 07:59:50.000000 botok-0.8.8/botok/tries/basictrie.py
+-rw-r--r--   0 root         (0) root         (0)     7499 2021-10-12 07:59:50.000000 botok-0.8.8/botok/tries/trie.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 07:59:52.775587 botok-0.8.8/botok/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-10-12 07:59:50.000000 botok-0.8.8/botok/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1136 2021-10-12 07:59:50.000000 botok-0.8.8/botok/utils/expose_data.py
+-rw-r--r--   0 root         (0) root         (0)      143 2021-10-12 07:59:50.000000 botok-0.8.8/botok/utils/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2021-10-12 07:59:50.000000 botok-0.8.8/botok/vars.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 07:59:52.771587 botok-0.8.8/botok.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7045 2021-10-12 07:59:52.000000 botok-0.8.8/botok.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1764 2021-10-12 07:59:52.000000 botok-0.8.8/botok.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-10-12 07:59:52.000000 botok-0.8.8/botok.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2021-10-12 07:59:52.000000 botok-0.8.8/botok.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2021-10-12 07:59:52.000000 botok-0.8.8/botok.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      246 2021-10-12 07:59:52.779587 botok-0.8.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2138 2021-10-12 07:59:50.000000 botok-0.8.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-12 07:59:52.775587 botok-0.8.8/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-10-12 07:59:50.000000 botok-0.8.8/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      373 2021-10-12 07:59:50.000000 botok-0.8.8/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     7168 2021-10-12 07:59:50.000000 botok-0.8.8/tests/test_bugs.py
+-rw-r--r--   0 root         (0) root         (0)     1855 2021-10-12 07:59:50.000000 botok-0.8.8/tests/test_config.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `botok-0.8.7/LICENSE` & `botok-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/PKG-INFO` & `botok-0.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botok
-Version: 0.8.7
+Version: 0.8.8
 Summary: Tibetan Word Tokenizer
 Home-page: https://github.com/Esukhia/botok
 Author: Esukhia development team
 Author-email: esukhiadev@gmail.com
 License: Apache2
 Project-URL: Source, https://github.com/Esukhia/botok
 Project-URL: Tracker, https://github.com/Esukhia/botok/issues
```

### Comparing `botok-0.8.7/README.md` & `botok-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/__init__.py` & `botok-0.8.8/botok/__init__.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/chunks/chunkframework.py` & `botok-0.8.8/botok/chunks/chunkframework.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/chunks/chunkframeworkbase.py` & `botok-0.8.8/botok/chunks/chunkframeworkbase.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/chunks/chunks.py` & `botok-0.8.8/botok/chunks/chunks.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/config.py` & `botok-0.8.8/botok/config.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/modifytokens/adjusttokens.py` & `botok-0.8.8/botok/modifytokens/adjusttokens.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/modifytokens/cqlmatcher.py` & `botok-0.8.8/botok/modifytokens/cqlmatcher.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/modifytokens/mergedagdra.py` & `botok-0.8.8/botok/modifytokens/mergedagdra.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/modifytokens/mergingmatcher.py` & `botok-0.8.8/botok/modifytokens/mergingmatcher.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/modifytokens/replacingmatcher.py` & `botok-0.8.8/botok/modifytokens/replacingmatcher.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/modifytokens/splitaffixed.py` & `botok-0.8.8/botok/modifytokens/splitaffixed.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/modifytokens/splittingmatcher.py` & `botok-0.8.8/botok/modifytokens/splittingmatcher.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/modifytokens/tokenmerge.py` & `botok-0.8.8/botok/modifytokens/tokenmerge.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/modifytokens/tokensplit.py` & `botok-0.8.8/botok/modifytokens/tokensplit.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/resources/README.md` & `botok-0.8.8/botok/resources/README.md`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/resources/SylComponents.json` & `botok-0.8.8/botok/resources/SylComponents.json`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/resources/bo_uni_table.csv` & `botok-0.8.8/botok/resources/bo_uni_table.csv`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/resources/particles.tsv` & `botok-0.8.8/botok/resources/particles.tsv`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/text/format.py` & `botok-0.8.8/botok/text/format.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/text/modify.py` & `botok-0.8.8/botok/text/modify.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/text/pipelinebase.py` & `botok-0.8.8/botok/text/pipelinebase.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/text/text.py` & `botok-0.8.8/botok/text/text.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/text/tokenize.py` & `botok-0.8.8/botok/text/tokenize.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/textunits/bostring.py` & `botok-0.8.8/botok/textunits/bostring.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/textunits/bosyl.py` & `botok-0.8.8/botok/textunits/bosyl.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/textunits/charcategories.py` & `botok-0.8.8/botok/textunits/charcategories.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/textunits/sylcomponents.py` & `botok-0.8.8/botok/textunits/sylcomponents.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/third_party/cqlparser.py` & `botok-0.8.8/botok/third_party/cqlparser.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/third_party/has_skrt_syl.py` & `botok-0.8.8/botok/third_party/has_skrt_syl.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/third_party/pynpl/cql.py` & `botok-0.8.8/botok/third_party/pynpl/cql.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/third_party/pynpl/fsa.py` & `botok-0.8.8/botok/third_party/pynpl/fsa.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/tokenizers/paragraphtokenizer.py` & `botok-0.8.8/botok/tokenizers/paragraphtokenizer.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/tokenizers/sentencetokenizer.py` & `botok-0.8.8/botok/tokenizers/sentencetokenizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding: utf8
-
+import re
 # variables used in the tests
 ending_particles = [
     "གོ་",
     "ངོ་",
     "དོ་",
     "ནོ་",
     "བོ་",
@@ -30,25 +30,55 @@
     "སྟེ་",
     "ཏེ་",
     "དེ་",
 ]  # separated because these seem to cut long sentences
 clause_boundaries = te_particles + ["ནས་", "ན་"]
 dagdra = ["པ་", "བ་", "པོ་", "བོ་"]
 
+normalization_patterns = [(' <utt>', ''),
+            ('༑', '།'), 
+            ('\s\s+', ' '), 
+            ('ln\d ', ''), 
+            ('([^༅།་ ]) །', '\g<1>་ །'), 
+            ('༅ །', '༅།'), 
+            ('([^་།\d] )', '\g<1>-'), 
+            ('([\s\n་།][གདབམའ][ཀཁགངཅཆཇཉཊཋཌཎཏཐདནཔཕབམཙཚཛཝཞཟའཡརལཤཥསཧཨཪ]) ', '\g<1>འ་ '), 
+            ('([^་།])\s-', '\g<1>་ -'), 
+            ('ཁྱད་པ་ -ར་', 'ཁྱད་པར་'), 
+            ('སངས་ རྒྱ་ -ས་', 'སངས་རྒྱས་'), 
+            ('བྱང་ཆུབ་སེམས་ དཔའ་', 'བྱང་ཆུབ་སེམས་དཔའ་'), 
+            ('ལ་ -ས་', 'ལས་'),
+            ('༌་', '་')]
+
+def get_normalized_sentence(tokens):
+    sentence = ''
+    for token in tokens:
+        sentence += f'{token.text} '
+    sentence = sentence.strip()
+    normalized_sentence = sentence
+    for pattern in normalization_patterns:
+        normalized_sentence = re.sub(pattern[0], pattern[1], normalized_sentence)
+    return normalized_sentence
 
 # Turn sentences as indices into sentences as follows:
-# (<sent_length>, [token1, token2, ..., tokenn]) where tokens are Token objects
+# { 'length':<sent_length>, 'tokens':[token1, token2, ..., tokenn], 'norm_sent':<normalized sentence>} where tokens are Token objects
 ############################################################
 def sentence_tokenizer(tokens):
     sent_indices = get_sentence_indices(tokens)
-    # get tokens for each sentence
     sentences = []
     for sentence in sent_indices:
+        cur_sentence = {}
         start, end, l = sentence["start"], sentence["end"], sentence["len"]
-        sentences.append((l, tokens[start : end + 1]))
+        norm_sentence = get_normalized_sentence(tokens[start : end + 1])
+        cur_sentence = {
+            'length': l,
+            'tokens': tokens[start : end + 1],
+            'norm_sent': norm_sentence
+        }
+        sentences.append(cur_sentence)
 
     return sentences
 
 
 # Get sentences in the form of indices
 ############################################################
 def get_sentence_indices(tokens):
```

### Comparing `botok-0.8.7/botok/tokenizers/token.py` & `botok-0.8.8/botok/tokenizers/token.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/tokenizers/tokenize.py` & `botok-0.8.8/botok/tokenizers/tokenize.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/tokenizers/wordtokenizer.py` & `botok-0.8.8/botok/tokenizers/wordtokenizer.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/tries/basictrie.py` & `botok-0.8.8/botok/tries/basictrie.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/tries/trie.py` & `botok-0.8.8/botok/tries/trie.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/utils/expose_data.py` & `botok-0.8.8/botok/utils/expose_data.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/botok/vars.py` & `botok-0.8.8/botok/vars.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 from enum import Enum, IntEnum
 
-__version__ = "0.8.7"
+__version__ = "0.8.8"
 
 NO_POS = "NOPOS"
 TSEK = "་"
 NAMCHE = "ཿ"
 SHAD = "།"
 AA = "འ"
 HASH = "#"
```

### Comparing `botok-0.8.7/botok.egg-info/PKG-INFO` & `botok-0.8.8/botok.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botok
-Version: 0.8.7
+Version: 0.8.8
 Summary: Tibetan Word Tokenizer
 Home-page: https://github.com/Esukhia/botok
 Author: Esukhia development team
 Author-email: esukhiadev@gmail.com
 License: Apache2
 Project-URL: Source, https://github.com/Esukhia/botok
 Project-URL: Tracker, https://github.com/Esukhia/botok/issues
```

### Comparing `botok-0.8.7/botok.egg-info/SOURCES.txt` & `botok-0.8.8/botok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/setup.py` & `botok-0.8.8/setup.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/tests/test_bugs.py` & `botok-0.8.8/tests/test_bugs.py`

 * *Files identical despite different names*

### Comparing `botok-0.8.7/tests/test_config.py` & `botok-0.8.8/tests/test_config.py`

 * *Files identical despite different names*

