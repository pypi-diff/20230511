# Comparing `tmp/itkdb_gtk-0.0.3.tar.gz` & `tmp/itkdb_gtk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itkdb_gtk-0.0.3.tar", last modified: Fri Apr 21 09:11:16 2023, max compression
+gzip compressed data, was "itkdb_gtk-0.0.4.tar", last modified: Thu May 11 14:06:58 2023, max compression
```

## Comparing `itkdb_gtk-0.0.3.tar` & `itkdb_gtk-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-21 09:11:16.519912 itkdb_gtk-0.0.3/
--rw-r--r--   0 lacasta    (503) staff       (20)     2499 2023-04-21 09:11:16.519702 itkdb_gtk-0.0.3/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)     1997 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.3/README.md
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-21 09:11:16.517522 itkdb_gtk-0.0.3/itkdb_gtk/
--rw-r--r--   0 lacasta    (503) staff       (20)    12287 2023-04-21 09:11:07.000000 itkdb_gtk-0.0.3/itkdb_gtk/GlueWeight.py
--rw-r--r--   0 lacasta    (503) staff       (20)     9902 2023-03-21 10:25:38.000000 itkdb_gtk-0.0.3/itkdb_gtk/ITkDBlogin.py
--rw-r--r--   0 lacasta    (503) staff       (20)    14205 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.3/itkdb_gtk/ITkDButils.py
--rw-r--r--   0 lacasta    (503) staff       (20)      552 2023-04-11 16:04:01.000000 itkdb_gtk-0.0.3/itkdb_gtk/__init__.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3342 2023-04-13 14:46:29.000000 itkdb_gtk-0.0.3/itkdb_gtk/checkComponent.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4376 2023-04-21 09:02:02.000000 itkdb_gtk-0.0.3/itkdb_gtk/dashBoard.py
--rw-r--r--   0 lacasta    (503) staff       (20)    20708 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.3/itkdb_gtk/dbGtkUtils.py
--rw-r--r--   0 lacasta    (503) staff       (20)    18718 2023-04-11 15:15:43.000000 itkdb_gtk-0.0.3/itkdb_gtk/getShipments.py
--rw-r--r--   0 lacasta    (503) staff       (20)     7140 2023-04-11 15:50:48.000000 itkdb_gtk-0.0.3/itkdb_gtk/groundingTest.py
--rw-r--r--   0 lacasta    (503) staff       (20)    19401 2023-04-11 15:22:03.000000 itkdb_gtk-0.0.3/itkdb_gtk/readAVSdata.py
--rw-r--r--   0 lacasta    (503) staff       (20)     2679 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.3/itkdb_gtk/readGoogleSheet.py
--rw-r--r--   0 lacasta    (503) staff       (20)    13133 2023-04-11 15:22:19.000000 itkdb_gtk-0.0.3/itkdb_gtk/sendShipments.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    21093 2023-04-11 15:23:27.000000 itkdb_gtk-0.0.3/itkdb_gtk/uploadPetalInformation.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    12171 2023-04-11 15:53:15.000000 itkdb_gtk-0.0.3/itkdb_gtk/uploadTest.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-21 09:11:16.519402 itkdb_gtk-0.0.3/itkdb_gtk.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)     2499 2023-04-21 09:11:16.000000 itkdb_gtk-0.0.3/itkdb_gtk.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      587 2023-04-21 09:11:16.000000 itkdb_gtk-0.0.3/itkdb_gtk.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-04-21 09:11:16.000000 itkdb_gtk-0.0.3/itkdb_gtk.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      239 2023-04-21 09:11:16.000000 itkdb_gtk-0.0.3/itkdb_gtk.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       62 2023-04-21 09:11:16.000000 itkdb_gtk-0.0.3/itkdb_gtk.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-04-21 09:11:16.000000 itkdb_gtk-0.0.3/itkdb_gtk.egg-info/top_level.txt
--rw-r--r--   0 lacasta    (503) staff       (20)     1083 2023-04-21 09:08:15.000000 itkdb_gtk-0.0.3/pyproject.toml
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-04-21 09:11:16.519975 itkdb_gtk-0.0.3/setup.cfg
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-11 14:06:58.786760 itkdb_gtk-0.0.4/
+-rw-r--r--   0 lacasta    (503) staff       (20)     2499 2023-05-11 14:06:58.786448 itkdb_gtk-0.0.4/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)     1997 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.4/README.md
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-11 14:06:58.783218 itkdb_gtk-0.0.4/itkdb_gtk/
+-rw-r--r--   0 lacasta    (503) staff       (20)    12294 2023-05-11 14:03:05.000000 itkdb_gtk-0.0.4/itkdb_gtk/GlueWeight.py
+-rw-r--r--   0 lacasta    (503) staff       (20)      172 2023-04-21 15:44:09.000000 itkdb_gtk-0.0.4/itkdb_gtk/ITkDB.desktop
+-rw-r--r--   0 lacasta    (503) staff       (20)    23991 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.4/itkdb_gtk/ITkDB.svg
+-rw-r--r--   0 lacasta    (503) staff       (20)     9902 2023-03-21 10:25:38.000000 itkdb_gtk-0.0.4/itkdb_gtk/ITkDBlogin.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    14208 2023-05-11 14:04:07.000000 itkdb_gtk-0.0.4/itkdb_gtk/ITkDButils.py
+-rw-r--r--   0 lacasta    (503) staff       (20)      552 2023-04-11 16:04:01.000000 itkdb_gtk-0.0.4/itkdb_gtk/__init__.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     3342 2023-04-13 14:46:29.000000 itkdb_gtk-0.0.4/itkdb_gtk/checkComponent.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     1432 2023-05-11 13:27:56.000000 itkdb_gtk-0.0.4/itkdb_gtk/checkJSon.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4375 2023-05-11 14:02:42.000000 itkdb_gtk-0.0.4/itkdb_gtk/dashBoard.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    20708 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.4/itkdb_gtk/dbGtkUtils.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    18718 2023-04-11 15:15:43.000000 itkdb_gtk-0.0.4/itkdb_gtk/getShipments.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     7140 2023-04-11 15:50:48.000000 itkdb_gtk-0.0.4/itkdb_gtk/groundingTest.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    19401 2023-04-11 15:22:03.000000 itkdb_gtk-0.0.4/itkdb_gtk/readAVSdata.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     2679 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.4/itkdb_gtk/readGoogleSheet.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    13133 2023-04-11 15:22:19.000000 itkdb_gtk-0.0.4/itkdb_gtk/sendShipments.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)    21093 2023-04-11 15:23:27.000000 itkdb_gtk-0.0.4/itkdb_gtk/uploadPetalInformation.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)    13382 2023-05-11 14:04:28.000000 itkdb_gtk-0.0.4/itkdb_gtk/uploadTest.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-11 14:06:58.785988 itkdb_gtk-0.0.4/itkdb_gtk.egg-info/
+-rw-r--r--   0 lacasta    (503) staff       (20)     2499 2023-05-11 14:06:58.000000 itkdb_gtk-0.0.4/itkdb_gtk.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      654 2023-05-11 14:06:58.000000 itkdb_gtk-0.0.4/itkdb_gtk.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-05-11 14:06:58.000000 itkdb_gtk-0.0.4/itkdb_gtk.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      239 2023-05-11 14:06:58.000000 itkdb_gtk-0.0.4/itkdb_gtk.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       62 2023-05-11 14:06:58.000000 itkdb_gtk-0.0.4/itkdb_gtk.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-05-11 14:06:58.000000 itkdb_gtk-0.0.4/itkdb_gtk.egg-info/top_level.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)     1087 2023-05-11 14:01:25.000000 itkdb_gtk-0.0.4/pyproject.toml
+-rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-05-11 14:06:58.786878 itkdb_gtk-0.0.4/setup.cfg
```

### Comparing `itkdb_gtk-0.0.3/PKG-INFO` & `itkdb_gtk-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkdb_gtk
-Version: 0.0.3
+Version: 0.0.4
 Summary: A collection of Gtk based GUI to access ITkDB.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `itkdb_gtk-0.0.3/README.md` & `itkdb_gtk-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.3/itkdb_gtk/GlueWeight.py` & `itkdb_gtk-0.0.4/itkdb_gtk/GlueWeight.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,23 +352,23 @@
 
     def upload_tests(self):
         """Upload tests to DB."""
         if len(self.test_list):
             for G in self.test_list:
                 m = G.values
                 print("### Uploading {} for module {}".format(m["testType"], m["component"]))
-                resp = ITkDButils.upload_test(session, m)
+                resp = ITkDButils.upload_test(self.session, m)
 
                 if resp is not None:
                     print(resp)
 
         else:
             for m in self.modules:
                 print("### Uploading {} for module {}".format(m["testType"], m["component"]))
-                resp = ITkDButils.upload_test(session, m)
+                resp = ITkDButils.upload_test(self.session, m)
 
                 if resp is not None:
                     print(resp)
 
 
 def main():
     """Main entry."""
@@ -421,10 +421,11 @@
     else:
         GW.modules = GW.parse_file(ifile)
         print(json.dumps(GW.modules, indent=2))
         GW.upload_tests()
         ifile.close()
 
     dlg.die()
-    
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `itkdb_gtk-0.0.3/itkdb_gtk/ITkDBlogin.py` & `itkdb_gtk-0.0.4/itkdb_gtk/ITkDBlogin.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.3/itkdb_gtk/ITkDButils.py` & `itkdb_gtk-0.0.4/itkdb_gtk/ITkDButils.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,15 @@
                 db_response = client.post('createTestRunAttachment',
                                           data=data,
                                           files=attachment)
 
         return None
 
     except Exception as e:
