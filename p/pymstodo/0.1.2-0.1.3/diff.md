# Comparing `tmp/pymstodo-0.1.2.tar.gz` & `tmp/pymstodo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymstodo-0.1.2.tar", last modified: Thu May 11 06:10:25 2023, max compression
+gzip compressed data, was "pymstodo-0.1.3.tar", last modified: Thu May 11 13:56:57 2023, max compression
```

## Comparing `pymstodo-0.1.2.tar` & `pymstodo-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:10:25.453453 pymstodo-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-11 06:10:07.000000 pymstodo-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-11 06:10:25.453453 pymstodo-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-11 06:10:07.000000 pymstodo-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:10:25.449453 pymstodo-0.1.2/pymstodo/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 06:10:07.000000 pymstodo-0.1.2/pymstodo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-05-11 06:10:07.000000 pymstodo-0.1.2/pymstodo/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:10:25.453453 pymstodo-0.1.2/pymstodo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-11 06:10:25.000000 pymstodo-0.1.2/pymstodo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-11 06:10:25.000000 pymstodo-0.1.2/pymstodo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 06:10:25.000000 pymstodo-0.1.2/pymstodo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-11 06:10:25.000000 pymstodo-0.1.2/pymstodo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 06:10:25.000000 pymstodo-0.1.2/pymstodo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 06:10:25.453453 pymstodo-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-11 06:10:07.000000 pymstodo-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:56:57.640868 pymstodo-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-11 13:56:48.000000 pymstodo-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-11 13:56:57.640868 pymstodo-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-11 13:56:48.000000 pymstodo-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:56:57.640868 pymstodo-0.1.3/pymstodo/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 13:56:48.000000 pymstodo-0.1.3/pymstodo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18737 2023-05-11 13:56:48.000000 pymstodo-0.1.3/pymstodo/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:56:57.640868 pymstodo-0.1.3/pymstodo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-11 13:56:57.000000 pymstodo-0.1.3/pymstodo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-11 13:56:57.000000 pymstodo-0.1.3/pymstodo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 13:56:57.000000 pymstodo-0.1.3/pymstodo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-11 13:56:57.000000 pymstodo-0.1.3/pymstodo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 13:56:57.000000 pymstodo-0.1.3/pymstodo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 13:56:57.640868 pymstodo-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-11 13:56:48.000000 pymstodo-0.1.3/setup.py
```

### Comparing `pymstodo-0.1.2/LICENSE` & `pymstodo-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymstodo-0.1.2/PKG-INFO` & `pymstodo-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymstodo
-Version: 0.1.2
+Version: 0.1.3
 Summary: Microsoft To Do API client
 Home-page: https://github.com/inbalboa/pymstodo
 Author: Sergey Shlyapugin
 Author-email: shlyapugin@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pymstodo-0.1.2/README.md` & `pymstodo-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pymstodo-0.1.2/pymstodo/client.py` & `pymstodo-0.1.3/pymstodo/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import os
 import time
 import json
 import dataclasses
 from datetime import datetime
+from enum import Enum
 from typing import Any, Dict, List, Literal, Optional, TypedDict, Union
 
 from requests_oauthlib import OAuth2Session
 
 
 class PymstodoError(Exception):
+    '''Basic Pymstodo exception'''
     pass
 
 
 class Token(TypedDict):
     token_type: str
     scope: List[str]
     expires_in: int
@@ -29,193 +31,255 @@
 
 
 class _Body(TypedDict):
     content: str
     contentType: Literal['text', 'html']
 
 
-@dataclasses.dataclass
-class TaskList:
+class WellknownListName(Enum):
+    '''
+    Well-known list name
+
+    Attributes:
+        DEFAULT_LIST: Default list
+        FLAGGED_EMAILS: Flagged emails
+        UNKNOWN_FUTURE_VALUE: Unknown future value
+    '''
+
+    DEFAULT_LIST = 'defaultList'
+    FLAGGED_EMAILS = 'flaggedEmails'
+    UNKNOWN_FUTURE_VALUE = 'unknownFutureValue'
+
+
+class TaskStatus(Enum):
+    '''
+    The state or progress of the task
+
+    Attributes:
+        notStarted: not started
+        inProgress: in progress
+        completed: completed
+        waitingOnOthers: waiting on others
+        deferred: deferred
     '''
