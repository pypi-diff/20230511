# Comparing `tmp/snakeML-0.0.4.tar.gz` & `tmp/snakeML-0.0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakeML-0.0.4.tar", last modified: Mon Mar 20 22:23:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

