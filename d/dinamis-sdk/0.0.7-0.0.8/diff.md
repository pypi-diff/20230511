# Comparing `tmp/dinamis-sdk-0.0.7.tar.gz` & `tmp/dinamis-sdk-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dinamis-sdk-0.0.7.tar", last modified: Tue Apr 25 17:30:45 2023, max compression
+gzip compressed data, was "dinamis-sdk-0.0.8.tar", last modified: Thu May 11 10:52:38 2023, max compression
```

## Comparing `dinamis-sdk-0.0.7.tar` & `dinamis-sdk-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:30:45.884950 dinamis-sdk-0.0.7/
--rw-rw-rw-   0 root         (0) root         (0)    11340 2023-02-22 11:50:47.000000 dinamis-sdk-0.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      191 2023-04-25 17:30:45.884950 dinamis-sdk-0.0.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-03-28 12:19:28.000000 dinamis-sdk-0.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:30:45.880950 dinamis-sdk-0.0.7/dinamis_sdk/
--rw-rw-rw-   0 root         (0) root         (0)      194 2023-03-28 09:22:01.000000 dinamis-sdk-0.0.7/dinamis_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8267 2023-03-28 09:22:01.000000 dinamis-sdk-0.0.7/dinamis_sdk/auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:30:45.884950 dinamis-sdk-0.0.7/dinamis_sdk/examples/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-03-31 13:55:36.000000 dinamis-sdk-0.0.7/dinamis_sdk/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-03-30 18:09:54.000000 dinamis-sdk-0.0.7/dinamis_sdk/examples/pyotb_ndvi_loss.py
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-03-30 18:09:54.000000 dinamis-sdk-0.0.7/dinamis_sdk/examples/pyotb_toa_mosaic.py
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-03-30 14:16:11.000000 dinamis-sdk-0.0.7/dinamis_sdk/examples/rio_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    15621 2023-03-28 09:22:01.000000 dinamis-sdk-0.0.7/dinamis_sdk/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     1717 2023-04-25 17:28:43.000000 dinamis-sdk-0.0.7/dinamis_sdk/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:30:45.884950 dinamis-sdk-0.0.7/dinamis_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      191 2023-04-25 17:30:45.000000 dinamis-sdk-0.0.7/dinamis_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2023-04-25 17:30:45.000000 dinamis-sdk-0.0.7/dinamis_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 17:30:45.000000 dinamis-sdk-0.0.7/dinamis_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 17:30:45.000000 dinamis-sdk-0.0.7/dinamis_sdk.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       54 2023-04-25 17:30:45.000000 dinamis-sdk-0.0.7/dinamis_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-25 17:30:45.000000 dinamis-sdk-0.0.7/dinamis_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 17:30:45.884950 dinamis-sdk-0.0.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-04-25 17:28:43.000000 dinamis-sdk-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:52:38.651153 dinamis-sdk-0.0.8/
+-rw-rw-rw-   0 root         (0) root         (0)    11340 2023-02-22 11:50:47.000000 dinamis-sdk-0.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-11 10:52:38.651153 dinamis-sdk-0.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-03-28 12:19:28.000000 dinamis-sdk-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:52:38.647153 dinamis-sdk-0.0.8/dinamis_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-03-28 09:22:01.000000 dinamis-sdk-0.0.8/dinamis_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8267 2023-03-28 09:22:01.000000 dinamis-sdk-0.0.8/dinamis_sdk/auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:52:38.651153 dinamis-sdk-0.0.8/dinamis_sdk/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-03-31 13:55:36.000000 dinamis-sdk-0.0.8/dinamis_sdk/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      920 2023-05-11 10:48:18.000000 dinamis-sdk-0.0.8/dinamis_sdk/examples/pyotb_ndvi_loss.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-05-11 10:48:18.000000 dinamis-sdk-0.0.8/dinamis_sdk/examples/pyotb_toa_mosaic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-03-30 14:16:11.000000 dinamis-sdk-0.0.8/dinamis_sdk/examples/rio_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    16407 2023-05-03 18:09:30.000000 dinamis-sdk-0.0.8/dinamis_sdk/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1717 2023-05-03 18:03:30.000000 dinamis-sdk-0.0.8/dinamis_sdk/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:52:38.647153 dinamis-sdk-0.0.8/dinamis_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-11 10:52:38.000000 dinamis-sdk-0.0.8/dinamis_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2023-05-11 10:52:38.000000 dinamis-sdk-0.0.8/dinamis_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 10:52:38.000000 dinamis-sdk-0.0.8/dinamis_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 10:52:38.000000 dinamis-sdk-0.0.8/dinamis_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       54 2023-05-11 10:52:38.000000 dinamis-sdk-0.0.8/dinamis_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-11 10:52:38.000000 dinamis-sdk-0.0.8/dinamis_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 10:52:38.651153 dinamis-sdk-0.0.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-05-03 18:03:30.000000 dinamis-sdk-0.0.8/setup.py
```

### Comparing `dinamis-sdk-0.0.7/LICENSE` & `dinamis-sdk-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.0.7/README.md` & `dinamis-sdk-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.0.7/dinamis_sdk/auth.py` & `dinamis-sdk-0.0.8/dinamis_sdk/auth.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.0.7/dinamis_sdk/examples/pyotb_ndvi_loss.py` & `dinamis-sdk-0.0.8/dinamis_sdk/examples/pyotb_ndvi_loss.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 from dinamis_sdk import sign_inplace
 
 api = Client.open(
     'https://stacapi-dinamis.apps.okd.crocc.meso.umontpellier.fr',
     modifier=sign_inplace
 )
 
