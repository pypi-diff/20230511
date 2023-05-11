# Comparing `tmp/patas-2.0.1.tar.gz` & `tmp/patas-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patas-2.0.1.tar", last modified: Wed May 10 18:55:40 2023, max compression
+gzip compressed data, was "patas-2.0.2.tar", last modified: Thu May 11 19:53:36 2023, max compression
```

## Comparing `patas-2.0.1.tar` & `patas-2.0.2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-10 18:55:40.174132 patas-2.0.1/
--rw-rw-r--   0 diego     (1000) diego     (1000)     9848 2023-05-10 18:55:40.174132 patas-2.0.1/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     9415 2023-05-10 18:53:22.000000 patas-2.0.1/README.md
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-10 18:55:40.170132 patas-2.0.1/patas/
--rw-rw-r--   0 diego     (1000) diego     (1000)       19 2023-05-08 20:38:56.000000 patas-2.0.1/patas/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      220 2023-05-10 15:41:35.000000 patas-2.0.1/patas/consts.py
--rw-rw-r--   0 diego     (1000) diego     (1000)    26087 2023-05-09 18:27:28.000000 patas-2.0.1/patas/grid_exec.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      330 2023-05-06 20:57:54.000000 patas-2.0.1/patas/log.py
--rwxrwxr-x   0 diego     (1000) diego     (1000)    15390 2023-05-10 15:42:56.000000 patas-2.0.1/patas/main.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     7619 2023-05-10 14:10:51.000000 patas-2.0.1/patas/parse.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1005 2023-05-10 15:45:41.000000 patas-2.0.1/patas/query_engine.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     6051 2023-05-08 20:43:58.000000 patas-2.0.1/patas/schemas.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     9283 2023-05-10 13:33:56.000000 patas-2.0.1/patas/utils.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-10 18:55:40.170132 patas-2.0.1/patas.egg-info/
--rw-rw-r--   0 diego     (1000) diego     (1000)     9848 2023-05-10 18:55:40.000000 patas-2.0.1/patas.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      383 2023-05-10 18:55:40.000000 patas-2.0.1/patas.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2023-05-10 18:55:40.000000 patas-2.0.1/patas.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       42 2023-05-10 18:55:40.000000 patas-2.0.1/patas.egg-info/entry_points.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       20 2023-05-10 18:55:40.000000 patas-2.0.1/patas.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       12 2023-05-10 18:55:40.000000 patas-2.0.1/patas.egg-info/top_level.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2023-05-10 18:55:40.174132 patas-2.0.1/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      845 2023-05-10 15:28:55.000000 patas-2.0.1/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-10 18:55:40.174132 patas-2.0.1/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)       18 2023-05-07 16:31:37.000000 patas-2.0.1/tests/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1420 2023-05-07 16:54:01.000000 patas-2.0.1/tests/test_schemas.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-11 19:53:36.976567 patas-2.0.2/
+-rw-rw-r--   0 diego     (1000) diego     (1000)    12412 2023-05-11 19:53:36.976567 patas-2.0.2/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)    11979 2023-05-11 18:21:37.000000 patas-2.0.2/README.md
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-11 19:53:36.976567 patas-2.0.2/patas/
+-rw-rw-r--   0 diego     (1000) diego     (1000)       19 2023-05-08 20:38:56.000000 patas-2.0.2/patas/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)    14584 2023-05-11 18:12:53.000000 patas-2.0.2/patas/argparsers.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      220 2023-05-11 16:37:09.000000 patas-2.0.2/patas/consts.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     5363 2023-05-11 18:09:55.000000 patas-2.0.2/patas/graphics.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)    26220 2023-05-11 14:18:45.000000 patas-2.0.2/patas/grid_explorer.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      330 2023-05-06 20:57:54.000000 patas-2.0.2/patas/log.py
+-rwxrwxr-x   0 diego     (1000) diego     (1000)     8198 2023-05-11 18:10:38.000000 patas-2.0.2/patas/main.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     7619 2023-05-10 14:10:51.000000 patas-2.0.2/patas/parse.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1005 2023-05-10 15:45:41.000000 patas-2.0.2/patas/query_engine.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     6292 2023-05-11 16:46:00.000000 patas-2.0.2/patas/schemas.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     9283 2023-05-10 13:33:56.000000 patas-2.0.2/patas/utils.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-11 19:53:36.976567 patas-2.0.2/patas.egg-info/
+-rw-rw-r--   0 diego     (1000) diego     (1000)    12412 2023-05-11 19:53:36.000000 patas-2.0.2/patas.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      425 2023-05-11 19:53:36.000000 patas-2.0.2/patas.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2023-05-11 19:53:36.000000 patas-2.0.2/patas.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       42 2023-05-11 19:53:36.000000 patas-2.0.2/patas.egg-info/entry_points.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       26 2023-05-11 19:53:36.000000 patas-2.0.2/patas.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       12 2023-05-11 19:53:36.000000 patas-2.0.2/patas.egg-info/top_level.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2023-05-11 19:53:36.976567 patas-2.0.2/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      852 2023-05-10 22:45:33.000000 patas-2.0.2/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-11 19:53:36.976567 patas-2.0.2/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)       18 2023-05-07 16:31:37.000000 patas-2.0.2/tests/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1420 2023-05-07 16:54:01.000000 patas-2.0.2/tests/test_schemas.py
```

### Comparing `patas-2.0.1/patas/grid_exec.py` & `patas-2.0.2/patas/grid_explorer.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 
 
 KEY_SSH_ON  = b'74ffc7c4-a6ad-4315-94cb-59d045a230c0'
 KEY_SSH_OFF = b'93dfc971-fa64-4beb-a24e-d8874738b9ca'
 KEY_CMD_ON  = b'15e6896c-3ea7-42a0-aa32-23e2ab3c0e12'
 KEY_CMD_OFF = b'e04a4348-8092-46a6-8e0c-d30d10c86fb3'
 
