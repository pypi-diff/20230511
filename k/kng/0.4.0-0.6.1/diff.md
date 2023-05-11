# Comparing `tmp/kng-0.4.0.tar.gz` & `tmp/kng-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kng-0.4.0.tar", max compression
+gzip compressed data, was "kng-0.6.1.tar", max compression
```

## Comparing `kng-0.4.0.tar` & `kng-0.6.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1066 2023-01-30 10:13:58.966160 kng-0.4.0/LICENSE
--rw-r--r--   0        0        0     1332 2023-03-06 02:47:55.579784 kng-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-01-30 10:14:35.543763 kng-0.4.0/kng/__init__.py
--rw-r--r--   0        0        0      533 2023-03-14 09:45:39.376053 kng-0.4.0/kng/dt.py
--rw-r--r--   0        0        0      769 2023-03-14 10:43:33.274166 kng-0.4.0/kng/iter.py
--rw-r--r--   0        0        0      572 2023-03-14 08:27:44.288414 kng-0.4.0/kng/misc.py
--rw-r--r--   0        0        0     1232 2023-03-14 10:52:28.510126 kng-0.4.0/kng/pd.py
--rw-r--r--   0        0        0      389 2023-03-14 08:45:03.744712 kng-0.4.0/kng/trade.py
--rw-r--r--   0        0        0      925 2023-03-14 11:08:44.175369 kng-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 kng-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-01-30 10:13:58.966160 kng-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1332 2023-03-06 02:47:55.579784 kng-0.6.1/README.md
+-rw-r--r--   0        0        0        0 2023-01-30 10:14:35.543763 kng-0.6.1/kng/__init__.py
+-rw-r--r--   0        0        0      533 2023-03-14 09:45:39.376053 kng-0.6.1/kng/dt.py
+-rw-r--r--   0        0        0      769 2023-03-14 10:43:33.274166 kng-0.6.1/kng/iter.py
+-rw-r--r--   0        0        0     1259 2023-03-14 14:32:45.331442 kng-0.6.1/kng/pd.py
+-rw-r--r--   0        0        0      571 2023-05-11 15:11:00.772789 kng-0.6.1/kng/pypi.py
+-rw-r--r--   0        0        0      389 2023-03-14 08:45:03.744712 kng-0.6.1/kng/trade.py
+-rw-r--r--   0        0        0      907 2023-05-11 15:21:14.454457 kng-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1763 1970-01-01 00:00:00.000000 kng-0.6.1/PKG-INFO
```

### Comparing `kng-0.4.0/LICENSE` & `kng-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kng-0.4.0/README.md` & `kng-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `kng-0.4.0/kng/dt.py` & `kng-0.6.1/kng/dt.py`

 * *Files identical despite different names*

### Comparing `kng-0.4.0/kng/iter.py` & `kng-0.6.1/kng/iter.py`

 * *Files identical despite different names*

### Comparing `kng-0.4.0/kng/misc.py` & `kng-0.6.1/kng/pypi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-"""misc utility functions"""
+"""pypi utility functions"""
+
+from requests import get
 
 
 def check_pypi_availability(pkg_name: str) -> bool:
     """check PyPi package name availability
 
     Args:
         pkg_name (str): package name to be checked
@@ -13,12 +15,10 @@
 
         >>> check_pypi_availability('ktemplate-bla-bla-bla')
         True
 
     Returns:
         bool: if package name avaialbe return True otherwise False
     """
-    from httpx import get
-
     url = f"https://pypi.org/pypi/{pkg_name}/json"
     response = get(url)
     return response.status_code != 200
```

### Comparing `kng-0.4.0/kng/pd.py` & `kng-0.6.1/kng/pd.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,18 +37,18 @@
     template = """
         <div style="float: left; padding: 10px;">
         <p style='font-family:"Courier New", Courier, monospace'>{0}</p>{1}
         </div>
     """
 
     def _repr_html_(self):
-        """html representation"""
+        """html representation, for notebook"""
         htmls = [
             self.template.format(title, df._repr_html_())
             for title, df in self.dfs.items()
         ]
         return "\n".join(htmls)
 
     def __repr__(self):
-        """string representation"""
+        """string representation, for console"""
         str_reps = [title + "\n" + repr(df) for title, df in self.dfs.items()]
         return "\n\n".join(str_reps)
```

### Comparing `kng-0.4.0/pyproject.toml` & `kng-0.6.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kng"
-version = "0.4.0"
+version = "0.6.1"
 description = "handy utility functions collection"
 authors = [ "Kelvin Ng <hoishing@gmail.com>",]
 readme = "README.md"
 repository = "https://github.com/hoishing/kng"
 homepage = "https://hoishing.github.io/kng"
 keywords = [ "utilities",]
 [[tool.poetry.packages]]
 include = "kng"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-httpx = "^0.23.3"
 
 [tool.poetry.scripts]
 pump = "pump:main"
 
 [tool.poetry.group.dev]
 optional = true
```

### Comparing `kng-0.4.0/PKG-INFO` & `kng-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: kng
-Version: 0.4.0
+Version: 0.6.1
 Summary: handy utility functions collection
 Home-page: https://hoishing.github.io/kng
 Keywords: utilities
 Author: Kelvin Ng
 Author-email: hoishing@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Project-URL: Repository, https://github.com/hoishing/kng
 Description-Content-Type: text/markdown
 
 # kng
 
 [![ci-badge]][ci-url] [![pypi-badge]][pypi-url] [![coverage-badge]][coverage-url] ![py-ver-badge] [![MIT-badge]][MIT-url] [![black-badge]][black-url]
```

