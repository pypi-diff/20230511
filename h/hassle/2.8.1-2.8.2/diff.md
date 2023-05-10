# Comparing `tmp/hassle-2.8.1.tar.gz` & `tmp/hassle-2.8.2.tar.gz`

## Comparing `hassle-2.8.1.tar` & `hassle-2.8.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 hassle-2.8.1/CHANGELOG.md
--rw-r--r--   0        0        0    33936 2020-02-02 00:00:00.000000 hassle-2.8.1/docs/hassle.html
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 hassle-2.8.1/docs/index.html
--rw-r--r--   0        0        0    44738 2020-02-02 00:00:00.000000 hassle-2.8.1/docs/search.js
--rw-r--r--   0        0        0    93372 2020-02-02 00:00:00.000000 hassle-2.8.1/docs/hassle/generate_tests.html
--rw-r--r--   0        0        0   134700 2020-02-02 00:00:00.000000 hassle-2.8.1/docs/hassle/hassle.html
--rw-r--r--   0        0        0   107599 2020-02-02 00:00:00.000000 hassle-2.8.1/docs/hassle/hassle_config.html
--rw-r--r--   0        0        0   116364 2020-02-02 00:00:00.000000 hassle-2.8.1/docs/hassle/hassle_utilities.html
--rw-r--r--   0        0        0   165062 2020-02-02 00:00:00.000000 hassle-2.8.1/docs/hassle/new_project.html
--rw-r--r--   0        0        0    53608 2020-02-02 00:00:00.000000 hassle-2.8.1/docs/hassle/run_tests.html
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/.gitignore_template
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/.vscode_template
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/README_template.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/__init__.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/generate_tests.py
--rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/hassle.py
--rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/hassle_config.py
--rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/hassle_utilities.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/license_template.txt
--rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/new_project.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/pyproject_template.toml
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/run_tests.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hassle-2.8.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hassle-2.8.1/LICENSE.txt
--rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 hassle-2.8.1/README.md
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 hassle-2.8.1/pyproject.toml
--rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 hassle-2.8.1/PKG-INFO
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 hassle-2.8.2/CHANGELOG.md
+-rw-r--r--   0        0        0    33936 2020-02-02 00:00:00.000000 hassle-2.8.2/docs/hassle.html
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 hassle-2.8.2/docs/index.html
+-rw-r--r--   0        0        0    44738 2020-02-02 00:00:00.000000 hassle-2.8.2/docs/search.js
+-rw-r--r--   0        0        0    93372 2020-02-02 00:00:00.000000 hassle-2.8.2/docs/hassle/generate_tests.html
+-rw-r--r--   0        0        0   134700 2020-02-02 00:00:00.000000 hassle-2.8.2/docs/hassle/hassle.html
+-rw-r--r--   0        0        0   107599 2020-02-02 00:00:00.000000 hassle-2.8.2/docs/hassle/hassle_config.html
+-rw-r--r--   0        0        0   116364 2020-02-02 00:00:00.000000 hassle-2.8.2/docs/hassle/hassle_utilities.html
+-rw-r--r--   0        0        0   165062 2020-02-02 00:00:00.000000 hassle-2.8.2/docs/hassle/new_project.html
+-rw-r--r--   0        0        0    53608 2020-02-02 00:00:00.000000 hassle-2.8.2/docs/hassle/run_tests.html
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hassle-2.8.2/src/hassle/.gitignore_template
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hassle-2.8.2/src/hassle/.vscode_template
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hassle-2.8.2/src/hassle/README_template.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hassle-2.8.2/src/hassle/__init__.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 hassle-2.8.2/src/hassle/generate_tests.py
+-rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 hassle-2.8.2/src/hassle/hassle.py
+-rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 hassle-2.8.2/src/hassle/hassle_config.py
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 hassle-2.8.2/src/hassle/hassle_utilities.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hassle-2.8.2/src/hassle/license_template.txt
+-rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 hassle-2.8.2/src/hassle/new_project.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hassle-2.8.2/src/hassle/pyproject_template.toml
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 hassle-2.8.2/src/hassle/run_tests.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hassle-2.8.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hassle-2.8.2/LICENSE.txt
+-rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 hassle-2.8.2/README.md
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 hassle-2.8.2/pyproject.toml
+-rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 hassle-2.8.2/PKG-INFO
```

### Comparing `hassle-2.8.1/CHANGELOG.md` & `hassle-2.8.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,29 @@
 # Changelog
 
