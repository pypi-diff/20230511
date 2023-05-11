# Comparing `tmp/osd_slides-0.1.3.tar.gz` & `tmp/osd_slides-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/osd_slides-0.1.3.tar", last modified: Wed Mar 29 01:34:43 2023, max compression
+gzip compressed data, was "dist/osd_slides-0.1.4.tar", last modified: Thu May 11 04:00:48 2023, max compression
```

## Comparing `osd_slides-0.1.3.tar` & `osd_slides-0.1.4.tar`

### file list

```diff
@@ -1,43 +1,35 @@
-drwxr-xr-x   0 kutaykarakas   (501) staff       (20)        0 2023-03-29 01:34:43.000000 osd_slides-0.1.3/
-drwxr-xr-x   0 kutaykarakas   (501) staff       (20)        0 2023-03-29 01:34:43.000000 osd_slides-0.1.3/.idea/
--rw-r--r--   0 kutaykarakas   (501) staff       (20)      176 2023-03-03 08:01:56.000000 osd_slides-0.1.3/.idea/.gitignore
-drwxr-xr-x   0 kutaykarakas   (501) staff       (20)        0 2023-03-29 01:34:43.000000 osd_slides-0.1.3/.idea/inspectionProfiles/
--rw-r--r--   0 kutaykarakas   (501) staff       (20)      506 2023-03-03 08:01:56.000000 osd_slides-0.1.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 kutaykarakas   (501) staff       (20)      174 2023-03-03 08:01:56.000000 osd_slides-0.1.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 kutaykarakas   (501) staff       (20)      185 2023-03-08 10:38:55.000000 osd_slides-0.1.3/.idea/misc.xml
--rw-r--r--   0 kutaykarakas   (501) staff       (20)      272 2023-03-03 08:01:56.000000 osd_slides-0.1.3/.idea/modules.xml
--rw-r--r--   0 kutaykarakas   (501) staff       (20)      385 2023-03-08 10:47:39.000000 osd_slides-0.1.3/.idea/osd-slides.iml
--rw-r--r--   0 kutaykarakas   (501) staff       (20)      180 2023-03-03 08:01:56.000000 osd_slides-0.1.3/.idea/vcs.xml
--rw-r--r--   0 kutaykarakas   (501) staff       (20)      624 2023-03-28 04:35:08.000000 osd_slides-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 kutaykarakas   (501) staff       (20)     1071 2023-02-20 02:17:39.000000 osd_slides-0.1.3/LICENSE
--rw-r--r--   0 kutaykarakas   (501) staff       (20)      439 2023-03-29 00:51:59.000000 osd_slides-0.1.3/MANIFEST.in
--rw-r--r--   0 kutaykarakas   (501) staff       (20)     2473 2023-03-28 04:23:34.000000 osd_slides-0.1.3/Makefile
--rw-r--r--   0 kutaykarakas   (501) staff       (20)     3847 2023-03-29 01:34:43.000000 osd_slides-0.1.3/PKG-INFO
--rw-r--r--   0 kutaykarakas   (501) staff       (20)     1736 2023-03-29 01:31:59.000000 osd_slides-0.1.3/README.md
-drwxr-xr-x   0 kutaykarakas   (501) staff       (20)        0 2023-03-29 01:34:43.000000 osd_slides-0.1.3/osd_slides/
-drwxr-xr-x   0 kutaykarakas   (501) staff       (20)        0 2023-03-29 01:34:43.000000 osd_slides-0.1.3/osd_slides/.pytest_cache/
--rw-r--r--   0 kutaykarakas   (501) staff       (20)       37 2023-03-04 04:31:43.000000 osd_slides-0.1.3/osd_slides/.pytest_cache/.gitignore
--rw-r--r--   0 kutaykarakas   (501) staff       (20)      191 2023-03-04 04:31:43.000000 osd_slides-0.1.3/osd_slides/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 kutaykarakas   (501) staff       (20)      302 2023-03-04 04:31:43.000000 osd_slides-0.1.3/osd_slides/.pytest_cache/README.md
-drwxr-xr-x   0 kutaykarakas   (501) staff       (20)        0 2023-03-29 01:34:43.000000 osd_slides-0.1.3/osd_slides/.pytest_cache/v/
-drwxr-xr-x   0 kutaykarakas   (501) staff       (20)        0 2023-03-29 01:34:43.000000 osd_slides-0.1.3/osd_slides/.pytest_cache/v/cache/
--rw-r--r--   0 kutaykarakas   (501) staff       (20)       31 2023-03-04 04:31:43.000000 osd_slides-0.1.3/osd_slides/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0 kutaykarakas   (501) staff       (20)        2 2023-03-04 04:32:39.000000 osd_slides-0.1.3/osd_slides/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 kutaykarakas   (501) staff       (20)        2 2023-03-04 04:32:39.000000 osd_slides-0.1.3/osd_slides/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 kutaykarakas   (501) staff       (20)       22 2023-03-08 10:47:39.000000 osd_slides-0.1.3/osd_slides/__init__.py
--rw-r--r--   0 kutaykarakas   (501) staff       (20)      192 2023-03-28 04:23:35.000000 osd_slides-0.1.3/osd_slides/__main__.py
--rw-r--r--   0 kutaykarakas   (501) staff       (20)     2115 2023-03-28 04:23:35.000000 osd_slides-0.1.3/osd_slides/main.py
-drwxr-xr-x   0 kutaykarakas   (501) staff       (20)        0 2023-03-29 01:34:43.000000 osd_slides-0.1.3/osd_slides/tests/
--rw-r--r--   0 kutaykarakas   (501) staff       (20)        0 2023-03-08 10:47:39.000000 osd_slides-0.1.3/osd_slides/tests/__init__.py
--rw-r--r--   0 kutaykarakas   (501) staff       (20)     8423 2023-03-28 04:23:35.000000 osd_slides-0.1.3/osd_slides/tests/test_all.py
-drwxr-xr-x   0 kutaykarakas   (501) staff       (20)        0 2023-03-29 01:34:43.000000 osd_slides-0.1.3/osd_slides.egg-info/
--rw-r--r--   0 kutaykarakas   (501) staff       (20)     3847 2023-03-29 01:34:42.000000 osd_slides-0.1.3/osd_slides.egg-info/PKG-INFO
--rw-r--r--   0 kutaykarakas   (501) staff       (20)      814 2023-03-29 01:34:43.000000 osd_slides-0.1.3/osd_slides.egg-info/SOURCES.txt
--rw-r--r--   0 kutaykarakas   (501) staff       (20)        1 2023-03-29 01:34:42.000000 osd_slides-0.1.3/osd_slides.egg-info/dependency_links.txt
--rw-r--r--   0 kutaykarakas   (501) staff       (20)      199 2023-03-29 01:34:42.000000 osd_slides-0.1.3/osd_slides.egg-info/requires.txt
--rw-r--r--   0 kutaykarakas   (501) staff       (20)        1 2023-03-29 01:34:42.000000 osd_slides-0.1.3/osd_slides.egg-info/top_level.txt
--rw-r--r--   0 kutaykarakas   (501) staff       (20)    83314 2023-03-03 08:01:56.000000 osd_slides-0.1.3/package-lock.json
--rw-r--r--   0 kutaykarakas   (501) staff       (20)       53 2023-03-03 08:01:56.000000 osd_slides-0.1.3/package.json
--rw-r--r--   0 kutaykarakas   (501) staff       (20)     3222 2023-03-29 00:51:59.000000 osd_slides-0.1.3/pyproject.toml
--rw-r--r--   0 kutaykarakas   (501) staff       (20)       38 2023-03-29 01:34:43.000000 osd_slides-0.1.3/setup.cfg
--rw-r--r--   0 kutaykarakas   (501) staff       (20)      166 2023-03-29 01:33:59.000000 osd_slides-0.1.3/setup.py
+drwxr-xr-x   0 kutaykarakas   (501) staff       (20)        0 2023-05-11 04:00:48.000000 osd_slides-0.1.4/
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)      747 2023-05-11 03:54:24.000000 osd_slides-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)     1071 2023-02-20 02:17:39.000000 osd_slides-0.1.4/LICENSE
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)      439 2023-03-29 00:51:59.000000 osd_slides-0.1.4/MANIFEST.in
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)     2893 2023-05-11 04:00:30.000000 osd_slides-0.1.4/Makefile
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)     5351 2023-05-11 04:00:48.000000 osd_slides-0.1.4/PKG-INFO
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)     3240 2023-05-11 03:54:24.000000 osd_slides-0.1.4/README.md
+drwxr-xr-x   0 kutaykarakas   (501) staff       (20)        0 2023-05-11 04:00:48.000000 osd_slides-0.1.4/osd_slides/
+drwxr-xr-x   0 kutaykarakas   (501) staff       (20)        0 2023-05-11 04:00:48.000000 osd_slides-0.1.4/osd_slides/.pytest_cache/
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)       37 2023-03-04 04:31:43.000000 osd_slides-0.1.4/osd_slides/.pytest_cache/.gitignore
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)      191 2023-03-04 04:31:43.000000 osd_slides-0.1.4/osd_slides/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)      302 2023-03-04 04:31:43.000000 osd_slides-0.1.4/osd_slides/.pytest_cache/README.md
+drwxr-xr-x   0 kutaykarakas   (501) staff       (20)        0 2023-05-11 04:00:48.000000 osd_slides-0.1.4/osd_slides/.pytest_cache/v/
+drwxr-xr-x   0 kutaykarakas   (501) staff       (20)        0 2023-05-11 04:00:48.000000 osd_slides-0.1.4/osd_slides/.pytest_cache/v/cache/
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)       31 2023-03-04 04:31:43.000000 osd_slides-0.1.4/osd_slides/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)        2 2023-03-04 04:32:39.000000 osd_slides-0.1.4/osd_slides/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)        2 2023-03-04 04:32:39.000000 osd_slides-0.1.4/osd_slides/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)       22 2023-03-08 10:47:39.000000 osd_slides-0.1.4/osd_slides/__init__.py
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)      223 2023-04-26 01:16:15.000000 osd_slides-0.1.4/osd_slides/__main__.py
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)     3298 2023-05-11 03:54:24.000000 osd_slides-0.1.4/osd_slides/main.py
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)     3838 2023-05-11 03:54:24.000000 osd_slides-0.1.4/osd_slides/search.py
+drwxr-xr-x   0 kutaykarakas   (501) staff       (20)        0 2023-05-11 04:00:48.000000 osd_slides-0.1.4/osd_slides/tests/
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)        0 2023-03-08 10:47:39.000000 osd_slides-0.1.4/osd_slides/tests/__init__.py
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)    12168 2023-05-10 23:13:25.000000 osd_slides-0.1.4/osd_slides/tests/test_all.py
+drwxr-xr-x   0 kutaykarakas   (501) staff       (20)        0 2023-05-11 04:00:48.000000 osd_slides-0.1.4/osd_slides.egg-info/
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)     5351 2023-05-11 04:00:48.000000 osd_slides-0.1.4/osd_slides.egg-info/PKG-INFO
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)      658 2023-05-11 04:00:48.000000 osd_slides-0.1.4/osd_slides.egg-info/SOURCES.txt
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)        1 2023-05-11 04:00:48.000000 osd_slides-0.1.4/osd_slides.egg-info/dependency_links.txt
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)      218 2023-05-11 04:00:48.000000 osd_slides-0.1.4/osd_slides.egg-info/requires.txt
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)        1 2023-05-11 04:00:48.000000 osd_slides-0.1.4/osd_slides.egg-info/top_level.txt
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)    83314 2023-03-03 08:01:56.000000 osd_slides-0.1.4/package-lock.json
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)       53 2023-03-03 08:01:56.000000 osd_slides-0.1.4/package.json
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)     3280 2023-04-26 01:16:15.000000 osd_slides-0.1.4/pyproject.toml
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)       38 2023-05-11 04:00:48.000000 osd_slides-0.1.4/setup.cfg
+-rw-r--r--   0 kutaykarakas   (501) staff       (20)      166 2023-03-29 01:44:54.000000 osd_slides-0.1.4/setup.py
```

### Comparing `osd_slides-0.1.3/LICENSE` & `osd_slides-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `osd_slides-0.1.3/Makefile` & `osd_slides-0.1.4/Makefile`

 * *Files 13% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
 format:  ## run autoformatting with black
 	python -m black osd_slides/ setup.py
 
 # alias
 fix: format
 