-        return(str(e))
+        return (str(e))
 
 
 def create_shipment(session, sender, recipient, items, name=None, send=False, type="domestic",
                     attachment=None, comments=None):
     """Create a chipment.
 
     Args:
@@ -490,15 +490,15 @@
         # print(json.dumps(vin, indent=1))
         if vin['valueType'] == "single":
             vtype = vin['dataType']
             val = None
             if vtype in uservalues:
                 val = uservalues[vtype]
             else:
-                print("default for data type ", vtype, " not found")
+                # print("default for data type ", vtype, " not found")
                 val = None
 
         else:
             val = None
 
         return val
```

### Comparing `itkdb_gtk-0.0.3/itkdb_gtk/__init__.py` & `itkdb_gtk-0.0.4/itkdb_gtk/__init__.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.3/itkdb_gtk/checkComponent.py` & `itkdb_gtk-0.0.4/itkdb_gtk/checkComponent.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.3/itkdb_gtk/dashBoard.py` & `itkdb_gtk-0.0.4/itkdb_gtk/dashBoard.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,14 @@
         recS.connect("clicked", self.receive_shipment)
         grid.attach(recS, 1, irow, 1, 1,)
 
         self.mainBox.pack_start(Gtk.Separator(orientation=Gtk.Orientation.HORIZONTAL), False, True, 5)
 
         self.show_all()
 
-
     def upload_test(self, *args):
         """Launch upload test."""
         bitn = 1
         bt = 1 << bitn
         if self.mask & bt:
             return
```

### Comparing `itkdb_gtk-0.0.3/itkdb_gtk/dbGtkUtils.py` & `itkdb_gtk-0.0.4/itkdb_gtk/dbGtkUtils.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.3/itkdb_gtk/getShipments.py` & `itkdb_gtk-0.0.4/itkdb_gtk/getShipments.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.3/itkdb_gtk/groundingTest.py` & `itkdb_gtk-0.0.4/itkdb_gtk/groundingTest.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.3/itkdb_gtk/readAVSdata.py` & `itkdb_gtk-0.0.4/itkdb_gtk/readAVSdata.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.3/itkdb_gtk/readGoogleSheet.py` & `itkdb_gtk-0.0.4/itkdb_gtk/readGoogleSheet.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.3/itkdb_gtk/sendShipments.py` & `itkdb_gtk-0.0.4/itkdb_gtk/sendShipments.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.3/itkdb_gtk/uploadPetalInformation.py` & `itkdb_gtk-0.0.4/itkdb_gtk/uploadPetalInformation.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.3/itkdb_gtk/uploadTest.py` & `itkdb_gtk-0.0.4/itkdb_gtk/uploadTest.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,31 +28,33 @@
         data (): The json data
 
     Returns
     -------
         boolean: True if valid, False otherwise.
 
     """
