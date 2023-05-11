# Comparing `tmp/volttron_sqlite_historian-0.1.1a9.tar.gz` & `tmp/volttron_sqlite_historian-0.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_sqlite_historian-0.1.1a9.tar", max compression
+gzip compressed data, was "volttron_sqlite_historian-0.2.0rc0.tar", max compression
```

## Comparing `volttron_sqlite_historian-0.1.1a9.tar` & `volttron_sqlite_historian-0.2.0rc0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11928 2022-11-30 00:05:35.185428 volttron_sqlite_historian-0.1.1a9/LICENSE
--rw-r--r--   0        0        0     3435 2022-11-30 00:05:35.185428 volttron_sqlite_historian-0.1.1a9/README.md
--rw-r--r--   0        0        0     1580 2022-11-30 00:06:45.985062 volttron_sqlite_historian-0.1.1a9/pyproject.toml
--rw-r--r--   0        0        0     1078 2022-11-30 00:05:35.185428 volttron_sqlite_historian-0.1.1a9/src/historian/sqlite/__init__.py
--rw-r--r--   0        0        0    30419 2022-11-30 00:05:35.185428 volttron_sqlite_historian-0.1.1a9/src/historian/sqlite/sqlitefuncts.py
--rw-r--r--   0        0        0     4451 1970-01-01 00:00:00.000000 volttron_sqlite_historian-0.1.1a9/setup.py
--rw-r--r--   0        0        0     4183 1970-01-01 00:00:00.000000 volttron_sqlite_historian-0.1.1a9/PKG-INFO
+-rw-r--r--   0        0        0    11928 2022-11-29 22:09:10.366783 volttron_sqlite_historian-0.2.0rc0/LICENSE
+-rw-r--r--   0        0        0     3435 2022-11-29 22:09:10.366783 volttron_sqlite_historian-0.2.0rc0/README.md
+-rw-r--r--   0        0        0     1581 2022-11-29 22:09:10.366783 volttron_sqlite_historian-0.2.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     1078 2022-11-29 22:09:10.366783 volttron_sqlite_historian-0.2.0rc0/src/historian/sqlite/__init__.py
+-rw-r--r--   0        0        0    30419 2022-11-29 22:09:10.366783 volttron_sqlite_historian-0.2.0rc0/src/historian/sqlite/sqlitefuncts.py
+-rw-r--r--   0        0        0     4452 1970-01-01 00:00:00.000000 volttron_sqlite_historian-0.2.0rc0/setup.py
+-rw-r--r--   0        0        0     4184 1970-01-01 00:00:00.000000 volttron_sqlite_historian-0.2.0rc0/PKG-INFO
```

### Comparing `volttron_sqlite_historian-0.1.1a9/LICENSE` & `volttron_sqlite_historian-0.2.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_sqlite_historian-0.1.1a9/README.md` & `volttron_sqlite_historian-0.2.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `volttron_sqlite_historian-0.1.1a9/pyproject.toml` & `volttron_sqlite_historian-0.2.0rc0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "volttron-sqlite-historian"
-version = "0.1.1a9"
+version = "0.2.0-rc"
 description = "None"
 authors = ["VOLTTRON Team <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/VOLTTRON/volttron-sqlite-historian"
 homepage = "https://github.com/VOLTTRON/volttron-sqlite-historian"
 keywords = []
```

### Comparing `volttron_sqlite_historian-0.1.1a9/src/historian/sqlite/__init__.py` & `volttron_sqlite_historian-0.2.0rc0/src/historian/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron_sqlite_historian-0.1.1a9/src/historian/sqlite/sqlitefuncts.py` & `volttron_sqlite_historian-0.2.0rc0/src/historian/sqlite/sqlitefuncts.py`

 * *Files identical despite different names*

### Comparing `volttron_sqlite_historian-0.1.1a9/setup.py` & `volttron_sqlite_historian-0.2.0rc0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 entry_points = \
 {'console_scripts': ['volttron-sqlite-historian = '
                      'historian.sql.historian:main']}
 
 setup_kwargs = {
     'name': 'volttron-sqlite-historian',
-    'version': '0.1.1a9',
+    'version': '0.2.0rc0',
     'description': 'None',
     'long_description': '[![Run Pytests](https://github.com/eclipse-volttron/volttron-sqlite-historian/actions/workflows/run-test.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-sqlite-historian/actions/workflows/run-test.yml)\n[![pypi version](https://img.shields.io/pypi/v/volttron-sqlite-historian.svg)](https://pypi.org/project/volttron-sqlite-historian/)\n\nVOLTTRON historian agent that stores data into a SQLite database\n\n\n## Requirements\n\n - Python >= 3.8\n\n## Installation\n\n1. Create and activate a virtual environment.\n\n   ```shell\n    python -m venv env\n    source env/bin/activate\n    ```\n\n2. Installing volttron-sqlite-historian requires a running volttron instance.\n\n    ```shell\n    pip install volttron\n    \n    # Start platform with output going to volttron.log\n    volttron -vv -l volttron.log &\n    ```\n\n3. Create a agent configuration file \n   SQLite historian supports two parameters\n    \n    - connection -  This is a mandatory parameter with type indicating the type of sql historian (i.e. sqlite) and params \n                    containing the path the database file.\n    \n    - tables_def - Optional parameter to provide custom table names for topics, data, and metadata.\n    \n    The configuration can be in a json or yaml formatted file.\n\n    Yaml Format:\n\n    ```yaml\n    connection:\n      # type should be sqlite\n      type: sqlite\n      params:\n        # Relative to the agents data directory\n        database: "data/historian.sqlite"\n    \n      tables_def:\n        # prefix for data, topics, and (in version < 4.0.0 metadata tables)\n        # default is ""\n        table_prefix: ""\n        # table name for time series data. default "data"\n        data_table: data\n        # table name for list of topics. default "topics"\n        topics_table: topics\n    ```\n    \n4. Install and start the volttron-sqlite-historian.\n\n    ```shell\n    vctl install volttron-sqlite-historian --agent-config <path to configuration> --start\n    ```\n\n5. View the status of the installed agent\n\n    ```shell\n    vctl status\n    ```\n\n## Development\n\nPlease see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).\n\nPlease see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)\n\n# Disclaimer Notice\n\nThis material was prepared as an account of work sponsored by an agency of the\nUnited States Government.  Neither the United States Government nor the United\nStates Department of Energy, nor Battelle, nor any of their employees, nor any\njurisdiction or organization that has cooperated in the development of these\nmaterials, makes any warranty, express or implied, or assumes any legal\nliability or responsibility for the accuracy, completeness, or usefulness or any\ninformation, apparatus, product, software, or process disclosed, or represents\nthat its use would not infringe privately owned rights.\n\nReference herein to any specific commercial product, process, or service by\ntrade name, trademark, manufacturer, or otherwise does not necessarily\nconstitute or imply its endorsement, recommendation, or favoring by the United\nStates Government or any agency thereof, or Battelle Memorial Institute. The\nviews and opinions of authors expressed herein do not necessarily state or\nreflect those of the United States Government or any agency thereof.\n',
     'author': 'VOLTTRON Team',
     'author_email': 'volttron@pnnl.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/VOLTTRON/volttron-sqlite-historian',
```

### Comparing `volttron_sqlite_historian-0.1.1a9/PKG-INFO` & `volttron_sqlite_historian-0.2.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-sqlite-historian
-Version: 0.1.1a9
+Version: 0.2.0rc0
 Summary: None
 Home-page: https://github.com/VOLTTRON/volttron-sqlite-historian
 License: Apache-2.0
 Author: VOLTTRON Team
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

