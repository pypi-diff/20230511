# Comparing `tmp/autoxx-0.0.11.tar.gz` & `tmp/autoxx-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.11.tar", max compression
+gzip compressed data, was "autoxx-0.0.12.tar", max compression
```

## Comparing `autoxx-0.0.11.tar` & `autoxx-0.0.12.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.11/README.md
--rw-r--r--   0        0        0      310 2023-05-06 05:23:14.108735 autoxx-0.0.11/autoxx/agent/base.py
--rw-r--r--   0        0        0      970 2023-05-08 02:54:46.023981 autoxx-0.0.11/autoxx/agent/researcher.py
--rw-r--r--   0        0        0     4126 2023-05-08 07:15:16.426595 autoxx-0.0.11/autoxx/agi.py
--rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.11/autoxx/js/overlay.js
--rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.11/autoxx/requirements.txt
--rw-r--r--   0        0        0     5307 2023-05-08 08:04:26.191393 autoxx-0.0.11/autoxx/search/simple_search.py
--rw-r--r--   0        0        0     4995 2023-05-07 02:59:38.452753 autoxx-0.0.11/autoxx/task_manager.py
--rw-r--r--   0        0        0      633 2023-05-08 08:07:15.998759 autoxx-0.0.11/pyproject.toml
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 autoxx-0.0.11/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.12/README.md
+-rw-r--r--   0        0        0      310 2023-05-06 05:23:14.108735 autoxx-0.0.12/autoxx/agent/base.py
+-rw-r--r--   0        0        0     1064 2023-05-08 14:09:26.013131 autoxx-0.0.12/autoxx/agent/researcher.py
+-rw-r--r--   0        0        0     4239 2023-05-09 11:57:08.681233 autoxx-0.0.12/autoxx/agi.py
+-rw-r--r--   0        0        0    14378 2023-05-11 01:33:36.997520 autoxx-0.0.12/autoxx/babyagi.py
+-rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.12/autoxx/js/overlay.js
+-rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.12/autoxx/requirements.txt
+-rw-r--r--   0        0        0     5697 2023-05-11 01:34:24.667007 autoxx-0.0.12/autoxx/search/simple_search.py
+-rw-r--r--   0        0        0     4924 2023-05-08 14:12:25.878274 autoxx-0.0.12/autoxx/task_manager.py
+-rw-r--r--   0        0        0      633 2023-05-11 01:35:46.862485 autoxx-0.0.12/pyproject.toml
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 autoxx-0.0.12/PKG-INFO
```

### Comparing `autoxx-0.0.11/autoxx/agent/researcher.py` & `autoxx-0.0.12/autoxx/agent/researcher.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,22 +8,27 @@
 
 class ResearchAgent(BaseAgent):  
   
     def execute(self, objective:str, task: str) -> str:  
         return simple_search(task)
   
     def post_process(self, objective:str, task_results:List[Dict]) -> str:  
-        task_context = [f"Task({task['task_description']}): {task['data']}" for task in task_results]
+        task_context = [f"Task({task['task']}): {task['result']}" for task in task_results]
         nl = '\n'
         prompt = (
-            "You are an task processing AI."
             f"Given the context {nl.join(task_context) } and objective: {objective}. "
             "Create a research report. "
         )
-        messages = [{
-            "role": "user",
-            "content": prompt,
-        }]
+        messages = [
+            {
+                "role": "system",
+                "content": "You are a research AI."
+            },
+            {
+                "role": "user",
+                "content": prompt,
+            }
+        ]
         return create_chat_completion(
             model=CFG.fast_llm_model,
             messages=messages,
         )
```

### Comparing `autoxx-0.0.11/autoxx/agi.py` & `autoxx-0.0.12/autoxx/agi.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,97 +3,105 @@
 from typing import Dict, List, Dict, Optional
 
 from autogpt.llm_utils import create_chat_completion
 from autogpt.config import Config
 
 response_format = """[
     {
-        "task_id": 1,
-        "task_description": "task description"
+        "id": 1,
+        "task": "task description",
+        "tool": "tool used to complete task"
     },
     {
-        "task_id": 2,
-        "task_description": "task description"
+        "id": 2,
+        "task": "task description",
+        "tool": "tool used to complete task"
     }
 ]"""
 
-def create_message(prompt: str) -> Dict[str, str]:
+def create_message(prompt: str) -> List[Dict]:
     """Create a message for the chat completion
 
     Args:
         chunk (str): The chunk of text to summarize
         question (str): The question to answer
 
     Returns:
         Dict[str, str]: The message to send to the chat completion
     """
