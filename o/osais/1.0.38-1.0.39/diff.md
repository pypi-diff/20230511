# Comparing `tmp/osais-1.0.38.tar.gz` & `tmp/osais-1.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-69e1mk0y\osais-1.0.38.tar", last modified: Wed Apr 19 09:40:34 2023, max compression
+gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-ywuybe2v\osais-1.0.39.tar", last modified: Wed May 10 16:57:15 2023, max compression
```

## Comparing `osais-1.0.38.tar` & `osais-1.0.39.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 09:40:34.524410 osais-1.0.38/
--rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.38/LICENSE
--rw-rw-rw-   0        0        0     1113 2023-04-19 09:40:34.524410 osais-1.0.38/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-04-05 15:00:45.000000 osais-1.0.38/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 09:40:34.519408 osais-1.0.38/osais/
--rw-rw-rw-   0        0        0      652 2023-04-19 09:40:02.000000 osais-1.0.38/osais/__init__.py
--rw-rw-rw-   0        0        0    42485 2023-04-19 09:39:54.000000 osais-1.0.38/osais/osais.py
-drwxrwxrwx   0        0        0        0 2023-04-19 09:40:34.522410 osais-1.0.38/osais.egg-info/
--rw-rw-rw-   0        0        0     1113 2023-04-19 09:40:34.000000 osais-1.0.38/osais.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-04-19 09:40:34.000000 osais-1.0.38/osais.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 09:40:34.000000 osais-1.0.38/osais.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-19 09:40:34.000000 osais-1.0.38/osais.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 09:40:34.000000 osais-1.0.38/osais.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.38/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 09:40:34.524410 osais-1.0.38/setup.cfg
--rw-rw-rw-   0        0        0     1124 2023-04-19 09:40:17.000000 osais-1.0.38/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:57:15.359558 osais-1.0.39/
+-rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.39/LICENSE
+-rw-rw-rw-   0        0        0     1113 2023-05-10 16:57:15.359558 osais-1.0.39/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-04-05 15:00:45.000000 osais-1.0.39/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 16:57:15.353557 osais-1.0.39/osais/
+-rw-rw-rw-   0        0        0      697 2023-05-10 16:56:35.000000 osais-1.0.39/osais/__init__.py
+-rw-rw-rw-   0        0        0    48893 2023-05-10 16:55:35.000000 osais-1.0.39/osais/osais.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:57:15.358557 osais-1.0.39/osais.egg-info/
+-rw-rw-rw-   0        0        0     1113 2023-05-10 16:57:15.000000 osais-1.0.39/osais.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-05-10 16:57:15.000000 osais-1.0.39/osais.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 16:57:15.000000 osais-1.0.39/osais.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-10 16:57:15.000000 osais-1.0.39/osais.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 16:57:15.000000 osais-1.0.39/osais.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.39/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 16:57:15.359558 osais-1.0.39/setup.cfg
+-rw-rw-rw-   0        0        0     1124 2023-05-10 16:56:51.000000 osais-1.0.39/setup.py
```

### Comparing `osais-1.0.38/LICENSE` & `osais-1.0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `osais-1.0.38/PKG-INFO` & `osais-1.0.39/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.38
+Version: 1.0.39
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.38/osais/__init__.py` & `osais-1.0.39/osais/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 A package for OSAIS virtual AI.
 """
-__version__="1.0.38"
+__version__="1.0.39"
 __author__ = "incubiq"
 __email__ = "eric@incubiq.com"
 
 from .osais import osais_isLocal
 from .osais import osais_loadConfig
 from .osais import osais_getEnv
 from .osais import osais_getHarwareInfo
 from .osais import osais_getDirectoryListing
 from .osais import osais_getInfo
 from .osais import osais_resetGateway
 from .osais import osais_authenticateAI
+from .osais import osais_authenticateClient
 from .osais import osais_initParser
 from .osais import osais_runAI
 from .osais import osais_notify
 from .osais import osais_onNotifyFileCreated
 from .osais import osais_resetOSAIS
 from .osais import osais_initializeAI
```

### Comparing `osais-1.0.38/osais/osais.py` & `osais-1.0.39/osais/osais.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__="1.0.38"
+__version__="1.0.39"
 
 ## ========================================================================
 ## 
 ##                      Utilities starts here 
 ## 
 ## ========================================================================
 
@@ -14,14 +14,15 @@
 import uuid 
 import subprocess as sp
 import pkg_resources
 import os
 import platform
 import ctypes
 import threading
+import boto3
 
 cuda=0                          ## from cuda import cuda, nvrtc
 gObserver=None
 
 ## ------------------------------------------------------------------------
 #       Observer (check updates in directory)
 ## ------------------------------------------------------------------------
