# Comparing `tmp/pyees-1.2.4.tar.gz` & `tmp/pyees-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.2.4.tar", last modified: Thu May 11 12:22:09 2023, max compression
+gzip compressed data, was "pyees-1.2.5.tar", last modified: Thu May 11 18:59:49 2023, max compression
```

## Comparing `pyees-1.2.4.tar` & `pyees-1.2.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 12:22:09.124577 pyees-1.2.4/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.2.4/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-05-11 12:22:09.140204 pyees-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 12:22:08.859592 pyees-1.2.4/pyees/
--rw-rw-rw-   0        0        0      445 2023-04-21 11:08:47.000000 pyees-1.2.4/pyees/__init__.py
--rw-rw-rw-   0        0        0    12829 2023-05-11 09:38:32.000000 pyees-1.2.4/pyees/fit.py
--rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.2.4/pyees/profilePyees.py
--rw-rw-rw-   0        0        0     9126 2023-05-11 09:38:14.000000 pyees-1.2.4/pyees/prop.py
--rw-rw-rw-   0        0        0    14733 2023-04-24 15:08:43.000000 pyees-1.2.4/pyees/readData.py
--rw-rw-rw-   0        0        0    10193 2023-04-21 12:20:02.000000 pyees-1.2.4/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.2.4/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     7669 2023-04-27 10:39:41.000000 pyees-1.2.4/pyees/testFit.py
--rw-rw-rw-   0        0        0    12431 2023-05-11 09:11:30.000000 pyees-1.2.4/pyees/testProp.py
--rw-rw-rw-   0        0        0     1059 2023-04-27 11:06:19.000000 pyees-1.2.4/pyees/testPyees.py
--rw-rw-rw-   0        0        0    15674 2023-04-24 15:13:29.000000 pyees-1.2.4/pyees/testReadData.py
--rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.2.4/pyees/testSolve.py
--rw-rw-rw-   0        0        0     8958 2023-04-15 19:26:44.000000 pyees-1.2.4/pyees/testUnit.py
--rw-rw-rw-   0        0        0    81533 2023-05-11 11:53:42.000000 pyees-1.2.4/pyees/testVariable.py
--rw-rw-rw-   0        0        0    44518 2023-05-11 12:21:25.000000 pyees-1.2.4/pyees/unit.py
--rw-rw-rw-   0        0        0    35130 2023-05-11 11:54:28.000000 pyees-1.2.4/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-05-11 12:22:09.062077 pyees-1.2.4/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-05-11 12:22:07.000000 pyees-1.2.4/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-05-11 12:22:07.000000 pyees-1.2.4/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 12:22:07.000000 pyees-1.2.4/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-05-11 12:22:07.000000 pyees-1.2.4/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-11 12:22:07.000000 pyees-1.2.4/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-11 12:22:09.171454 pyees-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1216 2023-05-11 12:21:41.000000 pyees-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 18:59:49.409227 pyees-1.2.5/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.2.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-05-11 18:59:49.417206 pyees-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 18:59:49.101053 pyees-1.2.5/pyees/
+-rw-rw-rw-   0        0        0      323 2023-05-11 18:59:34.000000 pyees-1.2.5/pyees/__init__.py
+-rw-rw-rw-   0        0        0    12829 2023-05-11 09:38:32.000000 pyees-1.2.5/pyees/fit.py
+-rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.2.5/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0     9126 2023-05-11 09:38:14.000000 pyees-1.2.5/pyees/prop.py
+-rw-rw-rw-   0        0        0    17661 2023-05-11 18:51:21.000000 pyees-1.2.5/pyees/readData.py
+-rw-rw-rw-   0        0        0    10193 2023-04-21 12:20:02.000000 pyees-1.2.5/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.2.5/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     7669 2023-04-27 10:39:41.000000 pyees-1.2.5/pyees/testFit.py
+-rw-rw-rw-   0        0        0    12431 2023-05-11 09:11:30.000000 pyees-1.2.5/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1059 2023-05-11 18:59:48.854708 pyees-1.2.5/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    15674 2023-04-24 15:13:29.000000 pyees-1.2.5/pyees/testReadData.py
+-rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.2.5/pyees/testSolve.py
+-rw-rw-rw-   0        0        0     8958 2023-04-15 19:26:44.000000 pyees-1.2.5/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    81533 2023-05-11 18:59:49.041211 pyees-1.2.5/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    44518 2023-05-11 12:21:25.000000 pyees-1.2.5/pyees/unit.py
+-rw-rw-rw-   0        0        0    35130 2023-05-11 11:54:28.000000 pyees-1.2.5/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-05-11 18:59:49.362354 pyees-1.2.5/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-05-11 18:59:47.000000 pyees-1.2.5/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-05-11 18:59:48.000000 pyees-1.2.5/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 18:59:47.000000 pyees-1.2.5/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-05-11 18:59:47.000000 pyees-1.2.5/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-11 18:59:47.000000 pyees-1.2.5/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-11 18:59:49.460091 pyees-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2023-05-11 18:59:39.000000 pyees-1.2.5/setup.py
```

### Comparing `pyees-1.2.4/LICENSE.txt` & `pyees-1.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.2.4/PKG-INFO` & `pyees-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.2.4
+Version: 1.2.5
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.2.4/README.md` & `pyees-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.2.4/pyees/fit.py` & `pyees-1.2.5/pyees/fit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.4/pyees/profilePyees.py` & `pyees-1.2.5/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.4/pyees/prop.py` & `pyees-1.2.5/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.4/pyees/readData.py` & `pyees-1.2.5/pyees/readData.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,112 @@
 import numpy as np
 import openpyxl
 import xlrd
