# Comparing `tmp/exergenics-2.8.0.tar.gz` & `tmp/exergenics-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exergenics-2.8.0.tar", last modified: Wed May  3 02:26:44 2023, max compression
+gzip compressed data, was "exergenics-2.9.0.tar", last modified: Thu May 11 01:56:55 2023, max compression
```

## Comparing `exergenics-2.8.0.tar` & `exergenics-2.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:26:44.858461 exergenics-2.8.0/
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-03 02:26:44.858461 exergenics-2.8.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:26:44.858461 exergenics-2.8.0/exergenics/
--rw-rw-r--   0 root         (0) root         (0)       37 2023-05-03 02:25:28.000000 exergenics-2.8.0/exergenics/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    62080 2023-05-03 02:25:28.000000 exergenics-2.8.0/exergenics/exergenics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:26:44.858461 exergenics-2.8.0/exergenics.egg-info/
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-03 02:26:44.000000 exergenics-2.8.0/exergenics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      225 2023-05-03 02:26:44.000000 exergenics-2.8.0/exergenics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 02:26:44.000000 exergenics-2.8.0/exergenics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-05-03 02:26:44.000000 exergenics-2.8.0/exergenics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-03 02:26:44.000000 exergenics-2.8.0/exergenics.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 02:26:44.858461 exergenics-2.8.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      672 2023-05-03 02:26:42.000000 exergenics-2.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 01:56:55.689067 exergenics-2.9.0/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-11 01:56:55.689067 exergenics-2.9.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 01:56:55.689067 exergenics-2.9.0/exergenics/
+-rw-rw-r--   0 root         (0) root         (0)       37 2023-05-11 01:55:36.000000 exergenics-2.9.0/exergenics/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    62506 2023-05-11 01:55:36.000000 exergenics-2.9.0/exergenics/exergenics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 01:56:55.689067 exergenics-2.9.0/exergenics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-11 01:56:55.000000 exergenics-2.9.0/exergenics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      225 2023-05-11 01:56:55.000000 exergenics-2.9.0/exergenics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 01:56:55.000000 exergenics-2.9.0/exergenics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-05-11 01:56:55.000000 exergenics-2.9.0/exergenics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-11 01:56:55.000000 exergenics-2.9.0/exergenics.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 01:56:55.689067 exergenics-2.9.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      672 2023-05-11 01:56:53.000000 exergenics-2.9.0/setup.py
```

### Comparing `exergenics-2.8.0/exergenics/exergenics.py` & `exergenics-2.9.0/exergenics/exergenics.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,16 @@
     ex__setJobData = "setJobData"
     ex__setStage = "setStage"
     ex__getWeather = "getWeather"
     ex__sendCSVToPortal = "sendCSVToPortal"
     ex__setEquipmentVariableValue = "setEquipmentVariable"
     ex__getEquipmentVariableValue = "getEquipmentVariable"
 
+    ex__getReportData = "getReport"
+
     slackEndpoint = "https://slack.com/api/chat.postMessage"
 
     # Constructor - assign credentials
     def __init__(self, username="", password="", useProductionApi=True, token=None, database="default"):
         if token is not None:
             self.authorizationToken = token
         else:
@@ -306,14 +308,22 @@
 
         req = "https://" + subDomain + ".exergenicsportal.com/api/ex/index.php?I_AM_LAMBDA=eyJraWQiOiJpRlwvb0dLamdOTjdLMlEwMWNFRndXUkFROWFZWWdKZ3BBZlNOdDJyWWFIQT0iLCJhbGciOiJSUzI1NiJ9&path=/getWeather/" + buildingCode + "&httpMethod=GET&awsSubscriptionKey=7b786790-6e4e-4310-bfc7-d30aec6beb02&queryStringParameters={\"distance\":" + \
               str(distance) + \
               "}&postParams=&whoAmI=getWeatherProduction&"
         request = requests.get(req)
         return request.json()["body"]
 
