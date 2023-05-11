# Comparing `tmp/scipion-em-pwperformance-0.0.4.tar.gz` & `tmp/scipion-em-pwperformance-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-pwperformance-0.0.4.tar", last modified: Fri Feb 19 15:05:37 2021, max compression
+gzip compressed data, was "scipion-em-pwperformance-0.0.5.tar", last modified: Thu May 11 12:47:01 2023, max compression
```

## Comparing `scipion-em-pwperformance-0.0.4.tar` & `scipion-em-pwperformance-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-19 15:05:37.598442 scipion-em-pwperformance-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2021-02-19 14:59:20.000000 scipion-em-pwperformance-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-02-19 14:59:20.000000 scipion-em-pwperformance-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2021-02-19 15:05:37.598442 scipion-em-pwperformance-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      702 2021-02-19 14:59:20.000000 scipion-em-pwperformance-0.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-19 15:05:37.594442 scipion-em-pwperformance-0.0.4/pwperformance/
--rw-r--r--   0 runner    (1001) docker     (121)     3920 2021-02-19 14:59:20.000000 scipion-em-pwperformance-0.0.4/pwperformance/StaticVsInstanceMethod.py
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-02-19 14:59:20.000000 scipion-em-pwperformance-0.0.4/pwperformance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      286 2021-02-19 14:59:20.000000 scipion-em-pwperformance-0.0.4/pwperformance/hassAttrVsTry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-19 15:05:37.594442 scipion-em-pwperformance-0.0.4/pwperformance/loggers/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-02-19 14:59:20.000000 scipion-em-pwperformance-0.0.4/pwperformance/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9206 2021-02-19 14:59:20.000000 scipion-em-pwperformance-0.0.4/pwperformance/loggers/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (121)     2956 2021-02-19 14:59:20.000000 scipion-em-pwperformance-0.0.4/pwperformance/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-19 15:05:37.594442 scipion-em-pwperformance-0.0.4/pwperformance/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-02-19 14:59:20.000000 scipion-em-pwperformance-0.0.4/pwperformance/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1537 2021-02-19 14:59:20.000000 scipion-em-pwperformance-0.0.4/pwperformance/tests/test_exportsteps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1402 2021-02-19 14:59:20.000000 scipion-em-pwperformance-0.0.4/pwperformance/tests/test_influxhandler.py
--rw-r--r--   0 runner    (1001) docker     (121)     2790 2021-02-19 14:59:20.000000 scipion-em-pwperformance-0.0.4/pwperformance/tests/test_profiling_load.py
--rw-r--r--   0 runner    (1001) docker     (121)     7264 2021-02-19 14:59:20.000000 scipion-em-pwperformance-0.0.4/pwperformance/tests/test_set_performance.py
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-02-19 14:59:20.000000 scipion-em-pwperformance-0.0.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-19 15:05:37.598442 scipion-em-pwperformance-0.0.4/scipion_em_pwperformance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2021-02-19 15:05:37.000000 scipion-em-pwperformance-0.0.4/scipion_em_pwperformance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      734 2021-02-19 15:05:37.000000 scipion-em-pwperformance-0.0.4/scipion_em_pwperformance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-19 15:05:37.000000 scipion-em-pwperformance-0.0.4/scipion_em_pwperformance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-02-19 15:05:37.000000 scipion-em-pwperformance-0.0.4/scipion_em_pwperformance.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-02-19 15:05:37.000000 scipion-em-pwperformance-0.0.4/scipion_em_pwperformance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-02-19 15:05:37.000000 scipion-em-pwperformance-0.0.4/scipion_em_pwperformance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-02-19 15:05:37.598442 scipion-em-pwperformance-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2454 2021-02-19 14:59:20.000000 scipion-em-pwperformance-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:47:01.423133 scipion-em-pwperformance-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-11 12:45:02.000000 scipion-em-pwperformance-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-11 12:45:02.000000 scipion-em-pwperformance-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-05-11 12:47:01.423133 scipion-em-pwperformance-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-11 12:45:02.000000 scipion-em-pwperformance-0.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:47:01.419133 scipion-em-pwperformance-0.0.5/pwperformance/
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-11 12:45:02.000000 scipion-em-pwperformance-0.0.5/pwperformance/StaticVsInstanceMethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-11 12:45:02.000000 scipion-em-pwperformance-0.0.5/pwperformance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-11 12:45:02.000000 scipion-em-pwperformance-0.0.5/pwperformance/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-11 12:45:02.000000 scipion-em-pwperformance-0.0.5/pwperformance/hassAttrVsTry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:47:01.419133 scipion-em-pwperformance-0.0.5/pwperformance/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-11 12:45:02.000000 scipion-em-pwperformance-0.0.5/pwperformance/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-05-11 12:45:02.000000 scipion-em-pwperformance-0.0.5/pwperformance/loggers/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-11 12:45:02.000000 scipion-em-pwperformance-0.0.5/pwperformance/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:47:01.423133 scipion-em-pwperformance-0.0.5/pwperformance/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:45:02.000000 scipion-em-pwperformance-0.0.5/pwperformance/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-11 12:45:02.000000 scipion-em-pwperformance-0.0.5/pwperformance/tests/test_exportsteps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-11 12:45:02.000000 scipion-em-pwperformance-0.0.5/pwperformance/tests/test_influxhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-11 12:45:02.000000 scipion-em-pwperformance-0.0.5/pwperformance/tests/test_profiling_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-05-11 12:45:02.000000 scipion-em-pwperformance-0.0.5/pwperformance/tests/test_set_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 12:45:02.000000 scipion-em-pwperformance-0.0.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:47:01.423133 scipion-em-pwperformance-0.0.5/scipion_em_pwperformance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-05-11 12:47:01.000000 scipion-em-pwperformance-0.0.5/scipion_em_pwperformance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-11 12:47:01.000000 scipion-em-pwperformance-0.0.5/scipion_em_pwperformance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 12:47:01.000000 scipion-em-pwperformance-0.0.5/scipion_em_pwperformance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 12:47:01.000000 scipion-em-pwperformance-0.0.5/scipion_em_pwperformance.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-11 12:47:01.000000 scipion-em-pwperformance-0.0.5/scipion_em_pwperformance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 12:47:01.000000 scipion-em-pwperformance-0.0.5/scipion_em_pwperformance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 12:47:01.423133 scipion-em-pwperformance-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-11 12:45:02.000000 scipion-em-pwperformance-0.0.5/setup.py
```

### Comparing `scipion-em-pwperformance-0.0.4/LICENSE` & `scipion-em-pwperformance-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-pwperformance-0.0.4/pwperformance/StaticVsInstanceMethod.py` & `scipion-em-pwperformance-0.0.5/pwperformance/StaticVsInstanceMethod.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,110 +1,112 @@
 from pwperformance.main import Timer
 
