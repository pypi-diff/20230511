# Comparing `tmp/mrfix-0.0.1.tar.gz` & `tmp/mrfix-1.0.0.tar.gz`

## Comparing `mrfix-0.0.1.tar` & `mrfix-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-0.0.1/LICENZE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-0.0.1/src/mrfix/__init__.py
--rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 mrfix-0.0.1/src/mrfix/mrfix.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 mrfix-0.0.1/.gitignore
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 mrfix-0.0.1/README.md
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 mrfix-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 mrfix-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-1.0.0/LICENZE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-1.0.0/src/mrfix/__init__.py
+-rw-r--r--   0        0        0    12696 2020-02-02 00:00:00.000000 mrfix-1.0.0/src/mrfix/mrfix.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 mrfix-1.0.0/.gitignore
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 mrfix-1.0.0/README.md
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mrfix-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10352 2020-02-02 00:00:00.000000 mrfix-1.0.0/PKG-INFO
```

### Comparing `mrfix-0.0.1/LICENZE` & `mrfix-1.0.0/LICENZE`

 * *Files identical despite different names*

### Comparing `mrfix-0.0.1/src/mrfix/mrfix.py` & `mrfix-1.0.0/src/mrfix/mrfix.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,27 @@
+import sys
 import time
 import requests
 from loguru import logger
-from selenium.common.exceptions import NoSuchElementException, WebDriverException
+from selenium.common.exceptions import NoSuchElementException
+from selenium.common.exceptions import WebDriverException
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver import ActionChains
 from selenium.webdriver.common.keys import Keys
+import datetime
 import pyperclip
+from selenium import webdriver
+from selenium.webdriver.support.wait import WebDriverWait
+from selenium.webdriver.support import expected_conditions as EC
+import selenium.webdriver.support.ui as ui
 
-class MrFix:
+
+
+class MrFix :
 
     def assertElementsIsPresentByXpatch(self, xpath_elements):
         try:
             elements = self.find_elements(By.XPATH, xpath_elements)
             return [True, len(elements)]
         except NoSuchElementException:
             return [False, 0]
@@ -26,237 +35,354 @@
 
     def assertElementIsPresentByXPath_Send(self, xpath_input, send_message):
         try:
             element = self.find_element(By.XPATH, xpath_input)
             element.clear()
             length = len(element.get_attribute('value'))
             element.send_keys(length * Keys.BACKSPACE)
-            time.sleep(2)
+            time.sleep(0.5)
             element.send_keys(send_message)
             return True
         except NoSuchElementException:
             return (False)
 
-    def check_exists_by_xpath(self, xpath):
+    def check_exists_xpath(self, xpath_element):
         try:
-            self.find_element(By.XPATH, xpath)
+            self.set_page_load_timeout(1)
+            self.implicitly_wait(1)
+            self.find_element(By.XPATH, xpath_element)
+            self.implicitly_wait(10)
+            self.set_page_load_timeout(10)
         except NoSuchElementException:
             return False
         return True
 
-    def select_and_click_element(self, xpath):
-        assert MrFix.assertElementIsPresentByXPath_Click(self, xpath), f'Элемента {xpath} на странице нет'
+    def click_element(self, xpath_element):
+        if MrFix.check_exists_xpath(self, xpath_element) == True:
+            self.find_element(By.XPATH, xpath_element).click()
+        else:
+            print(f'Element {xpath_element} not exists')
+            sys.exit()
+
+
+    def click_drop_down_text(self, xpath_element, element_text):
+        if MrFix.check_exists_xpath(self, xpath_element) == False:
+            print(f'Element {xpath_element} not exists')
+            sys.exit()
+        element = self.find_element(By.XPATH, xpath_element)
+        element.click()
+        all_options = element.find_elements_by_tag_name("option")
+        for option in all_options:
+            if option.get_attribute("text") == element_text:
+                option.click()
+                break
+
+    def send_input_text(self, xpath_input, input_text):
+        if MrFix.check_exists_xpath(self, xpath_input) == False:
+            print(f'Element {xpath_input} not exists')
+            sys.exit()
+        MrFix.assertElementIsPresentByXPath_Send(self, xpath_input, input_text)
 
