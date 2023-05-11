# Comparing `tmp/quickops-1.0.tar.gz` & `tmp/quickops-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickops-1.0.tar", last modified: Thu May 11 18:37:25 2023, max compression
+gzip compressed data, was "quickops-1.1.tar", last modified: Thu May 11 20:46:53 2023, max compression
```

## Comparing `quickops-1.0.tar` & `quickops-1.1.tar`

### file list

```diff
@@ -1,13 +1,67 @@
-drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 18:37:25.947369 quickops-1.0/
--rw-rw-r--   0 piksi     (1000) piksi     (1000)       92 2023-05-11 18:37:25.947369 quickops-1.0/PKG-INFO
--rw-rw-r--   0 piksi     (1000) piksi     (1000)      754 2023-05-11 18:24:29.000000 quickops-1.0/README.md
-drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 18:37:25.947369 quickops-1.0/ops/
--rw-rw-r--   0 piksi     (1000) piksi     (1000)      211 2023-04-24 19:32:24.000000 quickops-1.0/ops/__init__.py
-drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 18:37:25.947369 quickops-1.0/quickops.egg-info/
--rw-rw-r--   0 piksi     (1000) piksi     (1000)       92 2023-05-11 18:37:25.000000 quickops-1.0/quickops.egg-info/PKG-INFO
--rw-rw-r--   0 piksi     (1000) piksi     (1000)      197 2023-05-11 18:37:25.000000 quickops-1.0/quickops.egg-info/SOURCES.txt
--rw-rw-r--   0 piksi     (1000) piksi     (1000)        1 2023-05-11 18:37:25.000000 quickops-1.0/quickops.egg-info/dependency_links.txt
--rw-rw-r--   0 piksi     (1000) piksi     (1000)       83 2023-05-11 18:37:25.000000 quickops-1.0/quickops.egg-info/entry_points.txt
--rw-rw-r--   0 piksi     (1000) piksi     (1000)        4 2023-05-11 18:37:25.000000 quickops-1.0/quickops.egg-info/top_level.txt
--rw-rw-r--   0 piksi     (1000) piksi     (1000)       38 2023-05-11 18:37:25.947369 quickops-1.0/setup.cfg
--rw-rw-r--   0 piksi     (1000) piksi     (1000)      373 2023-05-11 18:23:50.000000 quickops-1.0/setup.py
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.553532 quickops-1.1/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)      555 2023-05-11 20:29:24.000000 quickops-1.1/MANIFEST.in
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)       92 2023-05-11 20:46:53.553532 quickops-1.1/PKG-INFO
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)      754 2023-05-11 18:24:29.000000 quickops-1.1/README.md
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)      211 2023-04-24 19:32:24.000000 quickops-1.1/ops/__init__.py
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/cli/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)     5763 2023-05-11 18:36:04.000000 quickops-1.1/ops/cli/__init__.py
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/cli/arguments/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)       88 2023-05-02 05:53:28.000000 quickops-1.1/ops/cli/arguments/__init__.py
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)     4203 2023-05-11 18:32:54.000000 quickops-1.1/ops/cli/arguments/option_helpers.py
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)     1559 2023-05-11 18:26:57.000000 quickops-1.1/ops/cli/ops.py
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)     1374 2023-05-09 20:53:40.000000 quickops-1.1/ops/constants.py
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/entities/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)        0 2023-05-07 13:51:53.000000 quickops-1.1/ops/entities/__init__.py
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.545528 quickops-1.1/ops/entities/docker/
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/entities/docker/c++/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)      365 2023-05-11 17:19:51.000000 quickops-1.1/ops/entities/docker/c++/Dockerfile
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/entities/docker/npm/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)      174 2023-05-10 19:09:53.000000 quickops-1.1/ops/entities/docker/npm/Dockerfile
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/entities/docker/python/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)      326 2023-05-11 17:13:44.000000 quickops-1.1/ops/entities/docker/python/Dockerfile
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/entities/docker/springboot/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)      567 2023-05-11 17:19:51.000000 quickops-1.1/ops/entities/docker/springboot/Dockerfile
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.545528 quickops-1.1/ops/entities/gitlab/
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/entities/gitlab/django/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)      831 2023-05-11 03:58:38.000000 quickops-1.1/ops/entities/gitlab/django/gitlab-ci.yml
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/entities/gitlab/docker/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)      652 2023-05-11 03:58:38.000000 quickops-1.1/ops/entities/gitlab/docker/gitlab-ci.yml
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/entities/gitlab/gradle/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)      506 2023-05-11 03:58:38.000000 quickops-1.1/ops/entities/gitlab/gradle/gitlab-ci.yml
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/entities/gitlab/maven/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)     1034 2023-05-11 03:58:38.000000 quickops-1.1/ops/entities/gitlab/maven/gitlab-ci.yml
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/entities/gitlab/npm/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)     1712 2023-05-11 03:58:38.000000 quickops-1.1/ops/entities/gitlab/npm/gitlab-ci.yml
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/entities/jenkins/
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/entities/jenkins/django/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)     1749 2023-05-11 16:55:06.000000 quickops-1.1/ops/entities/jenkins/django/Jenkinsfile.groovy
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/entities/jenkins/docker/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)     1713 2023-05-11 16:55:06.000000 quickops-1.1/ops/entities/jenkins/docker/Jenkinsfile.groovy
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/entities/jenkins/gradle/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)     1522 2023-05-11 16:55:06.000000 quickops-1.1/ops/entities/jenkins/gradle/Jenkinsfile.groovy
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/entities/jenkins/maven/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)     1816 2023-05-11 17:26:55.000000 quickops-1.1/ops/entities/jenkins/maven/Jenkinsfile.groovy
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/entities/jenkins/npm/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)     1156 2023-05-11 16:55:06.000000 quickops-1.1/ops/entities/jenkins/npm/Jenkinsfile.groovy
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/entities/jenkins/sonarqube/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)     1769 2023-05-11 16:55:06.000000 quickops-1.1/ops/entities/jenkins/sonarqube/Jenkinsfile.groovy
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.549530 quickops-1.1/ops/errors/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)     5848 2023-05-11 18:36:36.000000 quickops-1.1/ops/errors/__init__.py
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)      143 2023-05-11 20:46:13.000000 quickops-1.1/ops/release.py
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.553532 quickops-1.1/ops/utils/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)        0 2023-05-06 14:01:58.000000 quickops-1.1/ops/utils/__init__.py
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)     1765 2023-05-09 20:33:22.000000 quickops-1.1/ops/utils/color.py
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)    10025 2023-05-11 17:39:59.000000 quickops-1.1/ops/utils/display.py
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)      818 2023-05-09 19:10:39.000000 quickops-1.1/ops/utils/singleton.py
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.553532 quickops-1.1/ops/utils/text/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)     1169 2023-05-09 19:35:27.000000 quickops-1.1/ops/utils/text/__init__.py
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)     4791 2023-05-09 20:07:06.000000 quickops-1.1/ops/utils/text/converters.py
+drwxrwxr-x   0 piksi     (1000) piksi     (1000)        0 2023-05-11 20:46:53.553532 quickops-1.1/quickops.egg-info/
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)       92 2023-05-11 20:46:53.000000 quickops-1.1/quickops.egg-info/PKG-INFO
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)     1163 2023-05-11 20:46:53.000000 quickops-1.1/quickops.egg-info/SOURCES.txt
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)        1 2023-05-11 20:46:53.000000 quickops-1.1/quickops.egg-info/dependency_links.txt
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)       83 2023-05-11 20:46:53.000000 quickops-1.1/quickops.egg-info/entry_points.txt
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)        4 2023-05-11 20:46:53.000000 quickops-1.1/quickops.egg-info/top_level.txt
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)       38 2023-05-11 20:46:53.553532 quickops-1.1/setup.cfg
+-rw-rw-r--   0 piksi     (1000) piksi     (1000)      384 2023-05-11 20:40:21.000000 quickops-1.1/setup.py
```

### Comparing `quickops-1.0/README.md` & `quickops-1.1/README.md`

 * *Files identical despite different names*

