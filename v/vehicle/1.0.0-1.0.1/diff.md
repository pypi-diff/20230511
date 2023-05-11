# Comparing `tmp/vehicle-1.0.0.tar.gz` & `tmp/vehicle-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vehicle-1.0.0.tar", max compression
+gzip compressed data, was "vehicle-1.0.1.tar", max compression
```

## Comparing `vehicle-1.0.0.tar` & `vehicle-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2023-03-23 18:32:20.321193 vehicle-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     6174 2023-03-23 18:32:20.321193 vehicle-1.0.0/README.md
--rw-r--r--   0        0        0     3629 2023-03-23 18:32:41.793265 vehicle-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      465 2023-03-23 18:32:20.321193 vehicle-1.0.0/src/vehicle/__init__.py
--rw-r--r--   0        0        0     1462 2023-03-23 18:32:20.325193 vehicle-1.0.0/src/vehicle/const.py
--rw-r--r--   0        0        0      283 2023-03-23 18:32:20.325193 vehicle-1.0.0/src/vehicle/exceptions.py
--rw-r--r--   0        0        0     5577 2023-03-23 18:32:20.325193 vehicle-1.0.0/src/vehicle/models.py
--rw-r--r--   0        0        0        0 2023-03-23 18:32:20.325193 vehicle-1.0.0/src/vehicle/py.typed
--rw-r--r--   0        0        0     5072 2023-03-23 18:32:20.325193 vehicle-1.0.0/src/vehicle/rdw.py
--rw-r--r--   0        0        0     7583 1970-01-01 00:00:00.000000 vehicle-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-11 10:04:12.064142 vehicle-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0     6182 2023-05-11 10:04:12.064142 vehicle-1.0.1/README.md
+-rw-r--r--   0        0        0     3629 2023-05-11 10:04:26.552325 vehicle-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      465 2023-05-11 10:04:12.068142 vehicle-1.0.1/src/vehicle/__init__.py
+-rw-r--r--   0        0        0     1462 2023-05-11 10:04:12.068142 vehicle-1.0.1/src/vehicle/const.py
+-rw-r--r--   0        0        0      283 2023-05-11 10:04:12.068142 vehicle-1.0.1/src/vehicle/exceptions.py
+-rw-r--r--   0        0        0     5579 2023-05-11 10:04:12.068142 vehicle-1.0.1/src/vehicle/models.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:04:12.068142 vehicle-1.0.1/src/vehicle/py.typed
+-rw-r--r--   0        0        0     5082 2023-05-11 10:04:12.068142 vehicle-1.0.1/src/vehicle/rdw.py
+-rw-r--r--   0        0        0     7591 1970-01-01 00:00:00.000000 vehicle-1.0.1/PKG-INFO
```

### Comparing `vehicle-1.0.0/LICENSE.md` & `vehicle-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vehicle-1.0.0/README.md` & `vehicle-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 ## Contributing
 
 This is an active open-source project. We are always open to people who want to
 use the code or contribute to it.
 
 We've set up a separate document for our
-[contribution guidelines](CONTRIBUTING.md).
+[contribution guidelines](.github/CONTRIBUTING.md).
 
 Thank you for being involved! :heart_eyes:
 
 ## Setting up a development environment
 
 The easiest way to start, is by opening a CodeSpace here on GitHub, or by using
 the [Dev Container][devcontainer] feature of Visual Studio Code.
```

### Comparing `vehicle-1.0.0/pyproject.toml` & `vehicle-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,43 +18,43 @@
 maintainers = ["Franck Nijhof <opensource@frenck.dev>"]
 name = "vehicle"
 packages = [
   {include = "vehicle", from = "src"},
 ]
 readme = "README.md"
 repository = "https://github.com/frenck/python-vehicle"
-version = "1.0.0"
+version = "1.0.1"
 
 [tool.poetry.dependencies]
 aiohttp = ">=3.0.0"
 pydantic = "^1.8.0"
 python = "^3.10"
 yarl = ">=1.6.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/frenck/python-vehicle/issues"
 Changelog = "https://github.com/frenck/python-vehicle/releases"
 
 [tool.poetry.group.dev.dependencies]
 aresponses = "2.1.6"
