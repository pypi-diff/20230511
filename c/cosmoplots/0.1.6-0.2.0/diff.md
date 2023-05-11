# Comparing `tmp/cosmoplots-0.1.6.tar.gz` & `tmp/cosmoplots-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmoplots-0.1.6.tar", max compression
+gzip compressed data, was "cosmoplots-0.2.0.tar", max compression
```

## Comparing `cosmoplots-0.1.6.tar` & `cosmoplots-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1076 2022-05-31 13:01:50.152224 cosmoplots-0.1.6/LICENSE
--rw-r--r--   0        0        0     2487 2022-05-31 13:01:50.152224 cosmoplots-0.1.6/README.md
--rw-r--r--   0        0        0       70 2022-05-31 13:02:03.372234 cosmoplots-0.1.6/cosmoplots/__init__.py
--rw-r--r--   0        0        0     1874 2022-05-31 13:01:50.156224 cosmoplots-0.1.6/cosmoplots/axes.py
--rw-r--r--   0        0        0     5516 2022-05-31 13:01:50.156224 cosmoplots-0.1.6/cosmoplots/figure_defs.py
--rw-r--r--   0        0        0      485 2022-05-31 13:02:03.372234 cosmoplots-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3302 2022-05-31 13:02:05.997168 cosmoplots-0.1.6/setup.py
--rw-r--r--   0        0        0     3143 2022-05-31 13:02:05.997508 cosmoplots-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-11 11:59:16.709257 cosmoplots-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3463 2023-05-11 11:59:16.709257 cosmoplots-0.2.0/README.md
+-rw-r--r--   0        0        0       92 2023-05-11 11:59:16.713257 cosmoplots-0.2.0/cosmoplots/__init__.py
+-rw-r--r--   0        0        0     1874 2023-05-11 11:59:16.713257 cosmoplots-0.2.0/cosmoplots/axes.py
+-rw-r--r--   0        0        0     2723 2023-05-11 11:59:29.221358 cosmoplots-0.2.0/cosmoplots/colors.py
+-rw-r--r--   0        0        0     5516 2023-05-11 11:59:16.713257 cosmoplots-0.2.0/cosmoplots/figure_defs.py
+-rw-r--r--   0        0        0      485 2023-05-11 11:59:29.221358 cosmoplots-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4170 1970-01-01 00:00:00.000000 cosmoplots-0.2.0/PKG-INFO
```

### Comparing `cosmoplots-0.1.6/LICENSE` & `cosmoplots-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.1.6/cosmoplots/axes.py` & `cosmoplots-0.2.0/cosmoplots/axes.py`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.1.6/cosmoplots/figure_defs.py` & `cosmoplots-0.2.0/cosmoplots/figure_defs.py`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.1.6/setup.py` & `cosmoplots-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,122 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+# cosmoplots
 
-packages = \
-['cosmoplots']
+Routines to get a sane default configuration for production quality plots. Used by complex systems modelling group at UiT.
 
-package_data = \
-{'': ['*']}
+## Installation
 