-    return {
-        "role": "user",
-        "content": prompt,
-    }
+    return [
+        {
+            "role": "system",
+            "content": "You are a task manager AI."
+        },
+        {
+            "role": "user",
+            "content": prompt
+        }
+    ]
 
 def task_creation_agent(objective: str, task: Dict, task_list: List[str], allowed_new_task: Optional[int] = 1):
     prompt = (
-        f"You are an task creation AI that uses the result of an execution agent to create new tasks with the following objective: {objective}.\n"
-        f"The last completed task has the result: {task['data']}. "
-        f"This result was based on this task description: {task['task_description']}. "
+        f"You are a task management AI that uses the result of the last to create new tasks with the following objective: {objective}.\n"
+        f"The last completed task has the result: {task['result']}. "
+        f"This result was based on this task description: {task['task']}. "
         f"These are incomplete tasks: {', '.join(task_list)}. "
         f"Based on the result, create new tasks to be completed by the AI system that do not overlap with incomplete tasks. Up to {allowed_new_task} new tasks can be created.\n"
         "You should only respond in JSON format as described below \n"
         f"Response Format: \n{response_format} \nEnsure the response can be parsed by Python json.loads"
     )
 
-    messages = [create_message(prompt)]
+    messages = create_message(prompt)
     response = create_chat_completion(
         model=Config().fast_llm_model,
         messages=messages,
     )
 
     new_tasks = json.loads(response)
-    return [{"task_description": task["task_description"]} for task in new_tasks]
+    return [{"task": task["task"]} for task in new_tasks]
 
 def prioritization_agent(this_task_id:int, objective:str, task_list:deque) -> deque:
-    task_descriptions = [t["task_description"] for t in task_list]
+    task_descriptions = [t["task"] for t in task_list]
     next_task_id = int(this_task_id)+1
     prompt = (
-        f"You are an task prioritization AI tasked with cleaning the formatting of and reprioritizing the following tasks: {task_descriptions}. "
+        f"You are a task prioritization AI tasked with cleaning the formatting of and reprioritizing the following tasks: {task_descriptions}. "
         f"Consider the ultimate objective of your team: {objective}. \n"
         "Tasks should be sorted from highest to lowest priority.\n"
         "Higher-priority tasks are those that act as pre-requisites or are more essential for meeting the objective.\n"
         f"Do not remove any tasks and don't add any new tasks. Return the result as a numbered list, like:\n"
         "#. First task\n"
         "#. Second task\n"
         f"Start the task list with number {next_task_id}."
     )
 
-    messages = [create_message(prompt)]
+    messages = create_message(prompt)
     response = create_chat_completion(
         model=Config().fast_llm_model,
         messages=messages,
     )
 
     new_tasks = response.split('\n')
     task_list = []
     for task_string in new_tasks:
         task_parts = task_string.strip().split(".", 1)
         if len(task_parts) == 2:
             task_id = task_parts[0].strip()
             task_description = task_parts[1].strip()
-            task_list.append({"task_id": task_id, "task_description": task_description})
+            task_list.append({"id": task_id, "task": task_description})
     return task_list
 
 def init_task_list(objective: str, max_tasks_count: Optional[int] = 4) -> List[Dict]:
     task_id_counter = 0
     prompt = (
-        f"You are an task creation AI that creates tasks with the following objective: {objective}.\n"
+        f"You are a task management AI tasked with creating tasks for the following objective: {objective}.\n"
         f"Up to {max_tasks_count - 1} new tasks can be created to complete this objective. "
         "You should only respond in JSON format as described below \n"
         f"Response Format: \n{response_format} \nEnsure the response can be parsed by Python json.loads"
     )
-    messages = [create_message(prompt)]
+    messages = create_message(prompt)
     response = create_chat_completion(
         model=Config().fast_llm_model,
         messages=messages,
     )
 
     new_tasks = json.loads(response)
     task_list = []
```

### Comparing `autoxx-0.0.11/autoxx/js/overlay.js` & `autoxx-0.0.12/autoxx/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.11/autoxx/search/simple_search.py` & `autoxx-0.0.12/autoxx/search/simple_search.py`

 * *Files 7% similar despite different names*

```diff
@@ -113,15 +113,31 @@
 
     Args:
         driver (WebDriver): The webdriver to use to add the header
 
     Returns:
         None
     """
-    driver.execute_script(open(f"{FILE_DIR}/js/overlay.js", "r").read())
+    try:
+        with open(f"{FILE_DIR}/js/overlay.js", "r") as overlay_file:
+            overlay_script = overlay_file.read()
+        driver.execute_script(overlay_script)
+    except Exception as e:
+        print(f"Error executing overlay.js: {e}")
+
+def close_browser(driver: WebDriver) -> None:
+    """Close the browser
+
+    Args:
+        driver (WebDriver): The webdriver to close
+
+    Returns:
+        None
+    """
+    driver.quit()
 
 
 def browse_website(url: str, question: str) -> List[str]:
     """Browse a website and summarize it
 
     Args:
         url (str): The url to browse
