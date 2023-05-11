# Comparing `tmp/duckduckgo_search-2.9.3.tar.gz` & `tmp/duckduckgo_search-2.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-2.9.3.tar", last modified: Thu May  4 16:32:07 2023, max compression
+gzip compressed data, was "duckduckgo_search-2.9.4.tar", last modified: Thu May 11 20:07:21 2023, max compression
```

## Comparing `duckduckgo_search-2.9.3.tar` & `duckduckgo_search-2.9.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:32:07.790330 duckduckgo_search-2.9.3/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-05-04 16:32:07.790330 duckduckgo_search-2.9.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    34567 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:32:07.790330 duckduckgo_search-2.9.3/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:32:07.790330 duckduckgo_search-2.9.3/duckduckgo_search/cli/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10405 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/cli/ddgs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6254 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/ddg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2750 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/ddg_answers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6457 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/ddg_images.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7090 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/ddg_maps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3855 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/ddg_news.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1005 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/ddg_suggestions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1550 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/ddg_translate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3976 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/ddg_videos.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3841 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:32:07.790330 duckduckgo_search-2.9.3/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-05-04 16:32:07.000000 duckduckgo_search-2.9.3/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-04 16:32:07.000000 duckduckgo_search-2.9.3/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:32:07.000000 duckduckgo_search-2.9.3/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 16:32:07.000000 duckduckgo_search-2.9.3/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-04 16:32:07.000000 duckduckgo_search-2.9.3/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 16:32:07.000000 duckduckgo_search-2.9.3/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 16:32:07.790330 duckduckgo_search-2.9.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:32:07.790330 duckduckgo_search-2.9.3/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1619 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/tests/test_ddg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/tests/test_ddg_answers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2510 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/tests/test_ddg_images.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      418 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/tests/test_ddg_maps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/tests/test_ddg_news.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/tests/test_ddg_suggestions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/tests/test_ddg_translate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-05-04 16:31:47.000000 duckduckgo_search-2.9.3/tests/test_ddg_videos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:07:21.352626 duckduckgo_search-2.9.4/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-05-11 20:07:21.352626 duckduckgo_search-2.9.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34567 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:07:21.348626 duckduckgo_search-2.9.4/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:07:21.348626 duckduckgo_search-2.9.4/duckduckgo_search/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10405 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/cli/ddgs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6309 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/ddg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2856 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/ddg_answers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6557 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/ddg_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7190 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/ddg_maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3953 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/ddg_news.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1062 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/ddg_suggestions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1605 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/ddg_translate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4076 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/ddg_videos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3939 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:07:21.348626 duckduckgo_search-2.9.4/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-05-11 20:07:21.000000 duckduckgo_search-2.9.4/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-11 20:07:21.000000 duckduckgo_search-2.9.4/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:07:21.000000 duckduckgo_search-2.9.4/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-11 20:07:21.000000 duckduckgo_search-2.9.4/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 20:07:21.000000 duckduckgo_search-2.9.4/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 20:07:21.000000 duckduckgo_search-2.9.4/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:07:21.352626 duckduckgo_search-2.9.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:07:21.352626 duckduckgo_search-2.9.4/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1619 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/tests/test_ddg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/tests/test_ddg_answers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2510 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/tests/test_ddg_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      418 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/tests/test_ddg_maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/tests/test_ddg_news.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/tests/test_ddg_suggestions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/tests/test_ddg_translate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-05-11 20:06:58.000000 duckduckgo_search-2.9.4/tests/test_ddg_videos.py
```

### Comparing `duckduckgo_search-2.9.3/LICENSE.md` & `duckduckgo_search-2.9.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.3/PKG-INFO` & `duckduckgo_search-2.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 2.9.3
+Version: 2.9.4
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-2.9.3/README.md` & `duckduckgo_search-2.9.4/README.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.3/duckduckgo_search/__init__.py` & `duckduckgo_search-2.9.4/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.3/duckduckgo_search/cli/ddgs.py` & `duckduckgo_search-2.9.4/duckduckgo_search/cli/ddgs.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.3/duckduckgo_search/ddg.py` & `duckduckgo_search-2.9.4/duckduckgo_search/ddg.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,17 @@
         page_data = None
         for i in range(2):
             try:
                 resp = SESSION.get("https://links.duckduckgo.com/d.js", params=payload)
                 resp.raise_for_status()
                 page_data = resp.json().get("results", None)
                 break
-            except Exception:
-                logger.exception("")
+            except Exception as ex:
+                logger.debug(f"get_ddg_page() {keywords=} {type(ex).__name__} {ex}")
+
                 if i == 1 and not max_results:
                     return None
                 if "506-00.js" in resp.url:
                     payload["vqd"] = _refresh_vqd(keywords)
 
         page_results = []
         if page_data:
```

### Comparing `duckduckgo_search-2.9.3/duckduckgo_search/ddg_answers.py` & `duckduckgo_search-2.9.4/duckduckgo_search/ddg_answers.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,16 +32,16 @@
         "format": "json",
     }
     page_data = []
     try:
         resp = SESSION.get("https://api.duckduckgo.com/", params=payload)
         resp.raise_for_status()
         page_data = resp.json()
-    except Exception:
-        logger.exception("")
+    except Exception as ex:
+        logger.debug(f"ddg_answers() {keywords=} {type(ex).__name__} {ex}")
     if page_data:
         answer = page_data.get("AbstractText", None)
         if answer:
             results.append(
                 {
                     "icon": None,
                     "text": answer,
@@ -57,16 +57,16 @@
             "format": "json",
         }
         page_data = []
         try:
             resp = SESSION.get("https://api.duckduckgo.com/", params=payload)
             resp.raise_for_status()
             page_data = resp.json().get("RelatedTopics", [])
-        except Exception:
-            logger.exception("")
+        except Exception as ex:
+            logger.debug(f"ddg_answers() {keywords=} {type(ex).__name__} {ex}")
 
         for i, row in enumerate(page_data):
             topic = row.get("Name", None)
             if not topic:
                 icon = row["Icon"].get("URL", None)
                 results.append(
                     {
```

### Comparing `duckduckgo_search-2.9.3/duckduckgo_search/ddg_images.py` & `duckduckgo_search-2.9.4/duckduckgo_search/ddg_images.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,16 +60,19 @@
         page_data = None
         for i in range(2):
             try:
                 resp = SESSION.get("https://duckduckgo.com/i.js", params=payload)
                 resp.raise_for_status()
                 page_data = resp.json().get("results", None)
                 break
-            except Exception:
-                logger.exception("")
+            except Exception as ex:
+                logger.debug(
+                    f"get_ddg_images_page() {keywords=} {type(ex).__name__} {ex}"
+                )
+
                 if i == 1 and not max_results:
                     return None
                 if "506-00.js" in resp.url:
                     payload["vqd"] = _refresh_vqd(keywords)
 
         page_results = []
         if page_data:
```

### Comparing `duckduckgo_search-2.9.3/duckduckgo_search/ddg_maps.py` & `duckduckgo_search-2.9.4/duckduckgo_search/ddg_maps.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,16 +110,16 @@
                 params=params,
                 headers=headers,
             )
             resp.raise_for_status()
             coordinates = resp.json()[0]["boundingbox"]
             lat_t, lon_l = Decimal(coordinates[1]), Decimal(coordinates[2])
             lat_b, lon_r = Decimal(coordinates[0]), Decimal(coordinates[3])
-        except Exception:
-            logger.exception("")
+        except Exception as ex:
+            logger.debug(f"ddg_maps() {keywords=} {type(ex).__name__} {ex}")
             return
 
     # if a radius is specified, expand the search square
     lat_t += Decimal(radius) * Decimal(0.008983)
     lat_b -= Decimal(radius) * Decimal(0.008983)
     lon_l -= Decimal(radius) * Decimal(0.008983)
     lon_r += Decimal(radius) * Decimal(0.008983)
@@ -147,16 +147,16 @@
             "strict_bbox": "1",
         }
         page_data = None
         try:
             resp = SESSION.get("https://duckduckgo.com/local.js", params=params)
             resp.raise_for_status()
             page_data = resp.json()["results"]
-        except Exception:
-            logger.exception("")
+        except Exception as ex:
+            logger.debug(f"ddg_maps() {keywords=} {type(ex).__name__} {ex}")
             break
 
         if not page_data:
             break
 
         for res in page_data:
             result = MapsResult()
```

### Comparing `duckduckgo_search-2.9.3/duckduckgo_search/ddg_news.py` & `duckduckgo_search-2.9.4/duckduckgo_search/ddg_news.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,19 @@
         page_data = None
         for i in range(2):
             try:
                 resp = SESSION.get("https://duckduckgo.com/news.js", params=payload)
                 resp.raise_for_status()
                 page_data = resp.json().get("results", None)
                 break
-            except Exception:
-                logger.exception("")
+            except Exception as ex:
+                logger.debug(
+                    f"get_ddg_news_page() {keywords=} {type(ex).__name__} {ex}"
+                )
+
                 if i == 1 and not max_results:
                     return None
                 if "506-00.js" in resp.url:
                     payload["vqd"] = _refresh_vqd(keywords)
 
         page_results = []
         if page_data:
```

### Comparing `duckduckgo_search-2.9.3/duckduckgo_search/ddg_suggestions.py` & `duckduckgo_search-2.9.4/duckduckgo_search/ddg_suggestions.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,14 +31,14 @@
         "q": keywords,
         "kl": region,
     }
     try:
         resp = SESSION.get("https://duckduckgo.com/ac", params=payload)
         resp.raise_for_status()
         results = resp.json()
-    except Exception:
-        logger.exception("")
+    except Exception as ex:
+        logger.debug(f"ddg_suggestions() {keywords=} {type(ex).__name__} {ex}")
 
     if output:
         _do_output("ddg_suggestions", keywords, output, results)
 
     return results
