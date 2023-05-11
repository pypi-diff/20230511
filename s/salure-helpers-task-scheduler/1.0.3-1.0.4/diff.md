# Comparing `tmp/salure_helpers_task_scheduler-1.0.3.tar.gz` & `tmp/salure_helpers_task_scheduler-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_task_scheduler-1.0.3.tar", last modified: Thu Dec 22 15:15:21 2022, max compression
+gzip compressed data, was "dist/salure_helpers_task_scheduler-1.0.4.tar", last modified: Thu May 11 09:09:10 2023, max compression
```

## Comparing `salure_helpers_task_scheduler-1.0.3.tar` & `salure_helpers_task_scheduler-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-22 15:15:21.000000 salure_helpers_task_scheduler-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      269 2022-12-22 15:15:21.000000 salure_helpers_task_scheduler-1.0.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-22 15:15:21.000000 salure_helpers_task_scheduler-1.0.3/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-22 15:15:21.000000 salure_helpers_task_scheduler-1.0.3/salure_helpers/task_scheduler/
--rw-rw-rw-   0 root         (0) root         (0)       70 2022-12-22 15:15:07.000000 salure_helpers_task_scheduler-1.0.3/salure_helpers/task_scheduler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    39135 2022-12-22 15:15:07.000000 salure_helpers_task_scheduler-1.0.3/salure_helpers/task_scheduler/task_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-22 15:15:21.000000 salure_helpers_task_scheduler-1.0.3/salure_helpers_task_scheduler.egg-info/
--rw-r--r--   0 root         (0) root         (0)      269 2022-12-22 15:15:21.000000 salure_helpers_task_scheduler-1.0.3/salure_helpers_task_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      414 2022-12-22 15:15:21.000000 salure_helpers_task_scheduler-1.0.3/salure_helpers_task_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-22 15:15:21.000000 salure_helpers_task_scheduler-1.0.3/salure_helpers_task_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-22 15:15:21.000000 salure_helpers_task_scheduler-1.0.3/salure_helpers_task_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      151 2022-12-22 15:15:21.000000 salure_helpers_task_scheduler-1.0.3/salure_helpers_task_scheduler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-12-22 15:15:21.000000 salure_helpers_task_scheduler-1.0.3/salure_helpers_task_scheduler.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-22 15:15:21.000000 salure_helpers_task_scheduler-1.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      614 2022-12-22 15:15:07.000000 salure_helpers_task_scheduler-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers/task_scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-11 09:08:57.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers/task_scheduler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    38959 2023-05-11 09:08:57.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers/task_scheduler/task_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers_task_scheduler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers_task_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      414 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers_task_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers_task_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers_task_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      151 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers_task_scheduler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers_task_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-05-11 09:08:57.000000 salure_helpers_task_scheduler-1.0.4/setup.py
```

### Comparing `salure_helpers_task_scheduler-1.0.3/salure_helpers/task_scheduler/task_scheduler.py` & `salure_helpers_task_scheduler-1.0.4/salure_helpers/task_scheduler/task_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,16 +421,14 @@
             email_to = email_variable.split(',')
             if isinstance(email_to, list):
                 # The email_errors_to variable is a simple string. Convert it to a list and add a name because mandrill is asking for it
                 email_list = []
                 for i in email_to:
                     email_list.append({'name': 'SalureConnect User', 'mail': i.strip()})
                 # Set the content of the mail and all other stuff
-                email_from = 'connect@salure.nl'
-                name_from = 'SalureConnect'
                 task = self.mysql.select(table='task_scheduler', selection='title', filter=f'WHERE id = {self.task_id}')[0][
                     0]
                 finished_at = \
                     self.mysql.select(table='task_scheduler', selection='last_reload', filter=f'WHERE id = {self.task_id}')[0][
                         0]
                 if failed:
                     subject = f'Task \'{task}\' has failed'
@@ -438,9 +436,8 @@
                               f'The task is failed. ' \
                               f'to visit the SalureConnect scheduler, click here: <a href="https://salureconnect.com/connectors/task-scheduler/">here</a>. Here you can find the logs and find more information on why this task had failed.'
                 else:
                     subject = f'Task \'{task}\' is finished with errors'
                     content = f'Task \'{task}\' with ID \'{self.task_id}\' has runned and is finished at {finished_at}. ' \
                               f'The task is finished with {self.error_count} errors. ' \
                               f'to visit the SalureConnect scheduler, click here: <a href="https://salureconnect.com/connectors/task-scheduler/">here</a>. Here you can find the logs and find more information on why this task had some errors.'
-                MailClient().send_mail(email_to=email_list, email_from=email_from,
-                                       name_from=name_from, subject=subject, content=content, language='EN')
+                MailClient().send_mail(email_to=email_list, subject=subject, content=content, language='EN')
```

### Comparing `salure_helpers_task_scheduler-1.0.3/setup.py` & `salure_helpers_task_scheduler-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='salure_helpers_task_scheduler',
-    version='1.0.3',
+    version='1.0.4',
     description='Task Scheduler from Salure',
     long_description='Task Schedule from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.task_scheduler"],
     license='Salure License',
     install_requires=[
```