@@ -129,14 +145,15 @@
 
     Returns:
         str: The summary of the website
     """
     driver, text = scrape_text_with_selenium(url=url)
     add_header(driver)
     summary = summarize_chunks(text=text, question=question, url=url, driver=driver)
+    close_browser(driver)
     return summary
 
 def simple_search(question:str, search_num:Optional[int]=2) -> str:
     search_result = google_search(query=question, num_results=search_num)
     search_search_json = json.loads(search_result)
     summaries = []
```

### Comparing `autoxx-0.0.11/autoxx/task_manager.py` & `autoxx-0.0.12/autoxx/task_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,44 +23,44 @@
 
     def execute(self) -> str:
         self.status = "running"
         # Main loop
         while self.task_cur < len(self.task_list):
             # Print the task list
             incomplete_list = [self.task_list[i]  for i in range(self.task_cur, len(self.task_list))]
-            logging.info(f"\033[95m\033[1m INCOMPLETE TASK LIST({self.objective}) \033[0m\033[0m {[str(t['task_id'])+': '+t['task_description'] for t in incomplete_list]}")
+            logging.info(f"\033[95m\033[1m INCOMPLETE TASK LIST({self.objective}) \033[0m\033[0m {[str(t['id'])+': '+t['task'] for t in incomplete_list]}")
 
             # Step 1: Pull the first task
             task = incomplete_list[0]
-            logging.info(f"\033[92m\033[1m NEXT TASK({self.objective}) \033[0m\033[0m" + str(task['task_id'])+": "+task['task_description'])
+            logging.info(f"\033[92m\033[1m NEXT TASK({self.objective}) \033[0m\033[0m" + str(task['id'])+": "+task['task'])
 
             try:
                 # Send to execution function to complete the task based on the context
-                result = self.agent.execute(self.objective, task["task_description"])
-                this_task_id = int(task["task_id"])
+                result = self.agent.execute(self.objective, task["task"])
+                this_task_id = int(task["id"])
                 logging.info(f"\033[93m\033[1m TASK RESULT({self.objective}) \033[0m\033[0m {result}")
             except Exception as e:  
                 logging.error(f"An error occurred while executing the task({self.objective}): {e}")
                 self.status = "error"
                 self.error_message = str(e)  
                 return str(e)
                 # You can also handle specific exceptions if needed, e.g., KeyError, ValueError, etc.  
                 # To do this, add additional except blocks for each specific exception type.  
 
-            task["data"] = result
+            task["result"] = result
             self.task_cur += 1
 
             # Step 2: Create new tasks
             task_id_counter = len(self.task_list)
             if self.max_tasks_count-task_id_counter > 0:
-                new_tasks = task_creation_agent(self.objective,  task, [t["task_description"]  for t in self.task_list[self.task_cur:]], self.max_tasks_count-task_id_counter)
+                new_tasks = task_creation_agent(self.objective,  task, [t["task"]  for t in self.task_list[self.task_cur:]], self.max_tasks_count-task_id_counter)
 
                 for new_task in new_tasks:
                     task_id_counter += 1
-                    new_task.update({"task_id": task_id_counter})
+                    new_task.update({"id": task_id_counter})
                     self.task_list.append(new_task)
 
                 incomplete_list = incomplete_list[1:]
                 # Step 3: Reprioritize task list
                 if len(self.task_list)-self.task_cur > 1:
                     reprioritized_tasks = prioritization_agent(this_task_id, self.objective, self.task_list[self.task_cur:])
                     self.task_list = self.task_list[:self.task_cur] + reprioritized_tasks
@@ -72,15 +72,15 @@
                 return final_result
             time.sleep(1)  # Sleep before checking the task list again
 
     def stat(self) -> Dict:
         current = self.task_cur
         if current >= len(self.task_list):
             current -= 1
-        return {"current_task": self.task_list[current]["task_id"], "task_list": self.task_list, "final_answer": self.final_answer, "status": self.status, "error_message": self.error_message}
+        return {"current_task": self.task_list[current]["id"], "task_list": self.task_list, "final_answer": self.final_answer, "status": self.status, "error_message": self.error_message}
   
 class TaskManager:  
     def __init__(self):  
         self.tasks = {}  
   
     def create_task(self, objective: str, max_tasks_count: Optional[int] = 3):  
         if objective in self.tasks:
```

### Comparing `autoxx-0.0.11/pyproject.toml` & `autoxx-0.0.12/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.11"
+version = "0.0.12"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `autoxx-0.0.11/PKG-INFO` & `autoxx-0.0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.11
+Version: 0.0.12
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

