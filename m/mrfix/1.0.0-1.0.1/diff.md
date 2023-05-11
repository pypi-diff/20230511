# Comparing `tmp/mrfix-1.0.0.tar.gz` & `tmp/mrfix-1.0.1.tar.gz`

## Comparing `mrfix-1.0.0.tar` & `mrfix-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-1.0.0/LICENZE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-1.0.0/src/mrfix/__init__.py
--rw-r--r--   0        0        0    12696 2020-02-02 00:00:00.000000 mrfix-1.0.0/src/mrfix/mrfix.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 mrfix-1.0.0/.gitignore
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 mrfix-1.0.0/README.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mrfix-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    10352 2020-02-02 00:00:00.000000 mrfix-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-1.0.1/LICENZE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-1.0.1/src/mrfix/__init__.py
+-rw-r--r--   0        0        0    12750 2020-02-02 00:00:00.000000 mrfix-1.0.1/src/mrfix/mrfix.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 mrfix-1.0.1/.gitignore
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 mrfix-1.0.1/README.md
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mrfix-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    10352 2020-02-02 00:00:00.000000 mrfix-1.0.1/PKG-INFO
```

### Comparing `mrfix-1.0.0/LICENZE` & `mrfix-1.0.1/LICENZE`

 * *Files identical despite different names*

### Comparing `mrfix-1.0.0/src/mrfix/mrfix.py` & `mrfix-1.0.1/src/mrfix/mrfix.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from selenium import webdriver
 from selenium.webdriver.support.wait import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 import selenium.webdriver.support.ui as ui
 
 
 
-class MrFix :
+class MrFixUI :
 
     def assertElementsIsPresentByXpatch(self, xpath_elements):
         try:
             elements = self.find_elements(By.XPATH, xpath_elements)
             return [True, len(elements)]
         except NoSuchElementException:
             return [False, 0]
@@ -53,50 +53,50 @@
             self.implicitly_wait(10)
             self.set_page_load_timeout(10)
         except NoSuchElementException:
             return False
         return True
 
     def click_element(self, xpath_element):
-        if MrFix.check_exists_xpath(self, xpath_element) == True:
+        if MrFixUI.check_exists_xpath(self, xpath_element) == True:
             self.find_element(By.XPATH, xpath_element).click()
         else:
             print(f'Element {xpath_element} not exists')
             sys.exit()
 
 
     def click_drop_down_text(self, xpath_element, element_text):
-        if MrFix.check_exists_xpath(self, xpath_element) == False:
+        if MrFixUI.check_exists_xpath(self, xpath_element) == False:
             print(f'Element {xpath_element} not exists')
             sys.exit()
         element = self.find_element(By.XPATH, xpath_element)
         element.click()
         all_options = element.find_elements_by_tag_name("option")
         for option in all_options:
             if option.get_attribute("text") == element_text:
                 option.click()
                 break
 
     def send_input_text(self, xpath_input, input_text):
-        if MrFix.check_exists_xpath(self, xpath_input) == False:
+        if MrFixUI.check_exists_xpath(self, xpath_input) == False:
             print(f'Element {xpath_input} not exists')
             sys.exit()
-        MrFix.assertElementIsPresentByXPath_Send(self, xpath_input, input_text)
+        MrFixUI.assertElementIsPresentByXPath_Send(self, xpath_input, input_text)
 
 
     def return_elements_array(self, xpath_elements):
-        if MrFix.check_exists_xpath(self, xpath_elements) == False:
+        if MrFixUI.check_exists_xpath(self, xpath_elements) == False:
             print(f'Element {xpath_elements} not exists')
             sys.exit()
-        elements_array = MrFix.assertElementsIsPresentByXpatch(self, xpath_elements)
+        elements_array = MrFixUI.assertElementsIsPresentByXpatch(self, xpath_elements)
         return elements_array
 
 
     def return_elements_array2(self, xpath_elements):
