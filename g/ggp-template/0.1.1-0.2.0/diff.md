# Comparing `tmp/ggp_template-0.1.1.tar.gz` & `tmp/ggp_template-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ggp_template-0.1.1.tar", last modified: Wed May  3 04:12:08 2023, max compression
+gzip compressed data, was "ggp_template-0.2.0.tar", last modified: Thu May 11 08:05:53 2023, max compression
```

## Comparing `ggp_template-0.1.1.tar` & `ggp_template-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 04:12:08.403733 ggp_template-0.1.1/
--rw-rw-rw-   0        0        0     1094 2023-05-02 20:29:31.000000 ggp_template-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2979 2023-05-03 04:12:08.403733 ggp_template-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2424 2023-05-03 04:10:59.000000 ggp_template-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 04:12:08.387509 ggp_template-0.1.1/ggp/
--rw-rw-rw-   0        0        0        0 2023-05-02 19:58:45.000000 ggp_template-0.1.1/ggp/__init__.py
--rw-rw-rw-   0        0        0     1973 2023-05-03 04:06:12.000000 ggp_template-0.1.1/ggp/make.py
--rw-rw-rw-   0        0        0      637 2023-05-02 21:48:54.000000 ggp_template-0.1.1/ggp/new.py
-drwxrwxrwx   0        0        0        0 2023-05-03 04:12:08.391723 ggp_template-0.1.1/ggp/templates/
--rw-rw-rw-   0        0        0     2404 2023-05-02 19:59:54.000000 ggp_template-0.1.1/ggp/templates/sample.html
--rw-rw-rw-   0        0        0     1354 2023-05-02 20:00:31.000000 ggp_template-0.1.1/ggp/templates/sample.js
-drwxrwxrwx   0        0        0        0 2023-05-03 04:12:08.403733 ggp_template-0.1.1/ggp_template.egg-info/
--rw-rw-rw-   0        0        0     2979 2023-05-03 04:12:08.000000 ggp_template-0.1.1/ggp_template.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-03 04:12:08.000000 ggp_template-0.1.1/ggp_template.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 04:12:08.000000 ggp_template-0.1.1/ggp_template.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-03 04:12:08.000000 ggp_template-0.1.1/ggp_template.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      709 2023-05-03 04:11:49.000000 ggp_template-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 04:12:08.403733 ggp_template-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 08:05:53.421435 ggp_template-0.2.0/
+-rw-rw-rw-   0        0        0     1074 2023-05-03 04:22:58.000000 ggp_template-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4472 2023-05-11 08:05:53.420432 ggp_template-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3823 2023-05-11 07:50:47.000000 ggp_template-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 08:05:53.402431 ggp_template-0.2.0/ggp/
+-rw-rw-rw-   0        0        0        0 2023-05-03 04:22:58.000000 ggp_template-0.2.0/ggp/__init__.py
+-rw-rw-rw-   0        0        0     3136 2023-05-11 07:37:22.000000 ggp_template-0.2.0/ggp/make.py
+-rw-rw-rw-   0        0        0      621 2023-05-03 04:22:58.000000 ggp_template-0.2.0/ggp/new.py
+drwxrwxrwx   0        0        0        0 2023-05-11 08:05:53.406433 ggp_template-0.2.0/ggp/templates/
+-rw-rw-rw-   0        0        0     2452 2023-05-11 06:23:15.000000 ggp_template-0.2.0/ggp/templates/loadworker.js
+-rw-rw-rw-   0        0        0     2323 2023-05-03 04:22:58.000000 ggp_template-0.2.0/ggp/templates/sample.html
+-rw-rw-rw-   0        0        0     1302 2023-05-03 04:22:58.000000 ggp_template-0.2.0/ggp/templates/sample.js
+drwxrwxrwx   0        0        0        0 2023-05-11 08:05:53.419432 ggp_template-0.2.0/ggp_template.egg-info/
+-rw-rw-rw-   0        0        0     4472 2023-05-11 08:05:53.000000 ggp_template-0.2.0/ggp_template.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-05-11 08:05:53.000000 ggp_template-0.2.0/ggp_template.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 08:05:53.000000 ggp_template-0.2.0/ggp_template.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-11 08:05:53.000000 ggp_template-0.2.0/ggp_template.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      684 2023-05-11 08:05:25.000000 ggp_template-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 08:05:53.421435 ggp_template-0.2.0/setup.cfg
```

### Comparing `ggp_template-0.1.1/LICENSE` & `ggp_template-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Praneeth Kolichala
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Praneeth Kolichala
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `ggp_template-0.1.1/ggp/new.py` & `ggp_template-0.2.0/ggp/new.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from pathlib import Path
-from argparse import ArgumentParser, FileType
-
-base_template_path = Path(__file__).parent / "templates"
-
-with open((base_template_path / "sample.js").resolve()) as f:
-    sample_js = f.read()
-
-if __name__ == "__main__":
-    parser = ArgumentParser(
-                    prog='ggp.new',
-                    description='Automatically generate a template for your player')
-    parser.add_argument('out', help='The js file to write to (defaults to main.js)',
-                        type=FileType('w'), nargs='?', default='main.js')
-    args = parser.parse_args()
-    print(sample_js, file=args.out)
+from pathlib import Path
+from argparse import ArgumentParser, FileType
+
+base_template_path = Path(__file__).parent / "templates"
+
+with open((base_template_path / "sample.js").resolve()) as f:
+    sample_js = f.read()
+
+if __name__ == "__main__":
+    parser = ArgumentParser(
+                    prog='ggp.new',
+                    description='Automatically generate a template for your player')
+    parser.add_argument('out', help='The js file to write to (defaults to main.js)',
+                        type=FileType('w'), nargs='?', default='main.js')
+    args = parser.parse_args()
+    print(sample_js, file=args.out)
```

