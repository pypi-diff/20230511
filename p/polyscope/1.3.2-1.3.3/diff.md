# Comparing `tmp/polyscope-1.3.2.tar.gz` & `tmp/polyscope-1.3.3-cp39-cp39-macosx_10_9_universal2.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheelhouse/polyscope-1.3.2.tar", last modified: Thu May 11 05:52:24 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