-    **To-Do task list** contains one or more todoTask resources.
+
+    NOT_STARTED = 'notStarted'
+    IN_PROGRESS = 'inProgress'
+    COMPLETED = 'completed'
+    WAITING_ON_OTHERS = 'waitingOnOthers'
+    DEFERRED = 'deferred'
+
+
+class TaskStatusFilter(Enum):
     '''
+    Tasks status filter
+
+    Attributes:
+        completed: only completed tasks
+        notCompleted: only non-completed tasks
+        all: all tasks
+    '''
+
+    COMPLETED = 'completed'
+    NOT_COMPLETED = 'notCompleted'
+    ALL = 'all'
+
+
+@dataclasses.dataclass
+class TaskList:
+    '''**To-Do task list** contains one or more task'''
 
     list_id: str
-    '''The identifier of the task list, unique in the user's mailbox. Read-only.'''
+    '''The identifier of the task list, unique in the user's mailbox. Read-only'''
 
     displayName: str
-    '''The name of the task list.'''
+    '''The name of the task list'''
 
     isOwner: bool
-    '''`True` if the user is owner of the given task list.'''
+    '''`True` if the user is owner of the given task list'''
 
     isShared: bool
-    '''`True` if the task list is shared with other users.'''
+    '''`True` if the task list is shared with other users'''
 
-    wellknownListName: Literal['none', 'defaultList', 'flaggedEmails', 'unknownFutureValue']
-    '''Property indicating the list name if the given list is a well-known list. Possible values are: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.'''
+    wellknownListName: str
 
     def __init__(self, **kwargs: Any) -> None:
         for f in dataclasses.fields(self):
             setattr(self, f.name, kwargs.get('id' if f.name == 'list_id' else f.name))
 
     def __str__(self) -> str:
         return self.displayName.replace('|', '—').strip()
 
     @property
     def link(self) -> str:
+        '''Link to the task list on web.'''
         return 'href=https://to-do.live.com/tasks/{self.list_id}'
 
+    @property
+    def wellknown_list_name(self) -> Optional[WellknownListName]:
+        '''Property indicating the list name if the given list is a well-known list'''
+        return None if self.wellknownListName == 'none' else WellknownListName(self.wellknownListName)
+
 
 @dataclasses.dataclass
 class Task:
-    '''
-    **To-Do task** represents a task, such as a piece of work or personal item, that can be tracked and completed.
-    '''
+    '''**To-Do task** represents a task, such as a piece of work or personal item, that can be tracked and completed'''
 
     task_id: str
-    '''Unique identifier for the task. By default, this value changes when the item is moved from one list to another.'''
+    '''Unique identifier for the task. By default, this value changes when the item is moved from one list to another'''
 
     body: _Body
 
     categories: list[str]
-    '''The categories associated with the task.'''
+    '''The categories associated with the task'''
 
     completedDateTime: str
+    '''The date and time in the specified time zone that the task was finished. It is in UTC and uses ISO 8601 format'''
+
     createdDateTime: str
+    '''The date and time when the task was created. It is in UTC and uses ISO 8601 format'''
+
     dueDateTime: _DueDate
 
     hasAttachments: bool
-    '''Indicates whether the task has attachments.'''
+    '''Indicates whether the task has attachments'''
 
     title: str
-    '''A brief description of the task.'''
+    '''A brief description of the task'''
 
     importance: Literal['low', 'normal', 'high']
-    '''The importance of the task. Possible values are: `low`, `normal`, `high`.'''
+    '''The importance of the task. Possible values are: `low`, `normal`, `high`'''
 
     isReminderOn: bool
-    '''Set to true if an alert is set to remind the user of the task.'''
+    '''Set to true if an alert is set to remind the user of the task'''
 
     lastModifiedDateTime: str
+    '''The date and time when the task was last modified. It is in UTC and uses ISO 8601 format'''
+
     reminderDateTime: str