-    def select_and_send_in_input(self, xpath_input, send_message) -> object:
-        assert MrFix.assertElementIsPresentByXPath_Send(self, xpath_input,
-                                                           send_message), f'Элемента {xpath_input} на странице нет'
 
-    def check_exists_elements_count(self, xpath_elements):
+    def return_elements_array(self, xpath_elements):
+        if MrFix.check_exists_xpath(self, xpath_elements) == False:
+            print(f'Element {xpath_elements} not exists')
+            sys.exit()
         elements_array = MrFix.assertElementsIsPresentByXpatch(self, xpath_elements)
-        assert elements_array[0], f'Элементов {xpath_elements} на странице нет'
         return elements_array
 
-    def scroll_down_and_click_element(self, xpath_down_link):
 
-        SCROLL_PAUSE_TIME = 0.5
+    def return_elements_array2(self, xpath_elements):
+        if MrFix.check_exists_xpath(self, xpath_elements) == False:
+            print(f'Element {xpath_elements} not exists')
+            sys.exit()
+        elements_array = self.find_elements(By.XPATH, xpath_elements)
+        return elements_array
+
+
+    def scroll_down_click_element(self, xpath_down_link):
+        scroll_pause_time = 0.5
         # Get scroll height
         last_height = self.execute_script("return document.body.scrollHeight")
         while True:
             # Scroll down to bottom
             self.execute_script("window.scrollTo(0, document.body.scrollHeight);")
 
             # Wait to load page
-            time.sleep(SCROLL_PAUSE_TIME)
+            time.sleep(scroll_pause_time)
 
             # Calculate new scroll height and compare with last scroll height
             new_height = self.execute_script("return document.body.scrollHeight")
-            if new_height == last_height:
+            if new_height == last_height or MrFix.check_exists_xpath(self, xpath_down_link):
                 break
             last_height = new_height
+        assert MrFix.assertElementIsPresentByXPath_Click(self, xpath_down_link), f'Element {xpath_down_link} not exists'
 
-        assert MrFix.assertElementIsPresentByXPath_Click(self,
-                                                            xpath_down_link), f'Элемент {xpath_down_link} внизу страницы не обнаружен'
-
-    def select_drop_down_element_text(self, xpath_drop_down_list, element_text):
 
-        element = self.find_element(By.XPATH, xpath_drop_down_list)
-        element.click()
-        all_options = element.find_elements_by_tag_name("option")
-        for option in all_options:
-            if option.get_attribute("text") == element_text:  # print("Value is: %s" % option.get_attribute("value"))
-                option.click()
-                break
-
-    def select_element_and_click_enter(self, xpath_element):
+    def click_element_key_enter(self, xpath_element):
+        if MrFix.check_exists_xpath(self, xpath_element) == False:
+            print(f'Element {xpath_element} not exists')
+            sys.exit()
         self.find_element(By.XPATH, xpath_element).send_keys(Keys.RETURN)
-        assert MrFix.assertElementIsPresentByXPath_Click(self, xpath_element), f'Элемента {xpath_element} на странице нет'
+
 
     def autorization_user(self, url, login, password):
         session = requests.Session()
         session.post(url, {
             'username': login,
             'password': password,
             'remember': 1,
         })
 
+
     def uploading_file(self, xpath_input_file, file_path):
+        if MrFix.check_exists_xpath(self, xpath_input_file) == False:
+            print(f'Element {xpath_input_file} not exists')
+            sys.exit()
         self.find_element(By.XPATH, xpath_input_file).send_keys(file_path)