-install_requires = \
-['matplotlib>=3.3.2', 'numpy>=1.15.0']
-
-setup_kwargs = {
-    'name': 'cosmoplots',
-    'version': '0.1.6',
-    'description': 'Routines to get a sane default configuration for production quality plots.',
-    'long_description': '# cosmoplots\n\nRoutines to get a sane default configuration for production quality plots. Used by complex systems modelling group at UiT.\n\n## Installation\n\nThe package is published to PyPI and can be installed with\n\n```sh\npip install cosmoplots\n```\n\nIf you want the development version you must first clone the repo to your local machine,\nthen install the project and its dependencies with [poetry]:\n\n```sh\ngit clone https://github.com/uit-cosmo/cosmoplots.git\ncd cosmoplots\npoetry install\n```\n\n## Usage\n\nSet your `rcparams` before plotting in your code, for example:\n\n```Python\nimport cosmoplots\n\naxes_size = cosmoplots.set_rcparams_dynamo(plt.rcParams, num_cols=1, ls="thin")\n```\n\n## `change_log_axis_base`\n\n```python\nimport matplotlib.pyplot as plt\nimport numpy as np\nimport cosmoplots\n\naxes_size = cosmoplots.set_rcparams_dynamo(plt.rcParams, num_cols=1, ls="thin")\na = np.exp(np.linspace(-3, 5, 100))\nfig = plt.figure()\nax = fig.add_axes(axes_size)\nax.set_xlabel("X Axis")\nax.set_ylabel("Y Axis")\nbase = 2  # Default is 10, but 2 works equally well\ncosmoplots.change_log_axis_base(ax, "x", base=base)\n# Do plotting ...\n# If you use "plot", the change_log_axis_base can be called at the top (along with add_axes\n# etc.), but using loglog, semilogx, semilogy will re-set, and the change_log_axis_base\n# function must be called again.\nax.plot(a)\nplt.show()\n```\n\n## `matplotlib` vs. `cosmoplots` defaults\n\n```python\nimport matplotlib.pyplot as plt\nimport numpy as np\nimport cosmoplots\n\n# Matplotlib --------------------------------------------------------------------------- #\na = np.exp(np.linspace(-3, 5, 100))\nfig = plt.figure()\nax = fig.add_subplot()\nax.set_xlabel("X Axis")\nax.set_ylabel("Y Axis")\nax.semilogy(a)\n# plt.savefig("assets/matplotlib.png")\nplt.show()\n\n# Cosmoplots --------------------------------------------------------------------------- #\naxes_size = cosmoplots.set_rcparams_dynamo(plt.rcParams, num_cols=1, ls="thin")\na = np.exp(np.linspace(-3, 5, 100))\nfig = plt.figure()\nax = fig.add_axes(axes_size)\nax.set_xlabel("X Axis")\nax.set_ylabel("Y Axis")\ncosmoplots.change_log_axis_base(ax, "y")\nax.semilogy(a)\n# Commenting out the below line result in the default base10 ticks\ncosmoplots.change_log_axis_base(ax, "y")\n# plt.savefig("assets/cosmoplots.png")\nplt.show()\n```\n\n| `matplotlib` | `cosmoplots` |\n| :--------: | :--------: |\n| ![matplotlib](./assets/matplotlib.png) | ![cosmoplots](./assets/cosmoplots.png) |\n\n<!-- Links -->\n[poetry]: https://python-poetry.org\n',
-    'author': 'gregordecristoforo',
-    'author_email': 'gregor.decristoforo@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/uit-cosmo/cosmoplots',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8',
-}
+The package is published to PyPI and can be installed with
 
