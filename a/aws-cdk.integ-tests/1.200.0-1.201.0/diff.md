# Comparing `tmp/aws-cdk.integ-tests-1.200.0.tar.gz` & `tmp/aws_cdk.integ_tests-1.201.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src432989618/src/packages/@aws-cdk/integ-tests/dist/python/aws-cdk.integ-tests-1.200.0.tar", last modified: Wed Apr 26 19:54:35 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

