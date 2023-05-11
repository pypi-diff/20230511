# Comparing `tmp/gpt4-openai-api-0.1.0.tar.gz` & `tmp/gpt4-openai-api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gpt4-openai-api-0.1.0.tar", last modified: Sun May  7 22:40:36 2023, max compression
+gzip compressed data, was "dist\gpt4-openai-api-0.2.0.tar", last modified: Thu May 11 20:52:26 2023, max compression
```

## Comparing `gpt4-openai-api-0.1.0.tar` & `gpt4-openai-api-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 22:40:36.622969 gpt4-openai-api-0.1.0/
--rw-rw-rw-   0        0        0      800 2023-05-07 22:40:36.619969 gpt4-openai-api-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-07 22:40:36.550970 gpt4-openai-api-0.1.0/gpt4_openai/
--rw-rw-rw-   0        0        0     2545 2023-05-07 22:37:30.000000 gpt4-openai-api-0.1.0/gpt4_openai/__init__.py
--rw-rw-rw-   0        0        0    22919 2023-05-07 20:12:58.000000 gpt4-openai-api-0.1.0/gpt4_openai/driver.py
-drwxrwxrwx   0        0        0        0 2023-05-07 22:40:36.601974 gpt4-openai-api-0.1.0/gpt4_openai_api.egg-info/
--rw-rw-rw-   0        0        0      800 2023-05-07 22:40:36.000000 gpt4-openai-api-0.1.0/gpt4_openai_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-05-07 22:40:36.000000 gpt4-openai-api-0.1.0/gpt4_openai_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 22:40:36.000000 gpt4-openai-api-0.1.0/gpt4_openai_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-05-07 22:40:36.000000 gpt4-openai-api-0.1.0/gpt4_openai_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-07 22:40:36.000000 gpt4-openai-api-0.1.0/gpt4_openai_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 22:40:36.623971 gpt4-openai-api-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      978 2023-05-07 22:40:33.000000 gpt4-openai-api-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 22:40:36.612974 gpt4-openai-api-0.1.0/test/
--rw-rw-rw-   0        0        0     1291 2023-05-07 22:38:49.000000 gpt4-openai-api-0.1.0/test/test.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:26.288120 gpt4-openai-api-0.2.0/
+-rw-rw-rw-   0        0        0      800 2023-05-11 20:52:26.287123 gpt4-openai-api-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:26.250120 gpt4-openai-api-0.2.0/gpt4_openai/
+-rw-rw-rw-   0        0        0     2559 2023-05-11 20:46:34.000000 gpt4-openai-api-0.2.0/gpt4_openai/__init__.py
+-rw-rw-rw-   0        0        0    24235 2023-05-11 20:46:44.000000 gpt4-openai-api-0.2.0/gpt4_openai/driver.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:26.281118 gpt4-openai-api-0.2.0/gpt4_openai_api.egg-info/
+-rw-rw-rw-   0        0        0      800 2023-05-11 20:52:26.000000 gpt4-openai-api-0.2.0/gpt4_openai_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-05-11 20:52:26.000000 gpt4-openai-api-0.2.0/gpt4_openai_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 20:52:26.000000 gpt4-openai-api-0.2.0/gpt4_openai_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-11 20:52:26.000000 gpt4-openai-api-0.2.0/gpt4_openai_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-11 20:52:26.000000 gpt4-openai-api-0.2.0/gpt4_openai_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 20:52:26.289121 gpt4-openai-api-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      978 2023-05-11 20:51:20.000000 gpt4-openai-api-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:52:26.284120 gpt4-openai-api-0.2.0/test/
+-rw-rw-rw-   0        0        0      434 2023-05-11 20:47:25.000000 gpt4-openai-api-0.2.0/test/test.py
+-rw-rw-rw-   0        0        0      997 2023-05-07 23:29:24.000000 gpt4-openai-api-0.2.0/test/test_langchain.py
```

### Comparing `gpt4-openai-api-0.1.0/PKG-INFO` & `gpt4-openai-api-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: gpt4-openai-api
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python package for unofficial GPT-4 API access via chat.openai.com using Selenium browser
 Home-page: https://github.com/Erol444/gpt4-openai-api
 Author: Erol444
 Author-email: erol123444@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `gpt4-openai-api-0.1.0/gpt4_openai/__init__.py` & `gpt4-openai-api-0.2.0/gpt4_openai/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
         response = ""
         # OpenAI: 50 requests / hour for each account
         if self.call >= 45:
             raise ValueError("You have reached the maximum number of requests per hour ! Help me to Improve. Abusing this tool is at your own risk")
         else:
             sleep(2)
-            data = self.chatbot.send_message(prompt)
+            data = self.chatbot.send_message(prompt, model='gpt4')
             #print(data)
             response = data["message"]
             self.conversation = data["conversation_id"]
             FullResponse = data
             self.call += 1
 
         #add to history
```

