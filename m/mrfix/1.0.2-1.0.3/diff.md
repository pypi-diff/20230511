# Comparing `tmp/mrfix-1.0.2.tar.gz` & `tmp/mrfix-1.0.3.tar.gz`

## Comparing `mrfix-1.0.2.tar` & `mrfix-1.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-1.0.2/LICENZE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-1.0.2/src/mrfix/__init__.py
--rw-r--r--   0        0        0    12750 2020-02-02 00:00:00.000000 mrfix-1.0.2/src/mrfix/mrfix.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 mrfix-1.0.2/.gitignore
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 mrfix-1.0.2/README.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mrfix-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    10352 2020-02-02 00:00:00.000000 mrfix-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-1.0.3/LICENZE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-1.0.3/src/mrfix/__init__.py
+-rw-r--r--   0        0        0    13283 2020-02-02 00:00:00.000000 mrfix-1.0.3/src/mrfix/mrfix.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 mrfix-1.0.3/.gitignore
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 mrfix-1.0.3/README.md
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mrfix-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    10352 2020-02-02 00:00:00.000000 mrfix-1.0.3/PKG-INFO
```

### Comparing `mrfix-1.0.2/LICENZE` & `mrfix-1.0.3/LICENZE`

 * *Files identical despite different names*

### Comparing `mrfix-1.0.2/src/mrfix/mrfix.py` & `mrfix-1.0.3/src/mrfix/mrfix.py`

 * *Files 5% similar despite different names*

```diff
@@ -328,26 +328,38 @@
         try:
             self.find_element_by_partial_link_text(text).click()
             return True
         except NoSuchElementException:
             return False
 
 
-    def make_element_displayed_and_click(self, xpath_element):
+    def for_down_make_element_displayed_and_click(self, xpath_element):
         while not MrFixUI.check_displayed_element(self, xpath_element):
             MrFixUI.pressing_down_arrow_key(self, 1)
         MrFixUI.click_element(self, xpath_element)
 
 
-    def make_element_displayed_and_send(self, xpath_element, send_text):
+    def for_up_make_element_displayed_and_click(self, xpath_element):
+        while not MrFixUI.check_displayed_element(self, xpath_element):
+            MrFixUI.pressing_up_arrow_key(self, 1)
+        MrFixUI.click_element(self, xpath_element)
+
+
+    def for_down_make_element_displayed_and_send(self, xpath_element, send_text):
         while not MrFixUI.check_displayed_element(self, xpath_element):
             MrFixUI.pressing_down_arrow_key(self, 1)
         MrFixUI.send_input_text(self, xpath_element, send_text)
 
 
+    def for_up_make_element_displayed_and_send(self, xpath_element, send_text):
+        while not MrFixUI.check_displayed_element(self, xpath_element):
+            MrFixUI.pressing_up_arrow_key(self, 1)
+        MrFixUI.send_input_text(self, xpath_element, send_text)
+
+
     def find_href_on_page(self, link):
         link_availability = False
         if MrFixUI.check_exists_xpath(self, "//a[@href]") == True:
             elems = self.find_element(By.XPATH, "//a[@href]")
         for elem in elems:
             s = elem.get_attribute("href")
             if link in s:
```

### Comparing `mrfix-1.0.2/.gitignore` & `mrfix-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mrfix-1.0.2/README.md` & `mrfix-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mrfix-1.0.2/pyproject.toml` & `mrfix-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system] 
 requires = ["hatchling"] 
 build-backend = "hatchling.build"
 
 [project] 
 name = "mrfix"
-version = "1.0.2"
+version = "1.0.3"
 authors = [   
   { name="Valerii Zhuravlev", email="valerzhurav2011@gmail.com" },
 ] 
 description = "A package with a set of decorator-methods for automatic testing of the user interface using Python + Selenium"
 readme = "README.md" 
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `mrfix-1.0.2/PKG-INFO` & `mrfix-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrfix
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package with a set of decorator-methods for automatic testing of the user interface using Python + Selenium
 Project-URL: Homepage, https://github.com/MrFix-Autotesting-Framework
 Author-email: Valerii Zhuravlev <valerzhurav2011@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

