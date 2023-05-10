# Comparing `tmp/noiftimer-2.0.0.tar.gz` & `tmp/noiftimer-2.1.0.tar.gz`

## Comparing `noiftimer-2.0.0.tar` & `noiftimer-2.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 noiftimer-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 noiftimer-2.0.0/docs/index.html
--rw-r--r--   0        0        0    34120 2020-02-02 00:00:00.000000 noiftimer-2.0.0/docs/noiftimer.html
--rw-r--r--   0        0        0    24774 2020-02-02 00:00:00.000000 noiftimer-2.0.0/docs/search.js
--rw-r--r--   0        0        0   130100 2020-02-02 00:00:00.000000 noiftimer-2.0.0/docs/noiftimer/noiftimer.html
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 noiftimer-2.0.0/src/noiftimer/__init__.py
--rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 noiftimer-2.0.0/src/noiftimer/noiftimer.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 noiftimer-2.0.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 noiftimer-2.0.0/LICENSE.txt
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 noiftimer-2.0.0/README.md
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 noiftimer-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 noiftimer-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 noiftimer-2.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 noiftimer-2.1.0/docs/index.html
+-rw-r--r--   0        0        0    34120 2020-02-02 00:00:00.000000 noiftimer-2.1.0/docs/noiftimer.html
+-rw-r--r--   0        0        0    26805 2020-02-02 00:00:00.000000 noiftimer-2.1.0/docs/search.js
+-rw-r--r--   0        0        0   151271 2020-02-02 00:00:00.000000 noiftimer-2.1.0/docs/noiftimer/noiftimer.html
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 noiftimer-2.1.0/src/noiftimer/__init__.py
+-rw-r--r--   0        0        0     6842 2020-02-02 00:00:00.000000 noiftimer-2.1.0/src/noiftimer/noiftimer.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 noiftimer-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 noiftimer-2.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 noiftimer-2.1.0/README.md
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 noiftimer-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 noiftimer-2.1.0/PKG-INFO
```

### Comparing `noiftimer-2.0.0/CHANGELOG.md` & `noiftimer-2.1.0/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,44 @@
 # Changelog
 
-## 1.3.0 (2023-03-31)
+## 2.0.0 (2023-04-15)
+
+#### New Features
+
+* add history property
+* make Self typing python 3.10 compatible
+#### Fixes
+
+* initialize result in time_it
+* update time_it to call average time correctly
+#### Refactorings
+
+* convert most members to properties
+* revert datetime library usage back to time library
+* import Self from typing_extensions
+#### Others
+
+* update readme
+* remove unused import
+* remove current_elapsed_time() making package compatible with python >=3.6
+
+
+## v1.3.0 (2023-03-31)
 
 #### Fixes
 
 * return <1{unit} from format_time when an empty string is returned
 #### Refactorings
 
 * convert format_time() to a staticmethod
 * remove _get_time_unit and use divmod instead
+#### Others
+
+* build v1.3.0
+* update changelog
 
 
 ## v1.2.0 (2023-03-30)
 
 #### New Features
 
 * add time_it decorator
```

### Comparing `noiftimer-2.0.0/docs/noiftimer.html` & `noiftimer-2.1.0/docs/noiftimer.html`

 * *Files identical despite different names*

### Comparing `noiftimer-2.0.0/docs/search.js` & `noiftimer-2.1.0/docs/search.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -693,81 +693,132 @@
         "kind": "module",
         "doc": "<p></p>\n"
     }, {
         "fullname": "noiftimer.noiftimer.time_it",
         "modulename": "noiftimer.noiftimer",
         "qualname": "time_it",
         "kind": "function",
-        "doc": "<p>Decorator to time function execution time\nand print the results.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><strong>loops</strong>:  How many times to loop the function,\nstarting and stopping the timer before and after\neach loop.</li>\n</ul>\n",
+        "doc": "<p>Decorator to time function execution time and print the results.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>loops</code>: How many times to execute the decorated function,\nstarting and stopping the timer before and after each loop.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">loops</span><span class=\"p\">:</span> <span class=\"nb\">int</span> <span class=\"o\">=</span> <span class=\"mi\">1</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Callable</span><span class=\"p\">[</span><span class=\"o\">...</span><span class=\"p\">,</span> <span class=\"n\">Any</span><span class=\"p\">]</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "noiftimer.noiftimer.Timer",
         "modulename": "noiftimer.noiftimer",
         "qualname": "Timer",
         "kind": "class",
-        "doc": "<p>Simple timer class that tracks total elapsed time\nand average time between calls to 'start' and 'stop'.</p>\n"
+        "doc": "<p>Simple timer class that tracks total elapsed time\nand average time between calls to <code>start()</code> and <code>stop()</code>.</p>\n"
     }, {
         "fullname": "noiftimer.noiftimer.Timer.__init__",
         "modulename": "noiftimer.noiftimer",
         "qualname": "Timer.__init__",
         "kind": "function",
-        "doc": "<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>averaging_window_length</strong>:  Number of start/stop cycles\nto calculate the average elapsed time with.</p></li>\n<li><p><strong>subsecond_resolution</strong>:  Whether to print formatted time\nstrings with subsecond resolution or not.</p></li>\n</ul>\n",
+        "doc": "<h4 id=\"params\">:params:</h4>\n\n<ul>\n<li><p><code>averaging_window_length</code>: Number of start/stop cycles to calculate the average elapsed time with.</p></li>\n<li><p><code>subsecond_resolution</code>: Whether to print formatted time strings with subsecond resolution or not.</p></li>\n</ul>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">averaging_window_length</span><span class=\"p\">:</span> <span class=\"nb\">int</span> <span class=\"o\">=</span> <span class=\"mi\">10</span>, </span><span class=\"param\"><span class=\"n\">subsecond_resolution</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span></span>)</span>"
     }, {
         "fullname": "noiftimer.noiftimer.Timer.started",
         "modulename": "noiftimer.noiftimer",
         "qualname": "Timer.started",
         "kind": "variable",
-        "doc": "<p>Returns whether the timer has\nbeen started and is currently running.</p>\n",
+        "doc": "<p>Returns whether the timer has been started and is currently running.</p>\n",
         "annotation": ": bool"
     }, {
         "fullname": "noiftimer.noiftimer.Timer.elapsed",
         "modulename": "noiftimer.noiftimer",
         "qualname": "Timer.elapsed",
         "kind": "variable",
-        "doc": "<p>Return the currently elapsed time.</p>\n",
+        "doc": "<p>Returns the currently elapsed time.</p>\n",
         "annotation": ": float"
     }, {
         "fullname": "noiftimer.noiftimer.Timer.elapsed_str",
         "modulename": "noiftimer.noiftimer",
         "qualname": "Timer.elapsed_str",
         "kind": "variable",
-        "doc": "<p>Return the currently elapsed time\nas a formatted string.</p>\n",
+        "doc": "<p>Returns the currently elapsed time as a formatted string.</p>\n",
         "annotation": ": str"
     }, {
+        "fullname": "noiftimer.noiftimer.Timer.average_elapsed",
+        "modulename": "noiftimer.noiftimer",
+        "qualname": "Timer.average_elapsed",
+        "kind": "variable",
+        "doc": "<p>Returns the average elapsed time.</p>\n",
+        "annotation": ": float"
+    }, {
+        "fullname": "noiftimer.noiftimer.Timer.average_elapsed_str",
+        "modulename": "noiftimer.noiftimer",
+        "qualname": "Timer.average_elapsed_str",
+        "kind": "variable",
+        "doc": "<p>Returns the average elapsed time as a formatted string.</p>\n",
+        "annotation": ": str"
+    }, {
+        "fullname": "noiftimer.noiftimer.Timer.start_time",
+        "modulename": "noiftimer.noiftimer",
+        "qualname": "Timer.start_time",
+        "kind": "variable",
+        "doc": "<p>Returns the timestamp of the last call to <code>start()</code>.</p>\n",
+        "annotation": ": float"
+    }, {
+        "fullname": "noiftimer.noiftimer.Timer.stop_time",
+        "modulename": "noiftimer.noiftimer",
+        "qualname": "Timer.stop_time",
+        "kind": "variable",
+        "doc": "<p>Returns the timestamp of the last call to <code>stop()</code>.</p>\n",
+        "annotation": ": float"
+    }, {
+        "fullname": "noiftimer.noiftimer.Timer.history",
+        "modulename": "noiftimer.noiftimer",
+        "qualname": "Timer.history",
+        "kind": "variable",
+        "doc": "<p>Returns the history buffer for this timer.</p>\n\n<p>At most, it will be <code>averaging_window_length</code> elements long.</p>\n",
+        "annotation": ": list[float]"
+    }, {
         "fullname": "noiftimer.noiftimer.Timer.start",
         "modulename": "noiftimer.noiftimer",
         "qualname": "Timer.start",
         "kind": "function",
-        "doc": "<p>Start timer.\nReturns this Timer instance so\ntimer start can be chained to\nTimer creation.</p>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">timer</span> <span class=\"o\">=</span> <span class=\"n\">Timer</span><span class=\"p\">()</span><span class=\"o\">.</span><span class=\"n\">start</span><span class=\"p\">()</span>\n</code></pre>\n</div>\n",
+        "doc": "<p>Start the timer.</p>\n\n<p>Returns this Timer instance so timer start can be chained to Timer creation if desired.</p>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">timer</span> <span class=\"o\">=</span> <span class=\"n\">Timer</span><span class=\"p\">()</span><span class=\"o\">.</span><span class=\"n\">start</span><span class=\"p\">()</span>\n</code></pre>\n</div>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span><span class=\"p\">:</span> <span class=\"n\">Self</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Self</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "noiftimer.noiftimer.Timer.stop",
         "modulename": "noiftimer.noiftimer",
         "qualname": "Timer.stop",
         "kind": "function",
-        "doc": "<p>Stop timer.</p>\n\n<p>Calculates elapsed time and average elapsed time.</p>\n",
+        "doc": "<p>Stop the timer.</p>\n\n<p>Calculates elapsed time and average elapsed time.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">):</span></span>",
+        "funcdef": "def"
+    }, {
+        "fullname": "noiftimer.noiftimer.Timer.pause",
+        "modulename": "noiftimer.noiftimer",
+        "qualname": "Timer.pause",
+        "kind": "function",
+        "doc": "<p>Pause the timer.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">):</span></span>",
+        "funcdef": "def"
+    }, {
+        "fullname": "noiftimer.noiftimer.Timer.unpause",
+        "modulename": "noiftimer.noiftimer",
+        "qualname": "Timer.unpause",
+        "kind": "function",
+        "doc": "<p>Unpause the timer.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "noiftimer.noiftimer.Timer.format_time",
         "modulename": "noiftimer.noiftimer",
         "qualname": "Timer.format_time",
         "kind": "function",
-        "doc": "<p>Returns num_seconds as a string with units.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><strong>subsecond_resolution</strong>:  Include milliseconds\nand microseconds with the output.</li>\n</ul>\n",
+        "doc": "<p>Returns <code>num_seconds</code> as a string with units.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>subsecond_resolution</code>: Include milliseconds and microseconds with the output.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">num_seconds</span><span class=\"p\">:</span> <span class=\"nb\">float</span>, </span><span class=\"param\"><span class=\"n\">subsecond_resolution</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "noiftimer.noiftimer.Timer.stats",
         "modulename": "noiftimer.noiftimer",
         "qualname": "Timer.stats",
         "kind": "variable",
-        "doc": "<p>Returns a string stating the currently elapsed time\nand the average elapsed time.</p>\n",
+        "doc": "<p>Returns a string stating the currently elapsed time and the average elapsed time.</p>\n",
         "annotation": ": str"
     }];
 
     // mirrored in build-search-index.js (part 1)
     // Also split on html tags. this is a cheap heuristic, but good enough.
     elasticlunr.tokenizer.setSeperator(/[\s\-.;&_'"=,()]+|<[^>]*>/);
```

### Comparing `noiftimer-2.0.0/docs/noiftimer/noiftimer.html` & `noiftimer-2.1.0/docs/noiftimer/noiftimer.html`

 * *Files 3% similar despite different names*

```diff
@@ -45,20 +45,41 @@
                         <li>
                                 <a class="variable" href="#Timer.elapsed">elapsed</a>
                         </li>
                         <li>
                                 <a class="variable" href="#Timer.elapsed_str">elapsed_str</a>
                         </li>
                         <li>
+                                <a class="variable" href="#Timer.average_elapsed">average_elapsed</a>
+                        </li>
+                        <li>
+                                <a class="variable" href="#Timer.average_elapsed_str">average_elapsed_str</a>
+                        </li>
+                        <li>
+                                <a class="variable" href="#Timer.start_time">start_time</a>
+                        </li>
+                        <li>
+                                <a class="variable" href="#Timer.stop_time">stop_time</a>
+                        </li>
+                        <li>
+                                <a class="variable" href="#Timer.history">history</a>
+                        </li>
+                        <li>
                                 <a class="function" href="#Timer.start">start</a>
                         </li>
                         <li>
                                 <a class="function" href="#Timer.stop">stop</a>
                         </li>
                         <li>
+                                <a class="function" href="#Timer.pause">pause</a>
+                        </li>
+                        <li>
+                                <a class="function" href="#Timer.unpause">unpause</a>
+                        </li>
+                        <li>
                                 <a class="function" href="#Timer.format_time">format_time</a>
                         </li>
                         <li>
                                 <a class="variable" href="#Timer.stats">stats</a>
                         </li>
                 </ul>
 
@@ -87,20 +108,20 @@
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">time</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">Any</span><span class="p">,</span> <span class="n">Callable</span>
 </span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a>
 </span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">from</span> <span class="nn">typing_extensions</span> <span class="kn">import</span> <span class="n">Self</span>
 </span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a>
 </span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a>
 </span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="k">def</span> <span class="nf">time_it</span><span class="p">(</span><span class="n">loops</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">1</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">]:</span>
-</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a>    <span class="sd">&quot;&quot;&quot;Decorator to time function execution time</span>
-</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="sd">    and print the results.</span>
-</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>
-</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a><span class="sd">    :param loops: How many times to loop the function,</span>
-</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a><span class="sd">    starting and stopping the timer before and after</span>
-</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="sd">    each loop.&quot;&quot;&quot;</span>
+</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a>    <span class="sd">&quot;&quot;&quot;Decorator to time function execution time and print the results.</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a>
+</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>
+</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a><span class="sd">    `loops`: How many times to execute the decorated function,</span>
+</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="sd">    starting and stopping the timer before and after each loop.&quot;&quot;&quot;</span>
 </span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>
 </span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>    <span class="k">def</span> <span class="nf">decorator</span><span class="p">(</span><span class="n">func</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">]:</span>
 </span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>        <span class="k">def</span> <span class="nf">wrapper</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
 </span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>            <span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">loops</span><span class="p">)</span>
 </span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>            <span class="n">result</span> <span class="o">=</span> <span class="kc">None</span>
 </span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>            <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">loops</span><span class="p">):</span>
 </span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>                <span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
@@ -112,145 +133,189 @@
 </span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>            <span class="k">return</span> <span class="n">result</span>
 </span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>
 </span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>        <span class="k">return</span> <span class="n">wrapper</span>
 </span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>
 </span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>    <span class="k">return</span> <span class="n">decorator</span>
 </span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>
 </span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a><span class="k">class</span> <span class="nc">Timer</span><span class="p">:</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>    <span class="sd">&quot;&quot;&quot;Simple timer class that tracks total elapsed time</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a><span class="sd">    and average time between calls to &#39;start&#39; and &#39;stop&#39;.&quot;&quot;&quot;</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">10</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>    <span class="p">):</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>        <span class="sd">&quot;&quot;&quot;:param averaging_window_length: Number of start/stop cycles</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a><span class="sd">        to calculate the average elapsed time with.</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a><span class="k">class</span> <span class="nc">_Pauser</span><span class="p">:</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_pause_start</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_pause_total</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_paused</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>    <span class="k">def</span> <span class="nf">pause</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_pause_start</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_paused</span> <span class="o">=</span> <span class="kc">True</span>
 </span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a><span class="sd">        :param subsecond_resolution: Whether to print formatted time</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a><span class="sd">        strings with subsecond resolution or not.&quot;&quot;&quot;</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="n">averaging_window_length</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span> <span class="o">=</span> <span class="n">subsecond_resolution</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="nd">@property</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>    <span class="k">def</span> <span class="nf">started</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether the timer has</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a><span class="sd">        been started and is currently running.&quot;&quot;&quot;</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_started</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>    <span class="k">def</span> <span class="nf">unpause</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_pause_total</span> <span class="o">+=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_pause_start</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_paused</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>    <span class="k">def</span> <span class="nf">reset</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_pause_start</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_pause_total</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_paused</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>    <span class="nd">@property</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>    <span class="k">def</span> <span class="nf">pause_total</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_paused</span><span class="p">:</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_pause_total</span> <span class="o">+</span> <span class="p">(</span><span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_pause_start</span><span class="p">)</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_pause_total</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>
 </span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>    <span class="nd">@property</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>    <span class="k">def</span> <span class="nf">elapsed</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>        <span class="sd">&quot;&quot;&quot;Return the currently elapsed time.&quot;&quot;&quot;</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_started</span><span class="p">:</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>            <span class="k">return</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>    <span class="nd">@property</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>    <span class="k">def</span> <span class="nf">elapsed_str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="sd">&quot;&quot;&quot;Return the currently elapsed time</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a><span class="sd">        as a formatted string.&quot;&quot;&quot;</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span><span class="p">)</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>    <span class="nd">@property</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>    <span class="k">def</span> <span class="nf">average_elapsed</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>    <span class="nd">@property</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>    <span class="k">def</span> <span class="nf">average_elapsed_str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span><span class="p">)</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a><span class="k">class</span> <span class="nc">Timer</span><span class="p">:</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>    <span class="sd">&quot;&quot;&quot;Simple timer class that tracks total elapsed time</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a><span class="sd">    and average time between calls to `start()` and `stop()`.&quot;&quot;&quot;</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">10</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>    <span class="p">):</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a><span class="sd">        * `averaging_window_length`: Number of start/stop cycles to calculate the average elapsed time with.</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a><span class="sd">        * `subsecond_resolution`: Whether to print formatted time strings with subsecond resolution or not.&quot;&quot;&quot;</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="n">averaging_window_length</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span> <span class="o">=</span> <span class="n">subsecond_resolution</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_pauser</span> <span class="o">=</span> <span class="n">_Pauser</span><span class="p">()</span>
 </span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>
 </span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="nd">@property</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>    <span class="k">def</span> <span class="nf">start_time</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>    <span class="nd">@property</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>    <span class="k">def</span> <span class="nf">stop_time</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>    <span class="nd">@property</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>    <span class="k">def</span> <span class="nf">history</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">float</span><span class="p">]:</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_history</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>    <span class="k">def</span> <span class="nf">start</span><span class="p">(</span><span class="bp">self</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>        <span class="sd">&quot;&quot;&quot;Start timer.</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a><span class="sd">        Returns this Timer instance so</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="sd">        timer start can be chained to</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a><span class="sd">        Timer creation.</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>    <span class="k">def</span> <span class="nf">started</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether the timer has been started and is currently running.&quot;&quot;&quot;</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_started</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>    <span class="nd">@property</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>    <span class="k">def</span> <span class="nf">elapsed</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="sd">&quot;&quot;&quot;Returns the currently elapsed time.&quot;&quot;&quot;</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_started</span><span class="p">:</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>            <span class="k">return</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_pauser</span><span class="o">.</span><span class="n">pause_total</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>    <span class="nd">@property</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>    <span class="k">def</span> <span class="nf">elapsed_str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>        <span class="sd">&quot;&quot;&quot;Returns the currently elapsed time as a formatted string.&quot;&quot;&quot;</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span><span class="p">)</span>
 </span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a><span class="sd">        &gt;&gt;&gt; timer = Timer().start()&quot;&quot;&quot;</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="k">return</span> <span class="bp">self</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="nd">@property</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="k">def</span> <span class="nf">average_elapsed</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="sd">&quot;&quot;&quot;Returns the average elapsed time.&quot;&quot;&quot;</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span>
 </span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="k">def</span> <span class="nf">stop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="sd">&quot;&quot;&quot;Stop timer.</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a><span class="sd">        Calculates elapsed time and average elapsed time.&quot;&quot;&quot;</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_save_elapsed_time</span><span class="p">()</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">)</span> <span class="o">/</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">))</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="nd">@property</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>    <span class="k">def</span> <span class="nf">average_elapsed_str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>        <span class="sd">&quot;&quot;&quot;Returns the average elapsed time as a formatted string.&quot;&quot;&quot;</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span><span class="p">)</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>    <span class="nd">@property</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>    <span class="k">def</span> <span class="nf">start_time</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>        <span class="sd">&quot;&quot;&quot;Returns the timestamp of the last call to `start()`.&quot;&quot;&quot;</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span>
 </span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>    <span class="k">def</span> <span class="nf">_save_elapsed_time</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>        <span class="sd">&quot;&quot;&quot;Saves current elapsed time to the history buffer</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a><span class="sd">        in a FIFO manner.&quot;&quot;&quot;</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">averaging_window_length</span><span class="p">:</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span><span class="p">)</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>    <span class="k">def</span> <span class="nf">format_time</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="sd">&quot;&quot;&quot;Returns num_seconds as a string with units.</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a><span class="sd">        :param subsecond_resolution: Include milliseconds</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a><span class="sd">        and microseconds with the output.&quot;&quot;&quot;</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="n">microsecond</span> <span class="o">=</span> <span class="mf">0.000001</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>        <span class="n">millisecond</span> <span class="o">=</span> <span class="mf">0.001</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>        <span class="n">second</span> <span class="o">=</span> <span class="mi">1</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>        <span class="n">seconds_per_minute</span> <span class="o">=</span> <span class="mi">60</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>        <span class="n">seconds_per_hour</span> <span class="o">=</span> <span class="mi">3600</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>        <span class="n">seconds_per_day</span> <span class="o">=</span> <span class="mi">86400</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>        <span class="n">seconds_per_week</span> <span class="o">=</span> <span class="mi">604800</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>        <span class="n">seconds_per_month</span> <span class="o">=</span> <span class="mi">2419200</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="n">seconds_per_year</span> <span class="o">=</span> <span class="mi">29030400</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="n">time_units</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>            <span class="p">(</span><span class="n">seconds_per_year</span><span class="p">,</span> <span class="s2">&quot;y&quot;</span><span class="p">),</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>            <span class="p">(</span><span class="n">seconds_per_month</span><span class="p">,</span> <span class="s2">&quot;mn&quot;</span><span class="p">),</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>            <span class="p">(</span><span class="n">seconds_per_week</span><span class="p">,</span> <span class="s2">&quot;w&quot;</span><span class="p">),</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>            <span class="p">(</span><span class="n">seconds_per_day</span><span class="p">,</span> <span class="s2">&quot;d&quot;</span><span class="p">),</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>            <span class="p">(</span><span class="n">seconds_per_hour</span><span class="p">,</span> <span class="s2">&quot;h&quot;</span><span class="p">),</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>            <span class="p">(</span><span class="n">seconds_per_minute</span><span class="p">,</span> <span class="s2">&quot;m&quot;</span><span class="p">),</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>            <span class="p">(</span><span class="n">second</span><span class="p">,</span> <span class="s2">&quot;s&quot;</span><span class="p">),</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>            <span class="p">(</span><span class="n">millisecond</span><span class="p">,</span> <span class="s2">&quot;ms&quot;</span><span class="p">),</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>            <span class="p">(</span><span class="n">microsecond</span><span class="p">,</span> <span class="s2">&quot;us&quot;</span><span class="p">),</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>        <span class="p">]</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">subsecond_resolution</span><span class="p">:</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>            <span class="n">time_units</span> <span class="o">=</span> <span class="n">time_units</span><span class="p">[:</span><span class="o">-</span><span class="mi">2</span><span class="p">]</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>        <span class="n">time_string</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>        <span class="k">for</span> <span class="n">time_unit</span> <span class="ow">in</span> <span class="n">time_units</span><span class="p">:</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>            <span class="n">unit_amount</span><span class="p">,</span> <span class="n">num_seconds</span> <span class="o">=</span> <span class="nb">divmod</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">,</span> <span class="n">time_unit</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>            <span class="k">if</span> <span class="n">unit_amount</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>                <span class="n">time_string</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">int</span><span class="p">(</span><span class="n">unit_amount</span><span class="p">)</span><span class="si">}{</span><span class="n">time_unit</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2"> &quot;</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>        <span class="k">if</span> <span class="n">time_string</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>            <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;&lt;1</span><span class="si">{</span><span class="n">time_units</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">][</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>        <span class="k">return</span> <span class="n">time_string</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>    <span class="nd">@property</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>    <span class="k">def</span> <span class="nf">stats</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>        <span class="sd">&quot;&quot;&quot;Returns a string stating the currently elapsed time</span>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a><span class="sd">        and the average elapsed time.&quot;&quot;&quot;</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="se">\n</span><span class="s2">average elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">average_elapsed_str</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>    <span class="nd">@property</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="k">def</span> <span class="nf">stop_time</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>        <span class="sd">&quot;&quot;&quot;Returns the timestamp of the last call to `stop()`.&quot;&quot;&quot;</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>    <span class="nd">@property</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>    <span class="k">def</span> <span class="nf">history</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">float</span><span class="p">]:</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="sd">&quot;&quot;&quot;Returns the history buffer for this timer.</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a><span class="sd">        At most, it will be `averaging_window_length` elements long.&quot;&quot;&quot;</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_history</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>    <span class="k">def</span> <span class="nf">start</span><span class="p">(</span><span class="bp">self</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="sd">&quot;&quot;&quot;Start the timer.</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="sd">        Returns this Timer instance so timer start can be chained to Timer creation if desired.</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a><span class="sd">        &gt;&gt;&gt; timer = Timer().start()&quot;&quot;&quot;</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">started</span><span class="p">:</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_started</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="k">return</span> <span class="bp">self</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>    <span class="k">def</span> <span class="nf">stop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="sd">&quot;&quot;&quot;Stop the timer.</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a><span class="sd">        Calculates elapsed time and average elapsed time.&quot;&quot;&quot;</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">started</span><span class="p">:</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_started</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span> <span class="o">=</span> <span class="p">(</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_pauser</span><span class="o">.</span><span class="n">pause_total</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>            <span class="p">)</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_pauser</span><span class="o">.</span><span class="n">reset</span><span class="p">()</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_save_elapsed_time</span><span class="p">()</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">)</span> <span class="o">/</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">))</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>    <span class="k">def</span> <span class="nf">pause</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>        <span class="sd">&quot;&quot;&quot;Pause the timer.&quot;&quot;&quot;</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_pauser</span><span class="o">.</span><span class="n">pause</span><span class="p">()</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>    <span class="k">def</span> <span class="nf">unpause</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>        <span class="sd">&quot;&quot;&quot;Unpause the timer.&quot;&quot;&quot;</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_pauser</span><span class="o">.</span><span class="n">unpause</span><span class="p">()</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>    <span class="k">def</span> <span class="nf">_save_elapsed_time</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>        <span class="sd">&quot;&quot;&quot;Saves current elapsed time to the history buffer in a FIFO manner.&quot;&quot;&quot;</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">averaging_window_length</span><span class="p">:</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span><span class="p">)</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>    <span class="k">def</span> <span class="nf">format_time</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>        <span class="sd">&quot;&quot;&quot;Returns `num_seconds` as a string with units.</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a><span class="sd">        `subsecond_resolution`: Include milliseconds and microseconds with the output.&quot;&quot;&quot;</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>        <span class="n">microsecond</span> <span class="o">=</span> <span class="mf">0.000001</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>        <span class="n">millisecond</span> <span class="o">=</span> <span class="mf">0.001</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>        <span class="n">second</span> <span class="o">=</span> <span class="mi">1</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>        <span class="n">seconds_per_minute</span> <span class="o">=</span> <span class="mi">60</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>        <span class="n">seconds_per_hour</span> <span class="o">=</span> <span class="mi">3600</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="n">seconds_per_day</span> <span class="o">=</span> <span class="mi">86400</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>        <span class="n">seconds_per_week</span> <span class="o">=</span> <span class="mi">604800</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>        <span class="n">seconds_per_month</span> <span class="o">=</span> <span class="mi">2419200</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>        <span class="n">seconds_per_year</span> <span class="o">=</span> <span class="mi">29030400</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>        <span class="n">time_units</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>            <span class="p">(</span><span class="n">seconds_per_year</span><span class="p">,</span> <span class="s2">&quot;y&quot;</span><span class="p">),</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>            <span class="p">(</span><span class="n">seconds_per_month</span><span class="p">,</span> <span class="s2">&quot;mn&quot;</span><span class="p">),</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>            <span class="p">(</span><span class="n">seconds_per_week</span><span class="p">,</span> <span class="s2">&quot;w&quot;</span><span class="p">),</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>            <span class="p">(</span><span class="n">seconds_per_day</span><span class="p">,</span> <span class="s2">&quot;d&quot;</span><span class="p">),</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>            <span class="p">(</span><span class="n">seconds_per_hour</span><span class="p">,</span> <span class="s2">&quot;h&quot;</span><span class="p">),</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>            <span class="p">(</span><span class="n">seconds_per_minute</span><span class="p">,</span> <span class="s2">&quot;m&quot;</span><span class="p">),</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>            <span class="p">(</span><span class="n">second</span><span class="p">,</span> <span class="s2">&quot;s&quot;</span><span class="p">),</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>            <span class="p">(</span><span class="n">millisecond</span><span class="p">,</span> <span class="s2">&quot;ms&quot;</span><span class="p">),</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>            <span class="p">(</span><span class="n">microsecond</span><span class="p">,</span> <span class="s2">&quot;us&quot;</span><span class="p">),</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="p">]</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">subsecond_resolution</span><span class="p">:</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>            <span class="n">time_units</span> <span class="o">=</span> <span class="n">time_units</span><span class="p">[:</span><span class="o">-</span><span class="mi">2</span><span class="p">]</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="n">time_string</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="k">for</span> <span class="n">time_unit</span> <span class="ow">in</span> <span class="n">time_units</span><span class="p">:</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>            <span class="n">unit_amount</span><span class="p">,</span> <span class="n">num_seconds</span> <span class="o">=</span> <span class="nb">divmod</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">,</span> <span class="n">time_unit</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>            <span class="k">if</span> <span class="n">unit_amount</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>                <span class="n">time_string</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">int</span><span class="p">(</span><span class="n">unit_amount</span><span class="p">)</span><span class="si">}{</span><span class="n">time_unit</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2"> &quot;</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="k">if</span> <span class="n">time_string</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>            <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;&lt;1</span><span class="si">{</span><span class="n">time_units</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">][</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="k">return</span> <span class="n">time_string</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>    <span class="nd">@property</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>    <span class="k">def</span> <span class="nf">stats</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>        <span class="sd">&quot;&quot;&quot;Returns a string stating the currently elapsed time and the average elapsed time.&quot;&quot;&quot;</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="se">\n</span><span class="s2">average elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">average_elapsed_str</span><span class="si">}</span><span class="s2">&quot;</span>
 </span></pre></div>
 
 
             </section>
                 <section id="time_it">
                             <input id="time_it-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -259,20 +324,20 @@
         <span class="name">time_it</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">loops</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">1</span></span><span class="return-annotation">) -> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="time_it-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#time_it"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="time_it-8"><a href="#time_it-8"><span class="linenos"> 8</span></a><span class="k">def</span> <span class="nf">time_it</span><span class="p">(</span><span class="n">loops</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">1</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">]:</span>
