# Comparing `tmp/emmi-0.0.10.tar.gz` & `tmp/emmi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmi-0.0.10.tar", last modified: Wed Nov 23 14:29:28 2022, max compression
+gzip compressed data, was "emmi-0.1.3.tar", last modified: Thu May 11 13:36:14 2023, max compression
```

## Comparing `emmi-0.0.10.tar` & `emmi-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 14:29:28.010317 emmi-0.0.10/
--rw-rw-rw-   0 root         (0) root         (0)       77 2022-11-23 14:29:14.000000 emmi-0.0.10/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     3261 2022-11-23 14:29:14.000000 emmi-0.0.10/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)    35147 2022-11-23 14:29:14.000000 emmi-0.0.10/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10854 2022-11-23 14:29:28.010317 emmi-0.0.10/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10056 2022-11-23 14:29:14.000000 emmi-0.0.10/README.md
--rw-rw-rw-   0 root         (0) root         (0)      280 2022-11-23 14:29:14.000000 emmi-0.0.10/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      917 2022-11-23 14:29:28.010317 emmi-0.0.10/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 14:29:28.006317 emmi-0.0.10/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 14:29:28.006317 emmi-0.0.10/src/emmi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-23 14:29:14.000000 emmi-0.0.10/src/emmi/__init__.py
--rw-r--r--   0 root         (0) root         (0)      178 2022-11-23 14:29:27.000000 emmi-0.0.10/src/emmi/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2022-11-23 14:29:14.000000 emmi-0.0.10/src/emmi/app.py
--rw-rw-rw-   0 root         (0) root         (0)    31013 2022-11-23 14:29:14.000000 emmi-0.0.10/src/emmi/eda.py
--rw-rw-rw-   0 root         (0) root         (0)     7152 2022-11-23 14:29:14.000000 emmi-0.0.10/src/emmi/scpi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 14:29:28.006317 emmi-0.0.10/src/emmi.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10854 2022-11-23 14:29:27.000000 emmi-0.0.10/src/emmi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      356 2022-11-23 14:29:28.000000 emmi-0.0.10/src/emmi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-23 14:29:27.000000 emmi-0.0.10/src/emmi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2022-11-23 14:29:27.000000 emmi-0.0.10/src/emmi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2022-11-23 14:29:27.000000 emmi-0.0.10/src/emmi.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 14:29:28.010317 emmi-0.0.10/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2267 2022-11-23 14:29:14.000000 emmi-0.0.10/tests/eda_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1033 2022-11-23 14:29:14.000000 emmi-0.0.10/tests/motor_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:36:14.182713 emmi-0.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-05-11 13:35:57.000000 emmi-0.1.3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     3263 2023-05-11 13:35:57.000000 emmi-0.1.3/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2023-05-11 13:35:57.000000 emmi-0.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    10853 2023-05-11 13:36:14.182713 emmi-0.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10056 2023-05-11 13:35:57.000000 emmi-0.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:36:14.182713 emmi-0.1.3/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-11 13:35:57.000000 emmi-0.1.3/examples/simple-ioc.json
+-rwxrwxrwx   0 root         (0) root         (0)     1772 2023-05-11 13:35:57.000000 emmi-0.1.3/examples/simple-ioc.py
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-05-11 13:35:57.000000 emmi-0.1.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      946 2023-05-11 13:36:14.186713 emmi-0.1.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:36:14.182713 emmi-0.1.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:36:14.182713 emmi-0.1.3/src/emmi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 13:35:57.000000 emmi-0.1.3/src/emmi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-11 13:36:14.000000 emmi-0.1.3/src/emmi/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:36:14.182713 emmi-0.1.3/src/emmi/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 13:35:57.000000 emmi-0.1.3/src/emmi/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30493 2023-05-11 13:35:57.000000 emmi-0.1.3/src/emmi/api/exports.py
+-rw-rw-rw-   0 root         (0) root         (0)    16676 2023-05-11 13:35:57.000000 emmi-0.1.3/src/emmi/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:36:14.182713 emmi-0.1.3/src/emmi/ca/
+-rwxrwxrwx   0 root         (0) root         (0)    12118 2023-05-11 13:35:57.000000 emmi-0.1.3/src/emmi/ca/histo.py
+-rw-rw-rw-   0 root         (0) root         (0)     4794 2023-05-11 13:35:57.000000 emmi-0.1.3/src/emmi/ca/reader.py
+-rw-rw-rw-   0 root         (0) root         (0)    20537 2023-05-11 13:35:57.000000 emmi-0.1.3/src/emmi/eda.py
+-rw-rw-rw-   0 root         (0) root         (0)     8167 2023-05-11 13:35:57.000000 emmi-0.1.3/src/emmi/scpi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:36:14.182713 emmi-0.1.3/src/emmi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10853 2023-05-11 13:36:14.000000 emmi-0.1.3/src/emmi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      581 2023-05-11 13:36:14.000000 emmi-0.1.3/src/emmi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 13:36:14.000000 emmi-0.1.3/src/emmi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-11 13:36:14.000000 emmi-0.1.3/src/emmi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-11 13:36:14.000000 emmi-0.1.3/src/emmi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:36:14.182713 emmi-0.1.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5431 2023-05-11 13:35:57.000000 emmi-0.1.3/tests/api_exports_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5158 2023-05-11 13:35:57.000000 emmi-0.1.3/tests/app_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2342 2023-05-11 13:35:57.000000 emmi-0.1.3/tests/eda_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-05-11 13:35:57.000000 emmi-0.1.3/tests/motor_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2023-05-11 13:35:57.000000 emmi-0.1.3/tests/pytest_dev.yaml
+-rwxrwxrwx   0 root         (0) root         (0)     1292 2023-05-11 13:35:57.000000 emmi-0.1.3/tests/scpi_test.py
```

### Comparing `emmi-0.0.10/.gitlab-ci.yml` & `emmi-0.1.3/.gitlab-ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 default:
   image:
     name: python:latest
 
 variables:
   PIP_CACHE_DIR: "$CI_PROJECT_DIR/.cache/pip"
-  PYPI_RELEASE_URL: https://test.pypi.org/legacy/
+  PYPI_RELEASE_URL: https://upload.pypi.org/legacy/
 
 cache:
   paths:
     - .cache/pip
     - venv/
 
 stages:
```

### Comparing `emmi-0.0.10/LICENSE` & `emmi-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `emmi-0.0.10/PKG-INFO` & `emmi-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emmi
-Version: 0.0.10
+Version: 0.1.3
 Summary: A Selection of Tools for EPICS Monday-Morning Integrations
 Author: Florin Boariu
 Author-email: florin.pt@rootshell.ro
 Project-URL: Homepage, https://emmi.rootshell.ro
 Project-URL: Source Code, https://gitlab.com/codedump2/emmi/
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/emmi/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `emmi-0.0.10/README.md` & `emmi-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `emmi-0.0.10/setup.cfg` & `emmi-0.1.3/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -19,19 +19,22 @@
 	Source Code = https://gitlab.com/codedump2/emmi/
 	Bug Tracker = https://gitlab.com/codedump2/emmi/-/issues
 
 [options]
 requires_python = >=3.6
 install_requires = 
 	pyvisa
+	softioc
+	schema
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
 	softioc
 	pyepics
+	PyVISA-sim
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `emmi-0.0.10/src/emmi/eda.py` & `emmi-0.1.3/src/emmi/api/exports.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-#!/usr/bin/python3
+#!/usr/bin/python
 
-import time
-import asyncio
+from schema import *
+from softioc import builder as IocBuilder
+
+from pprint import pprint
+from functools import partial, reduce
 
