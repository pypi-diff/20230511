# Comparing `tmp/generic-path-0.4.tar.gz` & `tmp/generic-path-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generic-path-0.4.tar", last modified: Thu May 11 04:06:33 2023, max compression
+gzip compressed data, was "generic-path-0.4.1.tar", last modified: Thu May 11 04:27:23 2023, max compression
```

## Comparing `generic-path-0.4.tar` & `generic-path-0.4.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 04:06:33.193546 generic-path-0.4/
--rw-rw-rw-   0        0        0     4131 2023-05-11 03:24:36.000000 generic-path-0.4/CHANGELOG.md
--rw-rw-rw-   0        0        0    17098 2023-05-02 02:11:14.000000 generic-path-0.4/LICENSE.txt
--rw-rw-rw-   0        0        0       22 2023-05-11 03:48:03.000000 generic-path-0.4/MANIFEST.in
--rw-rw-rw-   0        0        0    11410 2023-05-11 04:06:33.193546 generic-path-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5648 2023-05-11 03:52:10.000000 generic-path-0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 04:06:33.177546 generic-path-0.4/docs/
-drwxrwxrwx   0        0        0        0 2023-05-11 04:06:33.186546 generic-path-0.4/docs/html/
--rw-rw-rw-   0        0        0     3123 2023-05-06 01:58:24.000000 generic-path-0.4/docs/html/favicon.png
--rw-rw-rw-   0        0        0   522801 2023-05-11 03:49:45.000000 generic-path-0.4/docs/html/gpath.html
--rw-rw-rw-   0        0        0      136 2023-05-11 03:49:45.000000 generic-path-0.4/docs/html/index.html
--rw-rw-rw-   0        0        0   221953 2023-05-11 03:49:45.000000 generic-path-0.4/docs/html/search.js
--rw-rw-rw-   0        0        0     2208 2023-05-11 03:48:24.000000 generic-path-0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-11 04:06:33.193546 generic-path-0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-11 04:06:33.177546 generic-path-0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-11 04:06:33.189547 generic-path-0.4/src/generic_path.egg-info/
--rw-rw-rw-   0        0        0    11410 2023-05-11 04:06:33.000000 generic-path-0.4/src/generic_path.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2023-05-11 04:06:33.000000 generic-path-0.4/src/generic_path.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 04:06:33.000000 generic-path-0.4/src/generic_path.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      300 2023-05-11 04:06:33.000000 generic-path-0.4/src/generic_path.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-11 04:06:33.000000 generic-path-0.4/src/generic_path.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-11 04:06:33.190546 generic-path-0.4/src/gpath/
--rw-rw-rw-   0        0        0       97 2023-05-11 04:06:05.000000 generic-path-0.4/src/gpath/__init__.py
--rw-rw-rw-   0        0        0      212 2023-05-11 00:59:57.000000 generic-path-0.4/src/gpath/_compat.py
--rw-rw-rw-   0        0        0    36829 2023-05-11 02:28:52.000000 generic-path-0.4/src/gpath/_gpath.py
-drwxrwxrwx   0        0        0        0 2023-05-11 04:06:33.191546 generic-path-0.4/src/gpath/_rules/
--rw-rw-rw-   0        0        0      129 2023-05-11 00:59:57.000000 generic-path-0.4/src/gpath/_rules/__init__.py
--rw-rw-rw-   0        0        0      146 2023-05-11 00:59:57.000000 generic-path-0.4/src/gpath/_rules/_common.py
--rw-rw-rw-   0        0        0      409 2023-05-11 00:59:57.000000 generic-path-0.4/src/gpath/_rules/_rules.py
-drwxrwxrwx   0        0        0        0 2023-05-11 04:06:33.192547 generic-path-0.4/tests/
--rw-rw-rw-   0        0        0    37854 2023-05-11 02:28:00.000000 generic-path-0.4/tests/test_gpath.py
+drwxrwxrwx   0        0        0        0 2023-05-11 04:27:23.241230 generic-path-0.4.1/
+-rw-rw-rw-   0        0        0     4178 2023-05-11 04:20:31.000000 generic-path-0.4.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0    17098 2023-05-02 02:11:14.000000 generic-path-0.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       22 2023-05-11 04:07:03.000000 generic-path-0.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    11459 2023-05-11 04:27:23.240231 generic-path-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5648 2023-05-11 04:07:03.000000 generic-path-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 04:27:23.195188 generic-path-0.4.1/docs/
+drwxrwxrwx   0        0        0        0 2023-05-11 04:27:23.231708 generic-path-0.4.1/docs/html/
+-rw-rw-rw-   0        0        0     3123 2023-05-06 01:58:24.000000 generic-path-0.4.1/docs/html/favicon.png
+-rw-rw-rw-   0        0        0   522665 2023-05-11 04:27:13.000000 generic-path-0.4.1/docs/html/gpath.html
+-rw-rw-rw-   0        0        0      136 2023-05-11 04:27:13.000000 generic-path-0.4.1/docs/html/index.html
+-rw-rw-rw-   0        0        0   221787 2023-05-11 04:27:13.000000 generic-path-0.4.1/docs/html/search.js
+-rw-rw-rw-   0        0        0     2208 2023-05-11 04:07:03.000000 generic-path-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 04:27:23.241230 generic-path-0.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 04:27:23.196188 generic-path-0.4.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 04:27:23.235709 generic-path-0.4.1/src/generic_path.egg-info/
+-rw-rw-rw-   0        0        0    11459 2023-05-11 04:27:23.000000 generic-path-0.4.1/src/generic_path.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2023-05-11 04:27:23.000000 generic-path-0.4.1/src/generic_path.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 04:27:23.000000 generic-path-0.4.1/src/generic_path.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      300 2023-05-11 04:27:23.000000 generic-path-0.4.1/src/generic_path.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-11 04:27:23.000000 generic-path-0.4.1/src/generic_path.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 04:27:23.237710 generic-path-0.4.1/src/gpath/
+-rw-rw-rw-   0        0        0       99 2023-05-11 04:26:56.000000 generic-path-0.4.1/src/gpath/__init__.py
+-rw-rw-rw-   0        0        0      212 2023-05-11 04:07:03.000000 generic-path-0.4.1/src/gpath/_compat.py
+-rw-rw-rw-   0        0        0    36783 2023-05-11 04:19:47.000000 generic-path-0.4.1/src/gpath/_gpath.py
+drwxrwxrwx   0        0        0        0 2023-05-11 04:27:23.239229 generic-path-0.4.1/src/gpath/_rules/
+-rw-rw-rw-   0        0        0      129 2023-05-11 04:07:03.000000 generic-path-0.4.1/src/gpath/_rules/__init__.py
+-rw-rw-rw-   0        0        0      146 2023-05-11 04:07:03.000000 generic-path-0.4.1/src/gpath/_rules/_common.py
+-rw-rw-rw-   0        0        0      409 2023-05-11 04:07:03.000000 generic-path-0.4.1/src/gpath/_rules/_rules.py
+drwxrwxrwx   0        0        0        0 2023-05-11 04:27:23.240231 generic-path-0.4.1/tests/
+-rw-rw-rw-   0        0        0    37854 2023-05-11 04:07:03.000000 generic-path-0.4.1/tests/test_gpath.py
```

### Comparing `generic-path-0.4/CHANGELOG.md` & `generic-path-0.4.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 ## Changelog
 
 This project follows [PEP 440](https://peps.python.org/pep-0440/) and [Semantic Versioning (SemVer)](https://semver.org/spec/v2.0.0.html). In addition to the guarantees specified by SemVer, for versions before 1.0, this project guarantees backwards compatibility of the API for patch version updates (0.<var>y</var>.<b><var>z</var></b>).
 
 The recommended version specifier is <code>generic-path ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>generic-path ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
 
+### 0.4.1
+
+- Fixed embedded documentation
+
 ### 0.4
 
 #### Breaking API changes
 
 - Replaced the following instance methods with read-only properties:
 	- <code><var>g</var>.get_parent_level()</code> → <code><var>g</var>.parent_level</code>
 	- <code><var>g</var>.get_parent_parts()</code> → <code><var>g</var>.parent_parts</code>
```

### Comparing `generic-path-0.4/LICENSE.txt` & `generic-path-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `generic-path-0.4/PKG-INFO` & `generic-path-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generic-path
-Version: 0.4
+Version: 0.4.1
 Summary: Generalised abstract file path that provides path manipulations independent from the local environment
 Author-email: Yu Shiyang <yu.shiyang@gnayihs.uy>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/yushiyangk/GPath
 Project-URL: Documentation, https://gpath.gnayihs.uy/
 Project-URL: Issues, https://github.com/yushiyangk/GPath/issues
 Keywords: python,filepath,filesystem,cross-platform
@@ -179,14 +179,18 @@
 
 ## Changelog
 
 This project follows [PEP 440](https://peps.python.org/pep-0440/) and [Semantic Versioning (SemVer)](https://semver.org/spec/v2.0.0.html). In addition to the guarantees specified by SemVer, for versions before 1.0, this project guarantees backwards compatibility of the API for patch version updates (0.<var>y</var>.<b><var>z</var></b>).
 
 The recommended version specifier is <code>generic-path ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>generic-path ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
 
+### 0.4.1
+
+- Fixed embedded documentation
+
 ### 0.4
 
 #### Breaking API changes
 
 - Replaced the following instance methods with read-only properties:
 	- <code><var>g</var>.get_parent_level()</code> → <code><var>g</var>.parent_level</code>
 	- <code><var>g</var>.get_parent_parts()</code> → <code><var>g</var>.parent_parts</code>
```

### Comparing `generic-path-0.4/README.md` & `generic-path-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `generic-path-0.4/docs/html/favicon.png` & `generic-path-0.4.1/docs/html/favicon.png`

 * *Files identical despite different names*

### Comparing `generic-path-0.4/docs/html/gpath.html` & `generic-path-0.4.1/docs/html/gpath.html`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,15 @@
 gpath    </h1>
 
                 
                         <input id="mod-gpath-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-gpath-view-source"><span>View Source</span></label>
 
-                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">1</span></a><span class="n">__version__</span> <span class="o">=</span> <span class="s1">&#39;0.4.dev3&#39;</span>
+                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">1</span></a><span class="n">__version__</span> <span class="o">=</span> <span class="s1">&#39;0.4.1&#39;</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos">2</span></a>
 </span><span id="L-3"><a href="#L-3"><span class="linenos">3</span></a><span class="kn">from</span> <span class="nn">._gpath</span> <span class="kn">import</span> <span class="n">GPath</span><span class="p">,</span> <span class="n">GPathLike</span>
 </span><span id="L-4"><a href="#L-4"><span class="linenos">4</span></a>
 </span><span id="L-5"><a href="#L-5"><span class="linenos">5</span></a><span class="n">__all__</span> <span class="o">=</span> <span class="p">(</span><span class="s1">&#39;GPath&#39;</span><span class="p">,</span> <span class="s1">&#39;GPathLike&#39;</span><span class="p">)</span>
 </span></pre></div>
 
 
@@ -326,27 +326,27 @@
 </span><span id="GPath-155"><a href="#GPath-155"><span class="linenos"> 155</span></a>			<span class="k">else</span><span class="p">:</span>
 </span><span id="GPath-156"><a href="#GPath-156"><span class="linenos"> 156</span></a>				<span class="n">path</span> <span class="o">=</span> <span class="n">path</span><span class="o">.</span><span class="n">decode</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_encoding</span><span class="p">)</span>
 </span><span id="GPath-157"><a href="#GPath-157"><span class="linenos"> 157</span></a>
 </span><span id="GPath-158"><a href="#GPath-158"><span class="linenos"> 158</span></a>		<span class="c1"># path is a str</span>
 </span><span id="GPath-159"><a href="#GPath-159"><span class="linenos"> 159</span></a>
 </span><span id="GPath-160"><a href="#GPath-160"><span class="linenos"> 160</span></a>		<span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">path</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="mi">2</span> <span class="ow">and</span> <span class="n">path</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span> <span class="ow">in</span> <span class="n">_rules</span><span class="o">.</span><span class="n">generic_rules</span><span class="o">.</span><span class="n">drive_postfixes</span><span class="p">:</span>
 </span><span id="GPath-161"><a href="#GPath-161"><span class="linenos"> 161</span></a>			<span class="bp">self</span><span class="o">.</span><span class="n">_drive</span> <span class="o">=</span> <span class="n">path</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="GPath-162"><a href="#GPath-162"><span class="linenos"> 162</span></a>			<span class="n">deviceless_path</span> <span class="o">=</span> <span class="n">path</span><span class="p">[</span><span class="mi">2</span><span class="p">:]</span>
+</span><span id="GPath-162"><a href="#GPath-162"><span class="linenos"> 162</span></a>			<span class="n">driveless_path</span> <span class="o">=</span> <span class="n">path</span><span class="p">[</span><span class="mi">2</span><span class="p">:]</span>
 </span><span id="GPath-163"><a href="#GPath-163"><span class="linenos"> 163</span></a>		<span class="k">else</span><span class="p">:</span>
-</span><span id="GPath-164"><a href="#GPath-164"><span class="linenos"> 164</span></a>			<span class="n">deviceless_path</span> <span class="o">=</span> <span class="n">path</span>
+</span><span id="GPath-164"><a href="#GPath-164"><span class="linenos"> 164</span></a>			<span class="n">driveless_path</span> <span class="o">=</span> <span class="n">path</span>
 </span><span id="GPath-165"><a href="#GPath-165"><span class="linenos"> 165</span></a>
 </span><span id="GPath-166"><a href="#GPath-166"><span class="linenos"> 166</span></a>		<span class="k">for</span> <span class="n">root</span> <span class="ow">in</span> <span class="n">_rules</span><span class="o">.</span><span class="n">generic_rules</span><span class="o">.</span><span class="n">roots</span><span class="p">:</span>
-</span><span id="GPath-167"><a href="#GPath-167"><span class="linenos"> 167</span></a>			<span class="k">if</span> <span class="n">deviceless_path</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="n">root</span><span class="p">):</span>
+</span><span id="GPath-167"><a href="#GPath-167"><span class="linenos"> 167</span></a>			<span class="k">if</span> <span class="n">driveless_path</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="n">root</span><span class="p">):</span>
 </span><span id="GPath-168"><a href="#GPath-168"><span class="linenos"> 168</span></a>				<span class="bp">self</span><span class="o">.</span><span class="n">_root</span> <span class="o">=</span> <span class="kc">True</span>
 </span><span id="GPath-169"><a href="#GPath-169"><span class="linenos"> 169</span></a>				<span class="k">break</span>
 </span><span id="GPath-170"><a href="#GPath-170"><span class="linenos"> 170</span></a>
 </span><span id="GPath-171"><a href="#GPath-171"><span class="linenos"> 171</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_root</span><span class="p">:</span>
-</span><span id="GPath-172"><a href="#GPath-172"><span class="linenos"> 172</span></a>			<span class="n">rootless_path</span> <span class="o">=</span> <span class="n">deviceless_path</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
+</span><span id="GPath-172"><a href="#GPath-172"><span class="linenos"> 172</span></a>			<span class="n">rootless_path</span> <span class="o">=</span> <span class="n">driveless_path</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
 </span><span id="GPath-173"><a href="#GPath-173"><span class="linenos"> 173</span></a>		<span class="k">else</span><span class="p">:</span>