@@ -31,21 +32,31 @@
 
 class NewFileHandler(FileSystemEventHandler):
     def __init__(self, fnOnFileCreated, _args):
         self.fnOnFileCreated = fnOnFileCreated
         self._args = _args
 
     def on_created(self, event):
+        global gS3Bucket
+        global gS3
+
         if event.is_directory:
             return
         if event.event_type == 'created':
             ## only notify if uid in the filename (otherwise we are getting notified of another AI's job !)
             if self._args["-uid"] in event.src_path:
                 self.fnOnFileCreated(os.path.dirname(event.src_path), os.path.basename(event.src_path), self._args)
 
+                ## also send to S3
+                if gS3!=None:
+                    # Filename - File to upload
+                    # Bucket - Bucket to upload to (the top level directory under AWS S3)
+                    # Key - S3 object name (can contain subdirectories). If not specified then file_name is used
+                    gS3.meta.client.upload_file(Filename=event.src_path, Bucket=gS3Bucket, Key="output/"+os.path.basename(event.src_path))
+
 def start_observer_thread(path, fnOnFileCreated, _args):
 
     ## watch directory and call back if file was created
     def watch_directory(path, fnOnFileCreated, _args):    
         global gObserver
         if gObserver!=None:
             gObserver.stop()
@@ -367,17 +378,26 @@
 gOriginOSAIS=None               ## location of OSAIS
 
 ## authenticate into a local OSAIS (debug)
 gAuthTokenLocal=None            ## auth token into a local OSAIS (debug) for when working as virtual Ai
 gTokenLocal=None                ## token used for authentication into a local OSAIS (debug)
 gSecretLocal=None               ## secret used for authentication into a local OSAIS (debug)
 gOriginLocalOSAIS=None          ## location of a local OSAIS (debug)
+gClientID=None                  ## ID to authenticate as client into OSAIS (using the ai page to request AI processing)
+gClientSecret=None              ## Pwd to authenticate as client into OSAIS (using the ai page to request AI processing)
+gClientAuthToken=None           ## the resulting Auth token as Client, after login
+gClientAuthTokenLocal=None      ## the resulting Auth token as Client, after login (for debug)
 
 gOriginGateway=None             ## location of the local gateway for this (local) AI
 
+## AWS related
+gS3=None
+gS3Bucket=None
+gAWSSession=None
+
 ## IP and Ports
 gExtIP=get_external_ip()        ## where this AI can be accessed from outside (IP)
 gIPLocal=get_container_ip()     ## where this AI can be accessed locally
 gPortAI=None                    ## port where this AI is accessed (will be set by AI config)
 gPortGateway=3023               ## port where the gateway can be accessed
 gPortLocalOSAIS=3022            ## port where a local OSAIS can be accessed
 
@@ -458,76 +478,119 @@
     global gIPLocal
     global gExtIP
  
     _ip=gExtIP
     if gIsVirtualAI==False:
         _ip=gIPLocal                ## we register with local ip if we are in local gateway mode
 
-    _json=_loadConfig(_name)
+    _jsonAI=_loadConfig(_name)
+    _jsonBase=_loadConfig("osais")
 
     objCudaInfo=getCudaInfo()
     gpuName="no GPU"
     if objCudaInfo != 0 and "name" in objCudaInfo and objCudaInfo["name"]:
         gpuName=objCudaInfo["name"]
 
     return {
         "username": gUsername,
         "os": get_os_name(),
         "gpu": gpuName,
         "machine": get_machine_name(),
         "ip": _ip,
         "port": gPortAI,
-        "engine": _json
+        "config_ai": _jsonAI,
+        "config_base": _jsonBase
     }
 
 ## PUBLIC - are we running locally?
 def osais_isLocal():
     global gIsLocal
     return gIsLocal
 
 ## PUBLIC - load the config of this AI
 def osais_loadConfig(_name): 
     return _loadConfig(_name)
 
 ## PUBLIC - Get env from file (local or docker)
 def osais_getEnv(_filename):
     global gUsername
+    global gDemoID
+    global gDemoSecret
     global gIsVirtualAI
     global gIsLocal
     global gName
+    global gAWSSession
+    global gS3
+    global gS3Bucket
+
+    AWSID=None
+    AWSSecret=None
 
     ## read env from config file
     try:
         with open(_filename, "r") as f:
             content = f.read()
+        print(f'Reading env vars from {_filename}')
         variables = content.split("\n")
         for var in variables:
             if var!="":
                 key, value = var.split("=")
                 if key == "USERNAME":
                     gUsername = value
                 elif key == "IS_LOCAL":
                     gIsLocal = (value=="True")
                 elif key == "IS_VIRTUALAI":
                     gIsVirtualAI = (value=="True")
                 elif key == "ENGINE":
                     gName = value