-        if MrFix.check_exists_xpath(self, xpath_elements) == False:
+        if MrFixUI.check_exists_xpath(self, xpath_elements) == False:
             print(f'Element {xpath_elements} not exists')
             sys.exit()
         elements_array = self.find_elements(By.XPATH, xpath_elements)
         return elements_array
 
 
     def scroll_down_click_element(self, xpath_down_link):
@@ -108,22 +108,22 @@
             self.execute_script("window.scrollTo(0, document.body.scrollHeight);")
 
             # Wait to load page
             time.sleep(scroll_pause_time)
 
             # Calculate new scroll height and compare with last scroll height
             new_height = self.execute_script("return document.body.scrollHeight")
-            if new_height == last_height or MrFix.check_exists_xpath(self, xpath_down_link):
+            if new_height == last_height or MrFixUI.check_exists_xpath(self, xpath_down_link):
                 break
             last_height = new_height
-        assert MrFix.assertElementIsPresentByXPath_Click(self, xpath_down_link), f'Element {xpath_down_link} not exists'
+        assert MrFixUI.assertElementIsPresentByXPath_Click(self, xpath_down_link), f'Element {xpath_down_link} not exists'
 
 
     def click_element_key_enter(self, xpath_element):
-        if MrFix.check_exists_xpath(self, xpath_element) == False:
+        if MrFixUI.check_exists_xpath(self, xpath_element) == False:
             print(f'Element {xpath_element} not exists')
             sys.exit()
         self.find_element(By.XPATH, xpath_element).send_keys(Keys.RETURN)
 
 
     def autorization_user(self, url, login, password):
         session = requests.Session()
@@ -131,15 +131,15 @@
             'username': login,
             'password': password,
             'remember': 1,
         })
 
 
     def uploading_file(self, xpath_input_file, file_path):
-        if MrFix.check_exists_xpath(self, xpath_input_file) == False:
+        if MrFixUI.check_exists_xpath(self, xpath_input_file) == False:
             print(f'Element {xpath_input_file} not exists')
             sys.exit()
         self.find_element(By.XPATH, xpath_input_file).send_keys(file_path)
 
 
     def switch_to_current_window(self):
         self.switch_to.active_element
@@ -149,49 +149,49 @@
                 # Close first window
                 self.close()
                 # set second window active (handle)
                 self.switch_to.window(handle)
 
 
     def get_elements_attribute(self, xpath_element, attribute):
-        if MrFix.check_exists_xpath(self, xpath_element) == False:
+        if MrFixUI.check_exists_xpath(self, xpath_element) == False:
             print(f'Element {xpath_element} not exists')
             sys.exit()
         element = self.find_element(By.XPATH, xpath_element)
         return element.get_attribute(attribute)
 
 
     def get_elements_text(self, xpath_element):
-        if MrFix.check_exists_xpath(self, xpath_element) == False:
+        if MrFixUI.check_exists_xpath(self, xpath_element) == False:
             print(f'Element {xpath_element} not exists')
             sys.exit()
         element = self.find_element(By.XPATH, xpath_element)
         return element.text
 
 
     def select_drop_down_value(self, xpath_drop_down, drop_down_value):
-        if MrFix.check_exists_xpath(self, xpath_drop_down) == False:
+        if MrFixUI.check_exists_xpath(self, xpath_drop_down) == False:
             print(f'Element {xpath_drop_down} not exists')
             sys.exit()
         select = Select(self.find_element(By.XPATH, xpath_drop_down))
         # select by value
         select.select_by_value(drop_down_value)
 
 
     def select_drop_down_text(self, xpath_drop_down, drop_down_text):
-        if MrFix.check_exists_xpath(self, xpath_drop_down) == False:
+        if MrFixUI.check_exists_xpath(self, xpath_drop_down) == False:
             print(f'Element {xpath_drop_down} not exists')
             sys.exit()
         select = Select(self.find_element(By.XPATH, xpath_drop_down))
         # select by visible text
         select.select_by_visible_text(drop_down_text)
 
 
     def clear_input_element(self, xpath_input_element):
