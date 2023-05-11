# Comparing `tmp/estela-0.2.tar.gz` & `tmp/estela-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estela-0.2.tar", last modified: Mon Apr 24 16:25:20 2023, max compression
+gzip compressed data, was "estela-0.2.1.tar", last modified: Fri May  5 22:08:45 2023, max compression
```

## Comparing `estela-0.2.tar` & `estela-0.2.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-04-24 16:25:20.162544 estela-0.2/
--rw-r--r--   0 mgonnav    (501) staff       (20)      257 2023-04-24 16:25:20.162430 estela-0.2/PKG-INFO
--rw-r--r--   0 mgonnav    (501) staff       (20)     1548 2023-01-09 17:55:22.000000 estela-0.2/README.md
-drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-04-24 16:25:20.159279 estela-0.2/estela.egg-info/
--rw-r--r--   0 mgonnav    (501) staff       (20)      257 2023-04-24 16:25:20.000000 estela-0.2/estela.egg-info/PKG-INFO
--rw-r--r--   0 mgonnav    (501) staff       (20)      910 2023-04-24 16:25:20.000000 estela-0.2/estela.egg-info/SOURCES.txt
--rw-r--r--   0 mgonnav    (501) staff       (20)        1 2023-04-24 16:25:20.000000 estela-0.2/estela.egg-info/dependency_links.txt
--rw-r--r--   0 mgonnav    (501) staff       (20)       51 2023-04-24 16:25:20.000000 estela-0.2/estela.egg-info/entry_points.txt
--rw-r--r--   0 mgonnav    (501) staff       (20)       38 2023-04-24 16:25:20.000000 estela-0.2/estela.egg-info/requires.txt
--rw-r--r--   0 mgonnav    (501) staff       (20)       11 2023-04-24 16:25:20.000000 estela-0.2/estela.egg-info/top_level.txt
-drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-04-24 16:25:20.160346 estela-0.2/estela_cli/
--rw-r--r--   0 mgonnav    (501) staff       (20)        0 2022-07-18 19:23:21.000000 estela-0.2/estela_cli/__init__.py
--rw-r--r--   0 mgonnav    (501) staff       (20)      528 2023-04-24 16:24:02.000000 estela-0.2/estela_cli/__main__.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     2357 2022-07-18 19:23:21.000000 estela-0.2/estela_cli/context.py
-drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-04-24 16:25:20.160777 estela-0.2/estela_cli/create/
--rw-r--r--   0 mgonnav    (501) staff       (20)      332 2022-07-18 19:23:21.000000 estela-0.2/estela_cli/create/__init__.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     2040 2023-01-26 21:18:07.000000 estela-0.2/estela_cli/create/cronjob.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     1792 2023-01-26 21:18:07.000000 estela-0.2/estela_cli/create/job.py
--rw-r--r--   0 mgonnav    (501) staff       (20)      629 2022-07-18 19:23:21.000000 estela-0.2/estela_cli/create/project.py
-drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-04-24 16:25:20.161000 estela-0.2/estela_cli/data/
--rw-r--r--   0 mgonnav    (501) staff       (20)      333 2023-01-09 17:55:22.000000 estela-0.2/estela_cli/data/__init__.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     2529 2023-01-09 17:55:22.000000 estela-0.2/estela_cli/data/job.py
-drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-04-24 16:25:20.161214 estela-0.2/estela_cli/delete/
--rw-r--r--   0 mgonnav    (501) staff       (20)      306 2022-07-18 19:23:21.000000 estela-0.2/estela_cli/delete/__init__.py
--rw-r--r--   0 mgonnav    (501) staff       (20)      562 2022-07-18 19:23:21.000000 estela-0.2/estela_cli/delete/project.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     3280 2023-01-09 17:55:22.000000 estela-0.2/estela_cli/deploy.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     8674 2023-04-24 16:24:18.000000 estela-0.2/estela_cli/estela_client.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     2950 2023-01-09 17:55:22.000000 estela-0.2/estela_cli/init.py
-drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-04-24 16:25:20.161749 estela-0.2/estela_cli/list/
--rw-r--r--   0 mgonnav    (501) staff       (20)      358 2022-07-18 19:23:21.000000 estela-0.2/estela_cli/list/__init__.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     1888 2023-01-26 21:18:07.000000 estela-0.2/estela_cli/list/cronjob.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     1835 2023-01-26 21:18:07.000000 estela-0.2/estela_cli/list/job.py
--rw-r--r--   0 mgonnav    (501) staff       (20)      448 2022-07-18 19:23:21.000000 estela-0.2/estela_cli/list/project.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     1151 2022-07-18 19:23:21.000000 estela-0.2/estela_cli/list/spider.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     3577 2022-07-18 19:23:21.000000 estela-0.2/estela_cli/login.py
--rw-r--r--   0 mgonnav    (501) staff       (20)      517 2022-07-18 19:23:21.000000 estela-0.2/estela_cli/logout.py
-drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-04-24 16:25:20.161970 estela-0.2/estela_cli/stop/
--rw-r--r--   0 mgonnav    (501) staff       (20)      312 2022-07-18 19:23:21.000000 estela-0.2/estela_cli/stop/__init__.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     1110 2022-07-18 19:23:21.000000 estela-0.2/estela_cli/stop/job.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     1027 2023-04-19 22:49:34.000000 estela-0.2/estela_cli/templates.py
-drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-04-24 16:25:20.162286 estela-0.2/estela_cli/update/
--rw-r--r--   0 mgonnav    (501) staff       (20)      317 2022-07-18 19:23:21.000000 estela-0.2/estela_cli/update/__init__.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     1977 2022-07-18 19:23:21.000000 estela-0.2/estela_cli/update/cronjob.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     1590 2022-07-18 19:23:21.000000 estela-0.2/estela_cli/update/job.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     4093 2023-01-26 21:18:07.000000 estela-0.2/estela_cli/utils.py
--rw-r--r--   0 mgonnav    (501) staff       (20)       38 2023-04-24 16:25:20.162581 estela-0.2/setup.cfg
--rw-r--r--   0 mgonnav    (501) staff       (20)      599 2023-04-24 16:24:44.000000 estela-0.2/setup.py
+drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-05-05 22:08:45.287894 estela-0.2.1/
+-rw-r--r--   0 mgonnav    (501) staff       (20)      259 2023-05-05 22:08:45.287777 estela-0.2.1/PKG-INFO
+-rw-r--r--   0 mgonnav    (501) staff       (20)     1548 2023-01-09 17:55:22.000000 estela-0.2.1/README.md
+drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-05-05 22:08:45.282647 estela-0.2.1/estela.egg-info/
+-rw-r--r--   0 mgonnav    (501) staff       (20)      259 2023-05-05 22:08:45.000000 estela-0.2.1/estela.egg-info/PKG-INFO
+-rw-r--r--   0 mgonnav    (501) staff       (20)      910 2023-05-05 22:08:45.000000 estela-0.2.1/estela.egg-info/SOURCES.txt
+-rw-r--r--   0 mgonnav    (501) staff       (20)        1 2023-05-05 22:08:45.000000 estela-0.2.1/estela.egg-info/dependency_links.txt
+-rw-r--r--   0 mgonnav    (501) staff       (20)       51 2023-05-05 22:08:45.000000 estela-0.2.1/estela.egg-info/entry_points.txt
+-rw-r--r--   0 mgonnav    (501) staff       (20)       38 2023-05-05 22:08:45.000000 estela-0.2.1/estela.egg-info/requires.txt
+-rw-r--r--   0 mgonnav    (501) staff       (20)       11 2023-05-05 22:08:45.000000 estela-0.2.1/estela.egg-info/top_level.txt
+drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-05-05 22:08:45.284757 estela-0.2.1/estela_cli/
+-rw-r--r--   0 mgonnav    (501) staff       (20)       49 2023-05-05 21:57:11.000000 estela-0.2.1/estela_cli/__init__.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)      543 2023-05-05 21:55:52.000000 estela-0.2.1/estela_cli/__main__.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)     2357 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/context.py
+drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-05-05 22:08:45.285517 estela-0.2.1/estela_cli/create/
+-rw-r--r--   0 mgonnav    (501) staff       (20)      332 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/create/__init__.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)     2040 2023-01-26 21:18:07.000000 estela-0.2.1/estela_cli/create/cronjob.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)     1792 2023-01-26 21:18:07.000000 estela-0.2.1/estela_cli/create/job.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)      629 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/create/project.py
+drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-05-05 22:08:45.285841 estela-0.2.1/estela_cli/data/
+-rw-r--r--   0 mgonnav    (501) staff       (20)      333 2023-01-09 17:55:22.000000 estela-0.2.1/estela_cli/data/__init__.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)     2734 2023-05-05 20:34:19.000000 estela-0.2.1/estela_cli/data/job.py
+drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-05-05 22:08:45.286193 estela-0.2.1/estela_cli/delete/
+-rw-r--r--   0 mgonnav    (501) staff       (20)      306 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/delete/__init__.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)      562 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/delete/project.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)     3280 2023-01-09 17:55:22.000000 estela-0.2.1/estela_cli/deploy.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)     8738 2023-05-05 21:55:16.000000 estela-0.2.1/estela_cli/estela_client.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)     2950 2023-01-09 17:55:22.000000 estela-0.2.1/estela_cli/init.py
+drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-05-05 22:08:45.286884 estela-0.2.1/estela_cli/list/
+-rw-r--r--   0 mgonnav    (501) staff       (20)      358 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/list/__init__.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)     1888 2023-01-26 21:18:07.000000 estela-0.2.1/estela_cli/list/cronjob.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)     1835 2023-01-26 21:18:07.000000 estela-0.2.1/estela_cli/list/job.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)      448 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/list/project.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)     1151 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/list/spider.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)     3577 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/login.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)      517 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/logout.py
+drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-05-05 22:08:45.287168 estela-0.2.1/estela_cli/stop/
+-rw-r--r--   0 mgonnav    (501) staff       (20)      312 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/stop/__init__.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)     1110 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/stop/job.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)     1027 2023-04-19 22:49:34.000000 estela-0.2.1/estela_cli/templates.py
+drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-05-05 22:08:45.287601 estela-0.2.1/estela_cli/update/
+-rw-r--r--   0 mgonnav    (501) staff       (20)      317 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/update/__init__.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)     1977 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/update/cronjob.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)     1590 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/update/job.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)     4179 2023-05-05 21:38:05.000000 estela-0.2.1/estela_cli/utils.py
+-rw-r--r--   0 mgonnav    (501) staff       (20)       38 2023-05-05 22:08:45.287928 estela-0.2.1/setup.cfg
+-rw-r--r--   0 mgonnav    (501) staff       (20)      601 2023-05-05 21:57:11.000000 estela-0.2.1/setup.py
```

### Comparing `estela-0.2/README.md` & `estela-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `estela-0.2/estela.egg-info/SOURCES.txt` & `estela-0.2.1/estela.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `estela-0.2/estela_cli/context.py` & `estela-0.2.1/estela_cli/context.py`

 * *Files identical despite different names*

### Comparing `estela-0.2/estela_cli/create/cronjob.py` & `estela-0.2.1/estela_cli/create/cronjob.py`

 * *Files identical despite different names*

### Comparing `estela-0.2/estela_cli/create/job.py` & `estela-0.2.1/estela_cli/create/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2/estela_cli/create/project.py` & `estela-0.2.1/estela_cli/create/project.py`

 * *Files identical despite different names*

### Comparing `estela-0.2/estela_cli/data/job.py` & `estela-0.2.1/estela_cli/data/job.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,85 +1,87 @@
 import time
 