+                elif key == "S3_BUCKET":
+                    gS3Bucket = value
+                elif key == "AWS_ACCESS_KEY_ID":
+                    AWSID = value
+                elif key == "AWS_ACCESS_KEY_SECRET":
+                    AWSSecret = value
     except Exception as err: 
         print(f'No env file {_filename}')
 
     # overload with env settings if any
     if os.environ.get('IS_LOCAL'):
-        gIsLocal=(os.environ.get('IS_LOCAL')=="True")
+        _isLocal=(os.environ.get('IS_LOCAL')=="True")
+        if _isLocal!=gIsLocal:
+            print(f'is Local updated to {_isLocal} from ENV var')
+            gIsLocal=_isLocal
     if os.environ.get('IS_VIRTUALAI'):
-        gIsVirtualAI=(os.environ.get('IS_VIRTUALAI')=="True")
+        _isVirtualAI=(os.environ.get('IS_VIRTUALAI')=="True")
+        if _isVirtualAI!=gIsVirtualAI:
+            print(f'is Virtual updated to {_isVirtualAI} from ENV var')
+            gIsVirtualAI=_isVirtualAI
     if os.environ.get('ENGINE'):
-        gName=os.environ.get('ENGINE')
+        _name=os.environ.get('ENGINE')
+        if _name!=gName:
+            print(f'Engine name updated to {_name} from ENV var')
+            gName=_name
+    if os.environ.get('S3_BUCKET'):
+        _s3=os.environ.get('S3_BUCKET')
+        if _s3!=gS3Bucket:
+            print(f'Set S3 bucket to {_s3} from ENV var')
+            gS3Bucket=_s3
     if os.environ.get('USERNAME') and gUsername==None:
         gUsername=os.environ.get('USERNAME')
-
+    if os.environ.get('AWS_ACCESS_KEY_ID') and AWSID==None:
+        AWSID=os.environ.get('AWS_ACCESS_KEY_ID')
+    if os.environ.get('AWS_ACCESS_KEY_SECRET') and AWSSecret==None:
+        AWSSecret=os.environ.get('AWS_ACCESS_KEY_SECRET')
+
+    if AWSID!=None and AWSSecret!=None:
+        gAWSSession = boto3.Session(
+            aws_access_key_id=AWSID,
+            aws_secret_access_key=AWSSecret
+        )
+        gS3 = gAWSSession.resource('s3')
+        print(f'Logged into AWS S3')
+        
     return {
         "username": gUsername,
         "isLocal": gIsLocal,
         "isVirtualAI": gIsVirtualAI,
         "name": gName
     }
 
@@ -633,15 +696,16 @@
         "isDocker": gIsDocker,    
         "lastActive_at": gLastChecked_at,
         "lastProcessStart_at": gLastProcessStart_at,
         "machine": gMachineName,
         "owner": gUsername, 
         "isAvailable": (gIsBusy==False),
         "averageResponseTime": _getAverageCost(), 
-        "json": objConf["engine"]
+        "config_ai": objConf["config_ai"],
+        "config_base": objConf["config_base"]
     }
 
 ## ------------------------------------------------------------------------
 #       connect to Gateway
 ## ------------------------------------------------------------------------
 
 # notify the gateway of our AI config file
@@ -777,20 +841,21 @@
             print("We got an authentication token into OSAIS Local (debug)")
             gAuthTokenLocal=objRes["authToken"]    
         except Exception as err:
             return True
 
     return True
 
-
 ## PUBLIC - Authenticate the Virtual AI into OSAIS
 def osais_authenticateAI():
     global gIsVirtualAI
     global gOriginOSAIS
     global gIsScheduled
+    global gDemoID
+    global gDemoSecret
     
     Resp={"data": None}
     if gIsVirtualAI:
 
         try:
             resp= _registerVAI()
             resp=_loginVAI()
@@ -798,18 +863,117 @@
             consoleLog("Exception raised while trying to authenticate to OSAIS")
             raise err
         
         # Run the scheduler
         if gIsScheduled==False:
             gIsScheduled=True
             schedule.every().day.at("10:30").do(_loginVAI)
-
+    
     return resp
 
 ## ------------------------------------------------------------------------
