# Comparing `tmp/pyowletapi-2023.5.7.tar.gz` & `tmp/pyowletapi-2023.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyowletapi-2023.5.7.tar", last modified: Thu May  4 14:42:03 2023, max compression
+gzip compressed data, was "pyowletapi-2023.5.9.tar", last modified: Tue May  9 08:52:39 2023, max compression
```

## Comparing `pyowletapi-2023.5.7.tar` & `pyowletapi-2023.5.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 14:42:03.823992 pyowletapi-2023.5.7/
--rw-rw-rw-   0        0        0     2175 2023-05-04 14:42:03.824991 pyowletapi-2023.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     1353 2023-05-02 10:29:46.000000 pyowletapi-2023.5.7/README.md
--rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyowletapi-2023.5.7/pyproject.toml
--rw-rw-rw-   0        0        0       85 2023-05-04 14:42:03.827004 pyowletapi-2023.5.7/setup.cfg
--rw-rw-rw-   0        0        0      846 2023-05-04 14:41:59.000000 pyowletapi-2023.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 14:42:03.720990 pyowletapi-2023.5.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-04 14:42:03.745989 pyowletapi-2023.5.7/src/pyowletapi/
--rw-rw-rw-   0        0        0       17 2023-05-02 10:29:46.000000 pyowletapi-2023.5.7/src/pyowletapi/__init__.py
--rw-rw-rw-   0        0        0    10013 2023-05-04 14:27:41.000000 pyowletapi-2023.5.7/src/pyowletapi/api.py
--rw-rw-rw-   0        0        0      318 2023-05-03 10:36:51.000000 pyowletapi-2023.5.7/src/pyowletapi/exceptions.py
--rw-rw-rw-   0        0        0     4281 2023-05-04 14:27:51.000000 pyowletapi-2023.5.7/src/pyowletapi/owlet.py
--rw-rw-rw-   0        0        0     7347 2023-05-04 14:37:50.000000 pyowletapi-2023.5.7/src/pyowletapi/sock.py
-drwxrwxrwx   0        0        0        0 2023-05-04 14:42:03.820990 pyowletapi-2023.5.7/src/pyowletapi.egg-info/
--rw-rw-rw-   0        0        0     2175 2023-05-04 14:42:03.000000 pyowletapi-2023.5.7/src/pyowletapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-05-04 14:42:03.000000 pyowletapi-2023.5.7/src/pyowletapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 14:42:03.000000 pyowletapi-2023.5.7/src/pyowletapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-04 14:42:03.000000 pyowletapi-2023.5.7/src/pyowletapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-04 14:42:03.000000 pyowletapi-2023.5.7/src/pyowletapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 08:52:39.392864 pyowletapi-2023.5.9/
+-rw-rw-rw-   0        0        0     2326 2023-05-09 08:52:39.393864 pyowletapi-2023.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1496 2023-05-09 08:51:20.000000 pyowletapi-2023.5.9/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyowletapi-2023.5.9/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-05-09 08:52:39.396865 pyowletapi-2023.5.9/setup.cfg
+-rw-rw-rw-   0        0        0      846 2023-05-09 08:42:29.000000 pyowletapi-2023.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 08:52:39.335864 pyowletapi-2023.5.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 08:52:39.357884 pyowletapi-2023.5.9/src/pyowletapi/
+-rw-rw-rw-   0        0        0       17 2023-05-02 10:29:46.000000 pyowletapi-2023.5.9/src/pyowletapi/__init__.py
+-rw-rw-rw-   0        0        0    10605 2023-05-09 08:45:32.000000 pyowletapi-2023.5.9/src/pyowletapi/api.py
+-rw-rw-rw-   0        0        0      318 2023-05-03 10:36:51.000000 pyowletapi-2023.5.9/src/pyowletapi/exceptions.py
+-rw-rw-rw-   0        0        0     4306 2023-05-09 08:46:26.000000 pyowletapi-2023.5.9/src/pyowletapi/owlet.py
+-rw-rw-rw-   0        0        0     7398 2023-05-09 08:45:43.000000 pyowletapi-2023.5.9/src/pyowletapi/sock.py
+drwxrwxrwx   0        0        0        0 2023-05-09 08:52:39.390863 pyowletapi-2023.5.9/src/pyowletapi.egg-info/
+-rw-rw-rw-   0        0        0     2326 2023-05-09 08:52:39.000000 pyowletapi-2023.5.9/src/pyowletapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-05-09 08:52:39.000000 pyowletapi-2023.5.9/src/pyowletapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 08:52:39.000000 pyowletapi-2023.5.9/src/pyowletapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-09 08:52:39.000000 pyowletapi-2023.5.9/src/pyowletapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-09 08:52:39.000000 pyowletapi-2023.5.9/src/pyowletapi.egg-info/top_level.txt
```

### Comparing `pyowletapi-2023.5.7/PKG-INFO` & `pyowletapi-2023.5.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyowletapi
-Version: 2023.5.7
+Version: 2023.5.9
 Summary: Owlet baby montior API wrapper
 Home-page: https://github.com/RyanClark123/pyowletapi
 Author: Ryan Clark
 License: UNKNOWN
 Description: # Introduction
         
         First pass at creating a wrapper for the Owlet baby monitor api, this currently only supports the sock v3 as I do not have a v2 to test with