-        assert MrFix.assertElementIsPresentByXPath_Click(self, xpath_input_file), f'Элемента {xpath_input_file} на странице нет'
-
-    def logging_file(log_file):
-        logger.remove()
-        logger.add(log_file, level='INFO',
-                   format="<lvl>[</lvl><c>{time:DD.MM.YYYY HH:mm:ss.SSS}</c><lvl>]</lvl> <lvl>{message}</lvl>",
-                   catch='True')
-
-    def get_elements_array(self, xpath_elements):
-        elements_array = self.find_elements(By.XPATH, xpath_elements)
-        assert MrFix.assertElementIsPresentByXPath_Click(self, xpath_elements), f'Элемента {xpath_elements} на странице нет'
-        return elements_array
 
 
     def switch_to_current_window(self):
         self.switch_to.active_element
         handles = self.window_handles
         for handle in handles:
             if self.current_window_handle != handle:
-                # Закрываем первое окно
+                # Close first window
                 self.close()
-                # переключаемся на второе окно', handle
+                # set second window active (handle)
                 self.switch_to.window(handle)
 
+
     def get_elements_attribute(self, xpath_element, attribute):
+        if MrFix.check_exists_xpath(self, xpath_element) == False:
+            print(f'Element {xpath_element} not exists')
+            sys.exit()
         element = self.find_element(By.XPATH, xpath_element)
-        assert MrFix.assertElementIsPresentByXPath_Click(self, xpath_element), f'Элемента {xpath_element} на странице нет'
         return element.get_attribute(attribute)
 
-    def get_text_of_element(self, xpath_element):
+
+    def get_elements_text(self, xpath_element):
+        if MrFix.check_exists_xpath(self, xpath_element) == False:
+            print(f'Element {xpath_element} not exists')
+            sys.exit()
         element = self.find_element(By.XPATH, xpath_element)
-        assert MrFix.assertElementIsPresentByXPath_Click(self, xpath_element), f'Элемента {xpath_element} на странице нет'
         return element.text
 
-    def clear_input_element(self, xpath_element):
-        element = self.find_element(By.XPATH, xpath_element)
+
+    def select_drop_down_value(self, xpath_drop_down, drop_down_value):
+        if MrFix.check_exists_xpath(self, xpath_drop_down) == False:
+            print(f'Element {xpath_drop_down} not exists')
+            sys.exit()
+        select = Select(self.find_element(By.XPATH, xpath_drop_down))
+        # select by value
+        select.select_by_value(drop_down_value)
+
+
+    def select_drop_down_text(self, xpath_drop_down, drop_down_text):
+        if MrFix.check_exists_xpath(self, xpath_drop_down) == False:
+            print(f'Element {xpath_drop_down} not exists')
+            sys.exit()
+        select = Select(self.find_element(By.XPATH, xpath_drop_down))
+        # select by visible text
+        select.select_by_visible_text(drop_down_text)
+
+
+    def clear_input_element(self, xpath_input_element):
+        if MrFix.check_exists_xpath(self, xpath_input_element) == False:
+            print(f'Element {xpath_input_element} not exists')
+            sys.exit()
+        element = self.find_element(By.XPATH, xpath_input_element)
+        element.send_keys(Keys.CONTROL, "a")
+        element.send_keys(Keys.DELETE)
         element.clear()
-        length = len(element.get_attribute('value'))
-        element.send_keys(length * Keys.BACKSPACE)
 
-    def press_down_arrow_key(self, n):
+
+    def pressing_down_arrow_key(self, n):
         action = ActionChains(self)
         for _ in range(n):
             action.send_keys(Keys.ARROW_DOWN)
             time.sleep(.1)
         action.perform()
 
-    def press_up_arrow_key_up(self, n):
+
+    def pressing_up_arrow_key(self, n):
         action = ActionChains(self)
-        for i in range(n):
+        for _ in range(n):
             action.send_keys(Keys.ARROW_UP)
-            time.sleep(0.1)
+            time.sleep(.1)
+        action.perform()
+
+
+    def pressing_left_arrow_key(self, n):
+        action = ActionChains(self)
+        for _ in range(n):
+            action.send_keys(Keys.ARROW_LEFT)
+            time.sleep(.1)
+        action.perform()
+
 
