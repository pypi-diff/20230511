# Comparing `tmp/sca_rhythm-0.4.0.tar.gz` & `tmp/sca_rhythm-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sca_rhythm-0.4.0.tar", max compression
+gzip compressed data, was "sca_rhythm-0.4.1.tar", max compression
```

## Comparing `sca_rhythm-0.4.0.tar` & `sca_rhythm-0.4.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.4.0/LICENSE.md
--rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.4.0/README.md
--rw-r--r--   0        0        0      357 2023-05-09 20:58:35.398293 sca_rhythm-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    15362 2023-05-09 20:58:20.237999 sca_rhythm-0.4.0/sca_rhythm/__init__.py
--rw-r--r--   0        0        0     2904 1970-01-01 00:00:00.000000 sca_rhythm-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.4.1/LICENSE.md
+-rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.4.1/README.md
+-rw-r--r--   0        0        0      375 2023-05-11 04:33:11.313461 sca_rhythm-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    15285 2023-05-11 04:15:42.637455 sca_rhythm-0.4.1/sca_rhythm/__init__.py
+-rw-r--r--   0        0        0     4590 2023-05-10 19:37:32.717746 sca_rhythm-0.4.1/sca_rhythm/progress.py
+-rw-r--r--   0        0        0     2943 1970-01-01 00:00:00.000000 sca_rhythm-0.4.1/PKG-INFO
```

### Comparing `sca_rhythm-0.4.0/LICENSE.md` & `sca_rhythm-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.0/README.md` & `sca_rhythm-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.0/sca_rhythm/__init__.py` & `sca_rhythm-0.4.1/sca_rhythm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         step = self.get_step(step_name)
         step['task_runs'] = step.get('task_runs', [])
         step['task_runs'].append({
             'date_start': datetime.datetime.utcnow(),
             'task_id': task_id
         })
         self.update()
-        print(f'starting {step_name} with task id: {task_id}')
+        # print(f'starting {step_name} with task id: {task_id}')
 
     def on_step_success(self, retval: tuple, step_name: str) -> None:
         """
         Called by an instance of WorkflowTask before after it completes work.
         calls the next step (if there is one) with the first element of the retval as an argument.
 
         :param retval: the return value of the task of tuple type. the first element is sent to the next step as an arg
@@ -189,15 +189,15 @@
 
             kwargs = {
                 'workflow_id': self.workflow['_id'],
                 'step': next_step['name']
             }
             # next_task.apply_async((retval[0],), kwargs)
             self.app.send_task(next_step['task'], (retval[0],), kwargs)
-            print(f'starting next step {next_step["name"]}')
+            # print(f'starting next step {next_step["name"]}')
 
     def update(self):
         """
         Update the workflow object in mongo db
         :return: None
         """
         self.workflow['updated_at'] = datetime.datetime.utcnow()
@@ -354,28 +354,28 @@
     add_to_parent = True
     trail = True
 
     def __init__(self):
         self.workflow = None
 
     def before_start(self, task_id, args, kwargs):
-        print(f'before_start, task_id:{task_id}, kwargs:{kwargs} name:{self.name}')
+        # print(f'before_start, task_id:{task_id}, kwargs:{kwargs} name:{self.name}')
         self.update_progress({})
 
         if 'workflow_id' in kwargs and 'step' in kwargs:
             workflow_id = kwargs['workflow_id']
             self.workflow = Workflow(self.app, workflow_id)
             self.workflow.on_step_start(kwargs['step'], task_id)
 
     def on_success(self, retval, task_id, args, kwargs):
-        print(f'on_success, task_id: {task_id}, kwargs: {kwargs}')
+        # print(f'on_success, task_id: {task_id}, kwargs: {kwargs}')
 
         if 'workflow_id' in kwargs and 'step' in kwargs:
             self.workflow.on_step_success(retval, kwargs['step'])
 
     def update_progress(self, progress_obj):
         # called_directly: This flag is set to true if the task was not executed by the worker.
         if not self.request.called_directly:
-            print(f'updating progress for {self.name}', progress_obj)
-            self.update_state(state='PROGRESS',
-                              meta=progress_obj
-                              )
+            self.update_state(
+                state='PROGRESS',
+                meta=progress_obj
+            )
```

### Comparing `sca_rhythm-0.4.0/PKG-INFO` & `sca_rhythm-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: sca-rhythm
-Version: 0.4.0
+Version: 0.4.1
 Summary: Create and manage workflows using Celery tasks
 Author: Deepak Duggirala
 Author-email: deepakduggi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: celery (>=5.2.7,<6.0.0)
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Rhythm
 Rhythm allows you to design and control workflows made of Celery tasks. A workflow is a sequence of steps to run one after the other. Rhythm simplifies the process of executing workflows consisting of long-running tasks with reliability.
 
 The following are the features of Rhythm workflows:
```