### Comparing `gpt4-openai-api-0.1.0/gpt4_openai/driver.py` & `gpt4-openai-api-0.2.0/gpt4_openai/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 chatgpt_streaming = (By.CLASS_NAME, 'result-streaming')
 chatgpt_big_response = (By.XPATH, '//div[@class="flex-1 overflow-hidden"]//div[p]')
 chatgpt_small_response = (
     By.XPATH,
     '//div[starts-with(@class, "markdown prose w-full break-words")]',
 )
 chatgpt_alert = (By.XPATH, '//div[@role="alert"]')
+chatgpt_dialog = (By.XPATH, '//div[@role="dialog"]')
 chatgpt_intro = (By.ID, 'headlessui-portal-root')
 chatgpt_login_btn = (By.XPATH, '//button[text()="Log in"]')
 chatgpt_login_h1 = (By.XPATH, '//h1[text()="Welcome back"]')
 chatgpt_logged_h1 = (By.XPATH, '//h1[text()="ChatGPT"]')
 
 chatgpt_new_chat = (By.LINK_TEXT, 'New chat')
 chatgpt_clear_convo = (By.LINK_TEXT, 'Clear conversations')
@@ -76,14 +77,15 @@
         :param login_cookies_path: The path to the cookies file to use for authentication
         :param captcha_solver: The captcha solver to use (`pypasser`, `2captcha`)
         :param solver_apikey: The apikey of the captcha solver to use (if any)
         :param proxy: The proxy to use for the browser (`https://ip:port`)
         :param chrome_args: The arguments to pass to the browser
         :param moderation: Whether to enable message moderation
         :param verbose: Whether to enable verbose logging
