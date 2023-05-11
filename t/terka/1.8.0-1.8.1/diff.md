# Comparing `tmp/terka-1.8.0.tar.gz` & `tmp/terka-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.8.0.tar", last modified: Wed May 10 19:38:21 2023, max compression
+gzip compressed data, was "terka-1.8.1.tar", last modified: Wed May 10 21:16:35 2023, max compression
```

## Comparing `terka-1.8.0.tar` & `terka-1.8.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 19:38:21.957159 terka-1.8.0/
--rw-r--r--   0 am        (1000) am        (1000)      292 2023-05-10 19:38:21.957159 terka-1.8.0/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-05-10 19:38:21.957159 terka-1.8.0/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      903 2023-05-10 19:37:49.000000 terka-1.8.0/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 19:38:21.953159 terka-1.8.0/terka/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.0/terka/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 19:38:21.953159 terka-1.8.0/terka/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.0/terka/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    16361 2023-04-26 19:48:32.000000 terka-1.8.0/terka/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-26 19:47:22.000000 terka-1.8.0/terka/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 19:38:21.953159 terka-1.8.0/terka/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    44829 2023-05-10 19:36:37.000000 terka-1.8.0/terka/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)     1513 2023-05-01 11:31:58.000000 terka-1.8.0/terka/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/event_history.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 19:38:21.953159 terka-1.8.0/terka/domain/external_connectors/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/external_connectors/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      265 2023-04-26 19:49:46.000000 terka-1.8.0/terka/domain/external_connectors/asana.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.8.0/terka/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     2244 2023-05-03 16:06:42.000000 terka-1.8.0/terka/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)     1495 2023-05-01 11:32:09.000000 terka-1.8.0/terka/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2082 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 19:38:21.953159 terka-1.8.0/terka/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.0/terka/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     6055 2023-04-30 19:45:41.000000 terka-1.8.0/terka/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 19:38:21.953159 terka-1.8.0/terka/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.0/terka/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    31416 2023-05-10 19:34:32.000000 terka-1.8.0/terka/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-26 19:47:22.000000 terka-1.8.0/terka/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-04-26 19:47:22.000000 terka-1.8.0/terka/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-04-26 19:47:22.000000 terka-1.8.0/terka/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     2382 2023-04-30 10:27:47.000000 terka-1.8.0/terka/service_layer/views.py
--rw-r--r--   0 am        (1000) am        (1000)     7907 2023-05-10 15:50:27.000000 terka-1.8.0/terka/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 19:38:21.953159 terka-1.8.0/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)      292 2023-05-10 19:38:21.000000 terka-1.8.0/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      993 2023-05-10 19:38:21.000000 terka-1.8.0/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-05-10 19:38:21.000000 terka-1.8.0/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       53 2023-05-10 19:38:21.000000 terka-1.8.0/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       52 2023-05-10 19:38:21.000000 terka-1.8.0/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)        6 2023-05-10 19:38:21.000000 terka-1.8.0/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 21:16:35.320383 terka-1.8.1/
+-rw-r--r--   0 am        (1000) am        (1000)      292 2023-05-10 21:16:35.320383 terka-1.8.1/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-05-10 21:16:35.320383 terka-1.8.1/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      903 2023-05-10 21:16:27.000000 terka-1.8.1/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 21:16:35.316383 terka-1.8.1/terka/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.1/terka/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 21:16:35.316383 terka-1.8.1/terka/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.1/terka/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    16361 2023-04-26 19:48:32.000000 terka-1.8.1/terka/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-26 19:47:22.000000 terka-1.8.1/terka/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 21:16:35.316383 terka-1.8.1/terka/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.1/terka/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-26 19:47:22.000000 terka-1.8.1/terka/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    44868 2023-05-10 19:44:06.000000 terka-1.8.1/terka/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-26 19:47:22.000000 terka-1.8.1/terka/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-04-26 19:47:22.000000 terka-1.8.1/terka/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)     1513 2023-05-01 11:31:58.000000 terka-1.8.1/terka/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-04-26 19:47:22.000000 terka-1.8.1/terka/domain/event_history.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 21:16:35.316383 terka-1.8.1/terka/domain/external_connectors/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.1/terka/domain/external_connectors/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      265 2023-04-26 19:49:46.000000 terka-1.8.1/terka/domain/external_connectors/asana.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.8.1/terka/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-04-26 19:47:22.000000 terka-1.8.1/terka/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     2244 2023-05-03 16:06:42.000000 terka-1.8.1/terka/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)     1495 2023-05-01 11:32:09.000000 terka-1.8.1/terka/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-26 19:47:22.000000 terka-1.8.1/terka/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2082 2023-04-26 19:47:22.000000 terka-1.8.1/terka/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-26 19:47:22.000000 terka-1.8.1/terka/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-26 19:47:22.000000 terka-1.8.1/terka/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 21:16:35.316383 terka-1.8.1/terka/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.1/terka/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     6055 2023-04-30 19:45:41.000000 terka-1.8.1/terka/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 21:16:35.320383 terka-1.8.1/terka/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.1/terka/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    31455 2023-05-10 19:47:59.000000 terka-1.8.1/terka/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-26 19:47:22.000000 terka-1.8.1/terka/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-04-26 19:47:22.000000 terka-1.8.1/terka/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-04-26 19:47:22.000000 terka-1.8.1/terka/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     2382 2023-04-30 10:27:47.000000 terka-1.8.1/terka/service_layer/views.py
+-rw-r--r--   0 am        (1000) am        (1000)     7907 2023-05-10 15:50:27.000000 terka-1.8.1/terka/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 21:16:35.316383 terka-1.8.1/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)      292 2023-05-10 21:16:35.000000 terka-1.8.1/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      993 2023-05-10 21:16:35.000000 terka-1.8.1/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-05-10 21:16:35.000000 terka-1.8.1/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       53 2023-05-10 21:16:35.000000 terka-1.8.1/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       52 2023-05-10 21:16:35.000000 terka-1.8.1/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)        6 2023-05-10 21:16:35.000000 terka-1.8.1/terka.egg-info/top_level.txt
```

### Comparing `terka-1.8.0/setup.py` & `terka-1.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 # README = (HERE.parent / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.8.0",
+    version="1.8.1",
     description="CLI utility for creating and managing tasks in a terminal",
     # long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