-</span><span id="time_it-9"><a href="#time_it-9"><span class="linenos"> 9</span></a>    <span class="sd">&quot;&quot;&quot;Decorator to time function execution time</span>
-</span><span id="time_it-10"><a href="#time_it-10"><span class="linenos">10</span></a><span class="sd">    and print the results.</span>
-</span><span id="time_it-11"><a href="#time_it-11"><span class="linenos">11</span></a>
-</span><span id="time_it-12"><a href="#time_it-12"><span class="linenos">12</span></a><span class="sd">    :param loops: How many times to loop the function,</span>
-</span><span id="time_it-13"><a href="#time_it-13"><span class="linenos">13</span></a><span class="sd">    starting and stopping the timer before and after</span>
-</span><span id="time_it-14"><a href="#time_it-14"><span class="linenos">14</span></a><span class="sd">    each loop.&quot;&quot;&quot;</span>
+</span><span id="time_it-9"><a href="#time_it-9"><span class="linenos"> 9</span></a>    <span class="sd">&quot;&quot;&quot;Decorator to time function execution time and print the results.</span>
+</span><span id="time_it-10"><a href="#time_it-10"><span class="linenos">10</span></a>
+</span><span id="time_it-11"><a href="#time_it-11"><span class="linenos">11</span></a><span class="sd">    #### :params:</span>
+</span><span id="time_it-12"><a href="#time_it-12"><span class="linenos">12</span></a>
+</span><span id="time_it-13"><a href="#time_it-13"><span class="linenos">13</span></a><span class="sd">    `loops`: How many times to execute the decorated function,</span>
+</span><span id="time_it-14"><a href="#time_it-14"><span class="linenos">14</span></a><span class="sd">    starting and stopping the timer before and after each loop.&quot;&quot;&quot;</span>
 </span><span id="time_it-15"><a href="#time_it-15"><span class="linenos">15</span></a>
 </span><span id="time_it-16"><a href="#time_it-16"><span class="linenos">16</span></a>    <span class="k">def</span> <span class="nf">decorator</span><span class="p">(</span><span class="n">func</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">]:</span>
 </span><span id="time_it-17"><a href="#time_it-17"><span class="linenos">17</span></a>        <span class="k">def</span> <span class="nf">wrapper</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
 </span><span id="time_it-18"><a href="#time_it-18"><span class="linenos">18</span></a>            <span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">loops</span><span class="p">)</span>
 </span><span id="time_it-19"><a href="#time_it-19"><span class="linenos">19</span></a>            <span class="n">result</span> <span class="o">=</span> <span class="kc">None</span>
 </span><span id="time_it-20"><a href="#time_it-20"><span class="linenos">20</span></a>            <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">loops</span><span class="p">):</span>
 </span><span id="time_it-21"><a href="#time_it-21"><span class="linenos">21</span></a>                <span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
@@ -285,24 +350,20 @@
 </span><span id="time_it-28"><a href="#time_it-28"><span class="linenos">28</span></a>
 </span><span id="time_it-29"><a href="#time_it-29"><span class="linenos">29</span></a>        <span class="k">return</span> <span class="n">wrapper</span>
 </span><span id="time_it-30"><a href="#time_it-30"><span class="linenos">30</span></a>
 </span><span id="time_it-31"><a href="#time_it-31"><span class="linenos">31</span></a>    <span class="k">return</span> <span class="n">decorator</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Decorator to time function execution time
-and print the results.</p>
+            <div class="docstring"><p>Decorator to time function execution time and print the results.</p>
 
-<h6 id="parameters">Parameters</h6>
+<h4 id="params">:params:</h4>
 
-<ul>
-<li><strong>loops</strong>:  How many times to loop the function,
-starting and stopping the timer before and after
-each loop.</li>
-</ul>
+<p><code>loops</code>: How many times to execute the decorated function,
+starting and stopping the timer before and after each loop.</p>
 </div>
 
 
                 </section>
                 <section id="Timer">
                             <input id="Timer-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
@@ -310,231 +371,312 @@
     <span class="def">class</span>
     <span class="name">Timer</span>:
 
                 <label class="view-source-button" for="Timer-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Timer"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer-34"><a href="#Timer-34"><span class="linenos"> 34</span></a><span class="k">class</span> <span class="nc">Timer</span><span class="p">:</span>
-</span><span id="Timer-35"><a href="#Timer-35"><span class="linenos"> 35</span></a>    <span class="sd">&quot;&quot;&quot;Simple timer class that tracks total elapsed time</span>
-</span><span id="Timer-36"><a href="#Timer-36"><span class="linenos"> 36</span></a><span class="sd">    and average time between calls to &#39;start&#39; and &#39;stop&#39;.&quot;&quot;&quot;</span>
-</span><span id="Timer-37"><a href="#Timer-37"><span class="linenos"> 37</span></a>
-</span><span id="Timer-38"><a href="#Timer-38"><span class="linenos"> 38</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="Timer-39"><a href="#Timer-39"><span class="linenos"> 39</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">10</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="Timer-40"><a href="#Timer-40"><span class="linenos"> 40</span></a>    <span class="p">):</span>
-</span><span id="Timer-41"><a href="#Timer-41"><span class="linenos"> 41</span></a>        <span class="sd">&quot;&quot;&quot;:param averaging_window_length: Number of start/stop cycles</span>
-</span><span id="Timer-42"><a href="#Timer-42"><span class="linenos"> 42</span></a><span class="sd">        to calculate the average elapsed time with.</span>
-</span><span id="Timer-43"><a href="#Timer-43"><span class="linenos"> 43</span></a>
-</span><span id="Timer-44"><a href="#Timer-44"><span class="linenos"> 44</span></a><span class="sd">        :param subsecond_resolution: Whether to print formatted time</span>
-</span><span id="Timer-45"><a href="#Timer-45"><span class="linenos"> 45</span></a><span class="sd">        strings with subsecond resolution or not.&quot;&quot;&quot;</span>
-</span><span id="Timer-46"><a href="#Timer-46"><span class="linenos"> 46</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
-</span><span id="Timer-47"><a href="#Timer-47"><span class="linenos"> 47</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span>
-</span><span id="Timer-48"><a href="#Timer-48"><span class="linenos"> 48</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="Timer-49"><a href="#Timer-49"><span class="linenos"> 49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="Timer-50"><a href="#Timer-50"><span class="linenos"> 50</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="Timer-51"><a href="#Timer-51"><span class="linenos"> 51</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="Timer-52"><a href="#Timer-52"><span class="linenos"> 52</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="n">averaging_window_length</span>
-</span><span id="Timer-53"><a href="#Timer-53"><span class="linenos"> 53</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span> <span class="o">=</span> <span class="n">subsecond_resolution</span>
-</span><span id="Timer-54"><a href="#Timer-54"><span class="linenos"> 54</span></a>
-</span><span id="Timer-55"><a href="#Timer-55"><span class="linenos"> 55</span></a>    <span class="nd">@property</span>
-</span><span id="Timer-56"><a href="#Timer-56"><span class="linenos"> 56</span></a>    <span class="k">def</span> <span class="nf">started</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Timer-57"><a href="#Timer-57"><span class="linenos"> 57</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether the timer has</span>
-</span><span id="Timer-58"><a href="#Timer-58"><span class="linenos"> 58</span></a><span class="sd">        been started and is currently running.&quot;&quot;&quot;</span>
-</span><span id="Timer-59"><a href="#Timer-59"><span class="linenos"> 59</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_started</span>
-</span><span id="Timer-60"><a href="#Timer-60"><span class="linenos"> 60</span></a>
-</span><span id="Timer-61"><a href="#Timer-61"><span class="linenos"> 61</span></a>    <span class="nd">@property</span>
-</span><span id="Timer-62"><a href="#Timer-62"><span class="linenos"> 62</span></a>    <span class="k">def</span> <span class="nf">elapsed</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
-</span><span id="Timer-63"><a href="#Timer-63"><span class="linenos"> 63</span></a>        <span class="sd">&quot;&quot;&quot;Return the currently elapsed time.&quot;&quot;&quot;</span>
-</span><span id="Timer-64"><a href="#Timer-64"><span class="linenos"> 64</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_started</span><span class="p">:</span>
-</span><span id="Timer-65"><a href="#Timer-65"><span class="linenos"> 65</span></a>            <span class="k">return</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span>
-</span><span id="Timer-66"><a href="#Timer-66"><span class="linenos"> 66</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Timer-67"><a href="#Timer-67"><span class="linenos"> 67</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span>
-</span><span id="Timer-68"><a href="#Timer-68"><span class="linenos"> 68</span></a>
-</span><span id="Timer-69"><a href="#Timer-69"><span class="linenos"> 69</span></a>    <span class="nd">@property</span>
-</span><span id="Timer-70"><a href="#Timer-70"><span class="linenos"> 70</span></a>    <span class="k">def</span> <span class="nf">elapsed_str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Timer-71"><a href="#Timer-71"><span class="linenos"> 71</span></a>        <span class="sd">&quot;&quot;&quot;Return the currently elapsed time</span>
-</span><span id="Timer-72"><a href="#Timer-72"><span class="linenos"> 72</span></a><span class="sd">        as a formatted string.&quot;&quot;&quot;</span>
-</span><span id="Timer-73"><a href="#Timer-73"><span class="linenos"> 73</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span><span class="p">)</span>
-</span><span id="Timer-74"><a href="#Timer-74"><span class="linenos"> 74</span></a>
-</span><span id="Timer-75"><a href="#Timer-75"><span class="linenos"> 75</span></a>    <span class="nd">@property</span>
-</span><span id="Timer-76"><a href="#Timer-76"><span class="linenos"> 76</span></a>    <span class="k">def</span> <span class="nf">average_elapsed</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
-</span><span id="Timer-77"><a href="#Timer-77"><span class="linenos"> 77</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span>
-</span><span id="Timer-78"><a href="#Timer-78"><span class="linenos"> 78</span></a>
-</span><span id="Timer-79"><a href="#Timer-79"><span class="linenos"> 79</span></a>    <span class="nd">@property</span>
-</span><span id="Timer-80"><a href="#Timer-80"><span class="linenos"> 80</span></a>    <span class="k">def</span> <span class="nf">average_elapsed_str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Timer-81"><a href="#Timer-81"><span class="linenos"> 81</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer-61"><a href="#Timer-61"><span class="linenos"> 61</span></a><span class="k">class</span> <span class="nc">Timer</span><span class="p">:</span>
+</span><span id="Timer-62"><a href="#Timer-62"><span class="linenos"> 62</span></a>    <span class="sd">&quot;&quot;&quot;Simple timer class that tracks total elapsed time</span>
+</span><span id="Timer-63"><a href="#Timer-63"><span class="linenos"> 63</span></a><span class="sd">    and average time between calls to `start()` and `stop()`.&quot;&quot;&quot;</span>
+</span><span id="Timer-64"><a href="#Timer-64"><span class="linenos"> 64</span></a>
+</span><span id="Timer-65"><a href="#Timer-65"><span class="linenos"> 65</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="Timer-66"><a href="#Timer-66"><span class="linenos"> 66</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">10</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="Timer-67"><a href="#Timer-67"><span class="linenos"> 67</span></a>    <span class="p">):</span>
+</span><span id="Timer-68"><a href="#Timer-68"><span class="linenos"> 68</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="Timer-69"><a href="#Timer-69"><span class="linenos"> 69</span></a><span class="sd">        #### :params:</span>
+</span><span id="Timer-70"><a href="#Timer-70"><span class="linenos"> 70</span></a><span class="sd">        * `averaging_window_length`: Number of start/stop cycles to calculate the average elapsed time with.</span>
+</span><span id="Timer-71"><a href="#Timer-71"><span class="linenos"> 71</span></a>
+</span><span id="Timer-72"><a href="#Timer-72"><span class="linenos"> 72</span></a><span class="sd">        * `subsecond_resolution`: Whether to print formatted time strings with subsecond resolution or not.&quot;&quot;&quot;</span>
+</span><span id="Timer-73"><a href="#Timer-73"><span class="linenos"> 73</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="Timer-74"><a href="#Timer-74"><span class="linenos"> 74</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span>
+</span><span id="Timer-75"><a href="#Timer-75"><span class="linenos"> 75</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="Timer-76"><a href="#Timer-76"><span class="linenos"> 76</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="Timer-77"><a href="#Timer-77"><span class="linenos"> 77</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Timer-78"><a href="#Timer-78"><span class="linenos"> 78</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="Timer-79"><a href="#Timer-79"><span class="linenos"> 79</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="n">averaging_window_length</span>
+</span><span id="Timer-80"><a href="#Timer-80"><span class="linenos"> 80</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span> <span class="o">=</span> <span class="n">subsecond_resolution</span>
+</span><span id="Timer-81"><a href="#Timer-81"><span class="linenos"> 81</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_pauser</span> <span class="o">=</span> <span class="n">_Pauser</span><span class="p">()</span>
 </span><span id="Timer-82"><a href="#Timer-82"><span class="linenos"> 82</span></a>
 </span><span id="Timer-83"><a href="#Timer-83"><span class="linenos"> 83</span></a>    <span class="nd">@property</span>