-
-setup(**setup_kwargs)
+```sh
+pip install cosmoplots
+```
+
+If you want the development version you must first clone the repo to your local machine,
+then install the project and its dependencies with [poetry]:
+
+```sh
+git clone https://github.com/uit-cosmo/cosmoplots.git
+cd cosmoplots
+poetry install
+```
+
+## Usage
+
+Set your `rcparams` before plotting in your code, for example:
+
+```Python
+import cosmoplots
+
+axes_size = cosmoplots.set_rcparams_dynamo(plt.rcParams, num_cols=1, ls="thin")
+```
+
+## `change_log_axis_base`
+
+```python
+import matplotlib.pyplot as plt
+import numpy as np
+import cosmoplots
+
+axes_size = cosmoplots.set_rcparams_dynamo(plt.rcParams, num_cols=1, ls="thin")
+a = np.exp(np.linspace(-3, 5, 100))
+fig = plt.figure()
+ax = fig.add_axes(axes_size)
+ax.set_xlabel("X Axis")
+ax.set_ylabel("Y Axis")
+base = 2  # Default is 10, but 2 works equally well
+cosmoplots.change_log_axis_base(ax, "x", base=base)
+# Do plotting ...
+# If you use "plot", the change_log_axis_base can be called at the top (along with add_axes
+# etc.), but using loglog, semilogx, semilogy will re-set, and the change_log_axis_base
+# function must be called again.
+ax.plot(a)
+plt.show()
+```
+
+## `matplotlib` vs. `cosmoplots` defaults
+
+```python
+import matplotlib.pyplot as plt
+import numpy as np
+import cosmoplots
+
+# Matplotlib --------------------------------------------------------------------------- #
+a = np.exp(np.linspace(-3, 5, 100))
+fig = plt.figure()
+ax = fig.add_subplot()
+ax.set_xlabel("X Axis")
+ax.set_ylabel("Y Axis")
+ax.semilogy(a)
+# plt.savefig("assets/matplotlib.png")
+plt.show()
+
+# Cosmoplots --------------------------------------------------------------------------- #
+axes_size = cosmoplots.set_rcparams_dynamo(plt.rcParams, num_cols=1, ls="thin")
+a = np.exp(np.linspace(-3, 5, 100))
+fig = plt.figure()
+ax = fig.add_axes(axes_size)
+ax.set_xlabel("X Axis")
+ax.set_ylabel("Y Axis")
+cosmoplots.change_log_axis_base(ax, "y")
+ax.semilogy(a)
+# Commenting out the below line result in the default base10 ticks
+cosmoplots.change_log_axis_base(ax, "y")
+# plt.savefig("assets/cosmoplots.png")
+plt.show()
+```
+
+| `matplotlib` | `cosmoplots` |
+| :--------: | :--------: |
+| ![matplotlib](./assets/matplotlib.png) | ![cosmoplots](./assets/cosmoplots.png) |
+
+<!-- Links -->
+[poetry]: https://python-poetry.org
+
+
+## `generate_hex_colors`
+
+This function generates the hex numbers for the colours extracted from a `matplotlib` colour map based on the number of points of interest.
+The colors change gradually from bright to dark or vice versa.
+```python
+import matplotlib.pyplot as plt
+import cosmoplots
+
+axes_size = cosmoplots.set_rcparams_dynamo(plt.rcParams, num_cols=1, ls="thin")
+
+
+color_list = cosmoplots.generate_hex_colors(5, 'viridis', show_swatch=True, ascending=True)
+plt.savefig("./assets/hex_colors.png")
+
+# Print color_list to retrieve the hex numbers
+print(color_list) #['#fde725', '#5ec962', '#21918c', '#3b528b', '#440154']
+
+fig = plt.figure()
+ax = fig.add_axes(axes_size)
+for i, color in enumerate(color_list):
+    ax.plot([1,2],[i,i+1], c = color)
+
+plt.savefig("./assets/hex_colors_example.png")
+plt.show()
+```
+| `hex_colors.png` | hex_colors_example.png |
+| :--------: | :--------: | 
+| ![colors](./assets/hex_colors.png) | ![colors](./assets/hex_colors_example.png) |
```

### Comparing `cosmoplots-0.1.6/PKG-INFO` & `cosmoplots-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: cosmoplots
-Version: 0.1.6
+Version: 0.2.0
 Summary: Routines to get a sane default configuration for production quality plots.
 Home-page: https://github.com/uit-cosmo/cosmoplots
 License: MIT
 Author: gregordecristoforo
 Author-email: gregor.decristoforo@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.3.2)
 Requires-Dist: numpy (>=1.15.0)
 Description-Content-Type: text/markdown
 
 # cosmoplots
 
 Routines to get a sane default configuration for production quality plots. Used by complex systems modelling group at UiT.
@@ -105,7 +106,37 @@
 | `matplotlib` | `cosmoplots` |
 | :--------: | :--------: |
 | ![matplotlib](./assets/matplotlib.png) | ![cosmoplots](./assets/cosmoplots.png) |
 
 <!-- Links -->
 [poetry]: https://python-poetry.org
 
+
+## `generate_hex_colors`
+
+This function generates the hex numbers for the colours extracted from a `matplotlib` colour map based on the number of points of interest.
+The colors change gradually from bright to dark or vice versa.
+```python
+import matplotlib.pyplot as plt
+import cosmoplots
+
+axes_size = cosmoplots.set_rcparams_dynamo(plt.rcParams, num_cols=1, ls="thin")
+
+
+color_list = cosmoplots.generate_hex_colors(5, 'viridis', show_swatch=True, ascending=True)
+plt.savefig("./assets/hex_colors.png")
+
+# Print color_list to retrieve the hex numbers
+print(color_list) #['#fde725', '#5ec962', '#21918c', '#3b528b', '#440154']
+
+fig = plt.figure()
+ax = fig.add_axes(axes_size)
+for i, color in enumerate(color_list):
+    ax.plot([1,2],[i,i+1], c = color)
+
+plt.savefig("./assets/hex_colors_example.png")
+plt.show()
+```
+| `hex_colors.png` | hex_colors_example.png |
+| :--------: | :--------: | 
+| ![colors](./assets/hex_colors.png) | ![colors](./assets/hex_colors_example.png) |
+
```

