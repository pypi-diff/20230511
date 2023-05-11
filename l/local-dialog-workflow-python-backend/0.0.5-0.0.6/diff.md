# Comparing `tmp/local-dialog-workflow-python-backend-0.0.5.tar.gz` & `tmp/local-dialog-workflow-python-backend-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local-dialog-workflow-python-backend-0.0.5.tar", last modified: Fri Apr 28 23:19:56 2023, max compression
+gzip compressed data, was "local-dialog-workflow-python-backend-0.0.6.tar", last modified: Thu May 11 18:35:22 2023, max compression
```

## Comparing `local-dialog-workflow-python-backend-0.0.5.tar` & `local-dialog-workflow-python-backend-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:19:56.826454 local-dialog-workflow-python-backend-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-28 23:19:56.826454 local-dialog-workflow-python-backend-0.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:19:56.826454 local-dialog-workflow-python-backend-0.0.5/dialog_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    19852 2023-04-28 23:19:44.000000 local-dialog-workflow-python-backend-0.0.5/dialog_workflow/Act.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-28 23:19:44.000000 local-dialog-workflow-python-backend-0.0.5/dialog_workflow/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-28 23:19:44.000000 local-dialog-workflow-python-backend-0.0.5/dialog_workflow/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-28 23:19:44.000000 local-dialog-workflow-python-backend-0.0.5/dialog_workflow/TablesAsObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 23:19:44.000000 local-dialog-workflow-python-backend-0.0.5/dialog_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-28 23:19:44.000000 local-dialog-workflow-python-backend-0.0.5/dialog_workflow/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-04-28 23:19:44.000000 local-dialog-workflow-python-backend-0.0.5/dialog_workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:19:56.826454 local-dialog-workflow-python-backend-0.0.5/local_dialog_workflow_python_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-28 23:19:56.000000 local-dialog-workflow-python-backend-0.0.5/local_dialog_workflow_python_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-28 23:19:56.000000 local-dialog-workflow-python-backend-0.0.5/local_dialog_workflow_python_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:19:56.000000 local-dialog-workflow-python-backend-0.0.5/local_dialog_workflow_python_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 23:19:56.000000 local-dialog-workflow-python-backend-0.0.5/local_dialog_workflow_python_backend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-28 23:19:44.000000 local-dialog-workflow-python-backend-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 23:19:56.826454 local-dialog-workflow-python-backend-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-28 23:19:44.000000 local-dialog-workflow-python-backend-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:35:22.842187 local-dialog-workflow-python-backend-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-11 18:35:22.842187 local-dialog-workflow-python-backend-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-11 18:35:11.000000 local-dialog-workflow-python-backend-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:35:22.842187 local-dialog-workflow-python-backend-0.0.6/dialog_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    19827 2023-05-11 18:35:11.000000 local-dialog-workflow-python-backend-0.0.6/dialog_workflow/Act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-11 18:35:11.000000 local-dialog-workflow-python-backend-0.0.6/dialog_workflow/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-11 18:35:11.000000 local-dialog-workflow-python-backend-0.0.6/dialog_workflow/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-11 18:35:11.000000 local-dialog-workflow-python-backend-0.0.6/dialog_workflow/TablesAsObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:35:11.000000 local-dialog-workflow-python-backend-0.0.6/dialog_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-11 18:35:11.000000 local-dialog-workflow-python-backend-0.0.6/dialog_workflow/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-05-11 18:35:11.000000 local-dialog-workflow-python-backend-0.0.6/dialog_workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:35:22.842187 local-dialog-workflow-python-backend-0.0.6/local_dialog_workflow_python_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-11 18:35:22.000000 local-dialog-workflow-python-backend-0.0.6/local_dialog_workflow_python_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-11 18:35:22.000000 local-dialog-workflow-python-backend-0.0.6/local_dialog_workflow_python_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:35:22.000000 local-dialog-workflow-python-backend-0.0.6/local_dialog_workflow_python_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 18:35:22.000000 local-dialog-workflow-python-backend-0.0.6/local_dialog_workflow_python_backend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 18:35:11.000000 local-dialog-workflow-python-backend-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 18:35:22.842187 local-dialog-workflow-python-backend-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-11 18:35:11.000000 local-dialog-workflow-python-backend-0.0.6/setup.py
```

### Comparing `local-dialog-workflow-python-backend-0.0.5/dialog_workflow/Act.py` & `local-dialog-workflow-python-backend-0.0.6/dialog_workflow/Act.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from dialog_workflow.utils import *
+from utils import *
 import time
 import msvcrt
 import requests
 from AgeDetection import DetectAge