-</span><span id="Timer-84"><a href="#Timer-84"><span class="linenos"> 84</span></a>    <span class="k">def</span> <span class="nf">start_time</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
-</span><span id="Timer-85"><a href="#Timer-85"><span class="linenos"> 85</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span>
-</span><span id="Timer-86"><a href="#Timer-86"><span class="linenos"> 86</span></a>
-</span><span id="Timer-87"><a href="#Timer-87"><span class="linenos"> 87</span></a>    <span class="nd">@property</span>
-</span><span id="Timer-88"><a href="#Timer-88"><span class="linenos"> 88</span></a>    <span class="k">def</span> <span class="nf">stop_time</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
-</span><span id="Timer-89"><a href="#Timer-89"><span class="linenos"> 89</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span>
-</span><span id="Timer-90"><a href="#Timer-90"><span class="linenos"> 90</span></a>
-</span><span id="Timer-91"><a href="#Timer-91"><span class="linenos"> 91</span></a>    <span class="nd">@property</span>
-</span><span id="Timer-92"><a href="#Timer-92"><span class="linenos"> 92</span></a>    <span class="k">def</span> <span class="nf">history</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">float</span><span class="p">]:</span>
-</span><span id="Timer-93"><a href="#Timer-93"><span class="linenos"> 93</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_history</span>
-</span><span id="Timer-94"><a href="#Timer-94"><span class="linenos"> 94</span></a>
-</span><span id="Timer-95"><a href="#Timer-95"><span class="linenos"> 95</span></a>    <span class="k">def</span> <span class="nf">start</span><span class="p">(</span><span class="bp">self</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Timer-96"><a href="#Timer-96"><span class="linenos"> 96</span></a>        <span class="sd">&quot;&quot;&quot;Start timer.</span>
-</span><span id="Timer-97"><a href="#Timer-97"><span class="linenos"> 97</span></a><span class="sd">        Returns this Timer instance so</span>
-</span><span id="Timer-98"><a href="#Timer-98"><span class="linenos"> 98</span></a><span class="sd">        timer start can be chained to</span>
-</span><span id="Timer-99"><a href="#Timer-99"><span class="linenos"> 99</span></a><span class="sd">        Timer creation.</span>
+</span><span id="Timer-84"><a href="#Timer-84"><span class="linenos"> 84</span></a>    <span class="k">def</span> <span class="nf">started</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Timer-85"><a href="#Timer-85"><span class="linenos"> 85</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether the timer has been started and is currently running.&quot;&quot;&quot;</span>
+</span><span id="Timer-86"><a href="#Timer-86"><span class="linenos"> 86</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_started</span>
+</span><span id="Timer-87"><a href="#Timer-87"><span class="linenos"> 87</span></a>
+</span><span id="Timer-88"><a href="#Timer-88"><span class="linenos"> 88</span></a>    <span class="nd">@property</span>
+</span><span id="Timer-89"><a href="#Timer-89"><span class="linenos"> 89</span></a>    <span class="k">def</span> <span class="nf">elapsed</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="Timer-90"><a href="#Timer-90"><span class="linenos"> 90</span></a>        <span class="sd">&quot;&quot;&quot;Returns the currently elapsed time.&quot;&quot;&quot;</span>
+</span><span id="Timer-91"><a href="#Timer-91"><span class="linenos"> 91</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_started</span><span class="p">:</span>
+</span><span id="Timer-92"><a href="#Timer-92"><span class="linenos"> 92</span></a>            <span class="k">return</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_pauser</span><span class="o">.</span><span class="n">pause_total</span>
+</span><span id="Timer-93"><a href="#Timer-93"><span class="linenos"> 93</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="Timer-94"><a href="#Timer-94"><span class="linenos"> 94</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span>
+</span><span id="Timer-95"><a href="#Timer-95"><span class="linenos"> 95</span></a>
+</span><span id="Timer-96"><a href="#Timer-96"><span class="linenos"> 96</span></a>    <span class="nd">@property</span>
+</span><span id="Timer-97"><a href="#Timer-97"><span class="linenos"> 97</span></a>    <span class="k">def</span> <span class="nf">elapsed_str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Timer-98"><a href="#Timer-98"><span class="linenos"> 98</span></a>        <span class="sd">&quot;&quot;&quot;Returns the currently elapsed time as a formatted string.&quot;&quot;&quot;</span>
+</span><span id="Timer-99"><a href="#Timer-99"><span class="linenos"> 99</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span><span class="p">)</span>
 </span><span id="Timer-100"><a href="#Timer-100"><span class="linenos">100</span></a>
-</span><span id="Timer-101"><a href="#Timer-101"><span class="linenos">101</span></a><span class="sd">        &gt;&gt;&gt; timer = Timer().start()&quot;&quot;&quot;</span>
-</span><span id="Timer-102"><a href="#Timer-102"><span class="linenos">102</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
-</span><span id="Timer-103"><a href="#Timer-103"><span class="linenos">103</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="Timer-104"><a href="#Timer-104"><span class="linenos">104</span></a>        <span class="k">return</span> <span class="bp">self</span>
+</span><span id="Timer-101"><a href="#Timer-101"><span class="linenos">101</span></a>    <span class="nd">@property</span>
+</span><span id="Timer-102"><a href="#Timer-102"><span class="linenos">102</span></a>    <span class="k">def</span> <span class="nf">average_elapsed</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="Timer-103"><a href="#Timer-103"><span class="linenos">103</span></a>        <span class="sd">&quot;&quot;&quot;Returns the average elapsed time.&quot;&quot;&quot;</span>
+</span><span id="Timer-104"><a href="#Timer-104"><span class="linenos">104</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span>
 </span><span id="Timer-105"><a href="#Timer-105"><span class="linenos">105</span></a>
-</span><span id="Timer-106"><a href="#Timer-106"><span class="linenos">106</span></a>    <span class="k">def</span> <span class="nf">stop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Timer-107"><a href="#Timer-107"><span class="linenos">107</span></a>        <span class="sd">&quot;&quot;&quot;Stop timer.</span>
-</span><span id="Timer-108"><a href="#Timer-108"><span class="linenos">108</span></a>
-</span><span id="Timer-109"><a href="#Timer-109"><span class="linenos">109</span></a><span class="sd">        Calculates elapsed time and average elapsed time.&quot;&quot;&quot;</span>
-</span><span id="Timer-110"><a href="#Timer-110"><span class="linenos">110</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
-</span><span id="Timer-111"><a href="#Timer-111"><span class="linenos">111</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="Timer-112"><a href="#Timer-112"><span class="linenos">112</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span>
-</span><span id="Timer-113"><a href="#Timer-113"><span class="linenos">113</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_save_elapsed_time</span><span class="p">()</span>
-</span><span id="Timer-114"><a href="#Timer-114"><span class="linenos">114</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">)</span> <span class="o">/</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">))</span>
+</span><span id="Timer-106"><a href="#Timer-106"><span class="linenos">106</span></a>    <span class="nd">@property</span>
+</span><span id="Timer-107"><a href="#Timer-107"><span class="linenos">107</span></a>    <span class="k">def</span> <span class="nf">average_elapsed_str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Timer-108"><a href="#Timer-108"><span class="linenos">108</span></a>        <span class="sd">&quot;&quot;&quot;Returns the average elapsed time as a formatted string.&quot;&quot;&quot;</span>
+</span><span id="Timer-109"><a href="#Timer-109"><span class="linenos">109</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span><span class="p">)</span>
+</span><span id="Timer-110"><a href="#Timer-110"><span class="linenos">110</span></a>
+</span><span id="Timer-111"><a href="#Timer-111"><span class="linenos">111</span></a>    <span class="nd">@property</span>
+</span><span id="Timer-112"><a href="#Timer-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">start_time</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="Timer-113"><a href="#Timer-113"><span class="linenos">113</span></a>        <span class="sd">&quot;&quot;&quot;Returns the timestamp of the last call to `start()`.&quot;&quot;&quot;</span>
+</span><span id="Timer-114"><a href="#Timer-114"><span class="linenos">114</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span>
 </span><span id="Timer-115"><a href="#Timer-115"><span class="linenos">115</span></a>
