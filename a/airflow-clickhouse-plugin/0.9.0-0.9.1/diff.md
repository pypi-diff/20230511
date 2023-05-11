# Comparing `tmp/airflow-clickhouse-plugin-0.9.0.tar.gz` & `tmp/airflow-clickhouse-plugin-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airflow-clickhouse-plugin-0.9.0.tar", last modified: Fri Nov 18 13:57:58 2022, max compression
+gzip compressed data, was "dist/airflow-clickhouse-plugin-0.9.1.tar", last modified: Thu Dec  1 12:50:13 2022, max compression
```

## Comparing `airflow-clickhouse-plugin-0.9.0.tar` & `airflow-clickhouse-plugin-0.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 abryzgalov   (503) staff       (20)        0 2022-11-18 13:57:58.052934 airflow-clickhouse-plugin-0.9.0/
--rw-r--r--   0 abryzgalov   (503) staff       (20)    20075 2022-11-18 13:57:58.052634 airflow-clickhouse-plugin-0.9.0/PKG-INFO
--rw-r--r--   0 abryzgalov   (503) staff       (20)    16263 2022-11-18 13:45:34.000000 airflow-clickhouse-plugin-0.9.0/README.md
-drwxr-xr-x   0 abryzgalov   (503) staff       (20)        0 2022-11-18 13:57:58.046348 airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin/
--rw-r--r--   0 abryzgalov   (503) staff       (20)        0 2021-03-13 10:01:50.000000 airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin/__init__.py
--rw-r--r--   0 abryzgalov   (503) staff       (20)      477 2022-11-18 11:56:13.000000 airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin/__version__.py
-drwxr-xr-x   0 abryzgalov   (503) staff       (20)        0 2022-11-18 13:57:58.049495 airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin/hooks/
--rw-r--r--   0 abryzgalov   (503) staff       (20)        0 2021-03-13 10:01:50.000000 airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin/hooks/__init__.py
--rw-r--r--   0 abryzgalov   (503) staff       (20)     4157 2022-11-18 11:31:17.000000 airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin/hooks/clickhouse_hook.py
-drwxr-xr-x   0 abryzgalov   (503) staff       (20)        0 2022-11-18 13:57:58.050688 airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin/operators/
--rw-r--r--   0 abryzgalov   (503) staff       (20)        0 2021-03-13 10:01:50.000000 airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin/operators/__init__.py
--rw-r--r--   0 abryzgalov   (503) staff       (20)     1022 2021-06-09 11:08:27.000000 airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin/operators/clickhouse_operator.py
-drwxr-xr-x   0 abryzgalov   (503) staff       (20)        0 2022-11-18 13:57:58.051754 airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin/sensors/
--rw-r--r--   0 abryzgalov   (503) staff       (20)        0 2021-03-13 10:01:50.000000 airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin/sensors/__init__.py
--rw-r--r--   0 abryzgalov   (503) staff       (20)     1205 2022-11-18 12:35:34.000000 airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin/sensors/clickhouse_sql_sensor.py
-drwxr-xr-x   0 abryzgalov   (503) staff       (20)        0 2022-11-18 13:57:58.048841 airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin.egg-info/
--rw-r--r--   0 abryzgalov   (503) staff       (20)    20075 2022-11-18 13:57:57.000000 airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin.egg-info/PKG-INFO
--rw-r--r--   0 abryzgalov   (503) staff       (20)      696 2022-11-18 13:57:57.000000 airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 abryzgalov   (503) staff       (20)        1 2022-11-18 13:57:57.000000 airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 abryzgalov   (503) staff       (20)        1 2022-11-18 13:57:57.000000 airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin.egg-info/not-zip-safe
--rw-r--r--   0 abryzgalov   (503) staff       (20)      101 2022-11-18 13:57:57.000000 airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin.egg-info/requires.txt
--rw-r--r--   0 abryzgalov   (503) staff       (20)       26 2022-11-18 13:57:57.000000 airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin.egg-info/top_level.txt
--rw-r--r--   0 abryzgalov   (503) staff       (20)       38 2022-11-18 13:57:58.053073 airflow-clickhouse-plugin-0.9.0/setup.cfg
--rwxr-xr-x   0 abryzgalov   (503) staff       (20)     1421 2022-11-18 11:54:54.000000 airflow-clickhouse-plugin-0.9.0/setup.py
+drwxr-xr-x   0 abryzgalov   (503) staff       (20)        0 2022-12-01 12:50:13.206700 airflow-clickhouse-plugin-0.9.1/
+-rw-r--r--   0 abryzgalov   (503) staff       (20)    22353 2022-12-01 12:50:13.206419 airflow-clickhouse-plugin-0.9.1/PKG-INFO
+-rw-r--r--   0 abryzgalov   (503) staff       (20)    17829 2022-12-01 12:45:12.000000 airflow-clickhouse-plugin-0.9.1/README.md
+drwxr-xr-x   0 abryzgalov   (503) staff       (20)        0 2022-12-01 12:50:13.200599 airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin/
+-rw-r--r--   0 abryzgalov   (503) staff       (20)        0 2021-03-13 10:01:50.000000 airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin/__init__.py
+-rw-r--r--   0 abryzgalov   (503) staff       (20)      477 2022-12-01 12:45:46.000000 airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin/__version__.py
+drwxr-xr-x   0 abryzgalov   (503) staff       (20)        0 2022-12-01 12:50:13.202970 airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin/hooks/
+-rw-r--r--   0 abryzgalov   (503) staff       (20)        0 2021-03-13 10:01:50.000000 airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin/hooks/__init__.py
+-rw-r--r--   0 abryzgalov   (503) staff       (20)     4157 2022-11-18 11:31:17.000000 airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin/hooks/clickhouse_hook.py
+drwxr-xr-x   0 abryzgalov   (503) staff       (20)        0 2022-12-01 12:50:13.204064 airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin/operators/
+-rw-r--r--   0 abryzgalov   (503) staff       (20)        0 2021-03-13 10:01:50.000000 airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin/operators/__init__.py
+-rw-r--r--   0 abryzgalov   (503) staff       (20)     1022 2021-06-09 11:08:27.000000 airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin/operators/clickhouse_operator.py
+drwxr-xr-x   0 abryzgalov   (503) staff       (20)        0 2022-12-01 12:50:13.205371 airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin/sensors/
+-rw-r--r--   0 abryzgalov   (503) staff       (20)        0 2021-03-13 10:01:50.000000 airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin/sensors/__init__.py
+-rw-r--r--   0 abryzgalov   (503) staff       (20)     1205 2022-11-18 12:35:34.000000 airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin/sensors/clickhouse_sql_sensor.py
+drwxr-xr-x   0 abryzgalov   (503) staff       (20)        0 2022-12-01 12:50:13.202475 airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin.egg-info/
+-rw-r--r--   0 abryzgalov   (503) staff       (20)    22353 2022-12-01 12:50:12.000000 airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 abryzgalov   (503) staff       (20)      696 2022-12-01 12:50:12.000000 airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 abryzgalov   (503) staff       (20)        1 2022-12-01 12:50:12.000000 airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 abryzgalov   (503) staff       (20)        1 2022-12-01 12:50:12.000000 airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 abryzgalov   (503) staff       (20)      137 2022-12-01 12:50:12.000000 airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin.egg-info/requires.txt
+-rw-r--r--   0 abryzgalov   (503) staff       (20)       26 2022-12-01 12:50:12.000000 airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin.egg-info/top_level.txt
+-rw-r--r--   0 abryzgalov   (503) staff       (20)       38 2022-12-01 12:50:13.206794 airflow-clickhouse-plugin-0.9.1/setup.cfg
+-rwxr-xr-x   0 abryzgalov   (503) staff       (20)     1421 2022-11-18 11:54:54.000000 airflow-clickhouse-plugin-0.9.1/setup.py
```

### Comparing `airflow-clickhouse-plugin-0.9.0/PKG-INFO` & `airflow-clickhouse-plugin-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-clickhouse-plugin
-Version: 0.9.0
+Version: 0.9.1
 Summary: airflow-clickhouse-plugin - Airflow plugin to execute ClickHouse commands and queries
 Home-page: https://github.com/bryzgaloff/airflow-clickhouse-plugin
 Author: Anton Bryzgalov
 Author-email: tony.bryzgaloff@gmail.com
 License: MIT License
 Description: # Airflow ClickHouse Plugin
         
