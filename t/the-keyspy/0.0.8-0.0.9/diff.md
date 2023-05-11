# Comparing `tmp/the_keyspy-0.0.8.tar.gz` & `tmp/the_keyspy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "the_keyspy-0.0.8.tar", last modified: Sun Nov 21 17:53:22 2021, max compression
+gzip compressed data, was "the_keyspy-0.0.9.tar", last modified: Wed Dec 15 13:28:30 2021, max compression
```

## Comparing `the_keyspy-0.0.8.tar` & `the_keyspy-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2021-11-21 17:53:22.820539 the_keyspy-0.0.8/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1062 2021-11-21 16:29:29.000000 the_keyspy-0.0.8/LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      339 2021-11-21 17:53:22.820539 the_keyspy-0.0.8/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)       79 2021-11-21 17:53:22.824539 the_keyspy-0.0.8/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)      571 2021-11-21 17:52:27.000000 the_keyspy-0.0.8/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2021-11-21 17:53:22.820539 the_keyspy-0.0.8/the_keyspy/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7329 2021-11-21 17:44:00.000000 the_keyspy-0.0.8/the_keyspy/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2021-11-21 17:53:22.820539 the_keyspy-0.0.8/the_keyspy/devices/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1026 2021-11-21 17:18:26.000000 the_keyspy-0.0.8/the_keyspy/devices/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1829 2021-11-13 15:42:29.000000 the_keyspy-0.0.8/the_keyspy/devices/lock.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2021-11-21 17:53:22.820539 the_keyspy-0.0.8/the_keyspy.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      339 2021-11-21 17:53:22.000000 the_keyspy-0.0.8/the_keyspy.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      280 2021-11-21 17:53:22.000000 the_keyspy-0.0.8/the_keyspy.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2021-11-21 17:53:22.000000 the_keyspy-0.0.8/the_keyspy.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2021-11-21 17:53:22.000000 the_keyspy-0.0.8/the_keyspy.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       11 2021-11-21 17:53:22.000000 the_keyspy-0.0.8/the_keyspy.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2021-12-15 13:28:30.787083 the_keyspy-0.0.9/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1062 2021-11-21 16:29:29.000000 the_keyspy-0.0.9/LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      339 2021-12-15 13:28:30.787083 the_keyspy-0.0.9/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       79 2021-12-15 13:28:30.787083 the_keyspy-0.0.9/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      571 2021-12-15 13:28:15.000000 the_keyspy-0.0.9/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2021-12-15 13:28:30.787083 the_keyspy-0.0.9/the_keyspy/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7329 2021-11-21 17:44:00.000000 the_keyspy-0.0.9/the_keyspy/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2021-12-15 13:28:30.787083 the_keyspy-0.0.9/the_keyspy/devices/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1070 2021-12-15 13:20:05.000000 the_keyspy-0.0.9/the_keyspy/devices/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1828 2021-12-15 13:27:12.000000 the_keyspy-0.0.9/the_keyspy/devices/lock.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2021-12-15 13:28:30.787083 the_keyspy-0.0.9/the_keyspy.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      339 2021-12-15 13:28:30.000000 the_keyspy-0.0.9/the_keyspy.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      280 2021-12-15 13:28:30.000000 the_keyspy-0.0.9/the_keyspy.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2021-12-15 13:28:30.000000 the_keyspy-0.0.9/the_keyspy.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2021-12-15 13:28:30.000000 the_keyspy-0.0.9/the_keyspy.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       11 2021-12-15 13:28:30.000000 the_keyspy-0.0.9/the_keyspy.egg-info/top_level.txt
```

### Comparing `the_keyspy-0.0.8/LICENSE.txt` & `the_keyspy-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `the_keyspy-0.0.8/setup.py` & `the_keyspy-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import find_packages, setup
 
 setup(
     name='the_keyspy',
     packages=find_packages(include=('the_keyspy*',)),
-    version='0.0.8',
+    version='0.0.9',
     description='The Keys Api',
     author='Kevin Bonnoron',
     author_email='kevin.bonnoron@gmail.com',
     url='https://github.com/KevinBonnoron',
-    download_url='https://github.com/KevinBonnoron/the_keyspy/archive/refs/tags/v0.0.8.tar.gz',
+    download_url='https://github.com/KevinBonnoron/the_keyspy/archive/refs/tags/v0.0.9.tar.gz',
     license='MIT',
     install_requires=['dataclasses_json', 'requests'],
     setup_requires=['pytest-runner'],
     tests_require=['pytest==6.2.4'],
     test_suite='tests',
 )
```

### Comparing `the_keyspy-0.0.8/the_keyspy/__init__.py` & `the_keyspy-0.0.9/the_keyspy/__init__.py`

 * *Files identical despite different names*

### Comparing `the_keyspy-0.0.8/the_keyspy/devices/__init__.py` & `the_keyspy-0.0.9/the_keyspy/devices/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
 class Action(Enum):
     """All available actions"""
     OPEN = "open"
     CLOSE = "close"
     STATUS = "locker_status"
 
+    def __str__(self):
+        return self.value
+
 
 class TheKeysDevice:
     """Base class for all TheKeys devices"""
 
     def __init__(self, name: str, host: str, identifier: str, share_code: str) -> None:
         self.name = name
         self.host = host
@@ -29,11 +32,11 @@
 
     def action(self, action: Action) -> Any:
         """Execute action on the device"""
         timestamp = str(int(time.time()))
         hash = base64.b64encode(hmac.new(self.share_code.encode("ascii"), timestamp.encode("ascii"), "sha256").digest())
 
         response = requests.post(
-            f"{self.host}/{action.value}",
+            f"{self.host}/{action}",
             data={"hash": hash, "identifier": self.identifier, "ts": timestamp},
         )
         return response.json()
```

### Comparing `the_keyspy-0.0.8/the_keyspy/devices/lock.py` & `the_keyspy-0.0.9/the_keyspy/devices/lock.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 """The Keys lock device implementation"""
 import logging
+
 from . import Action, TheKeysDevice
 
 OPENED = "Door open"
 CLOSED = "Door closed"
 JAMMED = "Door jammed"
-UNKNOWED = ""
+UNKNOWN = ""
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class TheKeysLock(TheKeysDevice):
     """The Keys lock device implementation"""
 
     def __init__(self, name: str, host: str, identifier: str, share_code: str) -> None:
         super().__init__(
             name=name, host=host, identifier=identifier, share_code=share_code
         )
-        self.locker_status = UNKNOWED
+        self.locker_status = UNKNOWN
         self.__retrieve_lock_status()
 
-    def lock(self) -> None:
+    def lock(self) -> bool:
         """Lock this lock"""
         response = self.action(Action.CLOSE)
         if response["status"] == "ok":
             self.locker_status = CLOSED
         else:
             self.locker_status = JAMMED
 
         return response["status"] == "ok"
 
-    def unlock(self) -> None:
+    def unlock(self) -> bool:
         """Unlock this lock"""
         response = self.action(Action.OPEN)
         if response["status"] == "ok":
             self.locker_status = OPENED
         else:
             self.locker_status = JAMMED
```