+
 class Instance(object):
 
-    def method1(cls): pass
+    def method1(self): pass
 
-    def method2(cls): pass
+    def method2(self): pass
 
-    def method3(cls): pass
+    def method3(self): pass
 
-    def method4(cls): pass
+    def method4(self): pass
 
-    def method5(cls): pass
+    def method5(self): pass
 
-    def method6(cls): pass
+    def method6(self): pass
 
-    def method7(cls): pass
+    def method7(self): pass
 
-    def method8(cls): pass
+    def method8(self): pass
 
-    def method9(cls): pass
+    def method9(self): pass
 
-    def method10(cls): pass
+    def method10(self): pass
 
-    def method11(cls): pass
+    def method11(self): pass
 
-    def method12(cls): pass
+    def method12(self): pass
 
-    def method13(cls): pass
+    def method13(self): pass
 
-    def method14(cls): pass
+    def method14(self): pass
 
-    def method15(cls): pass
+    def method15(self): pass
 
-    def method16(cls): pass
+    def method16(self): pass
 
-    def method17(cls): pass
+    def method17(self): pass
 
-    def method18(cls): pass
+    def method18(self): pass
 
-    def method19(cls): pass
+    def method19(self): pass
 
-    def method20(cls): pass
+    def method20(self): pass
 
-    def method21(cls): pass
+    def method21(self): pass
 
-    def method22(cls): pass
+    def method22(self): pass
 