-</span><span id="Timer-116"><a href="#Timer-116"><span class="linenos">116</span></a>    <span class="k">def</span> <span class="nf">_save_elapsed_time</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Timer-117"><a href="#Timer-117"><span class="linenos">117</span></a>        <span class="sd">&quot;&quot;&quot;Saves current elapsed time to the history buffer</span>
-</span><span id="Timer-118"><a href="#Timer-118"><span class="linenos">118</span></a><span class="sd">        in a FIFO manner.&quot;&quot;&quot;</span>
-</span><span id="Timer-119"><a href="#Timer-119"><span class="linenos">119</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">averaging_window_length</span><span class="p">:</span>
-</span><span id="Timer-120"><a href="#Timer-120"><span class="linenos">120</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="Timer-121"><a href="#Timer-121"><span class="linenos">121</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span><span class="p">)</span>
-</span><span id="Timer-122"><a href="#Timer-122"><span class="linenos">122</span></a>
-</span><span id="Timer-123"><a href="#Timer-123"><span class="linenos">123</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="Timer-124"><a href="#Timer-124"><span class="linenos">124</span></a>    <span class="k">def</span> <span class="nf">format_time</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Timer-125"><a href="#Timer-125"><span class="linenos">125</span></a>        <span class="sd">&quot;&quot;&quot;Returns num_seconds as a string with units.</span>
-</span><span id="Timer-126"><a href="#Timer-126"><span class="linenos">126</span></a>
-</span><span id="Timer-127"><a href="#Timer-127"><span class="linenos">127</span></a><span class="sd">        :param subsecond_resolution: Include milliseconds</span>
-</span><span id="Timer-128"><a href="#Timer-128"><span class="linenos">128</span></a><span class="sd">        and microseconds with the output.&quot;&quot;&quot;</span>
-</span><span id="Timer-129"><a href="#Timer-129"><span class="linenos">129</span></a>        <span class="n">microsecond</span> <span class="o">=</span> <span class="mf">0.000001</span>
-</span><span id="Timer-130"><a href="#Timer-130"><span class="linenos">130</span></a>        <span class="n">millisecond</span> <span class="o">=</span> <span class="mf">0.001</span>
-</span><span id="Timer-131"><a href="#Timer-131"><span class="linenos">131</span></a>        <span class="n">second</span> <span class="o">=</span> <span class="mi">1</span>
-</span><span id="Timer-132"><a href="#Timer-132"><span class="linenos">132</span></a>        <span class="n">seconds_per_minute</span> <span class="o">=</span> <span class="mi">60</span>
-</span><span id="Timer-133"><a href="#Timer-133"><span class="linenos">133</span></a>        <span class="n">seconds_per_hour</span> <span class="o">=</span> <span class="mi">3600</span>
-</span><span id="Timer-134"><a href="#Timer-134"><span class="linenos">134</span></a>        <span class="n">seconds_per_day</span> <span class="o">=</span> <span class="mi">86400</span>
-</span><span id="Timer-135"><a href="#Timer-135"><span class="linenos">135</span></a>        <span class="n">seconds_per_week</span> <span class="o">=</span> <span class="mi">604800</span>
-</span><span id="Timer-136"><a href="#Timer-136"><span class="linenos">136</span></a>        <span class="n">seconds_per_month</span> <span class="o">=</span> <span class="mi">2419200</span>
-</span><span id="Timer-137"><a href="#Timer-137"><span class="linenos">137</span></a>        <span class="n">seconds_per_year</span> <span class="o">=</span> <span class="mi">29030400</span>
-</span><span id="Timer-138"><a href="#Timer-138"><span class="linenos">138</span></a>        <span class="n">time_units</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Timer-139"><a href="#Timer-139"><span class="linenos">139</span></a>            <span class="p">(</span><span class="n">seconds_per_year</span><span class="p">,</span> <span class="s2">&quot;y&quot;</span><span class="p">),</span>
-</span><span id="Timer-140"><a href="#Timer-140"><span class="linenos">140</span></a>            <span class="p">(</span><span class="n">seconds_per_month</span><span class="p">,</span> <span class="s2">&quot;mn&quot;</span><span class="p">),</span>
-</span><span id="Timer-141"><a href="#Timer-141"><span class="linenos">141</span></a>            <span class="p">(</span><span class="n">seconds_per_week</span><span class="p">,</span> <span class="s2">&quot;w&quot;</span><span class="p">),</span>
-</span><span id="Timer-142"><a href="#Timer-142"><span class="linenos">142</span></a>            <span class="p">(</span><span class="n">seconds_per_day</span><span class="p">,</span> <span class="s2">&quot;d&quot;</span><span class="p">),</span>
-</span><span id="Timer-143"><a href="#Timer-143"><span class="linenos">143</span></a>            <span class="p">(</span><span class="n">seconds_per_hour</span><span class="p">,</span> <span class="s2">&quot;h&quot;</span><span class="p">),</span>
-</span><span id="Timer-144"><a href="#Timer-144"><span class="linenos">144</span></a>            <span class="p">(</span><span class="n">seconds_per_minute</span><span class="p">,</span> <span class="s2">&quot;m&quot;</span><span class="p">),</span>
-</span><span id="Timer-145"><a href="#Timer-145"><span class="linenos">145</span></a>            <span class="p">(</span><span class="n">second</span><span class="p">,</span> <span class="s2">&quot;s&quot;</span><span class="p">),</span>
-</span><span id="Timer-146"><a href="#Timer-146"><span class="linenos">146</span></a>            <span class="p">(</span><span class="n">millisecond</span><span class="p">,</span> <span class="s2">&quot;ms&quot;</span><span class="p">),</span>
-</span><span id="Timer-147"><a href="#Timer-147"><span class="linenos">147</span></a>            <span class="p">(</span><span class="n">microsecond</span><span class="p">,</span> <span class="s2">&quot;us&quot;</span><span class="p">),</span>
-</span><span id="Timer-148"><a href="#Timer-148"><span class="linenos">148</span></a>        <span class="p">]</span>
-</span><span id="Timer-149"><a href="#Timer-149"><span class="linenos">149</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">subsecond_resolution</span><span class="p">:</span>
-</span><span id="Timer-150"><a href="#Timer-150"><span class="linenos">150</span></a>            <span class="n">time_units</span> <span class="o">=</span> <span class="n">time_units</span><span class="p">[:</span><span class="o">-</span><span class="mi">2</span><span class="p">]</span>
-</span><span id="Timer-151"><a href="#Timer-151"><span class="linenos">151</span></a>        <span class="n">time_string</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="Timer-152"><a href="#Timer-152"><span class="linenos">152</span></a>        <span class="k">for</span> <span class="n">time_unit</span> <span class="ow">in</span> <span class="n">time_units</span><span class="p">:</span>
-</span><span id="Timer-153"><a href="#Timer-153"><span class="linenos">153</span></a>            <span class="n">unit_amount</span><span class="p">,</span> <span class="n">num_seconds</span> <span class="o">=</span> <span class="nb">divmod</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">,</span> <span class="n">time_unit</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
-</span><span id="Timer-154"><a href="#Timer-154"><span class="linenos">154</span></a>            <span class="k">if</span> <span class="n">unit_amount</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="Timer-155"><a href="#Timer-155"><span class="linenos">155</span></a>                <span class="n">time_string</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">int</span><span class="p">(</span><span class="n">unit_amount</span><span class="p">)</span><span class="si">}{</span><span class="n">time_unit</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2"> &quot;</span>
-</span><span id="Timer-156"><a href="#Timer-156"><span class="linenos">156</span></a>        <span class="k">if</span> <span class="n">time_string</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
-</span><span id="Timer-157"><a href="#Timer-157"><span class="linenos">157</span></a>            <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;&lt;1</span><span class="si">{</span><span class="n">time_units</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">][</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="Timer-158"><a href="#Timer-158"><span class="linenos">158</span></a>        <span class="k">return</span> <span class="n">time_string</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="Timer-159"><a href="#Timer-159"><span class="linenos">159</span></a>
-</span><span id="Timer-160"><a href="#Timer-160"><span class="linenos">160</span></a>    <span class="nd">@property</span>
-</span><span id="Timer-161"><a href="#Timer-161"><span class="linenos">161</span></a>    <span class="k">def</span> <span class="nf">stats</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Timer-162"><a href="#Timer-162"><span class="linenos">162</span></a>        <span class="sd">&quot;&quot;&quot;Returns a string stating the currently elapsed time</span>
-</span><span id="Timer-163"><a href="#Timer-163"><span class="linenos">163</span></a><span class="sd">        and the average elapsed time.&quot;&quot;&quot;</span>
-</span><span id="Timer-164"><a href="#Timer-164"><span class="linenos">164</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="se">\n</span><span class="s2">average elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">average_elapsed_str</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="Timer-116"><a href="#Timer-116"><span class="linenos">116</span></a>    <span class="nd">@property</span>
+</span><span id="Timer-117"><a href="#Timer-117"><span class="linenos">117</span></a>    <span class="k">def</span> <span class="nf">stop_time</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="Timer-118"><a href="#Timer-118"><span class="linenos">118</span></a>        <span class="sd">&quot;&quot;&quot;Returns the timestamp of the last call to `stop()`.&quot;&quot;&quot;</span>
+</span><span id="Timer-119"><a href="#Timer-119"><span class="linenos">119</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span>
+</span><span id="Timer-120"><a href="#Timer-120"><span class="linenos">120</span></a>
+</span><span id="Timer-121"><a href="#Timer-121"><span class="linenos">121</span></a>    <span class="nd">@property</span>
+</span><span id="Timer-122"><a href="#Timer-122"><span class="linenos">122</span></a>    <span class="k">def</span> <span class="nf">history</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">float</span><span class="p">]:</span>
+</span><span id="Timer-123"><a href="#Timer-123"><span class="linenos">123</span></a>        <span class="sd">&quot;&quot;&quot;Returns the history buffer for this timer.</span>
+</span><span id="Timer-124"><a href="#Timer-124"><span class="linenos">124</span></a>
+</span><span id="Timer-125"><a href="#Timer-125"><span class="linenos">125</span></a><span class="sd">        At most, it will be `averaging_window_length` elements long.&quot;&quot;&quot;</span>
+</span><span id="Timer-126"><a href="#Timer-126"><span class="linenos">126</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_history</span>
+</span><span id="Timer-127"><a href="#Timer-127"><span class="linenos">127</span></a>
+</span><span id="Timer-128"><a href="#Timer-128"><span class="linenos">128</span></a>    <span class="k">def</span> <span class="nf">start</span><span class="p">(</span><span class="bp">self</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Timer-129"><a href="#Timer-129"><span class="linenos">129</span></a>        <span class="sd">&quot;&quot;&quot;Start the timer.</span>
+</span><span id="Timer-130"><a href="#Timer-130"><span class="linenos">130</span></a>
+</span><span id="Timer-131"><a href="#Timer-131"><span class="linenos">131</span></a><span class="sd">        Returns this Timer instance so timer start can be chained to Timer creation if desired.</span>
+</span><span id="Timer-132"><a href="#Timer-132"><span class="linenos">132</span></a>
+</span><span id="Timer-133"><a href="#Timer-133"><span class="linenos">133</span></a><span class="sd">        &gt;&gt;&gt; timer = Timer().start()&quot;&quot;&quot;</span>
+</span><span id="Timer-134"><a href="#Timer-134"><span class="linenos">134</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">started</span><span class="p">:</span>
+</span><span id="Timer-135"><a href="#Timer-135"><span class="linenos">135</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="Timer-136"><a href="#Timer-136"><span class="linenos">136</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_started</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="Timer-137"><a href="#Timer-137"><span class="linenos">137</span></a>        <span class="k">return</span> <span class="bp">self</span>
+</span><span id="Timer-138"><a href="#Timer-138"><span class="linenos">138</span></a>
+</span><span id="Timer-139"><a href="#Timer-139"><span class="linenos">139</span></a>    <span class="k">def</span> <span class="nf">stop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Timer-140"><a href="#Timer-140"><span class="linenos">140</span></a>        <span class="sd">&quot;&quot;&quot;Stop the timer.</span>
+</span><span id="Timer-141"><a href="#Timer-141"><span class="linenos">141</span></a>
+</span><span id="Timer-142"><a href="#Timer-142"><span class="linenos">142</span></a><span class="sd">        Calculates elapsed time and average elapsed time.&quot;&quot;&quot;</span>
+</span><span id="Timer-143"><a href="#Timer-143"><span class="linenos">143</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">started</span><span class="p">:</span>
+</span><span id="Timer-144"><a href="#Timer-144"><span class="linenos">144</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="Timer-145"><a href="#Timer-145"><span class="linenos">145</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_started</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="Timer-146"><a href="#Timer-146"><span class="linenos">146</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span> <span class="o">=</span> <span class="p">(</span>
+</span><span id="Timer-147"><a href="#Timer-147"><span class="linenos">147</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_pauser</span><span class="o">.</span><span class="n">pause_total</span>
+</span><span id="Timer-148"><a href="#Timer-148"><span class="linenos">148</span></a>            <span class="p">)</span>
+</span><span id="Timer-149"><a href="#Timer-149"><span class="linenos">149</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_pauser</span><span class="o">.</span><span class="n">reset</span><span class="p">()</span>
+</span><span id="Timer-150"><a href="#Timer-150"><span class="linenos">150</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_save_elapsed_time</span><span class="p">()</span>
+</span><span id="Timer-151"><a href="#Timer-151"><span class="linenos">151</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">)</span> <span class="o">/</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">))</span>
+</span><span id="Timer-152"><a href="#Timer-152"><span class="linenos">152</span></a>
+</span><span id="Timer-153"><a href="#Timer-153"><span class="linenos">153</span></a>    <span class="k">def</span> <span class="nf">pause</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Timer-154"><a href="#Timer-154"><span class="linenos">154</span></a>        <span class="sd">&quot;&quot;&quot;Pause the timer.&quot;&quot;&quot;</span>
+</span><span id="Timer-155"><a href="#Timer-155"><span class="linenos">155</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_pauser</span><span class="o">.</span><span class="n">pause</span><span class="p">()</span>
+</span><span id="Timer-156"><a href="#Timer-156"><span class="linenos">156</span></a>
+</span><span id="Timer-157"><a href="#Timer-157"><span class="linenos">157</span></a>    <span class="k">def</span> <span class="nf">unpause</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Timer-158"><a href="#Timer-158"><span class="linenos">158</span></a>        <span class="sd">&quot;&quot;&quot;Unpause the timer.&quot;&quot;&quot;</span>
+</span><span id="Timer-159"><a href="#Timer-159"><span class="linenos">159</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_pauser</span><span class="o">.</span><span class="n">unpause</span><span class="p">()</span>
+</span><span id="Timer-160"><a href="#Timer-160"><span class="linenos">160</span></a>
+</span><span id="Timer-161"><a href="#Timer-161"><span class="linenos">161</span></a>    <span class="k">def</span> <span class="nf">_save_elapsed_time</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Timer-162"><a href="#Timer-162"><span class="linenos">162</span></a>        <span class="sd">&quot;&quot;&quot;Saves current elapsed time to the history buffer in a FIFO manner.&quot;&quot;&quot;</span>
+</span><span id="Timer-163"><a href="#Timer-163"><span class="linenos">163</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">averaging_window_length</span><span class="p">:</span>
+</span><span id="Timer-164"><a href="#Timer-164"><span class="linenos">164</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="Timer-165"><a href="#Timer-165"><span class="linenos">165</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span><span class="p">)</span>
+</span><span id="Timer-166"><a href="#Timer-166"><span class="linenos">166</span></a>
+</span><span id="Timer-167"><a href="#Timer-167"><span class="linenos">167</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="Timer-168"><a href="#Timer-168"><span class="linenos">168</span></a>    <span class="k">def</span> <span class="nf">format_time</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Timer-169"><a href="#Timer-169"><span class="linenos">169</span></a>        <span class="sd">&quot;&quot;&quot;Returns `num_seconds` as a string with units.</span>
+</span><span id="Timer-170"><a href="#Timer-170"><span class="linenos">170</span></a>
+</span><span id="Timer-171"><a href="#Timer-171"><span class="linenos">171</span></a><span class="sd">        #### :params:</span>
+</span><span id="Timer-172"><a href="#Timer-172"><span class="linenos">172</span></a>
+</span><span id="Timer-173"><a href="#Timer-173"><span class="linenos">173</span></a><span class="sd">        `subsecond_resolution`: Include milliseconds and microseconds with the output.&quot;&quot;&quot;</span>
+</span><span id="Timer-174"><a href="#Timer-174"><span class="linenos">174</span></a>        <span class="n">microsecond</span> <span class="o">=</span> <span class="mf">0.000001</span>
+</span><span id="Timer-175"><a href="#Timer-175"><span class="linenos">175</span></a>        <span class="n">millisecond</span> <span class="o">=</span> <span class="mf">0.001</span>
+</span><span id="Timer-176"><a href="#Timer-176"><span class="linenos">176</span></a>        <span class="n">second</span> <span class="o">=</span> <span class="mi">1</span>
+</span><span id="Timer-177"><a href="#Timer-177"><span class="linenos">177</span></a>        <span class="n">seconds_per_minute</span> <span class="o">=</span> <span class="mi">60</span>
+</span><span id="Timer-178"><a href="#Timer-178"><span class="linenos">178</span></a>        <span class="n">seconds_per_hour</span> <span class="o">=</span> <span class="mi">3600</span>
+</span><span id="Timer-179"><a href="#Timer-179"><span class="linenos">179</span></a>        <span class="n">seconds_per_day</span> <span class="o">=</span> <span class="mi">86400</span>
+</span><span id="Timer-180"><a href="#Timer-180"><span class="linenos">180</span></a>        <span class="n">seconds_per_week</span> <span class="o">=</span> <span class="mi">604800</span>
+</span><span id="Timer-181"><a href="#Timer-181"><span class="linenos">181</span></a>        <span class="n">seconds_per_month</span> <span class="o">=</span> <span class="mi">2419200</span>
+</span><span id="Timer-182"><a href="#Timer-182"><span class="linenos">182</span></a>        <span class="n">seconds_per_year</span> <span class="o">=</span> <span class="mi">29030400</span>
+</span><span id="Timer-183"><a href="#Timer-183"><span class="linenos">183</span></a>        <span class="n">time_units</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="Timer-184"><a href="#Timer-184"><span class="linenos">184</span></a>            <span class="p">(</span><span class="n">seconds_per_year</span><span class="p">,</span> <span class="s2">&quot;y&quot;</span><span class="p">),</span>
+</span><span id="Timer-185"><a href="#Timer-185"><span class="linenos">185</span></a>            <span class="p">(</span><span class="n">seconds_per_month</span><span class="p">,</span> <span class="s2">&quot;mn&quot;</span><span class="p">),</span>
+</span><span id="Timer-186"><a href="#Timer-186"><span class="linenos">186</span></a>            <span class="p">(</span><span class="n">seconds_per_week</span><span class="p">,</span> <span class="s2">&quot;w&quot;</span><span class="p">),</span>
+</span><span id="Timer-187"><a href="#Timer-187"><span class="linenos">187</span></a>            <span class="p">(</span><span class="n">seconds_per_day</span><span class="p">,</span> <span class="s2">&quot;d&quot;</span><span class="p">),</span>
+</span><span id="Timer-188"><a href="#Timer-188"><span class="linenos">188</span></a>            <span class="p">(</span><span class="n">seconds_per_hour</span><span class="p">,</span> <span class="s2">&quot;h&quot;</span><span class="p">),</span>
+</span><span id="Timer-189"><a href="#Timer-189"><span class="linenos">189</span></a>            <span class="p">(</span><span class="n">seconds_per_minute</span><span class="p">,</span> <span class="s2">&quot;m&quot;</span><span class="p">),</span>
+</span><span id="Timer-190"><a href="#Timer-190"><span class="linenos">190</span></a>            <span class="p">(</span><span class="n">second</span><span class="p">,</span> <span class="s2">&quot;s&quot;</span><span class="p">),</span>
+</span><span id="Timer-191"><a href="#Timer-191"><span class="linenos">191</span></a>            <span class="p">(</span><span class="n">millisecond</span><span class="p">,</span> <span class="s2">&quot;ms&quot;</span><span class="p">),</span>
+</span><span id="Timer-192"><a href="#Timer-192"><span class="linenos">192</span></a>            <span class="p">(</span><span class="n">microsecond</span><span class="p">,</span> <span class="s2">&quot;us&quot;</span><span class="p">),</span>
+</span><span id="Timer-193"><a href="#Timer-193"><span class="linenos">193</span></a>        <span class="p">]</span>
+</span><span id="Timer-194"><a href="#Timer-194"><span class="linenos">194</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">subsecond_resolution</span><span class="p">:</span>
+</span><span id="Timer-195"><a href="#Timer-195"><span class="linenos">195</span></a>            <span class="n">time_units</span> <span class="o">=</span> <span class="n">time_units</span><span class="p">[:</span><span class="o">-</span><span class="mi">2</span><span class="p">]</span>
+</span><span id="Timer-196"><a href="#Timer-196"><span class="linenos">196</span></a>        <span class="n">time_string</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="Timer-197"><a href="#Timer-197"><span class="linenos">197</span></a>        <span class="k">for</span> <span class="n">time_unit</span> <span class="ow">in</span> <span class="n">time_units</span><span class="p">:</span>
+</span><span id="Timer-198"><a href="#Timer-198"><span class="linenos">198</span></a>            <span class="n">unit_amount</span><span class="p">,</span> <span class="n">num_seconds</span> <span class="o">=</span> <span class="nb">divmod</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">,</span> <span class="n">time_unit</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
+</span><span id="Timer-199"><a href="#Timer-199"><span class="linenos">199</span></a>            <span class="k">if</span> <span class="n">unit_amount</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="Timer-200"><a href="#Timer-200"><span class="linenos">200</span></a>                <span class="n">time_string</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">int</span><span class="p">(</span><span class="n">unit_amount</span><span class="p">)</span><span class="si">}{</span><span class="n">time_unit</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2"> &quot;</span>
+</span><span id="Timer-201"><a href="#Timer-201"><span class="linenos">201</span></a>        <span class="k">if</span> <span class="n">time_string</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
+</span><span id="Timer-202"><a href="#Timer-202"><span class="linenos">202</span></a>            <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;&lt;1</span><span class="si">{</span><span class="n">time_units</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">][</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="Timer-203"><a href="#Timer-203"><span class="linenos">203</span></a>        <span class="k">return</span> <span class="n">time_string</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="Timer-204"><a href="#Timer-204"><span class="linenos">204</span></a>
+</span><span id="Timer-205"><a href="#Timer-205"><span class="linenos">205</span></a>    <span class="nd">@property</span>
+</span><span id="Timer-206"><a href="#Timer-206"><span class="linenos">206</span></a>    <span class="k">def</span> <span class="nf">stats</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Timer-207"><a href="#Timer-207"><span class="linenos">207</span></a>        <span class="sd">&quot;&quot;&quot;Returns a string stating the currently elapsed time and the average elapsed time.&quot;&quot;&quot;</span>
+</span><span id="Timer-208"><a href="#Timer-208"><span class="linenos">208</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="se">\n</span><span class="s2">average elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">average_elapsed_str</span><span class="si">}</span><span class="s2">&quot;</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Simple timer class that tracks total elapsed time
-and average time between calls to 'start' and 'stop'.</p>
+and average time between calls to <code><a href="#Timer.start">start()</a></code> and <code><a href="#Timer.stop">stop()</a></code>.</p>
 </div>
 
 
                             <div id="Timer.__init__" class="classattr">
                                         <input id="Timer.__init__-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="name">Timer</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">10</span>, </span><span class="param"><span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span>)</span>
 
                 <label class="view-source-button" for="Timer.__init__-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Timer.__init__"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer.__init__-38"><a href="#Timer.__init__-38"><span class="linenos">38</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="Timer.__init__-39"><a href="#Timer.__init__-39"><span class="linenos">39</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">10</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="Timer.__init__-40"><a href="#Timer.__init__-40"><span class="linenos">40</span></a>    <span class="p">):</span>
