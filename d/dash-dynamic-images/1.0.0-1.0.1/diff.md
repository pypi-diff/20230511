# Comparing `tmp/dash-dynamic-images-1.0.0.tar.gz` & `tmp/dash-dynamic-images-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash-dynamic-images-1.0.0.tar", last modified: Thu May 11 15:09:18 2023, max compression
+gzip compressed data, was "dash-dynamic-images-1.0.1.tar", last modified: Thu May 11 16:47:50 2023, max compression
```

## Comparing `dash-dynamic-images-1.0.0.tar` & `dash-dynamic-images-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 15:09:18.503028 dash-dynamic-images-1.0.0/
--rw-rw-rw-   0        0        0     1090 2023-05-08 13:34:42.000000 dash-dynamic-images-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4600 2023-05-11 15:09:18.502030 dash-dynamic-images-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3973 2023-05-11 08:13:14.000000 dash-dynamic-images-1.0.0/README.md
--rw-rw-rw-   0        0        0      981 2023-05-11 07:52:05.000000 dash-dynamic-images-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-11 15:09:18.503028 dash-dynamic-images-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-11 15:09:18.447823 dash-dynamic-images-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-11 15:09:18.469030 dash-dynamic-images-1.0.0/src/dash_dynamic_images/
--rw-rw-rw-   0        0        0       68 2023-05-09 14:26:03.000000 dash-dynamic-images-1.0.0/src/dash_dynamic_images/__init__.py
--rw-rw-rw-   0        0        0     1200 2023-05-10 14:22:23.000000 dash-dynamic-images-1.0.0/src/dash_dynamic_images/_callback.py
--rw-rw-rw-   0        0        0     1495 2023-05-10 14:21:31.000000 dash-dynamic-images-1.0.0/src/dash_dynamic_images/_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:09:18.499029 dash-dynamic-images-1.0.0/src/dash_dynamic_images.egg-info/
--rw-rw-rw-   0        0        0     4600 2023-05-11 15:09:18.000000 dash-dynamic-images-1.0.0/src/dash_dynamic_images.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-05-11 15:09:18.000000 dash-dynamic-images-1.0.0/src/dash_dynamic_images.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 15:09:18.000000 dash-dynamic-images-1.0.0/src/dash_dynamic_images.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-11 15:09:18.000000 dash-dynamic-images-1.0.0/src/dash_dynamic_images.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-11 15:09:18.000000 dash-dynamic-images-1.0.0/src/dash_dynamic_images.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-11 15:09:18.500026 dash-dynamic-images-1.0.0/tests/
--rw-rw-rw-   0        0        0     2688 2023-05-10 14:45:56.000000 dash-dynamic-images-1.0.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:47:50.612579 dash-dynamic-images-1.0.1/
+-rw-rw-rw-   0        0        0     1090 2023-05-08 13:34:42.000000 dash-dynamic-images-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     4639 2023-05-11 16:47:50.612579 dash-dynamic-images-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4012 2023-05-11 15:14:50.000000 dash-dynamic-images-1.0.1/README.md
+-rw-rw-rw-   0        0        0      981 2023-05-11 16:47:22.000000 dash-dynamic-images-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 16:47:50.612579 dash-dynamic-images-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 16:47:50.565492 dash-dynamic-images-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 16:47:50.587392 dash-dynamic-images-1.0.1/src/dash_dynamic_images/
+-rw-rw-rw-   0        0        0       68 2023-05-09 14:26:03.000000 dash-dynamic-images-1.0.1/src/dash_dynamic_images/__init__.py
+-rw-rw-rw-   0        0        0     1200 2023-05-10 14:22:23.000000 dash-dynamic-images-1.0.1/src/dash_dynamic_images/_callback.py
+-rw-rw-rw-   0        0        0     1495 2023-05-10 14:21:31.000000 dash-dynamic-images-1.0.1/src/dash_dynamic_images/_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:47:50.612579 dash-dynamic-images-1.0.1/src/dash_dynamic_images.egg-info/
+-rw-rw-rw-   0        0        0     4639 2023-05-11 16:47:50.000000 dash-dynamic-images-1.0.1/src/dash_dynamic_images.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-05-11 16:47:50.000000 dash-dynamic-images-1.0.1/src/dash_dynamic_images.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 16:47:50.000000 dash-dynamic-images-1.0.1/src/dash_dynamic_images.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-11 16:47:50.000000 dash-dynamic-images-1.0.1/src/dash_dynamic_images.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-11 16:47:50.000000 dash-dynamic-images-1.0.1/src/dash_dynamic_images.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 16:47:50.612579 dash-dynamic-images-1.0.1/tests/
+-rw-rw-rw-   0        0        0     2688 2023-05-10 14:45:56.000000 dash-dynamic-images-1.0.1/tests/test_utils.py
```

### Comparing `dash-dynamic-images-1.0.0/LICENSE` & `dash-dynamic-images-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dash-dynamic-images-1.0.0/PKG-INFO` & `dash-dynamic-images-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-dynamic-images
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library that helps with embedding dynamic and generative images into Plotly Dash applications.
 Author-email: Tomasz Rewak <tomasz.rewak@gmail.com>
 Project-URL: Homepage, https://github.com/TomaszRewak/dash-dynamic-images
 Project-URL: Bug Tracker, https://github.com/TomaszRewak/dash-dynamic-images/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -90,14 +90,15 @@
 A complete example of an application:
 
 ```python
 import dash
 import dash_core_components as dcc
 import dash_html_components as html
 from dash_dynamic_images import image_callback
+from PIL import Image, ImageDraw
 
 
 app = dash.Dash()
 app.layout = html.Div(children=[
     html.Img(id='image'),
     dcc.Input(id='x', type='number', value=10),
     dcc.Input(id='y', type='number', value=10)
@@ -108,15 +109,15 @@
     app,
     dash.Output('image', 'src'),
     dash.Input('x', 'value'),
     dash.Input('y', 'value'))
 def generate_image(x, y):
     image = Image.new('RGB', (200, 200), color=(0, 0, 200))
     ImageDraw.Draw(image).line([(0, 0), (x, y)], width=5)
-    return 
+    return image
 
 
 if __name__ == '__main__':
     app.run_server(debug=True)
 ```
 
 # How it works