+import xlwt
 import os.path
 import re
 import string
 try:
-    from variable import variable
+    from variable import variable, scalarVariable
 except ImportError:
-    from pyees.variable import variable
+    from pyees.variable import variable, scalarVariable
 
-def fileFromSheets(Sheets):
-    ## TODO save Sheet as xlFile
-    raise NotImplementedError()
+
+
+def fileFromSheets(sheets, fileName):
+    _fileFromSheets(sheets, fileName)
+
+class _fileFromSheets():
+    def __init__(self, sheets, fileName) -> None:
+        
+        self.fileName = fileName
+        self.sheets = sheets
+        
+        extension = os.path.splitext(fileName)[1]
+        supportedExtensions = ['.xls', '.xlsx']
+        if extension not in supportedExtensions:
+            raise ValueError(f'The file extension is not supported. The supported extension are {supportedExtensions}')
+            
+        if extension == '.xls':
+            self.wb = xlwt.Workbook()                            
+            
+            def createSheet():
+                return self.wb.add_sheet()
+        
+            def write(sheet, row, col, value):
+                sheet.write(row, col, value)
+            
+            def getSheet(index):
+                return self.wb.add_sheet(f'Sheet {index + 1}')
+                       
+            
+        elif extension == '.xlsx':
+            self.wb = openpyxl.Workbook()
+            
+            def createSheet():
+                return self.wb.create_sheet()
+        
+            def write(sheet, row, col, value):
+                sheet.cell(row+1, col+1, value)
+            
+            def getSheet(index):
+                if index > 0:
+                    worksheet = self.createSheet()
+                else:
+                    worksheet = self.wb.active
+                return worksheet
+            
+        self.createSheet = createSheet
+        self.write = write
+        self.getSheet = getSheet
+        
+        self.saveSheets()
+        
+    def saveSheets(self):
+        
+        for ii, sheet in enumerate(self.sheets):
+            
+            worksheet = self.getSheet(ii)
+            
+            col = 0
+            for objectName in dir(sheet):
+                object = getattr(sheet, objectName)
+                if isinstance(object, scalarVariable):
+                    meas = object
+ 
+                    self.write(worksheet, 0, col, objectName)
+                    self.write(worksheet, 1, col, meas.unit)
+                    
+                    u = meas.unit
+                    scale = variable(1, u)
+                    meas /= scale
+                    
+                    for row, val in enumerate(meas):
+                        self.write(worksheet, row + 2, col, str(val))
+                    
+                    meas *= scale
+                                                
+                    col += 1          
+                         
+        self.wb.save(self.fileName)
+        
+            
+            
+        
+        
+        
 
 def sheetsFromFile(xlFile, dataRange: str | list[str], uncertRange: str | list[str] = None, sheets: int | list[int] = None):
-    dat = _SheetsFromFile(xlFile, dataRange, uncertRange, sheets)
+    dat = _sheetsFromFile(xlFile, dataRange, uncertRange, sheets)
     if len(dat.dat) == 1:
         return dat.dat[0]
     return dat.dat
 
 
-class _SheetsFromFile():
+class _sheetsFromFile():
 
     def __init__(self, xlFile, dataRange, uncertRange=None, sheets = None) -> None:
 
 
         # check the extension
         extension = os.path.splitext(xlFile)[1]
         supportedExtensions = ['.xls', '.xlsx']
@@ -183,47 +265,47 @@
                     raise ValueError(f'The header {head} could not be added to the sheet')
         return out
 
     def readData(self):
         self.dat = []
 
         # Looping over the sheets in the data file
-        for ii, sheet in enumerate(self.sheets):
+        for ii, sh in enumerate(self.sheets):
             
-            sheetData = Sheet()
+            sheetData = sheet()
             
             self.nCols = self.dataEndCol[ii] - self.dataStartCol[ii] + 1
             
             # determine the number of variables
