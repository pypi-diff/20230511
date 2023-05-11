# Comparing `tmp/t4flib-0.1.2.tar.gz` & `tmp/t4flib-0.1.4-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t4flib-0.1.2.tar", last modified: Thu May 11 19:18:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