+    '''The date and time in the specified time zone for a reminder alert of the task to occur. Uses ISO 8601 format'''
+
     startDateTime: str
+    '''The date and time in the specified time zone at which the task is scheduled to start. Uses ISO 8601 format'''
 
-    status: Literal['notStarted', 'inProgress', 'completed', 'waitingOnOthers', 'deferred']
-    '''Indicates the state or progress of the task. Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.'''
+    status: str
 
     def __init__(self, **kwargs: Any) -> None:
         for f in dataclasses.fields(self):
             setattr(self, f.name, kwargs.get('id' if f.name == 'task_id' else f.name))
 
     def __str__(self) -> str:
         title = self.title.replace('|', '—').strip()
         if self.due_date:
             title += f' • Due {self.due_date.strftime("%x")}'
 
         return title
 
     @property
     def body_text(self) -> Optional[str]:
-        '''The task body that typically contains information about the task.'''
+        '''The task body that typically contains information about the task'''
         if self.body:
             return self.body['content']
         else:
             return None
 
     @property
     def completed_date(self) -> Optional[datetime]:
-        '''The date and time in the specified time zone that the task was finished.'''
+        '''The date and time in the specified time zone that the task was finished'''
         if self.completedDateTime:
             return datetime.strptime(self.completedDateTime.split('.')[0], '%Y-%m-%dT%H:%M:%S')
         else:
             return None
 
     @property
     def created_date(self) -> Optional[datetime]:
-        '''The date and time when the task was created. It is in UTC.'''
+        '''The date and time when the task was created. It is in UTC'''
         if self.createdDateTime:
             return datetime.strptime(self.createdDateTime.split('.')[0], '%Y-%m-%dT%H:%M:%S')
         else:
             return None
 
     @property
     def due_date(self) -> Optional[datetime]:
-        '''The date and time in the specified time zone that the task is to be finished.'''
+        '''The date and time in the specified time zone that the task is to be finished'''
         if self.dueDateTime:
             return datetime.strptime(self.dueDateTime['dateTime'].split('.')[0], '%Y-%m-%dT%H:%M:%S')
         else:
             return None
 
     @property
     def last_mod_date(self) -> Optional[datetime]:
-        '''The date and time when the task was last modified. It is in UTC.'''
+        '''The date and time when the task was last modified. It is in UTC'''
         if self.lastModifiedDateTime:
             return datetime.strptime(self.lastModifiedDateTime.split('.')[0], '%Y-%m-%dT%H:%M:%S')
         else:
             return None
 
     @property
     def reminder_date(self) -> Optional[datetime]:
-        '''The date and time in the specified time zone for a reminder alert of the task to occur.'''
+        '''The date and time in the specified time zone for a reminder alert of the task to occur'''
         if self.reminderDateTime:
             return datetime.strptime(self.reminderDateTime.split('.')[0], '%Y-%m-%dT%H:%M:%S')
         else:
             return None
 
     @property
     def start_date(self) -> Optional[datetime]:
-        '''The date and time in the specified time zone at which the task is scheduled to start.    '''
+        '''The date and time in the specified time zone at which the task is scheduled to start'''
         if self.startDateTime:
             return datetime.strptime(self.startDateTime.split('.')[0], '%Y-%m-%dT%H:%M:%S')
         else:
             return None
 
+    @property
+    def task_status(self) -> TaskStatus:
+        '''Indicates the state or progress of the task'''
+        return TaskStatus(self.status)
+
 
 class ToDoConnection:
-    '''**To-Do connection**
-    your entry point to To-Do API
+    '''**To-Do connection** is your entry point to the To-Do API
+
+    Args:
+        client_id: API client ID
+        client_secret: API client secret
+        token: Token obtained by method `get_token`        
     '''
     _redirect: str = 'https://localhost/login/authorized'
     _scope: str = 'openid offline_access tasks.readwrite'
     _authority: str = 'https://login.microsoftonline.com/common'
     _authorize_endpoint: str = '/oauth2/v2.0/authorize'
     _token_endpoint: str = '/oauth2/v2.0/token'
     _base_api_url: str = 'https://graph.microsoft.com/v1.0/me/todo/'
 
     def __init__(self, client_id: str, client_secret: str, token: Token) -> None:
         self.client_id: str = client_id
-        '''API client ID.'''
-
         self.client_secret: str = client_secret
-        '''API client secret.'''
-
         self.token: Token = token
-        '''Token obtained by method `get_token`.'''
 
     @staticmethod
     def get_auth_url(client_id: str) -> Any:
-        '''Get the authorization_url.
-    
+        '''Get the authorization_url
+
         Args:
             client_id: API client ID
 
         Returns:
-            Authorization URL to show to the user.
+            Authorization URL to show to the user
         '''
         oa_sess = OAuth2Session(client_id, scope=ToDoConnection._scope, redirect_uri=ToDoConnection._redirect)
 
         authorize_url = f'{ToDoConnection._authority}{ToDoConnection._authorize_endpoint}'
         authorization_url, _ = oa_sess.authorization_url(authorize_url)
 
         return authorization_url
 
     @staticmethod
     def get_token(client_id: str, client_secret: str, redirect_resp: str) -> Any:
-        '''Fetch the access token.'''
+        '''Fetch the access token'''
         oa_sess = OAuth2Session(client_id, scope=ToDoConnection._scope, redirect_uri=ToDoConnection._redirect)
         token_url = f'{ToDoConnection._authority}{ToDoConnection._token_endpoint}'
         token = oa_sess.fetch_token(token_url, client_secret=client_secret, authorization_response=redirect_resp)
 
         return token
 
     def _refresh_token(self) -> None:
@@ -224,147 +288,146 @@
         if now >= expire_time:
             token_url = f'{ToDoConnection._authority}{ToDoConnection._token_endpoint}'
             oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope,
                                     token=self.token, redirect_uri=ToDoConnection._redirect)
             new_token = oa_sess.refresh_token(token_url, client_id=self.client_id, client_secret=self.client_secret)
             self.token = new_token
 
-    def get_lists(self, limit: Optional[int] = 99) -> Optional[List[TaskList]]:
-        '''Get a list of the task lists.
+    def get_lists(self, limit: Optional[int] = 99) -> List[TaskList]:
+        '''Get a list of the task lists
 
         Args:
-            limit: *optional* The limit size of the response (default is `99`)
+            limit: The limit size of the response
 
         Returns:
-            A list of the task lists.
+            A list of the task lists
 
         Raises:
-            `PymstodoError`: An error occurred accessing the API.
+            PymstodoError: An error occurred accessing the API
         '''
         self._refresh_token()
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
         resp = oa_sess.get(f'{ToDoConnection._base_api_url}lists?$top={limit}')
         if not resp.ok:
             raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
 
         contents = json.loads(resp.content.decode())['value']
         lists = [TaskList(**list_data) for list_data in contents]
 
         return lists
 
-    def create_list(self, name: str) -> Optional[TaskList]:
-        '''Create a new task list.
+    def create_list(self, name: str) -> TaskList:
+        '''Create a new task list
 
         Args:
             name: Title of the new task list
 
         Returns:
-            A created task list.
+            A created task list
 
         Raises:
-            `PymstodoError`: An error occurred accessing the API.
+            PymstodoError: An error occurred accessing the API
         '''
         self._refresh_token()
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
         resp = oa_sess.post(f'{ToDoConnection._base_api_url}lists', json={'displayName': name})
         if not resp.ok:
             raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
 
         contents = json.loads(resp.content.decode())
 
         return TaskList(**contents)
 
-    def get_list(self, list_id: str) -> Optional[TaskList]:
-        '''Read the properties of a task list.
+    def get_list(self, list_id: str) -> TaskList:
+        '''Read the properties of a task list
 
         Args:
             list_id: Unique identifier for the task list
 
         Returns:
-            A task list object.
+            A task list object
 
         Raises:
-            `PymstodoError`: An error occurred accessing the API.
+            PymstodoError: An error occurred accessing the API
         '''
         self._refresh_token()
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
         resp = oa_sess.get(f'{ToDoConnection._base_api_url}lists/{list_id}')
         if not resp.ok:
             raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
 
         contents = json.loads(resp.content.decode())
 
         return TaskList(**contents)
 
-    def update_list(self, list_id: str, **list_data: Union[str, bool]) -> Optional[TaskList]:
-        '''Update the properties of a task list.
+    def update_list(self, list_id: str, **list_data: Union[str, bool]) -> TaskList:
+        '''Update the properties of a task list
 
         Args:
             list_id: Unique identifier for the task list
             list_data: Task properties from `TaskList` object
 
         Returns:
             An updated task list.
 
         Raises:
-            `PymstodoError`: An error occurred accessing the API.'''
+            PymstodoError: An error occurred accessing the API'''
         self._refresh_token()
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
         resp = oa_sess.patch(f'{ToDoConnection._base_api_url}lists/{list_id}', json=list_data)
         if not resp.ok:
             raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
 
         contents = json.loads(resp.content.decode())
 
         return TaskList(**contents)
 
     def delete_list(self, list_id: str) -> bool:
-        '''Delete a task list.
+        '''Delete a task list
 
         Args:
             list_id: Unique identifier for the task list
 
         Returns:
-            `True`: If success.
+            `True` if success
 
         Raises:
-            `PymstodoError`: An error occurred accessing the API.'''
+            PymstodoError: An error occurred accessing the API'''
         self._refresh_token()
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
         resp = oa_sess.delete(f'{ToDoConnection._base_api_url}lists/{list_id}')
         if not resp.ok:
             raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
 
         return True
 
-    def get_tasks(self, list_id: str, limit: Optional[int] = 0, status: Optional[Literal['notStarted', 'inProgress', 'completed', 'waitingOnOthers', 'deferred']] = None) -> List[Task]:
-        '''Get tasks by a specified task list.
+    def get_tasks(self, list_id: str, limit: Optional[int] = 1000, status: Optional[TaskStatusFilter] = TaskStatusFilter.NOT_COMPLETED) -> List[Task]:
+        '''Get tasks by a specified task list
 
         Args:
             list_id: Unique identifier for the task list
-            limit: *optional* The limit size of the response (default is `1000`)
-            status: *optional* The state or progress of the task. Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred` (default is `notCompleted`)
+            limit: The limit size of the response
+            status: The state or progress of the task
 
         Returns:
-            Tasks of a specified task list.
+            Tasks of a specified task list
 
         Raises:
-            `PymstodoError`: An error occurred accessing the API.
+            PymstodoError: An error occurred accessing the API
         '''
         self._refresh_token()
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
         filters = {
-            'completed': "filter=status eq 'completed'",
-            'notCompleted': "filter=status ne 'completed'",
-            'all': None
+            TaskStatusFilter.COMPLETED: "filter=status eq 'completed'",
+            TaskStatusFilter.NOT_COMPLETED: "filter=status ne 'completed'",
+            TaskStatusFilter.ALL: None
         }
         eff_limit = limit or 1000
-        default_status = 'notCompleted'
         params = (
-            filters.get(status or default_status, filters[default_status]),
+            filters.get(status or TaskStatusFilter.NOT_COMPLETED, filters[TaskStatusFilter.NOT_COMPLETED]),
             f'top={eff_limit}'
         )
         params_str = '&$'.join(filter(None, params))
         url = f"{ToDoConnection._base_api_url}lists/{list_id}/tasks?${params_str}"
         contents: List[Dict[str, Any]] = []
         while (len(contents) < eff_limit or eff_limit <= 0) and url:
             resp = oa_sess.get(url)
@@ -376,27 +439,27 @@
         if limit:
             contents = contents[:limit]
         tasks = [Task(**task_data) for task_data in contents]
 
         return tasks
 
     def create_task(self, title: str, list_id: str, due_date: Optional[datetime] = None, body_text: Optional[str] = None) -> Task:
-        '''Create a new task in a specified task list.
+        '''Create a new task in a specified task list
 
         Args:
             title: A brief description of the task
             list_id: Unique identifier for the task list