+    errors = []
+    missing = []
     if "component" not in data:
-        print("Need reference to component, hex string")
-        return False
+        errors.append("Need reference to component, hex string")
+        missing.append("component")
 
     if "testType" not in data:
-        print("Need to know test type, short code")
-        return False
+        errors.append("Need to know test type, short code")
+        missing.append("testType")
 
     if "institution" not in data:
-        print("Need to know institution, short code")
-        return False
+        errors.append("Need to know institution, short code")
+        missing.append("institution")
 
     if "results" not in data:
-        print("Need some test results")
-        return False
+        errors.append("Need some test results")
+        missing.append("results")
 
-    return True
+    return errors, missing
 
 
 class UploadTest(dbGtkUtils.ITkDBWindow):
     """Collects informatio to upload a test and its attachments."""
 
     def __init__(self, session, payload=None, attachment=None):
         """Initialization.
@@ -195,23 +197,56 @@
 
         renderer = Gtk.CellRendererText()
         column = Gtk.TreeViewColumn("Description", renderer, text=2)
         self.tree.append_column(column)
 
         return scrolled
 
+    def get_test_institute(self):
+        """Select an institue."""
+        dlg = Gtk.Dialog(title="Select Institution.", flags=0)
+        dlg.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL,
+                        Gtk.STOCK_OK, Gtk.ResponseType.OK)
+        area = dlg.get_content_area()
+        box = Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
+        area.add(box)
+
+        box.pack_start(Gtk.Label(label="Select an Institute"), False, True, 0)
+
+        combo = self.create_institute_combo()
+        box.pack_start(combo, False, True, 5)
+
+        dlg.show_all()
+        rc = dlg.run()
+
+        out = None
+        if rc == Gtk.ResponseType.OK:
+            out = self.get_institute_from_combo(combo)
+
+        dlg.hide()
+        dlg.destroy()
+        return out
+
     def on_test_file(self, fdlg):
         """Test file browser clicked."""
         fnam = fdlg.get_filename()
 
         # The file exists by definition
         try:
             self.data = json.loads(open(fnam).read())
-            if not check_data(self.data):
-                dbGtkUtils.complain("Invalid JSON file", fnam)
+            errors, missing = check_data(self.data)
+
+            if len(missing):
+                if "institution" in missing and len(missing) == 1:
+                    site = self.get_test_institute()
+                    if site:
+                        self.data["institution"] = site
+                else:
+                    dbGtkUtils.complain("Invalid JSON file\n{}".format('\n'.join(errors)), fnam)
+
                 return
 
             self.entrySN.set_text(self.data["component"])
             self.entryTest.set_text(self.data["testType"])
 
         except Exception as E:
             self.data = None
@@ -329,14 +364,15 @@
             msg = rc[ipos:]
             dbGtkUtils.complain("Failed uploading test", msg)
 
         else:
             self.write_message("Upload successfull")
             dbGtkUtils.ask_for_confirmation("Upload successfull", "")
 
+
 def main():
     """Main entry."""
     parser = argparse.ArgumentParser()
 
     parser.add_argument("--test-file", help="Name of json file with test data")
     parser.add_argument("--component-id", help="Override component code")
     parser.add_argument("--raw_data", help="Raw data file", default=None)
@@ -377,8 +413,8 @@
         # Think
         pass
 
     dlg.die()
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `itkdb_gtk-0.0.3/itkdb_gtk.egg-info/PKG-INFO` & `itkdb_gtk-0.0.4/itkdb_gtk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkdb-gtk
-Version: 0.0.3
+Version: 0.0.4
 Summary: A collection of Gtk based GUI to access ITkDB.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `itkdb_gtk-0.0.3/itkdb_gtk.egg-info/SOURCES.txt` & `itkdb_gtk-0.0.4/itkdb_gtk.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 README.md
 pyproject.toml
 itkdb_gtk/GlueWeight.py
+itkdb_gtk/ITkDB.desktop
+itkdb_gtk/ITkDB.svg
 itkdb_gtk/ITkDBlogin.py
 itkdb_gtk/ITkDButils.py
 itkdb_gtk/__init__.py
 itkdb_gtk/checkComponent.py
+itkdb_gtk/checkJSon.py
 itkdb_gtk/dashBoard.py
 itkdb_gtk/dbGtkUtils.py
 itkdb_gtk/getShipments.py
 itkdb_gtk/groundingTest.py
 itkdb_gtk/readAVSdata.py
 itkdb_gtk/readGoogleSheet.py
 itkdb_gtk/sendShipments.py
```

### Comparing `itkdb_gtk-0.0.3/pyproject.toml` & `itkdb_gtk-0.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "itkdb_gtk"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@cern.ch" },
 ]
 description = "A collection of Gtk based GUI to access ITkDB."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
@@ -32,12 +32,12 @@
 sendShipments = "itkdb_gtk:sendShipments"
 uploadTest = "itkdb_gtk:uploadTest"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.package-data]
-mypkg = ["*.desktop", "*.svg"]
+itkdb_gtk = ["*.desktop", "*.svg"]
 
 [project.urls]
 "Homepage" = "https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils"
 "Bug Tracker" = "https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues"
```