-from dialog_workflow.TablesAsObjects import DialogWorkflowRecord, Variable, ProfileContext
+from TablesAsObjects import DialogWorkflowRecord, Variable, ProfileContext
 
 class action(object):
     def __init__(self, incoming_message: str, profile_id: int, language: str, profile_curr_state: int, variables: Variable):
         self.incoming_message = incoming_message
         self.profile_id = profile_id
         self.language = language
         self.variables = variables
         self.profile_curr_state = profile_curr_state
         self.accumulated_message = ""
         self.profile = ProfileContext()
+        self.variable = Variable()
 
     def act(self, dialog_workflow_record: DialogWorkflowRecord, got_response: bool):
         """This function applies the action of the relevant record with the profile's current state id.
         Params:
             1. dialog_workflow_record: The current record from the dialog workflow state table that is applied.
             2. got_response a bool indicator telling us if the user had sent back a response to the last outgoing message
                that we sent him from the same action or not. This will help understand if the action should 
@@ -69,29 +70,29 @@
                 return self.insert_missing_data()                
                                  
             
     def text_message_action(self):
         """Prints the paramter1 message after formatting: 
         "Hello {First Name}, how are you {feeling|doing}?" --> "Hello Tal, how are you doing? """
         message = self.record.parameter1
-        replace_fields_with_values_class = replace_fields_with_values(message, self.language, Variable())
+        replace_fields_with_values_class = replace_fields_with_values(message, self.language, self.variable)
         formatted_message = replace_fields_with_values_class.get_variable_values_and_chosen_option()
         self.accumulated_message = self.accumulated_message + formatted_message + '~'
         return False, None
 
     def question_action(self):
         """Asks a question and waits for an answer from user on STDIN. If the user responded in a certain amount of time,
         then moves to next state, otherwise moves to a different state.
         Note: this function waits for input for a certain amount of time only if using console application.
               If using websocket we send a json message to the user and exit the code normally"""
 
         if not self.got_response:
             self.accumulated_message += self.record.parameter1
-            outgoing_message = process_message(communication_type= DEFAULT_COMMUNICATION_TYPE, action_type= action_enum.TEXT_MESSAGE_ACTION.value, message= self.accumulated_message) 
-            if DEFAULT_COMMUNICATION_TYPE == communication_type_enum.WEBSOCKET.value:
+            outgoing_message = process_message(communication_type= COMMUNICATION_TYPE, action_type= action_enum.TEXT_MESSAGE_ACTION.value, message= self.accumulated_message) 
+            if COMMUNICATION_TYPE == communication_type_enum.WEBSOCKET.value:
                 return False, outgoing_message
             else:
                 self.accumulated_message = ""
             
             waiting_time = self.record.no_feedback_milliseconds 
             start_time = time.monotonic()
             input_str = None
@@ -179,33 +180,34 @@
         self.record.parameter1 = "" if self.record.parameter1 == None else self.record.parameter1
         if not self.got_response: #Adds the question and instructions to the accumulated_message to be sent to user.
             self.accumulated_message = self.accumulated_message + self.record.parameter1 +"~" + f"Please choose EXACTLY ONE option between 1-{len(child_nodes)}:~"
         is_state_changed, next_state_id, outgoing_message = generic_user_choice_action(self.record, self.accumulated_message, child_nodes, choose_exactly_one_option=True, got_response=self.got_response, chosen_numbers=self.incoming_message, profile=self.profile)
         if outgoing_message != None: #returns the outgoing message to send to the user.
             return False, outgoing_message
         self.profile_curr_state = next_state_id