-    def press_enter_key(self, n):
+    def pressing_right_arrow_key(self, n):
+        action = ActionChains(self)
+        for _ in range(n):
+            action.send_keys(Keys.ARROW_RIGHT)
+            time.sleep(.1)
+        action.perform()
+
+
+    def pressing_enter_key(self, n):
         action = ActionChains(self)
         for _ in range(n):
             action.send_keys(Keys.RETURN)
             time.sleep(.1)
         action.perform()
 
-    def press_tab_key(self, n):
+
+    def pressing_tab_key(self, n):
         action = ActionChains(self)
         for _ in range(n):
             action.send_keys(Keys.TAB)
             time.sleep(.1)
         action.perform()
 
-    def press_backspace_key(self, n):
+
+    def pressing_backspace_key(self, n):
         action = ActionChains(self)
         for _ in range(n):
             action.send_keys(Keys.BACKSPACE)
             time.sleep(.1)
         action.perform()
 
-    def press_space_key(self, n):
+
+    def pressing_delete_key(self, n):
         action = ActionChains(self)
         for _ in range(n):
-            action.send_keys(Keys.SPACE)
+            action.send_keys(Keys.DELETE)
             time.sleep(.1)
         action.perform()
 
-    def press_char(self, char, n):
+
+    def pressing_char_key(self, char, n):
         action = ActionChains(self)
         for _ in range(n):
             action.send_keys(char)
             time.sleep(.1)
         action.perform()
 
-    def find_and_click_text_link(self, text):
-        try:
-            self.find_element_by_partial_link_text(text).click()
-            return True
-        except NoSuchElementException:
-            return False
-
-    def find_and_return_href_on_page(self, link):
-        link_exists = False
-        url = ''
-        elems = self.find_element(By.XPATH, "//a[@href]")
-        for elem in elems:
-            s = elem.get_attribute("href")
-            if link in s:
-                link_exists = True
-                url = s
-        m = []
-        m.append(link_exists)
-        m.append(url)
-        return m
 
     def check_url(url):
         try:
-            url_exists = True
             response = requests.get(url)
         except ValueError:
-            url_exists = False
-        return url_exists
+            return False
+        return True
 
-    def set_attribute_value(self, xpath, value):
-        self.execute_script("arguments[0].setAttribute('value',arguments[1])",xpath, value)
-        assert MrFix.assertElementIsPresentByXPath_Click(self, xpath), f'Элемента {xpath} на странице нет'
 
     def open_url_in_new_tab(self, url):
         # open in new tab
         self.execute_script("window.open('%s', '_blank')" % url)
         # Switch to new tab
         self.switch_to.window(self.window_handles[-1])
 
-    def check_clickable_element_and_click(self, xpath_element):
+
+    def check_clickable_element(self, xpath_element):
         try:
+            if MrFix.check_exists_xpath(self, xpath_element) == False:
+                print(f'Element {xpath_element} not exists')
+                sys.exit()
             element = self.find_element(By.XPATH, xpath_element)
             element.click()
             return True
         except WebDriverException:
+            print("Element is not clickable")
             return False
 
-    def make_element_visible_and_click(self, xpath_element):
-        while not MrFix.check_clickable_element_and_click(self, xpath_element):
-            MrFix.press_down_arrow_key(self, 1)
-
-    def make_element_visible_and_send(self, xpath_element, send_text):
-        while not MrFix.check_clickable_element_and_click(self, xpath_element):
-            MrFix.press_down_arrow_key(self, 1)
-        MrFix.select_and_send_in_input(self, xpath_element, send_text)
-
-    def get_clipboard(self):
-        return str(pyperclip.paste())
 
     def check_visible_element(self, xpath_element):
         try:
-            element = self.find_element(By.XPATH, xpath_element)
+            element = self.find_element_by_xpath(xpath_element)
             return element.is_visible()
         except NoSuchElementException:
             return False
 
     def check_displayed_element(self, xpath_element):
         try:
-            element = self.find_element(By.XPATH, xpath_element)
+            element = self.find_element_by_xpath(xpath_element)
             return element.is_displayed()
         except NoSuchElementException:
-            return False
+            return False
+
+    def get_clipboard_text(self):
+        return str(pyperclip.paste())
+
+
+    def convert_string_to_float(string_value):
+        val = string_value.replace(',', '.')
+        if val != '':
+            val = val.replace(' ', '', 100)
+            val = float(val)
+            return val
+        else:
+            return 0
+
+
+    def find_text_on_page(self, text):
+        try:
+            self.find_element_by_partial_link_text(text).click()
+            return True
+        except NoSuchElementException:
+            return False
+
+
+    def make_element_displayed_and_click(self, xpath_element):
+        while not MrFix.check_displayed_element(self, xpath_element):
+            MrFix.pressing_down_arrow_key(self, 1)
+        MrFix.click_element(self, xpath_element)
+
+
+    def make_element_displayed_and_send(self, xpath_element, send_text):
+        while not MrFix.check_displayed_element(self, xpath_element):
+            MrFix.pressing_down_arrow_key(self, 1)
+        MrFix.send_input_text(self, xpath_element, send_text)
+
+
+    def find_href_on_page(self, link):
+        link_availability = False
+        if MrFix.check_exists_xpath(self, "//a[@href]") == True:
+            elems = self.find_element(By.XPATH, "//a[@href]")
+        for elem in elems:
+            s = elem.get_attribute("href")
+            if link in s:
+                link_availability = True
+        return link_availability
+
+
+    def waiting_process_complete(self, xpath_proccess, time_in_second):
+        for i in range(time_in_second * 2):
+            if MrFix.check_displayed_element(self, xpath_proccess):
+                time.sleep(0.5)
+            else:
+                time.sleep(0.5)
+                break
+
+
+    def waiting_appearance_element (self, xpath_element, time_in_second):
+        for i in range(time_in_second * 2):
+            if not MrFix.check_displayed_element(self, xpath_element):
+                time.sleep(0.5)
+            else:
+                time.sleep(0.5)
+                break
+
+
+    def check_class_in_element(self, xpath_element, text_in_class):
+        element = self.find_element(By.XPATH, xpath_element)
+        if text_in_class in str(element.get_attribute("class")):
+            return True
+        else:
+            return False
+
+
+
+
+
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mrfix-0.0.1/.gitignore` & `mrfix-1.0.0/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -136,17 +136,21 @@
 
 # utilities
 utilities/config_template.ini
 
 testCases/download/
 testCases/allure/
 
+
+
+
 __pycache__/
 .pytest_cache/
 /home/gm/PycharmProjects/VEA/TESTS/Tests/__pycache__/
 /home/gm/PycharmProjects/VEA/TESTS/Tests/.pytest_cache
 .idea/
 /home/gm/PycharmProjects/VEA/TESTS/utilities/__pycache__
 /home/gm/PycharmProjects/VEA/TESTS/TestRail/__pycache__
 logs/
 /home/gm/PycharmProjects/VEA/TESTS/MyData/__pycache__
 
+
```

### Comparing `mrfix-0.0.1/pyproject.toml` & `mrfix-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system] 
 requires = ["hatchling"] 
 build-backend = "hatchling.build"
 
 [project] 
 name = "mrfix"
-version = "0.0.1" 
+version = "1.0.0"
 authors = [   
   { name="Valerii Zhuravlev", email="valerzhurav2011@gmail.com" },
 ] 
-description = "A small decorator-package for UI-autotesting with Python + Selenium" 
+description = "A package with a set of decorator-methods for automatic testing of the user interface using Python + Selenium"
 readme = "README.md" 
 requires-python = ">=3.9"
 classifiers = [     
   "Programming Language :: Python :: 3",     
   "License :: OSI Approved :: MIT License",     
   "Operating System :: OS Independent", 
 ]
```