-        if MrFix.check_exists_xpath(self, xpath_input_element) == False:
+        if MrFixUI.check_exists_xpath(self, xpath_input_element) == False:
             print(f'Element {xpath_input_element} not exists')
             sys.exit()
         element = self.find_element(By.XPATH, xpath_input_element)
         element.send_keys(Keys.CONTROL, "a")
         element.send_keys(Keys.DELETE)
         element.clear()
 
@@ -281,15 +281,15 @@
         self.execute_script("window.open('%s', '_blank')" % url)
         # Switch to new tab
         self.switch_to.window(self.window_handles[-1])
 
 
     def check_clickable_element(self, xpath_element):
         try:
-            if MrFix.check_exists_xpath(self, xpath_element) == False:
+            if MrFixUI.check_exists_xpath(self, xpath_element) == False:
                 print(f'Element {xpath_element} not exists')
                 sys.exit()
             element = self.find_element(By.XPATH, xpath_element)
             element.click()
             return True
         except WebDriverException:
             print("Element is not clickable")
@@ -329,48 +329,48 @@
             self.find_element_by_partial_link_text(text).click()
             return True
         except NoSuchElementException:
             return False
 
 
     def make_element_displayed_and_click(self, xpath_element):
-        while not MrFix.check_displayed_element(self, xpath_element):
-            MrFix.pressing_down_arrow_key(self, 1)
-        MrFix.click_element(self, xpath_element)
+        while not MrFixUI.check_displayed_element(self, xpath_element):
+            MrFixUI.pressing_down_arrow_key(self, 1)
+        MrFixUI.click_element(self, xpath_element)
 
 
     def make_element_displayed_and_send(self, xpath_element, send_text):
-        while not MrFix.check_displayed_element(self, xpath_element):
-            MrFix.pressing_down_arrow_key(self, 1)
-        MrFix.send_input_text(self, xpath_element, send_text)
+        while not MrFixUI.check_displayed_element(self, xpath_element):
+            MrFixUI.pressing_down_arrow_key(self, 1)
+        MrFixUI.send_input_text(self, xpath_element, send_text)
 
 
     def find_href_on_page(self, link):
         link_availability = False
-        if MrFix.check_exists_xpath(self, "//a[@href]") == True:
+        if MrFixUI.check_exists_xpath(self, "//a[@href]") == True:
             elems = self.find_element(By.XPATH, "//a[@href]")
         for elem in elems:
             s = elem.get_attribute("href")
             if link in s:
                 link_availability = True
         return link_availability
 
 
     def waiting_process_complete(self, xpath_proccess, time_in_second):
         for i in range(time_in_second * 2):
-            if MrFix.check_displayed_element(self, xpath_proccess):
+            if MrFixUI.check_displayed_element(self, xpath_proccess):
                 time.sleep(0.5)
             else:
                 time.sleep(0.5)
                 break
 
 
     def waiting_appearance_element (self, xpath_element, time_in_second):
         for i in range(time_in_second * 2):
-            if not MrFix.check_displayed_element(self, xpath_element):
+            if not MrFixUI.check_displayed_element(self, xpath_element):
                 time.sleep(0.5)
             else:
                 time.sleep(0.5)
                 break
 
 
     def check_class_in_element(self, xpath_element, text_in_class):
```

### Comparing `mrfix-1.0.0/.gitignore` & `mrfix-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mrfix-1.0.0/README.md` & `mrfix-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mrfix-1.0.0/pyproject.toml` & `mrfix-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system] 
 requires = ["hatchling"] 
 build-backend = "hatchling.build"
 
 [project] 
 name = "mrfix"
-version = "1.0.0"
+version = "1.0.1"
 authors = [   
   { name="Valerii Zhuravlev", email="valerzhurav2011@gmail.com" },
 ] 
 description = "A package with a set of decorator-methods for automatic testing of the user interface using Python + Selenium"
 readme = "README.md" 
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `mrfix-1.0.0/PKG-INFO` & `mrfix-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrfix
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package with a set of decorator-methods for automatic testing of the user interface using Python + Selenium
 Project-URL: Homepage, https://github.com/MrFix-Autotesting-Framework
 Author-email: Valerii Zhuravlev <valerzhurav2011@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