+        self.accumulated_message = ""
         return is_state_changed, None
         
     def age_detection(self):
         """Action that recieves a path to a picture (for now the picture has to be stored in the folder) 
             and returns the approximate age of the person in the picture.
             Stores the picture in database storage."""
         if not self.got_response:
             self.accumulated_message += "Please insert a path to the picture~"
-            outgoing_message = process_message(communication_type= DEFAULT_COMMUNICATION_TYPE, action_type= action_enum.AGE_DETECTION.value, message= self.accumulated_message) 
-            if DEFAULT_COMMUNICATION_TYPE == communication_type_enum.WEBSOCKET.value:
+            outgoing_message = process_message(communication_type= COMMUNICATION_TYPE, action_type= action_enum.AGE_DETECTION.value, message= self.accumulated_message) 
+            if COMMUNICATION_TYPE == communication_type_enum.WEBSOCKET.value:
                 return False, outgoing_message
             else:
-                self.accumulated_message = ""            
-        else:
-            age_range = DetectAge.detect(self.incoming_message)
-            self.accumulated_message += f'The approximate age of the picture you have sent is: {age_range}~'
-            insert_profile_variable_value(self.profile_id, self.record.variable1_id, age_range, self.profile_curr_state)
-            store_age_detection_picture(age_range, self.profile_curr_state)
-            return False, None
+                self.accumulated_message = ""         
+                self.incoming_message = input()
+        age_range = DetectAge.detect(self.incoming_message)
+        self.accumulated_message += f'The approximate age of the picture you have sent is: {age_range}~'
+        insert_profile_variable_value(self.profile_id, self.record.variable1_id, age_range, self.profile_curr_state)
+        store_age_detection_picture(age_range, self.profile_curr_state)
+        return False, None
     
     def multi_choice_poll(self):
         """ Similar to Menu Action. If the user chose a single option we jump to next_state_id of the chosen option. 
             Otherwise we save the answers and jump to the next_state_id of the parent."""
         fields_to_select = ["parameter1", "next_state_id"]
         table_name = "dialog_workflow_state_view"
         values_from_where_to_select = [self.record.curr_state_id]
@@ -231,16 +233,16 @@
             Saves the chosen options in profile context."""
         groups = get_groups_with_text(self.record.parameter1)
         if not self.got_response:
             self.accumulated_message += "Please choose your desired interests. You may select more than one choice with a comma seperator.~"
             for i, child in enumerate(groups):
                 self.accumulated_message = self.accumulated_message + f'{i+1}) {child["title"]}~'            
             
-            outgoing_message = process_message(communication_type= DEFAULT_COMMUNICATION_TYPE, action_type= action_enum.PRESENT_GROUPS_WITH_CERTAIN_TEXT.value, message=self.accumulated_message) 
-            if DEFAULT_COMMUNICATION_TYPE == communication_type_enum.WEBSOCKET.value:
+            outgoing_message = process_message(communication_type= COMMUNICATION_TYPE, action_type= action_enum.PRESENT_GROUPS_WITH_CERTAIN_TEXT.value, message=self.accumulated_message) 
+            if COMMUNICATION_TYPE == communication_type_enum.WEBSOCKET.value:
                 return False, outgoing_message 
             else:
                 self.accumulated_message = ""
                 chosen_numbers = input()          
         else:
                 chosen_numbers = self.incoming_message.split(',')
                 chosen_numbers_list = [int(x) for x in chosen_numbers]
@@ -255,16 +257,16 @@
         parameter1_list = self.record.parameter1.split(",")
         schema = parameter1_list[0]
         table = parameter1_list[1]
         field_name = parameter1_list[2]
         record_id = parameter1_list[3]
         if not self.got_response:
             self.accumulated_message += f"Please insert your {field_name}~"
-            outgoing_message = process_message(communication_type= DEFAULT_COMMUNICATION_TYPE, action_type= action_enum.TEXT_MESSAGE_ACTION.value, message= self.accumulated_message) 
-            if DEFAULT_COMMUNICATION_TYPE == communication_type_enum.WEBSOCKET.value:
+            outgoing_message = process_message(communication_type= COMMUNICATION_TYPE, action_type= action_enum.TEXT_MESSAGE_ACTION.value, message= self.accumulated_message) 
+            if COMMUNICATION_TYPE == communication_type_enum.WEBSOCKET.value:
                 return False, outgoing_message
             else:
                 self.accumulated_message = ""
                 self.incoming_message = input()            
         else:
             try:
                 cursor.execute(f"""USE {schema}""")
@@ -283,16 +285,16 @@
             1. True if the users' next state should be changed to a child next state, False if there's no need to change it's state
             2. The next state id that the profile should be in, or None if the action didn't result in a change of state.
             3. The outging message to be sent to the user, or None if the message had already been sent."""
     # This is the first part of the action: sending the request to the user and waiting for an answer.
     if not got_response:
         for i, child in enumerate(child_nodes):
             accumulated_message = accumulated_message + f'{i+1}) {child["parameter1"]}~'
