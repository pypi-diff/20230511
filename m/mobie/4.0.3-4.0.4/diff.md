# Comparing `tmp/mobie-4.0.3.tar.gz` & `tmp/mobie-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobie-4.0.3.tar", last modified: Mon May  8 08:50:36 2023, max compression
+gzip compressed data, was "mobie-4.0.4.tar", last modified: Wed May 10 22:00:11 2023, max compression
```

## Comparing `mobie-4.0.3.tar` & `mobie-4.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:50:36.916808 mobie-4.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-08 08:50:35.000000 mobie-4.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-08 08:50:36.916808 mobie-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-08 08:50:35.000000 mobie-4.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:50:36.916808 mobie-4.0.3/mobie/
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-08 08:50:35.000000 mobie-4.0.3/mobie/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:50:36.916808 mobie-4.0.3/mobie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-08 08:50:36.000000 mobie-4.0.3/mobie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-08 08:50:36.000000 mobie-4.0.3/mobie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:50:36.000000 mobie-4.0.3/mobie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:50:36.000000 mobie-4.0.3/mobie.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 08:50:36.000000 mobie-4.0.3/mobie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 08:50:36.000000 mobie-4.0.3/mobie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:50:36.916808 mobie-4.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-08 08:50:35.000000 mobie-4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:00:11.989249 mobie-4.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-10 22:00:10.000000 mobie-4.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-10 22:00:11.989249 mobie-4.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-10 22:00:10.000000 mobie-4.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:00:11.989249 mobie-4.0.4/mobie/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-10 22:00:10.000000 mobie-4.0.4/mobie/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:00:11.989249 mobie-4.0.4/mobie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-10 22:00:11.000000 mobie-4.0.4/mobie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-10 22:00:11.000000 mobie-4.0.4/mobie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 22:00:11.000000 mobie-4.0.4/mobie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 22:00:11.000000 mobie-4.0.4/mobie.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 22:00:11.000000 mobie-4.0.4/mobie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-10 22:00:11.000000 mobie-4.0.4/mobie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 22:00:11.989249 mobie-4.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-10 22:00:10.000000 mobie-4.0.4/setup.py
```

### Comparing `mobie-4.0.3/LICENSE.txt` & `mobie-4.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mobie-4.0.3/README.md` & `mobie-4.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -53,20 +53,22 @@
 ./install.sh  # test the line of code suggested by the script!
 git add .; git commit -m "prepare for release"; git push
 ../scijava-scripts/release-version.sh --skip-version-check --skip-license-update
 # if successful this will say
 # * [new tag]mobie-viewer-fiji-3.0.10 -> mobie-viewer-fiji-3.0.10
 ```
 
-#### mobie-cmd repo
+#### mobie-cmd
 
 Within `mobie/__init.py__` ensure that
-`_artifactVersion = version("mobie")`   
+`_artifactVersion = version("mobie")`
 
 Within `setup.py` set `version` to `3.0.10`
+Note that you can set this version to a locally build snapshot, for local testing
+
 
 ```
 git add setup.py
 git commit -m "Version bump 3.0.10"
 ```
 
 
@@ -90,14 +92,19 @@
 ```
 git tag 3.0.10
 git push --tags
 ```
 
 Pushing a tag triggers build and deploy to pypi via github actions that are configured in the mobie-cmd repo.
 
+##### check that it worked
+
+1. https://github.com/mobie/mobie-cmd/actions => did the deploy work?
+2. https://github.com/conda-forge/mobie-feedstock => did ?? work?
+
 #### release on conda-forge
 
 deploying to pypi (s.a.) automatically triggers a PR in https://github.com/conda-forge/mobie-feedstock
 
 
 #### Troubleshooting
```

### Comparing `mobie-4.0.3/mobie/__init__.py` & `mobie-4.0.4/mobie/__init__.py`

 * *Files identical despite different names*

### Comparing `mobie-4.0.3/setup.py` & `mobie-4.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 entry_points = {
     "console_scripts": [
         "mobie=mobie:main",
     ]
 }
 
-version = "4.0.3"
+version = "4.0.4"
 
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3 :: Only",
 ]
 
 package_urls = {
```

