# Comparing `tmp/minot-0.1.1.tar.gz` & `tmp/minot-1.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/minot-0.1.1.tar", last modified: Fri Feb 19 11:15:06 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

