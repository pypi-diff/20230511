# Comparing `tmp/symba-2.1.0.tar.gz` & `tmp/symba-2.2.0-cp310-cp310-musllinux_1_1_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symba-2.1.0.tar", last modified: Wed Apr  5 00:27:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

