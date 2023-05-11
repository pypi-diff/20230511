# Comparing `tmp/pytest-wake-0.2.5.tar.gz` & `tmp/pytest_wake-0.3.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-wake-0.2.5.tar", last modified: Wed Sep 28 08:12:30 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