-</span><span id="Timer.__init__-41"><a href="#Timer.__init__-41"><span class="linenos">41</span></a>        <span class="sd">&quot;&quot;&quot;:param averaging_window_length: Number of start/stop cycles</span>
-</span><span id="Timer.__init__-42"><a href="#Timer.__init__-42"><span class="linenos">42</span></a><span class="sd">        to calculate the average elapsed time with.</span>
-</span><span id="Timer.__init__-43"><a href="#Timer.__init__-43"><span class="linenos">43</span></a>
-</span><span id="Timer.__init__-44"><a href="#Timer.__init__-44"><span class="linenos">44</span></a><span class="sd">        :param subsecond_resolution: Whether to print formatted time</span>
-</span><span id="Timer.__init__-45"><a href="#Timer.__init__-45"><span class="linenos">45</span></a><span class="sd">        strings with subsecond resolution or not.&quot;&quot;&quot;</span>
-</span><span id="Timer.__init__-46"><a href="#Timer.__init__-46"><span class="linenos">46</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
-</span><span id="Timer.__init__-47"><a href="#Timer.__init__-47"><span class="linenos">47</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span>
-</span><span id="Timer.__init__-48"><a href="#Timer.__init__-48"><span class="linenos">48</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="Timer.__init__-49"><a href="#Timer.__init__-49"><span class="linenos">49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="Timer.__init__-50"><a href="#Timer.__init__-50"><span class="linenos">50</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="Timer.__init__-51"><a href="#Timer.__init__-51"><span class="linenos">51</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="Timer.__init__-52"><a href="#Timer.__init__-52"><span class="linenos">52</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="n">averaging_window_length</span>
-</span><span id="Timer.__init__-53"><a href="#Timer.__init__-53"><span class="linenos">53</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span> <span class="o">=</span> <span class="n">subsecond_resolution</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer.__init__-65"><a href="#Timer.__init__-65"><span class="linenos">65</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="Timer.__init__-66"><a href="#Timer.__init__-66"><span class="linenos">66</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">10</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="Timer.__init__-67"><a href="#Timer.__init__-67"><span class="linenos">67</span></a>    <span class="p">):</span>
+</span><span id="Timer.__init__-68"><a href="#Timer.__init__-68"><span class="linenos">68</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="Timer.__init__-69"><a href="#Timer.__init__-69"><span class="linenos">69</span></a><span class="sd">        #### :params:</span>
+</span><span id="Timer.__init__-70"><a href="#Timer.__init__-70"><span class="linenos">70</span></a><span class="sd">        * `averaging_window_length`: Number of start/stop cycles to calculate the average elapsed time with.</span>
+</span><span id="Timer.__init__-71"><a href="#Timer.__init__-71"><span class="linenos">71</span></a>
+</span><span id="Timer.__init__-72"><a href="#Timer.__init__-72"><span class="linenos">72</span></a><span class="sd">        * `subsecond_resolution`: Whether to print formatted time strings with subsecond resolution or not.&quot;&quot;&quot;</span>
+</span><span id="Timer.__init__-73"><a href="#Timer.__init__-73"><span class="linenos">73</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="Timer.__init__-74"><a href="#Timer.__init__-74"><span class="linenos">74</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span>
+</span><span id="Timer.__init__-75"><a href="#Timer.__init__-75"><span class="linenos">75</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="Timer.__init__-76"><a href="#Timer.__init__-76"><span class="linenos">76</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="Timer.__init__-77"><a href="#Timer.__init__-77"><span class="linenos">77</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Timer.__init__-78"><a href="#Timer.__init__-78"><span class="linenos">78</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="Timer.__init__-79"><a href="#Timer.__init__-79"><span class="linenos">79</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="n">averaging_window_length</span>
+</span><span id="Timer.__init__-80"><a href="#Timer.__init__-80"><span class="linenos">80</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span> <span class="o">=</span> <span class="n">subsecond_resolution</span>
+</span><span id="Timer.__init__-81"><a href="#Timer.__init__-81"><span class="linenos">81</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_pauser</span> <span class="o">=</span> <span class="n">_Pauser</span><span class="p">()</span>
 </span></pre></div>
 
 
-            <div class="docstring"><h6 id="parameters">Parameters</h6>
+            <div class="docstring"><h4 id="params">:params:</h4>
 
 <ul>
-<li><p><strong>averaging_window_length</strong>:  Number of start/stop cycles
-to calculate the average elapsed time with.</p></li>
-<li><p><strong>subsecond_resolution</strong>:  Whether to print formatted time
-strings with subsecond resolution or not.</p></li>
+<li><p><code>averaging_window_length</code>: Number of start/stop cycles to calculate the average elapsed time with.</p></li>
+<li><p><code>subsecond_resolution</code>: Whether to print formatted time strings with subsecond resolution or not.</p></li>
 </ul>
 </div>
 
 
                             </div>
                             <div id="Timer.started" class="classattr">
                                 <div class="attr variable">
             <span class="name">started</span><span class="annotation">: bool</span>
 
         
     </div>
     <a class="headerlink" href="#Timer.started"></a>
     
-            <div class="docstring"><p>Returns whether the timer has
-been started and is currently running.</p>
+            <div class="docstring"><p>Returns whether the timer has been started and is currently running.</p>
 </div>
 
 
                             </div>
                             <div id="Timer.elapsed" class="classattr">
                                 <div class="attr variable">
             <span class="name">elapsed</span><span class="annotation">: float</span>
 
         
     </div>
     <a class="headerlink" href="#Timer.elapsed"></a>
     
-            <div class="docstring"><p>Return the currently elapsed time.</p>
+            <div class="docstring"><p>Returns the currently elapsed time.</p>
 </div>
 
 
                             </div>
                             <div id="Timer.elapsed_str" class="classattr">
                                 <div class="attr variable">
             <span class="name">elapsed_str</span><span class="annotation">: str</span>
 
         
     </div>
     <a class="headerlink" href="#Timer.elapsed_str"></a>
     
-            <div class="docstring"><p>Return the currently elapsed time
-as a formatted string.</p>
+            <div class="docstring"><p>Returns the currently elapsed time as a formatted string.</p>
+</div>
+
+
+                            </div>
+                            <div id="Timer.average_elapsed" class="classattr">
+                                <div class="attr variable">
+            <span class="name">average_elapsed</span><span class="annotation">: float</span>
+
+        
+    </div>
+    <a class="headerlink" href="#Timer.average_elapsed"></a>
+    
+            <div class="docstring"><p>Returns the average elapsed time.</p>
+</div>
+
+
+                            </div>
+                            <div id="Timer.average_elapsed_str" class="classattr">
+                                <div class="attr variable">
+            <span class="name">average_elapsed_str</span><span class="annotation">: str</span>
+
+        
+    </div>
+    <a class="headerlink" href="#Timer.average_elapsed_str"></a>
+    
+            <div class="docstring"><p>Returns the average elapsed time as a formatted string.</p>
+</div>
+
+
+                            </div>
+                            <div id="Timer.start_time" class="classattr">
+                                <div class="attr variable">
+            <span class="name">start_time</span><span class="annotation">: float</span>
+
+        
+    </div>
+    <a class="headerlink" href="#Timer.start_time"></a>
+    
+            <div class="docstring"><p>Returns the timestamp of the last call to <code><a href="#Timer.start">start()</a></code>.</p>
+</div>
+
+
+                            </div>
+                            <div id="Timer.stop_time" class="classattr">
+                                <div class="attr variable">
+            <span class="name">stop_time</span><span class="annotation">: float</span>
+
+        
+    </div>
+    <a class="headerlink" href="#Timer.stop_time"></a>
+    
+            <div class="docstring"><p>Returns the timestamp of the last call to <code><a href="#Timer.stop">stop()</a></code>.</p>
+</div>
+
+
+                            </div>
+                            <div id="Timer.history" class="classattr">
+                                <div class="attr variable">
+            <span class="name">history</span><span class="annotation">: list[float]</span>
+
+        
+    </div>
+    <a class="headerlink" href="#Timer.history"></a>
+    
+            <div class="docstring"><p>Returns the history buffer for this timer.</p>
+
+<p>At most, it will be <code>averaging_window_length</code> elements long.</p>
 </div>
 
 
                             </div>
                             <div id="Timer.start" class="classattr">
                                         <input id="Timer.start-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -542,31 +684,30 @@
         <span class="def">def</span>
         <span class="name">start</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span><span class="p">:</span> <span class="n">Self</span></span><span class="return-annotation">) -> <span class="n">Self</span>:</span></span>
 
                 <label class="view-source-button" for="Timer.start-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Timer.start"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer.start-95"><a href="#Timer.start-95"><span class="linenos"> 95</span></a>    <span class="k">def</span> <span class="nf">start</span><span class="p">(</span><span class="bp">self</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Timer.start-96"><a href="#Timer.start-96"><span class="linenos"> 96</span></a>        <span class="sd">&quot;&quot;&quot;Start timer.</span>
-</span><span id="Timer.start-97"><a href="#Timer.start-97"><span class="linenos"> 97</span></a><span class="sd">        Returns this Timer instance so</span>
-</span><span id="Timer.start-98"><a href="#Timer.start-98"><span class="linenos"> 98</span></a><span class="sd">        timer start can be chained to</span>
-</span><span id="Timer.start-99"><a href="#Timer.start-99"><span class="linenos"> 99</span></a><span class="sd">        Timer creation.</span>
-</span><span id="Timer.start-100"><a href="#Timer.start-100"><span class="linenos">100</span></a>
-</span><span id="Timer.start-101"><a href="#Timer.start-101"><span class="linenos">101</span></a><span class="sd">        &gt;&gt;&gt; timer = Timer().start()&quot;&quot;&quot;</span>
-</span><span id="Timer.start-102"><a href="#Timer.start-102"><span class="linenos">102</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
-</span><span id="Timer.start-103"><a href="#Timer.start-103"><span class="linenos">103</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="Timer.start-104"><a href="#Timer.start-104"><span class="linenos">104</span></a>        <span class="k">return</span> <span class="bp">self</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer.start-128"><a href="#Timer.start-128"><span class="linenos">128</span></a>    <span class="k">def</span> <span class="nf">start</span><span class="p">(</span><span class="bp">self</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Timer.start-129"><a href="#Timer.start-129"><span class="linenos">129</span></a>        <span class="sd">&quot;&quot;&quot;Start the timer.</span>
+</span><span id="Timer.start-130"><a href="#Timer.start-130"><span class="linenos">130</span></a>
+</span><span id="Timer.start-131"><a href="#Timer.start-131"><span class="linenos">131</span></a><span class="sd">        Returns this Timer instance so timer start can be chained to Timer creation if desired.</span>
+</span><span id="Timer.start-132"><a href="#Timer.start-132"><span class="linenos">132</span></a>
+</span><span id="Timer.start-133"><a href="#Timer.start-133"><span class="linenos">133</span></a><span class="sd">        &gt;&gt;&gt; timer = Timer().start()&quot;&quot;&quot;</span>
+</span><span id="Timer.start-134"><a href="#Timer.start-134"><span class="linenos">134</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">started</span><span class="p">:</span>
+</span><span id="Timer.start-135"><a href="#Timer.start-135"><span class="linenos">135</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="Timer.start-136"><a href="#Timer.start-136"><span class="linenos">136</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_started</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="Timer.start-137"><a href="#Timer.start-137"><span class="linenos">137</span></a>        <span class="k">return</span> <span class="bp">self</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Start timer.
-Returns this Timer instance so
-timer start can be chained to
-Timer creation.</p>
+            <div class="docstring"><p>Start the timer.</p>
+
+<p>Returns this Timer instance so timer start can be chained to Timer creation if desired.</p>
 
 <div class="pdoc-code codehilite">
 <pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">()</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
 </code></pre>
 </div>
 </div>
 
