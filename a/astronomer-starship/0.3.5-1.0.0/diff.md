# Comparing `tmp/astronomer-starship-0.3.5.tar.gz` & `tmp/astronomer_starship-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astronomer-starship-0.3.5.tar", last modified: Fri Apr 14 13:38:10 2023, max compression
+gzip compressed data, was "astronomer_starship-1.0.0.tar", max compression
```

## Comparing `astronomer-starship-0.3.5.tar` & `astronomer_starship-1.0.0.tar`

### file list

```diff
@@ -1,60 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.412764 astronomer-starship-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-04-14 13:38:10.412764 astronomer-starship-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.404765 astronomer-starship-0.3.5/aeroscope/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/aeroscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/aeroscope/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.404765 astronomer-starship-0.3.5/aeroscope/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/aeroscope/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.404765 astronomer-starship-0.3.5/aeroscope/plugins/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.404765 astronomer-starship-0.3.5/aeroscope/plugins/templates/aeroscope/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/aeroscope/plugins/templates/aeroscope/formhelper.html
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/aeroscope/plugins/templates/aeroscope/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/aeroscope/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.408764 astronomer-starship-0.3.5/astronomer_starship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-04-14 13:38:10.000000 astronomer-starship-0.3.5/astronomer_starship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-14 13:38:10.000000 astronomer-starship-0.3.5/astronomer_starship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:38:10.000000 astronomer-starship-0.3.5/astronomer_starship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-14 13:38:10.000000 astronomer-starship-0.3.5/astronomer_starship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 13:38:10.000000 astronomer-starship-0.3.5/astronomer_starship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 13:38:10.000000 astronomer-starship-0.3.5/astronomer_starship.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-14 13:38:10.412764 astronomer-starship-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.408764 astronomer-starship-0.3.5/starship/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18705 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.408764 astronomer-starship-0.3.5/starship/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/services/astrohub_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/services/local_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.408764 astronomer-starship-0.3.5/starship/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.408764 astronomer-starship-0.3.5/starship/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    39433 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/static/js/htmx.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/static/js/idiomorph.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    20094 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/static/js/popper.js
--rw-r--r--   0 runner    (1001) docker     (123)    25717 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/static/js/tippy.js
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/static/tail-spin.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.404765 astronomer-starship-0.3.5/starship/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.408764 astronomer-starship-0.3.5/starship/templates/starship/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:38:10.412764 astronomer-starship-0.3.5/starship/templates/starship/components/
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/dag_row.html
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/env_checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/github_loop.html
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/migrate_connection_button.html
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/migrate_pool_button.html
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/migrate_variable_button.html
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/tabs.html
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/tabs_loading.html
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/target_deployment_select.html
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/target_deployment_select_loading.html
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/test_connection_label.html
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/token_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/components/user_label.html
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/connections.html
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/dags.html
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/env.html
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/main.html
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/migration.html
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/pools.html
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-14 13:37:55.000000 astronomer-starship-0.3.5/starship/templates/starship/variables.html
+-rw-r--r--   0        0        0      547 2023-05-11 00:58:10.489593 astronomer_starship-1.0.0/LICENSE
+-rw-r--r--   0        0        0     9187 2023-05-11 00:58:10.489593 astronomer_starship-1.0.0/README.rst
+-rw-r--r--   0        0        0        0 2023-05-11 00:58:10.489593 astronomer_starship-1.0.0/astronomer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 00:58:10.489593 astronomer_starship-1.0.0/astronomer/aeroscope/__init__.py
+-rw-r--r--   0        0        0     2434 2023-05-11 00:58:10.489593 astronomer_starship-1.0.0/astronomer/aeroscope/operators.py
+-rw-r--r--   0        0        0     4126 2023-05-11 00:58:10.489593 astronomer_starship-1.0.0/astronomer/aeroscope/plugins/__init__.py
+-rw-r--r--   0        0        0      262 2023-05-11 00:58:10.489593 astronomer_starship-1.0.0/astronomer/aeroscope/plugins/templates/aeroscope/formhelper.html
+-rw-r--r--   0        0        0     2524 2023-05-11 00:58:10.489593 astronomer_starship-1.0.0/astronomer/aeroscope/plugins/templates/aeroscope/main.html
+-rw-r--r--   0        0        0     1561 2023-05-11 00:58:10.489593 astronomer_starship-1.0.0/astronomer/aeroscope/util.py
+-rw-r--r--   0        0        0        0 2023-05-11 00:58:10.489593 astronomer_starship-1.0.0/astronomer/starship/__init__.py
+-rw-r--r--   0        0        0    13578 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/main.py
+-rw-r--r--   0        0        0     7950 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/operators.py
+-rw-r--r--   0        0        0        0 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/services/__init__.py
+-rw-r--r--   0        0        0     7180 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/services/astro_client.py
+-rw-r--r--   0        0        0     4318 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/services/local_airflow_client.py
+-rw-r--r--   0        0        0     5230 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/services/remote_airflow_client.py
+-rw-r--r--   0        0        0    39434 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/static/js/htmx.min.js
+-rw-r--r--   0        0        0     7015 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/static/js/idiomorph.min.js
+-rw-r--r--   0        0        0    20095 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/static/js/popper.js
+-rw-r--r--   0        0        0    25717 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/static/js/tippy.js
+-rw-r--r--   0        0        0     1309 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/static/tail-spin.svg
+-rw-r--r--   0        0        0     2926 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/templates/starship/components/dag_row.html
+-rw-r--r--   0        0        0      283 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/templates/starship/components/env_checkbox.html
+-rw-r--r--   0        0        0      200 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/templates/starship/components/github_loop.html
+-rw-r--r--   0        0        0      738 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/templates/starship/components/migrate_connection_button.html
+-rw-r--r--   0        0        0      360 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/templates/starship/components/migrate_pool_button.html
+-rw-r--r--   0        0        0      367 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/templates/starship/components/migrate_variable_button.html
+-rw-r--r--   0        0        0     1194 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/templates/starship/components/tabs.html
+-rw-r--r--   0        0        0     2088 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/templates/starship/components/tabs_loading.html
+-rw-r--r--   0        0        0     1661 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/templates/starship/components/target_deployment_select.html
+-rw-r--r--   0        0        0     1227 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/templates/starship/components/target_deployment_select_loading.html
+-rw-r--r--   0        0        0      177 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/templates/starship/components/test_connection_label.html
+-rw-r--r--   0        0        0     2644 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/templates/starship/components/token_modal.html
+-rw-r--r--   0        0        0       15 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/templates/starship/components/user_label.html
+-rw-r--r--   0        0        0     1759 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/templates/starship/connections.html
+-rw-r--r--   0        0        0     1089 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/templates/starship/dags.html
+-rw-r--r--   0        0        0     1847 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/templates/starship/env.html
+-rw-r--r--   0        0        0      775 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/templates/starship/main.html
+-rw-r--r--   0        0        0      980 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/templates/starship/migration.html
+-rw-r--r--   0        0        0     1415 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/templates/starship/pools.html
+-rw-r--r--   0        0        0     1376 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/templates/starship/variables.html
+-rw-r--r--   0        0        0     1363 2023-05-11 00:58:10.493593 astronomer_starship-1.0.0/astronomer/starship/variables/operators.py
+-rw-r--r--   0        0        0     2734 2023-05-11 00:58:10.505593 astronomer_starship-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9984 1970-01-01 00:00:00.000000 astronomer_starship-1.0.0/PKG-INFO
```

### Comparing `astronomer-starship-0.3.5/aeroscope/operators.py` & `astronomer_starship-1.0.0/astronomer/aeroscope/operators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import Sequence
-
 import datetime
 import json
 import logging
 import os
 import socket
 import urllib
 from contextlib import redirect_stderr, redirect_stdout