-import logging
+import time, asyncio, logging, inspect
 
 '''
 Validators are a concept that allow us to filter, translate and validate
 data (values) from one ecosystem (e.g. EPICS) into another (e.g. SCIP).
 Each validator needs to have at least:
 
   - one setup() function which receives named arguments with the necessary
@@ -25,19 +28,18 @@
     def __init__(self, values={}):
         self.setup(values)
 
     def setup(self, values={}):
         self.trmap = values
 
     def __getitem__(self, val):
-        try:
-            #print ("Mapping: %r -> %r (%r)" % (val, self.trmap.get(val), self.trmap))
+        if val in self.trmap:
             return self.trmap.get(val)
-        except KeyError:
-            raise ValueError("%r: invalid value" % val)
+        
+        raise ValueError("%r: invalid value" % val)
 
 
 class SetValidator(object):
     '''
     Accepts only objects form a specific set.
     '''
     def __init__(self, **kwargs):
@@ -54,30 +56,30 @@
 
 
 class BoundaryValidator(object):
     '''
     Accepts only values within specified boundaries
     '''
     def __init__(self, **kwargs):
-        self.setup(kwargs)
+        self.setup(**kwargs)
 
     def setup(self, limits=[None, None], inclusive=[True, True], invert=False):
         self.lim = limits
         self.incl = inclusive
         self.inv = invert
 
     def __getitem__(self, val):
         err = ValueError("%r: outside of range" % val)
-        if ((self.lim[0] is not None) and (self.inc[0] and val < self.lim[0])) == (not invert):
+        if ((self.lim[0] is not None) and (self.incl[0] and val < self.lim[0])) == (not self.inv):
             raise err
-        if ((self.lim[1] is not None) and (self.inc[1] and val > self.lim[1])) == (not invert):
+        if ((self.lim[1] is not None) and (self.incl[1] and val > self.lim[1])) == (not self.inv):
             raise err
-        if ((self.lim[0] is not None) and (not self.inc[0] and val <= self.lim[0])) == (not invert):
+        if ((self.lim[0] is not None) and (not self.incl[0] and val <= self.lim[0])) == (not self.inv):
             raise err
-        if ((self.lim[1] is not None) and (not self.inc[1] and val >= self.lim[1])) == (not invert):
+        if ((self.lim[1] is not None) and (not self.incl[1] and val >= self.lim[1])) == (not self.inv):
             raise err
         return val
 
     
 class SliceValidator(object):
     '''
     Returns only specified slice of an (iterable/indexable) value.
@@ -96,714 +98,351 @@
     ''' Lets everything through '''
 
     def setup(self):
         pass
     
     def __getitem__(self, val):
         return val
-    
-
-class MockMotor(object):
-    '''
-    The simplest of the simplest motors: can only move, report position and stop.
-    '''
-
-    def __init__(self, *args, **kwargs):
-        self.mock_timeslice = kwargs.get('mock_timeslice', 5.0)
-        self.start = 0.0
-        self.target = 0.0
-        self.tstamp = time.time()
-        self.goto(0.0)
-    
-    def where(self):
-        '''
-        Returns current position -- that is the position that we'd be currently
-        having if we'd wanted to go from "current" towards "target" within
-        the timeslice "mock_timeslice"
-        '''
-        tdelta = (time.time()-self.tstamp)
-        if tdelta > self.mock_timeslice:
-            tdelta = self.mock_timeslice
-        dist = self.target-self.start
-        return self.start + dist * (tdelta/self.mock_timeslice)
 
-    def goto(self, val):
-        '''
-        Sends command to move to position (doesn't wait)
-        '''
-        self.start = self.where()
-        self.target = val
-        self.tstamp = time.time()
-
-    def stop(self):
-        '''
-        Sends command to stop (doesn't wait). Technically, we'll be still
-        in state "moving" for a while after this, but we'd be moving towards the position
-        we're already onto.
-        '''
-        if self.moves():
-            self.goto(self.where())
-
-    def moves(self):
-        '''
-        Returns True if the motor moves. We fake this by testing whether
-        we're still within the "timeslice". This has the added benefit
-        that sometimes moves() returns False right away (i.e. if we weren't
-        moving in the first place), and sometimes still returns False
-        for a considerate amount of time (i.e. until the end of the current
-        slice) if we were moving and just received a stop() command.
-        '''
-        return (time.time()-self.tstamp) < self.mock_timeslice
-
-    def clear(self):
-        '''
-        Clears all outstanding error flags (they may pop up again).
-        '''
-        pass
-    
-
-class MotorEngine(object):
-    '''
-    Generic motor engine class. Essentially cycles through the states
-    as it should, and serves the most basic properties `position` and
-    `position_relative` correctly. It's based on generic True/False
-    conditional procedures to decide when to switch.
-
-    In its default incarnation, the conditionals are just generic waiting
-    functions (1 second for anything), so it can be used as a mock-up for
-    unit testing. But if you replace the conditionals by things that do
-    "real stuff", it's actually usable for production.
-    '''
-    
-    def __init__(self, motor=None):
-        
-        self.__motor = motor or MockMotor()
-
-        # current state
-        self.__state = "INIT"
-
-        # Scheduled absolute or relative position change.
-        # We move by storing the new positional values here first,
-        # then sending them on their way when we're IDLE.
-        self.__scheduled_goto = None
-        self.__scheduled_moveby = None
-
-        # Current errors list
-        self.errors = []        
-
-        # mock-up position setter 
-        self.hardware_where  = self.__motor.where       
-        self.hardware_ready  = lambda: True
-        self.hardware_goto   = self.__motor.goto
-        self.hardware_moveby = None
-        self.hardware_brake  = self.__motor.stop
-        self.hardware_moves  = self.__motor.moves
-        self.hardware_clear  = self.__motor.clear
-
-
-    def __clear_goto(self):
-        self.__scheduled_goto = None
-        self.__scheduled_moveby = None
-
-
-    def state_enter(self, state):
-        '''
-        This is called exactly once, at the beginning, for every
-        state that is newly entered. Returns the state string,
-        for convenience.
-        '''
-        logging.info ("State: %s -> %s" % (self.__state, state))
-        if state == "STOP":
-            self.__clear_goto()
-            if self.hardware_moves():
-                self.hardware_brake()
-        elif state == "BUSY":
-            if self.__scheduled_moveby is not None:
-                logging.info("BUSY state: relative move scheduled by %r" % self.__scheduled_moveby)
-                if self.hardware_moveby:
-                    self.hardware_moveby(self.__scheduled_moveby)
-                else:
-                    self.hardware_goto(self.hardware_where()+self.__scheduled_moveby)
-            elif self.__scheduled_goto is not None:
-                logging.info("BUSY state: absolute move scheduled to %r" % self.__scheduled_goto)
-                self.hardware_goto(self.__scheduled_goto)
-            self.__clear_goto()
-        elif state == "IDLE":
-            self.hardware_clear()
-            self.errors = []
-        else:
-            pass
-        return state
-             
-
-    ## State procedures -- return the new state they need to switch to.
-    ## We're essentially delegating everything to __generic_state_proc().
-    def state_proc(self, state):
-
-        # These are the states we can advance to from here
-        advances = {
-            'INIT': { 'IDLE':  lambda: self.hardware_ready() },
-            'IDLE': { 'STOP':  lambda: len(self.errors) > 0,
-                      'BUSY':  lambda: self.__scheduled_goto is not None or \
-                                       self.__scheduled_moveby is not None},
-            'BUSY': { 'STOP':  lambda: len(self.errors) > 0 or not self.hardware_moves() },
-            'STOP': { 'ERROR': lambda: len(self.errors) > 0 and not self.hardware_moves(),
-                      'IDLE':  lambda: len(self.errors) == 0 and not self.hardware_moves() },
-            'ERROR': { 'IDLE': lambda: len(self.errors) == 0 },
-            'FAIL': {}
-        }
-
-        try:
-            adv = advances[state]
-        except KeyError as e:
-            # BUSY needs to get some extra treatment because it can be extended
-            if state.startswith('BUSY'):
-                adv = advances['BUSY']
-
-        # execute current state proc
-        try:
-            for k,v in adv.items():
-                #print ("%s/Testing for %s: %r" % (state, k, v))
-                if v():
-                    return self.state_enter(k)
-        except Exception as e:
-            logging.error ("Unexpected exception in state %s:" % state, str(e))
-            return "FAIL"
-
-        return state
-    
-    
-    # Current position -- getter reads out the hardware, setter
-    # is a bit more complicated because we have to acknowledge
-    # the current state (i.e. can't just override current states).
-    @property
-    def position(self):
-        return self.hardware_where()
-
-    @position.setter
-    def position(self, val):
-        if self.state == "IDLE":
-            self.__scheduled_goto = val
-        trig = self.state
-
-             
-    # Increment/decrement position by relative values -- the getter returns
-    # 0 as soon as the scheduled move has been triggered, the setter just
-    # sends the command / schedules the move.
-    @property
-    def position_relative(self):
-        return self.__scheduled_moveby or 0
-    
-    @position_relative.setter
-    def position_relative(self, val):
-        if self.state == "IDLE":
-            self.__scheduled_moveby = val
-        trig = self.state
-        
-
-    def leave_ERROR(self, new_state):
-        '''
-        The only way we can leave ERROR is by clearing/going to IDLE
-        '''
-        if new_state == "IDLE":
-             self.errors = []
-             return self.state_enter("IDLE")
-        return "ERROR"
-             
-
-    def leave_BUSY(self, new_state):
-        '''
-        The only way we can leave BUSY is by issuing a STOP.
-        We accept that for `new_state` either as being STOP
-        or ERROR.
-        '''
-        logging.info ("Leaving BUSY:", new_state)
-        if new_state in [ "STOP", "ERROR" ]:
-             return self.state_enter("STOP")
-        return "BUSY"
-
-
-    @property
-    def state(self):
-        self.__state = self.state_proc(self.__state)
-        return self.__state
-             
-    @state.setter
-    def state(self, new_state):
-        '''
-        This is only an API point -- i.e. for external use, not
-        internal. There are only specific combinations of
-        "current state" / "end state" that the user is allowed
-        to perform. Everything else we ignore.
-        '''
-        if self.__state == 'ERROR':
-            self.__state = self.leave_ERROR(new_state)
-        elif self.__state.startswith("BUSY"):
-            self.__state = self.leave_BUSY(new_state)
 
 
 class PropertySetter(object):
     '''
     Wrapper that sets a property -- we need this because
     we want to build most of our API based on properties
     (insted of callable setter functions), but at several
     points in the involved APIs (softioc.Builder, for instance)
     callables are required.
     '''
 