@@ -579,106 +720,151 @@
         <span class="def">def</span>
         <span class="name">stop</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Timer.stop-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Timer.stop"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer.stop-106"><a href="#Timer.stop-106"><span class="linenos">106</span></a>    <span class="k">def</span> <span class="nf">stop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Timer.stop-107"><a href="#Timer.stop-107"><span class="linenos">107</span></a>        <span class="sd">&quot;&quot;&quot;Stop timer.</span>
-</span><span id="Timer.stop-108"><a href="#Timer.stop-108"><span class="linenos">108</span></a>
-</span><span id="Timer.stop-109"><a href="#Timer.stop-109"><span class="linenos">109</span></a><span class="sd">        Calculates elapsed time and average elapsed time.&quot;&quot;&quot;</span>
-</span><span id="Timer.stop-110"><a href="#Timer.stop-110"><span class="linenos">110</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
-</span><span id="Timer.stop-111"><a href="#Timer.stop-111"><span class="linenos">111</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="Timer.stop-112"><a href="#Timer.stop-112"><span class="linenos">112</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span>
-</span><span id="Timer.stop-113"><a href="#Timer.stop-113"><span class="linenos">113</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_save_elapsed_time</span><span class="p">()</span>
-</span><span id="Timer.stop-114"><a href="#Timer.stop-114"><span class="linenos">114</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">)</span> <span class="o">/</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer.stop-139"><a href="#Timer.stop-139"><span class="linenos">139</span></a>    <span class="k">def</span> <span class="nf">stop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Timer.stop-140"><a href="#Timer.stop-140"><span class="linenos">140</span></a>        <span class="sd">&quot;&quot;&quot;Stop the timer.</span>
+</span><span id="Timer.stop-141"><a href="#Timer.stop-141"><span class="linenos">141</span></a>
+</span><span id="Timer.stop-142"><a href="#Timer.stop-142"><span class="linenos">142</span></a><span class="sd">        Calculates elapsed time and average elapsed time.&quot;&quot;&quot;</span>
+</span><span id="Timer.stop-143"><a href="#Timer.stop-143"><span class="linenos">143</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">started</span><span class="p">:</span>
+</span><span id="Timer.stop-144"><a href="#Timer.stop-144"><span class="linenos">144</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="Timer.stop-145"><a href="#Timer.stop-145"><span class="linenos">145</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_started</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="Timer.stop-146"><a href="#Timer.stop-146"><span class="linenos">146</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span> <span class="o">=</span> <span class="p">(</span>
+</span><span id="Timer.stop-147"><a href="#Timer.stop-147"><span class="linenos">147</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_pauser</span><span class="o">.</span><span class="n">pause_total</span>
+</span><span id="Timer.stop-148"><a href="#Timer.stop-148"><span class="linenos">148</span></a>            <span class="p">)</span>
+</span><span id="Timer.stop-149"><a href="#Timer.stop-149"><span class="linenos">149</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_pauser</span><span class="o">.</span><span class="n">reset</span><span class="p">()</span>
+</span><span id="Timer.stop-150"><a href="#Timer.stop-150"><span class="linenos">150</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_save_elapsed_time</span><span class="p">()</span>
+</span><span id="Timer.stop-151"><a href="#Timer.stop-151"><span class="linenos">151</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">)</span> <span class="o">/</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">))</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Stop timer.</p>
+            <div class="docstring"><p>Stop the timer.</p>
 
 <p>Calculates elapsed time and average elapsed time.</p>
 </div>
 
 
                             </div>
+                            <div id="Timer.pause" class="classattr">
+                                        <input id="Timer.pause-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">pause</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="Timer.pause-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#Timer.pause"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer.pause-153"><a href="#Timer.pause-153"><span class="linenos">153</span></a>    <span class="k">def</span> <span class="nf">pause</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Timer.pause-154"><a href="#Timer.pause-154"><span class="linenos">154</span></a>        <span class="sd">&quot;&quot;&quot;Pause the timer.&quot;&quot;&quot;</span>
+</span><span id="Timer.pause-155"><a href="#Timer.pause-155"><span class="linenos">155</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_pauser</span><span class="o">.</span><span class="n">pause</span><span class="p">()</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Pause the timer.</p>
+</div>
+
+
+                            </div>
+                            <div id="Timer.unpause" class="classattr">
+                                        <input id="Timer.unpause-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">unpause</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="Timer.unpause-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#Timer.unpause"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer.unpause-157"><a href="#Timer.unpause-157"><span class="linenos">157</span></a>    <span class="k">def</span> <span class="nf">unpause</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Timer.unpause-158"><a href="#Timer.unpause-158"><span class="linenos">158</span></a>        <span class="sd">&quot;&quot;&quot;Unpause the timer.&quot;&quot;&quot;</span>
+</span><span id="Timer.unpause-159"><a href="#Timer.unpause-159"><span class="linenos">159</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_pauser</span><span class="o">.</span><span class="n">unpause</span><span class="p">()</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Unpause the timer.</p>
+</div>
+
+
+                            </div>
                             <div id="Timer.format_time" class="classattr">
                                         <input id="Timer.format_time-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
                     <div class="decorator">@staticmethod</div>
 
         <span class="def">def</span>
         <span class="name">format_time</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">num_seconds</span><span class="p">:</span> <span class="nb">float</span>, </span><span class="param"><span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
 
                 <label class="view-source-button" for="Timer.format_time-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Timer.format_time"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer.format_time-123"><a href="#Timer.format_time-123"><span class="linenos">123</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="Timer.format_time-124"><a href="#Timer.format_time-124"><span class="linenos">124</span></a>    <span class="k">def</span> <span class="nf">format_time</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Timer.format_time-125"><a href="#Timer.format_time-125"><span class="linenos">125</span></a>        <span class="sd">&quot;&quot;&quot;Returns num_seconds as a string with units.</span>