-            headers = self.readRow(sheet, 0)[self.dataStartCol[ii]-1:self.dataStartCol[ii] - 1 + self.nCols]
+            headers = self.readRow(sh, 0)[self.dataStartCol[ii]-1:self.dataStartCol[ii] - 1 + self.nCols]
 
             headers = self.formatHeaders(headers)
-            units = self.readRow(sheet, 1)[self.dataStartCol[ii]-1:self.dataStartCol[ii] - 1 + self.nCols]
+            units = self.readRow(sh, 1)[self.dataStartCol[ii]-1:self.dataStartCol[ii] - 1 + self.nCols]
 
             # determine the number of datapoints
             nDataPoints = []
             for i in range(self.nCols):
-                nDataPoint = self.readCol(sheet, self.dataStartCol[ii] + i - 1)[2:]
+                nDataPoint = self.readCol(sh, self.dataStartCol[ii] + i - 1)[2:]
                 nDataPoint = sum([1 if elem not in ['', None] else 0 for elem in nDataPoint])
                 nDataPoints.append(nDataPoint)
             if not all(elem == nDataPoints[0] for elem in nDataPoints):
                 raise ValueError('There are not an equal amount of rows in the data')
             nDataPoint = nDataPoints[0]
 
             # read the data
             data = np.zeros([nDataPoint, self.nCols])
             for i in range(nDataPoint):
                 for j in range(self.nCols):
-                    data[i, j] = float(self.readCell(sheet, 2 + i, j+ self.dataStartCol[ii] - 1))
+                    data[i, j] = float(self.readCell(sh, 2 + i, j+ self.dataStartCol[ii] - 1))
 
             if not self.uncertStartCol[ii] is None:
                 # determine the number of rows in the uncertanty
                 nUncertanties = []
                 for i in range(self.nCols):
-                    nUncertanty = self.readCol(sheet, self.uncertStartCol[ii] - 1 + i)[2:]
+                    nUncertanty = self.readCol(sh, self.uncertStartCol[ii] - 1 + i)[2:]
                     nUncertanty = sum([1 if elem not in ['', None] else 0 for elem in nUncertanty])
                     nUncertanties.append(nUncertanty)
                 if not all(elem == nUncertanties[0] for elem in nUncertanties):
                     raise ValueError('There are not an equal amount of rows in the uncertanty')
                 nUncertanty = nUncertanties[0]
 
                 # evaluate the number of rows of the uncertanty
@@ -233,35 +315,36 @@
                 if nUncertanty == nDataPoint:
                     # There is one row of uncertanty for each row of data. Therefore there are no covariance data in the sheet
 
                     # read the uncertanty
                     uncert = np.zeros([nDataPoint, self.nCols])
                     for i in range(nDataPoint):
                         for j in range(self.nCols):
-                            uncert[i, j] = float(self.readCell(sheet, 2 + i, self.uncertStartCol[ii] - 1 + j))
+                            uncert[i, j] = float(self.readCell(sh, 2 + i, self.uncertStartCol[ii] - 1 + j))
 
                     # create the measurements uncertanties
                     for i in range(self.nCols):
                         name = headers[i]
                         unit = units[i]
                         val = np.array(data[:, i])
                         u = np.array(uncert[:, i])
                         var = variable(val, unit, uncert=u)
 
-                        sheetData._addMeasurement(name, var)
+                        setattr(sheetData, name, var)
+
                 else:
                     # There are covariance data in the sheet
 
                     # read the uncertanty
                     uncert = []
                     for i in range(nDataPoint):
                         u = np.zeros([self.nCols, self.nCols])
                         for j in range(self.nCols):
                             for k in range(self.nCols):
-                                u[j, k] = float(self.readCell(sheet, 2 + i * self.nCols + j, self.uncertStartCol[ii] - 1 + k))
+                                u[j, k] = float(self.readCell(sh, 2 + i * self.nCols + j, self.uncertStartCol[ii] - 1 + k))
                         uncert.append(u)
 
                     # check if each element in the uncertanty is symmetric
                     for elem in uncert:
                         if (elem.shape == elem.transpose().shape) and (elem == elem.transpose()).all():
                             pass
                         else:
@@ -281,78 +364,83 @@
                         covariance = [elem[:, i] for elem in uncert]
                         for j in range(self.nCols):
                             if i != j:
                                 cov = [elem[j] for elem in covariance]
                                 vars[i].addCovariance(vars[j], cov, str(vars[i]._unitObject * vars[j]._unitObject))
 
                     for head, var in zip(headers, vars):