@@ -27,31 +27,32 @@
         
         ## To do
         Tidy up exception logging
         
         Create test routines
         
         ## Use
-        import the base Olwet object 
+        import the api and sock objects
         
         ```python
-        from pyowletapi.owlet import Owlet
+        from pyowletapi.api import OwletAPI
+        from pyowlet.sock import Sock
         ```
         
-        create an Owlet object passing your region, username and password
+        create an api object passing your region, username and password, the OwletAPI will also take a aiohttp session as a keyword argument
         
         ```python
-        owlet = Owlet('europe', username, password)
+        api = OwletAPI('europe', username, password)
         ```
         
-        you can then authenticate against the Owlet servers using this object and get a list of devices (as sock objects)
+        you can then authenticate against the Owlet servers using this object and create a list of sock objects
         
         ```python
-        await owlet.authenticate()
-        devices = await owlet.devices()
+        await api.authenticate()
+        socks = {device['device']['dsn']: Sock(api, device['device']) for device in devices}
         ```
         
         to get current reading from sock call the update_properties function on each sock object
         ```python
         device.update_properties()
         ```
         This will return a tuple, the first element being the raw response as a dict and the second element is a more cut down dict version of the response showing only the most relevant data.
```

### Comparing `pyowletapi-2023.5.7/README.md` & `pyowletapi-2023.5.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -20,31 +20,32 @@
 
 ## To do
 Tidy up exception logging
 
 Create test routines
 
 ## Use
-import the base Olwet object 
+import the api and sock objects
 
 ```python
-from pyowletapi.owlet import Owlet
+from pyowletapi.api import OwletAPI
+from pyowlet.sock import Sock
 ```
 
-create an Owlet object passing your region, username and password
+create an api object passing your region, username and password, the OwletAPI will also take a aiohttp session as a keyword argument
 
 ```python
-owlet = Owlet('europe', username, password)
+api = OwletAPI('europe', username, password)
 ```
 
-you can then authenticate against the Owlet servers using this object and get a list of devices (as sock objects)
+you can then authenticate against the Owlet servers using this object and create a list of sock objects
 
 ```python
-await owlet.authenticate()
-devices = await owlet.devices()
+await api.authenticate()
+socks = {device['device']['dsn']: Sock(api, device['device']) for device in devices}
 ```
 
 to get current reading from sock call the update_properties function on each sock object
 ```python
 device.update_properties()
 ```
 This will return a tuple, the first element being the raw response as a dict and the second element is a more cut down dict version of the response showing only the most relevant data.
```

### Comparing `pyowletapi-2023.5.7/setup.py` & `pyowletapi-2023.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
    
     name="pyowletapi",