-</span><span id="Timer.format_time-126"><a href="#Timer.format_time-126"><span class="linenos">126</span></a>
-</span><span id="Timer.format_time-127"><a href="#Timer.format_time-127"><span class="linenos">127</span></a><span class="sd">        :param subsecond_resolution: Include milliseconds</span>
-</span><span id="Timer.format_time-128"><a href="#Timer.format_time-128"><span class="linenos">128</span></a><span class="sd">        and microseconds with the output.&quot;&quot;&quot;</span>
-</span><span id="Timer.format_time-129"><a href="#Timer.format_time-129"><span class="linenos">129</span></a>        <span class="n">microsecond</span> <span class="o">=</span> <span class="mf">0.000001</span>
-</span><span id="Timer.format_time-130"><a href="#Timer.format_time-130"><span class="linenos">130</span></a>        <span class="n">millisecond</span> <span class="o">=</span> <span class="mf">0.001</span>
-</span><span id="Timer.format_time-131"><a href="#Timer.format_time-131"><span class="linenos">131</span></a>        <span class="n">second</span> <span class="o">=</span> <span class="mi">1</span>
-</span><span id="Timer.format_time-132"><a href="#Timer.format_time-132"><span class="linenos">132</span></a>        <span class="n">seconds_per_minute</span> <span class="o">=</span> <span class="mi">60</span>
-</span><span id="Timer.format_time-133"><a href="#Timer.format_time-133"><span class="linenos">133</span></a>        <span class="n">seconds_per_hour</span> <span class="o">=</span> <span class="mi">3600</span>
-</span><span id="Timer.format_time-134"><a href="#Timer.format_time-134"><span class="linenos">134</span></a>        <span class="n">seconds_per_day</span> <span class="o">=</span> <span class="mi">86400</span>
-</span><span id="Timer.format_time-135"><a href="#Timer.format_time-135"><span class="linenos">135</span></a>        <span class="n">seconds_per_week</span> <span class="o">=</span> <span class="mi">604800</span>
-</span><span id="Timer.format_time-136"><a href="#Timer.format_time-136"><span class="linenos">136</span></a>        <span class="n">seconds_per_month</span> <span class="o">=</span> <span class="mi">2419200</span>
-</span><span id="Timer.format_time-137"><a href="#Timer.format_time-137"><span class="linenos">137</span></a>        <span class="n">seconds_per_year</span> <span class="o">=</span> <span class="mi">29030400</span>
-</span><span id="Timer.format_time-138"><a href="#Timer.format_time-138"><span class="linenos">138</span></a>        <span class="n">time_units</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Timer.format_time-139"><a href="#Timer.format_time-139"><span class="linenos">139</span></a>            <span class="p">(</span><span class="n">seconds_per_year</span><span class="p">,</span> <span class="s2">&quot;y&quot;</span><span class="p">),</span>
-</span><span id="Timer.format_time-140"><a href="#Timer.format_time-140"><span class="linenos">140</span></a>            <span class="p">(</span><span class="n">seconds_per_month</span><span class="p">,</span> <span class="s2">&quot;mn&quot;</span><span class="p">),</span>
-</span><span id="Timer.format_time-141"><a href="#Timer.format_time-141"><span class="linenos">141</span></a>            <span class="p">(</span><span class="n">seconds_per_week</span><span class="p">,</span> <span class="s2">&quot;w&quot;</span><span class="p">),</span>
-</span><span id="Timer.format_time-142"><a href="#Timer.format_time-142"><span class="linenos">142</span></a>            <span class="p">(</span><span class="n">seconds_per_day</span><span class="p">,</span> <span class="s2">&quot;d&quot;</span><span class="p">),</span>
-</span><span id="Timer.format_time-143"><a href="#Timer.format_time-143"><span class="linenos">143</span></a>            <span class="p">(</span><span class="n">seconds_per_hour</span><span class="p">,</span> <span class="s2">&quot;h&quot;</span><span class="p">),</span>
-</span><span id="Timer.format_time-144"><a href="#Timer.format_time-144"><span class="linenos">144</span></a>            <span class="p">(</span><span class="n">seconds_per_minute</span><span class="p">,</span> <span class="s2">&quot;m&quot;</span><span class="p">),</span>
-</span><span id="Timer.format_time-145"><a href="#Timer.format_time-145"><span class="linenos">145</span></a>            <span class="p">(</span><span class="n">second</span><span class="p">,</span> <span class="s2">&quot;s&quot;</span><span class="p">),</span>
-</span><span id="Timer.format_time-146"><a href="#Timer.format_time-146"><span class="linenos">146</span></a>            <span class="p">(</span><span class="n">millisecond</span><span class="p">,</span> <span class="s2">&quot;ms&quot;</span><span class="p">),</span>
-</span><span id="Timer.format_time-147"><a href="#Timer.format_time-147"><span class="linenos">147</span></a>            <span class="p">(</span><span class="n">microsecond</span><span class="p">,</span> <span class="s2">&quot;us&quot;</span><span class="p">),</span>
-</span><span id="Timer.format_time-148"><a href="#Timer.format_time-148"><span class="linenos">148</span></a>        <span class="p">]</span>
-</span><span id="Timer.format_time-149"><a href="#Timer.format_time-149"><span class="linenos">149</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">subsecond_resolution</span><span class="p">:</span>
-</span><span id="Timer.format_time-150"><a href="#Timer.format_time-150"><span class="linenos">150</span></a>            <span class="n">time_units</span> <span class="o">=</span> <span class="n">time_units</span><span class="p">[:</span><span class="o">-</span><span class="mi">2</span><span class="p">]</span>
-</span><span id="Timer.format_time-151"><a href="#Timer.format_time-151"><span class="linenos">151</span></a>        <span class="n">time_string</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="Timer.format_time-152"><a href="#Timer.format_time-152"><span class="linenos">152</span></a>        <span class="k">for</span> <span class="n">time_unit</span> <span class="ow">in</span> <span class="n">time_units</span><span class="p">:</span>
-</span><span id="Timer.format_time-153"><a href="#Timer.format_time-153"><span class="linenos">153</span></a>            <span class="n">unit_amount</span><span class="p">,</span> <span class="n">num_seconds</span> <span class="o">=</span> <span class="nb">divmod</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">,</span> <span class="n">time_unit</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
-</span><span id="Timer.format_time-154"><a href="#Timer.format_time-154"><span class="linenos">154</span></a>            <span class="k">if</span> <span class="n">unit_amount</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="Timer.format_time-155"><a href="#Timer.format_time-155"><span class="linenos">155</span></a>                <span class="n">time_string</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">int</span><span class="p">(</span><span class="n">unit_amount</span><span class="p">)</span><span class="si">}{</span><span class="n">time_unit</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2"> &quot;</span>
-</span><span id="Timer.format_time-156"><a href="#Timer.format_time-156"><span class="linenos">156</span></a>        <span class="k">if</span> <span class="n">time_string</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
-</span><span id="Timer.format_time-157"><a href="#Timer.format_time-157"><span class="linenos">157</span></a>            <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;&lt;1</span><span class="si">{</span><span class="n">time_units</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">][</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="Timer.format_time-158"><a href="#Timer.format_time-158"><span class="linenos">158</span></a>        <span class="k">return</span> <span class="n">time_string</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer.format_time-167"><a href="#Timer.format_time-167"><span class="linenos">167</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="Timer.format_time-168"><a href="#Timer.format_time-168"><span class="linenos">168</span></a>    <span class="k">def</span> <span class="nf">format_time</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Timer.format_time-169"><a href="#Timer.format_time-169"><span class="linenos">169</span></a>        <span class="sd">&quot;&quot;&quot;Returns `num_seconds` as a string with units.</span>
+</span><span id="Timer.format_time-170"><a href="#Timer.format_time-170"><span class="linenos">170</span></a>
+</span><span id="Timer.format_time-171"><a href="#Timer.format_time-171"><span class="linenos">171</span></a><span class="sd">        #### :params:</span>
+</span><span id="Timer.format_time-172"><a href="#Timer.format_time-172"><span class="linenos">172</span></a>
+</span><span id="Timer.format_time-173"><a href="#Timer.format_time-173"><span class="linenos">173</span></a><span class="sd">        `subsecond_resolution`: Include milliseconds and microseconds with the output.&quot;&quot;&quot;</span>
+</span><span id="Timer.format_time-174"><a href="#Timer.format_time-174"><span class="linenos">174</span></a>        <span class="n">microsecond</span> <span class="o">=</span> <span class="mf">0.000001</span>
+</span><span id="Timer.format_time-175"><a href="#Timer.format_time-175"><span class="linenos">175</span></a>        <span class="n">millisecond</span> <span class="o">=</span> <span class="mf">0.001</span>
+</span><span id="Timer.format_time-176"><a href="#Timer.format_time-176"><span class="linenos">176</span></a>        <span class="n">second</span> <span class="o">=</span> <span class="mi">1</span>
+</span><span id="Timer.format_time-177"><a href="#Timer.format_time-177"><span class="linenos">177</span></a>        <span class="n">seconds_per_minute</span> <span class="o">=</span> <span class="mi">60</span>
+</span><span id="Timer.format_time-178"><a href="#Timer.format_time-178"><span class="linenos">178</span></a>        <span class="n">seconds_per_hour</span> <span class="o">=</span> <span class="mi">3600</span>
+</span><span id="Timer.format_time-179"><a href="#Timer.format_time-179"><span class="linenos">179</span></a>        <span class="n">seconds_per_day</span> <span class="o">=</span> <span class="mi">86400</span>
+</span><span id="Timer.format_time-180"><a href="#Timer.format_time-180"><span class="linenos">180</span></a>        <span class="n">seconds_per_week</span> <span class="o">=</span> <span class="mi">604800</span>
+</span><span id="Timer.format_time-181"><a href="#Timer.format_time-181"><span class="linenos">181</span></a>        <span class="n">seconds_per_month</span> <span class="o">=</span> <span class="mi">2419200</span>
+</span><span id="Timer.format_time-182"><a href="#Timer.format_time-182"><span class="linenos">182</span></a>        <span class="n">seconds_per_year</span> <span class="o">=</span> <span class="mi">29030400</span>
+</span><span id="Timer.format_time-183"><a href="#Timer.format_time-183"><span class="linenos">183</span></a>        <span class="n">time_units</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="Timer.format_time-184"><a href="#Timer.format_time-184"><span class="linenos">184</span></a>            <span class="p">(</span><span class="n">seconds_per_year</span><span class="p">,</span> <span class="s2">&quot;y&quot;</span><span class="p">),</span>
+</span><span id="Timer.format_time-185"><a href="#Timer.format_time-185"><span class="linenos">185</span></a>            <span class="p">(</span><span class="n">seconds_per_month</span><span class="p">,</span> <span class="s2">&quot;mn&quot;</span><span class="p">),</span>
+</span><span id="Timer.format_time-186"><a href="#Timer.format_time-186"><span class="linenos">186</span></a>            <span class="p">(</span><span class="n">seconds_per_week</span><span class="p">,</span> <span class="s2">&quot;w&quot;</span><span class="p">),</span>
+</span><span id="Timer.format_time-187"><a href="#Timer.format_time-187"><span class="linenos">187</span></a>            <span class="p">(</span><span class="n">seconds_per_day</span><span class="p">,</span> <span class="s2">&quot;d&quot;</span><span class="p">),</span>
+</span><span id="Timer.format_time-188"><a href="#Timer.format_time-188"><span class="linenos">188</span></a>            <span class="p">(</span><span class="n">seconds_per_hour</span><span class="p">,</span> <span class="s2">&quot;h&quot;</span><span class="p">),</span>
+</span><span id="Timer.format_time-189"><a href="#Timer.format_time-189"><span class="linenos">189</span></a>            <span class="p">(</span><span class="n">seconds_per_minute</span><span class="p">,</span> <span class="s2">&quot;m&quot;</span><span class="p">),</span>
+</span><span id="Timer.format_time-190"><a href="#Timer.format_time-190"><span class="linenos">190</span></a>            <span class="p">(</span><span class="n">second</span><span class="p">,</span> <span class="s2">&quot;s&quot;</span><span class="p">),</span>
+</span><span id="Timer.format_time-191"><a href="#Timer.format_time-191"><span class="linenos">191</span></a>            <span class="p">(</span><span class="n">millisecond</span><span class="p">,</span> <span class="s2">&quot;ms&quot;</span><span class="p">),</span>
+</span><span id="Timer.format_time-192"><a href="#Timer.format_time-192"><span class="linenos">192</span></a>            <span class="p">(</span><span class="n">microsecond</span><span class="p">,</span> <span class="s2">&quot;us&quot;</span><span class="p">),</span>
+</span><span id="Timer.format_time-193"><a href="#Timer.format_time-193"><span class="linenos">193</span></a>        <span class="p">]</span>
+</span><span id="Timer.format_time-194"><a href="#Timer.format_time-194"><span class="linenos">194</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">subsecond_resolution</span><span class="p">:</span>
+</span><span id="Timer.format_time-195"><a href="#Timer.format_time-195"><span class="linenos">195</span></a>            <span class="n">time_units</span> <span class="o">=</span> <span class="n">time_units</span><span class="p">[:</span><span class="o">-</span><span class="mi">2</span><span class="p">]</span>
+</span><span id="Timer.format_time-196"><a href="#Timer.format_time-196"><span class="linenos">196</span></a>        <span class="n">time_string</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="Timer.format_time-197"><a href="#Timer.format_time-197"><span class="linenos">197</span></a>        <span class="k">for</span> <span class="n">time_unit</span> <span class="ow">in</span> <span class="n">time_units</span><span class="p">:</span>
+</span><span id="Timer.format_time-198"><a href="#Timer.format_time-198"><span class="linenos">198</span></a>            <span class="n">unit_amount</span><span class="p">,</span> <span class="n">num_seconds</span> <span class="o">=</span> <span class="nb">divmod</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">,</span> <span class="n">time_unit</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
+</span><span id="Timer.format_time-199"><a href="#Timer.format_time-199"><span class="linenos">199</span></a>            <span class="k">if</span> <span class="n">unit_amount</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="Timer.format_time-200"><a href="#Timer.format_time-200"><span class="linenos">200</span></a>                <span class="n">time_string</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">int</span><span class="p">(</span><span class="n">unit_amount</span><span class="p">)</span><span class="si">}{</span><span class="n">time_unit</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2"> &quot;</span>
+</span><span id="Timer.format_time-201"><a href="#Timer.format_time-201"><span class="linenos">201</span></a>        <span class="k">if</span> <span class="n">time_string</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
+</span><span id="Timer.format_time-202"><a href="#Timer.format_time-202"><span class="linenos">202</span></a>            <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;&lt;1</span><span class="si">{</span><span class="n">time_units</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">][</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="Timer.format_time-203"><a href="#Timer.format_time-203"><span class="linenos">203</span></a>        <span class="k">return</span> <span class="n">time_string</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Returns num_seconds as a string with units.</p>
+            <div class="docstring"><p>Returns <code>num_seconds</code> as a string with units.</p>
 
-<h6 id="parameters">Parameters</h6>
+<h4 id="params">:params:</h4>
 
-<ul>
-<li><strong>subsecond_resolution</strong>:  Include milliseconds
-and microseconds with the output.</li>
-</ul>
+<p><code>subsecond_resolution</code>: Include milliseconds and microseconds with the output.</p>
 </div>
 
 
                             </div>
                             <div id="Timer.stats" class="classattr">
                                 <div class="attr variable">
             <span class="name">stats</span><span class="annotation">: str</span>
 
         
     </div>
     <a class="headerlink" href="#Timer.stats"></a>
     
-            <div class="docstring"><p>Returns a string stating the currently elapsed time
-and the average elapsed time.</p>
+            <div class="docstring"><p>Returns a string stating the currently elapsed time and the average elapsed time.</p>
 </div>
 
 
                             </div>
                 </section>
     </main>
 <script>
```

#### html2text {}

```diff
@@ -5,35 +5,42 @@
 ***** API Documentation *****
     * time_it
     * Timer
           o Timer
           o started
           o elapsed
           o elapsed_str
+          o average_elapsed
+          o average_elapsed_str
+          o start_time
+          o stop_time
+          o history
           o start
           o stop
+          o pause
+          o unpause
           o format_time
           o stats
 built_with_pdoc[pdoc_logo]
 
 ****** noiftimer.noiftimer ******
 ⁰ View Source
 __1import time
 __2from typing import Any, Callable
 __3
 __4from typing_extensions import Self
 __5
 __6
 __7def time_it(loops: int = 1) -> Callable[..., Any]:
-__8    """Decorator to time function execution time
-__9    and print the results.
-_10
-_11    :param loops: How many times to loop the function,
-_12    starting and stopping the timer before and after
-_13    each loop."""
+__8    """Decorator to time function execution time and print the results.
+__9
+_10    #### :params:
+_11
+_12    `loops`: How many times to execute the decorated function,
+_13    starting and stopping the timer before and after each loop."""
 _14
 _15    def decorator(func: Callable[..., Any]) -> Callable[..., Any]:
 _16        def wrapper(*args, **kwargs) -> Any:
 _17            timer = Timer(loops)
 _18            result = None
 _19            for _ in range(loops):
 _20                timer.start()
@@ -46,158 +53,211 @@
 _26            return result
 _27
 _28        return wrapper
 _29
 _30    return decorator
 _31
 _32
-_33class Timer:
-_34    """Simple timer class that tracks total elapsed time
-_35    and average time between calls to 'start' and 'stop'."""
-_36
-_37    def __init__(
-_38        self, averaging_window_length: int = 10, subsecond_resolution: bool
-= True
-_39    ):
-_40        """:param averaging_window_length: Number of start/stop cycles
-_41        to calculate the average elapsed time with.
+_33class _Pauser:
+_34    def __init__(self):
+_35        self._pause_start = 0
+_36        self._pause_total = 0
+_37        self._paused = False
+_38
+_39    def pause(self):
+_40        self._pause_start = time.time()
+_41        self._paused = True
 _42
-_43        :param subsecond_resolution: Whether to print formatted time
-_44        strings with subsecond resolution or not."""
-_45        self._start_time = time.time()
-_46        self._stop_time = self.start_time
-_47        self._elapsed = 0
-_48        self._average_elapsed = 0
-_49        self._history: list[float] = []
-_50        self._started: bool = False
-_51        self.averaging_window_length: int = averaging_window_length
-_52        self.subsecond_resolution = subsecond_resolution
-_53
-_54    @property
-_55    def started(self) -> bool:
-_56        """Returns whether the timer has
-_57        been started and is currently running."""
-_58        return self._started
+_43    def unpause(self):
+_44        self._pause_total += time.time() - self._pause_start
+_45        self._paused = False
+_46
+_47    def reset(self):
+_48        self._pause_start = 0
+_49        self._pause_total = 0
+_50        self._paused = False
+_51
+_52    @property
+_53    def pause_total(self) -> float:
+_54        if self._paused:
+_55            return self._pause_total + (time.time() - self._pause_start)
+_56        else:
+_57            return self._pause_total
+_58
 _59
-_60    @property
-_61    def elapsed(self) -> float:
-_62        """Return the currently elapsed time."""
-_63        if self._started:
-_64            return time.time() - self._start_time
-_65        else:
-_66            return self._elapsed
-_67
-_68    @property
-_69    def elapsed_str(self) -> str:
-_70        """Return the currently elapsed time
-_71        as a formatted string."""
-_72        return self.format_time(self.elapsed, self.subsecond_resolution)
-_73
-_74    @property
-_75    def average_elapsed(self) -> float:
-_76        return self._average_elapsed
-_77
-_78    @property
-_79    def average_elapsed_str(self) -> str:
-_80        return self.format_time(self._average_elapsed,
-self.subsecond_resolution)
+_60class Timer:
+_61    """Simple timer class that tracks total elapsed time
+_62    and average time between calls to `start()` and `stop()`."""
+_63
+_64    def __init__(
+_65        self, averaging_window_length: int = 10, subsecond_resolution: bool
+= True
+_66    ):
+_67        """
+_68        #### :params:
+_69        * `averaging_window_length`: Number of start/stop cycles to
+calculate the average elapsed time with.
+_70
+_71        * `subsecond_resolution`: Whether to print formatted time strings
+with subsecond resolution or not."""
+_72        self._start_time = time.time()
+_73        self._stop_time = self.start_time
+_74        self._elapsed = 0
+_75        self._average_elapsed = 0
+_76        self._history: list[float] = []
+_77        self._started: bool = False
+_78        self.averaging_window_length: int = averaging_window_length
+_79        self.subsecond_resolution = subsecond_resolution
+_80        self._pauser = _Pauser()
 _81
 _82    @property
-_83    def start_time(self) -> float:
-_84        return self._start_time
-_85
-_86    @property
-_87    def stop_time(self) -> float:
-_88        return self._stop_time
-_89
-_90    @property
-_91    def history(self) -> list[float]:
-_92        return self._history
-_93
-_94    def start(self: Self) -> Self:
-_95        """Start timer.
-_96        Returns this Timer instance so
-_97        timer start can be chained to
-_98        Timer creation.
+_83    def started(self) -> bool:
+_84        """Returns whether the timer has been started and is currently
+running."""
+_85        return self._started
+_86
+_87    @property
+_88    def elapsed(self) -> float:
+_89        """Returns the currently elapsed time."""
+_90        if self._started:
+_91            return time.time() - self._start_time - self._pauser.pause_total
+_92        else:
+_93            return self._elapsed
+_94
+_95    @property
+_96    def elapsed_str(self) -> str:
+_97        """Returns the currently elapsed time as a formatted string."""
+_98        return self.format_time(self.elapsed, self.subsecond_resolution)
 _99
-100        >>> timer = Timer().start()"""
-101        self._start_time = time.time()
-102        self._started = True
-103        return self
+100    @property
+101    def average_elapsed(self) -> float:
+102        """Returns the average elapsed time."""
+103        return self._average_elapsed
 104
-105    def stop(self):
-106        """Stop timer.
-107
-108        Calculates elapsed time and average elapsed time."""
-109        self._stop_time = time.time()
-110        self._started = False
-111        self._elapsed = self._stop_time - self._start_time
-112        self._save_elapsed_time()
-113        self._average_elapsed = sum(self._history) / (len(self._history))
+105    @property
+106    def average_elapsed_str(self) -> str:
+107        """Returns the average elapsed time as a formatted string."""
+108        return self.format_time(self._average_elapsed,
+self.subsecond_resolution)
+109
+110    @property
+111    def start_time(self) -> float:
+112        """Returns the timestamp of the last call to `start()`."""
+113        return self._start_time
 114
-115    def _save_elapsed_time(self):
-116        """Saves current elapsed time to the history buffer
-117        in a FIFO manner."""
-118        if len(self._history) >= self.averaging_window_length:
-119            self._history.pop(0)
-120        self._history.append(self._elapsed)
-121
-122    @staticmethod
-123    def format_time(num_seconds: float, subsecond_resolution: bool = False)
+115    @property
+116    def stop_time(self) -> float:
+117        """Returns the timestamp of the last call to `stop()`."""
+118        return self._stop_time
+119
+120    @property
+121    def history(self) -> list[float]:
+122        """Returns the history buffer for this timer.
+123
+124        At most, it will be `averaging_window_length` elements long."""
+125        return self._history
+126
+127    def start(self: Self) -> Self:
+128        """Start the timer.
+129
+130        Returns this Timer instance so timer start can be chained to Timer
+creation if desired.
+131
+132        >>> timer = Timer().start()"""
+133        if not self.started:
+134            self._start_time = time.time()
+135            self._started = True
+136        return self
+137
+138    def stop(self):
+139        """Stop the timer.
+140
+141        Calculates elapsed time and average elapsed time."""
+142        if self.started:
+143            self._stop_time = time.time()
+144            self._started = False
+145            self._elapsed = (
+146                self._stop_time - self._start_time -
+self._pauser.pause_total
+147            )
+148            self._pauser.reset()
+149            self._save_elapsed_time()
+150            self._average_elapsed = sum(self._history) / (len
+(self._history))
+151
+152    def pause(self):
+153        """Pause the timer."""
+154        self._pauser.pause()
+155
+156    def unpause(self):
+157        """Unpause the timer."""
+158        self._pauser.unpause()
+159
+160    def _save_elapsed_time(self):
+161        """Saves current elapsed time to the history buffer in a FIFO
+manner."""
+162        if len(self._history) >= self.averaging_window_length:
+163            self._history.pop(0)
+164        self._history.append(self._elapsed)
+165
+166    @staticmethod
+167    def format_time(num_seconds: float, subsecond_resolution: bool = False)
 -> str:
-124        """Returns num_seconds as a string with units.
-125
-126        :param subsecond_resolution: Include milliseconds
-127        and microseconds with the output."""
-128        microsecond = 0.000001
-129        millisecond = 0.001
-130        second = 1
-131        seconds_per_minute = 60
-132        seconds_per_hour = 3600
-133        seconds_per_day = 86400
-134        seconds_per_week = 604800
-135        seconds_per_month = 2419200
-136        seconds_per_year = 29030400
-137        time_units = [
-138            (seconds_per_year, "y"),
-139            (seconds_per_month, "mn"),
-140            (seconds_per_week, "w"),
-141            (seconds_per_day, "d"),
-142            (seconds_per_hour, "h"),
-143            (seconds_per_minute, "m"),
-144            (second, "s"),
-145            (millisecond, "ms"),
-146            (microsecond, "us"),
-147        ]
-148        if not subsecond_resolution:
-149            time_units = time_units[:-2]
-150        time_string = ""
-151        for time_unit in time_units:
-152            unit_amount, num_seconds = divmod(num_seconds, time_unit[0])
-153            if unit_amount > 0:
-154                time_string += f"{int(unit_amount)}{time_unit[1]} "
-155        if time_string == "":
-156            return f"<1{time_units[-1][1]}"
-157        return time_string.strip()
-158
-159    @property
-160    def stats(self) -> str:
-161        """Returns a string stating the currently elapsed time
-162        and the average elapsed time."""
-163        return f"elapsed time: {self.elapsed_str}\naverage elapsed time:
+168        """Returns `num_seconds` as a string with units.
+169
+170        #### :params:
+171
+172        `subsecond_resolution`: Include milliseconds and microseconds with
+the output."""
+173        microsecond = 0.000001
+174        millisecond = 0.001
+175        second = 1
+176        seconds_per_minute = 60
+177        seconds_per_hour = 3600
+178        seconds_per_day = 86400
+179        seconds_per_week = 604800
+180        seconds_per_month = 2419200
+181        seconds_per_year = 29030400
+182        time_units = [
+183            (seconds_per_year, "y"),
+184            (seconds_per_month, "mn"),
+185            (seconds_per_week, "w"),
+186            (seconds_per_day, "d"),
+187            (seconds_per_hour, "h"),
+188            (seconds_per_minute, "m"),
+189            (second, "s"),
+190            (millisecond, "ms"),
+191            (microsecond, "us"),
+192        ]
+193        if not subsecond_resolution:
+194            time_units = time_units[:-2]
+195        time_string = ""
+196        for time_unit in time_units:
+197            unit_amount, num_seconds = divmod(num_seconds, time_unit[0])
+198            if unit_amount > 0:
+199                time_string += f"{int(unit_amount)}{time_unit[1]} "
+200        if time_string == "":
+201            return f"<1{time_units[-1][1]}"
+202        return time_string.strip()
+203
+204    @property
+205    def stats(self) -> str:
+206        """Returns a string stating the currently elapsed time and the
+average elapsed time."""
+207        return f"elapsed time: {self.elapsed_str}\naverage elapsed time:
 {self.average_elapsed_str}"
   ⁰
 def time_it(loops: int = 1) -> Callable[..., Any]: View Source
 _8def time_it(loops: int = 1) -> Callable[..., Any]:
-_9    """Decorator to time function execution time
-10    and print the results.
-11
-12    :param loops: How many times to loop the function,
-13    starting and stopping the timer before and after
-14    each loop."""
+_9    """Decorator to time function execution time and print the results.
+10
+11    #### :params:
+12
+13    `loops`: How many times to execute the decorated function,
+14    starting and stopping the timer before and after each loop."""
 15
 16    def decorator(func: Callable[..., Any]) -> Callable[..., Any]:
 17        def wrapper(*args, **kwargs) -> Any:
 18            timer = Timer(loops)
 19            result = None
 20            for _ in range(loops):
 21                timer.start()
@@ -209,257 +269,318 @@
 26            )
 27            return result
 28
 29        return wrapper
 30
 31    return decorator
 Decorator to time function execution time and print the results.
-* Parameters *
-    * loops: How many times to loop the function, starting and stopping the
-      timer before and after each loop.
+*** :params: ***
+loops: How many times to execute the decorated function, starting and stopping
+the timer before and after each loop.
   ⁰
 class Timer: View Source
