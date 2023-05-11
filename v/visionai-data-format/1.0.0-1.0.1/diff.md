# Comparing `tmp/visionai-data-format-1.0.0.tar.gz` & `tmp/visionai-data-format-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionai-data-format-1.0.0.tar", last modified: Tue May  2 07:40:22 2023, max compression
+gzip compressed data, was "visionai-data-format-1.0.1.tar", last modified: Thu May 11 07:26:20 2023, max compression
```

## Comparing `visionai-data-format-1.0.0.tar` & `visionai-data-format-1.0.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.374957 visionai-data-format-1.0.0/
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.295626 visionai-data-format-1.0.0/.github/
--rw-r--r--   0 christian   (501) staff       (20)      472 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 christian   (501) staff       (20)      288 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/.github/labels.yml
--rw-r--r--   0 christian   (501) staff       (20)       16 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/.github/semantic.yml
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.297401 visionai-data-format-1.0.0/.github/workflows/
--rw-r--r--   0 christian   (501) staff       (20)      699 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/.github/workflows/test.yml
--rw-r--r--   0 christian   (501) staff       (20)     3080 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/.gitignore
--rw-r--r--   0 christian   (501) staff       (20)     1741 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 christian   (501) staff       (20)     1507 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/Makefile
--rw-r--r--   0 christian   (501) staff       (20)      189 2023-05-02 07:40:22.373495 visionai-data-format-1.0.0/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)       69 2022-11-09 05:29:43.000000 visionai-data-format-1.0.0/README.md
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.300660 visionai-data-format-1.0.0/ci/
--rw-r--r--   0 christian   (501) staff       (20)      965 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/ci/.commitlint.yaml
--rw-r--r--   0 christian   (501) staff       (20)     1465 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/ci/COMMIT_MESSAGE_TEMPLATE
--rw-r--r--   0 christian   (501) staff       (20)       63 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/ci/dev.txt
--rw-r--r--   0 christian   (501) staff       (20)      312 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/ci/setup.cfg
--rw-r--r--   0 christian   (501) staff       (20)     3658 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/conftest.py
--rw-r--r--   0 christian   (501) staff       (20)       38 2023-05-02 07:40:22.375105 visionai-data-format-1.0.0/setup.cfg
--rw-r--r--   0 christian   (501) staff       (20)      577 2023-05-02 07:39:07.000000 visionai-data-format-1.0.0/setup.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.302478 visionai-data-format-1.0.0/tests/
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.332330 visionai-data-format-1.0.0/tests/test_data/
--rw-r--r--   0 christian   (501) staff       (20)     2549 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_contexts_data.json
--rw-r--r--   0 christian   (501) staff       (20)     7424 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/tests/test_data/fake_objects_data.json
--rw-r--r--   0 christian   (501) staff       (20)     5852 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_objects_data_single_lidar.json
--rw-r--r--   0 christian   (501) staff       (20)     5850 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_objects_data_single_lidar_wrong_class.json
--rw-r--r--   0 christian   (501) staff       (20)    10870 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_objects_data_single_lidar_wrong_objects_frame_intervals.json
--rw-r--r--   0 christian   (501) staff       (20)    10870 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_objects_data_single_lidar_wrong_visionai_frame_intervals.json
--rw-r--r--   0 christian   (501) staff       (20)     5852 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_objects_data_wrong_frame_properties_sensor.json
--rw-r--r--   0 christian   (501) staff       (20)      454 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_objects_data_wrong_visionai_streams_sensor.json
--rw-r--r--   0 christian   (501) staff       (20)    26678 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_objects_semantic_segmentation.json
--rw-r--r--   0 christian   (501) staff       (20)    25431 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_objects_semantic_segmentation_without_tags.json
--rw-r--r--   0 christian   (501) staff       (20)    26676 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_objects_semantic_segmentation_wrong_tags_classes.json
--rw-r--r--   0 christian   (501) staff       (20)     4796 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/tests/test_data/fake_raw_data.json
--rw-r--r--   0 christian   (501) staff       (20)      679 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_visionai_classification_ontology.json
--rw-r--r--   0 christian   (501) staff       (20)     5885 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_visionai_ontology.json
--rw-r--r--   0 christian   (501) staff       (20)      454 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_visionai_semantic_ontology.json
--rw-r--r--   0 christian   (501) staff       (20)     7052 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/tests/test_data/generated_objects_data.json
--rw-r--r--   0 christian   (501) staff       (20)     4424 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/tests/test_data/generated_raw_data.json
--rw-r--r--   0 christian   (501) staff       (20)     2177 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/tests/test_schemas.py
--rw-r--r--   0 christian   (501) staff       (20)     4727 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_validators.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.343932 visionai-data-format-1.0.0/visionai_data_format/
--rw-r--r--   0 christian   (501) staff       (20)     1609 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/Readme.md
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)     1400 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/bdd_to_vai.py
--rw-r--r--   0 christian   (501) staff       (20)     7697 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/coco_to_vai.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.352959 visionai-data-format-1.0.0/visionai_data_format/schemas/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/schemas/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)     2142 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/schemas/bdd_schema.py
--rw-r--r--   0 christian   (501) staff       (20)      679 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/schemas/coco_schema.py
--rw-r--r--   0 christian   (501) staff       (20)     1062 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/visionai_data_format/schemas/common.py
--rw-r--r--   0 christian   (501) staff       (20)      994 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/visionai_data_format/schemas/ontology.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.355971 visionai-data-format-1.0.0/visionai_data_format/schemas/utils/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-02 07:39:07.000000 visionai-data-format-1.0.0/visionai_data_format/schemas/utils/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)    39422 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/visionai_data_format/schemas/utils/validators.py
--rw-r--r--   0 christian   (501) staff       (20)    26771 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/visionai_data_format/schemas/visionai_schema.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.371650 visionai-data-format-1.0.0/visionai_data_format/utils/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/utils/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)      495 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/utils/calculation.py
--rw-r--r--   0 christian   (501) staff       (20)    10506 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/utils/checker.py
--rw-r--r--   0 christian   (501) staff       (20)      761 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/utils/classes.py
--rw-r--r--   0 christian   (501) staff       (20)      335 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/utils/common.py
--rw-r--r--   0 christian   (501) staff       (20)     6877 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/utils/converter.py
--rw-r--r--   0 christian   (501) staff       (20)     4059 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/utils/resize.py
--rw-r--r--   0 christian   (501) staff       (20)     1992 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/visionai_data_format/utils/validator.py
--rw-r--r--   0 christian   (501) staff       (20)     2274 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/vai_to_bdd.py
--rw-r--r--   0 christian   (501) staff       (20)     6237 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/vai_to_coco.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.348421 visionai-data-format-1.0.0/visionai_data_format.egg-info/
--rw-r--r--   0 christian   (501) staff       (20)      189 2023-05-02 07:40:22.000000 visionai-data-format-1.0.0/visionai_data_format.egg-info/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)     2353 2023-05-02 07:40:22.000000 visionai-data-format-1.0.0/visionai_data_format.egg-info/SOURCES.txt
--rw-r--r--   0 christian   (501) staff       (20)        1 2023-05-02 07:40:22.000000 visionai-data-format-1.0.0/visionai_data_format.egg-info/dependency_links.txt
--rw-r--r--   0 christian   (501) staff       (20)       40 2023-05-02 07:40:22.000000 visionai-data-format-1.0.0/visionai_data_format.egg-info/requires.txt
--rw-r--r--   0 christian   (501) staff       (20)       21 2023-05-02 07:40:22.000000 visionai-data-format-1.0.0/visionai_data_format.egg-info/top_level.txt
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.974892 visionai-data-format-1.0.1/
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.543804 visionai-data-format-1.0.1/.github/
+-rw-r--r--   0 christian   (501) staff       (20)      472 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 christian   (501) staff       (20)      288 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/.github/labels.yml
+-rw-r--r--   0 christian   (501) staff       (20)       16 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/.github/semantic.yml
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.545948 visionai-data-format-1.0.1/.github/workflows/
+-rw-r--r--   0 christian   (501) staff       (20)      699 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/.github/workflows/test.yml
+-rw-r--r--   0 christian   (501) staff       (20)     3080 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/.gitignore
+-rw-r--r--   0 christian   (501) staff       (20)     1741 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 christian   (501) staff       (20)     1507 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/Makefile
+-rw-r--r--   0 christian   (501) staff       (20)      189 2023-05-11 07:26:19.969912 visionai-data-format-1.0.1/PKG-INFO
+-rw-r--r--   0 christian   (501) staff       (20)       69 2022-11-09 05:29:43.000000 visionai-data-format-1.0.1/README.md
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.564077 visionai-data-format-1.0.1/ci/
+-rw-r--r--   0 christian   (501) staff       (20)      965 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/ci/.commitlint.yaml
+-rw-r--r--   0 christian   (501) staff       (20)     1465 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/ci/COMMIT_MESSAGE_TEMPLATE
+-rw-r--r--   0 christian   (501) staff       (20)       63 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/ci/dev.txt
+-rw-r--r--   0 christian   (501) staff       (20)      312 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/ci/setup.cfg
+-rw-r--r--   0 christian   (501) staff       (20)     3658 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/conftest.py
+-rw-r--r--   0 christian   (501) staff       (20)       38 2023-05-11 07:26:19.991616 visionai-data-format-1.0.1/setup.cfg
+-rw-r--r--   0 christian   (501) staff       (20)      577 2023-05-11 06:46:16.000000 visionai-data-format-1.0.1/setup.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.568459 visionai-data-format-1.0.1/tests/
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.603258 visionai-data-format-1.0.1/tests/test_data/
+-rw-r--r--   0 christian   (501) staff       (20)     2549 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_contexts_data.json
+-rw-r--r--   0 christian   (501) staff       (20)     7424 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_objects_data.json
+-rw-r--r--   0 christian   (501) staff       (20)     5852 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_objects_data_single_lidar.json
+-rw-r--r--   0 christian   (501) staff       (20)     5850 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_objects_data_single_lidar_wrong_class.json
+-rw-r--r--   0 christian   (501) staff       (20)    10870 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_objects_data_single_lidar_wrong_objects_frame_intervals.json
+-rw-r--r--   0 christian   (501) staff       (20)    10870 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_objects_data_single_lidar_wrong_visionai_frame_intervals.json
+-rw-r--r--   0 christian   (501) staff       (20)     5852 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_objects_data_wrong_frame_properties_sensor.json
+-rw-r--r--   0 christian   (501) staff       (20)      454 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_objects_data_wrong_visionai_streams_sensor.json
+-rw-r--r--   0 christian   (501) staff       (20)    26678 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_objects_semantic_segmentation.json
+-rw-r--r--   0 christian   (501) staff       (20)    25431 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_objects_semantic_segmentation_without_tags.json
+-rw-r--r--   0 christian   (501) staff       (20)    26676 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_objects_semantic_segmentation_wrong_tags_classes.json
+-rw-r--r--   0 christian   (501) staff       (20)     4796 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_raw_data.json
+-rw-r--r--   0 christian   (501) staff       (20)      679 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_visionai_classification_ontology.json
+-rw-r--r--   0 christian   (501) staff       (20)     5885 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_visionai_ontology.json
+-rw-r--r--   0 christian   (501) staff       (20)      454 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_visionai_semantic_ontology.json
+-rw-r--r--   0 christian   (501) staff       (20)     7052 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/generated_objects_data.json
+-rw-r--r--   0 christian   (501) staff       (20)     4424 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/generated_raw_data.json
+-rw-r--r--   0 christian   (501) staff       (20)     2177 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_schemas.py
+-rw-r--r--   0 christian   (501) staff       (20)     4739 2023-05-11 06:47:55.000000 visionai-data-format-1.0.1/tests/test_validators.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.619617 visionai-data-format-1.0.1/visionai_data_format/
+-rw-r--r--   0 christian   (501) staff       (20)     1609 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/Readme.md
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)     1400 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/bdd_to_vai.py
+-rw-r--r--   0 christian   (501) staff       (20)     7697 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/coco_to_vai.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.708067 visionai-data-format-1.0.1/visionai_data_format/schemas/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-11 06:22:30.000000 visionai-data-format-1.0.1/visionai_data_format/schemas/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)     2142 2023-05-11 06:22:30.000000 visionai-data-format-1.0.1/visionai_data_format/schemas/bdd_schema.py
+-rw-r--r--   0 christian   (501) staff       (20)      679 2023-05-11 06:22:30.000000 visionai-data-format-1.0.1/visionai_data_format/schemas/coco_schema.py
+-rw-r--r--   0 christian   (501) staff       (20)     1657 2023-05-11 06:46:16.000000 visionai-data-format-1.0.1/visionai_data_format/schemas/common.py
+-rw-r--r--   0 christian   (501) staff       (20)      994 2023-05-11 07:02:55.000000 visionai-data-format-1.0.1/visionai_data_format/schemas/ontology.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.754114 visionai-data-format-1.0.1/visionai_data_format/schemas/utils/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-11 06:22:30.000000 visionai-data-format-1.0.1/visionai_data_format/schemas/utils/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)    39369 2023-05-11 06:46:16.000000 visionai-data-format-1.0.1/visionai_data_format/schemas/utils/validators.py
+-rw-r--r--   0 christian   (501) staff       (20)    27999 2023-05-11 06:46:16.000000 visionai-data-format-1.0.1/visionai_data_format/schemas/visionai_schema.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.915197 visionai-data-format-1.0.1/visionai_data_format/utils/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/utils/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)      495 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/utils/calculation.py
+-rw-r--r--   0 christian   (501) staff       (20)    10506 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/utils/checker.py
+-rw-r--r--   0 christian   (501) staff       (20)      761 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/utils/classes.py
+-rw-r--r--   0 christian   (501) staff       (20)      335 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/utils/common.py
+-rw-r--r--   0 christian   (501) staff       (20)     6877 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/utils/converter.py
+-rw-r--r--   0 christian   (501) staff       (20)     4059 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/utils/resize.py
+-rw-r--r--   0 christian   (501) staff       (20)     1992 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/utils/validator.py
+-rw-r--r--   0 christian   (501) staff       (20)     2274 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/vai_to_bdd.py
+-rw-r--r--   0 christian   (501) staff       (20)     6237 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/vai_to_coco.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.629978 visionai-data-format-1.0.1/visionai_data_format.egg-info/
+-rw-r--r--   0 christian   (501) staff       (20)      189 2023-05-11 07:26:19.000000 visionai-data-format-1.0.1/visionai_data_format.egg-info/PKG-INFO
+-rw-r--r--   0 christian   (501) staff       (20)     2353 2023-05-11 07:26:19.000000 visionai-data-format-1.0.1/visionai_data_format.egg-info/SOURCES.txt
+-rw-r--r--   0 christian   (501) staff       (20)        1 2023-05-11 07:26:19.000000 visionai-data-format-1.0.1/visionai_data_format.egg-info/dependency_links.txt
+-rw-r--r--   0 christian   (501) staff       (20)       40 2023-05-11 07:26:19.000000 visionai-data-format-1.0.1/visionai_data_format.egg-info/requires.txt
+-rw-r--r--   0 christian   (501) staff       (20)       21 2023-05-11 07:26:19.000000 visionai-data-format-1.0.1/visionai_data_format.egg-info/top_level.txt
```

### Comparing `visionai-data-format-1.0.0/.github/workflows/test.yml` & `visionai-data-format-1.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/.gitignore` & `visionai-data-format-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/.pre-commit-config.yaml` & `visionai-data-format-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/Makefile` & `visionai-data-format-1.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/ci/.commitlint.yaml` & `visionai-data-format-1.0.1/ci/.commitlint.yaml`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/ci/COMMIT_MESSAGE_TEMPLATE` & `visionai-data-format-1.0.1/ci/COMMIT_MESSAGE_TEMPLATE`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/conftest.py` & `visionai-data-format-1.0.1/conftest.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/setup.py` & `visionai-data-format-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 AUTHOR = "LinkerVision"
 PACKAGE_NAME = "visionai-data-format"
