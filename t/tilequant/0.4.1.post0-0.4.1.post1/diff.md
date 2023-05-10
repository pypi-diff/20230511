# Comparing `tmp/tilequant-0.4.1.post0.tar.gz` & `tmp/tilequant-0.4.1.post1-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tilequant-0.4.1.post0.tar", last modified: Sat Nov  5 15:12:29 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