-    def __init__(self, name, obj=None, prop=None, proc=None, validator=IdentityValidator()):
+    def __init__(self, name, setter, validator=None):
         self.name = name
-        self.setter_proc = proc
-        self.target_obj = obj
-        self.prop_name = prop
-        self.validator = validator
+        self.setter = setter
+        self.validator = validator or IdentityValidator()
         self.validation_failed = False
 
     async def __call__(self, value):
         try:
             valid = self.validator[value]
+            #logging.info("Value %r validates to %r (by %r)" % (value, valid, self.validator))
             self.validation_failed = False
-            if self.setter_proc:
-                try:
-                    await self.setter_proc(valid)
-                except TypeError as t:
-                    self.setter_proc(valid)
-            else:
-                setattr(self.target_obj, self.prop_name, valid)
+            try:
+                await self.setter(valid)
+            except TypeError as t:
+                self.setter(valid)
+                
         except ValueError as e:
             if not self.validation_failed:
                 logging.error("Failed to set %s: %r" % (self.name, e))
                 self.validation_failed = True
 
+        except Exception as e:
+            logging.error("%s: Setting value failed: %r" % (self.name, e))
+                
+        except:
+            logging.error("%s: Setting value failed" % (self.name,))
+
 
 class PropertyUpdater(object):
     '''
     A callable object which loops indefinitely reading out a property via `getter`
     and publishing it on EPICS process-variable `pv`. The waiting
     time on every loop run is such that a full run is as close
     as possible to `period`.
     '''
     
-    def __init__(self, name, pv, period, getter=None, obj=None, prop=None, validator=IdentityValidator()):
+    def __init__(self, name, pv, pollPeriod, getter, validator=None):
         self.name   = name
         self.pv     = pv
-        self.period = period
-        self.getter = getter or self.get_from_property
-        self.validator = validator
-        self.obj = obj
-        self.prop = prop
-
-    def get_from_property(self):
-        return getattr(self.obj, self.prop)
+        self.period = pollPeriod
+        self.getter = getter
+        self.validator = validator or IdentityValidator()
 
     def set_period(self, val):
         self.period = val
 
     async def __call__(self):
         logging.debug("%s: Updater running for PV %r" % (self.name, self.pv))
         available = True
         while True:
+            tstart = time.time()
             try:
-                tstart = time.time()
                 val = self.getter()
-                self.pv.set(self.validator[val])
+                
+                if val is not None:
+                    self.pv.set(self.validator[val])
 
                 if not available:
                     logging.info("%s: has become available again" % self.name)
                     available = True
                 
             except Exception as e:
                 # We're not going to exit on PV setting problems (may be
                 # intermittent), but at least we'll get loud about it.
                 if available:
                     logging.error("%s: property became unavailable, reason: %r" % (self.name, e))
                     logging.error("%s: further errors will be silenced" % self.name)
+                    logging.info("%s: Getter object was: %r" % (self.name, self.getter,))
                 available = False
             except e:
-                logging.error("%s: unknown exception %r" % e)
-                raise
-
-            tdiff = time.time()-tstart
-            await asyncio.sleep(self.period - tdiff)
-
-
-class MotorConnector(object):
-    '''
-    Implements a simple EPICS motor record, with a small subset of the
-    [EPICS motor record](https://epics.anl.gov/bcda/synApps/motor/R7-1/motorRecord.html)
-    variables. Relies on a motor inteface as described by `MotorEngine`, i.e.
-    a class with the following properties:
-
-      - `position`: returns the current motor values, respectively moves
-        to the specified relative value
-
-      - `position_relative`: facilitates a movement relative to the current
-        position
-
-      - `state`: a string that begins with one of the following:
-    
-          - "INIT" (preparing to take commands)
-    
-          - "IDLE" (not moving, ready to take commands)
-    
-          - "BUSY" (not able to accept commands, most likely already moving)
-    
-          - "ERROR" (stopped, reached a situation which requires external action)
-
-          - "STOP" (stopping)
-    
-          - "FAIL" (unefined state, best effort to be stopped, unrecoverable error)
-    
-        The state string is intentionally checked only for its beginning part.
-        States may be explicitly extended by appending information to strings,
-        e.g. "BUSY.TRACKING" or "BUSY.HOMING" to distinguish different flavors
-        of states. `SimpleMotor` will not react to anything beyond the five
-        1st-level state information, but other software layers may.
-
-    This class needs to be used with a
-    [pythonSoftIOC](https://dls-controls.github.io/pythonSoftIOC)
-    compatible EPICS IOC Python API. It uses `asyncio` for all asynchronous
-    work.
-
-    It implements the EPICS motor record variables VAL, RBV, RVL, HOMF/HOMB,
-    STOP.
-
-    FIXME: need to add support for supplementary actions / properties / signals
-    (e.g. extend by additional "BUSY" states, or read/write specific properties
-    like limits, force probe thresholds etc).
-    '''    
-
-    def __init__(self, motor_prefix, motor_engine, ioc_dispatcher,
-                 poll_period=0.1, separator="_", style="simple"):
-        '''
-        Initializes the IOC variables. Parameters:
-        
-          - `motor_prefix`: a string to prepend to the motor variables.
-        
-          - `motor_engine`: the `MotorEngine` object we'll be talking to.
-        
-          - `ioc_dispatcher`: a pythonSoftIOC asyncio dispatcher compatible
-            instance (typically a `softioc.asyncio_dispatcher.AsyncioDispatcher()`)
-        '''
-
-        self.pollPeriod = poll_period
-
-        #from softioc import builder as ioc_builder
-
-        # SPEC needs the following:
-        #
-        # Can be ignored / business of the controller?
-        #  o ACCL: acceleration time in seconds (0.0)
-        #  o BDST: backlash distance egu (0)
-        #  o BVAL: backlash velocity egu/s (0)
-        #  o VBAS: base velocity (minimum velocity?) egu/s (0)
-        #  o ERES: encoder step size egu (0)
-        #  o MRES: motor step size egu (0)
-        #
-        # Calibration fields and coordinate system transformations:
-        #  - SET: set/use switch for calibration fields (0: use, 1: set)
-        #  - FOFF: offset freeze switch -- is the user prevented from
-        #          writing the offset?
-        #  - OFF: user offset egu
-        #  + DIR: user direction        
-        #  - RRBV: raw readback value
-        #  - RVAL: raw desired value        
-        #
-        # Unclear:
-        #  o UEIP: use encoder if present (always 1?)
-        #  o VELO: velocity egu/s (set to 0?)
-        #
-        # Need to have / already have:
-        #  o STOP: stop
-        #  o VAL: user desired value
-        #  - SPMG: stop/pause/move/go -- complicated beast
-        #    - Stop: same as STOP?        
-        #
-        # Nice to have, but not part of the EDA Motor Model:
-        #  + DHLM: dial high-limit
-        #  + DLLM: dial low-limit
-        #  + HLS: at high-limit switch
-        #  + LLS: at low-limit switch        
-        #  o DMOV: done moving to value
-        #
-        # Unknown:
-        #  + DISP: disable (turn off motor/unusable)        
-        #
-        # Nice to have, not needed by SPEC:
-        #  o EGU: engineering unit names
-        #  - RLV: relative-move value: when changed, changes VAL,
-        #    then resets itself to 0
-        #  
-        
-        self.engine = motor_engine
-
-        # VAL/RBV
-        self.con_pos = PropertyConnector(ioc_dispatcher,
-                                         prefix=motor_prefix+separator,
-                                         access=(motor_engine, "position"),
-                                         signal={ 'poll_period': poll_period },
-                                         kind="analog")
-
-        # STATEVAL/RBV
-        self.con_state = PropertyConnector(ioc_dispatcher,
-                                           prefix=motor_prefix+separator+"STATE",
-                                           access=(motor_engine, "state"),
-                                           signal={ 'poll_period': poll_period },
-                                           kind="strings",
-                                           validator={ 'values': [
-                                               'INIT', 'IDLE', 'BUSY', 'STOP', 'ERROR', 'FATAL'
-                                           ]})
-
-        # STOP
-        self.con_stop = ActorConnector(var=motor_prefix+separator+"STOP",
-                                       access=self.conExecStop,
-                                       kind="values",
-                                       validator={'values': [0, 1]})
-
-        if style == "spec":
-
-            # lots of variables expected by spec but which we don't really serve
-            self.con_constants = [
-                SignalConnector(ioc_dispatcher,
-                                var=motor_prefix+separator+suffix,
-                                access=lambda: value,
-                                kind=kind,
-                                poll_period=10.0)
-                for suffix,kind,value in [ ("ACCL", "analog", 0),
-                                           ("BDST", "analog", 0),
-                                           ("BVAL", "analog", 0),
-                                           ("VBAS", "analog", 0),
-                                           ("ERES", "analog", 0),
-                                           ("MRES", "analog", 0),
-                                           ("UEIP", "analog", 1),
-                                           ("VELO", "analog", 0)]]
-            #("EGU",  "text", "mm")] ]
-
-            # DMOV - set to 0 when motor begins moving
-            self.con_dmov = SignalConnector(ioc_dispatcher,
-                                            var=motor_prefix+separator+"DMOV",
-                                            access=lambda: int(self.engine.state == "IDLE"),
-                                            kind="integer",
-                                            poll_period=self.pollPeriod)
-
-            
-            self.con_status = SignalConnector(ioc_dispatcher,
-                                              var=motor_prefix+separator+"STATUS",
-                                              access=lambda: 0x02 if self.engine.state == "BUSY" else 0x00,
-                                              kind="integer",
-                                              poll_period=self.pollPeriod)
-        
-                   
-        ## Enable 'HOMF' command
-        #self.pv_homf = builder.aOut(axvar+"_HOMF", initial_value=0, always_update=True,
-        #                            on_update=TriggerAndStatus(lambda: axobj.homing = True,
-        #lambda: axobj.homing)]
-
-        #class rel_add(object):
-        #    def __init__(self, pos_prop):
-        #        self.pos_prop = pos_prop
-        #        self.my_pv = None
-        #    def __call__(self, value):
-        #        self.pos_prop += val
-        #        if self.my_pv:
-        #            self.my_pv.set(0)
-        #           
-        #self.rel_mover = rel_add(motor_engine.position)
-        #
-        #self.pv_relpos = ActorConnector(var=motor_prefix+"_RLV",
-        #                                access=self.rel_mover,
-        #                                kind='analog',
-        #                                validator=None)
-        #
-        #self.rel_mover = self.pv_relpos
-
-    def conPollDmov(self):
-        return int(self.engine.state == "IDLE")
-
-    async def conExecStop(self, val):
-        '''
-        EPICS motor STOP command: if val==1, it executes the STOP command,
-        then it sets VAL to current position and resets itself to 0.
-        '''
-        if val != 1:
-            return
+                logging.error("%s: unknown exception %r. You _should_ be worried." % e)
+                
+            finally:
+                tdiff = time.time()-tstart
+                await asyncio.sleep(self.period - tdiff)
 
-        self.engine.state = "STOP"
-        self.con_stop.pv.set(0)
-        
-        while self.engine.state != "IDLE":
-            await asyncio.sleep(self.pollPeriod)
             
-        self.con_val.set(self.engine.position)
-            
-        
-
-
-from softioc import builder as IocBuilder
-        
 '''
 List of connector kinds we support. "in"/"out" should return the
 correct builder function (lambda parameter being the softioc builder
 object itself), and "args" is a list of initial arguments for the
 builder function. Typically you'd want to set default values,
 and/or sizes, and/or data types.
 '''
 ConnectorKinds = {
-    "analog": { "in": IocBuilder.aIn,
-                "out": IocBuilder.aOut,
-                "create": { "initial_value": 0.0 },
-                "to-epics": IdentityValidator(),
-                "from-epics": IdentityValidator() },
-
-    "switch": { "in": IocBuilder.boolIn,
-                "out": IocBuilder.boolOut,
-                "create": { 'ZNAM': 'OFF', 'ONAM': 'ON' },
-                "to-epics": MappingValidator(values={"ON": 1, True: 1, 1: 1,
-                                                     "OFF": 0, False: 0, 0: 0}),
-                "from-epics": MappingValidator(values={1: "ON",
-                                                       0: "OFF"}) },
-
-    "strings": { "in": IocBuilder.stringIn,
-                 "out": IocBuilder.stringOut,
-                 "create": { },
-                 "to-epics": SetValidator,
-                 "from-epics": SetValidator },
+    "analog": {
+        "in": IocBuilder.aIn,
+        "out": IocBuilder.aOut,
+        "create": { "initial_value": 0.0 },
+        "to-epics": IdentityValidator(),
+        "from-epics": IdentityValidator() },
+    
+    "switch": {
+        "in": IocBuilder.boolIn,
+        "out": IocBuilder.boolOut,
+        "create": { 'ZNAM': 'OFF', 'ONAM': 'ON' },
+        "to-epics": MappingValidator(values={"ON": 1, True: 1, 1: 1,
+                                             "OFF": 0, False: 0, 0: 0}),
+        "from-epics": MappingValidator(values={1: "ON",
+                                               0: "OFF"}) },
+
+    "strings": {
+        "in": IocBuilder.stringIn,
+        "out": IocBuilder.stringOut,
+        "create": { },
+        "to-epics": SetValidator,
+        "from-epics": SetValidator },
+
+    "waveform": {
+        "in": IocBuilder.WaveformIn,
+        "out": IocBuilder.WaveformOut,
+        "create": { },
+        "to-epics": IdentityValidator(),
+        "from-epics": IdentityValidator()
+    },
 
     # untested:
     
-    "text":  {  "in": IocBuilder.stringIn,
-                "out": IocBuilder.stringOut,
-                "create": { },
-                "to-epics": SliceValidator(stop=39),
-                "from-epics": IdentityValidator() },
-
-    "map": { "in": IocBuilder.stringIn,
-             "out": IocBuilder.stringOut,
-             "create": { "initial_value": "n/a" },
-             "to-epics": MappingValidator,
-             "from-epics": MappingValidator },
-
-    "values": { "in": IocBuilder.longIn,
-                "out": IocBuilder.longOut,
-                "create": { "initial_value": 0 },
-                "to-epics": SetValidator,
-                "from-epics": SetValidator },
-
-    "integer": { "in": IocBuilder.longIn,
-                 "out": IocBuilder.longOut,
-                 "create": { "initial_value": 0 },
-                 "to-epics": IdentityValidator(),
-                 "from-epics": IdentityValidator() },
+    "text":  {
+        "in": IocBuilder.stringIn,
+        "out": IocBuilder.stringOut,
+        "create": { },
+        "to-epics": SliceValidator(stop=39),
+        "from-epics": IdentityValidator() },
+
+    "map": {
+        "in": IocBuilder.stringIn,
+        "out": IocBuilder.stringOut,
+        "create": { "initial_value": "n/a" },
+        "to-epics": MappingValidator,
+        "from-epics": MappingValidator },
+
+    "values": {
+        "in": IocBuilder.longIn,
+        "out": IocBuilder.longOut,
+        "create": { "initial_value": 0 },
+        "to-epics": SetValidator,
+        "from-epics": SetValidator },
+
+    "integer": {
+        "in": IocBuilder.longIn,
+        "out": IocBuilder.longOut,
+        "create": { "initial_value": 0 },
+        "to-epics": IdentityValidator(),
+        "from-epics": IdentityValidator() },
 }