+from typing import Sequence
 
 from airflow.exceptions import AirflowFailException
 from airflow.models import BaseOperator
-from aeroscope.util import clean_airflow_report_output
+
+from astronomer.aeroscope.util import clean_airflow_report_output
 
 
 class AeroscopeOperator(BaseOperator):
     template_fields: Sequence[str] = ("presigned_url", "organization")
 
     def __init__(
         self,
@@ -33,30 +33,42 @@
 
         import requests
 
         VERSION = os.getenv("TELESCOPE_REPORT_RELEASE_VERSION", "latest")
         a = "airflow_report.pyz"
         if VERSION == "latest":
             self.log.info("Running Latest Version of report")
-            urlretrieve("https://github.com/astronomer/telescope/releases/latest/download/airflow_report.pyz", a)
+            urlretrieve(
+                "https://github.com/astronomer/telescope/releases/latest/download/airflow_report.pyz",
+                a,
+            )
         else:
             try:
                 self.log.info(f"Running Version {VERSION} of report")
                 urlretrieve(
-                    f"https://github.com/astronomer/telescope/releases/download/{VERSION}/airflow_report.pyz", a
+                    f"https://github.com/astronomer/telescope/releases/download/{VERSION}/airflow_report.pyz",
+                    a,
                 )
             except urllib.error.HTTPError as e:
-                raise AirflowFailException(f"Error finding specified version:{VERSION} -- Reason:{e.reason}")
+                raise AirflowFailException(
+                    f"Error finding specified version:{VERSION} -- Reason:{e.reason}"
+                )
         s = io.StringIO()
         with redirect_stdout(s), redirect_stderr(s):
             runpy.run_path(a)
         date = datetime.datetime.now(datetime.timezone.utc).isoformat()[:10]
         content = {
             "telescope_version": "aeroscope-latest",
             "report_date": date,
             "organization_name": self.organization,
-            "local": {socket.gethostname(): {"airflow_report": clean_airflow_report_output(s.getvalue())}},
+            "local": {
+                socket.gethostname(): {
+                    "airflow_report": clean_airflow_report_output(s.getvalue())
+                }
+            },
         }
         upload = requests.put(self.presigned_url, data=json.dumps(content))
         if not upload.ok:
-            logging.error(f"Upload failed with code {upload.status_code}::{upload.text}")
+            logging.error(
+                f"Upload failed with code {upload.status_code}::{upload.text}"
+            )
             upload.raise_for_status()
```

### Comparing `astronomer-starship-0.3.5/aeroscope/plugins/__init__.py` & `astronomer_starship-1.0.0/astronomer/aeroscope/plugins/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,103 @@
 import datetime
 import json
 import os
 import socket
 import urllib.error
 from contextlib import redirect_stderr, redirect_stdout
+from textwrap import dedent
 
+import io
+import runpy
+from urllib.request import urlretrieve
 import requests
-from airflow.configuration import conf
 from airflow.plugins_manager import AirflowPlugin
-from aeroscope.util import clean_airflow_report_output
-from flask import Blueprint, Response, flash, redirect, request
+from flask import Blueprint, Response, flash, request
 from flask_appbuilder import BaseView as AppBuilderBaseView
 from flask_appbuilder import expose
 from wtforms import Form, StringField, validators
 
+from astronomer.aeroscope.util import clean_airflow_report_output
+
 bp = Blueprint(
     "starship_aeroscope",
     __name__,
     template_folder="templates",  # registers airflow/plugins/templates as a Jinja template folder
     static_folder="static",
     static_url_path="/static/aeroscope",
 )
 
 
 class AeroForm(Form):
     organization = StringField("Organization", [validators.Length(min=4, max=25)])
-    presigned_url = StringField("Pre-signed URL (optional)", [validators.URL(), validators.optional()])
+    presigned_url = StringField(
+        "Pre-signed URL (optional)",
+        description=dedent(
+            """The pre-signed URL field is optional and is to be supplied by an Astronomer Representative.
+    If the pre-signed URL is used, the results of the Telescope Report is shipped to Astronomer."""
+        ),
+        validators=[validators.URL(), validators.optional()],
+    )
 
 
 # Creating a flask appbuilder BaseView
 class StarshipAeroscope(AppBuilderBaseView):
     default_view = "aeroscope"
 
     @expose("/", methods=("GET", "POST"))
     def aeroscope(self):
         form = AeroForm(request.form)
-        if request.method == "POST" and form.validate() and request.form["action"] == "Download":
-
-            import io
-            import runpy
-            from urllib.request import urlretrieve
-
+        if (
+            request.method == "POST"
+            and form.validate()
+            and request.form["action"] == "Send/Download Report"
+        ):
             VERSION = os.getenv("TELESCOPE_REPORT_RELEASE_VERSION", "latest")
             a = "airflow_report.pyz"
             if VERSION == "latest":
-                urlretrieve("https://github.com/astronomer/telescope/releases/latest/download/airflow_report.pyz", a)
+                urlretrieve(
+                    "https://github.com/astronomer/telescope/releases/latest/download/airflow_report.pyz",
+                    a,
+                )
             else:
                 try:
                     urlretrieve(
-                        f"https://github.com/astronomer/telescope/releases/download/{VERSION}/airflow_report.pyz", a
+                        f"https://github.com/astronomer/telescope/releases/download/{VERSION}/airflow_report.pyz",
+                        a,
                     )
                 except urllib.error.HTTPError as e:
-                    flash(f"Error finding specified version:{VERSION} -- Reason:{e.reason}")
+                    flash(
+                        f"Error finding specified version:{VERSION} -- Reason:{e.reason}"
+                    )
             s = io.StringIO()
             with redirect_stdout(s), redirect_stderr(s):
                 runpy.run_path(a)
             date = datetime.datetime.now(datetime.timezone.utc).isoformat()[:10]
             content = {
                 "telescope_version": "aeroscope-latest",
                 "report_date": date,
                 "organization_name": form.organization.data,
-                "local": {socket.gethostname(): {"airflow_report": clean_airflow_report_output(s.getvalue())}},
+                "local": {
+                    socket.gethostname(): {
+                        "airflow_report": clean_airflow_report_output(s.getvalue())
+                    }
+                },
             }
             if len(form.presigned_url.data) > 1:
                 upload = requests.put(form.presigned_url.data, data=json.dumps(content))
                 if upload.ok:
                     flash("Upload successful")
                 else:
                     flash(upload.reason, "error")
             filename = f"{date}.{form.organization.data}.data.json"
             return Response(
                 json.dumps(content),
                 mimetype="application/json",
                 headers={"Content-Disposition": f"attachment;filename={filename}"},
             )
-        elif request.method == "POST" and request.form["action"] == "Back to Airflow":
-            return redirect(conf.get("webserver", "base_url"))
-
         else:
             return self.render_template("aeroscope/main.html", form=form)
 
 
 v_appbuilder_view = StarshipAeroscope()
```

### Comparing `astronomer-starship-0.3.5/aeroscope/util.py` & `astronomer_starship-1.0.0/astronomer/aeroscope/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 def clean_airflow_report_output(log_string: str) -> Union[dict, str]:
     r"""Look for the magic string from the Airflow report and then decode the base64 and convert to json
     Or return output as a list, trimmed and split on newlines
     >>> clean_airflow_report_output('INFO 123 - xyz - abc\n\n\nERROR - 1234\n%%%%%%%\naGVsbG8gd29ybGQ=')
     'hello world'
-    >>> clean_airflow_report_output('INFO 123 - xyz - abc\n\n\nERROR - 1234\n%%%%%%%\neyJvdXRwdXQiOiAiaGVsbG8gd29ybGQifQ==')
+    >>> clean_airflow_report_output('INFO 123-xyz - abc\n\nERROR-1234\n%%%%%%%\neyJvdXRwdXQiOiAiaGVsbG8gd29ybGQifQ==')
     {'output': 'hello world'}
     """
 
     def get_json_or_clean_str(o: str) -> Union[List[Any], Dict[Any, Any], Any]:
         """Either load JSON (if we can) or strip and split the string, while logging the error"""
         try:
             return json.loads(o)
@@ -28,14 +28,16 @@
     enumerated_log_lines = list(enumerate(log_lines))
     found_i = -1
     for i, line in enumerated_log_lines:
         if "%%%%%%%" in line:
             found_i = i + 1
             break
     if found_i != -1:
-        output = base64.decodebytes("\n".join(log_lines[found_i:]).encode("utf-8")).decode("utf-8")
+        output = base64.decodebytes(
+            "\n".join(log_lines[found_i:]).encode("utf-8")
+        ).decode("utf-8")
         try:
             return json.loads(output)
         except JSONDecodeError:
             return get_json_or_clean_str(output)
     else:
         return get_json_or_clean_str(log_string)
```

### Comparing `astronomer-starship-0.3.5/starship/main.py` & `astronomer_starship-1.0.0/astronomer/starship/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,161 +1,100 @@
 import os
-from urllib.parse import urlparse
-
-from cachetools.func import ttl_cache
+import logging
+from typing import Optional
+import jwt
 from airflow.plugins_manager import AirflowPlugin
-from airflow import models
-
-from airflow.www import auth
 from airflow.security import permissions
-
-import jwt
-
-from flask import Blueprint, session, request, redirect, url_for
-from flask_appbuilder import expose, BaseView as AppBuilderBaseView
-
-from starship.services.astrohub_client import AstroClient
-from starship.services.local_client import LocalAirflowClient
-
-import requests
-
-from pydash import at
-
-from python_graphql_client import GraphqlClient
+from airflow.www import auth
+from airflow.www.app import csrf
+from flask import Blueprint, Response, redirect, request, session, url_for
+from flask_appbuilder import BaseView as AppBuilderBaseView
+from flask_appbuilder import expose
+
+from astronomer.starship.services import (
+    astro_client,
+    local_airflow_client,
+    remote_airflow_client,
+)
+from astronomer.starship.services.astro_client import is_environment_variable_migrated
+from astronomer.starship.services.remote_airflow_client import is_pool_migrated
 
 bp = Blueprint(
     "starship",
     __name__,
     template_folder="templates",
     static_folder="static",
     static_url_path="/static/starship",
 )
 
 
-class AstroMigration(AppBuilderBaseView):
-    default_view = "main"
-
-    def __init__(self):
-        super().__init__()
-        self.local_client: LocalAirflowClient = LocalAirflowClient()
-        self.astro_client: AstroClient = AstroClient()
-
-    def get_astro_username(self, token):
-        if not token:
-            pass
-
-        headers = {"Authorization": f"Bearer {token}"}
-        client = GraphqlClient(
-            endpoint="https://api.astronomer.io/hub/v1", headers=headers
-        )
-
-        query = "{self {user {username}}}"
-
-        try:
-            api_rv = at(client.execute(query), "data.self.user.username")[0]
-
-            return api_rv
-        except Exception as exc:
-            print(exc)
-            return None
-
-    @ttl_cache(ttl=30)
-    def astro_orgs(self, token):
-        if not token:
-            return {}
-
-        headers = {"Authorization": f"Bearer {token}"}
-        url = "https://api.astronomer.io/v1alpha1/organizations"
-
-        try:
-            api_rv = requests.get(url, headers=headers).json()
-
-            return {org["id"]: org for org in (api_rv or [])}
-        except Exception as exc:
-            print(exc)
-            return {}
-
-
-    @ttl_cache(ttl=30)
-    def astro_deployments(self, token):
-        if not token:
-            return {}
-
-        headers = {"Authorization": f"Bearer {token}"}
-
-        orgs = self.astro_orgs(token)
-        short_name = os.getenv("STARSHIP_ORG_SHORTNAME", [_ for _ in orgs.values()][0]['shortName'])
-
-        # FIXME use the first org for now. change to a select in the near term.
-        url = f"https://api.astronomer.io/v1alpha1/organizations/{short_name}/deployments"
-
-        try:
-            api_rv = requests.get(url, headers=headers).json()["deployments"]
-
-            return {deploy["id"]: deploy for deploy in (api_rv or [])}
-        except Exception as exc:
-            print(exc)
-            return {}
-
-    def get_astro_config(self, deployment_url: str, token: str):
-        resp = requests.get(
-            f"{deployment_url}/api/v1/config",
-            headers={"Authorization": f"Bearer {token}"},
-        )
-        return resp.json()
-
-    def get_astro_variables(self, deployment_url: str, token: str):
-        resp = requests.get(
-            f"{deployment_url}/api/v1/variables",
-            headers={"Authorization": f"Bearer {token}"},
-        )
-        return resp.json()["variables"]
+def get_page_data(page):
+    return {
+        "AstroMigration.tabs_vars": {
+            "component": "variables",
+            "vars": {var.key: var for var in local_airflow_client.get_variables()},
+        },
+        "AstroMigration.tabs_dags": {
+            "component": "dags",
+            "dags": local_airflow_client.get_dags(),
+        },
+        "AstroMigration.tabs_pools": {
+            "component": "pools",
+            "pools": {pool.pool: pool for pool in local_airflow_client.get_pools()},
+        },
+        "AstroMigration.tabs_conns": {
+            "component": "connections",
+            "conns": {
+                conn.conn_id: conn for conn in local_airflow_client.get_connections()
+            },
+        },
+        "AstroMigration.tabs_env": {
+            "component": "env",
+            "environ": os.environ,
+        },
+    }[page]
 
-    def get_astro_pools(self, deployment_url: str, token: str):
-        resp = requests.get(
-            f"{deployment_url}/api/v1/pools",
-            headers={"Authorization": f"Bearer {token}"},
-        )
-        return resp.json()["pools"]
 
-    @ttl_cache(ttl=1)
-    def get_astro_connections(self, deployment_url: str, token: str):
-        resp = requests.get(
-            f"{deployment_url}/api/v1/connections",
-            headers={"Authorization": f"Bearer {token}"},
-        )
-        return resp.json()["connections"]
+class AstroMigration(AppBuilderBaseView):
+    default_view = "main"
 
     @expose("/", methods=["GET", "POST"])
     @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_CONFIG)])
     def main(self):
         session.update(request.form)