+    def getReportData(self, jobId):
+        activityUrl = "{}/{}".format(self.ex__getReportData, jobId)
+        self.lastStatus, self.lastResponse = self.doRequest(
+            self.getExchangeEndpoint(), activityUrl, {})
+        if self.noResponse():
+            return False
+        return self.lastResponse
+
     def setEquipmentVariableValue(self, plantCode, equipmentTag, variableName, variableValue):
         activityUrl = "{}/{}/{}/?variableName={}&variableValue={}".format(self.ex__setEquipmentVariableValue, plantCode,
                                                                           equipmentTag, variableName, variableValue)
         self.lastStatus, self.lastResponse = self.doRequest(
             self.getExchangeEndpoint(), activityUrl, {})
         if self.noResponse():
             return False
@@ -1180,35 +1190,36 @@
                                                   titleColor)
         self.putFile(plantCode, urlToChart, portalCategory,
                      chartName, equipCode, jobId)
         return urlToChart
     
     def portalChart_generalised3D(self, plantCode, chartName, portalCategory, dataJSON,
                                       xAxisTitle="xAxisTitle", yAxisTitle="yAxisTitle", zAxisTitle="zAxisTitle",
-                                      fileName="fileName", backgroundColor="white", fontSize=16, fontFamily="Verdana",
-                                      fontColor="black", legendFamily="Verdana", legendSize=15, legendColor="black",
+                                      fileName="fileName", markerSize=3, backgroundColor="white", fontSize=12, fontFamily="Verdana",
+                                      fontColor="black", legendFamily="Verdana", legendSize=12, legendColor="black",
                                       legendBg="LightSteelBlue", equipCode="", jobId=""):
-        urlToChart = self.plotlyGeneralised3D(dataJSON, xAxisTitle, yAxisTitle, zAxisTitle, fileName,
+        urlToChart = self.plotlyGeneralised3D(dataJSON, xAxisTitle, yAxisTitle, zAxisTitle, fileName, markerSize,
                                                   backgroundColor, fontSize, fontFamily, fontColor, legendFamily,
                                                   legendSize, legendColor, legendBg)
         self.putFile(plantCode, urlToChart, portalCategory,
                      chartName, equipCode, jobId)
         return urlToChart
 
     def plotlyGeneralised3D(self, dataJSON, xAxisTitle="xAxisTitle", yAxisTitle="yAxisTitle", zAxisTitle="zAxisTitle",
-                                fileName="fileName", backgroundColor="white", fontSize=16, fontFamily="Verdana",
-                                fontColor="black", legendFamily="Verdana", legendSize=15, legendColor="black",
+                                fileName="fileName", markerSize=3, backgroundColor="white", fontSize=12, fontFamily="Verdana",
+                                fontColor="black", legendFamily="Verdana", legendSize=12, legendColor="black",
                                 legendBg="LightSteelBlue"):
 
         return self.plotlyRequest("generalised3D", {
             "dataJSON": dataJSON,
             "xAxisTitle": xAxisTitle,
             "yAxisTitle": yAxisTitle,
             "zAxisTitle": zAxisTitle,
             "fileName": fileName,
+            "markerSize": markerSize,
             "backgroundColor": backgroundColor,
             "fontSize": fontSize,
             "fontFamily": fontFamily,
             "fontColor": fontColor,
             "legendFamily": legendFamily,
             "legendSize": legendSize,
             "legendColor": legendColor,
```

### Comparing `exergenics-2.8.0/setup.py` & `exergenics-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='exergenics',
-    version='2.8.0',
+    version='2.9.0',
     author="John Christian",
     author_email='john.christian@exergenics.com',
     packages=['exergenics'],
     long_description="",
     long_description_content_type="text/markdown",
     # package_dir={'': 'src'},
     url='https://github.com/Exergenics/internal-portal-api',
```