-## 2.8.0 (2023-05-09)
+## 2.8.2 (2023-05-10)
+
+#### Fixes
+
+* swap build and increment_version order so version isn't incremented if build/tests fail
+
+
+## v2.8.1 (2023-05-10)
+
+#### Fixes
+
+* modify pip install invocation for better multi-platform support
+#### Others
+
+* build v2.8.1
+* update changelog
+* remove unused import
+
+
+## v2.8.0 (2023-05-09)
 
 #### New Features
 
 * add tests execution to build command
 * add -st/--skip_tests flag to hassle parser
 #### Fixes
 
@@ -15,14 +34,16 @@
 
 * replace os.system calls to git with gitbetter.git methods
 * replace os.system calls for black and isort with direct invocations
 * extract build process into it's own function
 * make run_tests() invoke pytest and coverage directly and return pytest result
 #### Others
 
+* build v2.8.0
+* update changelog
 * remove unused import
 
 
 ## v2.7.1 (2023-05-02)
 
 #### Fixes
```

### Comparing `hassle-2.8.1/docs/hassle.html` & `hassle-2.8.2/docs/hassle.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.1/docs/search.js` & `hassle-2.8.2/docs/search.js`

 * *Files identical despite different names*

### Comparing `hassle-2.8.1/docs/hassle/generate_tests.html` & `hassle-2.8.2/docs/hassle/generate_tests.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.1/docs/hassle/hassle.html` & `hassle-2.8.2/docs/hassle/hassle.html`

 * *Files 0% similar despite different names*

```diff
@@ -274,19 +274,19 @@
 </span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>
 </span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">generate_tests</span><span class="p">:</span>
 </span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>        <span class="n">generate_test_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
 </span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>
 </span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">run_tests</span><span class="p">:</span>
 </span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>        <span class="n">run_tests</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
 </span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">:</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">increment_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">)</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">build</span><span class="p">:</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>        <span class="n">build</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">skip_tests</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite_dependencies</span><span class="p">)</span>
 </span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">build</span><span class="p">:</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="n">build</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">skip_tests</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite_dependencies</span><span class="p">)</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">:</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">increment_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">)</span>
 </span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>
 </span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">:</span>
 </span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
 </span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>        <span class="c1"># If we&#39;re going to add tag for current version</span>
 </span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>        <span class="c1"># commit changelog first</span>
 </span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
 </span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>            <span class="nb">input</span><span class="p">(</span>
@@ -580,19 +580,19 @@
 </span><span id="main-213"><a href="#main-213"><span class="linenos">213</span></a>
 </span><span id="main-214"><a href="#main-214"><span class="linenos">214</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">generate_tests</span><span class="p">:</span>
 </span><span id="main-215"><a href="#main-215"><span class="linenos">215</span></a>        <span class="n">generate_test_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
 </span><span id="main-216"><a href="#main-216"><span class="linenos">216</span></a>
 </span><span id="main-217"><a href="#main-217"><span class="linenos">217</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">run_tests</span><span class="p">:</span>
 </span><span id="main-218"><a href="#main-218"><span class="linenos">218</span></a>        <span class="n">run_tests</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
 </span><span id="main-219"><a href="#main-219"><span class="linenos">219</span></a>
-</span><span id="main-220"><a href="#main-220"><span class="linenos">220</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">:</span>
-</span><span id="main-221"><a href="#main-221"><span class="linenos">221</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">increment_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">)</span>
+</span><span id="main-220"><a href="#main-220"><span class="linenos">220</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">build</span><span class="p">:</span>
+</span><span id="main-221"><a href="#main-221"><span class="linenos">221</span></a>        <span class="n">build</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">skip_tests</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite_dependencies</span><span class="p">)</span>
 </span><span id="main-222"><a href="#main-222"><span class="linenos">222</span></a>