-from email.policy import default
 import click
-from click import ClickException
 
 from estela_cli.login import login
-from estela_cli.utils import (
-    get_estela_settings,
-    get_project_path,
-    save_data,
-    save_chunk_data,
-)
-from estela_cli.templates import OK_EMOJI, BAD_EMOJI, CLOCK_EMOJI
+from estela_cli.templates import BAD_EMOJI, CLOCK_EMOJI, OK_EMOJI
+from estela_cli.utils import get_estela_settings, save_chunk_data, save_data
 
 SHORT_HELP = "Retrieve data from a job"
-ALLOWED_FORMATS = ["json", "csv"]
+ALLOWED_DATA_TYPES = ["items", "requests", "logs", "stats"]
+ALLOWED_DATA_FORMATS = ["json", "csv"]
 
 
 @click.command(short_help=SHORT_HELP)
 @click.argument("jid", required=True)
 @click.argument("sid", required=True)
 @click.argument("pid", required=False)
 @click.option(
+    "-t",
+    "--datatype",
+    type=click.Choice(ALLOWED_DATA_TYPES, case_sensitive=False),
+    default="items",
+)
+@click.option(
     "-f",
     "--format",
-    type=click.Choice(ALLOWED_FORMATS, case_sensitive=False),
+    type=click.Choice(ALLOWED_DATA_FORMATS, case_sensitive=False),
     default="json",
 )
 def estela_command(
     jid,
     sid,
     pid,
+    datatype,
     format,
 ):