-PACKAGE_VERSION = "1.0.0"
+PACKAGE_VERSION = "1.0.1"
 DESC = "converter tool for visionai format"
 REQUIRED = ["pydantic"]
 REQUIRES_PYTHON = ">=3.7, <4"
 EXTRAS = {
     "test": [
         "pytest",
         "mock",
```

### Comparing `visionai-data-format-1.0.0/tests/test_data/fake_contexts_data.json` & `visionai-data-format-1.0.1/tests/test_data/fake_contexts_data.json`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/tests/test_data/fake_objects_data.json` & `visionai-data-format-1.0.1/tests/test_data/fake_objects_data.json`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/tests/test_data/fake_objects_data_single_lidar.json` & `visionai-data-format-1.0.1/tests/test_data/fake_objects_data_single_lidar.json`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/tests/test_data/fake_objects_data_single_lidar_wrong_class.json` & `visionai-data-format-1.0.1/tests/test_data/fake_objects_data_single_lidar_wrong_class.json`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/tests/test_data/fake_objects_data_single_lidar_wrong_objects_frame_intervals.json` & `visionai-data-format-1.0.1/tests/test_data/fake_objects_data_single_lidar_wrong_objects_frame_intervals.json`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/tests/test_data/fake_objects_data_single_lidar_wrong_visionai_frame_intervals.json` & `visionai-data-format-1.0.1/tests/test_data/fake_objects_data_single_lidar_wrong_visionai_frame_intervals.json`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/tests/test_data/fake_objects_data_wrong_frame_properties_sensor.json` & `visionai-data-format-1.0.1/tests/test_data/fake_objects_data_wrong_frame_properties_sensor.json`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/tests/test_data/fake_objects_semantic_segmentation.json` & `visionai-data-format-1.0.1/tests/test_data/fake_objects_semantic_segmentation.json`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/tests/test_data/fake_objects_semantic_segmentation_without_tags.json` & `visionai-data-format-1.0.1/tests/test_data/fake_objects_semantic_segmentation_without_tags.json`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/tests/test_data/fake_objects_semantic_segmentation_wrong_tags_classes.json` & `visionai-data-format-1.0.1/tests/test_data/fake_objects_semantic_segmentation_wrong_tags_classes.json`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/tests/test_data/fake_raw_data.json` & `visionai-data-format-1.0.1/tests/test_data/fake_raw_data.json`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/tests/test_data/fake_visionai_classification_ontology.json` & `visionai-data-format-1.0.1/tests/test_data/fake_visionai_classification_ontology.json`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/tests/test_data/fake_visionai_ontology.json` & `visionai-data-format-1.0.1/tests/test_data/fake_visionai_ontology.json`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/tests/test_data/generated_objects_data.json` & `visionai-data-format-1.0.1/tests/test_data/generated_objects_data.json`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/tests/test_data/generated_raw_data.json` & `visionai-data-format-1.0.1/tests/test_data/generated_raw_data.json`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/tests/test_schemas.py` & `visionai-data-format-1.0.1/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/tests/test_validators.py` & `visionai-data-format-1.0.1/tests/test_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     errors = VisionAIModel(
         **fake_objects_data_single_lidar_wrong_class
     ).validate_with_ontology(
         ontology=ontology,
     )
 
-    assert errors == ["Label with classes {'children'} doesn't accepted"]
+    assert errors == ["Attribute objects with classes {'children'} doesn't accepted"]
 
 
 def test_validate_semantic_segmentation(
     fake_visionai_semantic_ontology, fake_objects_semantic_segmentation
 ):
 
     ontology = Ontology(**fake_visionai_semantic_ontology).dict(exclude_unset=True)
```

### Comparing `visionai-data-format-1.0.0/visionai_data_format/Readme.md` & `visionai-data-format-1.0.1/visionai_data_format/Readme.md`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/visionai_data_format/bdd_to_vai.py` & `visionai-data-format-1.0.1/visionai_data_format/bdd_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/visionai_data_format/coco_to_vai.py` & `visionai-data-format-1.0.1/visionai_data_format/coco_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/visionai_data_format/schemas/bdd_schema.py` & `visionai-data-format-1.0.1/visionai_data_format/schemas/bdd_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/visionai_data_format/schemas/coco_schema.py` & `visionai-data-format-1.0.1/visionai_data_format/schemas/coco_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/visionai_data_format/schemas/ontology.py` & `visionai-data-format-1.0.1/visionai_data_format/schemas/ontology.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/visionai_data_format/schemas/utils/validators.py` & `visionai-data-format-1.0.1/visionai_data_format/schemas/utils/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,14 @@
     if not attributes:
         return {}
     attributes_map = defaultdict(set)
     for attr_type, data_list in attributes.items():
         if not data_list:
             continue
 
-        attr_type = "option" if attr_type == "vec" else attr_type
-
         for data in data_list:
             name = data.get("name").upper()
             key = f"{name}:{attr_type}"
             option = {}
             if not data.get("val"):
                 continue
             if isinstance(
@@ -871,24 +869,23 @@
 ) -> Optional[str]:
 
     if not ontology_attributes_map:
         ontology_attributes_map = {}
     ontology_classes = set(ontology_data.keys())
     visionai_frames = visionai.get("frames", {})
     visionai_objects = visionai.get(root_key, {})
-
     extra_classes, classes_attributes_map = validate_classes(
         visionai=visionai,
         ontology_classes=ontology_classes,
         root_key=root_key,
         sub_root_key=data_key_map["sub_root_key"],
     )
 
     if extra_classes:
-        return f"Label with classes {extra_classes} doesn't accepted"
+        return f"Attribute {root_key} with classes {extra_classes} doesn't accepted"
 
     valid_attr, valid_attr_data = validate_attributes(
         classes_attributes_map, ontology_attributes_map
     )
     if not valid_attr:
         obj_cls, name_type = valid_attr_data
         return f"Attribute {root_key} error : class [{obj_cls}] attribute error [{name_type}]"
```

### Comparing `visionai-data-format-1.0.0/visionai_data_format/schemas/visionai_schema.py` & `visionai-data-format-1.0.1/visionai_data_format/schemas/visionai_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal  #
 
 from pydantic import (
-    BaseModel,
     Extra,
     Field,
     StrictBool,
     StrictInt,
     StrictStr,
     conlist,
     root_validator,
     validator,
 )
 
+from visionai_data_format.schemas.common import ExcludedNoneBaseModel
 from visionai_data_format.schemas.ontology import Ontology
 from visionai_data_format.schemas.utils.validators import (
     build_ontology_attributes_map,
     validate_contexts,
     validate_objects,
     validate_streams,
 )
@@ -80,36 +80,36 @@
     CAMERA = "camera"
     LIDAR = "lidar"
     RADAR = "radar"
     GPS_IMU = "gps_imu"
     OTHER = "other"
 
 
-class Attributes(BaseModel):
+class Attributes(ExcludedNoneBaseModel):
     class Config:
         extra = Extra.forbid
 
     boolean: List[StaticBoolean] = Field(default_factory=list)
     num: List[StaticNum] = Field(default_factory=list)
     text: List[StaticText] = Field(default_factory=list)
     vec: List[StaticVec] = Field(default_factory=list)
 
 
-class CoordinateSystemWRTParent(BaseModel):
+class CoordinateSystemWRTParent(ExcludedNoneBaseModel):
     matrix4x4: List[Union[float, int]]
 
     @validator("matrix4x4")
     def validate_matrix4x4(cls, value):
         assert (
             len(value) == 16
         ), f"value {value} with length {len(value)} is not allowed"
         return value
 
 
-class CoordinateSystem(BaseModel):
+class CoordinateSystem(ExcludedNoneBaseModel):
     type: CoordinateSystemType
     parent: StrictStr
     children: List[StrictStr]
     pose_wrt_parent: Optional[CoordinateSystemWRTParent] = Field(default=None)
 
     class Config:
         extra = Extra.forbid
@@ -117,15 +117,15 @@
 
     @validator("pose_wrt_parent")
     def validate_pose_wrt_parent(cls, value):
         assert value, f"value {value} is not allowed"
         return value
 
 
-class FrameInterval(BaseModel):
+class FrameInterval(ExcludedNoneBaseModel):
     class Config:
         extra = Extra.forbid
 
     frame_start: StrictInt = Field(
         ..., description="Initial frame number of the interval."
     )
     frame_end: StrictInt = Field(
@@ -141,15 +141,15 @@
             raise ValueError(
                 "Range is not accepted,"
                 + f" frame start : {frame_start} , frame end : {frame_end}"
             )
         return values
 
 
-class IntrinsicsPinhole(BaseModel):
+class IntrinsicsPinhole(ExcludedNoneBaseModel):
     camera_matrix_3x4: List[float]
     distortion_coeffs_1xN: Optional[List[Union[float, int]]] = None
     height_px: int
     width_px: int
 
     @validator("distortion_coeffs_1xN")
     def validate_distortion_coeffs_1xN(cls, value):
@@ -160,25 +160,25 @@
     def validate_camera_matrix_3x4(cls, value):
         assert (
             value and len(value) == 12
         ), f"value {value} is not allowed, must be a list of 12 float values"
         return value
 
 
-class Metadata(BaseModel):
+class Metadata(ExcludedNoneBaseModel):
     class Config:
         use_enum_values = True
         extra = Extra.allow
 
     schema_version: SchemaVersion = Field(
         description="Version number of the VisionAI schema this annotation JSON object follows.",
     )
 
 
-class StaticBoolean(BaseModel):
+class StaticBoolean(ExcludedNoneBaseModel):
 
     attributes: Optional[Attributes] = None
     name: StrictStr = Field(
         ...,
         description="This is a string encoding the name of this object data."
         + " It is used as index inside the corresponding object data pointers.",
     )
@@ -195,17 +195,22 @@
 
 
 class DynamicBoolean(StaticBoolean):
     stream: StrictStr = Field(
         ...,
         description="Name of the stream in respect of which this object data is expressed.",
     )
+    confidence_score: Optional[float] = Field(
+        None,
+        description="The confidence score of model prediction of this object."
+        + " Ground truth does not have this attribute.",
+    )
 
 
-class StaticNum(BaseModel):
+class StaticNum(ExcludedNoneBaseModel):
     class Config:
         use_enum_values = True
         extra = Extra.forbid
 
     attributes: Optional[Attributes] = None
     name: StrictStr = Field(
         ...,
@@ -223,17 +228,22 @@
 
 
 class DynamicNum(StaticNum):
     stream: StrictStr = Field(
         ...,
         description="Name of the stream in respect of which this object data is expressed.",
     )
+    confidence_score: Optional[float] = Field(
+        None,
+        description="The confidence score of model prediction of this object."
+        + " Ground truth does not have this attribute.",
+    )
 
 
-class StaticText(BaseModel):
+class StaticText(ExcludedNoneBaseModel):
     class Config:
         use_enum_values = True
         extra = Extra.forbid
 
     attributes: Optional[Attributes] = None
     name: Optional[StrictStr] = Field(
         None,
@@ -250,16 +260,22 @@
 
 class DynamicText(StaticText):
     stream: StrictStr = Field(
         ...,
         description="Name of the stream in respect of which this object data is expressed.",
     )
 
+    confidence_score: Optional[float] = Field(
+        None,
+        description="The confidence score of model prediction of this object."
+        + " Ground truth does not have this attribute.",
+    )
+
 
-class VecBaseNoName(BaseModel):
+class VecBaseNoName(ExcludedNoneBaseModel):
     attributes: Optional[Attributes] = None
     type: Optional[TypeRange] = Field(
         None,
         description="This attribute specifies whether the vector shall be"
         + " considered as a descriptor of individual values or as a definition of a range.",
     )
     val: List[Union[float, int, str]] = Field(
@@ -280,17 +296,22 @@
 
 
 class DynamicVec(StaticVec):
     stream: StrictStr = Field(
         ...,
         description="Name of the stream in respect of which this object data is expressed.",
     )
+    confidence_score: Optional[float] = Field(
+        None,
+        description="The confidence score of model prediction of this object."
+        + " Ground truth does not have this attribute.",
+    )
 
 
-class BaseStaticElementData(BaseModel):
+class BaseStaticElementData(ExcludedNoneBaseModel):
 
     boolean: Optional[List[StaticBoolean]] = Field(
         None, description='List of "boolean" that describe this object.'
     )
     num: Optional[List[StaticNum]] = Field(
         None, description='List of "number" that describe this object.'
     )
@@ -298,15 +319,15 @@
         None, description='List of "text" that describe this object.'
     )
     vec: Optional[List[StaticVec]] = Field(
         None, description='List of "vec" that describe this object.'
     )
 
 
-class BaseDynamicElementData(BaseModel):
+class BaseDynamicElementData(ExcludedNoneBaseModel):
 
     boolean: Optional[List[DynamicBoolean]] = Field(
         None, description='List of "boolean" that describe this object.'
     )
     num: Optional[List[DynamicNum]] = Field(
         None, description='List of "number" that describe this object.'
     )
@@ -314,15 +335,15 @@
         None, description='List of "text" that describe this object.'
     )
     vec: Optional[List[DynamicVec]] = Field(
         None, description='List of "vec" that describe this object.'
     )
 
 
-class ElementDataPointer(BaseModel):
+class ElementDataPointer(ExcludedNoneBaseModel):
 
     attributes: Optional[Dict[StrictStr, AttributeType]] = Field(
         None,
         description="This is a JSON object which contains pointers to the attributes of"
         + ' the element data pointed by this pointer. The attributes pointer keys shall be the "name" of the'
         + " attribute of the element data this pointer points to.",
     )
@@ -348,15 +369,15 @@
         extra = Extra.forbid
 
     type: AttributeType = Field(
         ..., description="Type of the element data pointed by this pointer."
     )
 
 
-class Context(BaseModel):
+class Context(ExcludedNoneBaseModel):
     class Config:
         extra = Extra.forbid
 
     frame_intervals: List[FrameInterval] = Field(
         ...,
         description="The array of frame intervals where this object exists or is defined.",
     )
@@ -439,15 +460,15 @@
 
 
 class ObjectDataStatic(BaseStaticElementData):
     class Config:
         extra = Extra.forbid
 
 
-class Object(BaseModel):
+class Object(ExcludedNoneBaseModel):
     class Config:
         extra = Extra.forbid
 
     frame_intervals: List[FrameInterval] = Field(
         ...,
         description="The array of frame intervals where this object exists or is defined.",
     )
@@ -514,92 +535,92 @@
             raise ValueError(
                 f"Dynamic object data pointer {error_name_list}"
                 + " missing frame intervals"
             )
         return values
 
 
-class StreamProperties(BaseModel):
+class StreamProperties(ExcludedNoneBaseModel):
     intrinsics_pinhole: IntrinsicsPinhole
 
 
-class TagData(BaseModel):
+class TagData(ExcludedNoneBaseModel):
     vec: List[StaticVec] = Field(...)
 
     @validator("vec")
     def validate_vec(cls, values):
         assert len(values) == 1, "Only allow one data inside list"
         value = values[0]
         assert value.type == "values", "Value {} is not allowed"
         return values
 
 
-class Stream(BaseModel):
+class Stream(ExcludedNoneBaseModel):
     type: StreamType
     uri: Optional[StrictStr] = ""
     description: Optional[StrictStr] = ""
     stream_properties: Optional[StreamProperties] = None
 
     class Config:
         use_enum_values = True
 
     @validator("stream_properties")
     def validate_stream_properties(cls, value):
         assert value, f"value {value} is not allowed"
         return value
 
 
-class Tag(BaseModel):
+class Tag(ExcludedNoneBaseModel):
     ontology_uid: StrictStr
     type: StrictStr
     tag_data: TagData
 
 
-class TimeStampElement(BaseModel):
+class TimeStampElement(ExcludedNoneBaseModel):
     timestamp: str
 
     class Config:
         extra = Extra.forbid
 
     @validator("timestamp")
     def validate_timestamp(cls, value):
         iso_time_regex = r"^(\d{4})-(\d{2})-(\d{2})T(\d{2}):(\d{2}):(\d{2}\.\d{3})(Z|[+-]((\d{2}:\d{2})|(\d{4})))$"
         assert re.match(iso_time_regex, value), f"Wrong timestamp format : {value}"
         return value
 
 
-class StreamPropertyUnderFrameProperty(BaseModel):
+class StreamPropertyUnderFrameProperty(ExcludedNoneBaseModel):
     sync: Optional[TimeStampElement] = None
 
 
-class FramePropertyStream(BaseModel):
+class FramePropertyStream(ExcludedNoneBaseModel):
     uri: str = Field(description="the urls of image")
     stream_properties: Optional[StreamPropertyUnderFrameProperty] = Field(
         None, description="Additional properties of the stream"
     )
 
     class Config:
         extra = Extra.allow
 
     @validator("stream_properties")
     def validate_stream_properties(cls, value):
         assert value, f"value {value} is not allowed"
         return value
 
 
-class FrameProperties(BaseModel):
+class FrameProperties(ExcludedNoneBaseModel):
     timestamp: Optional[str] = Field(
         None,
         descriptions="A relative or absolute time reference that specifies "
         + "the time instant this frame corresponds to",
     )
     streams: Dict[StrictStr, FramePropertyStream]
 
 
-class ObjectDataElement(BaseModel):
+class ObjectDataElement(ExcludedNoneBaseModel):
 
     attributes: Optional[Attributes] = None
     name: StrictStr = Field(
         description="This is a string encoding the name of this object data."
         + " It is used as index inside the corresponding object data pointers.",
     )
     stream: StrictStr = Field(
@@ -682,15 +703,15 @@
     @validator("name")
     def validate_name_field(cls, value):
         if value != "semantic_mask":
             raise ValueError("Name value must be `semantic_mask`")
         return value
 
 
-class DynamicObjectData(BaseModel):
+class DynamicObjectData(ExcludedNoneBaseModel):
     class Config:
         extra = Extra.forbid
 
     bbox: Optional[List[Bbox]] = Field(
         None, description='List of "bbox" that describe this object.'
     )
     cuboid: Optional[List[Cuboid]] = Field(
@@ -704,23 +725,23 @@
     )
     binary: Optional[List[Binary]] = Field(
         None,
         description='List of "binary" that describe this object semantic mask info.',
     )
 
 
-class ObjectUnderFrame(BaseModel):
+class ObjectUnderFrame(ExcludedNoneBaseModel):
     object_data: DynamicObjectData
 
 
-class ContextUnderFrame(BaseModel):
+class ContextUnderFrame(ExcludedNoneBaseModel):
     context_data: DynamicContextData
 
 
-class Frame(BaseModel):
+class Frame(ExcludedNoneBaseModel):
     class Config:
         extra = Extra.forbid
 
     objects: Optional[Dict[StrictStr, ObjectUnderFrame]] = Field(
         default=None,
         description="This is a JSON object that contains dynamic information on VisionAI objects."
         + " Object keys are strings containing numerical UIDs or 32 bytes UUIDs."
@@ -735,15 +756,15 @@
     )
 
     frame_properties: FrameProperties = Field(
         description="This is a JSON object which contains information about this frame.",
     )
 
 
-class VisionAI(BaseModel):
+class VisionAI(ExcludedNoneBaseModel):
     class Config:
         extra = Extra.forbid
 
     contexts: Optional[Dict[StrictStr, Context]] = Field(
         default=None,
         description="This is the JSON object of VisionAI classified class context."
         + " Object keys are strings containing numerical UIDs or 32 bytes UUIDs.",
@@ -816,15 +837,15 @@
     @validator("tags")
     def validate_tags(cls, value):
 
         assert value, f" Value {value} is not allowed"
         return value
 
 
-class VisionAIModel(BaseModel):
+class VisionAIModel(ExcludedNoneBaseModel):
     class Config:
         extra = Extra.forbid
 
     visionai: VisionAI
 
     def validate_with_ontology(self, ontology: Type[Ontology]) -> List[str]:
```

### Comparing `visionai-data-format-1.0.0/visionai_data_format/utils/checker.py` & `visionai-data-format-1.0.1/visionai_data_format/utils/checker.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/visionai_data_format/utils/classes.py` & `visionai-data-format-1.0.1/visionai_data_format/utils/classes.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/visionai_data_format/utils/converter.py` & `visionai-data-format-1.0.1/visionai_data_format/utils/converter.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/visionai_data_format/utils/resize.py` & `visionai-data-format-1.0.1/visionai_data_format/utils/resize.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/visionai_data_format/utils/validator.py` & `visionai-data-format-1.0.1/visionai_data_format/utils/validator.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/visionai_data_format/vai_to_bdd.py` & `visionai-data-format-1.0.1/visionai_data_format/vai_to_bdd.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/visionai_data_format/vai_to_coco.py` & `visionai-data-format-1.0.1/visionai_data_format/vai_to_coco.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.0/visionai_data_format.egg-info/SOURCES.txt` & `visionai-data-format-1.0.1/visionai_data_format.egg-info/SOURCES.txt`

 * *Files identical despite different names*