-                        sheetData._addMeasurement(head, var)
+                        setattr(sheetData, head, var)
             else:
                 # There are no uncertaty data in the sheet
 
                 # create the measurements without uncertanties
                 for i in range(self.nCols):
                     name = headers[i]
                     unit = units[i]
                     val = np.array(data[:, i])
                     var = variable(val, unit)
-                    sheetData._addMeasurement(name, var)
+                    setattr(sheetData, name, var)
 
             self.dat.append(sheetData)
 
 
 
-class Sheet():
+class sheet():
     def __init__(self):
-        self.measurements = []
-        self.measurementNames = []
-
-    def _addMeasurement(self, name, var):
-        self.measurements.append(var)
-        self.measurementNames.append(name)
-        setattr(self, name, var)
+        pass
 
     def printContents(self):
-        for name in self.measurementNames:
-            print(name)
+        for key, item in self.__dict__.items():
+            if isinstance(item, scalarVariable):
+                print(key)
 
     def __getitem__(self, index):
-        measurements = []
-        for meas in self.measurements:
-            val = meas.value[index]
-            unit = meas.unit
-            uncert = meas.uncert[index]
-            measurements.append(variable(val, unit, uncert))
-
-        sheet = Sheet()
-
-        for measurement, measurementName in zip(measurements, self.measurementNames):
-            sheet._addMeasurement(measurementName, measurement)
-
-        return sheet
+        sh = sheet()
+        for key, item in self.__dict__.items():
+            if isinstance(item, scalarVariable):
+                setattr(sh, key, item[index])
+        return sh
 
     def append(self, other):
-        if not isinstance(other, Sheet):
+        if not isinstance(other, sheet):
             raise ValueError('You can only append two sheets together')
 
+        selfMeasurements = []
+        selfMeasurementNames = []
+        otherMeasurements = []
+        otherMeasurementNames = []
+        
+        for key,item in self.__dict__.items():
+            if isinstance(item,scalarVariable):
+                selfMeasurementNames.append(key)
+                selfMeasurements.append(item)
+
+        for key,item in other.__dict__.items():
+            if isinstance(item,scalarVariable):
+                otherMeasurementNames.append(key)
+                otherMeasurements.append(item)
+
         # Test if all names are the same
-        for elem in self.measurementNames:
-            if elem not in other.measurementNames:
+        for elem in selfMeasurementNames:
+            if elem not in otherMeasurementNames:
                 raise ValueError('You can only append sheets with the excact same measurements. The names did not match')
 
-        for elem in other.measurementNames:
-            if elem not in self.measurementNames:
+        for elem in otherMeasurementNames:
+            if elem not in selfMeasurementNames:
                 raise ValueError('You can only append sheets with the excact same measurements. The names did not match')
 
         # append the measurements from other to self
-        for elem, elemNames in zip(self.measurements, self.measurementNames):
-            index = other.measurementNames.index(elemNames)
-            elem.append(other.measurements[index])    
+        for measurement, measurementName in zip(selfMeasurements, selfMeasurementNames):
+            index = otherMeasurementNames.index(measurementName)
+            measurement.append(otherMeasurements[index])    
         
     def __iter__(self):
-        return iter(self.measurements)
-
-
+        
+        variables = []
+        for _, item in self.__dict__.items():
+            if isinstance(item, scalarVariable):
+                variables.append(item)
+        
+        return iter(variables)
     
     
-
-
+
```

### Comparing `pyees-1.2.4/pyees/solve.py` & `pyees-1.2.5/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.4/pyees/stackOverflowODR.py` & `pyees-1.2.5/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.4/pyees/testFit.py` & `pyees-1.2.5/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.4/pyees/testProp.py` & `pyees-1.2.5/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.4/pyees/testPyees.py` & `pyees-1.2.5/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.4/pyees/testReadData.py` & `pyees-1.2.5/pyees/testReadData.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.4/pyees/testSolve.py` & `pyees-1.2.5/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.4/pyees/testUnit.py` & `pyees-1.2.5/pyees/testUnit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.4/pyees/testVariable.py` & `pyees-1.2.5/pyees/testVariable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.4/pyees/unit.py` & `pyees-1.2.5/pyees/unit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.4/pyees/variable.py` & `pyees-1.2.5/pyees/variable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.4/pyees.egg-info/PKG-INFO` & `pyees-1.2.5/pyees.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.2.4
+Version: 1.2.5
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.2.4/setup.py` & `pyees-1.2.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.2.4',
+    version='1.2.5',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
     install_requires=[            # I get to this in a second
-        'numpy', 'scipy', 'openpyxl', 'xlrd', 'pyfluids'
+        'numpy', 'scipy', 'openpyxl', 'xlrd', 'pyfluids', 'xlwt'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',      # Define that your audience are developers
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',  # Specify which pyhton versions that you want to support
```