```

### Comparing `dash-dynamic-images-1.0.0/README.md` & `dash-dynamic-images-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 A complete example of an application:
 
 ```python
 import dash
 import dash_core_components as dcc
 import dash_html_components as html
 from dash_dynamic_images import image_callback
+from PIL import Image, ImageDraw
 
 
 app = dash.Dash()
 app.layout = html.Div(children=[
     html.Img(id='image'),
     dcc.Input(id='x', type='number', value=10),
     dcc.Input(id='y', type='number', value=10)
@@ -94,15 +95,15 @@
     app,
     dash.Output('image', 'src'),
     dash.Input('x', 'value'),
     dash.Input('y', 'value'))
 def generate_image(x, y):
     image = Image.new('RGB', (200, 200), color=(0, 0, 200))
     ImageDraw.Draw(image).line([(0, 0), (x, y)], width=5)
-    return 
+    return image
 
 
 if __name__ == '__main__':
     app.run_server(debug=True)
 ```
 
 # How it works
```

### Comparing `dash-dynamic-images-1.0.0/pyproject.toml` & `dash-dynamic-images-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dash-dynamic-images"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name="Tomasz Rewak", email="tomasz.rewak@gmail.com" },
 ]
 description = "A library that helps with embedding dynamic and generative images into Plotly Dash applications."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dash-dynamic-images-1.0.0/src/dash_dynamic_images/_callback.py` & `dash-dynamic-images-1.0.1/src/dash_dynamic_images/_callback.py`

 * *Files identical despite different names*

### Comparing `dash-dynamic-images-1.0.0/src/dash_dynamic_images/_utils.py` & `dash-dynamic-images-1.0.1/src/dash_dynamic_images/_utils.py`

 * *Files identical despite different names*

### Comparing `dash-dynamic-images-1.0.0/src/dash_dynamic_images.egg-info/PKG-INFO` & `dash-dynamic-images-1.0.1/src/dash_dynamic_images.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-dynamic-images
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library that helps with embedding dynamic and generative images into Plotly Dash applications.
 Author-email: Tomasz Rewak <tomasz.rewak@gmail.com>
 Project-URL: Homepage, https://github.com/TomaszRewak/dash-dynamic-images
 Project-URL: Bug Tracker, https://github.com/TomaszRewak/dash-dynamic-images/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -90,14 +90,15 @@
 A complete example of an application:
 
 ```python
 import dash
 import dash_core_components as dcc
 import dash_html_components as html
 from dash_dynamic_images import image_callback
+from PIL import Image, ImageDraw
 
 
 app = dash.Dash()
 app.layout = html.Div(children=[
     html.Img(id='image'),
     dcc.Input(id='x', type='number', value=10),
     dcc.Input(id='y', type='number', value=10)
@@ -108,15 +109,15 @@
     app,
     dash.Output('image', 'src'),
     dash.Input('x', 'value'),
     dash.Input('y', 'value'))
 def generate_image(x, y):
     image = Image.new('RGB', (200, 200), color=(0, 0, 200))
     ImageDraw.Draw(image).line([(0, 0), (x, y)], width=5)
-    return 
+    return image
 
 
 if __name__ == '__main__':
     app.run_server(debug=True)
 ```
 
 # How it works
```

### Comparing `dash-dynamic-images-1.0.0/tests/test_utils.py` & `dash-dynamic-images-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