@@ -29,15 +29,16 @@
             as various timeouts, `compression`, `secure`, etc through Airflow
             [Connection.extra][airflow-conn-extra] property.
         
         # Installation and dependencies
         
         `pip install -U airflow-clickhouse-plugin`
         
-        Dependencies: `apache-airflow` and `clickhouse-driver`.
+        Dependencies: `apache-airflow` with `apache-airflow-providers-common-sql`
+            (usually pre-packed with Airflow) and `clickhouse-driver`.
         
         ## Python and Airflow versions support
         
         Different versions of the plugin support different combinations of Python and
             Airflow versions. We _primarily_ support **Airflow 2.0+ and Python 3.7+**.
             If you need to use the plugin with older Python-Airflow combinations, pick a
             suitable plugin version:
@@ -179,14 +180,32 @@
             contain a JSON object which will be [deserialized][airflow-conn-dejson] and
             all of its properties will be passed as-is to the `Client`.
         
         For example, if Airflow connection contains `extra={"secure":true}` then
             the `Client.__init__` will receive `secure=True` keyword argument in
             addition to other non-empty connection attributes.
         
+        #### Compression
+        
+        You should install several packages to support compression. For example, for lz4:
+        
+        ```bash
+        pip3 install clickhouse-cityhash lz4
+        ```
+        
+        Then you should include `compression` parameter in airflow connection uri: `extra={"compression":"lz4"}`.  You can get 
+        additional information about extra options from [official documentation of clickhouse-driver](https://clickhouse-driver.readthedocs.io/en/latest/installation.html#installation-pypi)
+        
+        Connection URI should look like in the example below:
+        
+        `clickhouse://login:password@host:port/?compression=lz4`
+        
+        See [official documentation](https://airflow.apache.org/docs/apache-airflow/stable/howto/connection.html) to 
+        get more info about connections in Airflow.
+        
         ### Default values
         
         If the Airflow connection attribute is not set then it is not passed to the
             `Client` at all. In that case the default value of the corresponding
             [clickhouse_driver.Connection][ch-driver-connection] argument is used (e.g.
             `user` defaults to `'default'`).
         
@@ -304,51 +323,121 @@
             )
         ```
         
         # How to run tests
         
         ## Unit tests
         
-        From the root project directory: `python -m unittest discover -s tests/unit`
+        From the root project directory
+        
+        Using `make`:
+        
+        ```bash
+        make unit
+        ```
+        
+        Using `python`:
+        
+        ```bash
+        python -m unittest discover -s tests
+        ```
         
         ## Integration tests
         
         Integration tests require access to ClickHouse server. Tests use connection
             URI defined [via environment variable][airflow-conn-env]
             `AIRFLOW_CONN_CLICKHOUSE_DEFAULT` with `clickhouse://localhost` as default.
         
-        Run from the project root: `python -m unittest discover -s tests/integration` 
+        You can run ClickHouse server in a local Docker container using the following command:
+        
+        Using `make`:
+        
+        ```bash
+        make run-clickhouse
+        ```
+        
+        Using `shell`:
+        
+        ```bash
+        docker run -p 9000:9000 --ulimit nofile=262144:262144 -it clickhouse/clickhouse-server
+        ```
+        
+        And then run from the project root:
+        
+        Using `make`:
+        
+        ```bash
+        make integration
+        ```
+        
+        Using `python`:
+        
+        ```bash
+        python3 -m unittest discover -s tests/integration
+        ```
         
         ## All tests
         
-        From the root project directory: `python -m unittest discover -s tests`
+        From the root project directory:
+        
+        Using `make`:
+        
+        ```bash
+        make tests
+        ```
+        
+        Using `python`:
+        
+        ```bash
+        python3 -m unittest discover -s tests
+        ```
         
         ### Github Actions
         
         [GitHub Action][github-action-src] is set up for this project.
         
         ### Run tests using Docker
         
         Run ClickHouse server inside Docker:
         
+        Using `shell`:
+        
         ```bash
-        docker exec -it $(docker run --rm -d yandex/clickhouse-server) bash
+        docker exec -it $(docker run --rm -d clickhouse/clickhouse-server) bash
+        ```
+        
+        Using `make`:
+        
+        ```bash
+        make run-clickhouse-dind
         ```
         
         The above command will open `bash` inside the container.
         
         Install dependencies into container and run tests (execute inside container):
         
+        Using `python`:
+        
+        ```bash
+        apt-get update
+        apt-get install -y python3.10 python3-pip git make
+        git clone https://github.com/whisklabs/airflow-clickhouse-plugin.git
+        cd airflow-clickhouse-plugin
+        python3.10 -m pip install -r requirements.txt
+        python3.10 -m unittest discover -s tests
+        ```
+        
+        Using `make`:
+        
         ```bash
         apt-get update
-        apt-get install -y python3.8 python3-pip git
+        apt-get install -y python3.10 python3-pip git make
         git clone https://github.com/whisklabs/airflow-clickhouse-plugin.git
         cd airflow-clickhouse-plugin
-        python3.8 -m pip install -r requirements.txt
-        python3.8 -m unittest discover -s tests
+        make tests
         ```
         
         # Contributors
         
         * Created by Anton Bryzgalov, [@bryzgaloff](https://github.com/bryzgaloff), originally at [Whisk, Samsung](https://github.com/whisklabs)
         * Inspired by Viktor Taranenko, [@viktortnk](https://github.com/viktortnk) (Whisk, Samsung)
```

### Comparing `airflow-clickhouse-plugin-0.9.0/README.md` & `airflow-clickhouse-plugin-0.9.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -21,15 +21,16 @@
     as various timeouts, `compression`, `secure`, etc through Airflow
     [Connection.extra][airflow-conn-extra] property.
 
 # Installation and dependencies
 
 `pip install -U airflow-clickhouse-plugin`
 
-Dependencies: `apache-airflow` and `clickhouse-driver`.
+Dependencies: `apache-airflow` with `apache-airflow-providers-common-sql`
+    (usually pre-packed with Airflow) and `clickhouse-driver`.
 
 ## Python and Airflow versions support
 
 Different versions of the plugin support different combinations of Python and
     Airflow versions. We _primarily_ support **Airflow 2.0+ and Python 3.7+**.
     If you need to use the plugin with older Python-Airflow combinations, pick a
     suitable plugin version:
@@ -171,14 +172,32 @@
     contain a JSON object which will be [deserialized][airflow-conn-dejson] and
     all of its properties will be passed as-is to the `Client`.
 
 For example, if Airflow connection contains `extra={"secure":true}` then
     the `Client.__init__` will receive `secure=True` keyword argument in
     addition to other non-empty connection attributes.
 
+#### Compression
+
+You should install several packages to support compression. For example, for lz4:
+
+```bash
+pip3 install clickhouse-cityhash lz4
+```
+
+Then you should include `compression` parameter in airflow connection uri: `extra={"compression":"lz4"}`.  You can get 
+additional information about extra options from [official documentation of clickhouse-driver](https://clickhouse-driver.readthedocs.io/en/latest/installation.html#installation-pypi)
+
+Connection URI should look like in the example below:
+
+`clickhouse://login:password@host:port/?compression=lz4`
+
+See [official documentation](https://airflow.apache.org/docs/apache-airflow/stable/howto/connection.html) to 
+get more info about connections in Airflow.
+
 ### Default values
 
 If the Airflow connection attribute is not set then it is not passed to the
     `Client` at all. In that case the default value of the corresponding
     [clickhouse_driver.Connection][ch-driver-connection] argument is used (e.g.
     `user` defaults to `'default'`).
 
@@ -296,51 +315,121 @@
     )
 ```
 
 # How to run tests
 
 ## Unit tests
 
-From the root project directory: `python -m unittest discover -s tests/unit`
+From the root project directory
+
+Using `make`:
+
+```bash
+make unit
+```
+
+Using `python`:
+
+```bash
+python -m unittest discover -s tests
+```
 
 ## Integration tests
 
 Integration tests require access to ClickHouse server. Tests use connection
     URI defined [via environment variable][airflow-conn-env]
     `AIRFLOW_CONN_CLICKHOUSE_DEFAULT` with `clickhouse://localhost` as default.
 
-Run from the project root: `python -m unittest discover -s tests/integration` 
+You can run ClickHouse server in a local Docker container using the following command:
+
+Using `make`:
+
+```bash
+make run-clickhouse
+```
+
+Using `shell`:
+
+```bash
+docker run -p 9000:9000 --ulimit nofile=262144:262144 -it clickhouse/clickhouse-server
+```
+
+And then run from the project root:
+
+Using `make`:
+
+```bash
+make integration
+```
+
+Using `python`:
+
+```bash
+python3 -m unittest discover -s tests/integration
+```
 
 ## All tests
 
-From the root project directory: `python -m unittest discover -s tests`
+From the root project directory:
+
+Using `make`:
+
+```bash
+make tests
+```
+
+Using `python`:
+
+```bash
+python3 -m unittest discover -s tests
+```
 
 ### Github Actions
 
 [GitHub Action][github-action-src] is set up for this project.
 
 ### Run tests using Docker
 
 Run ClickHouse server inside Docker:
 
+Using `shell`:
+
 ```bash
-docker exec -it $(docker run --rm -d yandex/clickhouse-server) bash
+docker exec -it $(docker run --rm -d clickhouse/clickhouse-server) bash
+```
+
+Using `make`:
+
+```bash
+make run-clickhouse-dind
 ```
 
 The above command will open `bash` inside the container.
 
 Install dependencies into container and run tests (execute inside container):
 
+Using `python`:
+
+```bash
+apt-get update
+apt-get install -y python3.10 python3-pip git make
+git clone https://github.com/whisklabs/airflow-clickhouse-plugin.git
+cd airflow-clickhouse-plugin
+python3.10 -m pip install -r requirements.txt
+python3.10 -m unittest discover -s tests
+```
+
+Using `make`:
+
 ```bash
 apt-get update
-apt-get install -y python3.8 python3-pip git
+apt-get install -y python3.10 python3-pip git make
 git clone https://github.com/whisklabs/airflow-clickhouse-plugin.git
 cd airflow-clickhouse-plugin
-python3.8 -m pip install -r requirements.txt
-python3.8 -m unittest discover -s tests
+make tests
 ```
 
 # Contributors
 
 * Created by Anton Bryzgalov, [@bryzgaloff](https://github.com/bryzgaloff), originally at [Whisk, Samsung](https://github.com/whisklabs)
 * Inspired by Viktor Taranenko, [@viktortnk](https://github.com/viktortnk) (Whisk, Samsung)
```

### Comparing `airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin/hooks/clickhouse_hook.py` & `airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin/hooks/clickhouse_hook.py`

 * *Files identical despite different names*

### Comparing `airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin/operators/clickhouse_operator.py` & `airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin/operators/clickhouse_operator.py`

 * *Files identical despite different names*

### Comparing `airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin/sensors/clickhouse_sql_sensor.py` & `airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin/sensors/clickhouse_sql_sensor.py`

 * *Files identical despite different names*

### Comparing `airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin.egg-info/PKG-INFO` & `airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-clickhouse-plugin
-Version: 0.9.0
+Version: 0.9.1
 Summary: airflow-clickhouse-plugin - Airflow plugin to execute ClickHouse commands and queries
 Home-page: https://github.com/bryzgaloff/airflow-clickhouse-plugin
 Author: Anton Bryzgalov
 Author-email: tony.bryzgaloff@gmail.com
 License: MIT License
 Description: # Airflow ClickHouse Plugin
         
@@ -29,15 +29,16 @@
             as various timeouts, `compression`, `secure`, etc through Airflow
             [Connection.extra][airflow-conn-extra] property.
         
         # Installation and dependencies
         
         `pip install -U airflow-clickhouse-plugin`
         
-        Dependencies: `apache-airflow` and `clickhouse-driver`.
+        Dependencies: `apache-airflow` with `apache-airflow-providers-common-sql`
+            (usually pre-packed with Airflow) and `clickhouse-driver`.
         
         ## Python and Airflow versions support
         
         Different versions of the plugin support different combinations of Python and
             Airflow versions. We _primarily_ support **Airflow 2.0+ and Python 3.7+**.
             If you need to use the plugin with older Python-Airflow combinations, pick a
             suitable plugin version:
@@ -179,14 +180,32 @@
             contain a JSON object which will be [deserialized][airflow-conn-dejson] and
             all of its properties will be passed as-is to the `Client`.
         
         For example, if Airflow connection contains `extra={"secure":true}` then
             the `Client.__init__` will receive `secure=True` keyword argument in
             addition to other non-empty connection attributes.
         
+        #### Compression
+        
+        You should install several packages to support compression. For example, for lz4:
+        
+        ```bash
+        pip3 install clickhouse-cityhash lz4
+        ```
+        
+        Then you should include `compression` parameter in airflow connection uri: `extra={"compression":"lz4"}`.  You can get 
+        additional information about extra options from [official documentation of clickhouse-driver](https://clickhouse-driver.readthedocs.io/en/latest/installation.html#installation-pypi)
+        
+        Connection URI should look like in the example below:
+        
+        `clickhouse://login:password@host:port/?compression=lz4`
+        
+        See [official documentation](https://airflow.apache.org/docs/apache-airflow/stable/howto/connection.html) to 
+        get more info about connections in Airflow.
+        
         ### Default values
         
         If the Airflow connection attribute is not set then it is not passed to the
             `Client` at all. In that case the default value of the corresponding
             [clickhouse_driver.Connection][ch-driver-connection] argument is used (e.g.
             `user` defaults to `'default'`).
         
@@ -304,51 +323,121 @@
             )
         ```
         
         # How to run tests
         
         ## Unit tests
         
-        From the root project directory: `python -m unittest discover -s tests/unit`
+        From the root project directory
+        
+        Using `make`:
+        
+        ```bash
+        make unit
+        ```
+        
+        Using `python`:
+        
+        ```bash
+        python -m unittest discover -s tests
+        ```
         
         ## Integration tests
         
         Integration tests require access to ClickHouse server. Tests use connection
             URI defined [via environment variable][airflow-conn-env]
             `AIRFLOW_CONN_CLICKHOUSE_DEFAULT` with `clickhouse://localhost` as default.
         
-        Run from the project root: `python -m unittest discover -s tests/integration` 
+        You can run ClickHouse server in a local Docker container using the following command:
+        
+        Using `make`:
+        
+        ```bash
+        make run-clickhouse
+        ```
+        
+        Using `shell`:
+        
+        ```bash
+        docker run -p 9000:9000 --ulimit nofile=262144:262144 -it clickhouse/clickhouse-server
+        ```
+        
+        And then run from the project root:
+        
+        Using `make`:
+        
+        ```bash
+        make integration
+        ```
+        
+        Using `python`:
+        
+        ```bash
+        python3 -m unittest discover -s tests/integration
+        ```
         
         ## All tests
         
-        From the root project directory: `python -m unittest discover -s tests`
+        From the root project directory:
+        
+        Using `make`:
+        
+        ```bash
+        make tests
+        ```
+        
+        Using `python`:
+        
+        ```bash
+        python3 -m unittest discover -s tests
+        ```
         
         ### Github Actions
         
         [GitHub Action][github-action-src] is set up for this project.
         
         ### Run tests using Docker
         
         Run ClickHouse server inside Docker:
         
+        Using `shell`:
+        
         ```bash
-        docker exec -it $(docker run --rm -d yandex/clickhouse-server) bash
+        docker exec -it $(docker run --rm -d clickhouse/clickhouse-server) bash
+        ```
+        
+        Using `make`:
+        
+        ```bash
+        make run-clickhouse-dind
         ```
         
         The above command will open `bash` inside the container.
         
         Install dependencies into container and run tests (execute inside container):
         
+        Using `python`:
+        
+        ```bash
+        apt-get update
+        apt-get install -y python3.10 python3-pip git make
+        git clone https://github.com/whisklabs/airflow-clickhouse-plugin.git
+        cd airflow-clickhouse-plugin
+        python3.10 -m pip install -r requirements.txt
+        python3.10 -m unittest discover -s tests
+        ```
+        
+        Using `make`:
+        
         ```bash
         apt-get update
-        apt-get install -y python3.8 python3-pip git
+        apt-get install -y python3.10 python3-pip git make
         git clone https://github.com/whisklabs/airflow-clickhouse-plugin.git
         cd airflow-clickhouse-plugin
-        python3.8 -m pip install -r requirements.txt
-        python3.8 -m unittest discover -s tests
+        make tests
         ```
         
         # Contributors
         
         * Created by Anton Bryzgalov, [@bryzgaloff](https://github.com/bryzgaloff), originally at [Whisk, Samsung](https://github.com/whisklabs)
         * Inspired by Viktor Taranenko, [@viktortnk](https://github.com/viktortnk) (Whisk, Samsung)
```

### Comparing `airflow-clickhouse-plugin-0.9.0/airflow_clickhouse_plugin.egg-info/SOURCES.txt` & `airflow-clickhouse-plugin-0.9.1/airflow_clickhouse_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airflow-clickhouse-plugin-0.9.0/setup.py` & `airflow-clickhouse-plugin-0.9.1/setup.py`

 * *Files identical despite different names*