-    def method23(cls): pass
+    def method23(self): pass
 
-    def method24(cls): pass
+    def method24(self): pass
 
-    def method25(cls): pass
+    def method25(self): pass
 
-    def method26(cls): pass
+    def method26(self): pass
 
-    def method27(cls): pass
+    def method27(self): pass
 
-    def method28(cls): pass
+    def method28(self): pass
 
-    def method29(cls): pass
+    def method29(self): pass
 
-    def method30(cls): pass
+    def method30(self): pass
 
-    def method31(cls): pass
+    def method31(self): pass
 
-    def method32(cls): pass
+    def method32(self): pass
 
-    def method33(cls): pass
+    def method33(self): pass
 
-    def method34(cls): pass
+    def method34(self): pass
 
-    def method35(cls): pass
+    def method35(self): pass
 
-    def method36(cls): pass
+    def method36(self): pass
 
-    def method37(cls): pass
+    def method37(self): pass
 
-    def method38(cls): pass
+    def method38(self): pass
 
-    def method39(cls): pass
+    def method39(self): pass
 
-    def method40(cls): pass
+    def method40(self): pass
 
-    def method41(cls): pass
+    def method41(self): pass
 
-    def method42(cls): pass
+    def method42(self): pass
 
-    def method43(cls): pass
+    def method43(self): pass
 
-    def method44(cls): pass
+    def method44(self): pass
 
-    def method45(cls): pass
+    def method45(self): pass
 
-    def method46(cls): pass
+    def method46(self): pass
 
-    def method47(cls): pass
+    def method47(self): pass
 
-    def method48(cls): pass
+    def method48(self): pass
 
-    def method49(cls): pass
+    def method49(self): pass
+
+    def method50(self): pass
 
-    def method50(cls): pass
 
 class Static(object):
     @classmethod
     def method1(cls): pass
     @classmethod
     def method2(cls): pass
     @classmethod
@@ -201,16 +203,15 @@
     def method48(cls): pass
     @classmethod
     def method49(cls): pass
     @classmethod
     def method50(cls): pass
 
 
-
 with Timer(msg="Inst.") as t:
     for i in range(1**6):
         Instance()
 
 
 with Timer(msg="Static") as t:
     for i in range(1**6):