```

### Comparing `terka-1.8.0/terka/adapters/orm.py` & `terka-1.8.1/terka/adapters/orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.0/terka/adapters/repository.py` & `terka-1.8.1/terka/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.0/terka/domain/collaborators.py` & `terka-1.8.1/terka/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.0/terka/domain/commands.py` & `terka-1.8.1/terka/domain/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -969,15 +969,17 @@
         if self.repo.list(SprintTask, {"task": task.id, "sprint": sprint.id}):
             exit("task already added to sprint")
         if sprint.status.name == "ACTIVE":
 
             story_points = input(
                 f"Please enter story points estimation for task <{task.id}>: {task.name}: "
             )
-            if not story_points.isnumeric():
+            try:
+                float(story_points)
+            except ValueError:
                 self.console.print(
                     "[red]Provide number when specifying story points[/red]")
                 exit()
         else:
             story_points = 0
         obj = SprintTask(task=task.id,
                          story_points=story_points,
```

### Comparing `terka-1.8.0/terka/domain/commentary.py` & `terka-1.8.1/terka/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.0/terka/domain/epic.py` & `terka-1.8.1/terka/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.0/terka/domain/event_history.py` & `terka-1.8.1/terka/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.0/terka/domain/project.py` & `terka-1.8.1/terka/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.0/terka/domain/sprint.py` & `terka-1.8.1/terka/domain/sprint.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.0/terka/domain/story.py` & `terka-1.8.1/terka/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.0/terka/domain/tag.py` & `terka-1.8.1/terka/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.0/terka/domain/task.py` & `terka-1.8.1/terka/domain/task.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.0/terka/domain/time_tracker.py` & `terka-1.8.1/terka/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.0/terka/entrypoints/cli.py` & `terka-1.8.1/terka/entrypoints/cli.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.0/terka/service_layer/printer.py` & `terka-1.8.1/terka/service_layer/printer.py`

 * *Files 0% similar despite different names*

```diff
@@ -562,20 +562,21 @@
                     custom_sort=None):
         if all_tasks:
             completed_tasks = []
         else:
             completed_tasks = None
             completed_story_points = None
         if not custom_sort:
-            custom_sort = "status"
+            custom_sort = "status.value"
         if story_points:
             completed_story_points = []
+            sorting = attrgetter(custom_sort)
             entities = [(entity, story_point) for entity, story_point in
                         sorted(zip(entities, story_points),
-                               key=lambda x: getattr(x[0], custom_sort),
+                               key=lambda x: sorting(x[0]),
                                reverse=True)]
         else:
             completed_story_points = None
         for column in default_columns:
             table.add_column(column)
         for entity in entities:
             if story_points:
```

### Comparing `terka-1.8.0/terka/service_layer/services.py` & `terka-1.8.1/terka/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.0/terka/service_layer/ui.py` & `terka-1.8.1/terka/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.0/terka/service_layer/vertical_layout.css` & `terka-1.8.1/terka/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.8.0/terka/service_layer/views.py` & `terka-1.8.1/terka/service_layer/views.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.0/terka/utils.py` & `terka-1.8.1/terka/utils.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.0/terka.egg-info/SOURCES.txt` & `terka-1.8.1/terka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

