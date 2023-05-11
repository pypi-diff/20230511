# Comparing `tmp/klassez-0.1a2.tar.gz` & `tmp/klassez-0.2a0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klassez-0.1a2.tar", last modified: Wed Apr 19 14:11:01 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