+show-format:  ## show what will change when format is run
+	python -m black --check --diff osd_slides setup.py
+
 check:  ## check assets for packaging
 	check-manifest -v
 
 # Alias
 checks: check
 
 # annotate:  ## run type checking
@@ -64,24 +67,24 @@
 
 # major:
 # 	bump2version major
 
 # ########
 # # DIST #
 # ########
-# dist-build:  # Build python dist
-# 	python setup.py sdist bdist_wheel
+ dist-build:  # Build python dist
+ 	python setup.py sdist bdist_wheel
 
-# dist-check:
-# 	python -m twine check dist/*
+ dist-check:
+ 	python -m twine check dist/*
 
-# dist: clean build dist-build dist-check  ## Build dists
+ dist: clean build dist-build dist-check  ## Build dists
 
-# publish:  # Upload python assets
-# 	echo "would usually run python -m twine upload dist/* --skip-existing"
+ publish:  # Upload python assets
+ 	echo "would usually run python -m twine upload dist/* --skip-existing"
 
 #########
 # CLEAN #
 #########
 deep-clean: ## clean everything from the repository
 	git clean -fdx
 
@@ -94,8 +97,22 @@
 # .DEFAULT_GOAL := help
 # help:
 # 	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
 
 # print-%:
 # 	@echo '$*=$($*)'
 
-# .PHONY: develop build install lint lints format fix check checks annotate test coverage show-coverage tests show-version patch minor major dist-build dist-check dist publish deep-clean clean help
+# .PHONY: develop build install lint lints format fix check checks annotate test coverage show-coverage tests show-version patch minor major dist-build dist-check dist publish deep-clean clean help
+TMPREPO=/tmp/docs/bt
+docs:
+	$(MAKE) -C docs/ clean
+	$(MAKE) -C docs/ html
+
+pages:
+	rm -rf $(TMPREPO)
+	git clone -b gh-pages git@github.com:kkarakas/osd-slides.git $(TMPREPO)
+	rm -rf $(TMPREPO)/*
+	cp -r docs/_build/html/* $(TMPREPO)
+	cd $(TMPREPO);\
+	git add -A ;\
+	git commit -a -m 'auto-updating docs' ;\
+	git push
```

### Comparing `osd_slides-0.1.3/osd_slides/main.py` & `osd_slides-0.1.4/osd_slides/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,84 +1,105 @@
 import requests
 from bs4 import BeautifulSoup
 import sys
 import subprocess
 
+from osd_slides.search import Search
+
 # TODO perhaps better to use properties file
 #  using jproperties here instead of using a string.
 url = "https://www.cs.columbia.edu/~paine/4995/lectures/"
 
 
-def fefmalsmc():
-    if len(sys.argv) >= 3:
-        print("Too many arguments")
-        # perhaps should throw an error or something
-
-    elif len(sys.argv) < 2:
-        print("Too few arguments")
-    # length 2 acceptable
-    else:
-        if sys.argv[1] == "download":
-            searchAndDownloadPdf()
-
-        elif sys.argv[1] == "show":
-            showDownloadablePdf()
-
-
-# TODO be able to download individual files
-def searchAndDownloadPdf():
-    docs = readAvailableHtmlDocs()
+class Downloader:
+    def fefmalsmc(self):
+        if len(sys.argv) >= 4:  # perhaps should be 3 now
+            print("Too many arguments")
+            # perhaps should throw an error or something
+
+        elif len(sys.argv) < 2:
+            print("Too few arguments")
+        # length 2 acceptable
+        else:
+            if sys.argv[1] == "download":
+                self.searchAndDownloadPdf()
+
+            elif sys.argv[1] == "show":
+                self.showDownloadablePdf()
+
+            elif sys.argv[1] == "search":
+                print("Which slides would you like to search in? Please provide slides with spaces between them: ")
+                slides = input().split()
+                print("Slides reading completed")
+                # a = Search(url, [sys.argv[2]])
+                a = Search(url, slides)
+                print("What keyword would you like to look up: ")
+                a.lookup(input())
+                print("Which one would you like to open? please provide the number.")
+                a.open(int(input()) - 1)
+                # TODO change it to make it better
+
+    # TODO be able to download individual files
+    def searchAndDownloadPdf(self):
+        '''Downloads all the class presentations.
+
+        Returns:
+            Null
+        '''
+        docs = self.readAvailableHtmlDocs()
+
+        for doc in docs:
+            try:
+                file = doc.find("a")["href"]
+                # file = doc
+                self.downloadPdf(file)
+            except TypeError:
+                pass
+
+        print("done")
+
+    def showDownloadablePdf(self):
+        '''Shows all the downloaddable pdf's.
+
+        Returns:
+            Null
+        '''
+        docs = self.readAvailableHtmlDocs()
+
+        for doc in docs:
+            print(doc.find("a")["href"])
+            # print(doc)
+
+    def readAvailableHtmlDocs(self):
+        # TODO handle when response is not 200
+        response = requests.get(url)
+        soup = BeautifulSoup(response.text, "html.parser")
+        table = soup.find("table")
+        table_rows = table.find_all("tr")
+        blacklist = {
+            "example.html",
+        }
+        docs = []
+        for row in table_rows:
+            if row.find("a") and row.find("a")["href"].endswith(".html"):
+                link = row.find("a")["href"]
+                if link in blacklist:  # blacklisted
+                    continue
+                docs.append(row)
+                # TODO we can change this to link to make it simpler
+
+        return docs
 
-    for doc in docs:
+    def downloadPdf(self, file):
+        print("Downloading file: ", file)
         try:
-            file = doc.find("a")["href"]
-            # file = doc
-            downloadPdf(file)
-        except TypeError:
-            pass
-
-    print("done")
-
-
-def showDownloadablePdf():
-    docs = readAvailableHtmlDocs()
-
-    for doc in docs:
-        print(doc.find("a")["href"])
-        # print(doc)
-
-
-def readAvailableHtmlDocs():
-    # TODO handle when response is not 200
-    response = requests.get(url)
-    soup = BeautifulSoup(response.text, "html.parser")
-    table = soup.find("table")
-    table_rows = table.find_all("tr")
-    blacklist = {
-        "example.html",
-    }
-    docs = []
-    for row in table_rows:
-        if row.find("a") and row.find("a")["href"].endswith(".html"):
-            link = row.find("a")["href"]
-            if link in blacklist:  # blacklisted
-                continue
-            docs.append(row)
-            # TODO we can change this to link to make it simpler
-
-    return docs
-
-
-def downloadPdf(file):
-    print("Downloading file: ", file)
-    try:
-        a = subprocess.run(
-            ["npx", "decktape", "reveal", url + file + "#/", file[:-4] + "pdf"],
-            capture_output=True,
-            check=True,
-        )
-        print(a.stderr)
-    except subprocess.CalledProcessError as exc:
-        print("Standard error was {}".format(exc.stderr))
+            a = subprocess.run(
+                ["npx", "decktape", "reveal", url + file + "#/", file[:-4] + "pdf"],  # noqa: E501
+                capture_output=True,
+                check=True,
+            )
+            print(a.stderr)
+        except subprocess.CalledProcessError as exc:
+            print("Standard error was {}".format(exc.stderr))
 
-    # print(a.stdout)
-    print("File ", file, " downloaded")
+        # print(a.stdout)
+        print("File ", file, " downloaded")
```

### Comparing `osd_slides-0.1.3/package-lock.json` & `osd_slides-0.1.4/package-lock.json`

 * *Files identical despite different names*

### Comparing `osd_slides-0.1.3/pyproject.toml` & `osd_slides-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "osd_slides"
 authors = [{name = "Kutay Karakas", email = "kutay@karakas.co"}]
 description="osd-slides is a tool to download Prof. Paine's slides through terminal with one command."
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 requires-python = ">=3.7"
 dependencies = ["beautifulsoup4==4.11.2"]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
@@ -87,14 +87,18 @@
     "flake8-pyproject",
     "mypy",
     "pytest>=4.3.0",
     "pytest-cov>=2.6.1",
     "pytest-mock>=3.10.0",
     "twine",
     "wheel",
+    "sphinx",
+#    "sphinx_rtd_theme",
+    "myst-parser"
+
 ]
 
 [tool.black]
 color = true
 line-length = 120
 target-version = ['py310']
 skip-string-normalization = true
```