-        return self.render_template("starship/main.html")
+        return self.render_template(
+            "starship/main.html",
+            data={"tab": session.get("tab", "AstroMigration.tabs_conns")},
+        )
 
-    @staticmethod
-    @ttl_cache(ttl=3600)
-    def get_jwk(token: str):
-        jwks_url = "https://auth.astronomer.io/.well-known/jwks.json"
-        jwks_client = jwt.PyJWKClient(jwks_url)
-        return jwks_client.get_signing_key_from_jwt(token)
+    @expose("/dag_history/receive", methods=["GET", "POST"])
+    @csrf.exempt
+    def receive_dag_history(self):
+        data = request.json
+        try:
+            local_airflow_client.receive_dag(data=data)
+            return Response("OK", 200)
+        except Exception as e:
+            logging.exception(e)
+            return Response(str(e), 200)
 
     @expose("/modal/token")
     def modal_token_entry(self):
         token = session.get("token")
 
         if not token:
             return self.render_template(
                 "starship/components/token_modal.html", show=True, error=None
             )
 
         try:
             jwt.decode(
                 token,
                 audience=["astronomer-ee"],
-                key=self.get_jwk(token).key,
+                key=astro_client.get_jwk(token).key,
                 algorithms=["RS256"],
             )
         except jwt.exceptions.ExpiredSignatureError:
             return self.render_template(
                 "starship/components/token_modal.html", show=True, error="expired"
             )
         except jwt.exceptions.InvalidTokenError:
@@ -165,101 +104,75 @@
 
         return self.render_template("starship/components/token_modal.html", show=False)
 
     @expose("/button/save_token", methods=("POST",))
     @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_CONFIG)])
     def button_save_token(self):
         session["token"] = request.form.get("astroUserToken")
-        return self.render_template("starship/migration.html")
+        tab = session.get("tab", "AstroMigration.tabs_conns")
+        return self.render_template("starship/migration.html", data={"tab": tab})
 
     @expose("/tabs/dags")
     @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_DAG)])
     def tabs_dags(self):
-        data = {"component": "dags", "dags": self.local_client.get_dags()}
-
-        self.local_client.get_dags()
-
-        return self.render_template("starship/dags.html", data=data)
+        session["tab"] = "AstroMigration.tabs_dags"
+        return self.render_template(
+            "starship/dags.html", data=get_page_data(session["tab"])
+        )
 
     @expose("/tabs/variables")
     @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_VARIABLE)])
     def tabs_vars(self):
-        data = {
-            "component": "variables",
-            "vars": {var.key: var for var in self.local_client.get_variables()},
-        }
-
-        return self.render_template("starship/variables.html", data=data)
+        session["tab"] = "AstroMigration.tabs_vars"
+        return self.render_template(
+            "starship/variables.html", data=get_page_data(session["tab"])
+        )
 
     @expose("/tabs/pools")
     @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_VARIABLE)])
     def tabs_pools(self):
-        data = {
-            "component": "pools",
-            "pools": {pool.pool: pool for pool in self.local_client.get_pools()},
-        }
-
-        return self.render_template("starship/pools.html", data=data)
+        session["tab"] = "AstroMigration.tabs_pools"
+        return self.render_template(
+            "starship/pools.html", data=get_page_data(session["tab"])
+        )
 
     @expose("/tabs/connections")
     @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_CONNECTION)])
     def tabs_conns(self):
-        data = {
-            "component": "connections",
-            "conns": {
-                conn.conn_id: conn for conn in self.local_client.get_connections()
-            },
-        }
-
-        return self.render_template("starship/connections.html", data=data)
+        session["tab"] = "AstroMigration.tabs_conns"
+        return self.render_template(
+            "starship/connections.html", data=get_page_data(session["tab"])
+        )
 
     @expose("/tabs/env")
     @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_CONFIG)])
     def tabs_env(self):
-        import os
-
-        data = {
-            "component": "env",
-            "environ": os.environ,
-        }
-
-        return self.render_template("starship/env.html", data=data)
+        session["tab"] = "AstroMigration.tabs_env"
+        return self.render_template(
+            "starship/env.html", data=get_page_data(session["tab"])
+        )
 
     @expose(
         "/button_migrate_connection/<string:deployment>/<string:conn_id>",
         methods=("GET", "POST"),
     )
     @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_CONNECTION)])
     def button_migrate_connection(self, conn_id: str, deployment: str):
-        deployment_url = self.get_deployment_url(deployment)
+        token = session.get("token")
+        deployment_url = astro_client.get_deployment_url(deployment, token)
 
         if request.method == "POST":
             local_connections = {
-                conn.conn_id: conn for conn in self.local_client.get_connections()
+                conn.conn_id: conn for conn in local_airflow_client.get_connections()
             }
-
-            r = requests.post(
-                f"{deployment_url}/api/v1/connections",
-                headers={"Authorization": f"Bearer {session.get('token')}"},
-                json={
-                    "connection_id": local_connections[conn_id].conn_id,
-                    "conn_type": local_connections[conn_id].conn_type,
-                    "host": local_connections[conn_id].host,
-                    "login": local_connections[conn_id].login,
-                    "schema": local_connections[conn_id].schema,
-                    "port": local_connections[conn_id].port,
-                    "password": local_connections[conn_id].password or "",
-                    "extra": local_connections[conn_id].extra,
-                },
+            remote_airflow_client.create_connection(
+                deployment_url, token, local_connections[conn_id]
             )
-            r.raise_for_status()
 
-        deployment_conns = self.get_astro_connections(
-            deployment_url, session.get("token")
-        )
+        deployment_conns = remote_airflow_client.get_connections(deployment_url, token)
 
         is_migrated = conn_id in [
             remote_conn["connection_id"] for remote_conn in deployment_conns
         ]
 
         return self.render_template(
             "starship/components/migrate_connection_button.html",
@@ -267,274 +180,186 @@
             deployment=deployment,
             is_migrated=is_migrated,
         )
 
     @expose("/label_test_connection/<string:deployment>/<string:conn_id>")
     @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_CONNECTION)])
     def label_test_connection(self, conn_id: str, deployment: str):
