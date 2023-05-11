# Comparing `tmp/eis1600-0.8.9.tar.gz` & `tmp/eis1600-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis1600-0.8.9.tar", last modified: Thu May  4 09:07:22 2023, max compression
+gzip compressed data, was "eis1600-0.9.0.tar", last modified: Thu May 11 10:51:08 2023, max compression
```

## Comparing `eis1600-0.8.9.tar` & `eis1600-0.9.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.117847 eis1600-0.8.9/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.8.9/LICENSE
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7956 2023-05-04 09:07:22.117847 eis1600-0.8.9/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5895 2023-04-13 08:22:59.000000 eis1600-0.8.9/README.md
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.105847 eis1600-0.8.9/eis1600/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.8.9/eis1600/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.105847 eis1600-0.8.9/eis1600/dates/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.8.9/eis1600/dates/Date.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.9/eis1600/dates/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5856 2023-04-06 11:34:18.000000 eis1600-0.8.9/eis1600/dates/date_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3924 2023-04-12 06:44:26.000000 eis1600-0.8.9/eis1600/dates/methods.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.105847 eis1600-0.8.9/eis1600/gazetteers/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4225 2023-04-14 12:34:00.000000 eis1600-0.8.9/eis1600/gazetteers/Onomastics.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5679 2023-05-04 09:06:11.000000 eis1600-0.8.9/eis1600/gazetteers/Toponyms.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.8.9/eis1600/gazetteers/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.109847 eis1600-0.8.9/eis1600/gazetteers/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.9/eis1600/gazetteers/data/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    96536 2023-04-17 09:44:13.000000 eis1600-0.8.9/eis1600/gazetteers/data/onomastic_gazetteer.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      482 2023-03-23 10:19:45.000000 eis1600-0.8.9/eis1600/gazetteers/data/regions_gazetteer.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1307 2023-04-03 09:19:01.000000 eis1600-0.8.9/eis1600/gazetteers/data/spelling_gazetteer.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)   218682 2023-04-27 07:51:31.000000 eis1600-0.8.9/eis1600/gazetteers/data/toponyms.csv
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.109847 eis1600-0.8.9/eis1600/helper/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      730 2023-04-27 07:54:20.000000 eis1600-0.8.9/eis1600/helper/EntityTags.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-24 10:02:09.000000 eis1600-0.8.9/eis1600/helper/Singleton.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.8.9/eis1600/helper/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.8.9/eis1600/helper/ar_normalization.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.113847 eis1600-0.8.9/eis1600/helper/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.8.9/eis1600/helper/data/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      256 2023-04-19 13:02:11.000000 eis1600-0.8.9/eis1600/helper/data/entity_tags.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1237 2023-04-12 06:44:26.000000 eis1600-0.8.9/eis1600/helper/fix_miu_annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      365 2023-03-31 11:03:40.000000 eis1600-0.8.9/eis1600/helper/logging.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      637 2023-04-06 09:28:14.000000 eis1600-0.8.9/eis1600/helper/markdown_methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3739 2023-04-20 08:46:34.000000 eis1600-0.8.9/eis1600/helper/markdown_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.8.9/eis1600/helper/miu_random_revisions.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10796 2023-04-05 11:18:46.000000 eis1600-0.8.9/eis1600/helper/repo.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      598 2023-04-26 15:20:40.000000 eis1600-0.8.9/eis1600/helper/yml_methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1291 2023-05-04 08:45:34.000000 eis1600-0.8.9/eis1600/helper/yml_to_json.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.113847 eis1600-0.8.9/eis1600/markdown/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.8.9/eis1600/markdown/UIDs.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.8.9/eis1600/markdown/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4794 2023-02-23 07:56:48.000000 eis1600-0.8.9/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4574 2023-02-23 07:56:48.000000 eis1600-0.8.9/eis1600/markdown/insert_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    12991 2023-05-04 08:54:08.000000 eis1600-0.8.9/eis1600/markdown/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2856 2023-02-23 07:56:48.000000 eis1600-0.8.9/eis1600/markdown/update_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5284 2023-04-05 08:21:34.000000 eis1600-0.8.9/eis1600/markdown/update_uids_old_process.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.113847 eis1600-0.8.9/eis1600/miu/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3484 2023-04-12 15:29:30.000000 eis1600-0.8.9/eis1600/miu/HeadingTracker.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8773 2023-05-04 08:45:34.000000 eis1600-0.8.9/eis1600/miu/YAMLHandler.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.8.9/eis1600/miu/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2715 2023-02-23 07:39:16.000000 eis1600-0.8.9/eis1600/miu/disassemble_into_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8907 2023-04-12 06:50:23.000000 eis1600-0.8.9/eis1600/miu/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2590 2022-11-21 11:57:36.000000 eis1600-0.8.9/eis1600/miu/reassemble_from_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6985 2023-05-04 08:45:34.000000 eis1600-0.8.9/eis1600/miu/yml_handling.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.117847 eis1600-0.8.9/eis1600/nlp/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.8.9/eis1600/nlp/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2017 2023-03-31 12:22:46.000000 eis1600-0.8.9/eis1600/nlp/cameltools.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3672 2023-03-31 11:52:32.000000 eis1600-0.8.9/eis1600/nlp/ner_annotate_mius.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2726 2023-04-05 11:18:46.000000 eis1600-0.8.9/eis1600/nlp/utils.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.117847 eis1600-0.8.9/eis1600/onomastics/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.8.9/eis1600/onomastics/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1596 2023-04-28 07:44:42.000000 eis1600-0.8.9/eis1600/onomastics/annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10489 2023-05-04 08:54:08.000000 eis1600-0.8.9/eis1600/onomastics/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.8.9/eis1600/onomastics/re_pattern.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.117847 eis1600-0.8.9/eis1600/processing/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.9/eis1600/processing/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4660 2023-04-12 08:23:03.000000 eis1600-0.8.9/eis1600/processing/postprocessing.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4604 2023-04-21 13:13:53.000000 eis1600-0.8.9/eis1600/processing/preprocessing.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.117847 eis1600-0.8.9/eis1600/stats/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.8.9/eis1600/stats/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.8.9/eis1600/stats/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.8.9/eis1600/stats/miu_stats.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-04 09:07:22.105847 eis1600-0.8.9/eis1600.egg-info/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7956 2023-05-04 09:07:22.000000 eis1600-0.8.9/eis1600.egg-info/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1959 2023-05-04 09:07:22.000000 eis1600-0.8.9/eis1600.egg-info/SOURCES.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-05-04 09:07:22.000000 eis1600-0.8.9/eis1600.egg-info/dependency_links.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      746 2023-05-04 09:07:22.000000 eis1600-0.8.9/eis1600.egg-info/entry_points.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       83 2023-05-04 09:07:22.000000 eis1600-0.8.9/eis1600.egg-info/requires.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-05-04 09:07:22.000000 eis1600-0.8.9/eis1600.egg-info/top_level.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-05-04 09:07:22.117847 eis1600-0.8.9/setup.cfg
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2297 2023-05-04 09:04:19.000000 eis1600-0.8.9/setup.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.308791 eis1600-0.9.0/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.9.0/LICENSE
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10053 2023-05-11 10:51:08.308791 eis1600-0.9.0/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7640 2023-05-11 10:42:54.000000 eis1600-0.9.0/README.md
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.296791 eis1600-0.9.0/eis1600/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.9.0/eis1600/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.300792 eis1600-0.9.0/eis1600/dates/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.9.0/eis1600/dates/Date.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.0/eis1600/dates/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5856 2023-04-06 11:34:18.000000 eis1600-0.9.0/eis1600/dates/date_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3924 2023-04-12 06:44:26.000000 eis1600-0.9.0/eis1600/dates/methods.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.300792 eis1600-0.9.0/eis1600/gazetteers/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4225 2023-04-14 12:34:00.000000 eis1600-0.9.0/eis1600/gazetteers/Onomastics.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5877 2023-05-05 07:34:23.000000 eis1600-0.9.0/eis1600/gazetteers/Toponyms.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.9.0/eis1600/gazetteers/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.300792 eis1600-0.9.0/eis1600/gazetteers/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.0/eis1600/gazetteers/data/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    96536 2023-04-17 09:44:13.000000 eis1600-0.9.0/eis1600/gazetteers/data/onomastic_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      482 2023-03-23 10:19:45.000000 eis1600-0.9.0/eis1600/gazetteers/data/regions_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1307 2023-04-03 09:19:01.000000 eis1600-0.9.0/eis1600/gazetteers/data/spelling_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)   218682 2023-04-27 07:51:31.000000 eis1600-0.9.0/eis1600/gazetteers/data/toponyms.csv
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.304792 eis1600-0.9.0/eis1600/helper/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      730 2023-04-27 07:54:20.000000 eis1600-0.9.0/eis1600/helper/EntityTags.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-24 10:02:09.000000 eis1600-0.9.0/eis1600/helper/Singleton.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.9.0/eis1600/helper/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.9.0/eis1600/helper/ar_normalization.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.304792 eis1600-0.9.0/eis1600/helper/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.9.0/eis1600/helper/data/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      256 2023-04-19 13:02:11.000000 eis1600-0.9.0/eis1600/helper/data/entity_tags.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1237 2023-04-12 06:44:26.000000 eis1600-0.9.0/eis1600/helper/fix_miu_annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      365 2023-03-31 11:03:40.000000 eis1600-0.9.0/eis1600/helper/logging.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      707 2023-05-10 14:33:13.000000 eis1600-0.9.0/eis1600/helper/markdown_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3739 2023-04-20 08:46:34.000000 eis1600-0.9.0/eis1600/helper/markdown_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.9.0/eis1600/helper/miu_random_revisions.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    11231 2023-05-11 10:42:54.000000 eis1600-0.9.0/eis1600/helper/repo.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      598 2023-04-26 15:20:40.000000 eis1600-0.9.0/eis1600/helper/yml_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1335 2023-05-11 10:36:39.000000 eis1600-0.9.0/eis1600/helper/yml_to_json.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.304792 eis1600-0.9.0/eis1600/markdown/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.9.0/eis1600/markdown/UIDs.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.9.0/eis1600/markdown/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4794 2023-02-23 07:56:48.000000 eis1600-0.9.0/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4574 2023-02-23 07:56:48.000000 eis1600-0.9.0/eis1600/markdown/insert_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    12991 2023-05-04 08:54:08.000000 eis1600-0.9.0/eis1600/markdown/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2856 2023-02-23 07:56:48.000000 eis1600-0.9.0/eis1600/markdown/update_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5284 2023-04-05 08:21:34.000000 eis1600-0.9.0/eis1600/markdown/update_uids_old_process.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.304792 eis1600-0.9.0/eis1600/miu/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3484 2023-04-12 15:29:30.000000 eis1600-0.9.0/eis1600/miu/HeadingTracker.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8819 2023-05-10 14:51:01.000000 eis1600-0.9.0/eis1600/miu/YAMLHandler.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.9.0/eis1600/miu/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2778 2023-05-11 10:36:39.000000 eis1600-0.9.0/eis1600/miu/disassemble_into_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8907 2023-04-12 06:50:23.000000 eis1600-0.9.0/eis1600/miu/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2590 2022-11-21 11:57:36.000000 eis1600-0.9.0/eis1600/miu/reassemble_from_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7584 2023-05-10 14:48:27.000000 eis1600-0.9.0/eis1600/miu/yml_handling.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.308791 eis1600-0.9.0/eis1600/nlp/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.9.0/eis1600/nlp/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2017 2023-03-31 12:22:46.000000 eis1600-0.9.0/eis1600/nlp/cameltools.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3682 2023-05-11 10:36:39.000000 eis1600-0.9.0/eis1600/nlp/ner_annotate_mius.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2726 2023-04-05 11:18:46.000000 eis1600-0.9.0/eis1600/nlp/utils.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.308791 eis1600-0.9.0/eis1600/onomastics/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.9.0/eis1600/onomastics/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1663 2023-05-11 10:36:39.000000 eis1600-0.9.0/eis1600/onomastics/annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10489 2023-05-04 08:54:08.000000 eis1600-0.9.0/eis1600/onomastics/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.9.0/eis1600/onomastics/re_pattern.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.308791 eis1600-0.9.0/eis1600/processing/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.0/eis1600/processing/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4660 2023-04-12 08:23:03.000000 eis1600-0.9.0/eis1600/processing/postprocessing.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4604 2023-04-21 13:13:53.000000 eis1600-0.9.0/eis1600/processing/preprocessing.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.308791 eis1600-0.9.0/eis1600/stats/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.9.0/eis1600/stats/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.9.0/eis1600/stats/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.9.0/eis1600/stats/miu_stats.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-05-11 10:51:08.300792 eis1600-0.9.0/eis1600.egg-info/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10053 2023-05-11 10:51:08.000000 eis1600-0.9.0/eis1600.egg-info/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1959 2023-05-11 10:51:08.000000 eis1600-0.9.0/eis1600.egg-info/SOURCES.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-05-11 10:51:08.000000 eis1600-0.9.0/eis1600.egg-info/dependency_links.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      746 2023-05-11 10:51:08.000000 eis1600-0.9.0/eis1600.egg-info/entry_points.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       83 2023-05-11 10:51:08.000000 eis1600-0.9.0/eis1600.egg-info/requires.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-05-11 10:51:08.000000 eis1600-0.9.0/eis1600.egg-info/top_level.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-05-11 10:51:08.308791 eis1600-0.9.0/setup.cfg
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2297 2023-05-11 10:50:52.000000 eis1600-0.9.0/setup.py
```

### Comparing `eis1600-0.8.9/LICENSE` & `eis1600-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/PKG-INFO` & `eis1600-0.9.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,33 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.8.9
+Version: 0.9.0
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
         