-bbox = [4, 42.99, 5, 44.05]
-
 
 def mosa(year):
     """Return a pyotb application that perform a mosaic."""
-    res = api.search(bbox=bbox, datetime=[f'{year}-01-01', f'{year}-12-25'])
+    res = api.search(
+        bbox=[4, 42.99, 5, 44.05],
+        datetime=[f"{year}-01-01", f"{year}-12-25"],
+        collections=["spot-6-7-drs"]
+    )
     urls = [f"/vsicurl/{r.assets['src_xs'].href}" for r in res.items()]
     return pyotb.Mosaic({"il": urls})
 
 
 def ndvi(xs):
     """Return a pyotb application that computes NDVI."""
     return pyotb.BandMath({"il": [xs], "exp": "(im1b4-im1b1)/(im1b4+im1b1)"})
 
 
-ndvi_22 = ndvi(mosa('2022'))
-ndvi_21 = ndvi(mosa('2021'))
+ndvi_22 = ndvi(mosa("2022"))
+ndvi_21 = ndvi(mosa("2021"))
 delta_ndvi = ndvi_22 - pyotb.Superimpose({"inr": ndvi_22, "inm": ndvi_21})
 delta_ndvi.write("ndvi_loss.tif?&box=5000:5000:4096:4096")
```

### Comparing `dinamis-sdk-0.0.7/dinamis_sdk/examples/rio_metadata.py` & `dinamis-sdk-0.0.8/dinamis_sdk/examples/rio_metadata.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.0.7/dinamis_sdk/s3.py` & `dinamis-sdk-0.0.8/dinamis_sdk/s3.py`

 * *Files 3% similar despite different names*

```diff
@@ -396,15 +396,15 @@
 
 sign_reference_file = sign_mapping
 
 
 def get_signed_urls(
         urls: List[str],
         retry_total: int = 10,
-        retry_backoff_factor: float = 0.8
+        retry_backoff_factor: float = .8
 ) -> Dict[str, SignedURL]:
     """
     Get multiple signed URLs.
 
     This will use the URL from the cache if it's present and not too close
     to expiring. The generated URL will be placed in the cache.
 
@@ -443,45 +443,60 @@
         log.debug(
             "Access token: %s...%s", access_token[:8], access_token[-8:]
         )
     signed_urls = {}
     for url in urls:
         signed_url_in_cache = CACHE.get(url)
         if signed_url_in_cache:
-            if signed_url_in_cache.ttl() > SIGNED_URL_TTL_MARGIN:
+            log.debug("URL %s already in cache", url)
+            ttl = signed_url_in_cache.ttl()
+            log.debug("URL %s TTL is %s", url, ttl)
+            if ttl > SIGNED_URL_TTL_MARGIN:
+                log.debug("Using cache (%s > %s)", ttl, SIGNED_URL_TTL_MARGIN)
                 signed_urls[url] = signed_url_in_cache
     not_signed_urls = [url for url in urls if url not in signed_urls]
     log.debug("Already signed URLs:\n %s", signed_urls)
-    # Refresh the token if there's less than SIGNED_URL_TTL_MARGIN seconds
-    # remaining, in order to give a small amount of time to do stuff with the
-    # url
-    session = requests.Session()
-    retry = urllib3.util.retry.Retry(
-        total=retry_total,
-        backoff_factor=retry_backoff_factor,
-    )
-    adapter = requests.adapters.HTTPAdapter(max_retries=retry)
-    session.mount("http://", adapter)
-    session.mount("https://", adapter)
-    response = session.post(
-        f"{S3_SIGNING_ENDPOINT}sign_urls",
-        params={"urls": not_signed_urls},
-        headers=headers
-    )
-    response.raise_for_status()
-
-    signed_url_batch = SignedURLBatch(**response.json())
-    if not signed_url_batch:
-        raise ValueError(
-            f"No signed url batch found in response: {response.json()}"
+    log.debug("Not signed URLs:\n %s", not_signed_urls)
+
+    if not_signed_urls:
+        # Refresh the token if there's less than SIGNED_URL_TTL_MARGIN seconds
+        # remaining, in order to give a small amount of time to do stuff with
+        # the url
+        session = requests.Session()
+        retry = urllib3.util.retry.Retry(
+            total=retry_total,
+            backoff_factor=retry_backoff_factor,
+            status_forcelist=[404, 429, 500, 502, 503, 504],
+            allowed_methods=False,
+        )
+        adapter = requests.adapters.HTTPAdapter(max_retries=retry)
+        session.mount("http://", adapter)
+        session.mount("https://", adapter)
+        response = session.post(
+            f"{S3_SIGNING_ENDPOINT}sign_urls",
+            params={"urls": not_signed_urls},
+            headers=headers
+        )
+        response.raise_for_status()
+
+        signed_url_batch = SignedURLBatch(**response.json())
+        if not signed_url_batch:
+            raise ValueError(
+                f"No signed url batch found in response: {response.json()}"
+            )
+        if not all(key in signed_url_batch.hrefs
+                   for key in not_signed_urls):
+            raise ValueError(
+                f"URLs to sign are {not_signed_urls} but returned signed URLs"
+                f"are for {signed_url_batch.hrefs.keys()}"
+            )
+        for url, href in signed_url_batch.hrefs.items():
+            signed_url = SignedURL(expiry=signed_url_batch.expiry, href=href)
+            CACHE[url] = signed_url
+            signed_urls[url] = signed_url
+        log.debug(
+            "Got signed urls %s in %s seconds",
+            signed_urls,
+            f"{time.time() - start_time:.2f}"
         )
-    for url, href in signed_url_batch.hrefs.items():
-        signed_url = SignedURL(expiry=signed_url_batch.expiry, href=href)
-        CACHE[url] = signed_url
-        signed_urls[url] = signed_url
-    log.debug(
-        "Got signed urls %s in %s seconds",
-        signed_urls,
-        f"{time.time() - start_time:.2f}"
-    )
 
     return signed_urls
```

### Comparing `dinamis-sdk-0.0.7/dinamis_sdk/utils.py` & `dinamis-sdk-0.0.8/dinamis_sdk/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Some helpers."""
-import appdirs
 import json
 import logging
 import os
+import appdirs
 from pydantic import BaseModel  # pylint: disable = no-name-in-module
 
 logging.basicConfig(level=os.environ.get("LOGLEVEL") or "INFO")
 log = logging.getLogger("dinamis_sdk")
 
 # Signed TTL margin default to 1800 seconds (30 minutes), or env. var.
 ttl_margin_from_env = os.environ.get("DINAMIS_SDK_TTL_MARGIN")
```