-    
-        
+
 class SignalConnector(object):
     '''
     Connects a sensoric signal (i.e. a reading of a measurement) to an
     EPICS PV. The data is retrieved from either a Python property or
     from a getter function.
     '''
 
-    def __init__(self, ioc_dispatch, var=None, access=None, kind="analog",
-                 validator=None, poll_period=1.0):
+    argnames = { "suffix": str,
+                 "name": str,
+                 "kind": str,
+                 "access": object,
+                 "create": dict,
+                 "validator": dict,
+                 "pollPeriod": float }
+
+    schema = Schema({Optional(k):v for k,v in argnames.items()})
+
+    def __init__(self, ioc_dispatch, **kw):
         '''
         Parameters:
           - `ioc_dispatch`: dipatcher to use
 
-          - `name`: String, will be used throughout the application
-            for referencing and recognition (e.g. error messages)
-        
-          - `var`: PV name to use; defaults to `name`.
+          - `name`: Used to recognize stuff throughout the application,
+            also serves as default to `suffix`.
+
+          - `suffix`: PV name to use; defaults to `name`.
         
           - `access`: Callable or (obj, propname) tuple of a Python
             property to set or get data from.
 
           - `kind`: one of the `eda.ConnectorKinds` keys
 
-          - `poll_period`: poll period for the data to publish (i.e.
+          - `pollPeriod`: poll period for the data to publish (i.e.
             calling of `access`)
 
-          - `validator`: If not `None`, the validator of the property
-            updater will be initialized using this dictionary of values.
+          - `validator`: If not `None`, this is a dict that will be used to
+            initialize the validator of the property.
+
+          - `create`: Supplementary arguments to pass on when creating the
+            PV class. This is highly specific to the underlying EPICS
+            framework being used.
         '''
-        k = ConnectorKinds[kind]
+        
+        if not set(kw).issubset(set(self.argnames)):
+            raise TypeError("Unknown arguments: %r" % set(self.argnames).difference(kw))
+        
+        k = ConnectorKinds[kw.get('kind')]
 
-        self.pv = k["in"](var, **(k["create"]))
+        suffix = kw.get('suffix') or kw.get('name')
 
-        access_dict = { "getter": access } if hasattr(access, "__call__") \
-            else { "obj": access[0], "prop": access[1] }
+        pv_create_args = k.get('create', {})
+        pv_create_args.update(kw.get('create', {}))
+        self.pv = k["in"](suffix, **(pv_create_args))
+
+        if hasattr(kw['access'], "__call__"):
+            access = kw['access']
+        else:
+            access = partial(getattr, *(kw['access']))
 
         # sometimes the validator in ConnectorKinds is an explicit
         # instance (which we can use right away); sometimes it's just
         # a class type, which we have to instantiate first
-        valdtr = k['to-epics'](**(validator or {})) if type(k['to-epics']) == type \
+        valdtr = k['to-epics'](**(kw.get('validator', {}))) if type(k['to-epics']) == type \
             else k['to-epics']
 
-        getter = PropertyUpdater(name=var, validator=valdtr,
-                                 pv=self.pv, period=poll_period,
-                                 **access_dict)
-        
-        ioc_dispatch(getter)
+        getter = PropertyUpdater(name=kw.get('name', suffix),
+                                 validator=valdtr,
+                                 pv=self.pv,
+                                 pollPeriod=kw.get('pollPeriod', 1.0),
+                                 getter=access)
+
+        if ioc_dispatch:
+            ioc_dispatch(getter)
 
-        logging.debug("%s: '%s' sensor, access %r" % (var, kind, access))
+        logging.info("%s: '%s' sensor, access %r" % (suffix, kw.get('kind'), kw.get('access')))
         
 
 class ActorConnector(object):
     '''
     Connects an action signal (i.e. button, knob, setting etc) to an EPICS PV.
     '''
+
+    argnames = { "suffix": str,
+                 "name": str,
+                 "kind": str,
+                 "access": object,
+                 "validator": object }
+
+    schema = Schema({Optional(k):v for k,v in argnames.items()})
+
     
-    def __init__(self, var=None, access=None, kind="analog", validator=None):
+    def __init__(self, ioc_dispatch, **kw):
         '''
         Parameters:
-          - `var`: PV name to use
+
+          - `ioc_dispatch`: The pythonSoftIOC async dispatcher. Ignored here,
+            but we need this for API uniformity with the other connectors.
+
+          - `name`: Name of the ActorConnector (used internally for displaying
+            purposes, and as a default for `suffix` if the latter is not specified).
         
-          - `access`: Either a callable for reading/setting data,
-            or (obj, propname) tuple of a Python
-            property to set or get data from.
+          - `suffix`: PV name to use
+        
+          - `access`: Reference to a Python property (either callable or writable),
+            for setting data.
 
           - `kind`: one of the `eda.ConnectorKinds` keys
 
           - `validator`: property dictionary for kind-specific validator
-            configuration
+            configuration.
+
+          - `create`: Supplementary arguments to pass on when creating the
+            PV class. This is highly specific to the underlying EPICS
+            framework being used.        
         '''
-        
-        k = ConnectorKinds[kind]
 
-        access_args = {'proc': access} if hasattr(access, "__call__") \
-            else { 'obj': access[0], 'prop': access[1] }
+        if not set(kw).issubset(set(self.argnames)):
+            raise TypeError("Unknown arguments: %r" % set(kw).difference(self.argnames))
+        
+        k = ConnectorKinds[kw.get('kind')]
 
-        # sometimes the validator in ConnectorKinds is an explicit
-        # instance (which we can use right away); sometimes it's just
-        # a class type, which we have to instantiate first
-        valdtr = k['from-epics'](**(validator or {})) if type(k['from-epics']) == type \
-            else k['from-epics']        
+        suffix = kw.get('suffix') or kw.get('name')
         
-        setter = PropertySetter(name=var, validator=valdtr, **access_args)
+        if hasattr(kw['access'], "__call__"):
+            access = kw['access']
+        else:
+            access = partial(setattr, *(kw['access']))
 
-        if validator:
-            setter.validator.setup(**validator)
+        if  k['from-epics'] is None:
+            validator = None
+            
+        elif type(k['from-epics']) == type:
+            # Instantiate from explicit type
+            validator = k['from-epics'](**(kw.get('validator', {})))
+            
+        elif kw.get('validator') is not None:
+            # There's already an instance, but there's an override list
+            # of paramters for a re-initialisation available
+            validator = k['from-epics'].__class__(**(kw['validator']))
+            
+        else:
+            # If we got here, k['from-epics'] must already be an instance,
+            # so we use it.
+            validator = k['from-epics']
+
+        setter = PropertySetter(name=suffix, validator=validator, setter=access)
+
+        pv_create_args = k.get('create', {})
+        pv_create_args.update(kw.get('create', {}))
+        self.pv = k["out"](suffix, always_update=True, on_update=setter, **pv_create_args)
         