-    version="2023.05.7",
+    version="2023.05.9",
     description="Owlet baby montior API wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/RyanClark123/pyowletapi",
     author="Ryan Clark",
     classifiers=[ 
         "License :: OSI Approved :: MIT License",
```

### Comparing `pyowletapi-2023.5.7/src/pyowletapi/api.py` & `pyowletapi-2023.5.9/src/pyowletapi/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import aiohttp
 import time
 import logging
 from logging import Logger
 from aiohttp.client_exceptions import ClientResponseError
 
-from .exceptions import OwletAuthenticationError, OwletConnectionError, OwletDevicesError, OwletError
+from .exceptions import (
+    OwletAuthenticationError,
+    OwletConnectionError,
+    OwletDevicesError,
+    OwletError,
+)
 
 logger: Logger = logging.getLogger(__package__)
 
 
 class OwletAPI:
     """
     A class that creates an API object, to be used to call against the Owlet baby Monitor API
@@ -46,19 +51,25 @@
         Returns a dictionary containing the API response with a list of devices
     activate:
         Turns on the base station, API requires that APP_ACTIVE be set to 1 to respond
     get_properties(device: str):
         For a provided device serial number this returns a dict of the current properties for this device from the API
     request(method: str, url: str, data: dict = None):
         method used for all the subsequent api calls after the original authenticate call, rather than repeating the same code multiple times
-        takes a method string which should either be 'GET' or 'POST', a url string for the relevant API endpoint and a dictionary containing 
+        takes a method string which should either be 'GET' or 'POST', a url string for the relevant API endpoint and a dictionary containing
         any data required to be passed to the api
     """
 
-    def __init__(self, region: str, user: str, password: str, session: aiohttp.ClientSession = None) -> None:
+    def __init__(
+        self,
+        region: str,
+        user: str,
+        password: str,
+        session: aiohttp.ClientSession = None,
+    ) -> None:
         """
         Sets all the necessary variables for the API caller based on the passed in information, if a session is not passed in then one is created
 
         Parameters
         ---------
         region (str):Region of user account, either world or europe
         user (str):Username (email) of user logging in
@@ -73,85 +84,96 @@
         self._auth_token: str = None
         self._expiry: float = None
         self.session = session
         self.headers = {}
         self.devices = {}
 
         self._region_info = {
-            'world': {
-                'url_mini': 'https://ayla-sso.owletdata.com/mini/',
-                'url_signin': 'https://user-field-1a2039d9.aylanetworks.com/api/v1/token_sign_in',
-                'url_base': 'https://ads-field-1a2039d9.aylanetworks.com/apiv1',
-                'apiKey': 'AIzaSyCsDZ8kWxQuLJAMVnmEhEkayH1TSxKXfGA',
-                'app_id': 'sso-prod-3g-id',
-                'app_secret': 'sso-prod-UEjtnPCtFfjdwIwxqnC0OipxRFU',
+            "world": {
+                "url_mini": "https://ayla-sso.owletdata.com/mini/",
+                "url_signin": "https://user-field-1a2039d9.aylanetworks.com/api/v1/token_sign_in",
+                "url_base": "https://ads-field-1a2039d9.aylanetworks.com/apiv1",
+                "apiKey": "AIzaSyCsDZ8kWxQuLJAMVnmEhEkayH1TSxKXfGA",
+                "app_id": "sso-prod-3g-id",
+                "app_secret": "sso-prod-UEjtnPCtFfjdwIwxqnC0OipxRFU",
+            },
+            "europe": {
+                "url_mini": "https://ayla-sso.eu.owletdata.com/mini/",
+                "url_signin": "https://user-field-eu-1a2039d9.aylanetworks.com/api/v1/token_sign_in",
+                "url_base": "https://ads-field-eu-1a2039d9.aylanetworks.com/apiv1",
+                "apiKey": "AIzaSyDm6EhV70wudwN3iOSq3vTjtsdGjdFLuuM",
+                "app_id": "OwletCare-Android-EU-fw-id",
+                "app_secret": "OwletCare-Android-EU-JKupMPBoj_Npce_9a95Pc8Qo0Mw",
             },
-            'europe': {
-                'url_mini': 'https://ayla-sso.eu.owletdata.com/mini/',
-                'url_signin': 'https://user-field-eu-1a2039d9.aylanetworks.com/api/v1/token_sign_in',
-                'url_base': 'https://ads-field-eu-1a2039d9.aylanetworks.com/apiv1',
-                'apiKey': 'AIzaSyDm6EhV70wudwN3iOSq3vTjtsdGjdFLuuM',
-                'app_id': 'OwletCare-Android-EU-fw-id',
-                'app_secret': 'OwletCare-Android-EU-JKupMPBoj_Npce_9a95Pc8Qo0Mw',
-            }
         }
 
         if self.session is None:
             self.session = aiohttp.ClientSession(raise_for_status=True)
 
-    async def authenticate(self) -> bool:
+    async def authenticate(self) -> None:
         """
         Authentiactes the user against the Owlet api using the provided details
 
         Sets the values of the headers and expiry time variables on the object
 
         Returns
         -------
         None
         """
-        if self._region not in ['europe','world']:
+        if self._region not in ["europe", "world"]:
             raise OwletAuthenticationError("Supplied region not valid")
-        
-        self._api_url = self._region_info[self._region]['url_base']
-
-        try:
-            if self._auth_token is not None:
-                raise OwletError
 
-            api_key = self._region_info[self._region]['apiKey']
-            async with self.session.request("POST", f'https://www.googleapis.com/identitytoolkit/v3/relyingparty/verifyPassword?key={api_key}', data={'email': self._user, 'password': self._password, 'returnSecureToken': True}, headers={
-                    'X-Android-Package': 'com.owletcare.owletcare', 'X-Android-Cert': '2A3BC26DB0B8B0792DBE28E6FFDC2598F9B12B74'}) as response:
+        self._api_url = self._region_info[self._region]["url_base"]
 
+        try:
+            api_key = self._region_info[self._region]["apiKey"]
+            async with self.session.request(
+                "POST",
+                f"https://www.googleapis.com/identitytoolkit/v3/relyingparty/verifyPassword?key={api_key}",
+                data={
+                    "email": self._user,
+                    "password": self._password,
+                    "returnSecureToken": True,
+                },
+                headers={
+                    "X-Android-Package": "com.owletcare.owletcare",
+                    "X-Android-Cert": "2A3BC26DB0B8B0792DBE28E6FFDC2598F9B12B74",
+                },
+            ) as response:
                 id_token = await response.json()
-                id_token = id_token['idToken']
-
-                async with self.session.request("GET", self._region_info[self._region]['url_mini'], headers={
-                        'Authorization': id_token}) as response:
+                id_token = id_token["idToken"]
 
+                async with self.session.request(
+                    "GET",
+                    self._region_info[self._region]["url_mini"],
+                    headers={"Authorization": id_token},
+                ) as response:
                     mini_token = await response.json()
-                    mini_token = mini_token['mini_token']
-
-                    async with self.session.request("POST", self._region_info[self._region]['url_signin'], json={
-                        "app_id": self._region_info[self._region]['app_id'],
-                        "app_secret": self._region_info[self._region]['app_secret'],
-                        "provider": "owl_id",
-                        "token": mini_token,
-                    }) as response:
+                    mini_token = mini_token["mini_token"]
 
+                    async with self.session.request(
+                        "POST",
+                        self._region_info[self._region]["url_signin"],
+                        json={
+                            "app_id": self._region_info[self._region]["app_id"],
+                            "app_secret": self._region_info[self._region]["app_secret"],
+                            "provider": "owl_id",
+                            "token": mini_token,
+                        },
+                    ) as response:
                         response = await response.json()
-                        access_token = response['access_token']
-
-                        self.headers['Authorization'] = 'auth_token ' + \
-                            access_token
-                        self._expiry = time.time() + response['expires_in']
-
-            return True
+                        access_token = response["access_token"]
+                        self.headers["Authorization"] = "auth_token " + access_token
+                        self._expiry = time.time() + response["expires_in"]
+                        print(self._expiry)
 
         except ClientResponseError:
-            raise OwletAuthenticationError("Bad request occurred check username and password and try again, did you select the correct region?")
+            raise OwletAuthenticationError(
+                "Bad request occurred check username and password and try again, did you select the correct region?"
+            )
         except Exception as error:
             raise OwletError from error
 
     async def close(self) -> None:
         """
         Closes the aiohttp ClientSession
 
@@ -169,31 +191,43 @@
         Returns
         ------
         dict: Dictionary containing the json response
         """
         if self._expiry <= time.time():
             self.authenticate()
 
-        return await self.request("GET", ('/devices.json'))
+        devices = await self.request("GET", ("/devices.json"))
+
+        if len(devices) < 1:
+            raise OwletDevicesError
+
+        return devices
 
     async def activate(self, device_serial: str) -> None:
         """
         Owlet API requires the APP_ACITVE be set to 1 to return properties, this sets that
 
         Parameters
         ---------
         device_serial (str):The serial number of the device being activated
 
         Returns
         -------
         None
         """
+
+        if self._expiry <= time.time():
+            self.authenticate()
+
         data = {"datapoint": {"metadata": {}, "value": 1}}
-        await self.request("POST",
-                           f'/dsns/{device_serial}/properties/APP_ACTIVE/datapoints.json', data=data)
+        await self.request(
+            "POST",
+            f"/dsns/{device_serial}/properties/APP_ACTIVE/datapoints.json",
+            data=data,
+        )
 
     async def get_properties(self, device: str) -> dict[str:list]:
         """
         Calls the Owlet API to get the current properties for a given device
 
         Parameters
         ----------
@@ -201,19 +235,18 @@
 
         Returns
         ------
         (dict):A dictionary containing all the current properties for the request device
         """
         properties = {}
         await self.activate(device)
-        response = await self.request("GET", f'/dsns/{device}/properties.json')
+        response = await self.request("GET", f"/dsns/{device}/properties.json")
 
         for property in response:
-            properties[property['property']
-                       ['name']] = property['property']
+            properties[property["property"]["name"]] = property["property"]
         return properties
 
     async def request(self, method: str, url: str, data: dict = None) -> dict:
         """
         Method for calling the Owlet API once authenticate has already been completed
 
         Parameters
@@ -223,13 +256,15 @@
         data (dict):A dictionary with the data to send to the API, only used when the activate method is called
 
         Returns
         ------
         dict: Dictionary containing the response
         """
         try:
-            async with self.session.request(method, self._api_url+url, headers=self.headers, json=data) as response:
+            async with self.session.request(
+                method, self._api_url + url, headers=self.headers, json=data
+            ) as response:
                 return await response.json()
         except ClientResponseError as error:
             raise OwletConnectionError from error
         except Exception as error:
             raise OwletError from error
```

### Comparing `pyowletapi-2023.5.7/src/pyowletapi/owlet.py` & `pyowletapi-2023.5.9/src/pyowletapi/owlet.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,28 +19,30 @@
     session : aiohttp.ClientSession
         The aiohttp ClientSession to be used for all API calls
     username : str
         username (email) of user logging in
     region : str
         region of user account, either world or europe
     api : OwletAPI
-        An instance of an OwletAPI object that will be used to communicate with the Owlet API   
+        An instance of an OwletAPI object that will be used to communicate with the Owlet API
 
     Methods
     -------
     authenticate:
         calls the authenticate method on the OwletAPI object telling it to authenticate
     devices:
         Calls the get_devices method on the OwletAPI object, returns a dictionary with the device serial numbers as the key
         and sock objects as the values
     close:
-        Calls the close method on the OwletAPI object, closes the ClientSession   
+        Calls the close method on the OwletAPI object, closes the ClientSession
     """
 
-    def __init__(self, region: str, username: str, password: str, session: ClientSession = None) -> None:
+    def __init__(
+        self, region: str, username: str, password: str, session: ClientSession = None
+    ) -> None:
         """
         Sets all the necessary variables for the API caller based on the passed in information
 
         Parameters
         --------
         region (str):Region of user account, either world or europe
         username (str):Username (email) of user logging in
@@ -59,44 +61,47 @@
         Method that calls the authenticate method on the OwletAPI object
 
         Returns
         ------
         (bool):Boolean showing the status of the authentication
         """
         try:
-            logger.info(
-                f"attempting login for {self.username}, region {self.region}")
-            if(await self._api.authenticate()):
+            logger.info(f"attempting login for {self.username}, region {self.region}")
+            if await self._api.authenticate():
                 logger.info("Authentication succesful")
                 return True
         except OwletAuthenticationError:
-                return False
+            return False
 
     async def get_devices(self) -> dict[str:Sock]:
         """
         Method that calls the get devices method on the OwletAPI and returns a dictionary of the results
 
         Returns
         -------
         (dict):Dictionary, the keys being the serial number of each device, the values are then a sock object for that device which contains all the relevant device
         properties
         """
         try:
             logger.info("retrieving devices")
             devices = await self._api.get_devices()
-            
+
             if len(devices) < 1:
                 raise OwletDevicesError
 
-            return {device['device']['dsn']: Sock(self._api, device['device']) for device in devices}
+            return {
+                device["device"]["dsn"]: Sock(self._api, device["device"])
+                for device in devices
+            }
         except OwletDevicesError("No devices exist for user"):
             logger.degug(
-                f"No devices exist for user {self.username}, region: {self.region}")
-            
-    async def check_device_exists(self, serial : str) -> bool:
+                f"No devices exist for user {self.username}, region: {self.region}"
+            )
+
+    async def check_device_exists(self, serial: str) -> bool:
         """
         Method that calls that checks if a specified device is valid for the current user
 
         Returns
         ------
         (bool):Boolean showing the result of the check, if True the device is valid otherwise an OwletDeviceError will be raised
         """