-_34class Timer:
-_35    """Simple timer class that tracks total elapsed time
-_36    and average time between calls to 'start' and 'stop'."""
-_37
-_38    def __init__(
-_39        self, averaging_window_length: int = 10, subsecond_resolution: bool
+_61class Timer:
+_62    """Simple timer class that tracks total elapsed time
+_63    and average time between calls to `start()` and `stop()`."""
+_64
+_65    def __init__(
+_66        self, averaging_window_length: int = 10, subsecond_resolution: bool
 = True
-_40    ):
-_41        """:param averaging_window_length: Number of start/stop cycles
-_42        to calculate the average elapsed time with.
-_43
-_44        :param subsecond_resolution: Whether to print formatted time
-_45        strings with subsecond resolution or not."""
-_46        self._start_time = time.time()
-_47        self._stop_time = self.start_time
-_48        self._elapsed = 0
-_49        self._average_elapsed = 0
-_50        self._history: list[float] = []
-_51        self._started: bool = False
-_52        self.averaging_window_length: int = averaging_window_length
-_53        self.subsecond_resolution = subsecond_resolution
-_54
-_55    @property
-_56    def started(self) -> bool:
-_57        """Returns whether the timer has
-_58        been started and is currently running."""
-_59        return self._started
-_60
-_61    @property
-_62    def elapsed(self) -> float:
-_63        """Return the currently elapsed time."""
-_64        if self._started:
-_65            return time.time() - self._start_time
-_66        else:
-_67            return self._elapsed
-_68
-_69    @property
-_70    def elapsed_str(self) -> str:
-_71        """Return the currently elapsed time
-_72        as a formatted string."""
-_73        return self.format_time(self.elapsed, self.subsecond_resolution)
-_74
-_75    @property
-_76    def average_elapsed(self) -> float:
-_77        return self._average_elapsed
-_78
-_79    @property
-_80    def average_elapsed_str(self) -> str:
-_81        return self.format_time(self._average_elapsed,
-self.subsecond_resolution)
+_67    ):
+_68        """
+_69        #### :params:
+_70        * `averaging_window_length`: Number of start/stop cycles to
+calculate the average elapsed time with.
+_71
+_72        * `subsecond_resolution`: Whether to print formatted time strings
+with subsecond resolution or not."""
+_73        self._start_time = time.time()
+_74        self._stop_time = self.start_time
+_75        self._elapsed = 0
+_76        self._average_elapsed = 0
+_77        self._history: list[float] = []
+_78        self._started: bool = False
+_79        self.averaging_window_length: int = averaging_window_length
+_80        self.subsecond_resolution = subsecond_resolution
+_81        self._pauser = _Pauser()
 _82
 _83    @property
-_84    def start_time(self) -> float:
-_85        return self._start_time
-_86
-_87    @property
-_88    def stop_time(self) -> float:
-_89        return self._stop_time
-_90
-_91    @property
-_92    def history(self) -> list[float]:
-_93        return self._history
-_94
-_95    def start(self: Self) -> Self:
-_96        """Start timer.
-_97        Returns this Timer instance so
-_98        timer start can be chained to
-_99        Timer creation.
+_84    def started(self) -> bool:
+_85        """Returns whether the timer has been started and is currently
+running."""
+_86        return self._started
+_87
+_88    @property
+_89    def elapsed(self) -> float:
+_90        """Returns the currently elapsed time."""
+_91        if self._started:
+_92            return time.time() - self._start_time - self._pauser.pause_total
+_93        else:
+_94            return self._elapsed
+_95
+_96    @property
+_97    def elapsed_str(self) -> str:
+_98        """Returns the currently elapsed time as a formatted string."""
+_99        return self.format_time(self.elapsed, self.subsecond_resolution)
 100
-101        >>> timer = Timer().start()"""
-102        self._start_time = time.time()
-103        self._started = True
-104        return self
+101    @property
+102    def average_elapsed(self) -> float:
+103        """Returns the average elapsed time."""
+104        return self._average_elapsed
 105
-106    def stop(self):
-107        """Stop timer.
-108
-109        Calculates elapsed time and average elapsed time."""
-110        self._stop_time = time.time()
-111        self._started = False
-112        self._elapsed = self._stop_time - self._start_time
-113        self._save_elapsed_time()
-114        self._average_elapsed = sum(self._history) / (len(self._history))
+106    @property
+107    def average_elapsed_str(self) -> str:
+108        """Returns the average elapsed time as a formatted string."""
+109        return self.format_time(self._average_elapsed,
+self.subsecond_resolution)
+110
+111    @property
+112    def start_time(self) -> float:
+113        """Returns the timestamp of the last call to `start()`."""
+114        return self._start_time
 115
-116    def _save_elapsed_time(self):
-117        """Saves current elapsed time to the history buffer
-118        in a FIFO manner."""
-119        if len(self._history) >= self.averaging_window_length:
-120            self._history.pop(0)
-121        self._history.append(self._elapsed)
-122
-123    @staticmethod
-124    def format_time(num_seconds: float, subsecond_resolution: bool = False)
+116    @property
+117    def stop_time(self) -> float:
+118        """Returns the timestamp of the last call to `stop()`."""
+119        return self._stop_time
+120
+121    @property
+122    def history(self) -> list[float]:
+123        """Returns the history buffer for this timer.
+124
+125        At most, it will be `averaging_window_length` elements long."""
+126        return self._history
+127
+128    def start(self: Self) -> Self:
+129        """Start the timer.
+130
+131        Returns this Timer instance so timer start can be chained to Timer
+creation if desired.
+132
+133        >>> timer = Timer().start()"""
+134        if not self.started:
+135            self._start_time = time.time()
+136            self._started = True
+137        return self
+138
+139    def stop(self):
+140        """Stop the timer.
+141
+142        Calculates elapsed time and average elapsed time."""
+143        if self.started:
+144            self._stop_time = time.time()
+145            self._started = False
+146            self._elapsed = (
+147                self._stop_time - self._start_time -
+self._pauser.pause_total
+148            )
+149            self._pauser.reset()
+150            self._save_elapsed_time()
+151            self._average_elapsed = sum(self._history) / (len
+(self._history))
+152
+153    def pause(self):
+154        """Pause the timer."""
+155        self._pauser.pause()
+156
+157    def unpause(self):
+158        """Unpause the timer."""
+159        self._pauser.unpause()
+160
+161    def _save_elapsed_time(self):
+162        """Saves current elapsed time to the history buffer in a FIFO
+manner."""
+163        if len(self._history) >= self.averaging_window_length:
+164            self._history.pop(0)
+165        self._history.append(self._elapsed)
+166
+167    @staticmethod
+168    def format_time(num_seconds: float, subsecond_resolution: bool = False)
 -> str:
-125        """Returns num_seconds as a string with units.
-126
-127        :param subsecond_resolution: Include milliseconds
-128        and microseconds with the output."""
-129        microsecond = 0.000001
-130        millisecond = 0.001
-131        second = 1
-132        seconds_per_minute = 60
-133        seconds_per_hour = 3600
-134        seconds_per_day = 86400
-135        seconds_per_week = 604800
-136        seconds_per_month = 2419200
-137        seconds_per_year = 29030400
-138        time_units = [
-139            (seconds_per_year, "y"),
-140            (seconds_per_month, "mn"),
-141            (seconds_per_week, "w"),
-142            (seconds_per_day, "d"),
-143            (seconds_per_hour, "h"),
-144            (seconds_per_minute, "m"),
-145            (second, "s"),
-146            (millisecond, "ms"),
-147            (microsecond, "us"),
-148        ]
-149        if not subsecond_resolution:
-150            time_units = time_units[:-2]
-151        time_string = ""
-152        for time_unit in time_units:
-153            unit_amount, num_seconds = divmod(num_seconds, time_unit[0])
-154            if unit_amount > 0:
-155                time_string += f"{int(unit_amount)}{time_unit[1]} "
-156        if time_string == "":
-157            return f"<1{time_units[-1][1]}"
-158        return time_string.strip()
-159
-160    @property
-161    def stats(self) -> str:
-162        """Returns a string stating the currently elapsed time
-163        and the average elapsed time."""
-164        return f"elapsed time: {self.elapsed_str}\naverage elapsed time:
+169        """Returns `num_seconds` as a string with units.
+170
+171        #### :params:
+172
+173        `subsecond_resolution`: Include milliseconds and microseconds with
+the output."""
+174        microsecond = 0.000001
+175        millisecond = 0.001
+176        second = 1
+177        seconds_per_minute = 60
+178        seconds_per_hour = 3600
+179        seconds_per_day = 86400
+180        seconds_per_week = 604800
+181        seconds_per_month = 2419200
+182        seconds_per_year = 29030400
+183        time_units = [
+184            (seconds_per_year, "y"),
+185            (seconds_per_month, "mn"),
+186            (seconds_per_week, "w"),
+187            (seconds_per_day, "d"),
+188            (seconds_per_hour, "h"),
+189            (seconds_per_minute, "m"),
+190            (second, "s"),
+191            (millisecond, "ms"),
+192            (microsecond, "us"),
+193        ]
+194        if not subsecond_resolution:
+195            time_units = time_units[:-2]
+196        time_string = ""
+197        for time_unit in time_units:
+198            unit_amount, num_seconds = divmod(num_seconds, time_unit[0])
+199            if unit_amount > 0:
+200                time_string += f"{int(unit_amount)}{time_unit[1]} "
+201        if time_string == "":
+202            return f"<1{time_units[-1][1]}"
+203        return time_string.strip()
+204
+205    @property
+206    def stats(self) -> str:
+207        """Returns a string stating the currently elapsed time and the
+average elapsed time."""
+208        return f"elapsed time: {self.elapsed_str}\naverage elapsed time:
 {self.average_elapsed_str}"
 Simple timer class that tracks total elapsed time and average time between
-calls to 'start' and 'stop'.
+calls to start() and stop().
 ⁰
 Timer(averaging_window_length: int = 10, subsecond_resolution: bool = True)
 View Source
-38    def __init__(
-39        self, averaging_window_length: int = 10, subsecond_resolution: bool =
+65    def __init__(
+66        self, averaging_window_length: int = 10, subsecond_resolution: bool =
 True
-40    ):
-41        """:param averaging_window_length: Number of start/stop cycles
-42        to calculate the average elapsed time with.
-43
-44        :param subsecond_resolution: Whether to print formatted time
-45        strings with subsecond resolution or not."""
-46        self._start_time = time.time()
-47        self._stop_time = self.start_time
-48        self._elapsed = 0
-49        self._average_elapsed = 0
-50        self._history: list[float] = []
-51        self._started: bool = False
-52        self.averaging_window_length: int = averaging_window_length
-53        self.subsecond_resolution = subsecond_resolution
-* Parameters *
+67    ):
+68        """
+69        #### :params:
+70        * `averaging_window_length`: Number of start/stop cycles to calculate
+the average elapsed time with.
+71
+72        * `subsecond_resolution`: Whether to print formatted time strings
+with subsecond resolution or not."""
+73        self._start_time = time.time()
+74        self._stop_time = self.start_time
+75        self._elapsed = 0
+76        self._average_elapsed = 0
+77        self._history: list[float] = []
+78        self._started: bool = False
+79        self.averaging_window_length: int = averaging_window_length
+80        self.subsecond_resolution = subsecond_resolution
+81        self._pauser = _Pauser()
+*** :params: ***
     * averaging_window_length: Number of start/stop cycles to calculate the
       average elapsed time with.
     * subsecond_resolution: Whether to print formatted time strings with
       subsecond resolution or not.
 started: bool
 Returns whether the timer has been started and is currently running.
 elapsed: float
-Return the currently elapsed time.
+Returns the currently elapsed time.
 elapsed_str: str
-Return the currently elapsed time as a formatted string.
+Returns the currently elapsed time as a formatted string.
+average_elapsed: float
+Returns the average elapsed time.
+average_elapsed_str: str
+Returns the average elapsed time as a formatted string.
+start_time: float
+Returns the timestamp of the last call to start().
+stop_time: float
+Returns the timestamp of the last call to stop().
+history: list[float]
+Returns the history buffer for this timer.
+At most, it will be averaging_window_length elements long.
 ⁰
 def start(self: Self) -> Self: View Source
-_95    def start(self: Self) -> Self:
-_96        """Start timer.
-_97        Returns this Timer instance so
-_98        timer start can be chained to
-_99        Timer creation.
-100
-101        >>> timer = Timer().start()"""
-102        self._start_time = time.time()
-103        self._started = True
-104        return self
-Start timer. Returns this Timer instance so timer start can be chained to Timer
-creation.
+128    def start(self: Self) -> Self:
+129        """Start the timer.
+130
+131        Returns this Timer instance so timer start can be chained to Timer
+creation if desired.
+132
+133        >>> timer = Timer().start()"""
+134        if not self.started:
+135            self._start_time = time.time()
+136            self._started = True
+137        return self
+Start the timer.
+Returns this Timer instance so timer start can be chained to Timer creation if
+desired.
 >>> timer = Timer().start()
 ⁰
 def stop(self): View Source
-106    def stop(self):
-107        """Stop timer.
-108
-109        Calculates elapsed time and average elapsed time."""
-110        self._stop_time = time.time()
-111        self._started = False
-112        self._elapsed = self._stop_time - self._start_time
-113        self._save_elapsed_time()
-114        self._average_elapsed = sum(self._history) / (len(self._history))
-Stop timer.
+139    def stop(self):
+140        """Stop the timer.
+141
+142        Calculates elapsed time and average elapsed time."""
+143        if self.started:
+144            self._stop_time = time.time()
+145            self._started = False
+146            self._elapsed = (
+147                self._stop_time - self._start_time -
+self._pauser.pause_total
+148            )
+149            self._pauser.reset()
+150            self._save_elapsed_time()
+151            self._average_elapsed = sum(self._history) / (len
+(self._history))
+Stop the timer.
 Calculates elapsed time and average elapsed time.
 ⁰
+def pause(self): View Source
+153    def pause(self):
+154        """Pause the timer."""
+155        self._pauser.pause()
+Pause the timer.
+⁰
+def unpause(self): View Source
+157    def unpause(self):
+158        """Unpause the timer."""
+159        self._pauser.unpause()
+Unpause the timer.
+⁰
 @staticmethod
 def format_time(num_seconds: float, subsecond_resolution: bool = False) -> str:
 View Source
-123    @staticmethod
-124    def format_time(num_seconds: float, subsecond_resolution: bool = False)
+167    @staticmethod
+168    def format_time(num_seconds: float, subsecond_resolution: bool = False)
 -> str:
-125        """Returns num_seconds as a string with units.
-126
-127        :param subsecond_resolution: Include milliseconds
-128        and microseconds with the output."""
-129        microsecond = 0.000001
-130        millisecond = 0.001
-131        second = 1
-132        seconds_per_minute = 60
-133        seconds_per_hour = 3600
-134        seconds_per_day = 86400
-135        seconds_per_week = 604800
-136        seconds_per_month = 2419200
-137        seconds_per_year = 29030400
-138        time_units = [
-139            (seconds_per_year, "y"),
-140            (seconds_per_month, "mn"),
-141            (seconds_per_week, "w"),
-142            (seconds_per_day, "d"),
-143            (seconds_per_hour, "h"),
-144            (seconds_per_minute, "m"),
-145            (second, "s"),
-146            (millisecond, "ms"),
-147            (microsecond, "us"),
-148        ]
-149        if not subsecond_resolution:
-150            time_units = time_units[:-2]
-151        time_string = ""
-152        for time_unit in time_units:
-153            unit_amount, num_seconds = divmod(num_seconds, time_unit[0])
-154            if unit_amount > 0:
-155                time_string += f"{int(unit_amount)}{time_unit[1]} "
-156        if time_string == "":
-157            return f"<1{time_units[-1][1]}"
-158        return time_string.strip()
+169        """Returns `num_seconds` as a string with units.
+170
+171        #### :params:
+172
+173        `subsecond_resolution`: Include milliseconds and microseconds with
+the output."""
+174        microsecond = 0.000001
+175        millisecond = 0.001
+176        second = 1
+177        seconds_per_minute = 60
+178        seconds_per_hour = 3600
+179        seconds_per_day = 86400
+180        seconds_per_week = 604800
+181        seconds_per_month = 2419200
+182        seconds_per_year = 29030400
+183        time_units = [
+184            (seconds_per_year, "y"),
+185            (seconds_per_month, "mn"),
+186            (seconds_per_week, "w"),
+187            (seconds_per_day, "d"),
+188            (seconds_per_hour, "h"),
+189            (seconds_per_minute, "m"),
+190            (second, "s"),
+191            (millisecond, "ms"),
+192            (microsecond, "us"),
+193        ]
+194        if not subsecond_resolution:
+195            time_units = time_units[:-2]
+196        time_string = ""
+197        for time_unit in time_units:
+198            unit_amount, num_seconds = divmod(num_seconds, time_unit[0])
+199            if unit_amount > 0:
+200                time_string += f"{int(unit_amount)}{time_unit[1]} "
+201        if time_string == "":
+202            return f"<1{time_units[-1][1]}"
+203        return time_string.strip()
 Returns num_seconds as a string with units.
-* Parameters *
-    * subsecond_resolution: Include milliseconds and microseconds with the
-      output.
+*** :params: ***
+subsecond_resolution: Include milliseconds and microseconds with the output.
 stats: str
 Returns a string stating the currently elapsed time and the average elapsed
 time.
```

### Comparing `noiftimer-2.0.0/LICENSE.txt` & `noiftimer-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `noiftimer-2.0.0/README.md` & `noiftimer-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `noiftimer-2.0.0/pyproject.toml` & `noiftimer-2.1.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "noiftimer"
 authors = [{name="Matt Manes"}]
 description = "Timing class for measuring elapsed time and average elapsed time."
-version = "2.0.0"
-requires-python = ">=3.9"
+version = "2.1.0"
+requires-python = ">=3.10"
 dependencies = ["pytest", "typing_extensions"]
 readme = "README.md"
 keywords = [
     "timer",
     "timing"
 ]
 classifiers = [
```

### Comparing `noiftimer-2.0.0/PKG-INFO` & `noiftimer-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: noiftimer
-Version: 2.0.0
+Version: 2.1.0
 Summary: Timing class for measuring elapsed time and average elapsed time.
 Project-URL: Homepage, https://github.com/matt-manes/noiftimer
 Project-URL: Documentation, https://github.com/matt-manes/noiftimer/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/noiftimer/tree/main/src/noiftimer
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: timer,timing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Requires-Dist: pytest
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # noiftimer
 Simple timer class to track elapsed time.<br>
 Install with:
```