-        Static()
+        Static()
```

### Comparing `scipion-em-pwperformance-0.0.4/pwperformance/loggers/influxdb.py` & `scipion-em-pwperformance-0.0.5/pwperformance/loggers/influxdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,18 +46,18 @@
         record.name will be passed as `logger` parameter.
     :param level_names: Allows the use of string error level names instead
         of numerical values. Defaults to False
     :param client_kwargs: Pass these args to the InfluxDBClient constructor
     """
 
     def __init__(self,
-                 token = "unset",
-                 bucket = "unset",
-                 org = "unset",
-                 url = "http://localhost:8086",
+                 token="unset",
+                 bucket="unset",
+                 org="unset",
+                 url="http://localhost:8086",
                  indexed_keys=['level', 'short_message'],
                  debugging_fields=True,
                  extra_fields=True,
                  localname=None,
                  measurement=None,
                  level_names=False,
                  backpop=True,
@@ -234,8 +234,8 @@
     return json.dumps(traceback.format_exception(*exc_info)) if exc_info else json.dumps([message])
 
 
 def add_extra_fields(message_dict, record):
     for key, value in record.__dict__.items():
         if key not in SKIP_LIST and not key.startswith('_'):
             message_dict[key] = value
-    return message_dict
+    return message_dict
```

### Comparing `scipion-em-pwperformance-0.0.4/pwperformance/tests/test_exportsteps.py` & `scipion-em-pwperformance-0.0.5/pwperformance/tests/test_exportsteps.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
 import pyworkflow
 from pyworkflow.project import Manager, Project
-# Get the manager
+
 from pwperformance.main import Benchmark, codespeed
 
 
 class TestExportSteps(unittest.TestCase):
 
     def testExportSteps(self):
 
@@ -15,31 +15,30 @@
 
         for project in manager.listProjects():
             projectFolder = manager.getProjectPath(project.projName)
 
             project = Project(pyworkflow.Config.getDomain(), projectFolder)
             project.load()
 
-
             for prot in project.getRuns():
                 protName = prot.getClassName()
                 for step in prot.loadSteps():
-                    stepName= "-".join([prot.getClassPackageName(), protName, step.funcName.get()])
+                    stepName = "-".join([prot.getClassPackageName(), protName, step.funcName.get()])
                     stepSeconds = step.getElapsedTime().total_seconds()
                     if stepName not in stepsStats:
                         stepsStats[stepName] = []
 
                     stepsStats[stepName].append(stepSeconds)
 
         # average steps
         for name in stepsStats:
             plugin, protClass, step = name.split("-")
             stepStats = stepsStats[name]
             mean = sum(stepStats) / len(stepStats)
             # DO not send mean values if higher than a threshold to keep chart in a decent visualization range
-            # We are loosing long duration steps, probably due to large
+            # We are losing long duration steps, probably due to large
             if mean < 30:
                 bm = Benchmark(time=mean,
-                           name= "-".join([protClass, step]))
-                codespeed.sendData(bm)
-
+                               name="-".join([protClass, step]))
+                codespeed.saveData(self, bm)
 
+        codespeed.sendData()
```

### Comparing `scipion-em-pwperformance-0.0.4/pwperformance/tests/test_influxhandler.py` & `scipion-em-pwperformance-0.0.5/pwperformance/tests/test_influxhandler.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,37 +4,44 @@
 from pwperformance.loggers import InfluxHandler
 import logging
 
 INFLUX_TOKEN = "INFLUX_TOKEN"
 
 logger = logging.getLogger(__file__)
 
+
 class TestInfluxHandler(unittest.TestCase):
 
     def testBasicSend(self):
         # Keys indexed by influx: search and filtering can only be done on this elements
 
         bucket = "scipion-benchmarks"
         org = "CNB"
         token = os.environ.get(INFLUX_TOKEN, None)
 
         if token is None:
             # Cancel the test
             logger.warning("Missing credentials to run this test. %s not set" % INFLUX_TOKEN)
             return
 
-        indexed_keys = ["project_name",	"prot_id" ,"prot_name", "step_id"]
-        ih = InfluxHandler(token= token, org= org, bucket= bucket, indexed_keys=indexed_keys, measurement="testBasicSend")
+        indexed_keys = ["project_name", "prot_id", "prot_name", "step_id"]
+        ih = InfluxHandler(token=token, org=org, bucket=bucket,
+                           indexed_keys=indexed_keys, measurement="testBasicSend")
         logger.addHandler(ih)
         logger.setLevel(logging.INFO)
-        logger.info("Testing sending data", extra=getExtraLogInfo("myproject", "START", prot_id=1, prot_name="ProtClass", step_id=1, duration=3.4))
+        logger.info("Testing sending data",
+                    extra=getExtraLogInfo("myproject", "START", prot_id=1,
+                                          prot_name="ProtClass", step_id=1,
+                                          duration=3.4))
         logger.info("Testing sending data")
 
-def getExtraLogInfo(project_name, status, prot_id=None, prot_name=None, step_id=None , duration=None):
+
+def getExtraLogInfo(project_name, status, prot_id=None, prot_name=None,
+                    step_id=None, duration=None):
     # Add TS!! optionally
     return {"project_name": project_name,
             "status": status,
             "prot_id": prot_id,
             "prot_name": prot_name,
             "step_id": step_id,
             "duration": duration
-    }
+            }
```

### Comparing `scipion-em-pwperformance-0.0.4/pwperformance/tests/test_profiling_load.py` & `scipion-em-pwperformance-0.0.5/pwperformance/tests/test_profiling_load.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import pyworkflow as pw
 import pyworkflow.project as pwobj
 from pwperformance.main import Timer, Benchmark, codespeed
 
 
 class TestProfilingLoadGUI(unittest.TestCase):
     root = tk.Tk()
-    def createCanvas(self):
 
+    def createCanvas(self):
         canvas = pwgui.Canvas(self.root, width=800, height=800,
                               tooltipDelay=1000,
                               name="runs_canvas",
                               takefocus=True,
                               highlightthickness=0)
 
         canvas.frame.grid(row=0, column=0, sticky='nsew')
@@ -38,19 +38,22 @@
             nodeId = node.run.getObjId() if node.run else 0
             nodeInfo = settings.getNodeById(nodeId)
             if nodeInfo is None:
                 settings.addNode(nodeId, x=0, y=0, expanded=True)
         return runsGraph
 
     def findProjects(self):
-        self.projectsPath = os.environ.get("PROFILING_PROJECTS_PATH", "/home/yunior/profilingProjects/")
+        self.projectsPath = os.path.join(pw.Config.SCIPION_USER_DATA, "projects")
+        projects = []
+
+        for item in os.listdir(self.projectsPath):
+            if os.path.isdir(os.path.join(self.projectsPath, item)):
+                projects.append(item)
 
-        if self.projectsPath is not None:
-            for base, dirs, files in os.walk(self.projectsPath):
-                return dirs
+        return projects
 
     def testLoadProjectGUI(self):
         t = Timer()
         localProjects = self.findProjects()
         t.tic()
         for projectFolder in localProjects:
             print("Profiling %s" % projectFolder)
@@ -63,13 +66,12 @@
                 runsGraph = self.getRunsGraph(project)
                 layout = pwgui.LevelTreeLayout()
                 canvas.drawGraph(runsGraph, layout, drawNode=None)
                 loadProjectTime = t.getElapsedTime()
                 bm = Benchmark(time=loadProjectTime.total_seconds(),
                                name="Load project %s with GUI with %s protocols" % (
                                projectFolder, self.numberofprotocols))
-                codespeed.sendData(bm)
-            except Exception as e:
+                codespeed.saveData(self, bm)
+            except Exception:
                 print("Error loading the project %s" % projectFolder)
 
-
-
+        codespeed.sendData()
```

### Comparing `scipion-em-pwperformance-0.0.4/pwperformance/tests/test_set_performance.py` & `scipion-em-pwperformance-0.0.5/pwperformance/tests/test_set_performance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-import sys
-
-
-# Initialize scipion environment
 import tempfile
 import unittest
-
-from pwperformance.main import Timer, Benchmark, BENCHMARK, codespeed
-from pwem.objects import SetOfCoordinates, Coordinate, SetOfParticles, Integer, Particle, Acquisition, Micrograph, Movie
 import os
-from  datetime import timedelta
+from datetime import timedelta
 
+from pwperformance.main import Timer, Benchmark, codespeed
+from pwem.objects import (SetOfCoordinates, Coordinate, SetOfParticles, Integer,
+                          Particle, Acquisition, Micrograph, Movie)
 from pyworkflow.tests import DataSet
 
 
 class TestSetPerformanceSteps(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
@@ -29,19 +25,20 @@
         # To avoid dict get
         newCoord = Coordinate()
         newCoord.setX(iteration)
         newCoord.setY(iteration)
         return newCoord
 
     def testBasicCoordinatesSet(self):
-
-        measureSetPerformance(SetOfCoordinates, self.basiccoordsFactory, "basic-coords")
+        res = measureSetPerformance(SetOfCoordinates, self.basiccoordsFactory, "basic-coords")
+        for r in res:
+            codespeed.saveData(self, r)
+        codespeed.sendData()
 
     def testExtendedCoordinatesSet(self):
-
         def coordsFactory(iteration):
             # newCoord =  Coordinate(x=i, y=i)
             # To avoid dict get
             newCoord = Coordinate()
             newCoord.setX(iteration)
             newCoord.setY(iteration)
             newCoord.extra1 = Integer(1)
@@ -53,18 +50,20 @@
             newCoord.extra7 = Integer(1)
             newCoord.extra8 = Integer(1)
             newCoord.extra9 = Integer(1)
             newCoord.extra10 = Integer(1)
 
             return newCoord
 
-        measureSetPerformance(SetOfCoordinates, coordsFactory, "extended-10-coords")
+        res = measureSetPerformance(SetOfCoordinates, coordsFactory, "extended-10-coords")
+        for r in res:
+            codespeed.saveData(self, r)
+        codespeed.sendData()
 
     def testSuperExtendedCoordinatesSet(self):
-
         def coordsFactory(iteration):
             # newCoord =  Coordinate(x=i, y=i)
             # To avoid dict get
             newCoord = Coordinate()
             newCoord.setX(iteration)
             newCoord.setY(iteration)
             newCoord.extra1 = Integer(1)
@@ -85,88 +84,106 @@
             newCoord.extra15 = Integer(1)
             newCoord.extra16 = Integer(1)
             newCoord.extra17 = Integer(1)
             newCoord.extra18 = Integer(1)
             newCoord.extra19 = Integer(1)
             newCoord.extra20 = Integer(1)
 
-
             return newCoord
 
-        measureSetPerformance(SetOfCoordinates, coordsFactory, "extended-20-coords", numberofitems=10**6)
+        res = measureSetPerformance(SetOfCoordinates, coordsFactory,
+                              "extended-20-coords", numberofitems=10 ** 6)
+        for r in res:
+            codespeed.saveData(self, r)
+        codespeed.sendData()
 
     def testBasicMicsSetPerformance(self):
-
         def micsFactory(index):
             newMic = Micrograph(location=self.mic1)
             return newMic
 
-        measureSetPerformance(SetOfParticles, micsFactory, "basic mics")
-
+        res = measureSetPerformance(SetOfParticles, micsFactory, "basic mics")
+        for r in res:
+            codespeed.saveData(self, r)
+        codespeed.sendData()
 
     def testBasicMoviesSetPerformance(self):
-
         def moviesFactory(index):
             newMovie = Movie(location=self.movieFn)
             return newMovie
 
-        measureSetPerformance(SetOfParticles, moviesFactory, "basic movies")
-
+        res = measureSetPerformance(SetOfParticles, moviesFactory, "basic movies")
+        for r in res:
+            codespeed.saveData(self, r)
+        codespeed.sendData()
 
     def testBasicParticlesSetPerformance(self):
-
         def particlesFactory(index):
-            newParticle = Particle(location=(1,self.particlesStk))
+            newParticle = Particle(location=(1, self.particlesStk))
             return newParticle
 
-        measureSetPerformance(SetOfParticles, particlesFactory, "basic particles")
-
+        res = measureSetPerformance(SetOfParticles, particlesFactory, "basic particles")
+        for r in res:
+            codespeed.saveData(self, r)
+        codespeed.sendData()
 
     def testComplexParticlesSetPerformance(self):
-
         def particlesFactory(index):
-            newParticle = Particle(location=(1,self.particlesStk))
-            newParticle.setCoordinate(Coordinate(x=1,y=2))
+            newParticle = Particle(location=(1, self.particlesStk))
+            newParticle.setCoordinate(Coordinate(x=1, y=2))
             newParticle.setAcquisition(Acquisition())
             return newParticle
 
-        measureSetPerformance(SetOfParticles, particlesFactory, "complex particles")
+        res = measureSetPerformance(SetOfParticles, particlesFactory, "complex particles")
+        for r in res:
+            codespeed.saveData(self, r)
+        codespeed.sendData()
 
     def testUsingGet(self):
         """ This benchmarks the time accessing an item as a dictionary, like set[id]."""
         items = 100
         soc = createSet(SetOfCoordinates)
-        createItems(soc, self.basiccoordsFactory, numberofitems=items)
+        results = createItems(soc, self.basiccoordsFactory, numberofitems=items)
         t = Timer("A %s Set.__item__ calls" % items)
         t.tic()
-        for id in range(1,items+1):
+        for id in range(1, items + 1):
             soc[id]
         t.toc()
         bm = Benchmark(time=t.getElapsedTime().total_seconds(),
                        name="A %s Set.__item__ calls" % items)
 
-        codespeed.sendData(bm)
+        results.append(bm)
+        for r in results:
+            codespeed.saveData(self, r)
+        codespeed.sendData()
+
 
 def measureSetPerformance(setClass, itemFactory, performanceTag, numberofitems=100000):
-    """ Measures instantiation, persistence and iteration of a set, sending data to a codespeed benchmark server"""
+    """ Measures instantiation, persistence and iteration of a set,
+    sending data to a codespeed benchmark server"""
 
     newSet = createSet(setClass)
 
-    createItems(newSet, itemFactory, numberofitems=numberofitems, performanceTag=performanceTag)
+    results = createItems(newSet, itemFactory, numberofitems=numberofitems, performanceTag=performanceTag)
+
+    bm = measureSetIteration(newSet, performanceTag)
+    results.append(bm)
 
-    measureSetIteration(newSet, performanceTag)
+    return results
 
 
 def createItems(set, itemfactory, numberofitems=100000, performanceTag=None):
     """ Create X items using numberofitems and the itemfactory method and reports its
     instantiation time and persistence time to the benchmark server
     :parameter set: Set instance to be used
     :parameter itemfactory: method to call to create a specific item. Receives the index of the iteration
     :parameter performanceTag: tag to use to create the benchmark name"""
 
+    results = []
+
     # To hold sum elapsed time
     creation = timedelta()
     append = timedelta()
 
     t = Timer()
     for i in range(numberofitems):
         t.tic()
@@ -175,46 +192,48 @@
         t.tic()
         set.append(newItem)
         append += t.getElapsedTime()
 
     set.write()
 
     if performanceTag:
-
         bm = Benchmark(time=creation.total_seconds(),
                        name="Instantiation of %s %s" % (numberofitems, performanceTag))
-
-        codespeed.sendData(bm)
+        results.append(bm)
 
         bm = Benchmark(time=append.total_seconds(),
                        name="Persistence of %s %s" % (numberofitems, performanceTag))
+        results.append(bm)
 
-        codespeed.sendData(bm)
+        bm = measureSetIteration(set, performanceTag)
+        results.append(bm)
+
+    return results
 
-        measureSetIteration(set, performanceTag)
 
 def createSet(setClass):
     """ Create a set based on the setClass in the system temporary folder"""
 
     tmpFolder = tempfile.gettempdir()
-    setFile = str(setClass.__name__) +  "%s.sqlite"
+    setFile = str(setClass.__name__) + "%s.sqlite"
     sqliteFile = os.path.join(tmpFolder, setFile % "")
 
     if os.path.exists(sqliteFile):
         os.remove(sqliteFile)
 
     return setClass.create(tmpFolder, template=setFile)
 
 
 def measureSetIteration(set, performanceTag):
     """ Measures the time  taken to iterate over the set passed.