```

### Comparing `pyowletapi-2023.5.7/src/pyowletapi/sock.py` & `pyowletapi-2023.5.9/src/pyowletapi/sock.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import datetime
 from .api import OwletAPI
 from typing import Union
 
 logger: Logger = logging.getLogger(__package__)
 
-CHARGING_STATUSES = ['NOT CHARGING', 'CHARGING', 'CHARGED']
+CHARGING_STATUSES = ["NOT CHARGING", "CHARGING", "CHARGED"]
 
 
 class Sock:
     """
     Class representing a Owlet sock device
 
     Attributes
@@ -19,65 +19,67 @@
     name : str
         The product name
     mode: str
         the product model
     serial : str
         the serial number of the device
     oem_model : str
-        The oem model of the device   
+        The oem model of the device
     sw_version : str
-        The software version of the device   
+        The software version of the device
     mac : str
-        The mac address the device   
+        The mac address the device
     lan_ip : str
-        The current lan ip address of the device   
+        The current lan ip address of the device
     connection_status : str
-        The current connection status of the device   
+        The current connection status of the device
     device_type : str
-        The device type   
+        The device type
     manuf_model : str
         The manunfacturer's model number
     api : OwletAPI
         The current OwletAPI object being used to call the Owlet API
     raw_properties : dict
         A dictionionary containing the raw response from the device properties api call
     properties : dict
-        A formatted, cut down version of the current device properties   
+        A formatted, cut down version of the current device properties
 
     Methods
     -------
     get_property:
         returns a specific property for the device
     get_properties:
         returns all the properties for the current device
     normalise_properties:
         takes the raw_properties and strips out only the most important properties making the dict object smaller and easier to use
     update_properties
         usees the OwletAPI object to call the Owlet server and return the current properties of the device.
     """
 