-        if not os.getenv("ENABLE_CONN_TEST"):
-            return "🟡"
-
-        deployment_url = self.get_deployment_url(deployment)
+        token = session.get("token")
+        deployment_url = astro_client.get_deployment_url(deployment, token)
 
-        local_connections = {
-            conn.conn_id: conn for conn in self.local_client.get_connections()
-        }
-
-        rv = requests.post(
-            f"{deployment_url}/api/v1/connections/test",
-            headers={"Authorization": f"Bearer {session.get('token')}"},
-            json={
-                "connection_id": local_connections[conn_id].conn_id,
-                "conn_type": local_connections[conn_id].conn_type,
-                "host": local_connections[conn_id].host,
-                "login": local_connections[conn_id].login,
-                "schema": local_connections[conn_id].schema,
-                "port": local_connections[conn_id].port,
-                "password": local_connections[conn_id].password or "",
-                "extra": local_connections[conn_id].extra,
-            },
+        local_connection = {
+            conn.conn_id: conn for conn in local_airflow_client.get_connections()
+        }[conn_id]
+        r = remote_airflow_client.do_test_connection(
+            deployment_url, token, local_connection
         )
 
         return self.render_template(
-            "starship/components/test_connection_label.html", data=rv.json(), conn_id=conn_id
+            "starship/components/test_connection_label.html",
+            data=r.json(),
+            conn_id=conn_id,
         )
 
     @expose(
         "/button/migrate/var/<string:deployment>/<string:variable>",
         methods=("GET", "POST"),
     )
     @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_VARIABLE)])
     def button_migrate_variable(self, variable: str, deployment: str):
-        deployment_url = self.get_deployment_url(deployment)
+        token = session.get("token")
+        deployment_url = astro_client.get_deployment_url(deployment, token)
 
         if request.method == "POST":
-            local_vars = {var.key: var for var in self.local_client.get_variables()}
-
-            r = requests.post(
-                f"{deployment_url}/api/v1/variables",
-                headers={"Authorization": f"Bearer {session.get('token')}"},
-                json={"key": variable, "value": local_vars[variable].val},
+            remote_airflow_client.create_variable(
+                deployment_url, token, local_airflow_client.get_variable(variable)
             )
-            r.raise_for_status()
 
-        remote_vars = self.get_astro_variables(deployment_url, session.get("token"))
-
-        is_migrated = variable in [remote_var["key"] for remote_var in remote_vars]
+        is_migrated = remote_airflow_client.is_variable_migrated(
+            deployment_url, token, variable
+        )
 
         return self.render_template(
             "starship/components/migrate_variable_button.html",
             variable=variable,
             deployment=deployment,
             is_migrated=is_migrated,
         )
 
     @expose(
         "/button/migrate/pool/<string:deployment>/<string:pool_name>",
         methods=("GET", "POST"),
     )
     @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_VARIABLE)])
-    def button_migrate_pool(self, pool_name: str, deployment: str):
-        deployment_url = self.get_deployment_url(deployment)
-
-        if request.method == "POST":
-            pool = [p for p in self.local_client.get_pools() if p.pool == pool_name][0]
-
-            r = requests.post(
-                f"{deployment_url}/api/v1/pools",
-                headers={"Authorization": f"Bearer {session.get('token')}"},
-                json={"name": pool_name, "slots": pool.slots, "description": pool.description},
-            )
-            print(r.request.body)
-            r.raise_for_status()
-
-        remote_vars = self.get_astro_pools(deployment_url, session.get("token"))
+    def button_migrate_pool(self, pool_name: str, deployment: Optional[str] = None):
+        token = session.get("token")
+        if deployment:
+            deployment_url = astro_client.get_deployment_url(deployment, token)
 
-        is_migrated = any((True for remote_var in remote_vars if remote_var.get("name", "") == pool_name))
+            if request.method == "POST":
+                pool = local_airflow_client.get_pool(pool_name)
+                remote_airflow_client.create_pool(deployment_url, token, pool)
+
+            is_migrated = is_pool_migrated(deployment_url, token, pool_name)
+        else:
+            # Deployment hasn't been selected yet
+            is_migrated = False
 
         return self.render_template(
             "starship/components/migrate_pool_button.html",
             pool=pool_name,
             deployment=deployment,
             is_migrated=is_migrated,
         )
 
     @expose("/button/migrate/env/<string:deployment>", methods=("POST",))
     @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_CONFIG)])
     def button_migrate_env(self, deployment: str):
-        import os
-
-        deployments = self.astro_deployments(session.get("token"))
-
-        headers = {"Authorization": f"Bearer {session.get('token')}"}
-        client = GraphqlClient(
-            endpoint="https://api.astronomer.io/hub/v1", headers=headers
-        )
-
-        query = """
-        fragment EnvironmentVariable on EnvironmentVariable {
-            key
-            value
-            isSecret
-            updatedAt
-        }
-        mutation deploymentVariablesUpdate($input: EnvironmentVariablesInput!) {
-            deploymentVariablesUpdate(input: $input) {
-                ...EnvironmentVariable
-            }
-        }
-        """
-
-        remote_vars = {
-            remote_var["key"]: {
-                "key": remote_var["key"],
-                "value": remote_var["value"],
-                "isSecret": remote_var["isSecret"],
-            }
-            for remote_var in deployments[deployment]["deploymentSpec"][
-                "environmentVariables"
-            ]
-        }
-
-        for _, key in (
-                (key, value)
-                for (key, value) in request.form.items()
-                if key != "csrf_token" and key not in remote_vars.keys()
-        ):
-            remote_vars.setdefault(
-                key,
-                {
-                    "key": key,
-                    "value": os.environ[key],
-                    "isSecret": False,
-                },
-            )
-
-        client.execute(
-            query,
-            {
-                "input": {
-                    "deploymentId": deployment,
-                    "environmentVariables": list(remote_vars.values()),
-                }
-            },
+        token = session.get("token")
+        items = dict(**request.form)
+        del items["csrf_token"]
+        astro_client.set_changed_environment_variables(
+            deployment, token, iter(items.values())
         )
-
         return self.tabs_env()
 
     @expose("/checkbox/migrate/env/<string:deployment>/<string:key>/", methods=("GET",))
     @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_CONFIG)])
     def checkbox_migrate_env(self, key: str, deployment: str):
-        deployments = self.astro_deployments(session.get("token"))
-
-        remote_vars = {
-            remote_var["key"]: {
-                "key": remote_var["key"],
-                "value": remote_var["value"],
-                "isSecret": remote_var["isSecret"],
-            }
-            for remote_var in deployments[deployment]["deploymentSpec"][
-                "environmentVariables"
-            ]
-        }
-
-        is_migrated = key in remote_vars.keys()
-
+        token = session.get("token")
+        is_migrated = is_environment_variable_migrated(deployment, token, key)
         return self.render_template(
             "starship/components/env_checkbox.html",
             target=key,
             deployment=deployment,
             is_migrated=is_migrated,
         )
 
     @expose("/component/astro-deployment-selector")
     def deployment_selector(self):
