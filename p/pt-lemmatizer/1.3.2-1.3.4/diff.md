# Comparing `tmp/pt_lemmatizer-1.3.2.tar.gz` & `tmp/pt_lemmatizer-1.3.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pt_lemmatizer-1.3.2.tar", last modified: Thu May 11 21:32:51 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