+#       authenticate into OSAIS as Client (user)
+## ------------------------------------------------------------------------
+
+def getClientInfo(_authToken):
+    global gOriginOSAIS
+    global gOriginLocalOSAIS
+
+    headers = {
+        "Content-Type": "application/json",
+        "Authorization": f"Bearer {_authToken}"
+    }
+
+    objRes=None
+    if gIsLocal:        # if local 
+        try:
+            response = requests.get(f"{gOriginLocalOSAIS}api/v1/private/client", headers=headers)
+            objRes=response.json()["data"]            
+        except Exception as err:
+            return {"data": objRes}
+    else:    
+        try:
+            response = requests.get(f"{gOriginOSAIS}api/v1/private/client", headers=headers)
+            objRes=response.json()["data"]            
+        except Exception as err:
+            return {"data": objRes}
+
+    return {"data": objRes}
+            
+
+# Authenticate into OSAIS (as client)
+def osais_authenticateClient(_id, _secret):
+    global gOriginOSAIS
+    global gOriginLocalOSAIS
+    global gClientAuthToken
+    global gClientAuthTokenLocal
+    global gIsLocal
+
+    authToken=None
+
+    headers = {
+        "Content-Type": "application/json"
+    }
+    resp={"data": None}
+    if gIsLocal:        # if local ... log as client into debug
+        try:
+            url=f"{gOriginLocalOSAIS}api/v1/public/client/demo"      ## get a demo auth token
+            if _id!= None:
+                url=f"{gOriginLocalOSAIS}api/v1/public/client/login"
+            response = requests.post(url, headers=headers, data=json.dumps({
+                "token": _id,
+                "secret": _secret
+            }))
+
+            objRes=response.json()["data"]
+            if objRes is None:
+                print("COULD NOT LOGIN AS CLIENT into OSAIS Local")
+            print("We got a CLIENT authentication token into OSAIS Local (debug)")
+            gClientAuthTokenLocal=objRes["authToken"]
+            authToken=gClientAuthTokenLocal
+            resp={"data": {
+                "token": objRes["token"],
+                "authToken": gClientAuthTokenLocal,
+            }}
+
+        except Exception as err:
+            ## no big deal
+            gClientAuthTokenLocal=None
+
+    else:       # else ... log as client into prod        
+        try:
+            url=f"{gOriginOSAIS}api/v1/public/client/demo"      ## get a demo auth token
+            if _id!= None:
+                url=f"{gOriginOSAIS}api/v1/public/client/login"
+            response = requests.post(url, headers=headers, data=json.dumps({
+                "token": _id,
+                "secret": _secret
+            }))
+
+            objRes=response.json()["data"]
+            if objRes is None:
+                print("COULD NOT LOGIN AS CLIENT, stopping it here")
+                sys.exit()
+            print("We got a CLIENT authentication token into OSAIS")
+            gClientAuthToken=objRes["authToken"]    
+            authToken=gClientAuthToken
+            resp={"data": {
+                "token": objRes["token"],
+                "authToken": gClientAuthToken,
+            }}
+
+        except Exception as err:
+            consoleLog("Exception raised while trying to login as CLIENT to PROD")
+            gClientAuthToken=None
+
+    dataClient=getClientInfo(authToken)
+    resp["data"]["user"]=dataClient["data"]["user"]
+    return resp 
+
+## ------------------------------------------------------------------------
 #       Run the AI
 ## ------------------------------------------------------------------------
 
 ## PUBLIC - parse args for OSAIS (not those for AI)
 def osais_initParser(aArg):
     global gArgsOSAIS
     global gInputDir
@@ -1176,19 +1340,21 @@
     print("===== /Config =====\r\n")
 
     ## make sure we have a config file
     _loadConfig(gName)
 
     ## where is OSAIS for us then?
     gOriginGateway=f"http://{gIPLocal}:{gPortGateway}/"         ## config for local gateway (local and not virtual)
+
+    ## we set OSAIS location in all cases (even if in gateway) because this AI can generate it s own page for sending reqs (needs a client logged into OSAIS)
+    if gIsLocal:
+        osais_resetOSAIS(None, f"http://{gIPLocal}:{gPortLocalOSAIS}/")
+    else:
+        osais_resetOSAIS("https://opensourceais.com/", None)
     if gIsVirtualAI:
-        if gIsLocal:
-            osais_resetOSAIS(None, f"http://{gIPLocal}:{gPortLocalOSAIS}/")
-        else:
-            osais_resetOSAIS("https://opensourceais.com/", None)
         try:
             osais_authenticateAI()
         except Exception as err:
             print("=> CRITICAL: Could not connect virtual AI "+gName+ " to OSAIS")
             return None
 
         if gAuthToken!=None:
```

### Comparing `osais-1.0.38/osais.egg-info/PKG-INFO` & `osais-1.0.39/osais.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.38
+Version: 1.0.39
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.38/setup.py` & `osais-1.0.39/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='osais',
-    version='1.0.38',
+    version='1.0.39',
     author='incubiq',
     author_email='eric@incubiq.com',
     description='The osais Python lib for connecting AIs to OSAIS cloud',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/incubiq/osais',
     keywords = "osais, opensourceais",
```

