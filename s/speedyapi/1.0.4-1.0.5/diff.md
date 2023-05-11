# Comparing `tmp/speedyapi-1.0.4.tar.gz` & `tmp/speedyapi-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Ushio\Documents\SpeedyAPI\dist\.tmp-rvvcwfvx\speedyapi-1.0.4.tar", last modified: Tue Mar 14 17:45:25 2023, max compression
+gzip compressed data, was "speedyapi-1.0.5.tar", last modified: Thu May 11 15:52:28 2023, max compression
```

## Comparing `speedyapi-1.0.4.tar` & `speedyapi-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 17:45:25.331722 speedyapi-1.0.4/
--rw-rw-rw-   0        0        0     4716 2023-03-14 17:45:25.331222 speedyapi-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3968 2023-03-14 17:07:28.000000 speedyapi-1.0.4/README.md
--rw-rw-rw-   0        0        0     1029 2023-03-14 17:45:05.000000 speedyapi-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-14 17:45:25.332221 speedyapi-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-14 17:45:25.300780 speedyapi-1.0.4/speedyapi/
--rw-rw-rw-   0        0        0     1318 2023-03-14 16:16:19.000000 speedyapi-1.0.4/speedyapi/__init__.py
--rw-rw-rw-   0        0        0    17926 2023-03-13 16:24:03.000000 speedyapi-1.0.4/speedyapi/color.py
--rw-rw-rw-   0        0        0       95 2023-03-09 11:09:35.000000 speedyapi-1.0.4/speedyapi/exceptions.py
--rw-rw-rw-   0        0        0     1912 2023-03-13 16:26:43.000000 speedyapi-1.0.4/speedyapi/handler.py
--rw-rw-rw-   0        0        0     2533 2023-03-13 16:40:21.000000 speedyapi-1.0.4/speedyapi/limiter.py
--rw-rw-rw-   0        0        0     1353 2023-03-13 16:43:52.000000 speedyapi-1.0.4/speedyapi/logging.py
--rw-rw-rw-   0        0        0    45229 2023-03-14 14:43:37.000000 speedyapi-1.0.4/speedyapi/main.py
--rw-rw-rw-   0        0        0     9457 2023-03-14 14:09:15.000000 speedyapi-1.0.4/speedyapi/parameters.py
--rw-rw-rw-   0        0        0     7891 2023-03-14 14:43:37.000000 speedyapi-1.0.4/speedyapi/respond.py
--rw-rw-rw-   0        0        0     5770 2023-03-13 17:43:12.000000 speedyapi-1.0.4/speedyapi/swagger.py
--rw-rw-rw-   0        0        0   115148 2023-03-12 17:02:26.000000 speedyapi-1.0.4/speedyapi/swagger_objects.py
--rw-rw-rw-   0        0        0     6086 2023-03-14 10:41:07.000000 speedyapi-1.0.4/speedyapi/tests.py
--rw-rw-rw-   0        0        0      284 2023-03-14 11:04:16.000000 speedyapi-1.0.4/speedyapi/types.py
--rw-rw-rw-   0        0        0    12692 2023-03-13 22:59:31.000000 speedyapi-1.0.4/speedyapi/util.py
-drwxrwxrwx   0        0        0        0 2023-03-14 17:45:25.329224 speedyapi-1.0.4/speedyapi.egg-info/
--rw-rw-rw-   0        0        0     4716 2023-03-14 17:45:25.000000 speedyapi-1.0.4/speedyapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      485 2023-03-14 17:45:25.000000 speedyapi-1.0.4/speedyapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 17:45:25.000000 speedyapi-1.0.4/speedyapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-03-14 17:45:25.000000 speedyapi-1.0.4/speedyapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-14 17:45:25.000000 speedyapi-1.0.4/speedyapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 15:52:28.956896 speedyapi-1.0.5/
+-rw-rw-rw-   0        0        0     4832 2023-05-11 15:52:28.955398 speedyapi-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4084 2023-03-14 17:49:52.000000 speedyapi-1.0.5/README.md
+-rw-rw-rw-   0        0        0     1029 2023-05-11 15:14:10.000000 speedyapi-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 15:52:28.957395 speedyapi-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 15:52:28.917449 speedyapi-1.0.5/speedyapi/
+-rw-rw-rw-   0        0        0     1318 2023-03-14 16:16:19.000000 speedyapi-1.0.5/speedyapi/__init__.py
+-rw-rw-rw-   0        0        0    17926 2023-03-13 16:24:03.000000 speedyapi-1.0.5/speedyapi/color.py
+-rw-rw-rw-   0        0        0       95 2023-03-09 11:09:35.000000 speedyapi-1.0.5/speedyapi/exceptions.py
+-rw-rw-rw-   0        0        0     1912 2023-03-13 16:26:43.000000 speedyapi-1.0.5/speedyapi/handler.py
+-rw-rw-rw-   0        0        0     2533 2023-03-13 16:40:21.000000 speedyapi-1.0.5/speedyapi/limiter.py
+-rw-rw-rw-   0        0        0     1353 2023-03-13 16:43:52.000000 speedyapi-1.0.5/speedyapi/logging.py
+-rw-rw-rw-   0        0        0    46067 2023-05-11 15:47:56.000000 speedyapi-1.0.5/speedyapi/main.py
+-rw-rw-rw-   0        0        0     9762 2023-05-11 15:12:58.000000 speedyapi-1.0.5/speedyapi/parameters.py
+-rw-rw-rw-   0        0        0     7881 2023-05-11 15:12:58.000000 speedyapi-1.0.5/speedyapi/respond.py
+-rw-rw-rw-   0        0        0     5882 2023-05-11 15:12:58.000000 speedyapi-1.0.5/speedyapi/swagger.py
+-rw-rw-rw-   0        0        0   115148 2023-03-12 17:02:26.000000 speedyapi-1.0.5/speedyapi/swagger_objects.py
+-rw-rw-rw-   0        0        0     7072 2023-05-11 15:12:58.000000 speedyapi-1.0.5/speedyapi/tests.py
+-rw-rw-rw-   0        0        0      284 2023-03-14 11:04:16.000000 speedyapi-1.0.5/speedyapi/types.py
+-rw-rw-rw-   0        0        0    12793 2023-05-11 15:12:58.000000 speedyapi-1.0.5/speedyapi/util.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:52:28.953401 speedyapi-1.0.5/speedyapi.egg-info/
+-rw-rw-rw-   0        0        0     4832 2023-05-11 15:52:28.000000 speedyapi-1.0.5/speedyapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      485 2023-05-11 15:52:28.000000 speedyapi-1.0.5/speedyapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 15:52:28.000000 speedyapi-1.0.5/speedyapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-11 15:52:28.000000 speedyapi-1.0.5/speedyapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 15:52:28.000000 speedyapi-1.0.5/speedyapi.egg-info/top_level.txt
```

### Comparing `speedyapi-1.0.4/PKG-INFO` & `speedyapi-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedyapi
-Version: 1.0.4
+Version: 1.0.5
 Summary: An easy to use Python module for creating API.
 Author: CodingYuno
 Project-URL: Source Code, https://github.com/CodingYuno/speedyapi/
 Project-URL: Issue Tracker, https://github.com/CodingYuno/speedyapi/issues/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -26,14 +26,18 @@
 - Parameter Parsing and Checking
 - API Authentication
 - Rate Limiting (user, address, global)
 - In-depth Endpoint Testing (Write tests to be run that confirm endpoints act as intended)
 - Automatic OpenAPI `swagger.json` Generation (with access to full specification)
 - Common JSON Response Formatting
 