-echo = lambda x: b" echo -e \"%s\"" % x.replace(b"-", b"-\b-")
+build_echo_cmd = lambda x: b" echo -e \"%s\"" % x.replace(b"-", b"-\b-")
 
-ECHO_SSH_ON  = echo(KEY_SSH_ON)
-ECHO_SSH_OFF = echo(KEY_SSH_OFF)
-ECHO_CMD_ON  = echo(KEY_CMD_ON)
+ECHO_SSH_ON  = build_echo_cmd(KEY_SSH_ON)
+ECHO_SSH_OFF = build_echo_cmd(KEY_SSH_OFF)
+ECHO_CMD_ON  = build_echo_cmd(KEY_CMD_ON)
 ECHO_CMD_OFF = b" echo -en \"\n $? %s\"" % KEY_CMD_OFF.replace(b"-", b"-\b-")
 
 
 def combine_variables(variables, combination={}):
 
     if len(variables) == len(combination):
         yield copy.copy(combination)
@@ -44,15 +44,15 @@
             
             for tmp in combine_variables(variables, combination):
                 yield tmp
             
         del combination[name]
 
 
-class QueueMsg(dict):
+class WorkerMessage(dict):
 
     def __init__(self, action, source=-1):
         self.action = action
         self.source = source
         self.data = {}
     
     def __setstate__(self, state):
@@ -72,55 +72,57 @@
 
     def __init__(self, 
             experiment_name, task_output_dir, work_dir, experiment_idd, combination_idd, 
             repeat_idd, task_idd, combination, cmdlines, max_tries):
 
         self.experiment_name = experiment_name
         self.combination_idd = combination_idd
-        self.experiment_idd = experiment_idd
-        self.output_dir = task_output_dir
-        self.combination = combination
-        self.repeat_idd = repeat_idd
-        self.max_tries = max_tries
-        self.work_dir = work_dir
-        self.task_idd = task_idd
-        self.commands = cmdlines
-        self.assigned_to = None
-        self.started_at = None
-        self.ended_at = None
-        self.duration = None
-        self.success = None
-        self.output = None
-        self.status = None
-        self.tries = 0
+        self.experiment_idd  = experiment_idd
+        self.output_dir      = task_output_dir
+        self.combination     = combination
+        self.repeat_idd      = repeat_idd
+        self.max_tries       = max_tries
+        self.work_dir        = work_dir
+        self.task_idd        = task_idd
+        self.commands        = cmdlines
+        self.assigned_to     = None
+        self.started_at      = None
+        self.ended_at        = None
+        self.duration        = None
+        self.success         = None
+        self.output          = None
+        self.status          = None
+        self.tries           = 0
     
     
     def __repr__(self):
-        comb = ";".join(f"{k}={v}" for k, v in self.combination.items())
-        return "%d %d %d %d %s %s" % (self.experiment_idd, self.combination_idd, 
-                    self.repeat_idd, self.task_idd, comb, self.commands)
+
+        combination = ";".join(f"{k}={v}" for k, v in self.combination.items())
+        return f"{self.experiment_idd} {self.combination_idd} {self.repeat_idd} {self.task_idd} {combination} {self.commands}"
 
 
 class ExecutorBuilder:
 
     def __init__(self, executor_type, node):
         self.executor_type = executor_type
         self.node = node
 
