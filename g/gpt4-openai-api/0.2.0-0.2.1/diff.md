# Comparing `tmp/gpt4-openai-api-0.2.0.tar.gz` & `tmp/gpt4-openai-api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gpt4-openai-api-0.2.0.tar", last modified: Thu May 11 20:52:26 2023, max compression
+gzip compressed data, was "dist\gpt4-openai-api-0.2.1.tar", last modified: Thu May 11 21:05:05 2023, max compression
```

## Comparing `gpt4-openai-api-0.2.0.tar` & `gpt4-openai-api-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 20:52:26.288120 gpt4-openai-api-0.2.0/
--rw-rw-rw-   0        0        0      800 2023-05-11 20:52:26.287123 gpt4-openai-api-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-11 20:52:26.250120 gpt4-openai-api-0.2.0/gpt4_openai/
--rw-rw-rw-   0        0        0     2559 2023-05-11 20:46:34.000000 gpt4-openai-api-0.2.0/gpt4_openai/__init__.py
--rw-rw-rw-   0        0        0    24235 2023-05-11 20:46:44.000000 gpt4-openai-api-0.2.0/gpt4_openai/driver.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:52:26.281118 gpt4-openai-api-0.2.0/gpt4_openai_api.egg-info/
--rw-rw-rw-   0        0        0      800 2023-05-11 20:52:26.000000 gpt4-openai-api-0.2.0/gpt4_openai_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-05-11 20:52:26.000000 gpt4-openai-api-0.2.0/gpt4_openai_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 20:52:26.000000 gpt4-openai-api-0.2.0/gpt4_openai_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-05-11 20:52:26.000000 gpt4-openai-api-0.2.0/gpt4_openai_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-11 20:52:26.000000 gpt4-openai-api-0.2.0/gpt4_openai_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 20:52:26.289121 gpt4-openai-api-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      978 2023-05-11 20:51:20.000000 gpt4-openai-api-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:52:26.284120 gpt4-openai-api-0.2.0/test/
--rw-rw-rw-   0        0        0      434 2023-05-11 20:47:25.000000 gpt4-openai-api-0.2.0/test/test.py
--rw-rw-rw-   0        0        0      997 2023-05-07 23:29:24.000000 gpt4-openai-api-0.2.0/test/test_langchain.py
+drwxrwxrwx   0        0        0        0 2023-05-11 21:05:05.873761 gpt4-openai-api-0.2.1/
+-rw-rw-rw-   0        0        0     5123 2023-05-11 21:05:05.871755 gpt4-openai-api-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-11 21:05:05.835759 gpt4-openai-api-0.2.1/gpt4_openai/
+-rw-rw-rw-   0        0        0     2559 2023-05-11 20:46:34.000000 gpt4-openai-api-0.2.1/gpt4_openai/__init__.py
+-rw-rw-rw-   0        0        0    24235 2023-05-11 20:46:44.000000 gpt4-openai-api-0.2.1/gpt4_openai/driver.py
+drwxrwxrwx   0        0        0        0 2023-05-11 21:05:05.865759 gpt4-openai-api-0.2.1/gpt4_openai_api.egg-info/
+-rw-rw-rw-   0        0        0     5123 2023-05-11 21:05:05.000000 gpt4-openai-api-0.2.1/gpt4_openai_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-05-11 21:05:05.000000 gpt4-openai-api-0.2.1/gpt4_openai_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 21:05:05.000000 gpt4-openai-api-0.2.1/gpt4_openai_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-11 21:05:05.000000 gpt4-openai-api-0.2.1/gpt4_openai_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-11 21:05:05.000000 gpt4-openai-api-0.2.1/gpt4_openai_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 21:05:05.873761 gpt4-openai-api-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1232 2023-05-11 21:05:02.000000 gpt4-openai-api-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 21:05:05.869755 gpt4-openai-api-0.2.1/test/
+-rw-rw-rw-   0        0        0      434 2023-05-11 20:47:25.000000 gpt4-openai-api-0.2.1/test/test.py
+-rw-rw-rw-   0        0        0      997 2023-05-07 23:29:24.000000 gpt4-openai-api-0.2.1/test/test_langchain.py
```

### Comparing `gpt4-openai-api-0.2.0/gpt4_openai/__init__.py` & `gpt4-openai-api-0.2.1/gpt4_openai/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt4-openai-api-0.2.0/gpt4_openai/driver.py` & `gpt4-openai-api-0.2.1/gpt4_openai/driver.py`

 * *Files identical despite different names*

### Comparing `gpt4-openai-api-0.2.0/test/test_langchain.py` & `gpt4-openai-api-0.2.1/test/test_langchain.py`

 * *Files identical despite different names*

