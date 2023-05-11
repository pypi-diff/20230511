# Comparing `tmp/multi_docker_build-0.7.1-py3-none-any.whl.zip` & `tmp/multi_docker_build-0.7.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7929 bytes, number of entries: 8
+Zip file size: 8094 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx        0 b- defN 21-Aug-12 17:45 multi_docker_build/__init__.py
--rw-rw-r--  2.0 unx    12164 b- defN 21-Aug-12 17:45 multi_docker_build/build_docker_images.py
--rw-rw-r--  2.0 unx     1059 b- defN 21-Aug-12 17:47 multi_docker_build-0.7.1.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     3998 b- defN 21-Aug-12 17:47 multi_docker_build-0.7.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 21-Aug-12 17:47 multi_docker_build-0.7.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       85 b- defN 21-Aug-12 17:47 multi_docker_build-0.7.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       19 b- defN 21-Aug-12 17:47 multi_docker_build-0.7.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      734 b- defN 21-Aug-12 17:47 multi_docker_build-0.7.1.dist-info/RECORD
-8 files, 18151 bytes uncompressed, 6619 bytes compressed:  63.5%
+-rw-rw-r--  2.0 unx    12409 b- defN 23-May-11 13:41 multi_docker_build/build_docker_images.py
+-rw-rw-r--  2.0 unx     1059 b- defN 23-May-11 13:42 multi_docker_build-0.7.2.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     4335 b- defN 23-May-11 13:42 multi_docker_build-0.7.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-11 13:42 multi_docker_build-0.7.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       84 b- defN 23-May-11 13:42 multi_docker_build-0.7.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       19 b- defN 23-May-11 13:42 multi_docker_build-0.7.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      734 b- defN 23-May-11 13:42 multi_docker_build-0.7.2.dist-info/RECORD
+8 files, 18732 bytes uncompressed, 6784 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: multi_docker_build/__init__.py
 Comment: 
 
 Filename: multi_docker_build/build_docker_images.py
 Comment: 
 
-Filename: multi_docker_build-0.7.1.dist-info/LICENSE.txt
+Filename: multi_docker_build-0.7.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: multi_docker_build-0.7.1.dist-info/METADATA
+Filename: multi_docker_build-0.7.2.dist-info/METADATA
 Comment: 
 
-Filename: multi_docker_build-0.7.1.dist-info/WHEEL
+Filename: multi_docker_build-0.7.2.dist-info/WHEEL
 Comment: 
 
-Filename: multi_docker_build-0.7.1.dist-info/entry_points.txt
+Filename: multi_docker_build-0.7.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: multi_docker_build-0.7.1.dist-info/top_level.txt
+Filename: multi_docker_build-0.7.2.dist-info/top_level.txt
 Comment: 
 
-Filename: multi_docker_build-0.7.1.dist-info/RECORD
+Filename: multi_docker_build-0.7.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## multi_docker_build/build_docker_images.py

```diff
@@ -27,20 +27,22 @@
 
 # TODO: expand to other formats (JSON, YAML, CSV) in the future if necessary or appropriate
 IMAGE_LIST_FILENAME = "docker_images.txt"
 
 BASE_DIR_BUILD_OPTION = "base_directory_build"
 GIT_VERSION_FILE_OPTION = "write_git_version"
 GIT_JSON_FILE_OPTION = "write_git_json"
+PLATFORMS_OPTION = "platforms"
 
 SUPPORTED_OPTIONS = frozenset(
     {
         BASE_DIR_BUILD_OPTION,
         GIT_VERSION_FILE_OPTION,
         GIT_JSON_FILE_OPTION,
+        PLATFORMS_OPTION,
     }
 )
 
 DOCKER = "docker"
 DOCKER_BUILD_COMMAND_TEMPLATE: List[str] = [
     DOCKER,
     "build",
@@ -293,14 +295,19 @@
         docker_build_command = [
             piece.format(
                 label=label,
                 dockerfile_path=dockerfile_path,
             )
             for piece in DOCKER_BUILD_COMMAND_TEMPLATE
         ]
+
+        if PLATFORMS_OPTION in options:
+            platforms_str = ",".join(options[PLATFORMS_OPTION].split("&"))
+            docker_build_command.append(f"--platform={platforms_str}")
+
         image_id = print_run(docker_build_command, pretend, return_stdout=True, cwd=build_dir)
         images_to_push.append(label)
         print("Tagged image", image_id, "as", label)
 
         if tag_timestamp:
             timestamp_tag_name = f"{label_base}:{timestamp}"
             tag_image(image_id, timestamp_tag_name, pretend)
```