-</span><span id="main-223"><a href="#main-223"><span class="linenos">223</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">build</span><span class="p">:</span>
-</span><span id="main-224"><a href="#main-224"><span class="linenos">224</span></a>        <span class="n">build</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">skip_tests</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite_dependencies</span><span class="p">)</span>
+</span><span id="main-223"><a href="#main-223"><span class="linenos">223</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">:</span>
+</span><span id="main-224"><a href="#main-224"><span class="linenos">224</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">increment_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">)</span>
 </span><span id="main-225"><a href="#main-225"><span class="linenos">225</span></a>
 </span><span id="main-226"><a href="#main-226"><span class="linenos">226</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">:</span>
 </span><span id="main-227"><a href="#main-227"><span class="linenos">227</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
 </span><span id="main-228"><a href="#main-228"><span class="linenos">228</span></a>        <span class="c1"># If we&#39;re going to add tag for current version</span>
 </span><span id="main-229"><a href="#main-229"><span class="linenos">229</span></a>        <span class="c1"># commit changelog first</span>
 </span><span id="main-230"><a href="#main-230"><span class="linenos">230</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
 </span><span id="main-231"><a href="#main-231"><span class="linenos">231</span></a>            <span class="nb">input</span><span class="p">(</span>
```

#### html2text {}

```diff
@@ -232,20 +232,20 @@
 212
 213    if args.generate_tests:
 214        generate_test_files(args.package)
 215
 216    if args.run_tests:
 217        run_tests(args.package)
 218
-219    if args.increment_version:
-220        hassle_utilities.increment_version(pyproject_path,
-args.increment_version)
+219    if args.build:
+220        build(args.package, args.skip_tests, args.overwrite_dependencies)
 221
-222    if args.build:
-223        build(args.package, args.skip_tests, args.overwrite_dependencies)
+222    if args.increment_version:
+223        hassle_utilities.increment_version(pyproject_path,
+args.increment_version)
 224
 225    if args.update_changelog:
 226        hassle_utilities.update_changelog(pyproject_path)
 227        # If we're going to add tag for current version
 228        # commit changelog first
 229        if args.tag_version:
 230            input(
@@ -505,20 +505,20 @@
 213
 214    if args.generate_tests:
 215        generate_test_files(args.package)
 216
 217    if args.run_tests:
 218        run_tests(args.package)
 219
-220    if args.increment_version:
-221        hassle_utilities.increment_version(pyproject_path,
-args.increment_version)
+220    if args.build:
+221        build(args.package, args.skip_tests, args.overwrite_dependencies)
 222
-223    if args.build:
-224        build(args.package, args.skip_tests, args.overwrite_dependencies)
+223    if args.increment_version:
+224        hassle_utilities.increment_version(pyproject_path,
+args.increment_version)
 225
 226    if args.update_changelog:
 227        hassle_utilities.update_changelog(pyproject_path)
 228        # If we're going to add tag for current version
 229        # commit changelog first
 230        if args.tag_version:
 231            input(
```

### Comparing `hassle-2.8.1/docs/hassle/hassle_config.html` & `hassle-2.8.2/docs/hassle/hassle_config.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.1/docs/hassle/hassle_utilities.html` & `hassle-2.8.2/docs/hassle/hassle_utilities.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.1/docs/hassle/new_project.html` & `hassle-2.8.2/docs/hassle/new_project.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.1/docs/hassle/run_tests.html` & `hassle-2.8.2/docs/hassle/run_tests.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.1/src/hassle/generate_tests.py` & `hassle-2.8.2/src/hassle/generate_tests.py`

 * *Files identical despite different names*

### Comparing `hassle-2.8.1/src/hassle/hassle.py` & `hassle-2.8.2/src/hassle/hassle.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -212,20 +212,20 @@
 
     if args.generate_tests:
         generate_test_files(args.package)
 
     if args.run_tests:
         run_tests(args.package)
 
-    if args.increment_version:
-        hassle_utilities.increment_version(pyproject_path, args.increment_version)
-
     if args.build:
         build(args.package, args.skip_tests, args.overwrite_dependencies)
 
+    if args.increment_version:
+        hassle_utilities.increment_version(pyproject_path, args.increment_version)
+
     if args.update_changelog:
         hassle_utilities.update_changelog(pyproject_path)
         # If we're going to add tag for current version
         # commit changelog first
         if args.tag_version:
             input(
                 "Press enter to continue after optionally pruning the updated changelog..."
```

### Comparing `hassle-2.8.1/src/hassle/hassle_config.py` & `hassle-2.8.2/src/hassle/hassle_config.py`

 * *Files identical despite different names*

### Comparing `hassle-2.8.1/src/hassle/hassle_utilities.py` & `hassle-2.8.2/src/hassle/hassle_utilities.py`

 * *Files identical despite different names*

### Comparing `hassle-2.8.1/src/hassle/license_template.txt` & `hassle-2.8.2/src/hassle/license_template.txt`

 * *Files identical despite different names*

### Comparing `hassle-2.8.1/src/hassle/new_project.py` & `hassle-2.8.2/src/hassle/new_project.py`

 * *Files identical despite different names*

### Comparing `hassle-2.8.1/src/hassle/pyproject_template.toml` & `hassle-2.8.2/src/hassle/pyproject_template.toml`

 * *Files identical despite different names*

### Comparing `hassle-2.8.1/src/hassle/run_tests.py` & `hassle-2.8.2/src/hassle/run_tests.py`

 * *Files identical despite different names*

### Comparing `hassle-2.8.1/LICENSE.txt` & `hassle-2.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hassle-2.8.1/README.md` & `hassle-2.8.2/README.md`

 * *Files identical despite different names*

### Comparing `hassle-2.8.1/pyproject.toml` & `hassle-2.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 226d 6174 746d 616e 6573 4070 6d2e 6d65  "mattmanes@pm.me
 000000a0: 227d 5d0d 0a64 6573 6372 6970 7469 6f6e  "}]..description
 000000b0: 203d 2022 4372 6561 7465 2c20 6275 696c   = "Create, buil
 000000c0: 642c 2074 6573 742c 2061 6e64 2070 7562  d, test, and pub
 000000d0: 6c69 7368 2050 7974 686f 6e20 7072 6f6a  lish Python proj
 000000e0: 6563 7473 2061 6e64 2070 6163 6b61 6765  ects and package
 000000f0: 732e 220d 0a76 6572 7369 6f6e 203d 2022  s."..version = "
-00000100: 322e 382e 3122 0d0a 7265 7175 6972 6573  2.8.1"..requires
+00000100: 322e 382e 3222 0d0a 7265 7175 6972 6573  2.8.2"..requires
 00000110: 2d70 7974 686f 6e20 3d20 223e 3d33 2e31  -python = ">=3.1
 00000120: 3022 0d0a 6465 7065 6e64 656e 6369 6573  0"..dependencies
 00000130: 203d 205b 0d0a 2020 2020 2262 6c61 636b   = [..    "black
 00000140: 222c 200d 0a20 2020 2022 6973 6f72 7422  ", ..    "isort"
 00000150: 2c20 0d0a 2020 2020 2270 7974 6573 747e  , ..    "pytest~
 00000160: 3d37 2e32 2e31 222c 200d 0a20 2020 2022  =7.2.1", ..    "
 00000170: 636f 7665 7261 6765 222c 0d0a 2020 2020  coverage",..
```

### Comparing `hassle-2.8.1/PKG-INFO` & `hassle-2.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassle
-Version: 2.8.1
+Version: 2.8.2
 Summary: Create, build, test, and publish Python projects and packages.
 Project-URL: Homepage, https://github.com/matt-manes/hassle
 Project-URL: Documentation, https://github.com/matt-manes/hassle/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/hassle/tree/main/src/hassle
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: automation,build,devops,packaging,test
```