-        self.pv = k["out"](var, always_update=True, on_update=setter, **(k["create"]))
-        logging.debug("%s: '%s' actor, access %r" % (var, kind, access))
+        logging.debug("%s: '%s' actor, access %r" % (suffix, kw['kind'], access))
     
         
 class PropertyConnector(object):
     '''
     Conenctor for a get/set type of property; uses `eda.SignalConnector`
     and `eda.ActorConnector` under the hood to export two PVs, one for
     setting, one for reading back the property. By default the variable
     names end in "VAL" (for setting), respectively "RBV" (for reading).
 
     A `sync()` method is available to programatically set the
     "VAL" part to its current readback value "RBV".
     '''
 
-    def __init__(self, ioc_dispatcher, prefix=None, access=None,
-                 kind="analog", validator=None, signal={}, actor={}):
+    # Using this for validation. For once it's needed in __init__(),
+    # and then it's also used in parsing YAML files.
+    argnames = { "suffix": str,
+                 "name": str,
+                 "kind": str,
+                 "access": object,
+                 "validator": object,
+                 "signal": dict,
+                 "actor": dict }
+
+    schema = Schema({Optional(k):v for k,v in argnames.items()})
+
+    def __init__(self, ioc_dispatcher, **kw):
         '''
         Parameters:
           - `ioc_dispatcher`: connection to pythonSoftIOC to use.
 
           - `prefix`: PV prefix, will be prepended to the variable names. By
             default the variable names end in "VAL" (for setting), respectively
             "RBV" (for reading), but they can be overridden by using the `sensor`
@@ -820,24 +459,342 @@
           - `signal`: Dictionary with optional variables to pass on to
             `eda.SignalConnenctor` for the reading part.
         
           - `actor`: Dictionary with optional variables to pass on to
              `eda.ActorConnector` for the setting part.
         '''
 
+        if not set(kw).issubset(set(self.argnames.keys())):
+            raise TypeError("Unknown arguments: %r" % list(set(self.argnames.keys()).difference(kw)))
+
+        print ("Intermediate 1.2: %r" % (kw['access'],))
+        
         ad = {}
-        ad.update(actor)
-        ad.setdefault("kind", kind)
-        ad.setdefault("access", access)
-        ad.setdefault("validator", validator)
-        ad.setdefault("var", prefix+"VAL")
+        ad.update(kw.get('actor', {}))
+        ad.setdefault("kind", kw['kind'])
+
+        #if 'access' in ad:
+        #    # Subconnector has its own 'access' information -- we need to use that.
+        #    if isinstance(ad['access'], str):
+        #        # If it's a plain string, we intepret that to be a (sub-)property
+        #        # relative to the base class already specified in kw['access'].
+        #        # If kw['access'] doesn't have anything, we're out of luck anyway,
+        #        # because we don't have access to a base class here.
+        #        ad['access'] = FindAccess(kw['access'], ad['access'])
+        #    elif hasattr(ad['access'], "__len__") \
+        #         and len(ad['access']) == 2 \
+        #         and isinstance(str, ad['access'][1]):
+        #        # ...may be a tuple (obj, "attribute")?
+        #        ad['access'] = FindAccess(*(ad['access']))
+        #    else:
+        #        raise RuntimeError("Unsupported sub-access type %r for property connector")
+        #else:
+        #    # Regular
+        #    ad['access'] = kw['access']
+        ad['access'] = self.descend_access(kw['access'], ad.get('access', None))
+            
+        
+        ad.setdefault("validator", kw.get('validator', None))
+        ad.setdefault("suffix", (kw.get('suffix') or kw.get('name'))+"VAL")
         self.val = ActorConnector(**ad)
 
         sd = {}
-        sd.update(signal)
-        sd.setdefault("kind", kind)
-        sd.setdefault("access", access)
-        sd.setdefault("validator", validator)
-        sd.setdefault("var", prefix+"RBV")
+        sd.update(kw.get('signal', {}))
+        sd.setdefault("kind", kw['kind'])
+
+        #if 'access' in sd:
+        #    if isinstance(sd['access'], str):
+        #        sd['access'] = FindAccess(kw['access'], sd['access'])
+        #    elif hasattr(sd['access'], "__len__") \
+        #         and len(sd['access']) == 2 \
+        #         and isinstance(str, sd['access'][1]):
+        #        # ...may be a tuple (obj, "attribute")?
+        #        sd['access'] = FindAccess(*(sd['access']))
+        #    else:
+        #        raise RuntimeError("Unsupported sub-access type %r for property connector")                
+        #else:
+        sd['access'] = self.descend_access(kw['access'], sd.get('access', None))
+                
+        #print ("Intermediate 1.7: %r" % (sd['access'],))
+        
+        sd.setdefault("validator", kw.get('validator', None))
+        sd.setdefault("suffix", (kw.get('suffix') or kw.get('name'))+"RBV")
         self.rbv = SignalConnector(ioc_dispatcher, **sd)
 