+        * [Workflow](#workflow)
+        * [Process](#process)
+        * [Installation](#installation)
+        * [Set Up](#set-up-virtual-environment-and-install-the-eis1600-pkg-there)
+        * [Working Directory Structure](#structure-of-the-working-directory)
+        * [Usage](#usage)
+          * [convert_mARkdown_to_EIS1600TMP](#convert-markdown-to-eis1600-files)
+          * [insert_uids](#convert-markdown-to-eis1600-files)
+          * [update_uids](#convert-markdown-to-eis1600-files)
+          * [disassemble_into_miu_files](#disassembling)
+          * [reassble-from-miu_files](#reassembling)
+          * [annotate_mius](#annotation)
+          * [onomastic_annotation](#only-onomastic-annotation)
+          * [miu_random_revision](#miu-revision)
+          * [yml_to_json](#collect-yamlheaders-into-json)
+        
         ## Workflow
         
         (*so that we do not forget again...*)
         
         1. Double-check text in the Google Spreadsheet; “tag” is as “double-checked” (Column **PREPARED**);
           - These double-checked files have been converted to `*.EIS1600` format
         2. The names of these files are then collected into `AUTOREPORT.md` under **DOUBLE-CHECKED Files (XX) - ready for MIU**.
@@ -19,23 +35,24 @@
         
         ## Process
         
         1. Convert from mARkdown to EIS1600TMP with `convert_mARkdown_to_EIS1600`
         2. Check the `.EIS1600TMP`
         3. Run `insert_uids` on the checked `.EIS1600TMP`
         4. Check again. If anything was changed in the EIS1600 file, run `update_uids`
-        5. After double-check, the file can be disassembled by `disassemble_into_miu_files data/<author>/<text>/<edition>.EIS1600`
+        5. After double-check, the file can be disassembled by `disassemble_into_miu_files <uri_of_that_file>.EIS1600`
         
         ## Installation
+        
+        After creating and activating the eis16000_env (see [Set Up](#set-up-virtual-environment-and-install-the-eis1600-pkg-there)), use:
         ```shell
         $ pip install eis1600
         ```
         
-        In case you have an older version installed, use
-        
+        In case you have an older version installed, use:
         ```shell
         $ pip install --upgrade eis1600
         ```
         
         ## Set Up Virtual Environment and Install the EIS1600 PKG there
         
         To not mess with other python installations, we recommend installing the package in a virual environment.
@@ -73,17 +90,34 @@
         Alias files:
         
         - on Linux:
           - `~.bash_aliases`
         - On Mac:
           - `.zshrc` if you use `zsh` (default in the latest versions Mac OS);
         
+        ## Structure of the working directory
+        
+        The working directory is always the main `EIS1600` directory which is a parent to all the different repositories.
+        The `EIS1600` directory has the following structure:
+        
+        ```
+        |
+        |---| eis_env
+        |---| EIS1600_MIUs
+        |---| gazetteers
+        |---| Master_Chronicle
+        |---| OpenITI_EIS1600_Texts
+        |---| Training_Data
+        ```
+        
+        Path variables are in the module `eis1600/helper/repo`.
+        
         ## Usage
         
-        ### Covert mARkdown to EIS1600 files
+        ### Convert mARkdown to EIS1600 files
         
         Converts mARkdown file to EIS1600TMP (without inserting UIDs).
         The .EIS1600TMP file will be created next to the .mARkdown file (you can insert .inProcess or .completed files as well).
         This command can be run from anywhere within the text repo - use auto complete (`tab`) to get the correct path to the file.
         Alternative: open command line from the folder which contains the file which shall be converted.
         ```shell
         $ convert_mARkdown_to_EIS1600TMP <uri>.mARkdown
@@ -108,57 +142,68 @@
         ```shell
         $ convert_mARkdown_to_EIS1600 <input_dir> <output_dir>
         $ insert_uids <input_dir> <output_dir>
         ```
         
         ### Disassembling
         
-        Disassemble files into the MIU repo. MIU repo has to be next to TEXT repo.
-        Must be run from the root of TEXT repo, this will disassemble all files from the `AUTOREPORT`.
+        Disassemble files into individual MIU files.
+        Run from the [parent directory](#structure-of-the-working-directory) `EIS1600`, this will disassemble all files from the `AUTOREPORT`.
         ```shell
         $ disassemble_into_miu_files
         ```
-        Give the relative path to a file to disassemble a singe file.
+        Can also be run from anywhere within the `EIS1600_MIUs/` directory with a single files as input.
+        E.G.:
         ```shell
-        $ disassemble_into_miu_files data/<author>/<text>/<edition>.EIS1600
+        $ disassemble_into_miu_files <uri_of_the_text>.EIS1600
         ```
         
         ### Reassembling
         
         Run inside MIU repo. Reassemble files into the TEXT repo, therefore, TEXT repo has to be next to MIU repo.
         ```shell
         $ reassemble_from_miu_files <uri>.IDs
         ```
         
         Use the `-e` option to process all files from the MIU repo. Must be run from the root of MIU repo.
         ```shell
         $ reassemble_from_miu_files -e <MIU_repo>
         ```
         
-        ### NER Annotation
+        ### Annotation
         
-        NER annotation for persons, toponyms, misc and dates.
+        NER annotation for persons, toponyms, misc, and also dates, beginning and ending of onomastic information (*NASAB*), and onomastics.
         
         To annotate all MIU files of a text give the IDs file as argument.
         Can be used with `-p` option to run in parallel.
         ```shell
         $ annotate_mius <uri>.IDs
         ```
         
         To annotate an individual MIU file, give MIU file as argument.
         ```shell
         $ annotate_mius <uri>/MIUs/<uri>.<UID>.EIS1600
         ```
         
         If no input is given, annotation is run for the whole repository. Can be used with `-p` option for parallelization.
-        Run from the parent dir of your MIU repo (internally used path starts with: `OpenITI_EIS1600_MIUs/`).
+        Run from the [parent directory](#structure-of-the-working-directory) `EIS1600` (internally used path starts with: `OpenITI_EIS1600_MIUs/`).
         ```shell
         $ annotate_mius -p
         ```
         
+        ### Only Onomastic Annotation
+        
+        **Only for test purposes!**
+        Can be run with `-D` to process one file at a time, otherwise runs in parallel.
+        Can be run with `-T` to use gold-standard data as input.
+        Run from the [parent directory](#structure-of-the-working-directory) `EIS1600`.
+        ```shell
+        $ onomastic_annotation
+        ```
+        
         ### MIU revision
         
         Run the following command from the root of the MIU repo to revise automated annotated files:
         ```shell
         $ miu_random_revisions
         ```
         
@@ -179,18 +224,17 @@
         reviewed    : NOT REVIEWED
         ```
         to
         ```yaml
         reviewed    : REVIEWED
         ```
         
-        ## For MC
-        
-        ### Collect YAMLHeader into JSON
+        ### Collect YAMLHeaders into JSON
         
+        Run from the [parent directory](#structure-of-the-working-directory) `EIS1600`:
         ```shell
         $ yml_to_json
         ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eis1600-0.8.9/eis1600/dates/Date.py` & `eis1600-0.9.0/eis1600/dates/Date.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/dates/date_patterns.py` & `eis1600-0.9.0/eis1600/dates/date_patterns.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/dates/methods.py` & `eis1600-0.9.0/eis1600/dates/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/gazetteers/Onomastics.py` & `eis1600-0.9.0/eis1600/gazetteers/Onomastics.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/gazetteers/Toponyms.py` & `eis1600-0.9.0/eis1600/gazetteers/Toponyms.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pandas as pd
 
 from eis1600.helper.Singleton import Singleton
 from eis1600.helper.ar_normalization import denormalize_list
 
 file_path = files('eis1600.gazetteers.data')
 thurayya_path = file_path.joinpath('toponyms.csv')
-regions_path = file_path.joinpath('regions_gazetteer.csv')
+provinces_path = file_path.joinpath('regions_gazetteer.csv')
 
 
 def toponyms_from_rows(row: pd.Series) -> YAMLToponym:
     toponym = {
             'uri': row['uri'],
             'label': row['placeLabel'],
             'geometry': {
@@ -60,22 +60,22 @@
 
 @Singleton
 class Toponyms:
     """
     Gazetteer
 
     :ivar DataFrame __df: The dataFrame.
-    :ivar __places List[str]: List of all place names and their prefixed variants.
-    :ivar __regions List[str]: List of all region names and their prefixed variants.
+    :ivar __settlements List[str]: List of all settlement names and their prefixed variants.
+    :ivar __provinces List[str]: List of all province names and their prefixed variants.
     :ivar __total List[str]: List of all toponyms and their prefixed variants.
     :ivar __rpl List[Tuple[str, str]]: List of tuples: expression and its replacement.
     """
     __df = None
-    __places = None
-    __regions = None
+    __settlements = None
+    __provinces = None
     __total = None
     __rpl = None
 
     def __init__(self) -> None:
         def split_toponyms(tops: str) -> List[str]:
             return tops.split('، ')
 
@@ -83,38 +83,38 @@
             coords_list = coords.strip('()').split(', ')
             x, y = coords_list
             return [float(x), float(y)]
 
         thurayya_df = pd.read_csv(thurayya_path, usecols=['uri', 'placeLabel', 'toponyms', 'province', 'typeLabel',
                                                           'geometry_type', 'geometry_coords'],
                                   converters={'toponyms': split_toponyms, 'geometry_coords': coords_as_list})
-        regions_df = pd.read_csv(regions_path)
+        provinces_df = pd.read_csv(provinces_path)
         prefixes = ['ب', 'و', 'وب']
 
         def get_all_variations(tops: List[str]) -> List[str]:
             variations = denormalize_list(tops)
             prefixed_variations = [prefix + top for prefix in prefixes for top in variations]
             return variations + prefixed_variations
 
         thurayya_df['toponyms'] = thurayya_df['toponyms'].apply(get_all_variations)
         Toponyms.__df = thurayya_df.explode('toponyms', ignore_index=True)
-        Toponyms.__places = Toponyms.__df['toponyms'].to_list()
-        regions = regions_df['REGION'].to_list()
-        Toponyms.__regions = regions + [prefix + reg for prefix in prefixes for reg in regions]
+        Toponyms.__settlements = Toponyms.__df['toponyms'].to_list()
+        provinces = provinces_df['REGION'].to_list()
+        Toponyms.__provinces = provinces + [prefix + reg for prefix in prefixes for reg in provinces]
 
-        Toponyms.__total = Toponyms.__places + Toponyms.__regions
+        Toponyms.__total = Toponyms.__settlements + Toponyms.__provinces
         Toponyms.__rpl = [(elem, elem.replace(' ', '_')) for elem in Toponyms.__total if ' ' in elem]
 
     @staticmethod
-    def places() -> List[str]:
-        return Toponyms.__places
+    def settlements() -> List[str]:
+        return Toponyms.__settlements
 
     @staticmethod
-    def regions() -> List[str]:
-        return Toponyms.__regions
+    def provinces() -> List[str]:
+        return Toponyms.__provinces
 
     @staticmethod
     def total() -> List[str]:
         return Toponyms.__total
 
     @staticmethod
     def replacements() -> List[Tuple[str, str]]:
@@ -138,26 +138,27 @@
                 }
         }
 
         return YAMLToponym(province)
 
     @staticmethod
     def look_up_entity(entity: str) -> Tuple[str, str, List[YAMLToponym], List[str]]:
-        """
+        """Look up tagged entity in settlements (there is no gazetteer of provinces so far).
 
         :param str entity: The token(s) which were tagged as toponym.
-        :return: placeLabel(s) as str, URI(s) as str, list of toponym uri(s), list of province uri(s),
-        list of toponym(s) coordinates, list of province(s) coordinates.
+        :return: placeLabel(s) as str, URI(s) as str, list of settlement uri(s), list of province uri(s),
+        list of settlement(s) coordinates, list of province(s) coordinates.
         """
-        if entity in Toponyms.__places:
+        # TODO settlements or total?
+        if entity in Toponyms.__settlements:
             matches = Toponyms.__df.loc[Toponyms.__df['toponyms'].str.fullmatch(entity), ['uri', 'placeLabel',
                                                                                           'province',
                                                                                           'geometry_type',
                                                                                           'geometry_coords']]
             uris = matches['uri'].to_list()
             provinces = matches['province'].to_list()
             place = matches['placeLabel'].unique()
 
-            toponyms = [toponyms_from_rows(row) for idx, row in matches.iterrows()]
-            return '::'.join(place), '@' + '@'.join(uris) + '@', toponyms, provinces
+            settlements = [toponyms_from_rows(row) for idx, row in matches.iterrows()]
+            return '::'.join(place), '@' + '@'.join(uris) + '@', settlements, provinces
         else:
             return entity, '', [], []
```

### Comparing `eis1600-0.8.9/eis1600/gazetteers/data/onomastic_gazetteer.csv` & `eis1600-0.9.0/eis1600/gazetteers/data/onomastic_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/gazetteers/data/spelling_gazetteer.csv` & `eis1600-0.9.0/eis1600/gazetteers/data/spelling_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/gazetteers/data/toponyms.csv` & `eis1600-0.9.0/eis1600/gazetteers/data/toponyms.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/helper/EntityTags.py` & `eis1600-0.9.0/eis1600/helper/EntityTags.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/helper/Singleton.py` & `eis1600-0.9.0/eis1600/helper/Singleton.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/helper/ar_normalization.py` & `eis1600-0.9.0/eis1600/helper/ar_normalization.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/helper/fix_miu_annotation.py` & `eis1600-0.9.0/eis1600/helper/fix_miu_annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/helper/markdown_methods.py` & `eis1600-0.9.0/eis1600/helper/markdown_methods.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from typing import Tuple
+
 from eis1600.helper.markdown_patterns import AGE_PATTERN, YEAR_PATTERN
 
 
-def get_yrs_tag_value(tag: str) -> int:
+def get_yrs_tag_value(tag: str) -> Tuple[int, str]:
     """Returns int value encoded in the tag for date and age tags.
 
     :param str tag: Annotation.
     :return int:  numeric value which was encoded in the tag.
     :raise ValueError: If the tag is not correct a ValueError is raised.
     """
     if YEAR_PATTERN.match(tag):
         m = YEAR_PATTERN.match(tag)
     elif AGE_PATTERN.match(tag):
         m = AGE_PATTERN.match(tag)
     else:
         raise ValueError
 
     if m.group('real'):
-        return int(m.group('real'))
+        return int(m.group('real')), m.group('cat')
     else:
-        return int(m.group('written'))
+        return int(m.group('written')), m.group('cat')
```

### Comparing `eis1600-0.8.9/eis1600/helper/markdown_patterns.py` & `eis1600-0.9.0/eis1600/helper/markdown_patterns.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/helper/miu_random_revisions.py` & `eis1600-0.9.0/eis1600/helper/miu_random_revisions.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/helper/repo.py` & `eis1600-0.9.0/eis1600/helper/repo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 
-This module contains functions to work with the EIS1600 text repo. This includes retrieving files from the repo,
-as well as reading and writing to the README file of that repo.
+This module contains functions to work with the EIS1600 repositories. This includes retrieving files from repos, writing
+files to repos, as well as reading and writing to README and AUTOREPORT files.
 
 Functions:
 :function write_to_readme(path, files, which, ext=None, checked=False, remove_duplicates=False):
 :function read_files_from_readme(path, which):
 :function update_texts_fixed_poetry_readme(path, which):
 :function get_files_from_eis1600_dir(path, file_list, file_ext_from, file_ext_to):
 :function travers_eis1600_dir(path, file_ext_from, file_ext_to): Discontinued
@@ -13,14 +13,21 @@
 import re
 from glob import glob
 from os.path import split, splitext
 from typing import List, Literal, Optional
 
 from eis1600.helper.markdown_patterns import FIXED_POETRY_OLD_PATH_PATTERN
 
+# Path variables
+MIU_REPO = 'EIS1600_MIUs/'
+TEXT_REPO = 'OpenITI_EIS1600_Texts/'
+TRAINING_DATA_REPO = 'Training_Data/'
+GAZETTEERS_REPO = 'gazetteers/'
+MC_REPO = 'MasterChronicle/'
+
 
 def get_entry(file_name: str, checked_entry: bool) -> str:
     """Formats README entry for that file_name.
 
     Only used internally.
     :param str file_name: The name of the file whose entry is added to the README
     :param bool checked_entry: Bool indicating if the checkbox of that entry is ticked or not
@@ -237,31 +244,33 @@
 def get_path_to_other_repo(infile: str, which: Literal['MIU', 'TEXT']) -> str:
     """
 
     :param str infile: file which gives URI of the text.
     :param Literal which: Indicating which repo you want to get the path to, accepts 'MIU' or 'TEXT'.
     :return str: path to the same URI in the requested repo
     """
-    out_path = '../'
-
-    if 'data' in infile:
-        out_path += infile.split('data')[0][2:]
-    elif infile == './':
-        pass
-    else:
-        depth = len(infile.split('/'))
-        print(depth)
-        if depth == 1:
-            out_path += '../../../../'
-        elif depth == 2:
-            out_path += '../../../'
-        elif depth == 3:
-            out_path += '../../'
+    if infile.startswith('./OpenITI_EIS1600_') or infile.startswith('./EIS1600_'):
+        if which == 'MIU':
+            return MIU_REPO + 'data/'
         else:
-            out_path += '../'
-
-    if which == 'MIU':
-        out_path += 'OpenITI_EIS1600_MIUs/data/'
+            return TEXT_REPO + 'data/'
     else:
-        out_path += 'OpenITI_EIS1600_Texts/data/'
+        out_path = '../'
 
-    return out_path
+        if 'data' in infile:
+            out_path += infile.split('data')[0][2:]
+        elif infile != './':
+            depth = len(infile.split('/'))
+            print(depth)
+            if depth == 1:
+                out_path += '../../../../'
+            elif depth == 2:
+                out_path += '../../../'
+            elif depth == 3:
+                out_path += '../../'
+            else:
+                out_path += '../'
+
+        if which == 'MIU':
+            return out_path + MIU_REPO + 'data/'
+        else:
+            return out_path + TEXT_REPO + 'data/'
```

### Comparing `eis1600-0.8.9/eis1600/helper/yml_methods.py` & `eis1600-0.9.0/eis1600/helper/yml_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/helper/yml_to_json.py` & `eis1600-0.9.0/eis1600/onomastics/annotation.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,47 @@
+from glob import glob
+from pathlib import Path
+
 import sys
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
-from pathlib import Path
-import jsonpickle
+from functools import partial
+
+from eis1600.helper.logging import setup_logger
 from p_tqdm import p_uimap
 
-from eis1600.processing.preprocessing import get_yml
+from eis1600.onomastics.methods import nasab_annotation
+from helper.repo import GAZETTEERS_REPO, TRAINING_DATA_REPO
 
 
 def main():
     arg_parser = ArgumentParser(
             prog=sys.argv[0], formatter_class=RawDescriptionHelpFormatter,
-            description='''Script to generate JSON from MIU YAMLHeaders.'''
+            description='''Script to annotate onomastic information in gold-standard MIUs.'''
     )
     arg_parser.add_argument('-D', '--debug', action='store_true')
-    args = arg_parser.parse_args()
+    arg_parser.add_argument('-T', '--test', action='store_true')
 
+    args = arg_parser.parse_args()
     debug = args.debug
-    with open('OpenITI_EIS1600_MIUs/gold_standard.txt', 'r', encoding='utf-8') as fh:
+    test = args.test
+
+    with open(TRAINING_DATA_REPO + 'gold_standard.txt', 'r', encoding='utf-8') as fh:
         files_txt = fh.read().splitlines()
-    infiles = ['OpenITI_EIS1600_MIUs/training_nasab/' + file for file in files_txt if Path(
-            'OpenITI_EIS1600_MIUs/training_nasab/' + file
-    ).exists()]
+    if test:
+        infiles = [TRAINING_DATA_REPO + 'gold_standard/' + file for file in files_txt if Path(
+                TRAINING_DATA_REPO + 'gold_standard/' + file).exists()]
+    else:
+        infiles = glob(TRAINING_DATA_REPO + 'training_data_nasab_ML2/*.EIS1600')
 
+    logger_nasab = setup_logger('nasab_unknown', TRAINING_DATA_REPO + 'logs/nasab_unknown.log')
     res = []
     if debug:
-        for file in infiles[:10]:
+        for file in infiles:
             print(file)
-            res.append(get_yml(file))
+            res.append(nasab_annotation(file, logger_nasab, test))
     else:
-        res = p_uimap(get_yml, infiles)
+        res += p_uimap(partial(nasab_annotation, logger_nasab=logger_nasab, test=test), infiles)
 
-    yml_dict = {}
-    for path, yml in res:
-        yml_dict[path] = yml.to_json()
-
-    with open('MasterChronicle/masterchronicleapp/src/data.json', 'w', encoding='utf-8') as fh:
-        json_str = jsonpickle.encode(yml_dict, unpicklable=False)
-        fh.write(json_str)
+    with open(GAZETTEERS_REPO + 'tagged.txt', 'w', encoding='utf-8') as fh:
+        fh.write('\n\n'.join(res))
 
     print('Done')
```

### Comparing `eis1600-0.8.9/eis1600/markdown/UIDs.py` & `eis1600-0.9.0/eis1600/markdown/UIDs.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py` & `eis1600-0.9.0/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/markdown/insert_uids.py` & `eis1600-0.9.0/eis1600/markdown/insert_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/markdown/methods.py` & `eis1600-0.9.0/eis1600/markdown/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/markdown/update_uids.py` & `eis1600-0.9.0/eis1600/markdown/update_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/markdown/update_uids_old_process.py` & `eis1600-0.9.0/eis1600/markdown/update_uids_old_process.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/miu/HeadingTracker.py` & `eis1600-0.9.0/eis1600/miu/HeadingTracker.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/miu/YAMLHandler.py` & `eis1600-0.9.0/eis1600/miu/YAMLHandler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 from ast import literal_eval
 from typing import Any, Dict, Optional
 
-
 from eis1600.gazetteers.Toponyms import YAMLToponym
 from eis1600.helper.markdown_patterns import MIU_HEADER
 from eis1600.helper.yml_methods import dict_to_yaml
 from eis1600.miu.HeadingTracker import HeadingTracker
 
 
 class YAMLHandler:
@@ -21,16 +20,16 @@
     :ivar List[str] dates_headings: List of dates tags contained in headings.
     :ivar List[int] dates: List of dates contained in the text.
     :ivar Dict onomstics: contains onomastic elements by category.
     :ivar str category: String categorising the type of the entry, bio, chr, dict, etc.
     """
     # Only attributes named in the following list are allowed to be added to the YAMLHeader - add any new attribute
     # to that list
-    __attr_from_annotation = ['dates', 'ages', 'onomastics', 'ambigious_toponyms', 'toponyms', 'places', 'provinces',
-                              'edges_places', 'edges_provinces']
+    __attr_from_annotation = ['dates', 'min_date', 'max_date', 'ages', 'onomastics', 'ambigious_toponyms', 'toponyms',
+                              'settlements', 'provinces', 'edges_settlements', 'edges_provinces']
 
     @staticmethod
     def __parse_yml_val(val: str, key: Optional[str] = None) -> Any:
         if val.isdigit():
             return int(val)
         if len(val.split('.')) == 2 and val.split('.')[0].isdigit() and val.split('.')[1].isdigit():
             return float(val)
@@ -40,26 +39,26 @@
             return False
         elif val == 'None' or val == '':
             return None
         elif val.startswith(('\'', '"')):
             return val.strip('\'"')
         elif val.startswith('['):
             # List - no comma allowed in strings, it is used as the separator!
-            raw_val_list = val[1:-1]    # strip '[]' but without stripping multiple in case we have nested lists
+            raw_val_list = val[1:-1]  # strip '[]' but without stripping multiple in case we have nested lists
             if raw_val_list.startswith('(') and raw_val_list.endswith(')'):
                 # List of tuples
                 val_list = raw_val_list.strip('()').split('), (')
                 values = []
                 for v in val_list:
                     t = v.split(', ')
                     values.append((YAMLHandler.__parse_yml_val(t[0]), YAMLHandler.__parse_yml_val(t[1])))
             elif raw_val_list.startswith('[') or raw_val_list.startswith('{'):
                 # Nested lists
                 nested_lists = literal_eval(val)
-                if key == 'places' or key == 'provinces':
+                if key == 'settlements' or key == 'provinces':
                     values = [YAMLToponym(toponym) for toponym in nested_lists]
                 elif key.startswith('edges'):
                     values = [[YAMLToponym(edge[0]), YAMLToponym(edge[1])] for edge in nested_lists]
                 else:
                     values = nested_lists
             else:
                 # List of other values
@@ -147,15 +146,15 @@
 
     def get_yamlfied(self) -> str:
         yaml_str = MIU_HEADER + 'Begin#\n\n'
         for key, val in vars(self).items():
             if val:
                 if key == 'category':
                     yaml_str += key + '    : \'' + val + '\'\n'
-                elif key == 'places' or key == 'provinces':
+                elif key == 'settlements' or key == 'provinces':
                     yaml_str += f'{key}    : {[toponym.as_dict() for toponym in val]}\n'
                 elif key.startswith('edges'):
                     yaml_str += f'{key}    : {[[edge[0].as_dict(), edge[1].as_dict()] for edge in val]}\n'
                 elif hasattr(val, 'get_yamlfied'):
                     yaml_str += f'{key}    : {val.get_yamlfied()}\n'
                 elif isinstance(val, dict):
                     yaml_str += f'{key}    :\n{dict_to_yaml(val, 1)}\n'
@@ -166,15 +165,15 @@
         return yaml_str
 
     def to_json(self) -> Dict:
         json_dict = {}
         for key, val in vars(self).items():
             if key != 'toponyms' and val:
                 # Toponym is only to control the entity and how it was identified
-                if key == 'places' or key == 'provinces':
+                if key == 'settlements' or key == 'provinces':
                     json_dict[key] = [elem.to_json() for elem in val]
                 elif key.startswith('edges'):
                     json_dict[key] = [[edge[0].to_json(), edge[1].to_json()] for edge in val]
                 elif hasattr(val, 'to_json'):
                     json_dict[key] = val.to_json()
                 else:
                     json_dict[key] = val
```

### Comparing `eis1600-0.8.9/eis1600/miu/disassemble_into_miu_files.py` & `eis1600-0.9.0/eis1600/miu/disassemble_into_miu_files.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,36 +6,37 @@
 
 from p_tqdm import p_uimap
 from tqdm import tqdm
 
 from eis1600.helper.repo import get_path_to_other_repo, read_files_from_autoreport, get_files_from_eis1600_dir, \
     write_to_readme
 from eis1600.miu.methods import disassemble_text
+from helper.repo import TEXT_REPO
 
 
 class CheckFileEndingAction(Action):
     def __call__(self, parser, namespace, input_arg, option_string=None):
         if input_arg and os.path.isfile(input_arg):
             filepath, fileext = os.path.splitext(input_arg)
             if fileext != '.EIS1600':
-                parser.error('You need to input a EIS1600 file')
+                parser.error('You need to input an EIS1600 file')
             else:
                 setattr(namespace, self.dest, input_arg)
         else:
             setattr(namespace, self.dest, None)
 
 
 def main():
     arg_parser = ArgumentParser(
             prog=sys.argv[0], formatter_class=RawDescriptionHelpFormatter,
             description='''Script to disassemble EIS1600 file(s) into MIU file(s).
 -----
 Give a single EIS1600 file as input
 or 
-Run without input arg to batch process all EIS1600 files in the EIS1600 directory.
+Run without input arg to batch process all double-checked EIS1600 files from the AUTOREPORT.
 '''
     )
     arg_parser.add_argument('-v', '--verbose', action='store_true')
     arg_parser.add_argument(
             'input', type=str, nargs='?',
             help='EIS1600 file to process',
             action=CheckFileEndingAction
@@ -49,18 +50,18 @@
         out_path = get_path_to_other_repo(infile, 'MIU')
         print(f'Disassemble {infile}')
         disassemble_text(infile, out_path, verbose)
         infiles = [infile.split('/')[-1]]
         path = out_path.split('data')[0]
         write_to_readme(path, infiles, '# Texts disassembled into MIU files\n')
     else:
-        input_dir = './'
+        input_dir = TEXT_REPO
         out_path = get_path_to_other_repo(input_dir, 'MIU')
 
-        print(f'Disassemble EIS1600 files from the EIS1600 repo')
+        print(f'Disassemble double-checked EIS1600 files from the AUTOREPORT')
         files_list = read_files_from_autoreport(input_dir)
 
         infiles = get_files_from_eis1600_dir(input_dir, files_list, 'EIS1600')
         if not infiles:
             print('There are no EIS1600 files to process')
             sys.exit()
```

### Comparing `eis1600-0.8.9/eis1600/miu/methods.py` & `eis1600-0.9.0/eis1600/miu/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/miu/reassemble_from_miu_files.py` & `eis1600-0.9.0/eis1600/miu/reassemble_from_miu_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/miu/yml_handling.py` & `eis1600-0.9.0/eis1600/miu/yml_handling.py`

 * *Files 8% similar despite different names*

```diff
@@ -113,16 +113,16 @@
         tag = m.group('entity')
         length = int(m.group('length'))
         entity = ' '.join(text_with_tags[m.end():].split(maxsplit=length)[:length])
 
         cat = entity_tags_df.loc[entity_tags_df['TAG'].str.fullmatch(tag), 'CATEGORY'].iloc[0]
         if cat == 'DATE' or cat == 'AGE':
             try:
-                val = get_yrs_tag_value(m.group(0))
-                add_to_entities_dict(entities_dict, cat, {'entity': entity, cat.lower(): val})
+                val, e_cat = get_yrs_tag_value(m.group(0))
+                add_to_entities_dict(entities_dict, cat, {'entity': entity, cat.lower(): val, 'cat': e_cat})
             except ValueError:
                 print(f'Tag is neither year nor age: {m.group(0)}\nCheck: {filename}')
                 return
         elif cat == 'TOPONYM':
             place, uri, list_of_uris, list_of_provinces = tg.look_up_entity(entity)
             if len(list_of_uris) > 1:
                 yml_handler.set_ambigious_toponyms()
@@ -149,13 +149,28 @@
             entities_dict['onomastics'] = {'nas': nas_dict}
 
     if 'onomastics' in entities_dict.keys():
         # Sort dict by keys
         entities_dict['onomastics'] = dict(sorted(entities_dict.get('onomastics').items()))
 
     if toponyms_set:
-        entities_dict['places'] = list(toponyms_set)
-        entities_dict['edges_places'] = [[a, b] for a, b in combinations(toponyms_set, 2)]
+        entities_dict['settlements'] = list(toponyms_set)
+        entities_dict['edges_settlements'] = [[a, b] for a, b in combinations(toponyms_set, 2)]
         provinces_set = set([tg.look_up_province(p) for p in provinces_set])
         entities_dict['provinces'] = list(provinces_set)
         entities_dict['edges_provinces'] = [[a, b] for a, b in combinations(provinces_set, 2)]
+
+    if entities_dict.get('dates'):
+        dates = entities_dict.get('dates')
+        birth_date = [d.get('date') for d in dates if d.get('cat') == 'B']
+        death_date = [d.get('date') for d in dates if d.get('cat') == 'D']
+        if death_date:
+            entities_dict['max_date'] = max(death_date)
+        else:
+            entities_dict['max_date'] = max([d.get('date') for d in dates])
+
+        if birth_date:
+            entities_dict['min_date'] = min(birth_date)
+        else:
+            entities_dict['min_date'] = entities_dict.get('max_date') - 70
+
     yml_handler.add_tagged_entities(entities_dict)
```

### Comparing `eis1600-0.8.9/eis1600/nlp/cameltools.py` & `eis1600-0.9.0/eis1600/nlp/cameltools.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/nlp/ner_annotate_mius.py` & `eis1600-0.9.0/eis1600/nlp/ner_annotate_mius.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from eis1600.helper.logging import setup_logger
 from p_tqdm import p_uimap
 from tqdm import tqdm
 
 from eis1600.helper.repo import get_files_from_eis1600_dir, read_files_from_readme
 from eis1600.miu.methods import annotate_miu_file, get_mius
+from helper.repo import MIU_REPO
 
 
 class CheckFileEndingAction(Action):
     def __call__(self, parser, namespace, input_arg, option_string=None):
         if input_arg and os.path.isfile(input_arg):
             filepath, fileext = os.path.splitext(input_arg)
             if fileext != '.IDs' and fileext != '.EIS1600':
@@ -62,19 +63,19 @@
                         annotate_miu_file(miu)
                     except Exception as e:
                         print(miu, e)
         else:
             print(f'NER annotate {infile}')
             annotate_miu_file(infile, force_annotation=force)
     else:
-        input_dir = 'OpenITI_EIS1600_MIUs/'
+        input_dir = MIU_REPO
 
         if not Path(input_dir).exists():
             print('Your working directory seems to be wrong, make sure it is set to the parent dir of '
-                  '`OpenITI_EIS1600_MIUs/`.')
+                  '`EIS1600_MIUs/`.')
             sys.exit()
 
         print(f'NER annotate MIU files')
         files_list = read_files_from_readme(input_dir, '# Texts disassembled into MIU files\n')
         infiles = get_files_from_eis1600_dir(input_dir, files_list, 'IDs')
         if not infiles:
             print('There are no IDs files to process')
```

### Comparing `eis1600-0.8.9/eis1600/nlp/utils.py` & `eis1600-0.9.0/eis1600/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/onomastics/methods.py` & `eis1600-0.9.0/eis1600/onomastics/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/onomastics/re_pattern.py` & `eis1600-0.9.0/eis1600/onomastics/re_pattern.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/processing/postprocessing.py` & `eis1600-0.9.0/eis1600/processing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/processing/preprocessing.py` & `eis1600-0.9.0/eis1600/processing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/stats/methods.py` & `eis1600-0.9.0/eis1600/stats/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600/stats/miu_stats.py` & `eis1600-0.9.0/eis1600/stats/miu_stats.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600.egg-info/PKG-INFO` & `eis1600-0.9.0/eis1600.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,33 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.8.9
+Version: 0.9.0
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
         
+        * [Workflow](#workflow)
+        * [Process](#process)
+        * [Installation](#installation)
+        * [Set Up](#set-up-virtual-environment-and-install-the-eis1600-pkg-there)
+        * [Working Directory Structure](#structure-of-the-working-directory)
+        * [Usage](#usage)
+          * [convert_mARkdown_to_EIS1600TMP](#convert-markdown-to-eis1600-files)
+          * [insert_uids](#convert-markdown-to-eis1600-files)
+          * [update_uids](#convert-markdown-to-eis1600-files)
+          * [disassemble_into_miu_files](#disassembling)
+          * [reassble-from-miu_files](#reassembling)
+          * [annotate_mius](#annotation)
+          * [onomastic_annotation](#only-onomastic-annotation)
+          * [miu_random_revision](#miu-revision)
+          * [yml_to_json](#collect-yamlheaders-into-json)
+        
         ## Workflow
         
         (*so that we do not forget again...*)
         
         1. Double-check text in the Google Spreadsheet; “tag” is as “double-checked” (Column **PREPARED**);
           - These double-checked files have been converted to `*.EIS1600` format
         2. The names of these files are then collected into `AUTOREPORT.md` under **DOUBLE-CHECKED Files (XX) - ready for MIU**.
@@ -19,23 +35,24 @@
         
         ## Process
         
         1. Convert from mARkdown to EIS1600TMP with `convert_mARkdown_to_EIS1600`
         2. Check the `.EIS1600TMP`
         3. Run `insert_uids` on the checked `.EIS1600TMP`
         4. Check again. If anything was changed in the EIS1600 file, run `update_uids`
-        5. After double-check, the file can be disassembled by `disassemble_into_miu_files data/<author>/<text>/<edition>.EIS1600`
+        5. After double-check, the file can be disassembled by `disassemble_into_miu_files <uri_of_that_file>.EIS1600`
         
         ## Installation
+        
+        After creating and activating the eis16000_env (see [Set Up](#set-up-virtual-environment-and-install-the-eis1600-pkg-there)), use:
         ```shell
         $ pip install eis1600
         ```
         
-        In case you have an older version installed, use
-        
+        In case you have an older version installed, use:
         ```shell
         $ pip install --upgrade eis1600
         ```
         
         ## Set Up Virtual Environment and Install the EIS1600 PKG there
         
         To not mess with other python installations, we recommend installing the package in a virual environment.
@@ -73,17 +90,34 @@
         Alias files:
         
         - on Linux:
           - `~.bash_aliases`
         - On Mac:
           - `.zshrc` if you use `zsh` (default in the latest versions Mac OS);
         
+        ## Structure of the working directory
+        
+        The working directory is always the main `EIS1600` directory which is a parent to all the different repositories.
+        The `EIS1600` directory has the following structure:
+        
+        ```
+        |
+        |---| eis_env
+        |---| EIS1600_MIUs
+        |---| gazetteers
+        |---| Master_Chronicle
+        |---| OpenITI_EIS1600_Texts
+        |---| Training_Data
+        ```
+        
+        Path variables are in the module `eis1600/helper/repo`.
+        
         ## Usage
         
-        ### Covert mARkdown to EIS1600 files
+        ### Convert mARkdown to EIS1600 files
         
         Converts mARkdown file to EIS1600TMP (without inserting UIDs).
         The .EIS1600TMP file will be created next to the .mARkdown file (you can insert .inProcess or .completed files as well).
         This command can be run from anywhere within the text repo - use auto complete (`tab`) to get the correct path to the file.
         Alternative: open command line from the folder which contains the file which shall be converted.
         ```shell
         $ convert_mARkdown_to_EIS1600TMP <uri>.mARkdown
@@ -108,57 +142,68 @@
         ```shell
         $ convert_mARkdown_to_EIS1600 <input_dir> <output_dir>
         $ insert_uids <input_dir> <output_dir>
         ```
         
         ### Disassembling
         
-        Disassemble files into the MIU repo. MIU repo has to be next to TEXT repo.
-        Must be run from the root of TEXT repo, this will disassemble all files from the `AUTOREPORT`.
+        Disassemble files into individual MIU files.
+        Run from the [parent directory](#structure-of-the-working-directory) `EIS1600`, this will disassemble all files from the `AUTOREPORT`.
         ```shell
         $ disassemble_into_miu_files
         ```
-        Give the relative path to a file to disassemble a singe file.
+        Can also be run from anywhere within the `EIS1600_MIUs/` directory with a single files as input.
+        E.G.:
         ```shell
-        $ disassemble_into_miu_files data/<author>/<text>/<edition>.EIS1600
+        $ disassemble_into_miu_files <uri_of_the_text>.EIS1600
         ```
         
         ### Reassembling
         
         Run inside MIU repo. Reassemble files into the TEXT repo, therefore, TEXT repo has to be next to MIU repo.
         ```shell
         $ reassemble_from_miu_files <uri>.IDs
         ```
         
         Use the `-e` option to process all files from the MIU repo. Must be run from the root of MIU repo.
         ```shell
         $ reassemble_from_miu_files -e <MIU_repo>
         ```
         
-        ### NER Annotation
+        ### Annotation
         
-        NER annotation for persons, toponyms, misc and dates.
+        NER annotation for persons, toponyms, misc, and also dates, beginning and ending of onomastic information (*NASAB*), and onomastics.
         
         To annotate all MIU files of a text give the IDs file as argument.
         Can be used with `-p` option to run in parallel.
         ```shell
         $ annotate_mius <uri>.IDs
         ```
         
         To annotate an individual MIU file, give MIU file as argument.
         ```shell
         $ annotate_mius <uri>/MIUs/<uri>.<UID>.EIS1600
         ```
         
         If no input is given, annotation is run for the whole repository. Can be used with `-p` option for parallelization.
-        Run from the parent dir of your MIU repo (internally used path starts with: `OpenITI_EIS1600_MIUs/`).
+        Run from the [parent directory](#structure-of-the-working-directory) `EIS1600` (internally used path starts with: `OpenITI_EIS1600_MIUs/`).
         ```shell
         $ annotate_mius -p
         ```
         
+        ### Only Onomastic Annotation
+        
+        **Only for test purposes!**
+        Can be run with `-D` to process one file at a time, otherwise runs in parallel.
+        Can be run with `-T` to use gold-standard data as input.
+        Run from the [parent directory](#structure-of-the-working-directory) `EIS1600`.
+        ```shell
+        $ onomastic_annotation
+        ```
+        
         ### MIU revision
         
         Run the following command from the root of the MIU repo to revise automated annotated files:
         ```shell
         $ miu_random_revisions
         ```
         
@@ -179,18 +224,17 @@
         reviewed    : NOT REVIEWED
         ```
         to
         ```yaml
         reviewed    : REVIEWED
         ```
         
-        ## For MC
-        
-        ### Collect YAMLHeader into JSON
+        ### Collect YAMLHeaders into JSON
         
+        Run from the [parent directory](#structure-of-the-working-directory) `EIS1600`:
         ```shell
         $ yml_to_json
         ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eis1600-0.8.9/eis1600.egg-info/SOURCES.txt` & `eis1600-0.9.0/eis1600.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/eis1600.egg-info/entry_points.txt` & `eis1600-0.9.0/eis1600.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.9/setup.py` & `eis1600-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='eis1600',
-      version='0.8.9',
+      version='0.9.0',
       description='EIS1600 project tools and utilities',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/EIS1600/eis1600-pkg',
       author='Lisa Mischer',
       author_email='mischer.lisa@gmail.com',
       license='MIT License',
```

