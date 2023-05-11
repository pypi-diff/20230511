# Comparing `tmp/ogc_na-0.2.3.tar.gz` & `tmp/ogc_na-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogc_na-0.2.3.tar", last modified: Thu May 11 16:30:41 2023, max compression
+gzip compressed data, was "ogc_na-0.2.4.tar", last modified: Thu May 11 16:45:05 2023, max compression
```

## Comparing `ogc_na-0.2.3.tar` & `ogc_na-0.2.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:30:41.339887 ogc_na-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:30:41.323887 ogc_na-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:30:41.327887 ogc_na-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-11 16:30:26.000000 ogc_na-0.2.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-11 16:30:26.000000 ogc_na-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-11 16:30:26.000000 ogc_na-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-11 16:30:41.339887 ogc_na-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-11 16:30:26.000000 ogc_na-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:30:41.327887 ogc_na-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-05-11 16:30:26.000000 ogc_na-0.2.3/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-11 16:30:26.000000 ogc_na-0.2.3/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-11 16:30:26.000000 ogc_na-0.2.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-11 16:30:26.000000 ogc_na-0.2.3/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-11 16:30:26.000000 ogc_na-0.2.3/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:30:41.323887 ogc_na-0.2.3/ogc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:30:41.331887 ogc_na-0.2.3/ogc/na/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-11 16:30:26.000000 ogc_na-0.2.3/ogc/na/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21506 2023-05-11 16:30:26.000000 ogc_na-0.2.3/ogc/na/annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-05-11 16:30:26.000000 ogc_na-0.2.3/ogc/na/domain_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-11 16:30:26.000000 ogc_na-0.2.3/ogc/na/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    31936 2023-05-11 16:30:26.000000 ogc_na-0.2.3/ogc/na/ingest_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:30:41.331887 ogc_na-0.2.3/ogc/na/input_filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-11 16:30:26.000000 ogc_na-0.2.3/ogc/na/input_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-11 16:30:26.000000 ogc_na-0.2.3/ogc/na/input_filters/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-05-11 16:30:26.000000 ogc_na-0.2.3/ogc/na/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-11 16:30:26.000000 ogc_na-0.2.3/ogc/na/provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    17028 2023-05-11 16:30:26.000000 ogc_na-0.2.3/ogc/na/update_vocabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-05-11 16:30:26.000000 ogc_na-0.2.3/ogc/na/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-11 16:30:26.000000 ogc_na-0.2.3/ogc/na/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:30:41.331887 ogc_na-0.2.3/ogc_na.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-11 16:30:41.000000 ogc_na-0.2.3/ogc_na.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-11 16:30:41.000000 ogc_na-0.2.3/ogc_na.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:30:41.000000 ogc_na-0.2.3/ogc_na.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-11 16:30:41.000000 ogc_na-0.2.3/ogc_na.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-11 16:30:41.000000 ogc_na-0.2.3/ogc_na.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-11 16:30:26.000000 ogc_na-0.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:30:41.335887 ogc_na-0.2.3/rdf/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-11 16:30:26.000000 ogc_na-0.2.3/rdf/catalog-v001.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-11 16:30:26.000000 ogc_na-0.2.3/rdf/domaincfg.vocab.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-11 16:30:26.000000 ogc_na-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:30:41.339887 ogc_na-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-11 16:30:26.000000 ogc_na-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:30:41.335887 ogc_na-0.2.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:30:26.000000 ogc_na-0.2.3/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:30:41.339887 ogc_na-0.2.3/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:30:26.000000 ogc_na-0.2.3/test/data/empty.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-11 16:30:26.000000 ogc_na-0.2.3/test/data/headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-11 16:30:26.000000 ogc_na-0.2.3/test/data/no-headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-11 16:30:26.000000 ogc_na-0.2.3/test/data/profile_tree.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-11 16:30:26.000000 ogc_na-0.2.3/test/data/profile_tree_cyclic.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-11 16:30:26.000000 ogc_na-0.2.3/test/data/sample-context.jsonld
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-11 16:30:26.000000 ogc_na-0.2.3/test/data/sample-schema-prop-c.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-11 16:30:26.000000 ogc_na-0.2.3/test/data/sample-schema.yml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-11 16:30:26.000000 ogc_na-0.2.3/test/data/uplift_context_valid.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-11 16:30:26.000000 ogc_na-0.2.3/test/test_annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-11 16:30:26.000000 ogc_na-0.2.3/test/test_ingest_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-11 16:30:26.000000 ogc_na-0.2.3/test/test_input_filters_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-11 16:30:26.000000 ogc_na-0.2.3/test/test_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:05.756099 ogc_na-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:05.752099 ogc_na-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:05.752099 ogc_na-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-11 16:44:52.000000 ogc_na-0.2.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-11 16:44:52.000000 ogc_na-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-11 16:44:52.000000 ogc_na-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-11 16:45:05.756099 ogc_na-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-11 16:44:52.000000 ogc_na-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:05.752099 ogc_na-0.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-05-11 16:44:52.000000 ogc_na-0.2.4/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-11 16:44:52.000000 ogc_na-0.2.4/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-11 16:44:52.000000 ogc_na-0.2.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-11 16:44:52.000000 ogc_na-0.2.4/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-11 16:44:52.000000 ogc_na-0.2.4/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:05.752099 ogc_na-0.2.4/ogc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:05.756099 ogc_na-0.2.4/ogc/na/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-11 16:44:52.000000 ogc_na-0.2.4/ogc/na/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21506 2023-05-11 16:44:52.000000 ogc_na-0.2.4/ogc/na/annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-05-11 16:44:52.000000 ogc_na-0.2.4/ogc/na/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-11 16:44:52.000000 ogc_na-0.2.4/ogc/na/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31936 2023-05-11 16:44:52.000000 ogc_na-0.2.4/ogc/na/ingest_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:05.756099 ogc_na-0.2.4/ogc/na/input_filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-11 16:44:52.000000 ogc_na-0.2.4/ogc/na/input_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-11 16:44:52.000000 ogc_na-0.2.4/ogc/na/input_filters/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-05-11 16:44:52.000000 ogc_na-0.2.4/ogc/na/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-11 16:44:52.000000 ogc_na-0.2.4/ogc/na/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17472 2023-05-11 16:44:52.000000 ogc_na-0.2.4/ogc/na/update_vocabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-05-11 16:44:52.000000 ogc_na-0.2.4/ogc/na/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-11 16:44:52.000000 ogc_na-0.2.4/ogc/na/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:05.756099 ogc_na-0.2.4/ogc_na.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-11 16:45:05.000000 ogc_na-0.2.4/ogc_na.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-11 16:45:05.000000 ogc_na-0.2.4/ogc_na.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:45:05.000000 ogc_na-0.2.4/ogc_na.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-11 16:45:05.000000 ogc_na-0.2.4/ogc_na.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-11 16:45:05.000000 ogc_na-0.2.4/ogc_na.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-11 16:44:52.000000 ogc_na-0.2.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:05.756099 ogc_na-0.2.4/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-11 16:44:52.000000 ogc_na-0.2.4/rdf/catalog-v001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-11 16:44:52.000000 ogc_na-0.2.4/rdf/domaincfg.vocab.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-11 16:44:52.000000 ogc_na-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:45:05.756099 ogc_na-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-11 16:44:52.000000 ogc_na-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:05.756099 ogc_na-0.2.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:44:52.000000 ogc_na-0.2.4/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:45:05.756099 ogc_na-0.2.4/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:44:52.000000 ogc_na-0.2.4/test/data/empty.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-11 16:44:52.000000 ogc_na-0.2.4/test/data/headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-11 16:44:52.000000 ogc_na-0.2.4/test/data/no-headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-11 16:44:52.000000 ogc_na-0.2.4/test/data/profile_tree.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-11 16:44:52.000000 ogc_na-0.2.4/test/data/profile_tree_cyclic.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-11 16:44:52.000000 ogc_na-0.2.4/test/data/sample-context.jsonld
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-11 16:44:52.000000 ogc_na-0.2.4/test/data/sample-schema-prop-c.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-11 16:44:52.000000 ogc_na-0.2.4/test/data/sample-schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-11 16:44:52.000000 ogc_na-0.2.4/test/data/uplift_context_valid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-11 16:44:52.000000 ogc_na-0.2.4/test/test_annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-11 16:44:52.000000 ogc_na-0.2.4/test/test_ingest_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-11 16:44:52.000000 ogc_na-0.2.4/test/test_input_filters_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-11 16:44:52.000000 ogc_na-0.2.4/test/test_profile.py
```

### Comparing `ogc_na-0.2.3/.github/workflows/python-publish.yml` & `ogc_na-0.2.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/.gitignore` & `ogc_na-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/PKG-INFO` & `ogc_na-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc_na
-Version: 0.2.3
+Version: 0.2.4
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.2.3/README.md` & `ogc_na-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/docs/examples.md` & `ogc_na-0.2.4/docs/examples.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/docs/gen_ref_pages.py` & `ogc_na-0.2.4/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/docs/index.md` & `ogc_na-0.2.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/docs/tutorials.md` & `ogc_na-0.2.4/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/mkdocs.yml` & `ogc_na-0.2.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/ogc/na/annotate_schema.py` & `ogc_na-0.2.4/ogc/na/annotate_schema.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/ogc/na/domain_config.py` & `ogc_na-0.2.4/ogc/na/domain_config.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/ogc/na/download.py` & `ogc_na-0.2.4/ogc/na/download.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/ogc/na/ingest_json.py` & `ogc_na-0.2.4/ogc/na/ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/ogc/na/input_filters/__init__.py` & `ogc_na-0.2.4/ogc/na/input_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/ogc/na/input_filters/csv.py` & `ogc_na-0.2.4/ogc/na/input_filters/csv.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/ogc/na/profile.py` & `ogc_na-0.2.4/ogc/na/profile.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/ogc/na/provenance.py` & `ogc_na-0.2.4/ogc/na/provenance.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/ogc/na/update_vocabs.py` & `ogc_na-0.2.4/ogc/na/update_vocabs.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from datetime import datetime
 from pathlib import Path
 from typing import Union, Generator
 
 import requests
 from rdflib import Graph, RDF, SKOS
 