-</span><span id="GPath-174"><a href="#GPath-174"><span class="linenos"> 174</span></a>			<span class="n">rootless_path</span> <span class="o">=</span> <span class="n">deviceless_path</span>
+</span><span id="GPath-174"><a href="#GPath-174"><span class="linenos"> 174</span></a>			<span class="n">rootless_path</span> <span class="o">=</span> <span class="n">driveless_path</span>
 </span><span id="GPath-175"><a href="#GPath-175"><span class="linenos"> 175</span></a>
 </span><span id="GPath-176"><a href="#GPath-176"><span class="linenos"> 176</span></a>
 </span><span id="GPath-177"><a href="#GPath-177"><span class="linenos"> 177</span></a>		<span class="n">parts</span> <span class="o">=</span> <span class="n">_split_relative</span><span class="p">(</span><span class="n">rootless_path</span><span class="p">,</span> <span class="n">delimiters</span><span class="o">=</span><span class="p">(</span><span class="nb">set</span><span class="p">(</span><span class="n">_rules</span><span class="o">.</span><span class="n">generic_rules</span><span class="o">.</span><span class="n">separators</span><span class="p">)</span> <span class="o">|</span> <span class="nb">set</span><span class="p">(</span><span class="n">_rules</span><span class="o">.</span><span class="n">generic_rules</span><span class="o">.</span><span class="n">separators</span><span class="p">)))</span>
 </span><span id="GPath-178"><a href="#GPath-178"><span class="linenos"> 178</span></a>		<span class="n">parts</span> <span class="o">=</span> <span class="n">_normalise_relative</span><span class="p">(</span><span class="n">parts</span><span class="p">)</span>
 </span><span id="GPath-179"><a href="#GPath-179"><span class="linenos"> 179</span></a>		<span class="n">parent_level</span> <span class="o">=</span> <span class="mi">0</span>
 </span><span id="GPath-180"><a href="#GPath-180"><span class="linenos"> 180</span></a>		<span class="k">while</span> <span class="n">parent_level</span> <span class="o">&lt;</span> <span class="nb">len</span><span class="p">(</span><span class="n">parts</span><span class="p">)</span> <span class="ow">and</span> <span class="n">parts</span><span class="p">[</span><span class="n">parent_level</span><span class="p">]</span> <span class="ow">in</span> <span class="n">_rules</span><span class="o">.</span><span class="n">generic_rules</span><span class="o">.</span><span class="n">parent_indicators</span><span class="p">:</span>
 </span><span id="GPath-181"><a href="#GPath-181"><span class="linenos"> 181</span></a>			<span class="n">parent_level</span> <span class="o">+=</span> <span class="mi">1</span>
@@ -354,15 +354,15 @@
 </span><span id="GPath-183"><a href="#GPath-183"><span class="linenos"> 183</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_root</span> <span class="o">==</span> <span class="kc">False</span><span class="p">:</span>
 </span><span id="GPath-184"><a href="#GPath-184"><span class="linenos"> 184</span></a>			<span class="bp">self</span><span class="o">.</span><span class="n">_parent_level</span> <span class="o">=</span> <span class="n">parent_level</span>
 </span><span id="GPath-185"><a href="#GPath-185"><span class="linenos"> 185</span></a>
 </span><span id="GPath-186"><a href="#GPath-186"><span class="linenos"> 186</span></a>
 </span><span id="GPath-187"><a href="#GPath-187"><span class="linenos"> 187</span></a>	<span class="nd">@property</span>
 </span><span id="GPath-188"><a href="#GPath-188"><span class="linenos"> 188</span></a>	<span class="k">def</span> <span class="nf">named_parts</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
 </span><span id="GPath-189"><a href="#GPath-189"><span class="linenos"> 189</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="GPath-190"><a href="#GPath-190"><span class="linenos"> 190</span></a><span class="sd">			Read-only named components of the path, not including the filesystem root, device name, or any parent directories</span>
+</span><span id="GPath-190"><a href="#GPath-190"><span class="linenos"> 190</span></a><span class="sd">			Read-only named components of the path, not including the filesystem root, drive name, or any parent directories</span>
 </span><span id="GPath-191"><a href="#GPath-191"><span class="linenos"> 191</span></a>
 </span><span id="GPath-192"><a href="#GPath-192"><span class="linenos"> 192</span></a><span class="sd">			Examples</span>
 </span><span id="GPath-193"><a href="#GPath-193"><span class="linenos"> 193</span></a><span class="sd">			--------</span>
 </span><span id="GPath-194"><a href="#GPath-194"><span class="linenos"> 194</span></a><span class="sd">			```python</span>
 </span><span id="GPath-195"><a href="#GPath-195"><span class="linenos"> 195</span></a><span class="sd">			GPath(&quot;usr/local/bin&quot;).named_parts     # [&quot;usr&quot;, &quot;local&quot;, &quot;bin&quot;]</span>
 </span><span id="GPath-196"><a href="#GPath-196"><span class="linenos"> 196</span></a><span class="sd">			GPath(&quot;../../Documents&quot;).named_parts   # [&quot;Documents&quot;]</span>
 </span><span id="GPath-197"><a href="#GPath-197"><span class="linenos"> 197</span></a><span class="sd">			GPath(&quot;/usr/bin&quot;).named_parts          # [&quot;usr&quot;, &quot;bin&quot;]</span>
@@ -398,15 +398,15 @@
 </span><span id="GPath-227"><a href="#GPath-227"><span class="linenos"> 227</span></a><span class="sd">			```</span>
 </span><span id="GPath-228"><a href="#GPath-228"><span class="linenos"> 228</span></a><span class="sd">		&quot;&quot;&quot;</span>
 </span><span id="GPath-229"><a href="#GPath-229"><span class="linenos"> 229</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">_rules</span><span class="o">.</span><span class="n">generic_rules</span><span class="o">.</span><span class="n">parent_indicators</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_parent_level</span><span class="p">)]</span>
 </span><span id="GPath-230"><a href="#GPath-230"><span class="linenos"> 230</span></a>
 </span><span id="GPath-231"><a href="#GPath-231"><span class="linenos"> 231</span></a>	<span class="nd">@property</span>
 </span><span id="GPath-232"><a href="#GPath-232"><span class="linenos"> 232</span></a>	<span class="k">def</span> <span class="nf">relative_parts</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
 </span><span id="GPath-233"><a href="#GPath-233"><span class="linenos"> 233</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="GPath-234"><a href="#GPath-234"><span class="linenos"> 234</span></a><span class="sd">			Read-only relative components of the path, not including the filesystem root or device name, with a copy of `parent_indicator` for each level of parent directory</span>
+</span><span id="GPath-234"><a href="#GPath-234"><span class="linenos"> 234</span></a><span class="sd">			Read-only relative components of the path, not including the filesystem root or drive name, with a copy of `parent_indicator` for each level of parent directory</span>
 </span><span id="GPath-235"><a href="#GPath-235"><span class="linenos"> 235</span></a>
 </span><span id="GPath-236"><a href="#GPath-236"><span class="linenos"> 236</span></a><span class="sd">			Examples</span>
 </span><span id="GPath-237"><a href="#GPath-237"><span class="linenos"> 237</span></a><span class="sd">			--------</span>
 </span><span id="GPath-238"><a href="#GPath-238"><span class="linenos"> 238</span></a><span class="sd">			```python</span>
 </span><span id="GPath-239"><a href="#GPath-239"><span class="linenos"> 239</span></a><span class="sd">			GPath(&quot;usr/local/bin&quot;).relative_parts     # [&quot;usr&quot;, &quot;local&quot;, &quot;bin&quot;]</span>
 </span><span id="GPath-240"><a href="#GPath-240"><span class="linenos"> 240</span></a><span class="sd">			GPath(&quot;../../Documents&quot;).relative_parts   # [&quot;..&quot;, &quot;..&quot;, &quot;Documents&quot;]</span>
 </span><span id="GPath-241"><a href="#GPath-241"><span class="linenos"> 241</span></a><span class="sd">			GPath(&quot;/usr/bin&quot;).relative_parts          # [&quot;usr&quot;, &quot;bin&quot;]</span>
@@ -414,22 +414,22 @@
 </span><span id="GPath-243"><a href="#GPath-243"><span class="linenos"> 243</span></a><span class="sd">			```</span>
 </span><span id="GPath-244"><a href="#GPath-244"><span class="linenos"> 244</span></a><span class="sd">		&quot;&quot;&quot;</span>
 </span><span id="GPath-245"><a href="#GPath-245"><span class="linenos"> 245</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parent_parts</span> <span class="o">+</span> <span class="nb">list</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_parts</span><span class="p">)</span>
 </span><span id="GPath-246"><a href="#GPath-246"><span class="linenos"> 246</span></a>
 </span><span id="GPath-247"><a href="#GPath-247"><span class="linenos"> 247</span></a>	<span class="nd">@property</span>
 </span><span id="GPath-248"><a href="#GPath-248"><span class="linenos"> 248</span></a>	<span class="k">def</span> <span class="nf">drive</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
 </span><span id="GPath-249"><a href="#GPath-249"><span class="linenos"> 249</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="GPath-250"><a href="#GPath-250"><span class="linenos"> 250</span></a><span class="sd">			Read-only device name</span>
+</span><span id="GPath-250"><a href="#GPath-250"><span class="linenos"> 250</span></a><span class="sd">			Read-only drive name</span>
 </span><span id="GPath-251"><a href="#GPath-251"><span class="linenos"> 251</span></a>
 </span><span id="GPath-252"><a href="#GPath-252"><span class="linenos"> 252</span></a><span class="sd">			Examples</span>
 </span><span id="GPath-253"><a href="#GPath-253"><span class="linenos"> 253</span></a><span class="sd">			--------</span>
 </span><span id="GPath-254"><a href="#GPath-254"><span class="linenos"> 254</span></a><span class="sd">			```python</span>
-</span><span id="GPath-255"><a href="#GPath-255"><span class="linenos"> 255</span></a><span class="sd">			GPath(&quot;C:/Windows&quot;).device       # &quot;C:&quot;</span>
-</span><span id="GPath-256"><a href="#GPath-256"><span class="linenos"> 256</span></a><span class="sd">			GPath(&quot;/usr/bin&quot;).device         # &quot;&quot;</span>
-</span><span id="GPath-257"><a href="#GPath-257"><span class="linenos"> 257</span></a><span class="sd">			GPath(&quot;../../Documents&quot;).device  # &quot;&quot;</span>
+</span><span id="GPath-255"><a href="#GPath-255"><span class="linenos"> 255</span></a><span class="sd">			GPath(&quot;C:/Windows&quot;).drive       # &quot;C:&quot;</span>
+</span><span id="GPath-256"><a href="#GPath-256"><span class="linenos"> 256</span></a><span class="sd">			GPath(&quot;/usr/bin&quot;).drive         # &quot;&quot;</span>
+</span><span id="GPath-257"><a href="#GPath-257"><span class="linenos"> 257</span></a><span class="sd">			GPath(&quot;../../Documents&quot;).drive  # &quot;&quot;</span>
 </span><span id="GPath-258"><a href="#GPath-258"><span class="linenos"> 258</span></a><span class="sd">			```</span>
 </span><span id="GPath-259"><a href="#GPath-259"><span class="linenos"> 259</span></a><span class="sd">		&quot;&quot;&quot;</span>
 </span><span id="GPath-260"><a href="#GPath-260"><span class="linenos"> 260</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_drive</span>
 </span><span id="GPath-261"><a href="#GPath-261"><span class="linenos"> 261</span></a>
 </span><span id="GPath-262"><a href="#GPath-262"><span class="linenos"> 262</span></a>	<span class="nd">@property</span>
 </span><span id="GPath-263"><a href="#GPath-263"><span class="linenos"> 263</span></a>	<span class="k">def</span> <span class="nf">absolute</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
 </span><span id="GPath-264"><a href="#GPath-264"><span class="linenos"> 264</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
@@ -737,15 +737,15 @@
 </span><span id="GPath-566"><a href="#GPath-566"><span class="linenos"> 566</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">with_drive</span><span class="p">(</span><span class="kc">None</span><span class="p">)</span>
 </span><span id="GPath-567"><a href="#GPath-567"><span class="linenos"> 567</span></a>
 </span><span id="GPath-568"><a href="#GPath-568"><span class="linenos"> 568</span></a>
 </span><span id="GPath-569"><a href="#GPath-569"><span class="linenos"> 569</span></a>	<span class="k">def</span> <span class="nf">common_with</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">other</span><span class="p">:</span> <span class="n">GPathLike</span><span class="p">,</span> <span class="n">allow_current</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_parents</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Optional</span><span class="p">[</span><span class="n">GPath</span><span class="p">]:</span>
 </span><span id="GPath-570"><a href="#GPath-570"><span class="linenos"> 570</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
 </span><span id="GPath-571"><a href="#GPath-571"><span class="linenos"> 571</span></a><span class="sd">			Find the longest common base path shared between `self` and `other`, or return None if no such path exists.</span>
 </span><span id="GPath-572"><a href="#GPath-572"><span class="linenos"> 572</span></a>
-</span><span id="GPath-573"><a href="#GPath-573"><span class="linenos"> 573</span></a><span class="sd">			A common base path might not exist if one path is an absolute path while the other is a relative path, or if the two paths are in different filesystems (with different device names), or in other cases as controlled by the `allow_current` and `allow_parents` options.</span>
+</span><span id="GPath-573"><a href="#GPath-573"><span class="linenos"> 573</span></a><span class="sd">			A common base path might not exist if one path is an absolute path while the other is a relative path, or if the two paths are in different filesystems (with different drive names), or in other cases as controlled by the `allow_current` and `allow_parents` options.</span>
 </span><span id="GPath-574"><a href="#GPath-574"><span class="linenos"> 574</span></a>
 </span><span id="GPath-575"><a href="#GPath-575"><span class="linenos"> 575</span></a><span class="sd">			If using the default options of `allow_current=True` and `allow_parent=False`, the binary operator for bitwise-and can be used: `__and__()` (usage: &lt;code&gt;&lt;var&gt;g1&lt;/var&gt; &amp; &lt;var&gt;g2&lt;/var&gt;&lt;/code&gt;).</span>
 </span><span id="GPath-576"><a href="#GPath-576"><span class="linenos"> 576</span></a>
 </span><span id="GPath-577"><a href="#GPath-577"><span class="linenos"> 577</span></a><span class="sd">			Parameters</span>
 </span><span id="GPath-578"><a href="#GPath-578"><span class="linenos"> 578</span></a><span class="sd">			----------</span>
 </span><span id="GPath-579"><a href="#GPath-579"><span class="linenos"> 579</span></a><span class="sd">			`other`</span>
 </span><span id="GPath-580"><a href="#GPath-580"><span class="linenos"> 580</span></a><span class="sd">			: the path to compare with</span>