+        :param headless: Whether to run the browser in headless mode
         '''
         self.__init_logger(verbose)
 
         self.__session_token = session_token
         self.__conversation_id = conversation_id
         self.__auth_type = auth_type
         self.__email = email
@@ -145,15 +147,15 @@
 
     def __init_logger(self, verbose: bool) -> None:
         '''
         Initialize the logger\n
         :param verbose: Whether to enable verbose logging
         '''
         self.logger = logging.getLogger('pyChatGPT')
-        self.logger.setLevel(logging.INFO)
+        self.logger.setLevel(logging.DEBUG)
         if verbose:
             formatter = logging.Formatter('[%(funcName)s] %(message)s')
             stream_handler = logging.StreamHandler()
             stream_handler.setFormatter(formatter)
             self.logger.addHandler(stream_handler)
 
     def __init_browser(self) -> None:
@@ -373,27 +375,47 @@
             self.__sleep(60)
 
     def __check_blocking_elements(self) -> None:
         '''
         Check for blocking elements and dismiss them
         '''
         self.logger.debug('Looking for blocking elements...')
+        
         try:
-            intro = WebDriverWait(self.driver, 3).until(
-                EC.presence_of_element_located(chatgpt_intro)
-            )
-            self.logger.debug('Dismissing intro...')
-            self.driver.execute_script('arguments[0].remove()', intro)
-        except SeleniumExceptions.TimeoutException:
+            # FInd a button to dismiss the dialog with class="btn relative btn-primary" inside the div[@role="dialog"]
+            btn_to_dismiss = WebDriverWait(self.driver, 5).until(
+                EC.presence_of_element_located((By.XPATH, '//div[@role="dialog"]//button[@class="btn relative btn-primary"]'))
+            )
+            if btn_to_dismiss:
+                self.logger.debug('Dismissing dialog...')
+                self.driver.execute_script('arguments[0].click()', btn_to_dismiss)
+        except:
+            pass
+        
+        try:
+            # for 3 times
+            i = 0
+            while i<=2:
+                self.__sleep(0.4)
+                if i !=2:
+                    #get the button with class="btn relative btn-neutral ml-auto"
+                    btn = WebDriverWait(self.driver, 5).until(
+                        EC.presence_of_element_located((By.XPATH, '//button[@class="btn relative btn-neutral ml-auto"]'))
+                    )
+                else:
+                    #get the button with class="btn relative btn-primary ml-auto"
+                    btn = WebDriverWait(self.driver, 5).until(
+                        EC.presence_of_element_located((By.XPATH, '//button[@class="btn relative btn-primary ml-auto"]'))
+                    )
+                if btn:
+                    self.logger.debug('Dismissing dialog...')
+                    self.driver.execute_script('arguments[0].click()', btn)
+                i+=1     
+        except:  
             pass
-
-        alerts = self.driver.find_elements(*chatgpt_alert)
-        if alerts:
-            self.logger.debug('Dismissing alert...')
-            self.driver.execute_script('arguments[0].remove()', alerts[0])
 
     def __stream_message(self):
         prev_content = ''
         while True:
             result_streaming = self.driver.find_elements(*chatgpt_streaming)
             responses = self.driver.find_elements(*chatgpt_big_response)
             if responses:
@@ -405,45 +427,47 @@
             content = response.text
             if content != prev_content:
                 yield content[len(prev_content) :]
                 prev_content = content
             if not result_streaming:
                 break
 
-    def send_message(self, message: str, stream: bool = False) -> dict:
+    def send_message(self, message: str, stream: bool = False, model: str = "default") -> dict:
         '''
         Send a message to ChatGPT\n
         :param message: Message to send
         :return: Dictionary with keys `message` and `conversation_id`
         '''
         self.logger.debug('Ensuring Cloudflare cookies...')
         self.__ensure_cf()
-        self.__check_blocking_elements()
+        #self.__check_blocking_elements()
 
         # Wait for page to load
         try:
             textbox = WebDriverWait(self.driver, 10).until(
                 EC.element_to_be_clickable(chatgpt_textbox)
             )
         except SeleniumExceptions.ElementClickInterceptedException():
             pass
 
         # If we have paid access, we should select GPT4 model
         try:
-            self.logger.debug('Trying to select model...')
-            WebDriverWait(self.driver, 3).until(
-                EC.presence_of_element_located(model_selector)
-            ).click()
-            self.logger.debug('Paid access detected, selecting GPT4 model...')
-            self.__sleep(1.0)
-            WebDriverWait(self.driver, 3).until(
-                EC.presence_of_element_located(gpt4_selector)
-            ).click()
-            self.logger.debug('GPT4 model selected')
+            if model == "gpt4":
+                self.logger.debug('Trying to select model...')
+                WebDriverWait(self.driver, 3).until(
+                    EC.presence_of_element_located(model_selector)
+                ).click()
+                self.logger.debug('Paid access detected, selecting GPT4 model...')
+                self.__sleep(1.0)
+                WebDriverWait(self.driver, 3).until(
+                    EC.presence_of_element_located(gpt4_selector)
+                ).click()
+                self.logger.debug('GPT4 model selected')
         except SeleniumExceptions.TimeoutException:
+            print(">>> WARNING <<<\n>> You don't have paid access to GPT4, using default model...")
             self.logger.debug('Paid access not detected, using default model...')
 
         self.logger.debug('Sending message...')
         try:
             textbox = WebDriverWait(self.driver, 3).until(
                 EC.element_to_be_clickable(chatgpt_textbox)
             )
@@ -485,27 +509,27 @@
                 self.logger.debug('Response is an error')
                 raise ValueError(response.text)
         response = self.driver.find_elements(*chatgpt_small_response)[-1]
 
         content = markdownify(response.get_attribute('innerHTML')).replace(
             'Copy code`', '`'
         )
+                
         pattern = re.compile(
             r'[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}'
         )
         matches = pattern.search(self.driver.current_url)
         if not matches:
             self.driver.refresh()
-            self.__sleep(1)
-            self.__check_blocking_elements()
-            self.__sleep(1)
+            self.__sleep(2)
+            #self.__check_blocking_elements()
             self.driver.execute_script("arguments[0].click();", WebDriverWait(self.driver, 10).until(
                 EC.element_to_be_clickable(chatgpt_chats_list_first_node)
             ))
-            self.__sleep(1)
+            self.__sleep(2)
             #print(self.driver.current_url)
             matches = pattern.search(self.driver.current_url)
 
 
         #get current url and print it
         #print(self.driver.current_url)
         #print(matches)
@@ -564,8 +588,8 @@
         Refresh the chat page
         '''
         if not self.driver.current_url.startswith(chatgpt_chat_url):
             return self.logger.debug('Current URL is not chat page, skipping refresh')
 
         self.driver.get(chatgpt_chat_url)
         self.__check_capacity(chatgpt_chat_url)