+
     def __call__(self):
         return self.executor_type(self.node)
 
 
 class BashExecutor:
     
     def __init__(self, node):
 
         self.is_alive = True
         self.node = node
     
+
     def execute(self, initrc, cmds):
 
         if type(cmds) is not list:
             cmds = [cmds]
 
         cmds = [x + b' 2>&1 ' for x in cmds]
 
@@ -149,14 +151,15 @@
         self.master, self.slave = pty.openpty()
         self._start_bash()
         
         self.conn_string = self._build_connnection_string(self.node)
 
         self._connect()
     
+
     def _build_connnection_string(self, node):
 
         tokens = [b' ssh']
 
         if node.private_key:
             tokens.append(b' -i ')
             tokens.append(node.private_key.encode())
@@ -302,49 +305,45 @@
     def start(self, queue_master):
 
         self.queue = Queue()
         self.process = Process(target=self.run, args=(self.queue, queue_master))
         self.process.start()
 
 
-    # def debug(self, *args):
-    #     debug(self.worker_idd, "|", *args)
-
-
     def run(self, queue_in, queue_master):
 
         try:
             executor = self.executor_builder()
 
-            msg_out = QueueMsg("ready", self.worker_idd)
+            msg_out = WorkerMessage("ready", self.worker_idd)
             queue_master.put(msg_out)
             
             while True:
                 msg_in = queue_in.get()
 
                 if msg_in.action == "execute":
                     success = self.execute(msg_in, executor)
 
-                    msg_out = QueueMsg("finished", self.worker_idd)
+                    msg_out = WorkerMessage("finished", self.worker_idd)
                     msg_out.success = success
                     queue_master.put(msg_out)
 
                     if not executor.is_alive:
                         executor = self.executor_builder()
 
-                    msg_out = QueueMsg("ready", self.worker_idd)
+                    msg_out = WorkerMessage("ready", self.worker_idd)
                     queue_master.put(msg_out)
                 
                 elif msg_in.action == "terminate":
                     break
                 
                 else:
                     warn("Unknown action:", msg_in.action)
             
-            msg_out = QueueMsg("ended", self.worker_idd)
+            msg_out = WorkerMessage("ended", self.worker_idd)
             queue_master.put(msg_out)
         except KeyboardInterrupt:
             pass
 
 
     def execute(self, msg_in, executor):
 
@@ -423,30 +422,31 @@
             for line in task.output:
                 os.write(sys.stdout.fileno(), line)
             warn("--- END OF FAILED OUTPUT ---")
 
         return task.success
 
 
-class GridExec():
+class GridExplorer():
 
     def __init__(self, task_filters, node_filters, 
             output_dir, redo_tasks, recreate, confirmed,
             experiments, clusters):
 
-        self.output_folder = expand_path(output_dir)
-        self.task_filters = task_filters
-        self.node_filters = node_filters
-        self.experiments = experiments
-        self.redo_tasks = redo_tasks
-        self.confirmed = confirmed
-        self.recreate = recreate
-        self.clusters = clusters
+        self.output_folder = expand_path  (output_dir)
+        self.task_filters  = task_filters
+        self.node_filters  = node_filters
+        self.experiments   = experiments
+        self.redo_tasks    = redo_tasks
+        self.confirmed     = confirmed
+        self.recreate      = recreate
+        self.clusters      = clusters
+
         self.workers:list[WorkerProcess] = None
-        self.tasks:list[Task] = None
+        self.tasks  :list[Task         ] = None
 
 
     def start(self):
 
         os.makedirs(self.output_folder, exist_ok=True)
 
         self._show_summary(self.experiments, self.clusters, self.confirmed)
@@ -458,16 +458,16 @@
 
     def _show_summary(self, experiments, clusters, confirmed):
 
         # Display experiments
 
         print(colors.white("\n --- Experiments --- \n"))
 
+        experiment: Experiment = None
         total_tasks = 0
-        experiment: Experiment
 
         for experiment in experiments:
             variables = experiment.vars
             current = 1
 
             for var in variables:
                 current *= len(var.values)
@@ -766,15 +766,15 @@
         try:
             print()
             info("Releasing workers...")
 
             # Sending TERMINATE signal
 
             for worker in self.workers:
-                msg = QueueMsg("terminate")
+                msg = WorkerMessage("terminate")
                 worker.queue.put(msg)
             
             # Waiting for ENDED signal
 
             while len(self.workers) != len(self.ended):
 
                 msg = self.queue.get()
@@ -816,15 +816,15 @@
         print(f"    Tasks completed: {len(self.done)}")
         print(f"    Tasks given up: {len(self.given_up)}")
         print()
 
     def _ready(self, msg_in):
 
         if self.todo:
-            msg_out = QueueMsg("execute")
+            msg_out = WorkerMessage("execute")
             msg_out.task = self.todo.pop()
             msg_out.task.assigned_to = msg_in.source
 
             self.doing.append(msg_out.task)
             self.workers[msg_in.source].queue.put(msg_out)
         
         else:
@@ -856,12 +856,12 @@
         
         if not self.idle:
             self.todo.append(task)
             return
 
         target = self.idle.pop()
 
-        msg_out = QueueMsg("execute")
+        msg_out = WorkerMessage("execute")
         msg_out.task = task
         msg_out.task.assigned_to = target
 
         self.workers[target].queue.put(msg_out)
```

### Comparing `patas-2.0.1/patas/parse.py` & `patas-2.0.2/patas/parse.py`

 * *Files identical despite different names*

### Comparing `patas-2.0.1/patas/query_engine.py` & `patas-2.0.2/patas/query_engine.py`

 * *Files identical despite different names*

### Comparing `patas-2.0.1/patas/schemas.py` & `patas-2.0.2/patas/schemas.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     def load_property(self, name, data, mandatory=False):
         
         if name in data:
             setattr(self, name, data[name])
         
         elif mandatory:
-            error("Missing mandatory property in Node schema: " + name)
+            error(f"Missing required property in {self.__class__.__name__}: {name}")
 
 
 class Node(Schema):
 
     def __init__(self, data=None):
         
         self.tags = []
@@ -119,33 +119,43 @@
 
 class ArithmeticVariable(Schema):
     
     def __init__(self, data=None):
 
         self.type = 'arithmetic'
         self.name = None
-        self.factor = 1
-        self.min = 0
-        self.max = 10
+        self.step = 1
+        self.min  = 0
+        self.max  = 10
 
         if data is not None:
             self.init_from(data)
 
         self.update()
     
     def update(self):
-        self._values = self.arange(self.first, self.last, self.step)
+        self._values = self.arange(self.min, self.max, self.step)
     
+    def arange(self, first, last, step):
+        current = first
+        res = []
+
+        while current <= last:
+            res.append(current)
+            current += step
+        
+        return res
+
     @property
     def values(self):
         return self._values
     
     def init_from(self, data):
 
-        self.load_property('factor', data)
+        self.load_property('step', data)
         self.load_property('name', data)
         self.load_property('min', data)
         self.load_property('max', data)
 
         return self
 
 
@@ -161,14 +171,15 @@
 
         if data is not None:
             self.init_from(data)
     
         self.update()
     
     def update(self):
+        
         self._values = list()
         current = self.first
         
         while current < self.last:
             self._values.append(current)
             current = current * self.factor
     
@@ -185,14 +196,15 @@
 
         return self
 
 
 class Experiment(Schema):
 
     def __init__(self):
+
         self.cmd = []
         self.name = None
         self.workdir = None
         self.repeat = 1
         self.max_tries = 3
         self.vars = []
     
@@ -219,17 +231,17 @@
                     elif data2['type'] == 'arithmetic':
                         self.vars.append(ArithmeticVariable(data2))
 
                     elif data2['type'] == 'geometric':
                         self.vars.append(GeometricVariable(data2))
 
                     else:
-                        error(f"Invalid property value in Variable Schema: type={data2['type']}")
+                        error(f"Invalid property value in {self.__class__.__name__}: type={data2['type']}")
                 else:
-                    error('Missing mandatory property in Variable Schema: type')
+                    error(f'Missing required property in {self.__class__.__name__}: type')
 
         return self
 
 
 def load_cluster(filepath):
     with open(filepath, "r") as fin:
         data = yaml.load(fin, Loader=yaml.FullLoader)
```

### Comparing `patas-2.0.1/patas/utils.py` & `patas-2.0.2/patas/utils.py`

 * *Files identical despite different names*

### Comparing `patas-2.0.1/setup.py` & `patas-2.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 import patas.consts as c
 import setuptools
 
 
 long_description_content_type = "text/markdown"
+
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name=c.name,
     version=c.version,
@@ -25,14 +26,14 @@
     ],
     entry_points = {
         'console_scripts': [
             'patas = patas.main:main'
         ],
     },
     install_requires=[
-        'tqdm', 'csvkit'
+        'csvkit', 'matplotlib'
     ],
     extras_require={
         "full": []
     }
 )
```

### Comparing `patas-2.0.1/tests/test_schemas.py` & `patas-2.0.2/tests/test_schemas.py`

 * *Files identical despite different names*

