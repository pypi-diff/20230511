# Comparing `tmp/iosense_connect-2.1.2.tar.gz` & `tmp/iosense_connect-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect-2.1.2.tar", last modified: Wed May 10 12:01:34 2023, max compression
+gzip compressed data, was "dist\iosense_connect-2.1.3.tar", last modified: Thu May 11 06:07:42 2023, max compression
```

## Comparing `iosense_connect-2.1.2.tar` & `iosense_connect-2.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 12:01:34.912703 iosense_connect-2.1.2/
--rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-2.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1062 2023-05-10 12:01:34.909015 iosense_connect-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-2.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 12:01:34.621196 iosense_connect-2.1.2/iosense_connect/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.1.2/iosense_connect/__init__.py
--rw-rw-rw-   0        0        0    22027 2023-05-10 12:00:03.000000 iosense_connect-2.1.2/iosense_connect/data_access.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:01:34.900920 iosense_connect-2.1.2/iosense_connect.egg-info/
--rw-rw-rw-   0        0        0     1062 2023-05-10 12:01:33.000000 iosense_connect-2.1.2/iosense_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-05-10 12:01:33.000000 iosense_connect-2.1.2/iosense_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 12:01:33.000000 iosense_connect-2.1.2/iosense_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-10 12:01:33.000000 iosense_connect-2.1.2/iosense_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 12:01:34.913701 iosense_connect-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0      614 2023-05-10 11:59:25.000000 iosense_connect-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 06:07:42.320991 iosense_connect-2.1.3/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-2.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1062 2023-05-11 06:07:42.320991 iosense_connect-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-2.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 06:07:42.258495 iosense_connect-2.1.3/iosense_connect/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.1.3/iosense_connect/__init__.py
+-rw-rw-rw-   0        0        0    22553 2023-05-11 06:07:34.000000 iosense_connect-2.1.3/iosense_connect/data_access.py
+drwxrwxrwx   0        0        0        0 2023-05-11 06:07:42.320991 iosense_connect-2.1.3/iosense_connect.egg-info/
+-rw-rw-rw-   0        0        0     1062 2023-05-11 06:07:41.000000 iosense_connect-2.1.3/iosense_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-05-11 06:07:41.000000 iosense_connect-2.1.3/iosense_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 06:07:41.000000 iosense_connect-2.1.3/iosense_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-11 06:07:41.000000 iosense_connect-2.1.3/iosense_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 06:07:42.320991 iosense_connect-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      614 2023-05-11 06:07:35.000000 iosense_connect-2.1.3/setup.py
```

### Comparing `iosense_connect-2.1.2/LICENSE.txt` & `iosense_connect-2.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iosense_connect-2.1.2/PKG-INFO` & `iosense_connect-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense_connect
-Version: 2.1.2
+Version: 2.1.3
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-2.1.2/README.md` & `iosense_connect-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `iosense_connect-2.1.2/iosense_connect/data_access.py` & `iosense_connect-2.1.3/iosense_connect/data_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -453,28 +453,37 @@
                     end_time = datetime.strptime(end_time, '%Y-%m-%d %H:%M:%S')
                     df = df[(df['time'] >= start_time) & (df['time'] <= end_time)]
                 except ValueError:
                     df = df[(df['time'] >= start_time) & (df['time'] <= end_time)]
                     pass
                 except Exception as e:
                     print('Message: \t',e)
-                if sensors != None:
-                    sensors.insert(0,'time')
-                    df =  df[sensors]
-                df.reset_index(drop=True, inplace=True)
-                last_date = df['time'].iloc[len(df) - 1]
-                start_date = last_date.date() + timedelta(days=1)
-                end_time = pd.to_datetime(end_time)
-                if last_date.date() != end_time.date():
-                    df1 = DataAccess.fetch_data(self, device_id ,start_time=str(start_date), alias=False,end_time=end_time,sensors=sensors, echo=True,onpremise=False,IST=True)
-                    df = pd.concat([df, df1])
-                else:
-                    df1 = DataAccess.fetch_data(self, device_id,start_time=str(last_date), alias=False,end_time=end_time,sensors=sensors, echo=True,onpremise=False,IST=True)
-                    df = pd.concat([df, df1])
-                df.reset_index(drop=True, inplace=True)
+                if sensors is None:
+                    sensors = list(df.columns)
+                    sensors.remove('time')
+                sensor_list_df = list(df.columns)
+                sensor_list_df.remove('time')
+                sensors_filtered = list(set(sensor_list_df).intersection(sensors))
+                if sensors != None and len(sensors_filtered) != 0:
+                    sensors_filtered.insert(0,'time')
+                    df =  df[sensors_filtered]
+                if len(sensors_filtered) == 0:
+                    df = pd.DataFrame()
+                if len(df) !=0:
+                    df.reset_index(drop=True, inplace=True)
+                    last_date = df['time'].iloc[len(df) - 1]
+                    start_date = last_date.date() + timedelta(days=1)
+                    end_time = pd.to_datetime(end_time)
+                    if last_date.date() != end_time.date():
+                        df1 = DataAccess.fetch_data(self, device_id ,start_time=str(start_date), alias=False,end_time=end_time,sensors=sensors, echo=True,onpremise=False,IST=True)
+                        df = pd.concat([df, df1])
+                    else:
+                        df1 = DataAccess.fetch_data(self, device_id,start_time=str(last_date), alias=False,end_time=end_time,sensors=sensors, echo=True,onpremise=False,IST=True)
+                        df = pd.concat([df, df1])
+                    df.reset_index(drop=True, inplace=True)
             else:
                 df_devices = DataAccess.get_device_details(self)
                 device_list = df_devices['devID'].tolist()
                 if device_id in device_list:
                     df = DataAccess.fetch_data(self, device_id, start_time,end_time, alias,sensors=sensors,echo=True,onpremise=onpremise,IST=IST)
                 else:
                     raise Exception('Message: Device not added in account')
```

### Comparing `iosense_connect-2.1.2/iosense_connect.egg-info/PKG-INFO` & `iosense_connect-2.1.3/iosense_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense-connect
-Version: 2.1.2
+Version: 2.1.3
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-2.1.2/setup.py` & `iosense_connect-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "iosense_connect",
-    version = "2.1.2",
+    version = "2.1.3",
     author = "Faclon-Labs",
     author_email = "reachus@faclon.com",
     description = "iosense connect library",
     packages = ["iosense_connect"],
     long_description = long_description,
     long_description_content_type = "text/markdown",
     classifiers = [
```