-            due_date: *optional* The date and time that the task is to be finished
-            body_text: *optional* Information about the task
+            due_date: The date and time that the task is to be finished
+            body_text: Information about the task
 
         Returns:
-            A created task.
+            A created task
 
         Raises:
-            `PymstodoError`: An error occurred accessing the API.'''
+            PymstodoError: An error occurred accessing the API'''
         self._refresh_token()
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
         task_data: Dict[str, Any] = {'title': title}
         if due_date:
             task_data['dueDateTime'] = {'dateTime': due_date.strftime('%Y-%m-%dT%H:%M:%S.0000000'), 'timeZone': 'UTC'}
         if body_text:
             task_data['body'] = {'content': body_text, 'contentType': 'text'}
@@ -405,88 +468,85 @@
             raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
 
         contents = json.loads(resp.content.decode())
 
         return Task(**contents)
 
     def get_task(self, task_id: str, list_id: str) -> Task:
-        '''Read the properties of a task.
+        '''Read the properties of a task
 
         Args:
             task_id: Unique identifier for the task
             list_id: Unique identifier for the task list
 
         Returns:
-            A task object.
+            A task object
 
         Raises:
-            `PymstodoError`: An error occurred accessing the API.'''
+            PymstodoError: An error occurred accessing the API'''
         self._refresh_token()
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
         resp = oa_sess.get(f'{ToDoConnection._base_api_url}lists/{list_id}/tasks/{task_id}')
         if not resp.ok:
             raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
 
         contents = json.loads(resp.content.decode())
 
         return Task(**contents)
 
     def update_task(self, task_id: str, list_id: str, **task_data: Union[str, int, bool]) -> Task:
-        '''Update the properties of a task.
+        '''Update the properties of a task
 
         Args:
             task_id: Unique identifier for the task
             list_id: Unique identifier for the task list
             task_data: Task properties from `Task` object
 
         Returns:
-            An updated task.
+            An updated task
 
         Raises:
-            `PymstodoError`: An error occurred accessing the API.'''
+            PymstodoError: An error occurred accessing the API'''
         self._refresh_token()
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
         resp = oa_sess.patch(f'{ToDoConnection._base_api_url}lists/{list_id}/tasks/{task_id}', json=task_data)
         if not resp.ok:
             raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
 
         contents = json.loads(resp.content.decode())
 
         return Task(**contents)
 
     def delete_task(self, task_id: str, list_id: str) -> bool:
-        '''Delete a task.
+        '''Delete a task
 
         Args:
             task_id: Unique identifier for the task
             list_id: Unique identifier for the task list
 
         Returns:
-            `True`: If success.
+            `True` if success
 
         Raises:
-            `PymstodoError`: An error occurred accessing the API.'''
+            PymstodoError: An error occurred accessing the API'''
         self._refresh_token()
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
         resp = oa_sess.delete(f'{ToDoConnection._base_api_url}lists/{list_id}/tasks/{task_id}')
         if not resp.ok:
             raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
 
         return True
 
     def complete_task(self, task_id: str, list_id: str) -> Task:
-        '''Complete a task.
+        '''Complete a task
 
         Args:
             task_id: Unique identifier for the task
             list_id: Unique identifier for the task list
 
         Returns:
-            A completed task.
+            A completed task
 
         Raises:
-            `PymstodoError`: An error occurred accessing the API.'''
+            PymstodoError: An error occurred accessing the API'''
         return self.update_task(task_id, list_id, status='completed')
 
-
-#os.environ['OAUTHLIB_RELAX_TOKEN_SCOPE'] = '1'
-#os.environ['OAUTHLIB_IGNORE_SCOPE_CHANGE'] = '1'
```

### Comparing `pymstodo-0.1.2/pymstodo.egg-info/PKG-INFO` & `pymstodo-0.1.3/pymstodo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymstodo
-Version: 0.1.2
+Version: 0.1.3
 Summary: Microsoft To Do API client
 Home-page: https://github.com/inbalboa/pymstodo
 Author: Sergey Shlyapugin
 Author-email: shlyapugin@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pymstodo-0.1.2/setup.py` & `pymstodo-0.1.3/setup.py`

 * *Files identical despite different names*