### Comparing `ggp_template-0.1.1/ggp/templates/sample.html` & `ggp_template-0.2.0/ggp/templates/sample.html`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-<html>
-
-<!--=======================================================================-->
-
-<head>
-  <title>$TITLE</title>
-  <script type='text/javascript' src='http://epilog.stanford.edu/javascript/epilog.js'></script>
-  <script type='text/javascript' src='http://gamemaster.stanford.edu/javascript/localstorage.js'></script>
-  <script type='text/javascript' src='http://gamemaster.stanford.edu/reasoning/general.js'></script>
-  <script type='text/javascript'>
-    var manager = 'manager';
-    var player = '$IDENT';
-  </script>
-$SCRIPTS
-</head>
-
-<!--=======================================================================-->
-
-<body bgcolor='#aabbbb' onload='doinitialize()'>
-  <center>
-    <table width='720' cellspacing='0' cellpadding='40' bgcolor='#ffffff'>
-      <tr>
-        <td>
-
-<!--=======================================================================-->
-
-<center>
-  <table width='640' cellpadding='0'>
-    <tr>
-      <td width='180' align='center' valign='center'>
-        <img width='130' src='http://gamemaster.stanford.edu/images/ggp.jpg'/>
-      </td>
-      <td align='center'>
-        <span style='font-size:18pt'>&nbsp;</span>
-        <span style='font-size:32pt'>Gamemaster</span><br/>
-      </td>
-      <td width='180' align='center' style='color:#000066;font-size:18px'>
-        <i>General<br/>Game<br/>Playing</i>
-      </td>
-    </tr>
-  </table>
-</center>
-
-<!--=======================================================================-->
-
-<br/>
-<table width='640' cellpadding='8' cellspacing='0' bgcolor='#f4f8f8' border='1'>
-  <tr height='40'>
-     <td align='center'>
-<table style='color:#000066;font-size:18px'>
-  <tr>
-    <td>
-Protocol: localstorage<br/>
-Strategy: $STRATEGY<br/>
-Identifier: <span id='player'>$IDENT</span> <img src="http://gamemaster.stanford.edu/images/pencil.gif" onclick='doplayer()'/>
-    </td>
-  </tr>
-</table>
-    </td>
-  </tr>
-</table>
-<br/>
-
-<!--=======================================================================-->
-
-<center>
-  <br/>
-  <textarea id='transcript' style='font-family:courier' rows='30' cols='80' readonly></textarea>
-</center>
-
-<!--=======================================================================-->
-
-        </td>
-      </tr>
-    </table>
-  </center>
-</body>
-
-<!--=======================================================================-->
-
-</html>
+<html>
+
+<!--=======================================================================-->
+
+<head>
+  <title>$TITLE</title>
+  <script type='text/javascript' src='http://epilog.stanford.edu/javascript/epilog.js'></script>
+  <script type='text/javascript' src='http://gamemaster.stanford.edu/javascript/localstorage.js'></script>
+  <script type='text/javascript' src='http://gamemaster.stanford.edu/reasoning/general.js'></script>
+  <script type='text/javascript'>
+    var manager = 'manager';
+    var player = '$IDENT';
+  </script>
+$SCRIPTS
+</head>
+
+<!--=======================================================================-->
+
+<body bgcolor='#aabbbb' onload='doinitialize()'>
+  <center>
+    <table width='720' cellspacing='0' cellpadding='40' bgcolor='#ffffff'>
+      <tr>
+        <td>
+
+<!--=======================================================================-->
+
+<center>
+  <table width='640' cellpadding='0'>
+    <tr>
+      <td width='180' align='center' valign='center'>
+        <img width='130' src='http://gamemaster.stanford.edu/images/ggp.jpg'/>
+      </td>
+      <td align='center'>
+        <span style='font-size:18pt'>&nbsp;</span>
+        <span style='font-size:32pt'>Gamemaster</span><br/>
+      </td>
+      <td width='180' align='center' style='color:#000066;font-size:18px'>
+        <i>General<br/>Game<br/>Playing</i>
+      </td>
+    </tr>
+  </table>
+</center>
+
+<!--=======================================================================-->
+
+<br/>
+<table width='640' cellpadding='8' cellspacing='0' bgcolor='#f4f8f8' border='1'>
+  <tr height='40'>
+     <td align='center'>
+<table style='color:#000066;font-size:18px'>
+  <tr>
+    <td>
+Protocol: localstorage<br/>
+Strategy: $STRATEGY<br/>
+Identifier: <span id='player'>$IDENT</span> <img src="http://gamemaster.stanford.edu/images/pencil.gif" onclick='doplayer()'/>
+    </td>
+  </tr>
+</table>
+    </td>
+  </tr>
+</table>
+<br/>
+
+<!--=======================================================================-->
+
+<center>
+  <br/>
+  <textarea id='transcript' style='font-family:courier' rows='30' cols='80' readonly></textarea>
+</center>
+
+<!--=======================================================================-->
+
+        </td>
+      </tr>
+    </table>
+  </center>
+</body>
+
+<!--=======================================================================-->
+
+</html>
```

### Comparing `ggp_template-0.1.1/ggp/templates/sample.js` & `ggp_template-0.2.0/ggp/templates/sample.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,52 +1,52 @@
-//==============================================================================
-// The code below defines a basic legal player.
-// Autogenerated by ggp_template.py
-// Replace the definitions of ping, start, play, stop, abort with your code.
-//==============================================================================
-
-var role = 'robot';
-var startclock = 10;
-var playclock = 10;
-
-var library = [];
-var roles = [];
-var state = [];
-var move = 'nil';
-
-//==============================================================================
-
-function ping() {
-    return 'ready'
-}
-
-function start(r, rs, sc, pc) {
-    role = r;
-    library = definemorerules([], rs.slice(1));
-    roles = findroles(library);
-    state = findinits(library);
-    startclock = numberize(sc);
-    playclock = numberize(pc);
-    return 'ready'
-}
-
-function play(move) {
-    if (move !== nil) {
-        state = simulate(move, state, library)
-    };
-    if (findcontrol(state, library) !== role) {
-        return false
-    };
-    return findlegalx(state, library)
-}
-
-function stop(move) {
-    return false
-}
-
-function abort() {
-    return false
-}
-
-//==============================================================================
-// End of player code
+//==============================================================================
+// The code below defines a basic legal player.
+// Autogenerated by ggp_template.py
+// Replace the definitions of ping, start, play, stop, abort with your code.
+//==============================================================================
+
+var role = 'robot';
+var startclock = 10;
+var playclock = 10;
+
+var library = [];
+var roles = [];
+var state = [];
+var move = 'nil';
+
+//==============================================================================
+
+function ping() {
+    return 'ready'
+}
+
+function start(r, rs, sc, pc) {
+    role = r;
+    library = definemorerules([], rs.slice(1));
+    roles = findroles(library);
+    state = findinits(library);
+    startclock = numberize(sc);
+    playclock = numberize(pc);
+    return 'ready'
+}
+
+function play(move) {
+    if (move !== nil) {
+        state = simulate(move, state, library)
+    };
+    if (findcontrol(state, library) !== role) {
+        return false
+    };
+    return findlegalx(state, library)
+}
+
+function stop(move) {
+    return false
+}
+
+function abort() {
+    return false
+}
+
+//==============================================================================
+// End of player code
 //==============================================================================
```