-        self.__check_blocking_elements()
+        self.__check_blocking_elements()
```

### Comparing `gpt4-openai-api-0.1.0/gpt4_openai_api.egg-info/PKG-INFO` & `gpt4-openai-api-0.2.0/gpt4_openai_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: gpt4-openai-api
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python package for unofficial GPT-4 API access via chat.openai.com using Selenium browser
 Home-page: https://github.com/Erol444/gpt4-openai-api
 Author: Erol444
 Author-email: erol123444@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `gpt4-openai-api-0.1.0/test/test.py` & `gpt4-openai-api-0.2.0/test/test_langchain.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,21 @@
 from dotenv import load_dotenv
 import os
 from gpt4_openai import GPT4OpenAI
+from langchain import LLMChain
+from langchain.prompts.chat import (ChatPromptTemplate, SystemMessagePromptTemplate, AIMessagePromptTemplate, HumanMessagePromptTemplate)
 
-print(GPT4OpenAI.__file__)
 load_dotenv()
 
-# Token is the __Secure-next-auth.session-token from chat.openai.com
-llm = GPT4OpenAI(token=os.environ["OPENAI_SESSION_TOKEN"], headless=False)
-response = llm('How ')
-print(response)
-
-# from langchain import PromptTemplate, LLMChain
-
-# from langchain.prompts.chat import (
-#     ChatPromptTemplate,
-#     SystemMessagePromptTemplate,
-#     AIMessagePromptTemplate,
-#     HumanMessagePromptTemplate,
-# )
+template="You are a helpful assistant that translates english to pirate."
+system_message_prompt = SystemMessagePromptTemplate.from_template(template)
+example_human = HumanMessagePromptTemplate.from_template("Hi")
+example_ai = AIMessagePromptTemplate.from_template("Argh me mateys")
+human_message_prompt = HumanMessagePromptTemplate.from_template("{text}")
 
-# from chatgpt_api import ChatGPT
-# llm = ChatGPT(token=token)
+chat_prompt = ChatPromptTemplate.from_messages([system_message_prompt, example_human, example_ai, human_message_prompt])
 
-# template="You are a helpful assistant that translates english to pirate."
-# system_message_prompt = SystemMessagePromptTemplate.from_template(template)
-# example_human = HumanMessagePromptTemplate.from_template("Hi")
-# example_ai = AIMessagePromptTemplate.from_template("Argh me mateys")
-# human_template="{text}"
-# human_message_prompt = HumanMessagePromptTemplate.from_template(human_template)
-
-# chat_prompt = ChatPromptTemplate.from_messages([system_message_prompt, example_human, example_ai, human_message_prompt])
-# chain = LLMChain(llm=llm, prompt=chat_prompt)
-# print('chain run:', chain.run("My plants are not very impressed with the humidity in my room"))
+# Token is the __Secure-next-auth.session-token from chat.openai.com
+llm = GPT4OpenAI(token=os.environ["OPENAI_SESSION_TOKEN"])
+chain = LLMChain(llm=llm, prompt=chat_prompt)
+print(chain.run("My name is John and I like to eat pizza."))
```