-        outgoing_message = process_message(communication_type= DEFAULT_COMMUNICATION_TYPE, action_type= action_enum.TEXT_MESSAGE_ACTION.value, message= accumulated_message) 
-        if DEFAULT_COMMUNICATION_TYPE == communication_type_enum.WEBSOCKET.value:
+        outgoing_message = process_message(communication_type= COMMUNICATION_TYPE, action_type= action_enum.TEXT_MESSAGE_ACTION.value, message= accumulated_message) 
+        if COMMUNICATION_TYPE == communication_type_enum.WEBSOCKET.value:
             return False, record.next_state_id, outgoing_message 
         else:
             chosen_numbers = input()
 
 
     # The user has to pick exactly one option
     if choose_exactly_one_option:
```

### Comparing `local-dialog-workflow-python-backend-0.0.5/dialog_workflow/Constants.py` & `local-dialog-workflow-python-backend-0.0.6/dialog_workflow/Constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     PRESENT_CHILD_GROUPS_NAMES_BY_ID = 13
     PRESENT_GROUPS_WITH_CERTAIN_TEXT = 14
     INSERT_MISSING_DATA = 15
 
 class communication_type_enum(Enum):
     CONSOLE = 1
     WEBSOCKET = 2
-DEFAULT_COMMUNICATION_TYPE = 1
+COMMUNICATION_TYPE = 2
 
 VARIABLE_NAMES_DICT = {1 : "Person Id" , 2 : "User Id", 3 : "Profile Id", 4 : "Lang Code", 
                        5 : "Name Prefix", 6 : "First Name", 7 : "Middle Name" , 
                        8 : "Last Name", 9 : "Name Suffix",  10 : "Full Name", 
                        11 : "Country", 12 : "State" , 13 : "County" , 14 : "City", 
                        15 : "Neighborhood", 16 : "Street", 17 : "House", 18 : "Suite/Apartment", 
                        19 : "Zip Code", 20 : "Post Result", 21 : "Age", 22 : "Result"}
```

### Comparing `local-dialog-workflow-python-backend-0.0.5/dialog_workflow/DialogWorkflow.py` & `local-dialog-workflow-python-backend-0.0.6/dialog_workflow/DialogWorkflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from dialog_workflow.utils import *
-from dialog_workflow.Act import action
-from dialog_workflow.TablesAsObjects import DialogWorkflowRecord, Variable
+from utils import *
+from Act import action
+from TablesAsObjects import DialogWorkflowRecord, Variable
 
 
 def get_preferred_language(profile_id: int):
     cursor.execute("""USE profile""")
     cursor.execute("""SELECT preferred_lang_code FROM profile_view WHERE user_id = %s""", [profile_id])
     language = (cursor.fetchone())["preferred_lang_code"]
     cursor.execute("""USE dialog_workflow""")