-    """Retrieve all data from a given job
+    """Retrieve data from a given job
 
     \b
     SID is the spider's sid
     PID is the project's pid (active project by default)
     JID is the job's id
+    DATATYPE is the type of data to retrieve
     FORMAT is the format to retrieve data
     """
 
     estela_client = login()
     if pid is None:
         try:
             estela_settings = get_estela_settings()
             pid = estela_settings["project"]["pid"]
         except:
             raise click.ClickException(
                 "No active project in the current directory. Please specify the PID."
             )
 
-    tmp_filename = ".{}-{}-{}-tmp".format(jid, pid, time.time())
-    filename = "{}-{}.{}".format(jid, pid, format)
+    tmp_filename = ".{}-{}-{}-{}-tmp".format(jid, pid, datatype, time.time())
+    filename = "{}-{}-{}.{}".format(jid, pid, datatype, format)
     try:
-        response = estela_client.get_spider_job_data(pid, sid, jid)
+        response = estela_client.get_spider_job_data(pid, sid, jid, datatype)
         with click.progressbar(
             length=int(response["count"]),
             label="{} Downloading job data".format(CLOCK_EMOJI),
             show_eta=True,
             show_percent=True,
             show_pos=True,
         ) as progress_bar:
             next_chunk = None
             while True:
-                response = estela_client.get_spider_job_data(pid, sid, jid, next_chunk)
+                response = estela_client.get_spider_job_data(pid, sid, jid, datatype, next_chunk)
                 chunk = response.get("results")
                 save_chunk_data(tmp_filename, chunk)
                 progress_bar.update(len(chunk))
                 next_chunk = response.get("next_chunk")
                 if next_chunk is None:
                     break
         click.echo("{} Data downloaded succesfully.".format(OK_EMOJI))
     except:
         raise click.ClickException(
             "{} Could not download the job data".format(BAD_EMOJI)
         )
 
     try:
-        save_data(filename, tmp_filename)
+        save_data(filename, tmp_filename, format)
         click.echo("{} Data saved succesfully.".format(OK_EMOJI))
     except:
         raise click.ClickException("{} Could not save the job data".format(BAD_EMOJI))
```

### Comparing `estela-0.2/estela_cli/delete/project.py` & `estela-0.2.1/estela_cli/delete/project.py`

 * *Files identical despite different names*

### Comparing `estela-0.2/estela_cli/deploy.py` & `estela-0.2.1/estela_cli/deploy.py`

 * *Files identical despite different names*

### Comparing `estela-0.2/estela_cli/estela_client.py` & `estela-0.2.1/estela_cli/estela_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from datetime import date, timedelta
 
 import requests
 
+from estela_cli import __version__
+
 
 class EstelaSimpleClient:
     token = None
 
     def __init__(self, host, username=None, password=None, token=None):
         self.host = host
         self.api_base = "{}/api".format(self.host)
@@ -22,15 +24,15 @@
             response = self.get("projects")
             self.check_status(response, 200)
 
     def url_for(self, endpoint):
         return "{}/{}".format(self.api_base, endpoint)
 
     def get_default_headers(self):
-        headers = {"User-Agent": "estela-cli/0.2"}
+        headers = {"User-Agent": f"estela-cli/{__version__}"}
         if self.token:
             headers["Authorization"] = "Token {}".format(self.token)
         return headers
 
     def post(self, endpoint, data=None, params=None, files=None):
         if files is None:
             files = {}
@@ -167,17 +169,17 @@
 
     def get_spider_job(self, pid, sid, jid):
         endpoint = "projects/{}/spiders/{}/jobs/{}".format(pid, sid, jid)
         response = self.get(endpoint)
         self.check_status(response, 200)
         return response.json()
 
-    def get_spider_job_data(self, pid, sid, jid, last_chunk=None):
-        endpoint = "projects/{}/spiders/{}/jobs/{}/data?mode=paged".format(
-            pid, sid, jid
+    def get_spider_job_data(self, pid, sid, jid, datatype, last_chunk=None):
+        endpoint = "projects/{}/spiders/{}/jobs/{}/data?type={}".format(
+            pid, sid, jid, datatype
         )
         if last_chunk:
             endpoint += "&current_chunk={}".format(last_chunk)
         response = self.get(endpoint)
         self.check_status(response, 200)
         return response.json()
```

### Comparing `estela-0.2/estela_cli/init.py` & `estela-0.2.1/estela_cli/init.py`

 * *Files identical despite different names*

### Comparing `estela-0.2/estela_cli/list/cronjob.py` & `estela-0.2.1/estela_cli/list/cronjob.py`

 * *Files identical despite different names*

### Comparing `estela-0.2/estela_cli/list/job.py` & `estela-0.2.1/estela_cli/list/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2/estela_cli/list/spider.py` & `estela-0.2.1/estela_cli/list/spider.py`

 * *Files identical despite different names*

### Comparing `estela-0.2/estela_cli/login.py` & `estela-0.2.1/estela_cli/login.py`

 * *Files identical despite different names*

### Comparing `estela-0.2/estela_cli/logout.py` & `estela-0.2.1/estela_cli/logout.py`

 * *Files identical despite different names*

### Comparing `estela-0.2/estela_cli/stop/job.py` & `estela-0.2.1/estela_cli/stop/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2/estela_cli/templates.py` & `estela-0.2.1/estela_cli/templates.py`

 * *Files identical despite different names*

### Comparing `estela-0.2/estela_cli/update/cronjob.py` & `estela-0.2.1/estela_cli/update/cronjob.py`

 * *Files identical despite different names*

### Comparing `estela-0.2/estela_cli/update/job.py` & `estela-0.2.1/estela_cli/update/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2/estela_cli/utils.py` & `estela-0.2.1/estela_cli/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,33 +105,34 @@
             F.write("[")
     with open(filename, "a", encoding="utf-8") as F:
         for item in data:
             F.write(json.dumps(item))
             F.write(",")
 
 
-def save_data(filename, tmp_filename):
+def save_data(filename, tmp_filename, format):
     project_path = get_project_path()
     filename = os.path.join(project_path, DATA_DIR, filename)
     tmp_filename = os.path.join(project_path, DATA_DIR, tmp_filename)
     with open(tmp_filename, "rb+") as F:
         F.seek(-1, 2)
         F.truncate()
         F.write(b"]\n")
 
-    if "json" in filename:
+    if format == "json":
         os.rename(tmp_filename, filename)
-    elif "csv" in filename:
+    elif format == "csv":
         with open(tmp_filename, "r", encoding="utf-8") as F:
             data = json.load(F)
         with open(filename, "w", encoding="utf-8") as F:
             keys = data[0].keys()
-            writer = csv.DictWriter(F, keys)
+            writer = csv.DictWriter(F, fieldnames=keys)
             writer.writeheader()
-            writer.writerows(data)
+            for row in data:
+                writer.writerow({k: v for k, v in row.items() if k in keys})
             os.remove(tmp_filename)
 
 
 def validate_key_value_format(ctx, param, value):
     try:
         key_value_pairs = []
         for pair in value:
```

### Comparing `estela-0.2/setup.py` & `estela-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="estela",
-    version="0.2",
+    version="0.2.1",
     description="Estela Command Line Interface",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "estela = estela_cli.__main__:cli",
         ],
     },
```

