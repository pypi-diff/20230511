# Comparing `tmp/aws-cdk.aws-iot-actions-1.200.0.tar.gz` & `tmp/aws_cdk.aws_iot_actions-1.201.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src432989618/src/packages/@aws-cdk/aws-iot-actions/dist/python/aws-cdk.aws-iot-actions-1.200.0.tar", last modified: Wed Apr 26 19:57:04 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