## Comparing `multi_docker_build-0.7.1.dist-info/LICENSE.txt` & `multi_docker_build-0.7.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `multi_docker_build-0.7.1.dist-info/METADATA` & `multi_docker_build-0.7.2.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: multi-docker-build
-Version: 0.7.1
+Version: 0.7.2
 Summary: Automated building/tagging/pushing of multiple Docker images in succession
 Home-page: https://github.com/mruffalo/multi-docker-build
 Author: Matt Ruffalo
 Author-email: matt.ruffalo@gmail.com
 License: MIT
 Keywords: docker automation
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -67,14 +66,23 @@
 desired (see below).
 
 The build option ``write_git_version`` accepts a file path argument, to which
 the output of ``git describe --dirty --always --abbrev=12`` is written. For example::
 
   image_label    path/to/Dockerfile    write_git_version=src/revision.txt
 
+
+Cross-platform builds
+---------------------
+
+The build option ``platforms`` accepts a ``&``-delimited list of platforms, which
+will be passed directly to ``docker build --platforms=...``, with ``&`` replaced by
+``,`` in the ``docker build`` invocation. Note that this may require usage of the
+newer ``buildx`` tool, replacing the legacy ``docker build``.
+
 Usage
 -----
 
 The command-line entry point provided by this script is
 ``build_docker_images``. By default, images will be tagged with
 ``:latest`` appended to the base image name.
 
@@ -102,9 +110,7 @@
                 (building, tagging, pushing).
 
 Requirements
 ------------
 
 Python 3.6 or newer for this script. Docker to build/tag/push images (version
 unimportant).
-
-
```

## Comparing `multi_docker_build-0.7.1.dist-info/RECORD` & `multi_docker_build-0.7.2.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 multi_docker_build/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-multi_docker_build/build_docker_images.py,sha256=wMjy5AKMHHgV-SEQtu46xw2YwOogb0cAjxlC9YTr2hw,12164
-multi_docker_build-0.7.1.dist-info/LICENSE.txt,sha256=kwSy3l1BE6oekFWAT11EHPjYohIoRcOxQsyF-QkkDK8,1059
-multi_docker_build-0.7.1.dist-info/METADATA,sha256=SL0pL7Vx0XSXy2eTzU84ve4W1EOE3784T6wkTy8dEDg,3998
-multi_docker_build-0.7.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-multi_docker_build-0.7.1.dist-info/entry_points.txt,sha256=JkhZ0hRAcyOlmO8cyszuAGtLLmjlY9HkmWTsZQQ870E,85
-multi_docker_build-0.7.1.dist-info/top_level.txt,sha256=ehQ-Qr6hMS0hnaDCLnHOvkcKdqKoe0BOpIWyJb9GePY,19
-multi_docker_build-0.7.1.dist-info/RECORD,,
+multi_docker_build/build_docker_images.py,sha256=mZjIbk0Eg-ugR5CB_C_Q6Oz3b32hRrd1HEwIBtAzB_I,12409
+multi_docker_build-0.7.2.dist-info/LICENSE.txt,sha256=kwSy3l1BE6oekFWAT11EHPjYohIoRcOxQsyF-QkkDK8,1059
+multi_docker_build-0.7.2.dist-info/METADATA,sha256=Q-05TUvKf2MaNntsnexIR_l5EOeWFkv1A3grZKdYMoc,4335
+multi_docker_build-0.7.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+multi_docker_build-0.7.2.dist-info/entry_points.txt,sha256=LFRRoL_lO4N7zCyO3uAInqgSwceE20P-erYcVd1WEJU,84
+multi_docker_build-0.7.2.dist-info/top_level.txt,sha256=ehQ-Qr6hMS0hnaDCLnHOvkcKdqKoe0BOpIWyJb9GePY,19
+multi_docker_build-0.7.2.dist-info/RECORD,,
```