@@ -33,8 +33,7 @@
         is_state_changed, outgoing_message = init_action.act(dialog_workflow_record, got_response)
         if outgoing_message != None:
             return outgoing_message
         init_action.profile_curr_state = dialog_workflow_record.next_state_id if is_state_changed == False else init_action.profile_curr_state
         update_profile_curr_state_in_DB(init_action.profile_curr_state, profile_id)
         got_response = False
 
-
```

### Comparing `local-dialog-workflow-python-backend-0.0.5/dialog_workflow/TablesAsObjects.py` & `local-dialog-workflow-python-backend-0.0.6/dialog_workflow/TablesAsObjects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from dialog_workflow.Constants import *
-from dialog_workflow.utils import insert_profile_variable_value, get_curr_state, get_variable_value_by_id
+from Constants import *
+from utils import insert_profile_variable_value, get_curr_state, get_variable_value_by_id
 
 class Variable(object):
     def __init__(self):
         self.name2id_dict = {}
         self.id2name_dict = {}
         self.next_variable_id = 1
         for variable_id in VARIABLE_NAMES_DICT:
```

### Comparing `local-dialog-workflow-python-backend-0.0.5/dialog_workflow/test.py` & `local-dialog-workflow-python-backend-0.0.6/dialog_workflow/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
-sys.path.append("C:\\Users\\User\\OneDrive\\Circles\\dialog-workflow-backend")
+# sys.path.append("C:\\Users\\User\\OneDrive\\Circles\\dialog-workflow-backend")
 import unittest
-from dialog_workflow.TablesAsObjects import *
-from dialog_workflow.DialogWorkflow import *
-from dialog_workflow.Constants import *
+from TablesAsObjects import *
+from DialogWorkflow import *
+from Constants import *
 
 """Please make sure to fill al the relevant data in the database in order for the tests to run correctly"""
 class TestVariable(unittest.TestCase):
     def setUp(self):
         self.variables = Variable() 
 
     def test_add(self):
@@ -122,26 +122,25 @@
         self.assertEqual(self.action.profile_curr_state, (child_nodes[int(incoming_message)-1])["next_state_id"])
     
     def test_age_detection(self):
         self.record_dict["workflow_action_id"] = 11
         self.record_dict["parameter1"] = "middle"
         self.record_dict["variable1_id"] = 7
         self.action.record = DialogWorkflowRecord(self.record_dict)        
-        _, json_message = self.action.age_detection(DEFAULT_COMMUNICATION_TYPE, self.record)
+        _, json_message = self.action.age_detection(COMMUNICATION_TYPE, self.record)
         self.assertEqual(json_message, self.record.parameter1)
 
     def test_multi_choice_poll_got_response_true(self): #Also tests the generic_user_choice_action function
         self.action.incoming_message = "1,2,3"
         ret = self.action.multi_choice_poll()
         self.assertEqual(ret, (False, None))
     
     def test_replace_fields_with_values(self):
         message = "My age is {Age}"
         replace_fields_with_values_class = replace_fields_with_values(message, "en", Variable())
         formatted_message = replace_fields_with_values_class.get_variable_values_and_chosen_option()
         self.assertEqual(formatted_message, "My age is 25")
 
 if __name__ == '__main__':
-    # unittest.main()
-    print(post_message(1,"1"))
+    unittest.main()
```

### Comparing `local-dialog-workflow-python-backend-0.0.5/dialog_workflow/utils.py` & `local-dialog-workflow-python-backend-0.0.6/dialog_workflow/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # TODO: Let's talk about Constants and the usage in this file
-from dialog_workflow.Constants import *
+from Constants import *
 import random
 import json
 from circles_local_aws_s3_storage_python.AWSStorage import AwsS3Storage
 
 # TOOD: Please include type to all parameters.
 # TODO: Please include return value.
 # TODO: Please add short documentation per PEP8 standard
```

### Comparing `local-dialog-workflow-python-backend-0.0.5/setup.py` & `local-dialog-workflow-python-backend-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='local-dialog-workflow-python-backend',  
-     version='0.0.5',
+     version='0.0.6',
      author="Circles",
      author_email="info@circle.life",
      description="PyPI Package for dialog workflow",
      long_description="This is a package for running the dialog workflow",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