+# Installation
+
+Simply run `pip install speedyapi`. The PyPI package is at https://pypi.org/project/speedyapi/
+
 # Dependencies
 
 - **[Python](https://www.python.org/downloads/)** 3.10
 - **[Requests](https://github.com/kennethreitz/requests)** >= 2.9.2
 - **[Flask](https://github.com/pallets/flask)** >= 2.2
 
 # Example Usage
```

### Comparing `speedyapi-1.0.4/README.md` & `speedyapi-1.0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 - Parameter Parsing and Checking
 - API Authentication
 - Rate Limiting (user, address, global)
 - In-depth Endpoint Testing (Write tests to be run that confirm endpoints act as intended)
 - Automatic OpenAPI `swagger.json` Generation (with access to full specification)
 - Common JSON Response Formatting
 
+# Installation
+
+Simply run `pip install speedyapi`. The PyPI package is at https://pypi.org/project/speedyapi/
+
 # Dependencies
 
 - **[Python](https://www.python.org/downloads/)** 3.10
 - **[Requests](https://github.com/kennethreitz/requests)** >= 2.9.2
 - **[Flask](https://github.com/pallets/flask)** >= 2.2
 
 # Example Usage
```

### Comparing `speedyapi-1.0.4/pyproject.toml` & `speedyapi-1.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "speedyapi"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="CodingYuno"},
 ]
 description = "An easy to use Python module for creating API."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `speedyapi-1.0.4/speedyapi/__init__.py` & `speedyapi-1.0.5/speedyapi/__init__.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.4/speedyapi/color.py` & `speedyapi-1.0.5/speedyapi/color.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.4/speedyapi/handler.py` & `speedyapi-1.0.5/speedyapi/handler.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.4/speedyapi/limiter.py` & `speedyapi-1.0.5/speedyapi/limiter.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.4/speedyapi/logging.py` & `speedyapi-1.0.5/speedyapi/logging.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.4/speedyapi/main.py` & `speedyapi-1.0.5/speedyapi/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,36 +122,36 @@
 
         # Added to replace the standard `404 not found` and `405 wrong method` thrown on unknown endpoints by Flask
         @self.endpoint(path="/<path:path>", docs_ignore=True)
         def catch_all(path):
             return invalid(key="cause", data=f"Unknown endpoint: /{path}", success=False)
 
         # Added to automatically handle favicon.ico
-        @self.endpoint(path=f"/{path_to_favicon}", docs_ignore=True)
+        @self.endpoint(path=f"/favicon.ico", docs_ignore=True)
         def favicon():
             try:
-                return send_file('favicon.ico', mimetype='image/vnd.microsoft.icon')
+                return send_file(path_to_favicon, mimetype='image/vnd.microsoft.icon')
             except FileNotFoundError:
                 return error(cause="FileNotFoundError")
 
         # Async and Sync methods for logging with a passed function
         # Standard logging to a file
         if inspect.iscoroutinefunction(logger):  # Async
             @self.after_request
             async def after_request(response):
                 if self.request_logging:
                     api_logging(response)
-                    await self.logger(response)
+                    await logger(response)
                 return response
         elif callable(logger):  # Sync
             @self.after_request
             async def after_request(response):
                 if self.request_logging:
                     api_logging(response)
-                    await self.logger(response)
+                    await logger(response)
                 return response
         elif type(logger) == str:  # Log to file
             @self.after_request
             async def after_request(response):
                 if self.request_logging:
                     api_logging(response, log_file=logger, print_logs=True)
                 return response
@@ -163,15 +163,15 @@
             return json(swagger_json)
 
         # The base path is used for Redoc documentation based on an automatically generated or manually set swagger.json file
         @self.endpoint(path=f"/", method="GET", docs_ignore=True)
         async def docs():
             return html(redoc_html(info.title, server=request.host_url))
 
-    def endpoint(self, path: str, method: str = "GET", authentication=None, name: str = None, description: str = None, docs_ignore: bool = False):
+    def endpoint(self, path: str, method: str = "GET", authentication: str | list = None, name: str = None, description: str = None, docs_ignore: bool = False, group: str = None):
         """
         Creation of endpoints for the API
 
         :param path: The path of the endpoint
         :param method: The method of the endpoint e.g. GET, POST, PUT .. (Unlike standard Flask please write separate endpoints for each method type if required)
         :param authentication: The authentication scope for the endpoint.
         :param name: The name of the endpoint (Used for swagger.json generation)
@@ -214,15 +214,17 @@
                     receive_time = time.time()
                     if authentication is not None:  # Standard Apikey authentication handling (As explained below in the `authentication` docstring you can use this for other methods e.g. oauth)
                         apikey = dict(request.args).get("key", dict(request.headers).get("Apikey", None))
                         request.apikey = apikey
                         auth_type = None
                         if apikey is None and self.async_auth_function_require_key:
                             return missing("key")  # If an apikey is required a missing key response is sent
-                        if self.async_auth_function and (auth_type := await self.async_auth_function()) is None:
+                        if self.async_auth_function and (auth_type := await self.async_auth_function()) not in authentication:
+                            if type(auth_type) == Response:
+                                return auth_type
                             return forbidden(cause="Access is forbidden, usually due to an invalid API key being used.")  # Standard 403 response (You can return your own custom response anywhere in the request context)
                         if type(auth_type) == Response:
                             return auth_type
                         request.authentication = auth_type
                     else:
                         request.authentication, request.apikey = None, None
                     response = await async_request_handler(f, print_traceback=self.print_traceback, *args, **kwargs)
@@ -237,52 +239,57 @@
                     receive_time = time.time()
                     if authentication is not None:
                         apikey = dict(request.args).get("key", dict(request.headers).get("Apikey", None))
                         request.apikey = apikey
                         auth_type = None
                         if apikey is None and self.auth_function_require_key:
                             return missing("key")
-                        if self.auth_function and (auth_type := self.auth_function()) is None:
+                        if self.auth_function and (auth_type := self.auth_function()) not in authentication:
+                            if type(auth_type) == Response:
+                                return auth_type
                             return forbidden(cause="Access is forbidden, usually due to an invalid API key being used.")
                         if type(auth_type) == Response:
                             return auth_type
                         request.authentication = auth_type
                     else:
                         request.authentication, request.apikey = None, None
                     response = request_handler(f, print_traceback=self.print_traceback, *args, **kwargs)
                     response.headers = {**response.headers, **{"Process-Time": round(time.time() - receive_time)}}
                     return response
 
                 return decorated_function
 
+        authentication = [authentication] if type(authentication) == str else authentication
+
         method = [method] if type(method) == str else method  # methods are placed in lists here as from this point onwards support for multiple methods is supported (Not yet supported throughout)
         if any(m.upper() not in ["GET", "POST", "HEAD", "PUT", "DELETE", "PATCH"] for m in method):
             raise InvalidMethod("Method must be one of `GET`, `POST`, `HEAD`, `PUT`, `DELETE`, `PATCH`")
 
         # Automatic documentation generation for the swagger.json file
         if not docs_ignore:
 
             # An api endpoint storage not used anywhere. Could be useful to a developer.
             self.api_endpoint_list.append({"path": path, "method": method, "authentication": authentication, "name": name, "description": description})
 
             if path not in self.swagger["paths"].keys():  # Path is not added to the PathsObject as a PathItemObject
                 self.swagger["paths"][path] = PathItemObject()  # New path added to the OpenAPI Paths object
             for meth in method:
                 self.swagger["paths"][path][meth.lower()] = OperationObject(
+                    tags=[group] if group else None,
                     summary=name,
                     description=description,
                     security=[],
                     responses=ResponsesObject()
                 )
 
                 # Adding authentication to the Operation Object (If you are using more complex authentication please add to `.swagger` inside your application file)
                 if authentication is not None:
                     self.swagger["paths"][path][meth.lower()]["security"] = [SecurityRequirementObject(
-                        Apikey=[authentication],
-                        key=[authentication]
+                        Apikey=authentication,
+                        key=authentication
                     )]
 
         return decorator
 
     def authentication(self, apikey_required: bool = False, description: str = None):
         """
         Used to create authentication functions for the API.
@@ -318,15 +325,15 @@
                 self.async_auth_function = f
                 self.async_auth_function_require_key = apikey_required
             else:
                 self.auth_function = f  # if the authentication function is `Sync`
                 self.auth_function_require_key = apikey_required
 
             # Add the security definition to the Swagger info object description to be accessed by Redoc
-            self.swagger.info.description += "\n\n<!-- ReDoc-Inject: <security-definitions> -->"
+            self.swagger.info.description += "\n\n# Authentication\n\n<!-- ReDoc-Inject: <security-definitions> -->"
 
             if apikey_required:
                 # If an apikey is being used standard apikey schemes are added to the security component of the swagger
                 self.swagger.components.securitySchemes = Map(
                     Apikey=SecuritySchemeObject(type="apiKey", name="Apikey", _in="header", description=description),
                     key=SecuritySchemeObject(type="apiKey", name="key", _in="query", description=description)
                 )
@@ -417,64 +424,67 @@
                         parsed_inputs = input_handler(parameter=parameter_object, **path_kwargs)  # Find the values of the parameters and parse them to correct types
                         if type(parsed_inputs) == Response:
                             return parsed_inputs  # If a request response has been raised during parsing e.g. missing or malformed it needs to be returned here too
                         else:
                             kwargs = kwargs | parsed_inputs  # Add the newly parsed input parameters to kwargs
                     return await f(**kwargs)
 
-                return async_decorated_function
             else:  # Endpoint using Standard Flask (not async)
                 @functools.wraps(f)
                 def decorated_function(**kwargs):
                     path_kwargs = kwargs
                     for parameter_object in args:
                         test_parameter_type(parameter_object)
                         parsed_inputs = input_handler(parameter=parameter_object, **path_kwargs)
                         if type(parsed_inputs) == Response:
                             return parsed_inputs
                         else:
                             kwargs = kwargs | parsed_inputs
                     return f(**kwargs)
 
+
             # We need to know the path and method of the endpoint from a higher up decorator so ast + inspect are used to visit the source
             path = get_decorators_args(f, is_async=inspect.iscoroutinefunction(f))[f.__name__]["endpoint"]["kwargs"]["path"]
             method = get_decorators_args(f, is_async=inspect.iscoroutinefunction(f))[f.__name__]["endpoint"]["kwargs"]["method"]
 
             # Each method for the endpoint needs to have parameters automatically added to its swagger.json
-            for meth, meth_obj in self.swagger["paths"][path].copy().items():
-                if meth.lower() != method.lower():  # The method is not from this endpoint so is ignored
-                    continue
-
-                meth_obj["parameters"] = []
-                for parameter_object in args:
-
-                    # This is not a part of the specification however I like to show options in bold at the bottom of the description string
-                    option_string = "" if parameter_object.options is None else f"\n\n**Options**: {', '.join(parameter_object.options)}"
-
-                    # JsonBodyParameter edge case is added to the parameter name (Warning this is not allowed in the OpenAPI specification)
-                    name_string = parameter_object.name if type(parameter_object) != JsonBodyParameter else f"Json Body: {{'{parameter_object.name}': <{parameter_object.type.__name__}>}}"
-
-                    if type(parameter_object) == JsonBodyParameter:  # No longer requires separate Parameter Object creation (Will be removed)
-                        meth_obj["parameters"].append(ParameterObject(
-                            name=name_string,
-                            description=parameter_object.description + option_string,
-                            _in=convert_param_to_in(parameter_object),
-                            schema={"type": parameter_object.type.__name__},
-                            required=parameter_object.required
-                        ))
-                    else:
-                        meth_obj["parameters"].append(ParameterObject(
-                            name=name_string,
-                            description=parameter_object.description + option_string,
-                            _in=convert_param_to_in(parameter_object),
-                            schema={"type": parameter_object.type.__name__},  # The name of the OpenAPI parameter object type is found
-                            required=parameter_object.required
-                        ))
+            if path in self.swagger["paths"]:
+                for meth, meth_obj in self.swagger["paths"][path].copy().items():
+                    if meth.lower() != method.lower():  # The method is not from this endpoint so is ignored
+                        continue
+
+                    meth_obj["parameters"] = []
+                    for parameter_object in args:
+
+                        # This is not a part of the specification however I like to show options in bold at the bottom of the description string
+                        option_string = "" if parameter_object.options is None else f"\n\n**Options**: {', '.join(parameter_object.options)}"
 
-            return decorated_function
+                        # JsonBodyParameter edge case is added to the parameter name (Warning this is not allowed in the OpenAPI specification)
+                        name_string = parameter_object.name if type(parameter_object) != JsonBodyParameter else f"Json Body: {{'{parameter_object.name}': <{parameter_object.type.__name__}>}}"
+                        if type(parameter_object) == JsonBodyParameter:  # No longer requires separate Parameter Object creation (Will be removed)
+                            meth_obj["parameters"].append(ParameterObject(
+                                name=name_string,
+                                description=parameter_object.description + option_string,
+                                _in=convert_param_to_in(parameter_object),
+                                schema={"type": parameter_object.type.__name__},
+                                required=parameter_object.required
+                            ))
+                        else:
+                            meth_obj["parameters"].append(ParameterObject(
+                                name=name_string,
+                                description=parameter_object.description + option_string,
+                                _in=convert_param_to_in(parameter_object),
+                                schema={"type": parameter_object.type.__name__},  # The name of the OpenAPI parameter object type is found
+                                required=parameter_object.required
+                            ))
+
+            if inspect.iscoroutinefunction(f):
+                return async_decorated_function
+            else:
+                return decorated_function
         return decorator
 
     def limits(self, user_limits: list = None, ip_limits: list = None, global_limits: list = None):
         """
         Add rate limits to the endpoint.
 
         :param user_limits: rate limit strings to be applied to individuals using the endpoint (distinguished by apikey)
@@ -520,14 +530,26 @@
 
         You can add rate limits for the whole API in the app creation arguments.
 
         I have not implemented automatic generation of documentation for rate limits as it is generally advisable to not reveal rate limits to users
         If you do wish to reveal the rate limit then just add it to the authentication description.
         """
         def decorator(f):
+
+            # We need to know the path and method of the endpoint from a higher up decorator so ast + inspect are used to visit the source
+            path = get_decorators_args(f, is_async=inspect.iscoroutinefunction(f))[f.__name__]["endpoint"]["kwargs"]["path"]
+            method = get_decorators_args(f, is_async=inspect.iscoroutinefunction(f))[f.__name__]["endpoint"]["kwargs"]["method"]
+
+            # Rate limit locations are created for the endpoint
+            self.rate_limits["paths"].setdefault(path, {})[method] = dict(
+                user_limits={},
+                ip_limits={},
+                global_limits={}
+            )
+
             if inspect.iscoroutinefunction(f):  # Endpoint using Async Flask
                 @functools.wraps(f)
                 async def async_decorated_function(**kwargs):
                     current_time_s = round(time.time())  # The recieve time is only created once per request
 
                     # Limits are checked for breaches for the per endpoint limits
                     user_res = update_limits(user_limits, current_time_s, self.rate_limits["paths"][path][method]["user_limits"], request.apikey)
@@ -561,26 +583,16 @@
                     overall_global_res = update_limits(self.global_limits, current_time_s, self.rate_limits["overall_limits"]["global_limits"])
 
                     if any(type(res) == int for res in [user_res, addr_res, global_res, overall_user_res, overall_addr_res, overall_global_res]):
                         return rate_limited(max([wt for wt in [user_res, addr_res, global_res, overall_user_res, overall_addr_res, overall_global_res] if type(wt) == int]))
 
                     return f(**kwargs)
 
-            # We need to know the path and method of the endpoint from a higher up decorator so ast + inspect are used to visit the source
-            path = get_decorators_args(f, is_async=inspect.iscoroutinefunction(f))[f.__name__]["endpoint"]["kwargs"]["path"]
-            method = get_decorators_args(f, is_async=inspect.iscoroutinefunction(f))[f.__name__]["endpoint"]["kwargs"]["method"]
-
-            # Rate limit locations are created for the endpoint
-            self.rate_limits["paths"].setdefault(path, {})[method] = dict(
-                user_limits={},
-                ip_limits={},
-                global_limits={}
-            )
+                return decorated_function
 
-            return decorated_function
         return decorator
 
     def tests(self, *args: Test):
         """
         Run tests on your endpoints to make sure they function properly and to help generate accurate OpenAPI schema
 
         The tests decorator can take an unlimited number of `Test` objects:
@@ -640,15 +652,15 @@
                 @functools.wraps(f)
                 def decorated_function(**kwargs):
                     return f(**kwargs)
                 return decorated_function
 
         return decorator
 
-    def run(self, host: str = None, port: int = None, tests: bool = False, swagger: str = None,
+    def run(self, host: str = None, port: int = None, tests: bool = False, swagger: str = None, print_test_responses: bool = False,
             threaded: bool = False, debug: bool = None, load_dotenv: bool = True, **kwargs):
         """
         Runs the application on a local development server.
 
         Do not use run() in a production setting. It is not intended to meet security and performance requirements for a production server.
          Instead, see /deploying/index for WSGI server recommendations. (From Flask run() docstring) - I recommend gunicorn for new developers
 
@@ -671,45 +683,45 @@
         def run_app():
             """ Run Flask development server inside thread """
             Flask.run(self, host=host, port=port, debug=debug, load_dotenv=load_dotenv, threaded=threaded, **kwargs)
 
         def test_thread(path, method, test):
             """ Thread for each endpoint test """
             nonlocal success_count, failed_count
-            test_response, test_success_count, test_failed_count = test.run(method=method, port=port)  # Run the test
+            test_response, test_success_count, test_failed_count = test.run(method=method, port=port, print_test_responses=print_test_responses)  # Run the test
             success_count += test_success_count
             failed_count += test_failed_count
-            response = self.swagger.paths[path][method].responses
+            if path in self.swagger.paths:
+                response = self.swagger.paths[path][method].responses
 
-            # Update the swagger.json to add the new Response Object based on the ran test
-            response[str(test_response.status_code)] = ResponseObject(
-                description=responses[test_response.status_code] or "",
-                content=Map()
-            )
+                # Update the swagger.json to add the new Response Object based on the ran test
+                response[str(test_response.status_code)] = ResponseObject(
+                    description=responses[test_response.status_code] or "",
+                    content=Map()
+                )
 
-            # Add schema to the Response Object using recursive generation
-            content = response[str(test_response.status_code)].content
-            content["application/json"] = MediaTypeObject(
-                schema=recursive_generation_of_json_response_schema(test_response.json())
-            )
+                # Add schema to the Response Object using recursive generation
+                content = response[str(test_response.status_code)].content
+                content["application/json"] = MediaTypeObject(
+                    schema=recursive_generation_of_json_response_schema(test_response.json())
+                )
 
-            # If an example is to be added it is set here (May be deprecated in future versions of the OpenAPI specification)
-            if test.example:
-                content["application/json"].schema["example"] = test_response
+                # If an example is to be added it is set here (May be deprecated in future versions of the OpenAPI specification)
+                if test.example:
+                    content["application/json"].schema["example"] = test_response
 
         color_print("-" * 90, color="white")
 
         if tests:
             app_thread = Thread(target=run_app, daemon=False)
             app_thread.start()  # API started here
             t0 = time.time()
             success_count, failed_count = 0, 0
 
             test_threads = set()
-
             for path, methods in self.endpoint_tests.items():
                 for method, tests in methods.items():
                     for test in tests:
                         # Each test has a thread spawned
                         test_threads.add(Thread(target=test_thread, kwargs=dict(path=path, method=method, test=test)))
             for test_thread in test_threads:
                 # Each test is run in parallel
```

### Comparing `speedyapi-1.0.4/speedyapi/parameters.py` & `speedyapi-1.0.5/speedyapi/parameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,17 +101,17 @@
     """  # Docstring repeated due to parent docstring not being passed by some IDEs
     pass
 
 
 class JsonBodyParameter(Parameter):
     """
     A Parameter object used for creating endpoint inputs that are provided via request body
-    
+
     This only supports json format payloads.
-    
+
         (Due to this not being a standard part of the OpenAPI specification or Redoc I add these as query parameters to swagger.json)
 
     :param name: The name of the parameter
     :param type: The data type of the parameter
     :param checks: Any checks that should be run on the parameter to make sure it meets the expected specification
     :param options: If there is only a select number of options the parameter should accept
     :param required: If the parameter is required for the endpoint
@@ -141,36 +141,44 @@
 
     else:
         raise InvalidParameter(parameter)
 
 
 def test_parameter_type(parameter_object):
     """ Check the parameter is an allowed type. """
-    if type(parameter_object) not in [PathParameter, QueryParameter, HeaderParameter, CookieParameter, JsonBodyParameter]:
+    if type(parameter_object) not in [PathParameter, QueryParameter, HeaderParameter, CookieParameter,
+                                      JsonBodyParameter]:
         raise TypeError("All arguments must be of type Parameter!")
 
 
 def input_handler(parameter: Parameter, **kwargs) -> dict | Response:
     request_inputs, parsed_inputs = get_request_inputs(parameter, **kwargs), {}
-    if (input_value := request_inputs.get(parameter.name, None)) is not None:  # Check if the parameter was provided with the request
+    if (input_value := request_inputs.get(parameter.name,
+                                          None)) is not None:  # Check if the parameter was provided with the request
         try:
             parameter.type(input_value)  # Check the type of the provided value
         except ValueError:
             return malformed(malformed_item=parameter.name)
         for check in (parameter.checks or []):  # Run checks on the provided value
             if not check(input_value):
                 return malformed(malformed_item=parameter.name)
         if parameter.options is not None:  # If options were limits check that the value is allowed
             if input_value not in parameter.options:
                 return malformed(malformed_item=parameter.name)
+        if parameter.type == Boolean:
+            input_value = True if input_value.lower() == "true" else False
         if parameter.type != String:
             try:
-                parsed_inputs[parameter.name] = ast.literal_eval(input_value)  # Attempt to convert to desired python type (literal_eval is safe to use do not worry)
+                parsed_inputs[parameter.name] = ast.literal_eval(
+                    input_value)  # Attempt to convert to desired python type (literal_eval is safe to use do not worry)
             except (ValueError, SyntaxError):
-                parsed_inputs[parameter.name] = input_value  # Value remains as a string to be parsed by the user in the request function context
+                parsed_inputs[
+                    parameter.name] = input_value  # Value remains as a string to be parsed by the user in the request function context
+        else:
+            parsed_inputs[parameter.name] = input_value
     elif parameter.required:  # Handle failure to provide required parameter with standard `missing` response
         return missing(missing_field=parameter.name)
     else:
         parsed_inputs[parameter.name] = parameter.default  # Set to the default parameter value
     return parsed_inputs
```

### Comparing `speedyapi-1.0.4/speedyapi/respond.py` & `speedyapi-1.0.5/speedyapi/respond.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json as json_lib
 
 from typing import Any
 from pygments import highlight
 from pygments.lexers import PythonLexer
 from pygments.formatters import HtmlFormatter
-from flask import redirect, send_file, Response
+from flask import redirect as redi, send_file, Response
 
 
 def json(data: dict | list | tuple | str | int | float | bool | None, status_code: int = 200, success_key: bool = True) -> Response:
     """
     :param data: data to send as json
     :param status_code: status code of the response
     :param success_key: Add {"success": True} key/value pair to the response
@@ -102,19 +102,19 @@
     return send_file(
         path_or_file=path_or_file,
         mimetype='image/gif',
         as_attachment=attachment
     )
 
 
-def redirect(redirect_url: str) -> redirect:
+def redirect(redirect_url: str) -> redi:
     """
     :param redirect_url: url to redirect user to
     """
-    return redirect(redirect_url, code=302)
+    return redi(redirect_url)
 
 
 def malformed(malformed_item: Any) -> Response:
     """
     :param malformed_item: input field that is malformed
     """
     return Response(
```

### Comparing `speedyapi-1.0.4/speedyapi/swagger.py` & `speedyapi-1.0.5/speedyapi/swagger.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                 obj[key[1:]] = obj.pop(key)
             if key == "logo":
                 obj["x-logo"] = obj.pop(key)
 
         return obj
 
 
-def redoc_html(title: str, server: str):
+def redoc_html(title: str, server: str, swagger_file: str = "swagger.json"):
     """
     :param title: The title of the page tab in browsers
     :param server: The server of the api to request the swagger.json from
 
     Credits: Redocly
     """
     return f"""<!DOCTYPE html>
@@ -110,15 +110,15 @@
       body {{
         margin: 0;
         padding: 0;
       }}
     </style>
   </head>
   <body>
-    <redoc spec-url="{server}swagger.json"></redoc>
+    <redoc spec-url="{server}{swagger_file}"></redoc>
     <script src="https://cdn.redoc.ly/redoc/latest/bundles/redoc.standalone.js"></script>
   </body>
 </html>"""
 
 
 def find_openapi_type(var):
     """ Convert python types to OpenAPI type strings """
@@ -152,10 +152,12 @@
     schema["type"] = type
 
     if type == "object":
         schema["properties"] = {}
         for key, sub_obj in obj.items():
             schema["properties"][key] = recursive_generation_of_json_response_schema(sub_obj)  # Recursion
     elif type == "array":
-        schema["items"] = recursive_generation_of_json_response_schema(obj[0])  # Recursion (Limits to the first object)
+        # TODO - needs to work for empty lists
+        if len(obj):
+            schema["items"] = recursive_generation_of_json_response_schema(obj[0])  # Recursion (Limits to the first object)
 
     return schema
```

### Comparing `speedyapi-1.0.4/speedyapi/swagger_objects.py` & `speedyapi-1.0.5/speedyapi/swagger_objects.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.4/speedyapi/util.py` & `speedyapi-1.0.5/speedyapi/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,18 @@
             for kw in n.keywords:
                 if "value" in vars(vars(kw)["value"]):  # Standard kwargs
                     decorators[node.name][name]["kwargs"][vars(kw)["arg"]] = vars(kw)["value"].value
                 else:
                     try:  # List kwargs 1
                         decorators[node.name][name]["kwargs"][vars(kw)["arg"]] = [x.value for x in vars(kw)["value"].values][0]
                     except AttributeError:  # List kwargs 2
-                        decorators[node.name][name]["kwargs"][vars(kw)["arg"]] = [x.value for x in vars(kw)["value"].elts]
+                        try:
+                            decorators[node.name][name]["kwargs"][vars(kw)["arg"]] = [x.value for x in vars(kw)["value"].elts]
+                        except:
+                            pass
 
     node_iter = ast.NodeVisitor()
 
     if is_async:
         node_iter.visit_AsyncFunctionDef = visit_func  # Async the visiting functon above to be used
     else:
         node_iter.visit_FunctionDef = visit_func  # Async the visiting functon above to be used
```

### Comparing `speedyapi-1.0.4/speedyapi.egg-info/PKG-INFO` & `speedyapi-1.0.5/speedyapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedyapi
-Version: 1.0.4
+Version: 1.0.5
 Summary: An easy to use Python module for creating API.
 Author: CodingYuno
 Project-URL: Source Code, https://github.com/CodingYuno/speedyapi/
 Project-URL: Issue Tracker, https://github.com/CodingYuno/speedyapi/issues/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -26,14 +26,18 @@
 - Parameter Parsing and Checking
 - API Authentication
 - Rate Limiting (user, address, global)
 - In-depth Endpoint Testing (Write tests to be run that confirm endpoints act as intended)
 - Automatic OpenAPI `swagger.json` Generation (with access to full specification)
 - Common JSON Response Formatting
 
+# Installation
+
+Simply run `pip install speedyapi`. The PyPI package is at https://pypi.org/project/speedyapi/
+
 # Dependencies
 
 - **[Python](https://www.python.org/downloads/)** 3.10
 - **[Requests](https://github.com/kennethreitz/requests)** >= 2.9.2
 - **[Flask](https://github.com/pallets/flask)** >= 2.2
 
 # Example Usage
```