-    def __init__(self, api: OwletAPI, data: dict[str:Union[str, int, bool, list]]) -> None:
+    def __init__(
+        self, api: OwletAPI, data: dict[str : Union[str, int, bool, list]]
+    ) -> None:
         """
         Constructs an Owlet sock object representing the owlet sock device
 
         Parameters
         ----------
         api (OwletAPI):OwletAPI object used to call the Owlet API
         data (dict):Data returned from the Owlet API showing the details of the sock
         """
-        self._name = data['product_name']
-        self._model = data['model']
-        self._serial = data['dsn']
-        self._oem_model = data['oem_model']
-        self._sw_version = data['sw_version']
-        self._mac = data['mac']
-        self._lan_ip = data['lan_ip']
-        self._connection_status = data['connection_status']
-        self._device_type = data['device_type']
-        self._manuf_model = data['manuf_model']
+        self._name = data["product_name"]
+        self._model = data["model"]
+        self._serial = data["dsn"]
+        self._oem_model = data["oem_model"]
+        self._sw_version = data["sw_version"]
+        self._mac = data["mac"]
+        self._lan_ip = data["lan_ip"]
+        self._connection_status = data["connection_status"]
+        self._device_type = data["device_type"]
+        self._manuf_model = data["manuf_model"]
 
         self._api = api
 
         self.raw_properties = {}
         self.properties = {}
 
     @property