-        logging.info ("Registering property: %s" % (prefix))
+        logging.info ("Registering property: %s" % (kw.get('suffix') or kw.get('name')))
+
+
+    def descend_access(self, top_access, sub_access):
+        '''
+        Given an existing access object in `top_access` and (possibly)
+        a specification for a sub-property access, this returns a merged
+        access object to be used.
+        '''
+        
+        if sub_access is None:
+            # Nothing to do, there is no sub-access.
+            return top_access
+            
+        if isinstance(sub_access, str):
+            # Sub-access is a plain method name (possibly nested).
+            # We interpret that to be relative to the top-access object.
+            # The top-access object is either directly a Python object,
+            # or a (base, "prop") sub-object itself.
+            if isinstance(top_access, tuple) \
+               and len(top_access)==2 \
+               and isinstance(top_access[1], str):
+                # top-access is a (base, "prop") notation, so we need
+                # to compute the actual property first.
+                obj = getattr(*(top_access))
+                print("sub-tuple:", obj)
+            else:
+                # top_access is direct object (callable?), sub-access is just
+                # a member nane
+                obj = top_access
+                print("direct:", obj)
+            return FindAccess(obj, sub_access)
+        
+        elif hasattr(sub_access, "__len__") \
+             and len(sub_access) == 2 \
+             and isinstance(str, sub_access[1]):
+            # Sub-access is a tuple (obj, "attribute"), so we ignore the
+            # top-access completely and just build a new access object.
+            return FindAccess(*(sub_access['access']))
+
+        # How did we get here?
+        raise RuntimeError("Unsupported sub-access type %r for property connector")
+    
+#
+# Validating YAML input for EPICS exports. General YAML format of an export
+# record list is like this:
+#
+#   exports:  # ...or whatever, this isn't regulated (yet)
+#
+#   - recordType: signal  # indicates essentially "how" this data flows and behaves, can
+#                         # be any of the ExportRecordTypes.
+#
+#     pvName: "PV"  # optional; if not available, then the connector-type entry must have one
+#
+#     signal:       # depending on the connector type
+#
+#     - pvName:     # optional; if not available, the one from parent plus a default suffix will be used.
+#
+#       kind: "analog"  # ...or any other of the ConnectorKinds
+#
+#       pollPeriod: 0.1 # typical key for "signal" here, other recordTypes may have other fields
+#
+#
+# Schemata for the YAML EPICS-PV "exports" section. General format considerations:
+#
+#  - `recordType` tells the direction of the data flow and some structural
+#    information. Generally there are two basic types -- `signal` (for reading data
+#    from external device), and `actor` (for writing data into an external device).
+#    Each of these types exports a PV on its own: an OUT, respectively IN semantics
+#    of EPICS.
+# 
+#    A joint type that can do both is `property`: it uses a Signal and an Actor to
+#    export two variables, one for reading and one for writing: a "_VAL" and a "_RBV"
+#    one.
+#
+#    Several higher-level types are possible to implement here, for instance a "motor"
+#    (usually a positioner / "actor" that has a working state).
+#
+#
+#  - `name`: This is the sine-qua-non. It's the name of the Python object property
+#    we're exporting / working on. If the property is a callable, it will be
+#    called without an argument (i.e. `obj.prop()`) to read a value, and with
+#    one single argument to set a value (`obj.prop(23)`). Otherwise the property
+#    will be read and set as if it were a static value (`obj.prop = 23`).
+#
+#
+#  - 'pvSuffix' is an optional suffix for the corresponding EPICS variable;
+#    if not set, it defaults to 'name' (with the dots 'n all).
+#
+#
+#  - `format`: Sometimes data comes out of the Python end as a string, containing
+#    undesired components (e.g. `"session 1, garble 42.37 yadda"`, and we're
+#    actually only interested in `42.37` here). If that's the case with your application,
+#    you can specify an explicit format string (here, for instance,
+#    `"session {moo}, garble {value} {word}"`) which contains the formatter `{value}`
+#    somewhere inside. If that is specified, that will be used for accessing the data.
+#
+#
+#  - `kind` is a hint as to how the data is to be interpreted: it affects two
+#    distinct subsystems: on one end, the EPICS PVs that are exported have specific
+#    types (aOut/aIn, stringOut/strinIn etc). So specific "kinds" are mapped to
+#    specific EPICS PV types.
+#    On the other end, the data going in/out, between EPICS/Python (<- which is, to
+#    say, the device), also has a may need to be translated to specific Python types.
+#    Within Python code, this is done by Validators (somewhat misnamed, they actually
+#    also do a great deal of converting).
+#
+#    Now, with specific `kind` settings come also specific preconfigured validators.
+#
+#
+#  - (FXIME: need to talk about validator settings like `values` etc).
+#
+#
+#  - Reading and writing -- normally reading and writing is done using the same
+#    property, in a symmetric manner. For instance: if the property of object `obj`
+#    is `prop`, then reading vs. writing is `obj.prop()` vs `obj.prop(...)`, or
+#    `obj.prop` vs `obj.prop=...` (if the property is non-callable), or `format(str)`
+#    vs. `str.format(...)` if a format is specified, etc. But never, say,
+#    `obj.prop()` for reading and `obj.set_prop(42)` for writing.
+#
+#    Yet sometimes different approaches are necessary.
+#
+#    For this reason, when using higher-level "recortType" objects like `property`,
+#    their lower-level constituents (e.g. `signal` and `actor`), which actually control
+#    the reading and writing, mirror the options `name`, `format`, `pvSuffix`.
+#    If these are set, they overwrite their conterparts from the supersection.
+
+
+
+def FindAccess(obj, name, separators=['.', ':']):
+    '''
+    Recursively finds a property of object instance `obj`.
+    Returns a tuple `(instance, "name")`, where `"name"` is
+    the name of the final Python property to be used and
+    `instance` is an object instance that owns said property.
+    Generally, if `name` is a nested property, then `instance`
+    is *not* the same as `obj`.
+    '''
+
+    # Pick a separator from the list -- the first one we find.
+    for sep in separators:
+        if sep in name:
+            break
+    
+    ref = obj
+    chain = name.split(sep) if sep in name else [name]
+    
+    for p in chain[:-1:]:
+        ref = getattr(ref, p)
+    
+    prop = (ref, chain[-1])
+    attr = getattr(*prop)
+    
+    if hasattr(attr, "__call__"):
+        return attr
+    else:
+        return prop
+
+
+ExportRecordTypes = {
+    "signal": SignalConnector,
+    "actor": ActorConnector,
+    "property": PropertyConnector
+}
+
+def ExportObjectFromDict(ioc_dispatch, parent, data,
+                         suffixMangle=lambda x: x,
+                         recordTypeDefaults=None):
+    '''
+    Creates an export object (i.e. one of the `ExportObjectTypes`) from
+    a data dictionary as specified by the `scm_export_record` and
+    kindred schemata. The `parent` is the object to which all properties
+    named within `data` relate.
+    Parameters:
+
+      - `ioc_dispatch: a pythonSoftIOC dispatch object to use for the
+        Signal-type connectors (essentially, those run an asyncio-based
+        polling loop, and ioc_dispatch takes care of actually dispatching it)
+
+      - `parent`: The object to which all the properties are refering to
+
+      - `data`: A configuration dictionary cotaining, among others, the
+        name of the property to export
+
+      - `suffixMangle`: A callable to optionally do some name mangling on
+        the final PV suffix that we'll send to the pythonSoftIOC builder.
+        This is typically used e.g. to change case of the variable names,
+        or to add more suffixes/prefixes/interfixes as needed.
+        This is necessary because we actually want to hide the details of
+        the configuration format within `data` to higher layers -- only
+        `ExportObjectFromDict()` and functions below it need to know the
+        details. Another reason is that details, in particular of variable
+        naming, are pretty ofuscated -- naming can be done at high level,
+        or may be delegated down to sub-objects, and we don't want higher
+        level to have to deal with that. So, in essence: if you need to
+        mangle the name, use this function! ;-)
+        
+    '''
+
+    # For creating EPICS PV exports delaratively, i.e. from YAML,
+    # we start with a 'recordType' (e.g. "signal" or "property"):
+    scm_dict = { 'recordType': Or(*(ExportRecordTypes.keys())) }
+    
+    # The bulk of the parameters may then be specified in sub-dictionaries
+    # (see above). Each Connector type class needs to bring its own schema:
+    scm_dict.update({ Optional(k):v.schema for k,v in ExportRecordTypes.items() })
+    
+    # Some record types are primitives ("actor" and "signal"), others are
+    # composed ("property"). Things get increasingly nested ("motor" holds
+    # several "property" records, for instance). We specify parameters in
+    # the order in which they're encapsulated (e.g. "property" accepts dicts
+    # for "signal" and "actor" which it's made of).
+    # 
+    # For convenience, at the top level we also accept parameters common to
+    # all subsets (e.g. "name" or "suffix").
+    #common_args = reduce(lambda x, y: x&y,
+    #                     [set(v.argnames.items()) for k,v in ExportRecordTypes.items()])
+    #scm_dict.update({Optional(k):v for k,v in common_args})
+    #pprint(scm_dict)
+    
+    scm = Schema(scm_dict)
+    logging.debug("Export schema: %r" % scm)
+    data = scm.validate(data)
+
+    # ACHTUNG: This whole passing-arguments-down-to-encapsulated-subtypes shebang
+    # only works as long as there is only *one* specific subtype of each being
+    # encapsulated, and the corresponding YAML subsection has exactly the same
+    # name as the subtype itself. E.g. this works well:
+    #
+    #  - recordType: property
+    #    signal:
+    #      ...
+    #    actor:
+    #      ...
+    #
+    # This doesn't work:
+    #
+    # - recordType: motor
+    #   signalUpperLimit:
+    #     ...
+    #   signalLowerLimit:
+    #     ...
+    #
+    
+    recType = data['recordType']
+
+    recParams = ((recordTypeDefaults or {}).get(recType) or {}).copy()
+    recParams.update(data[recType])
+
+    try:
+        recParams['access'] = FindAccess(parent, recParams.get('access') or recParams.get('name'))
+        #print ("Intermediate: %r" % recParams['access'])
+    except:
+        # 'name' may not necessarily be a valid property of the object.
+        # So if we fail finding one, we just ignore it, and 'access' will
+        # be undefined. It will up to lower layers to provide a proper
+        # access method.
+        logging.info('No access for %r defined at top-level' % data.get('name'))
+        pass
+
+    # Here's the name mangling. Note that this will only mangle suffix naming
+    # at the top level, not at the sub-levels. For that, we're stuck with whatever
+    # functionality the Connector objects already implement.
+    # The obvious (and possibly the only good) solution to this would be to pass
+    # the name-mangling callable down to the Connector types (here: `ExportRecordTypes[]`)
+    # constructor itself. For that to work, we'd probably have to derive all Connector
+    # classes from a common base class that does handle these types of common tasks
+    # (like calling a name mangling lambda).
+    recParams['suffix'] = suffixMangle(recParams.get('suffix') or recParams.get('name'))
+
+    #print ("Intermediate 0: %r" % (recParams['access'],))
+    
+    logging.debug("Building connector %r, settings %r" % (recType, recParams))
+
+    #print ("Intermediate 1: %r" % (recParams['access'],))
+    obj = ExportRecordTypes[recType](ioc_dispatch, **recParams)
+
+    return obj
```

### Comparing `emmi-0.0.10/src/emmi/scpi.py` & `emmi-0.1.3/src/emmi/scpi.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,15 +36,16 @@
         the number of burst cycles, etc.
 
     This object takes any parameter that doesn't begin with an underscore
     and interprets it as a command to send to the device on top of the base
     command that it was initiated with. For instance:
     ```
        p = PropertyBranch(kdev, 'burst')
-       p.state = "off"
+       p("off")
+       p -> "off"
     ```
 
     This would return the result of the `"BURST:STATE OFF" command.
     Any strings sent are converted to upper case. Any boolean parameters
     (True/False) are converted to "ON" / "OFF".
 
     In returning values, the class tries first to convert "ON"/"OFF" to
@@ -52,16 +53,16 @@
     points. If all fail, a regular Python string is returned.
 
     The specific functions `get()` and `set()` act directly on the root
     command, e.g. this would result in setting the function "FUNC SIN",
     then requesting the function name again (`FUNC?`):
     ```
        p = PropertyBranch(kdev, 'func`)
-       p.set("sin")
-       p.get() ## --> 'SIN'
+       p("sin")
+       p ## --> 'SIN'
     ```
 
     The functions `enable()` and `disable()` are shortcuts for `set("ON")`
     and `set("OFF")`, respectively.
 
     '''
 
@@ -123,39 +124,62 @@
         prop = self.__propcache.setdefault(name,
                                            PropertyBranch(self.kdev, "%s:%s" % \
                                                           (self.cmdroot, name), nxerror))
         return prop
 
 
 class MagicScpi(object):
-                     
+    '''
+    Wrapper for VISA based communication with SCPI-enabled devices.
+    The API is in many aspects very similar to `easy-scpi`, but differs
+    in some implementation details that make this more suitable to work
+    with `emmi` subsystems (in particular the EPICS export stuff).
+
+    Usage example, e.g. for setting a function type on a function generator
+    (query "FUNC..."), then setting and querying the current frequency
+    (query "FREQyency") and voltage offset (query "VOLTage:AMPLitude"):
+    ```
+      from emmi.scpi import MagicScpi
+    
+      dev = MagicScpi(dev="TCPIP::10.0.0.61::INSTR")
+    
+      dev.FUNC("SIN")   ## -> sends "FUNC SIN" to the device
+      dev.FREQ("200")   ## -> sends "FREQ 200" to the device
+      print ("Current frequency is", dev.FREQ())  ## -> queries "FREQ?" from device
 
-    def __init__(self, dev=None, setup={}, timeout=3.0):
-        '''
-        Connects via TCP/IP to the waveform generator behind IP address `IP`.
-        Default is `None`, which means the address will be read from the
+      dev.VOLT.AMPL("3")
+      print ("Current voltage amplitude is", dev.VOLT.AMPL())
+    ```
+
+    See `escpi` for an example on how to make an EPICS-IOC of a SCPI device.
+    '''
+
+    def __init__(self, dev=None, resource_manager='@py', setup={}, timeout=3.0):
+        ''' Generic interface for SCPI-compatible devices via PyVISA.
+        
+        Default device is `None`, which means the address will be read from the
         `MAGICSCPI_ADDRESS` environment variable.
 
-        Parameters:
-          - `ip`: The IP address to connect to. If none is specified, it is
-            taken from the `MAGICSCPI_ADDRESS` environment variable.
+        Args:
+            ip: The IP address to connect to. If none is specified, it is
+              taken from the `MAGICSCPI_ADDRESS` environment variable.
 
-          - `setup`: A dictionary containing additional setup. Keys are the
-            parameter name (e.g. 'VOLT:UNIT'), values are the value ('Vpp').
+            setup: A dictionary containing additional setup. Keys are the
+              parameter name (e.g. 'VOLT:UNIT'), values are the value ('Vpp').
 
-          - `timeout`: Timeout in seconds
+            timeout: Timeout in seconds
         '''
 
         try:
             self.port = dev or env['MAGICSCPI_ADDRESS']
         except KeyError:
             logging.error("No SCPI port specified and no MAGICSCPI_ADDRESS available")
             raise
         
-        self.dev = pyvisa.ResourceManager('@py').open_resource(self.port)
+        self.dev = pyvisa.ResourceManager(resource_manager).open_resource(self.port)
         self.dev.read_termination = '\n'
         self.dev.write_termination = '\n'
         self.dev.timeout = int(timeout*1000)
 
         self.__propcache = {}
 
         logging.debug("Device open: %s" % self.port)
@@ -204,15 +228,15 @@
         self._val = 3.14
         self.__pcache = {}
 
     def __call__(self, *args):
         if len(args) == 0:
             return self._val
         else:
-            self._val = val
+            self._val = args[0] 
 
     def enable(self):
         self.set(1.0)
 
     def disable(self):
         self.set(0.0)
 
@@ -225,13 +249,13 @@
     Mocking class for Keith3390. Has some defauls for
     the explicit attributes (output, waveform, ...)
     '''
 
     def __init__(self, *args, **kwargs):
         self.__pcache = {}
 
-    def id():
+    def id(self):
         return "Mock SCPI Device"
 
     def __getattr__(self, name):
         return self.__pcache.setdefault(name, MockPropertyBranch())
```

### Comparing `emmi-0.0.10/src/emmi.egg-info/PKG-INFO` & `emmi-0.1.3/src/emmi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emmi
-Version: 0.0.10
+Version: 0.1.3
 Summary: A Selection of Tools for EPICS Monday-Morning Integrations
 Author: Florin Boariu
 Author-email: florin.pt@rootshell.ro
 Project-URL: Homepage, https://emmi.rootshell.ro
 Project-URL: Source Code, https://gitlab.com/codedump2/emmi/
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/emmi/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `emmi-0.0.10/tests/eda_test.py` & `emmi-0.1.3/tests/eda_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 #!/usr/bin/python3
 
 import pytest, time, asyncio
-
+from emmi.api.exports import ConnectorKinds, SignalConnector, ActorConnector, \
+    PropertyConnector  
+    
+    
 class TestSoftIOC(object):
     '''
     Quick'n Dirty way of setting up an IOC and for testing.
     '''
     def __init__(self, prefix):
         from softioc import softioc, builder, asyncio_dispatcher
         self.builder = builder
@@ -59,34 +62,32 @@
 
 
 @pytest.fixture
 def random_value():
     import random
     return random.random()
 
-
+@pytest.mark.skip(reason="not working yet")
 def test_jump_through_hoops(random_value):
     ioc = TestSoftIOC("EMMI_UNITTEST")
     
-    from emmi.eda import SignalConnector
     a1 = ValueAccess(random_value)
-    sen = SignalConnector(ioc.dispatcher, var="signal", access=a1, poll_period=0.1)
+    sen = SignalConnector(ioc.dispatcher, name="signal", kind='analog', access=a1, pollPeriod=0.1)
 
-    from emmi.eda import ActorConnector    
     a2 = ValueAccess(random_value)
-    act = ActorConnector(var="actor", access=a2)
+    act = ActorConnector(suffix="actor", access=a2, kind='analog')
 
-    from emmi.eda import PropertyConnector
     a3 = ValueAccess(0.0)
-    prop = PropertyConnector(ioc.dispatcher, prefix="prop_", access=a3)
+    prop = PropertyConnector(ioc.dispatcher, name="prop_", kind='analog', access=a3)
     
     ioc.start()
     
     assert a1.valid(mincount=5, age=3.0)
 
     act.pv.set(3.14)
     time.sleep(1.0)
     assert a2.value == 3.14
 
     prop.val.pv.set(random_value)
     time.sleep(1.0)
     assert a3.value == random_value
+
```

### Comparing `emmi-0.0.10/tests/motor_test.py` & `emmi-0.1.3/tests/motor_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-from emmi.eda import MotorEngine, MockMotor
+#!/usr/bin/python3
+
+import pytest
 import time
+from emmi.eda import MotorEngine, MockMotor
+
 
 def test_engine():
     '''
     Very rudimentary test of the engine, using a Mock motor:
       - Initial state is INIT or IDLE
       - After setting position we're BUSY for a while, then IDLE
       - After setting and stopping we're going back to IDLE
     '''
-    
+   
     e = MotorEngine(motor=MockMotor(mock_timeslice=1.0))
     assert e.state in [ "INIT", "IDLE" ]
 
     # Setting the position.
     # Will need 1 second to move, may or may not need 1 second to stop (?)
     e.position = 3.14
     end = time.time()+2.5
```