+from ogc.na import util
 from ogc.na.domain_config import DomainConfiguration, DomainConfigurationEntry
 from ogc.na.profile import ProfileRegistry
 from ogc.na.provenance import generate_provenance, ProvenanceMetadata, FileProvenanceMetadata
 
 logger = logging.getLogger('ogc.na.update_vocabs')
 
 ENTAILED_FORMATS = [
@@ -262,15 +263,15 @@
         help="Update triplestore",
     )
 
     parser.add_argument(
         "-b",
         "--batch",
         action='store_true',
-        help="Batch entail all vocabs ( use -f to force overwrite of existing entailments )",
+        help="Batch entail all vocabs",
     )
 
     parser.add_argument(
         "-s",
         "--graph-store",
         default=os.environ.get("SPARQL_ENDPOINT"),
         help="SPARQL Graph Store-compatible endpoint (when --update enabled)"
@@ -315,14 +316,20 @@
 
     parser.add_argument(
         '--base-uri',
         default='https://raw.githubusercontent.com/opengeospatial/NamingAuthority/master/',
         help='Base URI for provenance metadata',
     )
 
+    parser.add_argument(
+        '--use-git-status',
+        action='store_true',
+        help='Use git status for obtaining batch filenames'
+    )
+
     args = parser.parse_args()
 
     setup_logging(args.debug)
 
     graph_store = args.graph_store or os.environ.get('SPARQL_GRAPH_STORE')
 
     if args.update and not graph_store:
@@ -335,25 +342,31 @@
 
     if graph_store:
         logger.info(f"Using SPARQL graph store %s with{'' if authdetails else 'out'} authentication", graph_store)
 
     mod_list = []
     add_list = []
 
-    if args.modified:
-        mod_list = args.modified.split(",")
-        logger.info("Modified: %s", mod_list)
-
-    if args.added:
-        add_list = args.added.split(",")
-        logger.info("Added: %s", add_list)
-
-    if args.removed:
-        dellist = args.removed.split(',')
-        logger.info("Removed: %s", dellist)
+    if args.use_git_status:
+        git_status = util.git_status()
+        add_list = git_status['added']
+        mod_list = git_status['modified'] + [r[1] for r in git_status['renamed']]
+        logger.info("Using git status\n - added: %s\n - modified: %s", add_list, mod_list)
+    else:
+        if args.modified:
+            mod_list = args.modified.split(",")
+            logger.info("Modified: %s", mod_list)
+
+        if args.added:
+            add_list = args.added.split(",")
+            logger.info("Added: %s", add_list)
+
+        if args.removed:
+            dellist = args.removed.split(',')
+            logger.info("Removed: %s", dellist)
 
     domain_cfg = DomainConfiguration(args.domain_cfg, working_directory=args.working_directory)
     cfg_entries = domain_cfg.entries
     if not len(cfg_entries):
         if args.domain:
             logger.warning('No configuration found in %s for domain %s, exiting',
                            args.domain_cfg, args.domain)
```

### Comparing `ogc_na-0.2.3/ogc/na/util.py` & `ogc_na-0.2.4/ogc/na/util.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/ogc/na/validation.py` & `ogc_na-0.2.4/ogc/na/validation.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/ogc_na.egg-info/PKG-INFO` & `ogc_na-0.2.4/ogc_na.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc-na
-Version: 0.2.3
+Version: 0.2.4
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.2.3/ogc_na.egg-info/SOURCES.txt` & `ogc_na-0.2.4/ogc_na.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/pyproject.toml` & `ogc_na-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/rdf/domaincfg.vocab.ttl` & `ogc_na-0.2.4/rdf/domaincfg.vocab.ttl`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/test/data/headers.csv` & `ogc_na-0.2.4/test/data/headers.csv`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/test/data/uplift_context_valid.yml` & `ogc_na-0.2.4/test/data/uplift_context_valid.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/test/test_annotate_schema.py` & `ogc_na-0.2.4/test/test_annotate_schema.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/test/test_ingest_json.py` & `ogc_na-0.2.4/test/test_ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/test/test_input_filters_csv.py` & `ogc_na-0.2.4/test/test_input_filters_csv.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.3/test/test_profile.py` & `ogc_na-0.2.4/test/test_profile.py`

 * *Files identical despite different names*