@@ -140,65 +142,72 @@
 
         Returns
         -------
         (dict):Request properties as a dict
         """
         return self.properties
 
-    async def normalise_properties(self, raw_properties: dict[str:dict]) -> dict[str:Union[bool, str, float]]:
+    async def normalise_properties(
+        self, raw_properties: dict[str:dict]
+    ) -> dict[str : Union[bool, str, float]]:
         """
         Takes the raw properties dictionary returned from the API and formats it into another dict that is more stripped down and easier to work with
 
         Parameters
         ----------
             raw_properties (dict[str:dict]):The raw properties returned from the API call
 
         Returns
         -------
             (dict):Returns the stripped down properties as a dict
         """
         properties = {}
-        properties['app_active'] = bool(raw_properties["APP_ACTIVE"]["value"])
+        properties["app_active"] = bool(raw_properties["APP_ACTIVE"]["value"])
 
-        properties['high_heart_rate_alert'] = bool(
-            raw_properties["HIGH_HR_ALRT"]["value"])
-        properties['high_oxygen_alert'] = bool(
-            raw_properties["HIGH_OX_ALRT"]["value"])
-        properties['low_battery_alert'] = bool(
-            raw_properties["LOW_BATT_ALRT"]["value"])
-        properties['low_heart_rate_alert'] = bool(
-            raw_properties["LOW_HR_ALRT"]["value"])
-        properties['low_oxygen_alert'] = bool(
-            raw_properties["LOW_OX_ALRT"]["value"])
-        properties['ppg_log_file'] = bool(
-            raw_properties["PPG_LOG_FILE"]["value"])
-        properties['firmware_update_available'] = bool(
-            raw_properties['FW_UPDATE_STATUS']['value'])
-        properties['lost_power_alert'] = bool(
-            raw_properties['LOST_POWER_ALRT']['value'])
-        properties['sock_disconnected'] = bool(
-            raw_properties['SOCK_DISCON_ALRT']['value'])
-        properties['sock_off'] = bool(raw_properties['SOCK_OFF']['value'])
+        properties["high_heart_rate_alert"] = bool(
+            raw_properties["HIGH_HR_ALRT"]["value"]
+        )
+        properties["high_oxygen_alert"] = bool(raw_properties["HIGH_OX_ALRT"]["value"])
+        properties["low_battery_alert"] = bool(raw_properties["LOW_BATT_ALRT"]["value"])
+        properties["low_heart_rate_alert"] = bool(
+            raw_properties["LOW_HR_ALRT"]["value"]
+        )
+        properties["low_oxygen_alert"] = bool(raw_properties["LOW_OX_ALRT"]["value"])
+        properties["ppg_log_file"] = bool(raw_properties["PPG_LOG_FILE"]["value"])
+        properties["firmware_update_available"] = bool(
+            raw_properties["FW_UPDATE_STATUS"]["value"]
+        )
+        properties["lost_power_alert"] = bool(
+            raw_properties["LOST_POWER_ALRT"]["value"]
+        )
+        properties["sock_disconnected"] = bool(
+            raw_properties["SOCK_DISCON_ALRT"]["value"]
+        )
+        properties["sock_off"] = bool(raw_properties["SOCK_OFF"]["value"])
 
         vitals = json.loads(raw_properties["REAL_TIME_VITALS"]["value"])
-        properties['oxygen_saturation'] = float(vitals["ox"])
-        properties['heart_rate'] = float(vitals["hr"])
-        properties['moving'] = bool(vitals["mv"])
-        properties['base_station_on'] = True if bool(
-            vitals['bso']) or bool(vitals['chg']) else False
-        properties['battery_percentage'] = float(vitals["bat"])
-        properties['battery_minutes'] = float(vitals["btt"])
-        properties['charging'] = True if int(vitals['chg']) in [1,2] else False
-        properties['signal_strength'] = float(vitals['rsi'])
-        properties['last_updated'] = datetime.datetime.strptime(
-            raw_properties["REAL_TIME_VITALS"]["data_updated_at"], '%Y-%m-%dT%H:%M:%SZ').strftime("%Y/%m/%d %H:%M:%S")
+        properties["oxygen_saturation"] = float(vitals["ox"])
+        properties["heart_rate"] = float(vitals["hr"])
+        properties["moving"] = bool(vitals["mv"])
+        properties["base_station_on"] = (
+            True if bool(vitals["bso"]) or bool(vitals["chg"]) else False
+        )
+        properties["battery_percentage"] = float(vitals["bat"])
+        properties["battery_minutes"] = float(vitals["btt"])
+        properties["charging"] = True if int(vitals["chg"]) in [1, 2] else False
+        properties["signal_strength"] = float(vitals["rsi"])
+        properties["last_updated"] = datetime.datetime.strptime(
+            raw_properties["REAL_TIME_VITALS"]["data_updated_at"], "%Y-%m-%dT%H:%M:%SZ"
+        ).strftime("%Y/%m/%d %H:%M:%S")
 
         return properties
 
-    async def update_properties(self) -> tuple[dict[str, dict], dict[str:Union[bool, str, float]]]:
+    async def update_properties(
+        self,
+    ) -> tuple[dict[str, dict], dict[str : Union[bool, str, float]]]:
         """
         Calls the Owlet api to update the properties and then returns both the raw response dict and the formatted dict from
         normalise_properties
 
         Returns
         -------
         (tuple):Tuple containing two dictionaries, one with the raw json response from the API and another with the stripped down properties from normalise_properties