@@ -1019,15 +1019,15 @@
 </span><span id="GPath-848"><a href="#GPath-848"><span class="linenos"> 848</span></a>			<span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;GPath(</span><span class="si">{</span><span class="nb">repr</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">))</span><span class="si">}{</span><span class="n">encoding_repr</span><span class="si">}</span><span class="s2">)&quot;</span>
 </span><span id="GPath-849"><a href="#GPath-849"><span class="linenos"> 849</span></a>		<span class="k">else</span><span class="p">:</span>
 </span><span id="GPath-850"><a href="#GPath-850"><span class="linenos"> 850</span></a>			<span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;GPath(</span><span class="si">{</span><span class="nb">repr</span><span class="p">(</span><span class="s1">&#39;&#39;</span><span class="p">)</span><span class="si">}{</span><span class="n">encoding_repr</span><span class="si">}</span><span class="s2">)&quot;</span>
 </span><span id="GPath-851"><a href="#GPath-851"><span class="linenos"> 851</span></a>
 </span><span id="GPath-852"><a href="#GPath-852"><span class="linenos"> 852</span></a>
 </span><span id="GPath-853"><a href="#GPath-853"><span class="linenos"> 853</span></a>	<span class="k">def</span> <span class="fm">__len__</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
 </span><span id="GPath-854"><a href="#GPath-854"><span class="linenos"> 854</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="GPath-855"><a href="#GPath-855"><span class="linenos"> 855</span></a><span class="sd">			Get the number of named path components, excluding any device name or parent directories.</span>
+</span><span id="GPath-855"><a href="#GPath-855"><span class="linenos"> 855</span></a><span class="sd">			Get the number of named path components, excluding any drive name or parent directories.</span>
 </span><span id="GPath-856"><a href="#GPath-856"><span class="linenos"> 856</span></a>
 </span><span id="GPath-857"><a href="#GPath-857"><span class="linenos"> 857</span></a><span class="sd">			Usage: &lt;code&gt;len(&lt;var&gt;g&lt;/var&gt;)&lt;/code&gt;</span>
 </span><span id="GPath-858"><a href="#GPath-858"><span class="linenos"> 858</span></a>
 </span><span id="GPath-859"><a href="#GPath-859"><span class="linenos"> 859</span></a><span class="sd">			Examples</span>
 </span><span id="GPath-860"><a href="#GPath-860"><span class="linenos"> 860</span></a><span class="sd">			--------</span>
 </span><span id="GPath-861"><a href="#GPath-861"><span class="linenos"> 861</span></a><span class="sd">			```python</span>
 </span><span id="GPath-862"><a href="#GPath-862"><span class="linenos"> 862</span></a><span class="sd">			len(GPath(&quot;/usr/bin&quot;))    # 2</span>
@@ -1037,15 +1037,15 @@
 </span><span id="GPath-866"><a href="#GPath-866"><span class="linenos"> 866</span></a><span class="sd">			```</span>
 </span><span id="GPath-867"><a href="#GPath-867"><span class="linenos"> 867</span></a><span class="sd">		&quot;&quot;&quot;</span>
 </span><span id="GPath-868"><a href="#GPath-868"><span class="linenos"> 868</span></a>		<span class="k">return</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_parts</span><span class="p">)</span>
 </span><span id="GPath-869"><a href="#GPath-869"><span class="linenos"> 869</span></a>
 </span><span id="GPath-870"><a href="#GPath-870"><span class="linenos"> 870</span></a>
 </span><span id="GPath-871"><a href="#GPath-871"><span class="linenos"> 871</span></a>	<span class="k">def</span> <span class="fm">__getitem__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">index</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="nb">int</span><span class="p">,</span> <span class="nb">slice</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]]:</span>
 </span><span id="GPath-872"><a href="#GPath-872"><span class="linenos"> 872</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="GPath-873"><a href="#GPath-873"><span class="linenos"> 873</span></a><span class="sd">			Get a 0-indexed named path component, or a slice of path components, excluding any device name or parent directories.</span>
+</span><span id="GPath-873"><a href="#GPath-873"><span class="linenos"> 873</span></a><span class="sd">			Get a 0-indexed named path component, or a slice of path components, excluding any drive name or parent directories.</span>
 </span><span id="GPath-874"><a href="#GPath-874"><span class="linenos"> 874</span></a>
 </span><span id="GPath-875"><a href="#GPath-875"><span class="linenos"> 875</span></a><span class="sd">			Usage: &lt;code&gt;&lt;var&gt;g&lt;/var&gt;[&lt;var&gt;n&lt;/var&gt;]&lt;/code&gt;, &lt;code&gt;&lt;var&gt;g&lt;/var&gt;[&lt;var&gt;start&lt;/var&gt;:&lt;var&gt;end&lt;/var&gt;]&lt;/code&gt;, &lt;code&gt;&lt;var&gt;g&lt;/var&gt;[&lt;var&gt;start&lt;/var&gt;:&lt;var&gt;end&lt;/var&gt;:&lt;var&gt;step&lt;/var&gt;]&lt;/code&gt;, etc.</span>
 </span><span id="GPath-876"><a href="#GPath-876"><span class="linenos"> 876</span></a>
 </span><span id="GPath-877"><a href="#GPath-877"><span class="linenos"> 877</span></a><span class="sd">			Examples</span>
 </span><span id="GPath-878"><a href="#GPath-878"><span class="linenos"> 878</span></a><span class="sd">			--------</span>
 </span><span id="GPath-879"><a href="#GPath-879"><span class="linenos"> 879</span></a><span class="sd">			```python</span>
 </span><span id="GPath-880"><a href="#GPath-880"><span class="linenos"> 880</span></a><span class="sd">			GPath(&quot;/usr/local/bin&quot;)[1]    # &quot;local&quot;</span>
@@ -1058,15 +1058,15 @@
 </span><span id="GPath-887"><a href="#GPath-887"><span class="linenos"> 887</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_parts</span><span class="p">[</span><span class="n">index</span><span class="p">]</span>
 </span><span id="GPath-888"><a href="#GPath-888"><span class="linenos"> 888</span></a>		<span class="k">elif</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">index</span><span class="p">,</span> <span class="nb">slice</span><span class="p">):</span>
 </span><span id="GPath-889"><a href="#GPath-889"><span class="linenos"> 889</span></a>			<span class="k">return</span> <span class="nb">list</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_parts</span><span class="p">[</span><span class="n">index</span><span class="p">])</span>
 </span><span id="GPath-890"><a href="#GPath-890"><span class="linenos"> 890</span></a>
 </span><span id="GPath-891"><a href="#GPath-891"><span class="linenos"> 891</span></a>
 </span><span id="GPath-892"><a href="#GPath-892"><span class="linenos"> 892</span></a>	<span class="k">def</span> <span class="fm">__iter__</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Iterator</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
 </span><span id="GPath-893"><a href="#GPath-893"><span class="linenos"> 893</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="GPath-894"><a href="#GPath-894"><span class="linenos"> 894</span></a><span class="sd">			Get an iterator through the named path components, excluding any device name or parent directories.</span>
+</span><span id="GPath-894"><a href="#GPath-894"><span class="linenos"> 894</span></a><span class="sd">			Get an iterator through the named path components, excluding any drive name or parent directories.</span>
 </span><span id="GPath-895"><a href="#GPath-895"><span class="linenos"> 895</span></a>
 </span><span id="GPath-896"><a href="#GPath-896"><span class="linenos"> 896</span></a><span class="sd">			Usage: &lt;code&gt;iter(&lt;var&gt;g&lt;/var&gt;)&lt;/code&gt; or &lt;code&gt;for &lt;var&gt;p&lt;/var&gt; in &lt;var&gt;g&lt;/var&gt;:&lt;/code&gt;</span>
 </span><span id="GPath-897"><a href="#GPath-897"><span class="linenos"> 897</span></a><span class="sd">		&quot;&quot;&quot;</span>
 </span><span id="GPath-898"><a href="#GPath-898"><span class="linenos"> 898</span></a>		<span class="k">return</span> <span class="nb">iter</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_parts</span><span class="p">)</span>
 </span><span id="GPath-899"><a href="#GPath-899"><span class="linenos"> 899</span></a>
 </span><span id="GPath-900"><a href="#GPath-900"><span class="linenos"> 900</span></a>
 </span><span id="GPath-901"><a href="#GPath-901"><span class="linenos"> 901</span></a>	<span class="k">def</span> <span class="fm">__contains__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">other</span><span class="p">:</span> <span class="n">GPathLike</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
@@ -1093,17 +1093,17 @@
 </span><span id="GPath-922"><a href="#GPath-922"><span class="linenos"> 922</span></a>		<span class="k">return</span> <span class="n">common_path</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="n">common_path</span> <span class="o">==</span> <span class="bp">self</span>
 </span><span id="GPath-923"><a href="#GPath-923"><span class="linenos"> 923</span></a>
 </span><span id="GPath-924"><a href="#GPath-924"><span class="linenos"> 924</span></a>
 </span><span id="GPath-925"><a href="#GPath-925"><span class="linenos"> 925</span></a>	<span class="k">def</span> <span class="fm">__add__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">other</span><span class="p">:</span> <span class="n">GPathLike</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">GPath</span><span class="p">:</span>
 </span><span id="GPath-926"><a href="#GPath-926"><span class="linenos"> 926</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
 </span><span id="GPath-927"><a href="#GPath-927"><span class="linenos"> 927</span></a><span class="sd">			Add (concatenate) `other` to the end of `self`, and return a new copy.</span>
 </span><span id="GPath-928"><a href="#GPath-928"><span class="linenos"> 928</span></a>
-</span><span id="GPath-929"><a href="#GPath-929"><span class="linenos"> 929</span></a><span class="sd">			If `other` is an absolute path, the returned path will be an absolute path that matches `other`, apart from the device name.</span>
+</span><span id="GPath-929"><a href="#GPath-929"><span class="linenos"> 929</span></a><span class="sd">			If `other` is an absolute path, the returned path will be an absolute path that matches `other`, apart from the drive name.</span>
 </span><span id="GPath-930"><a href="#GPath-930"><span class="linenos"> 930</span></a>
-</span><span id="GPath-931"><a href="#GPath-931"><span class="linenos"> 931</span></a><span class="sd">			If `other` has a device name, the returned path will have the same device name as `other`. Otherwise, the returned path will have the same device name as `self`. If neither has a device name, the returned path will not have a device name as well.</span>
+</span><span id="GPath-931"><a href="#GPath-931"><span class="linenos"> 931</span></a><span class="sd">			If `other` has a drive, the returned path will have the same drive as `other`. Otherwise, the returned path will have the same drive as `self`. If neither has a drive, the returned path will not have a drive as well.</span>
 </span><span id="GPath-932"><a href="#GPath-932"><span class="linenos"> 932</span></a>
 </span><span id="GPath-933"><a href="#GPath-933"><span class="linenos"> 933</span></a><span class="sd">			Alias: `__truediv__()`</span>
 </span><span id="GPath-934"><a href="#GPath-934"><span class="linenos"> 934</span></a>
 </span><span id="GPath-935"><a href="#GPath-935"><span class="linenos"> 935</span></a><span class="sd">			Usage: &lt;code&gt;&lt;var&gt;self&lt;/var&gt; + &lt;var&gt;other&lt;/var&gt;&lt;/code&gt; or &lt;code&gt;&lt;var&gt;self&lt;/var&gt; / &lt;var&gt;other&lt;/var&gt;&lt;/code&gt;</span>
 </span><span id="GPath-936"><a href="#GPath-936"><span class="linenos"> 936</span></a>
 </span><span id="GPath-937"><a href="#GPath-937"><span class="linenos"> 937</span></a><span class="sd">			Raises `ValueError` if either GPath is invalid</span>
 </span><span id="GPath-938"><a href="#GPath-938"><span class="linenos"> 938</span></a>
@@ -1327,31 +1327,31 @@
 			
 
 					<h2>Instance variables summary</h2>
 		<dl>
 				<dt><span class="name"><a href="#GPath.named_parts">named_parts</a></span><span class="annotation">: list[str]</span></dt>
 
 <dd>
-<p>Read-only named components of the path, not including the filesystem root, device name, or any parent directories</p></dd>
+<p>Read-only named components of the path, not including the filesystem root, drive name, or any parent directories</p></dd>
 	<dt><span class="name"><a href="#GPath.parent_level">parent_level</a></span><span class="annotation">: int</span></dt>
 
 <dd>
 <p>Read-only number of levels of parent directories that the path is relative to, which may be 0</p></dd>
 	<dt><span class="name"><a href="#GPath.parent_parts">parent_parts</a></span><span class="annotation">: list[str]</span></dt>
 
 <dd>
 <p>Read-only path components representing a parent directory that it is relative to, if any, with a copy of <code>parent_indicator</code> for each level of parent directory</p></dd>
 	<dt><span class="name"><a href="#GPath.relative_parts">relative_parts</a></span><span class="annotation">: list[str]</span></dt>
 
 <dd>
-<p>Read-only relative components of the path, not including the filesystem root or device name, with a copy of <code>parent_indicator</code> for each level of parent directory</p></dd>
+<p>Read-only relative components of the path, not including the filesystem root or drive name, with a copy of <code>parent_indicator</code> for each level of parent directory</p></dd>
 	<dt><span class="name"><a href="#GPath.drive">drive</a></span><span class="annotation">: str</span></dt>
 
 <dd>
-<p>Read-only device name</p></dd>
+<p>Read-only drive name</p></dd>
 	<dt><span class="name"><a href="#GPath.absolute">absolute</a></span><span class="annotation">: bool</span></dt>
 
 <dd>
 <p>Read-only flag for whether the path is an absolute path</p></dd>
 	<dt><span class="name"><a href="#GPath.root">root</a></span><span class="annotation">: bool</span></dt>
 
 <dd>
@@ -1429,23 +1429,23 @@
 	<dt>					<span class="name"><a href="#GPath.__repr__">__repr__</a></span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span></dt>
 
 <dd>
 <p>Return a string that, when printed, gives the Python code associated with instantiating the GPath object.</p></dd>
 	<dt>					<span class="name"><a href="#GPath.__len__">__len__</a></span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">) -> <span class="nb">int</span>:</span></span></dt>
 
 <dd>
-<p>Get the number of named path components, excluding any device name or parent directories.</p></dd>
+<p>Get the number of named path components, excluding any drive name or parent directories.</p></dd>
 	<dt>					<span class="name"><a href="#GPath.__getitem__">__getitem__</a></span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">index</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="nb">int</span><span class="p">,</span> <span class="nb">slice</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span>:</span></span></dt>
 
 <dd>
-<p>Get a 0-indexed named path component, or a slice of path components, excluding any device name or parent directories.</p></dd>
+<p>Get a 0-indexed named path component, or a slice of path components, excluding any drive name or parent directories.</p></dd>
 	<dt>					<span class="name"><a href="#GPath.__iter__">__iter__</a></span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">) -> <span class="n">Iterator</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>:</span></span></dt>
 
 <dd>
-<p>Get an iterator through the named path components, excluding any device name or parent directories.</p></dd>
+<p>Get an iterator through the named path components, excluding any drive name or parent directories.</p></dd>
 	<dt>					<span class="name"><a href="#GPath.__contains__">__contains__</a></span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">other</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="n"><a href="#GPath">GPath</a></span><span class="p">,</span> <span class="nb">str</span><span class="p">,</span> <span class="nb">bytes</span><span class="p">,</span> <span class="n">os</span><span class="o">.</span><span class="n">PathLike</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span></dt>
 
 <dd>
 <p>Check if the path represented by <code>self</code> contains the path represented by <code>other</code>; i.e. check if <code>self</code> is a parent directory of <code>other</code>.</p></dd>
 	<dt>					<span class="name"><a href="#GPath.__add__">__add__</a></span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">other</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="n"><a href="#GPath">GPath</a></span><span class="p">,</span> <span class="nb">str</span><span class="p">,</span> <span class="nb">bytes</span><span class="p">,</span> <span class="n">os</span><span class="o">.</span><span class="n">PathLike</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="n"><a href="#GPath">GPath</a></span>:</span></span></dt>
 
 <dd>
@@ -1544,27 +1544,27 @@
 </span><span id="GPath.__init__-155"><a href="#GPath.__init__-155"><span class="linenos">155</span></a>			<span class="k">else</span><span class="p">:</span>
 </span><span id="GPath.__init__-156"><a href="#GPath.__init__-156"><span class="linenos">156</span></a>				<span class="n">path</span> <span class="o">=</span> <span class="n">path</span><span class="o">.</span><span class="n">decode</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_encoding</span><span class="p">)</span>
 </span><span id="GPath.__init__-157"><a href="#GPath.__init__-157"><span class="linenos">157</span></a>
 </span><span id="GPath.__init__-158"><a href="#GPath.__init__-158"><span class="linenos">158</span></a>		<span class="c1"># path is a str</span>
 </span><span id="GPath.__init__-159"><a href="#GPath.__init__-159"><span class="linenos">159</span></a>
 </span><span id="GPath.__init__-160"><a href="#GPath.__init__-160"><span class="linenos">160</span></a>		<span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">path</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="mi">2</span> <span class="ow">and</span> <span class="n">path</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span> <span class="ow">in</span> <span class="n">_rules</span><span class="o">.</span><span class="n">generic_rules</span><span class="o">.</span><span class="n">drive_postfixes</span><span class="p">:</span>
 </span><span id="GPath.__init__-161"><a href="#GPath.__init__-161"><span class="linenos">161</span></a>			<span class="bp">self</span><span class="o">.</span><span class="n">_drive</span> <span class="o">=</span> <span class="n">path</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="GPath.__init__-162"><a href="#GPath.__init__-162"><span class="linenos">162</span></a>			<span class="n">deviceless_path</span> <span class="o">=</span> <span class="n">path</span><span class="p">[</span><span class="mi">2</span><span class="p">:]</span>
+</span><span id="GPath.__init__-162"><a href="#GPath.__init__-162"><span class="linenos">162</span></a>			<span class="n">driveless_path</span> <span class="o">=</span> <span class="n">path</span><span class="p">[</span><span class="mi">2</span><span class="p">:]</span>
 </span><span id="GPath.__init__-163"><a href="#GPath.__init__-163"><span class="linenos">163</span></a>		<span class="k">else</span><span class="p">:</span>
-</span><span id="GPath.__init__-164"><a href="#GPath.__init__-164"><span class="linenos">164</span></a>			<span class="n">deviceless_path</span> <span class="o">=</span> <span class="n">path</span>
+</span><span id="GPath.__init__-164"><a href="#GPath.__init__-164"><span class="linenos">164</span></a>			<span class="n">driveless_path</span> <span class="o">=</span> <span class="n">path</span>
 </span><span id="GPath.__init__-165"><a href="#GPath.__init__-165"><span class="linenos">165</span></a>
 </span><span id="GPath.__init__-166"><a href="#GPath.__init__-166"><span class="linenos">166</span></a>		<span class="k">for</span> <span class="n">root</span> <span class="ow">in</span> <span class="n">_rules</span><span class="o">.</span><span class="n">generic_rules</span><span class="o">.</span><span class="n">roots</span><span class="p">:</span>
-</span><span id="GPath.__init__-167"><a href="#GPath.__init__-167"><span class="linenos">167</span></a>			<span class="k">if</span> <span class="n">deviceless_path</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="n">root</span><span class="p">):</span>
+</span><span id="GPath.__init__-167"><a href="#GPath.__init__-167"><span class="linenos">167</span></a>			<span class="k">if</span> <span class="n">driveless_path</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="n">root</span><span class="p">):</span>
 </span><span id="GPath.__init__-168"><a href="#GPath.__init__-168"><span class="linenos">168</span></a>				<span class="bp">self</span><span class="o">.</span><span class="n">_root</span> <span class="o">=</span> <span class="kc">True</span>
 </span><span id="GPath.__init__-169"><a href="#GPath.__init__-169"><span class="linenos">169</span></a>				<span class="k">break</span>
 </span><span id="GPath.__init__-170"><a href="#GPath.__init__-170"><span class="linenos">170</span></a>
 </span><span id="GPath.__init__-171"><a href="#GPath.__init__-171"><span class="linenos">171</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_root</span><span class="p">:</span>
-</span><span id="GPath.__init__-172"><a href="#GPath.__init__-172"><span class="linenos">172</span></a>			<span class="n">rootless_path</span> <span class="o">=</span> <span class="n">deviceless_path</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
+</span><span id="GPath.__init__-172"><a href="#GPath.__init__-172"><span class="linenos">172</span></a>			<span class="n">rootless_path</span> <span class="o">=</span> <span class="n">driveless_path</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
 </span><span id="GPath.__init__-173"><a href="#GPath.__init__-173"><span class="linenos">173</span></a>		<span class="k">else</span><span class="p">:</span>
-</span><span id="GPath.__init__-174"><a href="#GPath.__init__-174"><span class="linenos">174</span></a>			<span class="n">rootless_path</span> <span class="o">=</span> <span class="n">deviceless_path</span>
+</span><span id="GPath.__init__-174"><a href="#GPath.__init__-174"><span class="linenos">174</span></a>			<span class="n">rootless_path</span> <span class="o">=</span> <span class="n">driveless_path</span>
 </span><span id="GPath.__init__-175"><a href="#GPath.__init__-175"><span class="linenos">175</span></a>
 </span><span id="GPath.__init__-176"><a href="#GPath.__init__-176"><span class="linenos">176</span></a>
 </span><span id="GPath.__init__-177"><a href="#GPath.__init__-177"><span class="linenos">177</span></a>		<span class="n">parts</span> <span class="o">=</span> <span class="n">_split_relative</span><span class="p">(</span><span class="n">rootless_path</span><span class="p">,</span> <span class="n">delimiters</span><span class="o">=</span><span class="p">(</span><span class="nb">set</span><span class="p">(</span><span class="n">_rules</span><span class="o">.</span><span class="n">generic_rules</span><span class="o">.</span><span class="n">separators</span><span class="p">)</span> <span class="o">|</span> <span class="nb">set</span><span class="p">(</span><span class="n">_rules</span><span class="o">.</span><span class="n">generic_rules</span><span class="o">.</span><span class="n">separators</span><span class="p">)))</span>
 </span><span id="GPath.__init__-178"><a href="#GPath.__init__-178"><span class="linenos">178</span></a>		<span class="n">parts</span> <span class="o">=</span> <span class="n">_normalise_relative</span><span class="p">(</span><span class="n">parts</span><span class="p">)</span>
 </span><span id="GPath.__init__-179"><a href="#GPath.__init__-179"><span class="linenos">179</span></a>		<span class="n">parent_level</span> <span class="o">=</span> <span class="mi">0</span>
 </span><span id="GPath.__init__-180"><a href="#GPath.__init__-180"><span class="linenos">180</span></a>		<span class="k">while</span> <span class="n">parent_level</span> <span class="o">&lt;</span> <span class="nb">len</span><span class="p">(</span><span class="n">parts</span><span class="p">)</span> <span class="ow">and</span> <span class="n">parts</span><span class="p">[</span><span class="n">parent_level</span><span class="p">]</span> <span class="ow">in</span> <span class="n">_rules</span><span class="o">.</span><span class="n">generic_rules</span><span class="o">.</span><span class="n">parent_indicators</span><span class="p">:</span>
 </span><span id="GPath.__init__-181"><a href="#GPath.__init__-181"><span class="linenos">181</span></a>			<span class="n">parent_level</span> <span class="o">+=</span> <span class="mi">1</span>
@@ -1607,15 +1607,15 @@
 
 
         
     </div>
     <a class="headerlink" href="#GPath.named_parts"></a>
     
     <div class="docstring">
-<p>Read-only named components of the path, not including the filesystem root, device name, or any parent directories</p>
+<p>Read-only named components of the path, not including the filesystem root, drive name, or any parent directories</p>
 
 <h2 id="examples">Examples</h2>
 
 <div class="pdoc-code codehilite">
 <pre><span></span><code><span class="n">GPath</span><span class="p">(</span><span class="s2">&quot;usr/local/bin&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">named_parts</span>     <span class="c1"># [&quot;usr&quot;, &quot;local&quot;, &quot;bin&quot;]</span>
 <span class="n">GPath</span><span class="p">(</span><span class="s2">&quot;../../Documents&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">named_parts</span>   <span class="c1"># [&quot;Documents&quot;]</span>
 <span class="n">GPath</span><span class="p">(</span><span class="s2">&quot;/usr/bin&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">named_parts</span>          <span class="c1"># [&quot;usr&quot;, &quot;bin&quot;]</span>
@@ -1678,15 +1678,15 @@
 
 
         
     </div>
     <a class="headerlink" href="#GPath.relative_parts"></a>
     
     <div class="docstring">
-<p>Read-only relative components of the path, not including the filesystem root or device name, with a copy of <code>parent_indicator</code> for each level of parent directory</p>
+<p>Read-only relative components of the path, not including the filesystem root or drive name, with a copy of <code>parent_indicator</code> for each level of parent directory</p>
 
 <h2 id="examples">Examples</h2>
 
 <div class="pdoc-code codehilite">
 <pre><span></span><code><span class="n">GPath</span><span class="p">(</span><span class="s2">&quot;usr/local/bin&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">relative_parts</span>     <span class="c1"># [&quot;usr&quot;, &quot;local&quot;, &quot;bin&quot;]</span>
 <span class="n">GPath</span><span class="p">(</span><span class="s2">&quot;../../Documents&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">relative_parts</span>   <span class="c1"># [&quot;..&quot;, &quot;..&quot;, &quot;Documents&quot;]</span>
 <span class="n">GPath</span><span class="p">(</span><span class="s2">&quot;/usr/bin&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">relative_parts</span>          <span class="c1"># [&quot;usr&quot;, &quot;bin&quot;]</span>
@@ -1703,22 +1703,22 @@
 
 
         
     </div>
     <a class="headerlink" href="#GPath.drive"></a>
     
     <div class="docstring">
-<p>Read-only device name</p>
+<p>Read-only drive name</p>
 
 <h2 id="examples">Examples</h2>
 
 <div class="pdoc-code codehilite">
-<pre><span></span><code><span class="n">GPath</span><span class="p">(</span><span class="s2">&quot;C:/Windows&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">device</span>       <span class="c1"># &quot;C:&quot;</span>
-<span class="n">GPath</span><span class="p">(</span><span class="s2">&quot;/usr/bin&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">device</span>         <span class="c1"># &quot;&quot;</span>
-<span class="n">GPath</span><span class="p">(</span><span class="s2">&quot;../../Documents&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">device</span>  <span class="c1"># &quot;&quot;</span>
+<pre><span></span><code><span class="n">GPath</span><span class="p">(</span><span class="s2">&quot;C:/Windows&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">drive</span>       <span class="c1"># &quot;C:&quot;</span>
+<span class="n">GPath</span><span class="p">(</span><span class="s2">&quot;/usr/bin&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">drive</span>         <span class="c1"># &quot;&quot;</span>
+<span class="n">GPath</span><span class="p">(</span><span class="s2">&quot;../../Documents&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">drive</span>  <span class="c1"># &quot;&quot;</span>
 </code></pre>
 </div></div>
 
 
 
                             </div>
                             <div id="GPath.absolute" class="classattr">
@@ -2305,15 +2305,15 @@
 
     </div>
     <a class="headerlink" href="#GPath.common_with"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="GPath.common_with-569"><a href="#GPath.common_with-569"><span class="linenos">569</span></a>	<span class="k">def</span> <span class="nf">common_with</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">other</span><span class="p">:</span> <span class="n">GPathLike</span><span class="p">,</span> <span class="n">allow_current</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_parents</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Optional</span><span class="p">[</span><span class="n">GPath</span><span class="p">]:</span>
 </span><span id="GPath.common_with-570"><a href="#GPath.common_with-570"><span class="linenos">570</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
 </span><span id="GPath.common_with-571"><a href="#GPath.common_with-571"><span class="linenos">571</span></a><span class="sd">			Find the longest common base path shared between `self` and `other`, or return None if no such path exists.</span>
 </span><span id="GPath.common_with-572"><a href="#GPath.common_with-572"><span class="linenos">572</span></a>
-</span><span id="GPath.common_with-573"><a href="#GPath.common_with-573"><span class="linenos">573</span></a><span class="sd">			A common base path might not exist if one path is an absolute path while the other is a relative path, or if the two paths are in different filesystems (with different device names), or in other cases as controlled by the `allow_current` and `allow_parents` options.</span>
+</span><span id="GPath.common_with-573"><a href="#GPath.common_with-573"><span class="linenos">573</span></a><span class="sd">			A common base path might not exist if one path is an absolute path while the other is a relative path, or if the two paths are in different filesystems (with different drive names), or in other cases as controlled by the `allow_current` and `allow_parents` options.</span>
 </span><span id="GPath.common_with-574"><a href="#GPath.common_with-574"><span class="linenos">574</span></a>
 </span><span id="GPath.common_with-575"><a href="#GPath.common_with-575"><span class="linenos">575</span></a><span class="sd">			If using the default options of `allow_current=True` and `allow_parent=False`, the binary operator for bitwise-and can be used: `__and__()` (usage: &lt;code&gt;&lt;var&gt;g1&lt;/var&gt; &amp; &lt;var&gt;g2&lt;/var&gt;&lt;/code&gt;).</span>
 </span><span id="GPath.common_with-576"><a href="#GPath.common_with-576"><span class="linenos">576</span></a>
 </span><span id="GPath.common_with-577"><a href="#GPath.common_with-577"><span class="linenos">577</span></a><span class="sd">			Parameters</span>
 </span><span id="GPath.common_with-578"><a href="#GPath.common_with-578"><span class="linenos">578</span></a><span class="sd">			----------</span>
 </span><span id="GPath.common_with-579"><a href="#GPath.common_with-579"><span class="linenos">579</span></a><span class="sd">			`other`</span>
 </span><span id="GPath.common_with-580"><a href="#GPath.common_with-580"><span class="linenos">580</span></a><span class="sd">			: the path to compare with</span>
@@ -2385,15 +2385,15 @@
 </span><span id="GPath.common_with-646"><a href="#GPath.common_with-646"><span class="linenos">646</span></a>		<span class="k">return</span> <span class="n">common_path</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Find the longest common base path shared between <code>self</code> and <code>other</code>, or return None if no such path exists.</p>
 
-<p>A common base path might not exist if one path is an absolute path while the other is a relative path, or if the two paths are in different filesystems (with different device names), or in other cases as controlled by the <code>allow_current</code> and <code>allow_parents</code> options.</p>
+<p>A common base path might not exist if one path is an absolute path while the other is a relative path, or if the two paths are in different filesystems (with different drive names), or in other cases as controlled by the <code>allow_current</code> and <code>allow_parents</code> options.</p>
 
 <p>If using the default options of <code>allow_current=True</code> and <code>allow_parent=False</code>, the binary operator for bitwise-and can be used: <code><a href="#GPath.__and__">__and__()</a></code> (usage: <code><var>g1</var> &amp; <var>g2</var></code>).</p>
 
 <h2 id="parameters">Parameters</h2>
 
 <p><code>other</code>
 : the path to compare with</p>
@@ -2866,15 +2866,15 @@
 
                 <label class="view-source-button" for="GPath.__len__-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GPath.__len__"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="GPath.__len__-853"><a href="#GPath.__len__-853"><span class="linenos">853</span></a>	<span class="k">def</span> <span class="fm">__len__</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
 </span><span id="GPath.__len__-854"><a href="#GPath.__len__-854"><span class="linenos">854</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="GPath.__len__-855"><a href="#GPath.__len__-855"><span class="linenos">855</span></a><span class="sd">			Get the number of named path components, excluding any device name or parent directories.</span>
+</span><span id="GPath.__len__-855"><a href="#GPath.__len__-855"><span class="linenos">855</span></a><span class="sd">			Get the number of named path components, excluding any drive name or parent directories.</span>
 </span><span id="GPath.__len__-856"><a href="#GPath.__len__-856"><span class="linenos">856</span></a>
 </span><span id="GPath.__len__-857"><a href="#GPath.__len__-857"><span class="linenos">857</span></a><span class="sd">			Usage: &lt;code&gt;len(&lt;var&gt;g&lt;/var&gt;)&lt;/code&gt;</span>
 </span><span id="GPath.__len__-858"><a href="#GPath.__len__-858"><span class="linenos">858</span></a>
 </span><span id="GPath.__len__-859"><a href="#GPath.__len__-859"><span class="linenos">859</span></a><span class="sd">			Examples</span>
 </span><span id="GPath.__len__-860"><a href="#GPath.__len__-860"><span class="linenos">860</span></a><span class="sd">			--------</span>
 </span><span id="GPath.__len__-861"><a href="#GPath.__len__-861"><span class="linenos">861</span></a><span class="sd">			```python</span>
 </span><span id="GPath.__len__-862"><a href="#GPath.__len__-862"><span class="linenos">862</span></a><span class="sd">			len(GPath(&quot;/usr/bin&quot;))    # 2</span>
@@ -2884,15 +2884,15 @@
 </span><span id="GPath.__len__-866"><a href="#GPath.__len__-866"><span class="linenos">866</span></a><span class="sd">			```</span>
 </span><span id="GPath.__len__-867"><a href="#GPath.__len__-867"><span class="linenos">867</span></a><span class="sd">		&quot;&quot;&quot;</span>
 </span><span id="GPath.__len__-868"><a href="#GPath.__len__-868"><span class="linenos">868</span></a>		<span class="k">return</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_parts</span><span class="p">)</span>
 </span></pre></div>
 
 
     <div class="docstring">
-<p>Get the number of named path components, excluding any device name or parent directories.</p>
+<p>Get the number of named path components, excluding any drive name or parent directories.</p>
 
 <p>Usage: <code>len(<var>g</var>)</code></p>
 
 <h2 id="examples">Examples</h2>
 
 <div class="pdoc-code codehilite">
 <pre><span></span><code><span class="nb">len</span><span class="p">(</span><span class="n">GPath</span><span class="p">(</span><span class="s2">&quot;/usr/bin&quot;</span><span class="p">))</span>    <span class="c1"># 2</span>
@@ -2915,15 +2915,15 @@
 
                 <label class="view-source-button" for="GPath.__getitem__-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GPath.__getitem__"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="GPath.__getitem__-871"><a href="#GPath.__getitem__-871"><span class="linenos">871</span></a>	<span class="k">def</span> <span class="fm">__getitem__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">index</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="nb">int</span><span class="p">,</span> <span class="nb">slice</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]]:</span>
 </span><span id="GPath.__getitem__-872"><a href="#GPath.__getitem__-872"><span class="linenos">872</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="GPath.__getitem__-873"><a href="#GPath.__getitem__-873"><span class="linenos">873</span></a><span class="sd">			Get a 0-indexed named path component, or a slice of path components, excluding any device name or parent directories.</span>
+</span><span id="GPath.__getitem__-873"><a href="#GPath.__getitem__-873"><span class="linenos">873</span></a><span class="sd">			Get a 0-indexed named path component, or a slice of path components, excluding any drive name or parent directories.</span>
 </span><span id="GPath.__getitem__-874"><a href="#GPath.__getitem__-874"><span class="linenos">874</span></a>
 </span><span id="GPath.__getitem__-875"><a href="#GPath.__getitem__-875"><span class="linenos">875</span></a><span class="sd">			Usage: &lt;code&gt;&lt;var&gt;g&lt;/var&gt;[&lt;var&gt;n&lt;/var&gt;]&lt;/code&gt;, &lt;code&gt;&lt;var&gt;g&lt;/var&gt;[&lt;var&gt;start&lt;/var&gt;:&lt;var&gt;end&lt;/var&gt;]&lt;/code&gt;, &lt;code&gt;&lt;var&gt;g&lt;/var&gt;[&lt;var&gt;start&lt;/var&gt;:&lt;var&gt;end&lt;/var&gt;:&lt;var&gt;step&lt;/var&gt;]&lt;/code&gt;, etc.</span>
 </span><span id="GPath.__getitem__-876"><a href="#GPath.__getitem__-876"><span class="linenos">876</span></a>
 </span><span id="GPath.__getitem__-877"><a href="#GPath.__getitem__-877"><span class="linenos">877</span></a><span class="sd">			Examples</span>
 </span><span id="GPath.__getitem__-878"><a href="#GPath.__getitem__-878"><span class="linenos">878</span></a><span class="sd">			--------</span>
 </span><span id="GPath.__getitem__-879"><a href="#GPath.__getitem__-879"><span class="linenos">879</span></a><span class="sd">			```python</span>
 </span><span id="GPath.__getitem__-880"><a href="#GPath.__getitem__-880"><span class="linenos">880</span></a><span class="sd">			GPath(&quot;/usr/local/bin&quot;)[1]    # &quot;local&quot;</span>
@@ -2936,15 +2936,15 @@
 </span><span id="GPath.__getitem__-887"><a href="#GPath.__getitem__-887"><span class="linenos">887</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_parts</span><span class="p">[</span><span class="n">index</span><span class="p">]</span>
 </span><span id="GPath.__getitem__-888"><a href="#GPath.__getitem__-888"><span class="linenos">888</span></a>		<span class="k">elif</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">index</span><span class="p">,</span> <span class="nb">slice</span><span class="p">):</span>
 </span><span id="GPath.__getitem__-889"><a href="#GPath.__getitem__-889"><span class="linenos">889</span></a>			<span class="k">return</span> <span class="nb">list</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_parts</span><span class="p">[</span><span class="n">index</span><span class="p">])</span>
 </span></pre></div>
 
 
     <div class="docstring">
-<p>Get a 0-indexed named path component, or a slice of path components, excluding any device name or parent directories.</p>
+<p>Get a 0-indexed named path component, or a slice of path components, excluding any drive name or parent directories.</p>
 
 <p>Usage: <code><var>g</var>[<var>n</var>]</code>, <code><var>g</var>[<var>start</var>:<var>end</var>]</code>, <code><var>g</var>[<var>start</var>:<var>end</var>:<var>step</var>]</code>, etc.</p>
 
 <h2 id="examples">Examples</h2>
 
 <div class="pdoc-code codehilite">
 <pre><span></span><code><span class="n">GPath</span><span class="p">(</span><span class="s2">&quot;/usr/local/bin&quot;</span><span class="p">)[</span><span class="mi">1</span><span class="p">]</span>    <span class="c1"># &quot;local&quot;</span>
@@ -2967,24 +2967,24 @@
 
                 <label class="view-source-button" for="GPath.__iter__-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GPath.__iter__"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="GPath.__iter__-892"><a href="#GPath.__iter__-892"><span class="linenos">892</span></a>	<span class="k">def</span> <span class="fm">__iter__</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Iterator</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
 </span><span id="GPath.__iter__-893"><a href="#GPath.__iter__-893"><span class="linenos">893</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="GPath.__iter__-894"><a href="#GPath.__iter__-894"><span class="linenos">894</span></a><span class="sd">			Get an iterator through the named path components, excluding any device name or parent directories.</span>
+</span><span id="GPath.__iter__-894"><a href="#GPath.__iter__-894"><span class="linenos">894</span></a><span class="sd">			Get an iterator through the named path components, excluding any drive name or parent directories.</span>
 </span><span id="GPath.__iter__-895"><a href="#GPath.__iter__-895"><span class="linenos">895</span></a>
 </span><span id="GPath.__iter__-896"><a href="#GPath.__iter__-896"><span class="linenos">896</span></a><span class="sd">			Usage: &lt;code&gt;iter(&lt;var&gt;g&lt;/var&gt;)&lt;/code&gt; or &lt;code&gt;for &lt;var&gt;p&lt;/var&gt; in &lt;var&gt;g&lt;/var&gt;:&lt;/code&gt;</span>
 </span><span id="GPath.__iter__-897"><a href="#GPath.__iter__-897"><span class="linenos">897</span></a><span class="sd">		&quot;&quot;&quot;</span>
 </span><span id="GPath.__iter__-898"><a href="#GPath.__iter__-898"><span class="linenos">898</span></a>		<span class="k">return</span> <span class="nb">iter</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_parts</span><span class="p">)</span>
 </span></pre></div>
 
 
     <div class="docstring">
-<p>Get an iterator through the named path components, excluding any device name or parent directories.</p>
+<p>Get an iterator through the named path components, excluding any drive name or parent directories.</p>
 
 <p>Usage: <code>iter(<var>g</var>)</code> or <code>for <var>p</var> in <var>g</var>:</code></p></div>
 
 
 
                             </div>
                             <div id="GPath.__contains__" class="classattr">
@@ -3056,17 +3056,17 @@
 
     </div>
     <a class="headerlink" href="#GPath.__add__"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="GPath.__add__-925"><a href="#GPath.__add__-925"><span class="linenos">925</span></a>	<span class="k">def</span> <span class="fm">__add__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">other</span><span class="p">:</span> <span class="n">GPathLike</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">GPath</span><span class="p">:</span>
 </span><span id="GPath.__add__-926"><a href="#GPath.__add__-926"><span class="linenos">926</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
 </span><span id="GPath.__add__-927"><a href="#GPath.__add__-927"><span class="linenos">927</span></a><span class="sd">			Add (concatenate) `other` to the end of `self`, and return a new copy.</span>
 </span><span id="GPath.__add__-928"><a href="#GPath.__add__-928"><span class="linenos">928</span></a>
-</span><span id="GPath.__add__-929"><a href="#GPath.__add__-929"><span class="linenos">929</span></a><span class="sd">			If `other` is an absolute path, the returned path will be an absolute path that matches `other`, apart from the device name.</span>
+</span><span id="GPath.__add__-929"><a href="#GPath.__add__-929"><span class="linenos">929</span></a><span class="sd">			If `other` is an absolute path, the returned path will be an absolute path that matches `other`, apart from the drive name.</span>
 </span><span id="GPath.__add__-930"><a href="#GPath.__add__-930"><span class="linenos">930</span></a>
-</span><span id="GPath.__add__-931"><a href="#GPath.__add__-931"><span class="linenos">931</span></a><span class="sd">			If `other` has a device name, the returned path will have the same device name as `other`. Otherwise, the returned path will have the same device name as `self`. If neither has a device name, the returned path will not have a device name as well.</span>
+</span><span id="GPath.__add__-931"><a href="#GPath.__add__-931"><span class="linenos">931</span></a><span class="sd">			If `other` has a drive, the returned path will have the same drive as `other`. Otherwise, the returned path will have the same drive as `self`. If neither has a drive, the returned path will not have a drive as well.</span>
 </span><span id="GPath.__add__-932"><a href="#GPath.__add__-932"><span class="linenos">932</span></a>
 </span><span id="GPath.__add__-933"><a href="#GPath.__add__-933"><span class="linenos">933</span></a><span class="sd">			Alias: `__truediv__()`</span>
 </span><span id="GPath.__add__-934"><a href="#GPath.__add__-934"><span class="linenos">934</span></a>
 </span><span id="GPath.__add__-935"><a href="#GPath.__add__-935"><span class="linenos">935</span></a><span class="sd">			Usage: &lt;code&gt;&lt;var&gt;self&lt;/var&gt; + &lt;var&gt;other&lt;/var&gt;&lt;/code&gt; or &lt;code&gt;&lt;var&gt;self&lt;/var&gt; / &lt;var&gt;other&lt;/var&gt;&lt;/code&gt;</span>
 </span><span id="GPath.__add__-936"><a href="#GPath.__add__-936"><span class="linenos">936</span></a>
 </span><span id="GPath.__add__-937"><a href="#GPath.__add__-937"><span class="linenos">937</span></a><span class="sd">			Raises `ValueError` if either GPath is invalid</span>
 </span><span id="GPath.__add__-938"><a href="#GPath.__add__-938"><span class="linenos">938</span></a>
@@ -3109,17 +3109,17 @@
 </span><span id="GPath.__add__-975"><a href="#GPath.__add__-975"><span class="linenos">975</span></a>		<span class="k">return</span> <span class="n">new_path</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Add (concatenate) <code>other</code> to the end of <code>self</code>, and return a new copy.</p>
 
-<p>If <code>other</code> is an absolute path, the returned path will be an absolute path that matches <code>other</code>, apart from the device name.</p>
+<p>If <code>other</code> is an absolute path, the returned path will be an absolute path that matches <code>other</code>, apart from the drive name.</p>
 
-<p>If <code>other</code> has a device name, the returned path will have the same device name as <code>other</code>. Otherwise, the returned path will have the same device name as <code>self</code>. If neither has a device name, the returned path will not have a device name as well.</p>
+<p>If <code>other</code> has a drive, the returned path will have the same drive as <code>other</code>. Otherwise, the returned path will have the same drive as <code>self</code>. If neither has a drive, the returned path will not have a drive as well.</p>
 
 <p>Alias: <code><a href="#GPath.__truediv__">__truediv__()</a></code></p>
 
 <p>Usage: <code><var>self</var> + <var>other</var></code> or <code><var>self</var> / <var>other</var></code></p>
 
 <p>Raises <code>ValueError</code> if either GPath is invalid</p>
```

#### html2text {}

```diff
@@ -38,15 +38,15 @@
           o __lshift__()
           o __rshift__()
     * GPathLike
 built_with_pdoc[pdoc_logo]
    Edit_on_GitHub
 ****** gpath ******
 ⁰ View Source
-1__version__ = '0.4.dev3'
+1__version__ = '0.4.1'
 2
 3from ._gpath import GPath, GPathLike
 4
 5__all__ = ('GPath', 'GPathLike')
   ⁰
 class GPath(Hashable, Sized, Iterable): View Source
 __85class GPath(Hashable, Sized, Iterable):
@@ -198,37 +198,37 @@
 # path is a str
 _159
 _160
 if len(path) >= 2 and path[1] in _rules.generic_rules.drive_postfixes:
 _161
 self._drive = path[0]
 _162
-deviceless_path = path[2:]
+driveless_path = path[2:]
 _163
 else:
 _164
-deviceless_path = path
+driveless_path = path
 _165
 _166
 for root in _rules.generic_rules.roots:
 _167
-if deviceless_path.startswith(root):
+if driveless_path.startswith(root):
 _168
 self._root = True
 _169
 break
 _170
 _171
 if self._root:
 _172
-rootless_path = deviceless_path[1:]
+rootless_path = driveless_path[1:]
 _173
 else:
 _174
-rootless_path = deviceless_path
+rootless_path = driveless_path
 _175
 _176
 _177
 parts = _split_relative(rootless_path, delimiters=(set
 (_rules.generic_rules.separators) | set(_rules.generic_rules.separators)))
 _178
 parts = _normalise_relative(parts)
@@ -251,15 +251,15 @@
 @property
 _188
 def named_parts(self) -> list[str]:
 _189
 """
 _190
 Read-only named components of the path, not including the filesystem root,
-device name, or any parent directories
+drive name, or any parent directories
 _191
 _192
 Examples
 _193
 --------
 _194
 ```python
@@ -338,15 +338,15 @@
 @property
 _232
 def relative_parts(self) -> list[str]:
 _233
 """
 _234
 Read-only relative components of the path, not including the filesystem root or
-device name, with a copy of `parent_indicator` for each level of parent
+drive name, with a copy of `parent_indicator` for each level of parent
 directory
 _235
 _236
 Examples
 _237
 --------
 _238
@@ -369,28 +369,28 @@
 _247
 @property
 _248
 def drive(self) -> str:
 _249
 """
 _250
-Read-only device name
+Read-only drive name
 _251
 _252
 Examples
 _253
 --------
 _254
 ```python
 _255
-GPath("C:/Windows").device       # "C:"
+GPath("C:/Windows").drive       # "C:"
 _256
-GPath("/usr/bin").device         # ""
+GPath("/usr/bin").drive         # ""
 _257
-GPath("../../Documents").device  # ""
+GPath("../../Documents").drive  # ""
 _258
 ```
 _259
 """
 _260
 return self._drive
 _261
@@ -999,15 +999,15 @@
 _571
 Find the longest common base path shared between `self` and `other`, or return
 None if no such path exists.
 _572
 _573
 A common base path might not exist if one path is an absolute path while the
 other is a relative path, or if the two paths are in different filesystems
-(with different device names), or in other cases as controlled by the
+(with different drive names), or in other cases as controlled by the
 `allow_current` and `allow_parents` options.
 _574
 _575
 If using the default options of `allow_current=True` and `allow_parent=False`,
 the binary operator for bitwise-and can be used: `__and__()` (usage:
 <code><var>g1</var> & <var>g2</var></code>).
 _576
@@ -1537,15 +1537,15 @@
 _851
 _852
 _853
 def __len__(self) -> int:
 _854
 """
 _855
-Get the number of named path components, excluding any device name or parent
+Get the number of named path components, excluding any drive name or parent
 directories.
 _856
 _857
 Usage: <code>len(<var>g</var>)</code>
 _858
 _859
 Examples
@@ -1571,15 +1571,15 @@
 _870
 _871
 def __getitem__(self, index: Union[int, slice]) -> Union[str, list[str]]:
 _872
 """
 _873
 Get a 0-indexed named path component, or a slice of path components, excluding
-any device name or parent directories.
+any drive name or parent directories.
 _874
 _875
 Usage: <code><var>g</var>[<var>n</var>]</code>, <code><var>g</var>[<var>start</
 var>:<var>end</var>]</code>, <code><var>g</var>[<var>start</var>:<var>end</
 var>:<var>step</var>]</code>, etc.
 _876
 _877
@@ -1611,15 +1611,15 @@
 _890
 _891
 _892
 def __iter__(self) -> Iterator[str]:
 _893
 """
 _894
-Get an iterator through the named path components, excluding any device name or
+Get an iterator through the named path components, excluding any drive name or
 parent directories.
 _895
 _896
 Usage: <code>iter(<var>g</var>)</code> or <code>for <var>p</var> in <var>g</
 var>:</code>
 _897
 """
@@ -1675,21 +1675,20 @@
 _926
 """
 _927
 Add (concatenate) `other` to the end of `self`, and return a new copy.
 _928
 _929
 If `other` is an absolute path, the returned path will be an absolute path that
-matches `other`, apart from the device name.
+matches `other`, apart from the drive name.
 _930
 _931
-If `other` has a device name, the returned path will have the same device name
-as `other`. Otherwise, the returned path will have the same device name as
-`self`. If neither has a device name, the returned path will not have a device
-name as well.
+If `other` has a drive, the returned path will have the same drive as `other`.
+Otherwise, the returned path will have the same drive as `self`. If neither has
+a drive, the returned path will not have a drive as well.
 _932
 _933
 Alias: `__truediv__()`
 _934
 _935
 Usage: <code><var>self</var> + <var>other</var></code> or <code><var>self</var>
 / <var>other</var></code>
@@ -2069,28 +2068,28 @@
 separator if possible to maximise cross-platform compatibility.
 ***** Constructor summary *****
       Initialise a normalised and generalised abstract file path, possibly by
       copying an existing GPath object.
 ***** Instance variables summary *****
   named_parts: list[str]
       Read-only named components of the path, not including the filesystem
-      root, device name, or any parent directories
+      root, drive name, or any parent directories
   parent_level: int
       Read-only number of levels of parent directories that the path is
       relative to, which may be 0
   parent_parts: list[str]
       Read-only path components representing a parent directory that it is
       relative to, if any, with a copy of parent_indicator for each level of
       parent directory
   relative_parts: list[str]
       Read-only relative components of the path, not including the filesystem
-      root or device name, with a copy of parent_indicator for each level of
+      root or drive name, with a copy of parent_indicator for each level of
       parent directory
   drive: str
-      Read-only device name
+      Read-only drive name
   absolute: bool
       Read-only flag for whether the path is an absolute path
   root: bool
       Read-only flag for whether the path is exactly the root of the filesystem
   encoding: Optional[str]
       Read-only encoding used to decode other paths that are given as bytes-
       like objects
@@ -2212,37 +2211,37 @@
 # path is a str
 159
 160
 if len(path) >= 2 and path[1] in _rules.generic_rules.drive_postfixes:
 161
 self._drive = path[0]
 162
-deviceless_path = path[2:]
+driveless_path = path[2:]
 163
 else:
 164
-deviceless_path = path
+driveless_path = path
 165
 166
 for root in _rules.generic_rules.roots:
 167
-if deviceless_path.startswith(root):
+if driveless_path.startswith(root):
 168
 self._root = True
 169
 break
 170
 171
 if self._root:
 172
-rootless_path = deviceless_path[1:]
+rootless_path = driveless_path[1:]
 173
 else:
 174
-rootless_path = deviceless_path
+rootless_path = driveless_path
 175
 176
 177
 parts = _split_relative(rootless_path, delimiters=(set
 (_rules.generic_rules.separators) | set(_rules.generic_rules.separators)))
 178
 parts = _normalise_relative(parts)
@@ -2275,15 +2274,15 @@
 ValueError if other is an invalid GPath
 ***** Examples *****
 GPath("/")
 GPath("/usr/bin")
 GPath("C:/Program Files")
 named_parts: list[str]
 Read-only named components of the path, not including the filesystem root,
-device name, or any parent directories
+drive name, or any parent directories
 ***** Examples *****
 GPath("usr/local/bin").named_parts     # ["usr", "local", "bin"]
 GPath("../../Documents").named_parts   # ["Documents"]
 GPath("/usr/bin").named_parts          # ["usr", "bin"]
 GPath("C:/Program Files").named_parts  # ["Program Files"]
 parent_level: int
 Read-only number of levels of parent directories that the path is relative to,
@@ -2295,26 +2294,26 @@
 Read-only path components representing a parent directory that it is relative
 to, if any, with a copy of parent_indicator for each level of parent directory
 ***** Examples *****
 GPath("../../Documents").parent_parts  # ["..", ".."]
 GPath("usr/local/bin").parent_parts    # []
 relative_parts: list[str]
 Read-only relative components of the path, not including the filesystem root or
-device name, with a copy of parent_indicator for each level of parent directory
+drive name, with a copy of parent_indicator for each level of parent directory
 ***** Examples *****
 GPath("usr/local/bin").relative_parts     # ["usr", "local", "bin"]
 GPath("../../Documents").relative_parts   # ["..", "..", "Documents"]
 GPath("/usr/bin").relative_parts          # ["usr", "bin"]
 GPath("C:/Program Files").relative_parts  # ["Program Files"]
 drive: str
-Read-only device name
+Read-only drive name
 ***** Examples *****
-GPath("C:/Windows").device       # "C:"
-GPath("/usr/bin").device         # ""
-GPath("../../Documents").device  # ""
+GPath("C:/Windows").drive       # "C:"
+GPath("/usr/bin").drive         # ""
+GPath("../../Documents").drive  # ""
 absolute: bool
 Read-only flag for whether the path is an absolute path
 ***** Examples *****
 GPath("/").absolute                # True
 GPath("C:/Windows").absolute       # True
 GPath("local/bin").absolute        # False
 GPath("../../Documents").absolute  # False
@@ -2943,15 +2942,15 @@
 571
 Find the longest common base path shared between `self` and `other`, or return
 None if no such path exists.
 572
 573
 A common base path might not exist if one path is an absolute path while the
 other is a relative path, or if the two paths are in different filesystems
-(with different device names), or in other cases as controlled by the
+(with different drive names), or in other cases as controlled by the
 `allow_current` and `allow_parents` options.
 574
 575
 If using the default options of `allow_current=True` and `allow_parent=False`,
 the binary operator for bitwise-and can be used: `__and__()` (usage:
 <code><var>g1</var> & <var>g2</var></code>).
 576
@@ -3093,15 +3092,15 @@
 return None
 646
 return common_path
 Find the longest common base path shared between self and other, or return None
 if no such path exists.
 A common base path might not exist if one path is an absolute path while the
 other is a relative path, or if the two paths are in different filesystems
-(with different device names), or in other cases as controlled by the
+(with different drive names), or in other cases as controlled by the
 allow_current and allow_parents options.
 If using the default options of allow_current=True and allow_parent=False, the
 binary operator for bitwise-and can be used: __and__() (usage: g1 & g2).
 ***** Parameters *****
 other : the path to compare with
 allow_current : whether two non-parent relative paths that do not share any
 components should be considered to have a common base path, namely the
@@ -3577,15 +3576,15 @@
 ⁰
 def __len__(self) -> int: View Source
 853
 def __len__(self) -> int:
 854
 """
 855
-Get the number of named path components, excluding any device name or parent
+Get the number of named path components, excluding any drive name or parent
 directories.
 856
 857
 Usage: <code>len(<var>g</var>)</code>
 858
 859
 Examples
@@ -3603,15 +3602,15 @@
 len(GPath("C:/"))         # 0
 866
 ```
 867
 """
 868
 return len(self._parts)
-Get the number of named path components, excluding any device name or parent
+Get the number of named path components, excluding any drive name or parent
 directories.
 Usage: len(g)
 ***** Examples *****
 len(GPath("/usr/bin"))    # 2
 len(GPath("/"))           # 0
 len(GPath("C:/Windows"))  # 0
 len(GPath("C:/"))         # 0
@@ -3620,15 +3619,15 @@
 Source
 871
 def __getitem__(self, index: Union[int, slice]) -> Union[str, list[str]]:
 872
 """
 873
 Get a 0-indexed named path component, or a slice of path components, excluding
-any device name or parent directories.
+any drive name or parent directories.
 874
 875
 Usage: <code><var>g</var>[<var>n</var>]</code>, <code><var>g</var>[<var>start</
 var>:<var>end</var>]</code>, <code><var>g</var>[<var>start</var>:<var>end</
 var>:<var>step</var>]</code>, etc.
 876
 877
@@ -3654,39 +3653,39 @@
 887
 return self._parts[index]
 888
 elif isinstance(index, slice):
 889
 return list(self._parts[index])
 Get a 0-indexed named path component, or a slice of path components, excluding
-any device name or parent directories.
+any drive name or parent directories.
 Usage: g[n], g[start:end], g[start:end:step], etc.
 ***** Examples *****
 GPath("/usr/local/bin")[1]    # "local"
 GPath("/usr/local/bin")[-1]   # "bin"
 GPath("/usr/local/bin")[1:]   # ["local", "bin"]
 GPath("/usr/local/bin")[::2]  # ["usr", "bin"]
 ⁰
 def __iter__(self) -> Iterator[str]: View Source
 892
 def __iter__(self) -> Iterator[str]:
 893
 """
 894
-Get an iterator through the named path components, excluding any device name or
+Get an iterator through the named path components, excluding any drive name or
 parent directories.
 895
 896
 Usage: <code>iter(<var>g</var>)</code> or <code>for <var>p</var> in <var>g</
 var>:</code>
 897
 """
 898
 return iter(self._parts)
-Get an iterator through the named path components, excluding any device name or
+Get an iterator through the named path components, excluding any drive name or
 parent directories.
 Usage: iter(g) or for p in g:
 ⁰
 def __contains__(self, other: Union[GPath, str, bytes, os.PathLike]) -> bool:
 View Source
 901
 def __contains__(self, other: GPathLike) -> bool:
@@ -3747,21 +3746,20 @@
 926
 """
 927
 Add (concatenate) `other` to the end of `self`, and return a new copy.
 928
 929
 If `other` is an absolute path, the returned path will be an absolute path that
-matches `other`, apart from the device name.
+matches `other`, apart from the drive name.
 930
 931
-If `other` has a device name, the returned path will have the same device name
-as `other`. Otherwise, the returned path will have the same device name as
-`self`. If neither has a device name, the returned path will not have a device
-name as well.
+If `other` has a drive, the returned path will have the same drive as `other`.
+Otherwise, the returned path will have the same drive as `self`. If neither has
+a drive, the returned path will not have a drive as well.
 932
 933
 Alias: `__truediv__()`
 934
 935
 Usage: <code><var>self</var> + <var>other</var></code> or <code><var>self</var>
 / <var>other</var></code>
@@ -3838,19 +3836,18 @@
 973
 new_path._drive = other._drive
 974
 975
 return new_path
 Add (concatenate) other to the end of self, and return a new copy.
 If other is an absolute path, the returned path will be an absolute path that
-matches other, apart from the device name.
-If other has a device name, the returned path will have the same device name as
-other. Otherwise, the returned path will have the same device name as self. If
-neither has a device name, the returned path will not have a device name as
-well.
+matches other, apart from the drive name.
+If other has a drive, the returned path will have the same drive as other.
+Otherwise, the returned path will have the same drive as self. If neither has a
+drive, the returned path will not have a drive as well.
 Alias: __truediv__()
 Usage: self + other or self / other
 Raises ValueError if either GPath is invalid
 ***** Examples *****
 GPath("/usr") + GPath("local/bin")                   # GPath("/usr/local/bin")
 GPath("C:/Windows/System32") + GPath("../SysWOW64")  # GPath("C:/Windows/
 SysWOW64")
```

### Comparing `generic-path-0.4/docs/html/search.js` & `generic-path-0.4.1/docs/html/search.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -711,15 +711,15 @@
                     "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">path</span><span class=\"p\">:</span> <span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">bytes</span><span class=\"p\">,</span> <span class=\"n\">os</span><span class=\"o\">.</span><span class=\"n\">PathLike</span><span class=\"p\">,</span> <span class=\"n\">gpath</span><span class=\"o\">.</span><span class=\"n\">_gpath</span><span class=\"o\">.</span><span class=\"n\">GPath</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">]</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;&#39;</span>,</span><span class=\"param\">\t<span class=\"n\">encoding</span><span class=\"p\">:</span> <span class=\"n\">Optional</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span>)</span>"
                 },
                 "gpath.GPath.named_parts": {
                     "fullname": "gpath.GPath.named_parts",
                     "modulename": "gpath",
                     "qualname": "GPath.named_parts",
                     "kind": "variable",
-                    "doc": "<p>Read-only named components of the path, not including the filesystem root, device name, or any parent directories</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;usr/local/bin&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">named_parts</span>     <span class=\"c1\"># [&quot;usr&quot;, &quot;local&quot;, &quot;bin&quot;]</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;../../Documents&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">named_parts</span>   <span class=\"c1\"># [&quot;Documents&quot;]</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/bin&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">named_parts</span>          <span class=\"c1\"># [&quot;usr&quot;, &quot;bin&quot;]</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;C:/Program Files&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">named_parts</span>  <span class=\"c1\"># [&quot;Program Files&quot;]</span>\n</code></pre>\n</div>\n",
+                    "doc": "<p>Read-only named components of the path, not including the filesystem root, drive name, or any parent directories</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;usr/local/bin&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">named_parts</span>     <span class=\"c1\"># [&quot;usr&quot;, &quot;local&quot;, &quot;bin&quot;]</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;../../Documents&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">named_parts</span>   <span class=\"c1\"># [&quot;Documents&quot;]</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/bin&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">named_parts</span>          <span class=\"c1\"># [&quot;usr&quot;, &quot;bin&quot;]</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;C:/Program Files&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">named_parts</span>  <span class=\"c1\"># [&quot;Program Files&quot;]</span>\n</code></pre>\n</div>\n",
                     "annotation": ": list[str]"
                 },
                 "gpath.GPath.parent_level": {
                     "fullname": "gpath.GPath.parent_level",
                     "modulename": "gpath",
                     "qualname": "GPath.parent_level",
                     "kind": "variable",
@@ -735,23 +735,23 @@
                     "annotation": ": list[str]"
                 },
                 "gpath.GPath.relative_parts": {
                     "fullname": "gpath.GPath.relative_parts",
                     "modulename": "gpath",
                     "qualname": "GPath.relative_parts",
                     "kind": "variable",
-                    "doc": "<p>Read-only relative components of the path, not including the filesystem root or device name, with a copy of <code>parent_indicator</code> for each level of parent directory</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;usr/local/bin&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">relative_parts</span>     <span class=\"c1\"># [&quot;usr&quot;, &quot;local&quot;, &quot;bin&quot;]</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;../../Documents&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">relative_parts</span>   <span class=\"c1\"># [&quot;..&quot;, &quot;..&quot;, &quot;Documents&quot;]</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/bin&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">relative_parts</span>          <span class=\"c1\"># [&quot;usr&quot;, &quot;bin&quot;]</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;C:/Program Files&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">relative_parts</span>  <span class=\"c1\"># [&quot;Program Files&quot;]</span>\n</code></pre>\n</div>\n",
+                    "doc": "<p>Read-only relative components of the path, not including the filesystem root or drive name, with a copy of <code>parent_indicator</code> for each level of parent directory</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;usr/local/bin&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">relative_parts</span>     <span class=\"c1\"># [&quot;usr&quot;, &quot;local&quot;, &quot;bin&quot;]</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;../../Documents&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">relative_parts</span>   <span class=\"c1\"># [&quot;..&quot;, &quot;..&quot;, &quot;Documents&quot;]</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/bin&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">relative_parts</span>          <span class=\"c1\"># [&quot;usr&quot;, &quot;bin&quot;]</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;C:/Program Files&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">relative_parts</span>  <span class=\"c1\"># [&quot;Program Files&quot;]</span>\n</code></pre>\n</div>\n",
                     "annotation": ": list[str]"
                 },
                 "gpath.GPath.drive": {
                     "fullname": "gpath.GPath.drive",
                     "modulename": "gpath",
                     "qualname": "GPath.drive",
                     "kind": "variable",
-                    "doc": "<p>Read-only device name</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;C:/Windows&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">device</span>       <span class=\"c1\"># &quot;C:&quot;</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/bin&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">device</span>         <span class=\"c1\"># &quot;&quot;</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;../../Documents&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">device</span>  <span class=\"c1\"># &quot;&quot;</span>\n</code></pre>\n</div>\n",
+                    "doc": "<p>Read-only drive name</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;C:/Windows&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">drive</span>       <span class=\"c1\"># &quot;C:&quot;</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/bin&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">drive</span>         <span class=\"c1\"># &quot;&quot;</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;../../Documents&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">drive</span>  <span class=\"c1\"># &quot;&quot;</span>\n</code></pre>\n</div>\n",
                     "annotation": ": str"
                 },
                 "gpath.GPath.absolute": {
                     "fullname": "gpath.GPath.absolute",
                     "modulename": "gpath",
                     "qualname": "GPath.absolute",
                     "kind": "variable",
@@ -829,15 +829,15 @@
                     "funcdef": "def"
                 },
                 "gpath.GPath.common_with": {
                     "fullname": "gpath.GPath.common_with",
                     "modulename": "gpath",
                     "qualname": "GPath.common_with",
                     "kind": "function",
-                    "doc": "<p>Find the longest common base path shared between <code>self</code> and <code>other</code>, or return None if no such path exists.</p>\n\n<p>A common base path might not exist if one path is an absolute path while the other is a relative path, or if the two paths are in different filesystems (with different device names), or in other cases as controlled by the <code>allow_current</code> and <code>allow_parents</code> options.</p>\n\n<p>If using the default options of <code>allow_current=True</code> and <code>allow_parent=False</code>, the binary operator for bitwise-and can be used: <code>__and__()</code> (usage: <code><var>g1</var> &amp; <var>g2</var></code>).</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>other</code>\n: the path to compare with</p>\n\n<p><code>allow_current</code>\n: whether two non-parent relative paths that do not share any components should be considered to have a common base path, namely the imaginary current working directory. For instance, <code>GPath(\"some/rel/path\").find_common(\"another/rel/path\")</code> will return <code>GPath(\"\")</code> if set to True, or return None if set to False.</p>\n\n<p><code>allow_parents</code>\n: whether two relative paths that are relative to different levels of parent directories should be considered to have a common base path, which is the highest level of parent directory between the two paths. For instance, <code>GPath(\"../rel/to/parent\").find_common(\"../../rel/to/grandparent\")</code> will return <code>GPath(\"../..\")</code> if set to True, or return None if set to False. <strong>Warning</strong>: when set to True, given a higher level of parent directory as output, it may not be possible to find the relative path to one of the inputs (see <code>relpath_from()</code>); in most cases False is more appropriate.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p><code>GPath</code>\n: the longest common base path, which may be empty, if it exists</p>\n\n<p><code>None</code>\n: otherwise</p>\n\n<h2 id=\"raises\">Raises</h2>\n\n<p><code>ValueError</code> if either <code>self</code> or <code>other</code> is an invalid GPath</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/bin&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">find_common</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/local/bin&quot;</span><span class=\"p\">)</span>               <span class=\"c1\"># GPath(&quot;/usr&quot;)</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;C:/Windows/System32&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">find_common</span><span class=\"p\">(</span><span class=\"s2\">&quot;C:/Program Files&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># GPath(&quot;C:/&quot;)</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;../Documents&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">find_common</span><span class=\"p\">(</span><span class=\"s2\">&quot;../Pictures&quot;</span><span class=\"p\">)</span>              <span class=\"c1\"># GPath(&quot;..&quot;)</span>\n</code></pre>\n</div>\n",
+                    "doc": "<p>Find the longest common base path shared between <code>self</code> and <code>other</code>, or return None if no such path exists.</p>\n\n<p>A common base path might not exist if one path is an absolute path while the other is a relative path, or if the two paths are in different filesystems (with different drive names), or in other cases as controlled by the <code>allow_current</code> and <code>allow_parents</code> options.</p>\n\n<p>If using the default options of <code>allow_current=True</code> and <code>allow_parent=False</code>, the binary operator for bitwise-and can be used: <code>__and__()</code> (usage: <code><var>g1</var> &amp; <var>g2</var></code>).</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>other</code>\n: the path to compare with</p>\n\n<p><code>allow_current</code>\n: whether two non-parent relative paths that do not share any components should be considered to have a common base path, namely the imaginary current working directory. For instance, <code>GPath(\"some/rel/path\").find_common(\"another/rel/path\")</code> will return <code>GPath(\"\")</code> if set to True, or return None if set to False.</p>\n\n<p><code>allow_parents</code>\n: whether two relative paths that are relative to different levels of parent directories should be considered to have a common base path, which is the highest level of parent directory between the two paths. For instance, <code>GPath(\"../rel/to/parent\").find_common(\"../../rel/to/grandparent\")</code> will return <code>GPath(\"../..\")</code> if set to True, or return None if set to False. <strong>Warning</strong>: when set to True, given a higher level of parent directory as output, it may not be possible to find the relative path to one of the inputs (see <code>relpath_from()</code>); in most cases False is more appropriate.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p><code>GPath</code>\n: the longest common base path, which may be empty, if it exists</p>\n\n<p><code>None</code>\n: otherwise</p>\n\n<h2 id=\"raises\">Raises</h2>\n\n<p><code>ValueError</code> if either <code>self</code> or <code>other</code> is an invalid GPath</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/bin&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">find_common</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/local/bin&quot;</span><span class=\"p\">)</span>               <span class=\"c1\"># GPath(&quot;/usr&quot;)</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;C:/Windows/System32&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">find_common</span><span class=\"p\">(</span><span class=\"s2\">&quot;C:/Program Files&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># GPath(&quot;C:/&quot;)</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;../Documents&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">find_common</span><span class=\"p\">(</span><span class=\"s2\">&quot;../Pictures&quot;</span><span class=\"p\">)</span>              <span class=\"c1\"># GPath(&quot;..&quot;)</span>\n</code></pre>\n</div>\n",
                     "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">other</span><span class=\"p\">:</span> <span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"n\">gpath</span><span class=\"o\">.</span><span class=\"n\">_gpath</span><span class=\"o\">.</span><span class=\"n\">GPath</span><span class=\"p\">,</span> <span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">bytes</span><span class=\"p\">,</span> <span class=\"n\">os</span><span class=\"o\">.</span><span class=\"n\">PathLike</span><span class=\"p\">]</span>,</span><span class=\"param\">\t<span class=\"n\">allow_current</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">allow_parents</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Optional</span><span class=\"p\">[</span><span class=\"n\">gpath</span><span class=\"o\">.</span><span class=\"n\">_gpath</span><span class=\"o\">.</span><span class=\"n\">GPath</span><span class=\"p\">]</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "gpath.GPath.subpath_from": {
                     "fullname": "gpath.GPath.subpath_from",
                     "modulename": "gpath",
                     "qualname": "GPath.subpath_from",
@@ -901,33 +901,33 @@
                     "funcdef": "def"
                 },
                 "gpath.GPath.__len__": {
                     "fullname": "gpath.GPath.__len__",
                     "modulename": "gpath",
                     "qualname": "GPath.__len__",
                     "kind": "function",
-                    "doc": "<p>Get the number of named path components, excluding any device name or parent directories.</p>\n\n<p>Usage: <code>len(<var>g</var>)</code></p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"nb\">len</span><span class=\"p\">(</span><span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/bin&quot;</span><span class=\"p\">))</span>    <span class=\"c1\"># 2</span>\n<span class=\"nb\">len</span><span class=\"p\">(</span><span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/&quot;</span><span class=\"p\">))</span>           <span class=\"c1\"># 0</span>\n<span class=\"nb\">len</span><span class=\"p\">(</span><span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;C:/Windows&quot;</span><span class=\"p\">))</span>  <span class=\"c1\"># 0</span>\n<span class=\"nb\">len</span><span class=\"p\">(</span><span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;C:/&quot;</span><span class=\"p\">))</span>         <span class=\"c1\"># 0</span>\n</code></pre>\n</div>\n",
+                    "doc": "<p>Get the number of named path components, excluding any drive name or parent directories.</p>\n\n<p>Usage: <code>len(<var>g</var>)</code></p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"nb\">len</span><span class=\"p\">(</span><span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/bin&quot;</span><span class=\"p\">))</span>    <span class=\"c1\"># 2</span>\n<span class=\"nb\">len</span><span class=\"p\">(</span><span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/&quot;</span><span class=\"p\">))</span>           <span class=\"c1\"># 0</span>\n<span class=\"nb\">len</span><span class=\"p\">(</span><span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;C:/Windows&quot;</span><span class=\"p\">))</span>  <span class=\"c1\"># 0</span>\n<span class=\"nb\">len</span><span class=\"p\">(</span><span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;C:/&quot;</span><span class=\"p\">))</span>         <span class=\"c1\"># 0</span>\n</code></pre>\n</div>\n",
                     "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">int</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "gpath.GPath.__getitem__": {
                     "fullname": "gpath.GPath.__getitem__",
                     "modulename": "gpath",
                     "qualname": "GPath.__getitem__",
                     "kind": "function",
-                    "doc": "<p>Get a 0-indexed named path component, or a slice of path components, excluding any device name or parent directories.</p>\n\n<p>Usage: <code><var>g</var>[<var>n</var>]</code>, <code><var>g</var>[<var>start</var>:<var>end</var>]</code>, <code><var>g</var>[<var>start</var>:<var>end</var>:<var>step</var>]</code>, etc.</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/local/bin&quot;</span><span class=\"p\">)[</span><span class=\"mi\">1</span><span class=\"p\">]</span>    <span class=\"c1\"># &quot;local&quot;</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/local/bin&quot;</span><span class=\"p\">)[</span><span class=\"o\">-</span><span class=\"mi\">1</span><span class=\"p\">]</span>   <span class=\"c1\"># &quot;bin&quot;</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/local/bin&quot;</span><span class=\"p\">)[</span><span class=\"mi\">1</span><span class=\"p\">:]</span>   <span class=\"c1\"># [&quot;local&quot;, &quot;bin&quot;]</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/local/bin&quot;</span><span class=\"p\">)[::</span><span class=\"mi\">2</span><span class=\"p\">]</span>  <span class=\"c1\"># [&quot;usr&quot;, &quot;bin&quot;]</span>\n</code></pre>\n</div>\n",
+                    "doc": "<p>Get a 0-indexed named path component, or a slice of path components, excluding any drive name or parent directories.</p>\n\n<p>Usage: <code><var>g</var>[<var>n</var>]</code>, <code><var>g</var>[<var>start</var>:<var>end</var>]</code>, <code><var>g</var>[<var>start</var>:<var>end</var>:<var>step</var>]</code>, etc.</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/local/bin&quot;</span><span class=\"p\">)[</span><span class=\"mi\">1</span><span class=\"p\">]</span>    <span class=\"c1\"># &quot;local&quot;</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/local/bin&quot;</span><span class=\"p\">)[</span><span class=\"o\">-</span><span class=\"mi\">1</span><span class=\"p\">]</span>   <span class=\"c1\"># &quot;bin&quot;</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/local/bin&quot;</span><span class=\"p\">)[</span><span class=\"mi\">1</span><span class=\"p\">:]</span>   <span class=\"c1\"># [&quot;local&quot;, &quot;bin&quot;]</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/local/bin&quot;</span><span class=\"p\">)[::</span><span class=\"mi\">2</span><span class=\"p\">]</span>  <span class=\"c1\"># [&quot;usr&quot;, &quot;bin&quot;]</span>\n</code></pre>\n</div>\n",
                     "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">index</span><span class=\"p\">:</span> <span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">slice</span><span class=\"p\">]</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]]</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "gpath.GPath.__iter__": {
                     "fullname": "gpath.GPath.__iter__",
                     "modulename": "gpath",
                     "qualname": "GPath.__iter__",
                     "kind": "function",
-                    "doc": "<p>Get an iterator through the named path components, excluding any device name or parent directories.</p>\n\n<p>Usage: <code>iter(<var>g</var>)</code> or <code>for <var>p</var> in <var>g</var>:</code></p>\n",
+                    "doc": "<p>Get an iterator through the named path components, excluding any drive name or parent directories.</p>\n\n<p>Usage: <code>iter(<var>g</var>)</code> or <code>for <var>p</var> in <var>g</var>:</code></p>\n",
                     "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">) -> <span class=\"n\">collections</span><span class=\"o\">.</span><span class=\"n\">abc</span><span class=\"o\">.</span><span class=\"n\">Iterator</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "gpath.GPath.__contains__": {
                     "fullname": "gpath.GPath.__contains__",
                     "modulename": "gpath",
                     "qualname": "GPath.__contains__",
@@ -937,15 +937,15 @@
                     "funcdef": "def"
                 },
                 "gpath.GPath.__add__": {
                     "fullname": "gpath.GPath.__add__",
                     "modulename": "gpath",
                     "qualname": "GPath.__add__",
                     "kind": "function",
-                    "doc": "<p>Add (concatenate) <code>other</code> to the end of <code>self</code>, and return a new copy.</p>\n\n<p>If <code>other</code> is an absolute path, the returned path will be an absolute path that matches <code>other</code>, apart from the device name.</p>\n\n<p>If <code>other</code> has a device name, the returned path will have the same device name as <code>other</code>. Otherwise, the returned path will have the same device name as <code>self</code>. If neither has a device name, the returned path will not have a device name as well.</p>\n\n<p>Alias: <code>__truediv__()</code></p>\n\n<p>Usage: <code><var>self</var> + <var>other</var></code> or <code><var>self</var> / <var>other</var></code></p>\n\n<p>Raises <code>ValueError</code> if either GPath is invalid</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr&quot;</span><span class=\"p\">)</span> <span class=\"o\">+</span> <span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;local/bin&quot;</span><span class=\"p\">)</span>                   <span class=\"c1\"># GPath(&quot;/usr/local/bin&quot;)</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;C:/Windows/System32&quot;</span><span class=\"p\">)</span> <span class=\"o\">+</span> <span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;../SysWOW64&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># GPath(&quot;C:/Windows/SysWOW64&quot;)</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;C:/Windows/System32&quot;</span><span class=\"p\">)</span> <span class=\"o\">+</span> <span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/bin&quot;</span><span class=\"p\">)</span>     <span class=\"c1\"># GPath(&quot;C:/usr/bin&quot;)</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;..&quot;</span><span class=\"p\">)</span> <span class=\"o\">+</span> <span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;../..&quot;</span><span class=\"p\">)</span>                         <span class=\"c1\"># GPath(&quot;../../..&quot;)</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;..&quot;</span><span class=\"p\">)</span> <span class=\"o\">/</span> <span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;../..&quot;</span><span class=\"p\">)</span>                         <span class=\"c1\"># GPath(&quot;../../..&quot;)</span>\n</code></pre>\n</div>\n",
+                    "doc": "<p>Add (concatenate) <code>other</code> to the end of <code>self</code>, and return a new copy.</p>\n\n<p>If <code>other</code> is an absolute path, the returned path will be an absolute path that matches <code>other</code>, apart from the drive name.</p>\n\n<p>If <code>other</code> has a drive, the returned path will have the same drive as <code>other</code>. Otherwise, the returned path will have the same drive as <code>self</code>. If neither has a drive, the returned path will not have a drive as well.</p>\n\n<p>Alias: <code>__truediv__()</code></p>\n\n<p>Usage: <code><var>self</var> + <var>other</var></code> or <code><var>self</var> / <var>other</var></code></p>\n\n<p>Raises <code>ValueError</code> if either GPath is invalid</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr&quot;</span><span class=\"p\">)</span> <span class=\"o\">+</span> <span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;local/bin&quot;</span><span class=\"p\">)</span>                   <span class=\"c1\"># GPath(&quot;/usr/local/bin&quot;)</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;C:/Windows/System32&quot;</span><span class=\"p\">)</span> <span class=\"o\">+</span> <span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;../SysWOW64&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># GPath(&quot;C:/Windows/SysWOW64&quot;)</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;C:/Windows/System32&quot;</span><span class=\"p\">)</span> <span class=\"o\">+</span> <span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;/usr/bin&quot;</span><span class=\"p\">)</span>     <span class=\"c1\"># GPath(&quot;C:/usr/bin&quot;)</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;..&quot;</span><span class=\"p\">)</span> <span class=\"o\">+</span> <span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;../..&quot;</span><span class=\"p\">)</span>                         <span class=\"c1\"># GPath(&quot;../../..&quot;)</span>\n<span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;..&quot;</span><span class=\"p\">)</span> <span class=\"o\">/</span> <span class=\"n\">GPath</span><span class=\"p\">(</span><span class=\"s2\">&quot;../..&quot;</span><span class=\"p\">)</span>                         <span class=\"c1\"># GPath(&quot;../../..&quot;)</span>\n</code></pre>\n</div>\n",
                     "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">other</span><span class=\"p\">:</span> <span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"n\">gpath</span><span class=\"o\">.</span><span class=\"n\">_gpath</span><span class=\"o\">.</span><span class=\"n\">GPath</span><span class=\"p\">,</span> <span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">bytes</span><span class=\"p\">,</span> <span class=\"n\">os</span><span class=\"o\">.</span><span class=\"n\">PathLike</span><span class=\"p\">]</span></span><span class=\"return-annotation\">) -> <span class=\"n\">gpath</span><span class=\"o\">.</span><span class=\"n\">_gpath</span><span class=\"o\">.</span><span class=\"n\">GPath</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "gpath.GPath.__sub__": {
                     "fullname": "gpath.GPath.__sub__",
                     "modulename": "gpath",
                     "qualname": "GPath.__sub__",
@@ -1265,15 +1265,15 @@
                 "gpath.GPath.__add__": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 77,
                     "bases": 0,
-                    "doc": 364
+                    "doc": 359
                 },
                 "gpath.GPath.__sub__": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 35,