-black = "23.1.0"
+black = "23.3.0"
 blacken-docs = "1.13.0"
 codespell = "2.2.4"
 covdefaults = "2.3.0"
-coverage = {version = "7.2.2", extras = ["toml"]}
-mypy = "1.1.1"
-pre-commit = "3.2.0"
+coverage = {version = "7.2.5", extras = ["toml"]}
+mypy = "1.3.0"
+pre-commit = "3.3.1"
 pre-commit-hooks = "4.4.0"
-pylint = "2.17.1"
-pytest = "7.2.2"
+pylint = "2.17.4"
+pytest = "7.3.1"
 pytest-asyncio = "0.21.0"
 pytest-cov = "4.0.0"
-ruff = "0.0.258"
+ruff = "0.0.265"
 safety = "2.4.0b1"
-yamllint = "1.30.0"
+yamllint = "1.31.0"
 
 [tool.coverage.report]
 show_missing = true
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
 source = ["vehicle"]
```

### Comparing `vehicle-1.0.0/src/vehicle/const.py` & `vehicle-1.0.1/src/vehicle/const.py`

 * *Files identical despite different names*

### Comparing `vehicle-1.0.0/src/vehicle/models.py` & `vehicle-1.0.1/src/vehicle/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         exported: Whether the vehicle is exported or not.
         first_admission: First date of registration.
         interior: Interior of the vehicle.
         last_odometer_registration_year: Last year odometer was registered.
         liability_insured: Whether the vehicle is insured or not.
         license_plate: Normalized license plate of the vehicle.
         list_price: List price of the vehicle.
-        mass_drivable: Mass of the vehicle when drivable in KG.
+        mass_driveable: Mass of the vehicle when driveable in KG.
         mass_empty: Empty mass of the vehicle in KG.
         model: Model of the vehicle.
         name_registration_date: Date of naming registration of the vehicle.
         name_registration_possible: Whether the vehicle is nameable or not.
         number_of_cylinders: Number of cylinders of the vehicle.
         number_of_doors: Number of doors of the vehicle.
         number_of_seats: Number of seats of the vehicle.
```

### Comparing `vehicle-1.0.0/src/vehicle/rdw.py` & `vehicle-1.0.1/src/vehicle/rdw.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         -------
             Normalized license plate.
         """
         return license_plate.upper().replace("-", "").replace(" ", "").strip()
 
     async def _request(
         self,
-        dataset: str,
+        dataset: Dataset,
         *,
         data: dict[str, Any] | None = None,
     ) -> dict[str, Any]:
         """Handle a request to a RDW open data (Socrata).
 
         A generic method for sending/handling HTTP requests done against
         the public RDW data.
@@ -64,15 +64,15 @@
         Raises:
         ------
             RDWConnectionError: An error occurred while communicating with
                 the Socrata API.
             RDWError: Received an unexpected response from the Socrata API.
         """
         version = metadata.version(__package__)
-        url = URL("https://opendata.rdw.nl/resource/").join(URL(f"{dataset}.json"))
+        url = URL("https://opendata.rdw.nl/resource/").join(URL(f"{dataset.value}.json"))
 
         headers = {
             "User-Agent": f"PythonVehicle/{version}",
             "Accept": "application/json, text/plain, */*",
         }
 
         if self.session is None:
```

### Comparing `vehicle-1.0.0/PKG-INFO` & `vehicle-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vehicle
-Version: 1.0.0
+Version: 1.0.1
 Summary: Asynchronous Python client providing RDW vehicle information.
 Home-page: https://github.com/frenck/python-vehicle
 License: MIT
 Keywords: rdw,vehicle,apk,api,async,client
 Author: Franck Nijhof
 Author-email: opensource@frenck.dev
 Maintainer: Franck Nijhof
@@ -97,15 +97,15 @@
 
 ## Contributing
 
 This is an active open-source project. We are always open to people who want to
 use the code or contribute to it.
 
 We've set up a separate document for our
-[contribution guidelines](CONTRIBUTING.md).
+[contribution guidelines](.github/CONTRIBUTING.md).
 
 Thank you for being involved! :heart_eyes:
 
 ## Setting up a development environment
 
 The easiest way to start, is by opening a CodeSpace here on GitHub, or by using
 the [Dev Container][devcontainer] feature of Visual Studio Code.
```