```

### Comparing `duckduckgo_search-2.9.3/duckduckgo_search/ddg_translate.py` & `duckduckgo_search-2.9.4/duckduckgo_search/ddg_translate.py`

 * *Files 14% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                 params=payload,
                 data=data.encode("utf-8"),
             )
             resp.raise_for_status()
             result = resp.json()
             result["original"] = data
             results.append(result)
-        except Exception:
+        except Exception as ex:
             VQD_CACHE.pop("translate", None)
-            logger.exception("")
+            logger.debug(f"ddg_translate() {keywords=} {type(ex).__name__} {ex}")
 
     if output:
         keywords = keywords[0]
         _do_output("ddg_translate", keywords, output, results)
     return results
```

### Comparing `duckduckgo_search-2.9.3/duckduckgo_search/ddg_videos.py` & `duckduckgo_search-2.9.4/duckduckgo_search/ddg_videos.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,16 +43,19 @@
         page_data = None
         for i in range(2):
             try:
                 resp = SESSION.get("https://duckduckgo.com/v.js", params=payload)
                 resp.raise_for_status()
                 page_data = resp.json().get("results", None)
                 break
-            except Exception:
-                logger.exception("")
+            except Exception as ex:
+                logger.debug(
+                    f"get_ddg_videos_page() {keywords=} {type(ex).__name__} {ex}"
+                )
+
                 if i == 1 and not max_results:
                     return None
                 if "506-00.js" in resp.url:
                     payload["vqd"] = _refresh_vqd(keywords)
 
         page_results = []
         if page_data:
```

### Comparing `duckduckgo_search-2.9.3/duckduckgo_search/utils.py` & `duckduckgo_search-2.9.4/duckduckgo_search/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,24 +44,24 @@
         return vqd_bytes.decode()
 
     payload = {"q": keywords}
     for _ in range(2):
         try:
             resp = SESSION.post("https://duckduckgo.com", data=payload, timeout=10)
             resp.raise_for_status()
-            vqd_index_start = resp.content.index(b"vqd='") + 5
-            vqd_index_end = resp.content.index(b"'", vqd_index_start)
+            vqd_index_start = resp.content.index(b'vqd="') + 5
+            vqd_index_end = resp.content.index(b'"', vqd_index_start)
             vqd_bytes = resp.content[vqd_index_start:vqd_index_end]
 
             if vqd_bytes:
                 VQD_CACHE[keywords] = vqd_bytes
                 return vqd_bytes.decode()
 
-        except Exception:
-            logger.exception("")
+        except Exception as ex:
+            logger.info(f"_get_vqd() {keywords=} {type(ex).__name__} {ex}")
 
         # refresh SESSION if not vqd
         prev_proxies = SESSION.proxies
         SESSION = requests.Session()
         SESSION.headers = HEADERS
         SESSION.proxies = prev_proxies
         logger.warning("keywords=%s. _get_vqd() is None, refreshing SESSION", keywords)
@@ -99,16 +99,16 @@
             url, headers=HEADERS_FILE_DOWNLOAD, stream=True, timeout=10
         ) as resp:
             resp.raise_for_status()
             resp.raw.decode_content = True
             with open(os.path.join(dir_path, filename), "wb") as file:
                 copyfileobj(resp.raw, file)
             logger.info(f"File downloaded {url}")
-    except Exception:
-        logger.exception("")
+    except Exception as ex:
+        logger.debug(f"_download_file {url=} {type(ex).__name__} {ex}")
 
 
 def _normalize(raw_html):
     """strip HTML tags"""
     if raw_html:
         return unescape(re.sub(RE_STRIP_TAGS, "", raw_html))
```

### Comparing `duckduckgo_search-2.9.3/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-2.9.4/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo-search
-Version: 2.9.3
+Version: 2.9.4
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-2.9.3/duckduckgo_search.egg-info/SOURCES.txt` & `duckduckgo_search-2.9.4/duckduckgo_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.3/pyproject.toml` & `duckduckgo_search-2.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.3/tests/test_ddg.py` & `duckduckgo_search-2.9.4/tests/test_ddg.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.3/tests/test_ddg_answers.py` & `duckduckgo_search-2.9.4/tests/test_ddg_answers.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.3/tests/test_ddg_images.py` & `duckduckgo_search-2.9.4/tests/test_ddg_images.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.3/tests/test_ddg_news.py` & `duckduckgo_search-2.9.4/tests/test_ddg_news.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.3/tests/test_ddg_suggestions.py` & `duckduckgo_search-2.9.4/tests/test_ddg_suggestions.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.3/tests/test_ddg_translate.py` & `duckduckgo_search-2.9.4/tests/test_ddg_translate.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.9.3/tests/test_ddg_videos.py` & `duckduckgo_search-2.9.4/tests/test_ddg_videos.py`

 * *Files identical despite different names*