-        deployments = self.astro_deployments(session.get("token"))
+        deployments = session.get("deployments")
+        if not deployments:
+            deployments = astro_client.get_deployments(session.get("token"))
+            session["deployments"] = deployments
+
+        user = session.get("user")
+        if not user:
+            user = astro_client.get_username(token=session.get("token"))
+            session["user"] = user
 
         return self.render_template(
             "starship/components/target_deployment_select.html",
             deployments=deployments,
-            username=self.get_astro_username(token=session.get("token")),
+            username=user,
         )
 
     @expose("/logout")
     def logout(self):
         session.pop("token")
+        session.pop("user")
+        session.pop("deployments")
         return redirect(url_for("Airflow.index"))
 
     @expose("/component/row/dags/<string:deployment>/<string:dag_id>")
     @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_DAG)])
     def dag_cutover_row_get(self, deployment: str, dag_id: str):
         return self.dag_cutover_row(deployment, dag_id)
 
     @expose(
         "/component/row/dags/<string:deployment>/<string:dest>/<string:dag_id>/<string:action>",
         methods=(
-                "GET",
-                "POST",
+            "GET",
+            "POST",
         ),
     )
     @auth.has_access([(permissions.ACTION_CAN_EDIT, permissions.RESOURCE_DAG)])
     def dag_cutover_row(
-            self, deployment: str, dag_id: str, dest: str = "local", action: str = None
+        self, deployment: str, dag_id: str, dest: str = "local", action: str = "init"
     ):
         if dest not in ["local", "astro"]:
-            raise Exception("dest must be 'local' or 'astro'")
+            raise RuntimeError("dest must be 'local' or 'astro'")
+        if action not in ["pause", "unpause", "migrate", "init"]:
+            raise Exception("action must be 'pause', 'unpause', or 'migrate'")
 
-        dag = self.local_client.get_dags()[dag_id]
-        deployment_url = self.get_deployment_url(deployment)
         token = session.get("token")
+        deployment_url = astro_client.get_deployment_url(deployment, token)
 
         if request.method == "POST":