```

### Comparing `pyowletapi-2023.5.7/src/pyowletapi.egg-info/PKG-INFO` & `pyowletapi-2023.5.9/src/pyowletapi.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyowletapi
-Version: 2023.5.7
+Version: 2023.5.9
 Summary: Owlet baby montior API wrapper
 Home-page: https://github.com/RyanClark123/pyowletapi
 Author: Ryan Clark
 License: UNKNOWN
 Description: # Introduction
         
         First pass at creating a wrapper for the Owlet baby monitor api, this currently only supports the sock v3 as I do not have a v2 to test with
@@ -27,31 +27,32 @@
         
         ## To do
         Tidy up exception logging
         
         Create test routines
         
         ## Use
-        import the base Olwet object 
+        import the api and sock objects
         
         ```python
-        from pyowletapi.owlet import Owlet
+        from pyowletapi.api import OwletAPI
+        from pyowlet.sock import Sock
         ```
         
-        create an Owlet object passing your region, username and password
+        create an api object passing your region, username and password, the OwletAPI will also take a aiohttp session as a keyword argument
         
         ```python
-        owlet = Owlet('europe', username, password)
+        api = OwletAPI('europe', username, password)
         ```
         
-        you can then authenticate against the Owlet servers using this object and get a list of devices (as sock objects)
+        you can then authenticate against the Owlet servers using this object and create a list of sock objects
         
         ```python
-        await owlet.authenticate()
-        devices = await owlet.devices()
+        await api.authenticate()
+        socks = {device['device']['dsn']: Sock(api, device['device']) for device in devices}
         ```
         
         to get current reading from sock call the update_properties function on each sock object
         ```python
         device.update_properties()
         ```
         This will return a tuple, the first element being the raw response as a dict and the second element is a more cut down dict version of the response showing only the most relevant data.
```