@@ -8630,15 +8630,15 @@
                                         "gpath.GPath.__getitem__": {
                                             "tf": 1
                                         },
                                         "gpath.GPath.__iter__": {
                                             "tf": 1
                                         },
                                         "gpath.GPath.__add__": {
-                                            "tf": 2.449489742783178
+                                            "tf": 1
                                         }
                                     },
                                     "df": 8,
                                     "d": {
                                         "docs": {
                                             "gpath.GPath.named_parts": {
                                                 "tf": 2.23606797749979
@@ -8825,55 +8825,14 @@
                                                 },
                                                 "df": 4
                                             }
                                         }
                                     }
                                 }
                             },
-                            "v": {
-                                "docs": {},
-                                "df": 0,
-                                "i": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "c": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "e": {
-                                            "docs": {
-                                                "gpath.GPath.named_parts": {
-                                                    "tf": 1
-                                                },
-                                                "gpath.GPath.relative_parts": {
-                                                    "tf": 1
-                                                },
-                                                "gpath.GPath.drive": {
-                                                    "tf": 2
-                                                },
-                                                "gpath.GPath.common_with": {
-                                                    "tf": 1
-                                                },
-                                                "gpath.GPath.__len__": {
-                                                    "tf": 1
-                                                },
-                                                "gpath.GPath.__getitem__": {
-                                                    "tf": 1
-                                                },
-                                                "gpath.GPath.__iter__": {
-                                                    "tf": 1
-                                                },
-                                                "gpath.GPath.__add__": {
-                                                    "tf": 2.449489742783178
-                                                }
-                                            },
-                                            "df": 8
-                                        }
-                                    }
-                                }
-                            },
                             "t": {
                                 "docs": {},
                                 "df": 0,
                                 "e": {
                                     "docs": {},
                                     "df": 0,
                                     "r": {
@@ -9128,14 +9087,61 @@
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
                         },
+                        "r": {
+                            "docs": {},
+                            "df": 0,
+                            "i": {
+                                "docs": {},
+                                "df": 0,
+                                "v": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "e": {
+                                        "docs": {
+                                            "gpath.GPath.named_parts": {
+                                                "tf": 1
+                                            },
+                                            "gpath.GPath.relative_parts": {
+                                                "tf": 1
+                                            },
+                                            "gpath.GPath.drive": {
+                                                "tf": 2
+                                            },
+                                            "gpath.GPath.with_drive": {
+                                                "tf": 3.605551275463989
+                                            },
+                                            "gpath.GPath.without_drive": {
+                                                "tf": 2.23606797749979
+                                            },
+                                            "gpath.GPath.common_with": {
+                                                "tf": 1
+                                            },
+                                            "gpath.GPath.__len__": {
+                                                "tf": 1
+                                            },
+                                            "gpath.GPath.__getitem__": {
+                                                "tf": 1
+                                            },
+                                            "gpath.GPath.__iter__": {
+                                                "tf": 1
+                                            },
+                                            "gpath.GPath.__add__": {
+                                                "tf": 2.449489742783178
+                                            }
+                                        },
+                                        "df": 10
+                                    }
+                                }
+                            }
+                        },
                         "o": {
                             "docs": {
                                 "gpath.GPath.common_with": {
                                     "tf": 1
                                 }
                             },
                             "df": 1,
@@ -9322,37 +9328,14 @@
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
                         },
-                        "r": {
-                            "docs": {},
-                            "df": 0,
-                            "i": {
-                                "docs": {},
-                                "df": 0,
-                                "v": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "e": {
-                                        "docs": {
-                                            "gpath.GPath.with_drive": {
-                                                "tf": 3.605551275463989
-                                            },
-                                            "gpath.GPath.without_drive": {
-                                                "tf": 2.23606797749979
-                                            }
-                                        },
-                                        "df": 2
-                                    }
-                                }
-                            }
-                        },
                         ":": {
                             "docs": {},
                             "df": 0,
                             "/": {
                                 "docs": {},
                                 "df": 0,
                                 "w": {
```

### Comparing `generic-path-0.4/pyproject.toml` & `generic-path-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `generic-path-0.4/src/generic_path.egg-info/PKG-INFO` & `generic-path-0.4.1/src/generic_path.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generic-path
-Version: 0.4
+Version: 0.4.1
 Summary: Generalised abstract file path that provides path manipulations independent from the local environment
 Author-email: Yu Shiyang <yu.shiyang@gnayihs.uy>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/yushiyangk/GPath
 Project-URL: Documentation, https://gpath.gnayihs.uy/
 Project-URL: Issues, https://github.com/yushiyangk/GPath/issues
 Keywords: python,filepath,filesystem,cross-platform
@@ -179,14 +179,18 @@
 
 ## Changelog
 
 This project follows [PEP 440](https://peps.python.org/pep-0440/) and [Semantic Versioning (SemVer)](https://semver.org/spec/v2.0.0.html). In addition to the guarantees specified by SemVer, for versions before 1.0, this project guarantees backwards compatibility of the API for patch version updates (0.<var>y</var>.<b><var>z</var></b>).
 
 The recommended version specifier is <code>generic-path ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>generic-path ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
 
+### 0.4.1
+
+- Fixed embedded documentation
+
 ### 0.4
 
 #### Breaking API changes
 
 - Replaced the following instance methods with read-only properties:
 	- <code><var>g</var>.get_parent_level()</code> → <code><var>g</var>.parent_level</code>
 	- <code><var>g</var>.get_parent_parts()</code> → <code><var>g</var>.parent_parts</code>
```

### Comparing `generic-path-0.4/src/gpath/_gpath.py` & `generic-path-0.4.1/src/gpath/_gpath.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,27 +154,27 @@
 			else:
 				path = path.decode(self._encoding)
 
 		# path is a str
 
 		if len(path) >= 2 and path[1] in _rules.generic_rules.drive_postfixes:
 			self._drive = path[0]
-			deviceless_path = path[2:]
+			driveless_path = path[2:]
 		else:
-			deviceless_path = path
+			driveless_path = path
 
 		for root in _rules.generic_rules.roots:
-			if deviceless_path.startswith(root):
+			if driveless_path.startswith(root):
 				self._root = True
 				break
 
 		if self._root:
-			rootless_path = deviceless_path[1:]
+			rootless_path = driveless_path[1:]
 		else:
-			rootless_path = deviceless_path
+			rootless_path = driveless_path
 
 
 		parts = _split_relative(rootless_path, delimiters=(set(_rules.generic_rules.separators) | set(_rules.generic_rules.separators)))
 		parts = _normalise_relative(parts)
 		parent_level = 0
 		while parent_level < len(parts) and parts[parent_level] in _rules.generic_rules.parent_indicators:
 			parent_level += 1
@@ -182,15 +182,15 @@
 		if self._root == False:
 			self._parent_level = parent_level
 
 
 	@property
 	def named_parts(self) -> list[str]:
 		"""
-			Read-only named components of the path, not including the filesystem root, device name, or any parent directories
+			Read-only named components of the path, not including the filesystem root, drive name, or any parent directories
 
 			Examples
 			--------
 			```python
 			GPath("usr/local/bin").named_parts     # ["usr", "local", "bin"]
 			GPath("../../Documents").named_parts   # ["Documents"]
 			GPath("/usr/bin").named_parts          # ["usr", "bin"]
@@ -226,15 +226,15 @@
 			```
 		"""
 		return [_rules.generic_rules.parent_indicators[0] for i in range(self._parent_level)]
 
 	@property
 	def relative_parts(self) -> list[str]:
 		"""
-			Read-only relative components of the path, not including the filesystem root or device name, with a copy of `parent_indicator` for each level of parent directory
+			Read-only relative components of the path, not including the filesystem root or drive name, with a copy of `parent_indicator` for each level of parent directory
 
 			Examples
 			--------
 			```python
 			GPath("usr/local/bin").relative_parts     # ["usr", "local", "bin"]
 			GPath("../../Documents").relative_parts   # ["..", "..", "Documents"]
 			GPath("/usr/bin").relative_parts          # ["usr", "bin"]
@@ -242,22 +242,22 @@
 			```
 		"""
 		return self.parent_parts + list(self._parts)
 
 	@property
 	def drive(self) -> str:
 		"""
-			Read-only device name
+			Read-only drive name
 
 			Examples
 			--------
 			```python
-			GPath("C:/Windows").device       # "C:"
-			GPath("/usr/bin").device         # ""
-			GPath("../../Documents").device  # ""
+			GPath("C:/Windows").drive       # "C:"
+			GPath("/usr/bin").drive         # ""
+			GPath("../../Documents").drive  # ""
 			```
 		"""
 		return self._drive
 
 	@property
 	def absolute(self) -> bool:
 		"""
@@ -565,15 +565,15 @@
 		return self.with_drive(None)
 
 
 	def common_with(self, other: GPathLike, allow_current: bool=True, allow_parents: bool=False) -> Optional[GPath]:
 		"""
 			Find the longest common base path shared between `self` and `other`, or return None if no such path exists.
 
-			A common base path might not exist if one path is an absolute path while the other is a relative path, or if the two paths are in different filesystems (with different device names), or in other cases as controlled by the `allow_current` and `allow_parents` options.
+			A common base path might not exist if one path is an absolute path while the other is a relative path, or if the two paths are in different filesystems (with different drive names), or in other cases as controlled by the `allow_current` and `allow_parents` options.
 
 			If using the default options of `allow_current=True` and `allow_parent=False`, the binary operator for bitwise-and can be used: `__and__()` (usage: <code><var>g1</var> & <var>g2</var></code>).
 
 			Parameters
 			----------
 			`other`
 			: the path to compare with
@@ -847,15 +847,15 @@
 			return f"GPath({repr(str(self))}{encoding_repr})"
 		else:
 			return f"GPath({repr('')}{encoding_repr})"
 
 
 	def __len__(self) -> int:
 		"""
-			Get the number of named path components, excluding any device name or parent directories.
+			Get the number of named path components, excluding any drive name or parent directories.
 
 			Usage: <code>len(<var>g</var>)</code>
 
 			Examples
 			--------
 			```python
 			len(GPath("/usr/bin"))    # 2
@@ -865,15 +865,15 @@
 			```
 		"""
 		return len(self._parts)
 
 
 	def __getitem__(self, index: Union[int, slice]) -> Union[str, list[str]]:
 		"""
-			Get a 0-indexed named path component, or a slice of path components, excluding any device name or parent directories.
+			Get a 0-indexed named path component, or a slice of path components, excluding any drive name or parent directories.
 
 			Usage: <code><var>g</var>[<var>n</var>]</code>, <code><var>g</var>[<var>start</var>:<var>end</var>]</code>, <code><var>g</var>[<var>start</var>:<var>end</var>:<var>step</var>]</code>, etc.
 
 			Examples
 			--------
 			```python
 			GPath("/usr/local/bin")[1]    # "local"
@@ -886,15 +886,15 @@
 			return self._parts[index]
 		elif isinstance(index, slice):
 			return list(self._parts[index])
 
 
 	def __iter__(self) -> Iterator[str]:
 		"""
-			Get an iterator through the named path components, excluding any device name or parent directories.
+			Get an iterator through the named path components, excluding any drive name or parent directories.
 
 			Usage: <code>iter(<var>g</var>)</code> or <code>for <var>p</var> in <var>g</var>:</code>
 		"""
 		return iter(self._parts)
 
 
 	def __contains__(self, other: GPathLike) -> bool:
@@ -921,17 +921,17 @@
 		return common_path is not None and common_path == self
 
 
 	def __add__(self, other: GPathLike) -> GPath:
 		"""
 			Add (concatenate) `other` to the end of `self`, and return a new copy.
 
-			If `other` is an absolute path, the returned path will be an absolute path that matches `other`, apart from the device name.
+			If `other` is an absolute path, the returned path will be an absolute path that matches `other`, apart from the drive name.
 
-			If `other` has a device name, the returned path will have the same device name as `other`. Otherwise, the returned path will have the same device name as `self`. If neither has a device name, the returned path will not have a device name as well.
+			If `other` has a drive, the returned path will have the same drive as `other`. Otherwise, the returned path will have the same drive as `self`. If neither has a drive, the returned path will not have a drive as well.
 
 			Alias: `__truediv__()`
 
 			Usage: <code><var>self</var> + <var>other</var></code> or <code><var>self</var> / <var>other</var></code>
 
 			Raises `ValueError` if either GPath is invalid
```

### Comparing `generic-path-0.4/tests/test_gpath.py` & `generic-path-0.4.1/tests/test_gpath.py`

 * *Files identical despite different names*