-    :parameter set set to iterate on
+    :parameter set to iterate on
     :parameter performanceTag: text to name the benchmark"""
 
     iterT = Timer()
     iterT.tic()
     for item in set.iterItems():
         pass
     iterT.toc()
     bm = Benchmark(time=iterT.getElapsedTime().total_seconds(),
                    name="Iteration-%s" % performanceTag)
-    codespeed.sendData(bm)
+
+    return bm
```

### Comparing `scipion-em-pwperformance-0.0.4/scipion_em_pwperformance.egg-info/SOURCES.txt` & `scipion-em-pwperformance-0.0.5/scipion_em_pwperformance.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.rst
 requirements.txt
 setup.py
 pwperformance/StaticVsInstanceMethod.py
 pwperformance/__init__.py
+pwperformance/client.py
 pwperformance/hassAttrVsTry.py
 pwperformance/main.py
 pwperformance/loggers/__init__.py
 pwperformance/loggers/influxdb.py
 pwperformance/tests/__init__.py
 pwperformance/tests/test_exportsteps.py
 pwperformance/tests/test_influxhandler.py
```

### Comparing `scipion-em-pwperformance-0.0.4/setup.py` & `scipion-em-pwperformance-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,24 +43,24 @@
     # For a list of valid classifiers, see
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[  # Optional
         # How maturupdateOutputMIcSete is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
-        'Development Status :: 2 - Pre-Alpha',
+        'Development Status :: 3 - Alpha',
         # Indicate who your project is intended for
         'Intended Audience :: Science/Research',
         # Pick your license as you wish
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
         'Topic :: Scientific/Engineering'
     ],
     keywords='scipion cryoem imageprocessing scipion-3.0',  # Optional
     packages=find_packages(),
     install_requires=[requirements],
     entry_points={
         'pyworkflow.plugin': 'pwperformance = pwperformance'
```