-            if action == "pause":
-                is_paused = True
-            elif action == "unpause":
-                is_paused = False
-            else:
-                raise Exception("action must be 'pause' or 'unpause'")
-
-            if dest == "local":
-                models.DagModel.get_dagmodel(dag_id).set_is_paused(is_paused=is_paused)
-            else:
-                resp = requests.patch(
-                    f"{deployment_url}/api/v1/dags?dag_id_pattern={dag_id}",
-                    headers={"Authorization": f"Bearer {token}"},
-                    json={"is_paused": is_paused},
+            if action == "migrate":
+                remote_airflow_client.migrate_dag(
+                    dag_id, deployment_url=deployment_url, token=token
                 )
-
-        resp = requests.get(
-            f"{deployment_url}/api/v1/dags/{dag_id}",
-            headers={"Authorization": f"Bearer {token}"},
-        )
-
-        is_on_astro = not resp.status_code == 404
-
-        resp_contents = resp.json()
+            else:
+                is_paused = "pause" == action
+                if dest == "local":
+                    local_airflow_client.set_dag_is_paused(dag_id, is_paused)
+                else:
+                    remote_airflow_client.set_dag_is_paused(
+                        dag_id, is_paused, deployment_url, token
+                    )
+
+        r = remote_airflow_client.get_dag(dag_id, deployment_url, token)
+        dag_runs = remote_airflow_client.get_dag_runs(
+            dag_id, deployment_url, token
+        ).json()
+        is_on_astro = not r.status_code == 404
+        remote_dag = r.json()
+        local_dag = local_airflow_client.get_dag(dag_id)
 
         return self.render_template(
             "starship/components/dag_row.html",
             dag_={
-                "id": dag.dag_id,
+                "id": local_dag.dag_id,
                 "is_on_astro": is_on_astro,
-                "is_paused_here": dag.is_paused,
-                "is_paused_on_astro": resp_contents["is_paused"]
-                if is_on_astro
-                else False,
+                "is_paused_here": local_dag.is_paused,
+                "is_paused_on_astro": remote_dag["is_paused"] if is_on_astro else False,
+                "has_history_on_astro": bool(dag_runs["total_entries"]),
             },
         )
 
-    def get_deployment_url(self, deployment):
-        astro_deployments = self.astro_deployments(session.get("token"))
-
-        if astro_deployments and astro_deployments.get(deployment):
-            url = urlparse(
-                astro_deployments[deployment]["webServerUrl"]
-            )
-            return f"https:/{url.netloc}/{url.path}"
-
 
 v_appbuilder_view = AstroMigration()
 
 v_appbuilder_package = {
     "name": "Migration Tool 🚀 Starship",
     "category": "Astronomer",
     "view": v_appbuilder_view,
```

### Comparing `astronomer-starship-0.3.5/starship/static/js/htmx.min.js` & `astronomer_starship-1.0.0/astronomer/starship/static/js/htmx.min.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text, with very long lines (39433), with no line terminators*

 * *Files 0% similar despite different names*

```diff
@@ -2458,8 +2458,8 @@
 00009990: 2865 297b 2428 652c 2268 746d 783a 7265  (e){$(e,"htmx:re
 000099a0: 7374 6f72 6564 222c 7b64 6f63 756d 656e  stored",{documen
 000099b0: 743a 5f28 292c 7472 6967 6765 7245 7665  t:_(),triggerEve
 000099c0: 6e74 3a24 7d29 7d29 7d7d 3b73 6574 5469  nt:$})})}};setTi
 000099d0: 6d65 6f75 7428 6675 6e63 7469 6f6e 2829  meout(function()
 000099e0: 7b24 2865 2c22 6874 6d78 3a6c 6f61 6422  {$(e,"htmx:load"
 000099f0: 2c7b 7d29 7d2c 3029 7d29 3b72 6574 7572  ,{})},0)});retur
-00009a00: 6e20 557d 2829 7d29 3b                   n U}()});
+00009a00: 6e20 557d 2829 7d29 3b0a                 n U}()});.
```

### Comparing `astronomer-starship-0.3.5/starship/static/js/idiomorph.min.js` & `astronomer_starship-1.0.0/astronomer/starship/static/js/idiomorph.min.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text, with very long lines (7014), with no line terminators*

 * *Files 0% similar despite different names*

```diff
@@ -432,8 +432,8 @@
 00001af0: 3b6e 2e73 6574 2874 2c65 297d 652e 6164  ;n.set(t,e)}e.ad
 00001b00: 6428 722e 6964 293b 743d 742e 7061 7265  d(r.id);t=t.pare
 00001b10: 6e74 456c 656d 656e 747d 7d7d 6675 6e63  ntElement}}}func
 00001b20: 7469 6f6e 2048 2865 2c74 297b 6c65 7420  tion H(e,t){let 
 00001b30: 6e3d 6e65 7720 4d61 703b 4528 652c 6e29  n=new Map;E(e,n)
 00001b40: 3b45 2874 2c6e 293b 7265 7475 726e 206e  ;E(t,n);return n
 00001b50: 7d72 6574 7572 6e7b 6d6f 7270 683a 657d  }return{morph:e}
-00001b60: 7d28 297d 293b                           }()});
+00001b60: 7d28 297d 293b 0a                        }()});.
```

### Comparing `astronomer-starship-0.3.5/starship/static/js/popper.js` & `astronomer_starship-1.0.0/astronomer/starship/static/js/popper.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text, with very long lines (20006)*

 * *Files 0% similar despite different names*

```diff
@@ -1249,8 +1249,8 @@
 00004e00: 7065 724f 6666 7365 7473 3d74 652c 652e  perOffsets=te,e.
 00004e10: 7072 6576 656e 744f 7665 7266 6c6f 773d  preventOverflow=
 00004e20: 6865 2c4f 626a 6563 742e 6465 6669 6e65  he,Object.define
 00004e30: 5072 6f70 6572 7479 2865 2c22 5f5f 6573  Property(e,"__es
 00004e40: 4d6f 6475 6c65 222c 7b76 616c 7565 3a21  Module",{value:!
 00004e50: 307d 297d 2929 3b0a 2f2f 2320 736f 7572  0})}));.//# sour
 00004e60: 6365 4d61 7070 696e 6755 524c 3d70 6f70  ceMappingURL=pop
-00004e70: 7065 722e 6d69 6e2e 6a73 2e6d 6170       per.min.js.map
+00004e70: 7065 722e 6d69 6e2e 6a73 2e6d 6170 0a    per.min.js.map.
```

### Comparing `astronomer-starship-0.3.5/starship/static/js/tippy.js` & `astronomer_starship-1.0.0/astronomer/starship/static/js/tippy.js`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.5/starship/static/tail-spin.svg` & `astronomer_starship-1.0.0/astronomer/starship/static/tail-spin.svg`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.5/starship/templates/starship/components/dag_row.html` & `astronomer_starship-1.0.0/astronomer/starship/templates/starship/components/dag_row.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <tr id="dag-{{dag_.id}}">
     <td>{{ dag_.id }}</td>
     <td>{{ dag_.is_on_astro }}</td>
     <td>
         {% if dag_.is_paused_here %}
         <button class="btn btn-success"
-                hx-post="{{ url_for('AstroMigration.dag_cutover_row', deployment=session.selectedAstroDeployment or 'undefined', dest='local', dag_id=dag_.id, action='unpause') }}"
+                hx-post="{{ url_for('AstroMigration.dag_cutover_row', deployment=session.selectedAstroDeployment or 'undefined', dag_id=dag_.id, dest='local', action='unpause') }}"
                 hx-target="#dag-{{dag_.id}}"
                 hx-swap="outerHTML"
         >
             <span class="glyphicon glyphicon-play" aria-hidden="true"></span>
         </button>
         {% else %}
         <button class="btn btn-danger"
@@ -39,8 +39,27 @@
                 hx-target="#dag-{{dag_.id}}"
                 hx-swap="outerHTML"
         >
             <span class="glyphicon glyphicon-pause" aria-hidden="true"></span>
         </button>
         {% endif %}
     </td>
-</tr>
+    <td>
+    {% if not dag_.is_on_astro %}
+        <button class="btn btn-default" disabled>
+            <span class="glyphicon glyphicon-upload" aria-hidden="true"></span>
+        </button>
+        {% elif dag_.has_history_on_astro %}
+                <button class="btn btn-default" disabled>
+            History Present on Target
+        </button>
+        {%  else %}
+              <button class="btn btn-default"
+                hx-post="{{ url_for('AstroMigration.dag_cutover_row', deployment=session.selectedAstroDeployment or 'undefined', dag_id=dag_.id, dest='astro', action='migrate') }}"
+                hx-target="#dag-{{dag_.id}}"
+                hx-swap="outerHTML"
+              >
+            <span class="glyphicon glyphicon-upload" aria-hidden="true"></span>
+        </button>
+        {%  endif %}
+    </td>
+</tr>
```

### Comparing `astronomer-starship-0.3.5/starship/templates/starship/components/migrate_connection_button.html` & `astronomer_starship-1.0.0/astronomer/starship/templates/starship/components/migrate_connection_button.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.5/starship/templates/starship/components/tabs.html` & `astronomer_starship-1.0.0/astronomer/starship/templates/starship/components/tabs.html`

 * *Files 18% similar despite different names*

```diff
@@ -5,17 +5,17 @@
         </li>
         <li class="nav-item {{ 'active' if data.component == 'variables' }}">
             <a class="nav-link" hx-get="{{ url_for('AstroMigration.tabs_vars') }}">Variables</a>
         </li>
         <li class="nav-item {{ 'active' if data.component == 'pools' }}">
             <a class="nav-link" hx-get="{{ url_for('AstroMigration.tabs_pools') }}">Pools</a>
         </li>
-<!--        <li class="nav-item {{ 'active' if data.component == 'env' }}">-->
-<!--            <a class="nav-link" hx-get="{{ url_for('AstroMigration.tabs_env') }}">Environment Variables</a>-->
-<!--        </li>-->
+        <li class="nav-item {{ 'active' if data.component == 'env' }}">
+            <a class="nav-link" hx-get="{{ url_for('AstroMigration.tabs_env') }}">Environment Variables</a>
+        </li>
         <li class="nav-item {{ 'active' if data.component == 'dags' }}">
             <a class="nav-link" hx-get="{{ url_for('AstroMigration.tabs_dags') }}">DAGs cutover</a>
         </li>
     </ul>
 </div>
 <div class="tab-content" id="tabs-content">
     <div class="container">
```

### Comparing `astronomer-starship-0.3.5/starship/templates/starship/components/tabs_loading.html` & `astronomer_starship-1.0.0/astronomer/starship/templates/starship/components/tabs_loading.html`

 * *Files 0% similar despite different names*

```diff
@@ -6,52 +6,53 @@
         <li class="nav-item" class="disabled">
             <a class="nav-link">Variables</a>
         </li>
         <li class="nav-item" class="disabled">
             <a class="nav-link">Pools</a>
         </li>
         <li class="nav-item" class="disabled">
-            <a class="nav-link">Environment Variables</a></li>
+            <a class="nav-link">Environment Variables</a>
+        </li>
         <li class="nav-item" class="disabled">
             <a class="nav-link">DAGs cutover</a>
         </li>
     </ul>
 </div>
 <div class="tab-content" id="tabs-content">
     <div class="container">
         {% block body %}
-        <form>
-            <table class="table table-striped table-bordered table-hover">
-                <thead>
-                <tr>
-                    <th scope="col">Type</th>
-                    <th scope="col">Id</th>
-                    <th scope="col">Host</th>
-                    <th scope="col">Login</th>
-                    <th scope="col">Schema</th>
-                    <th scope="col">Port</th>
-                    <th scope="col">Extra</th>
-                    <th>
-                    </th>
-                </tr>
-                </thead>
-                <tbody>
-                <tr>
-                    <td>Loading....</td>
-                    <td></td>
-                    <td></td>
-                    <td></td>
-                    <td></td>
-                    <td></td>
-                    <td style="font-family: monospace; overflow: hidden; text-overflow: ellipsis;"></td>
-                    <td class="text-right">
-                        <div>
-                            <button class="btn btn-default disabled">Migrate</button>
-                        </div>
-                    </td>
-                </tr>
-                </tbody>
-            </table>
-        </form>
+            <form>
+                <table class="table table-striped table-bordered table-hover">
+                    <thead>
+                    <tr>
+                        <th scope="col">Type</th>
+                        <th scope="col">Id</th>
+                        <th scope="col">Host</th>
+                        <th scope="col">Login</th>
+                        <th scope="col">Schema</th>
+                        <th scope="col">Port</th>
+                        <th scope="col">Extra</th>
+                        <th>
+                        </th>
+                    </tr>
+                    </thead>
+                    <tbody>
+                    <tr>
+                        <td>Loading....</td>
+                        <td></td>
+                        <td></td>
+                        <td></td>
+                        <td></td>
+                        <td></td>
+                        <td style="font-family: monospace; overflow: hidden; text-overflow: ellipsis;"></td>
+                        <td class="text-right">
+                            <div>
+                                <button class="btn btn-default disabled">Migrate</button>
+                            </div>
+                        </td>
+                    </tr>
+                    </tbody>
+                </table>
+            </form>
         {% endblock %}
     </div>
 </div>
```

### Comparing `astronomer-starship-0.3.5/starship/templates/starship/components/target_deployment_select.html` & `astronomer_starship-1.0.0/astronomer/starship/templates/starship/components/target_deployment_select.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.5/starship/templates/starship/components/target_deployment_select_loading.html` & `astronomer_starship-1.0.0/astronomer/starship/templates/starship/components/target_deployment_select_loading.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,8 @@
                 </div>
                 <div class="col-lg-3">
                     <button type="submit" disabled class="btn btn-primary mb3-l">Select</button>
                 </div>
             </div>
         </div>
     </form>
-</div>
+</div>
```

### Comparing `astronomer-starship-0.3.5/starship/templates/starship/components/token_modal.html` & `astronomer_starship-1.0.0/astronomer/starship/templates/starship/components/token_modal.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.5/starship/templates/starship/connections.html` & `astronomer_starship-1.0.0/astronomer/starship/templates/starship/connections.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -41,8 +41,8 @@
         {% endfor %}
         </tbody>
     </table>
 </form>
 {% else %}
 <h4>No connections found in local metadata database.</h4>
 {% endif %}
-{% endblock %}
+{% endblock %}
```

### Comparing `astronomer-starship-0.3.5/starship/templates/starship/dags.html` & `astronomer_starship-1.0.0/astronomer/starship/templates/starship/dags.html`

 * *Files 17% similar despite different names*

```diff
@@ -7,20 +7,21 @@
     <table class="table table-striped table-bordered table-hover">
         <thead>
         <tr>
             <th scope="col">DAG</th>
             <th scope="col">Present on Astro?</th>
             <th scope="col" style="width: 8%">Local</th>
             <th scope="col" style="width: 8%">Remote</th>
+            <th scope="col" style="width: 8%">Migrate</th>
         </tr>
         </thead>
         <tbody>
         {% for k, v in data.dags.items() %}
         <tr id="dag-{{k}}"
-            hx-get="{{ url_for('AstroMigration.dag_cutover_row_get', deployment=session.selectedAstroDeployment or 'undefined', dag_id=k) }}"
+            hx-get="{{ url_for('AstroMigration.dag_cutover_row_get', deployment=session.selectedAstroDeployment or 'undefined', dag_id=k, action='init') }}"
             hx-trigger="load delay:100ms"
             hx-target="#dag-{{k}}"
             hx-swap="outerHTML">
         </tr>
         {% endfor %}
         </tbody>
     </table>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
 {% extends "starship/components/tabs.html" %} {% block body %} {% if 'dags' in
 data and data.dags|length > 0 %}
-DAG Present on Astro? Local Remote
+DAG Present on Astro? Local Remote Migrate
 {% else %}
 *** No DAGs found in local instance. ***
 {% endif %} {% endblock %}
```

### Comparing `astronomer-starship-0.3.5/starship/templates/starship/env.html` & `astronomer_starship-1.0.0/astronomer/starship/templates/starship/env.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -40,8 +40,8 @@
             {% endfor %}
             </tbody>
         </table>
     </form>
 {% else %}
 <h4>No environment variables found in local instance.</h4>
 {% endif %}
-{% endblock %}
+{% endblock %}
```

### Comparing `astronomer-starship-0.3.5/starship/templates/starship/main.html` & `astronomer_starship-1.0.0/astronomer/starship/templates/starship/main.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.5/starship/templates/starship/migration.html` & `astronomer_starship-1.0.0/astronomer/starship/templates/starship/migration.html`

 * *Files 9% similar despite different names*

```diff
@@ -3,24 +3,24 @@
      hx-trigger="load delay:100ms"
      hx-target="#astro-token-entry"
      hx-swap="outerHTML">
 </div>
 <div id="astro-deployment-selector"
      hx-indicator="#astro-deployment-selector-loading"
      hx-get="{{ url_for('AstroMigration.deployment_selector') }}"
-     hx-trigger="load delay:100ms"
+     hx-trigger="load delay:10ms"
      hx-target="#astro-deployment-selector"
      hx-swap="innerHTML">
     <div id="astro-deployment-selector-loading" class="htmx-indicator">
         {% include 'starship/components/target_deployment_select_loading.html' %}
     </div>
 </div>
 <div id="tabs"
      hx-indicator="#tabs-loading"
-     hx-get="{{ url_for('AstroMigration.tabs_conns') }}"
-     hx-trigger="load delay:100ms"
+     hx-get="{{ url_for(data.tab) if data else url_for('AstroMigration.tabs_conns') }}"
+     hx-trigger="load delay:10ms"
      hx-target="#tabs"
      hx-swap="innerHTML">
     <div id="tabs-loading" class="htmx-indicator">
         {% include 'starship/components/tabs_loading.html' %}
     </div>
 </div>
```

### Comparing `astronomer-starship-0.3.5/starship/templates/starship/pools.html` & `astronomer_starship-1.0.0/astronomer/starship/templates/starship/pools.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
         {% endfor %}
         </tbody>
     </table>
 </form>
 {% else %}
 <h4>No pools found in local metadata database.</h4>
 {% endif %}
-{% endblock %}
+{% endblock %}
```

### Comparing `astronomer-starship-0.3.5/starship/templates/starship/variables.html` & `astronomer_starship-1.0.0/astronomer/starship/templates/starship/variables.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -31,8 +31,8 @@
             {% endfor %}
             </tbody>
         </table>
     </form>
 {% else %}
 <h4>No variables found in local metadata database.</h4>
 {% endif %}
-{% endblock %}
+{% endblock %}
```

