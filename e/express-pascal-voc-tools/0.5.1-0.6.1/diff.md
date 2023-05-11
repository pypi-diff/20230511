# Comparing `tmp/express-pascal-voc-tools-0.5.1.tar.gz` & `tmp/express-pascal-voc-tools-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "express-pascal-voc-tools-0.5.1.tar", last modified: Thu May 11 10:16:52 2023, max compression
+gzip compressed data, was "express-pascal-voc-tools-0.6.1.tar", last modified: Thu May 11 12:02:25 2023, max compression
```

## Comparing `express-pascal-voc-tools-0.5.1.tar` & `express-pascal-voc-tools-0.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 10:16:52.191170 express-pascal-voc-tools-0.5.1/
--rw-rw-rw-   0        0        0    35823 2023-05-09 09:49:08.000000 express-pascal-voc-tools-0.5.1/LICENSE
--rw-rw-rw-   0        0        0     4391 2023-05-11 10:16:52.187016 express-pascal-voc-tools-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     3907 2023-05-11 06:57:01.000000 express-pascal-voc-tools-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 10:16:52.139206 express-pascal-voc-tools-0.5.1/express_pascal_voc_tools.egg-info/
--rw-rw-rw-   0        0        0     4391 2023-05-11 10:16:51.000000 express-pascal-voc-tools-0.5.1/express_pascal_voc_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-05-11 10:16:51.000000 express-pascal-voc-tools-0.5.1/express_pascal_voc_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 10:16:51.000000 express-pascal-voc-tools-0.5.1/express_pascal_voc_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-11 10:16:51.000000 express-pascal-voc-tools-0.5.1/express_pascal_voc_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-11 10:16:51.000000 express-pascal-voc-tools-0.5.1/express_pascal_voc_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 10:16:52.191170 express-pascal-voc-tools-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      959 2023-05-11 08:00:59.000000 express-pascal-voc-tools-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 10:16:52.172016 express-pascal-voc-tools-0.5.1/voc_tools/
--rw-rw-rw-   0        0        0        0 2023-05-09 10:14:59.000000 express-pascal-voc-tools-0.5.1/voc_tools/__init__.py
--rw-rw-rw-   0        0        0      102 2023-05-11 08:12:31.000000 express-pascal-voc-tools-0.5.1/voc_tools/constants.py
--rw-rw-rw-   0        0        0     4536 2023-05-11 09:32:37.000000 express-pascal-voc-tools-0.5.1/voc_tools/reader.py
-drwxrwxrwx   0        0        0        0 2023-05-11 10:16:52.180017 express-pascal-voc-tools-0.5.1/voc_tools/unittest/
--rw-rw-rw-   0        0        0        0 2023-05-09 12:15:29.000000 express-pascal-voc-tools-0.5.1/voc_tools/unittest/__init__.py
--rw-rw-rw-   0        0        0     2900 2023-05-11 10:15:02.000000 express-pascal-voc-tools-0.5.1/voc_tools/unittest/reader_test.py
--rw-rw-rw-   0        0        0     8669 2023-05-11 10:15:02.000000 express-pascal-voc-tools-0.5.1/voc_tools/utils.py
--rw-rw-rw-   0        0        0      164 2023-05-11 08:37:02.000000 express-pascal-voc-tools-0.5.1/voc_tools/visulizer.py
--rw-rw-rw-   0        0        0        2 2023-05-09 13:20:51.000000 express-pascal-voc-tools-0.5.1/voc_tools/writer.py
+drwxrwxrwx   0        0        0        0 2023-05-11 12:02:25.012596 express-pascal-voc-tools-0.6.1/
+-rw-rw-rw-   0        0        0    35823 2023-05-09 09:49:08.000000 express-pascal-voc-tools-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0     4391 2023-05-11 12:02:25.007587 express-pascal-voc-tools-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3907 2023-05-11 06:57:01.000000 express-pascal-voc-tools-0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 12:02:24.958784 express-pascal-voc-tools-0.6.1/express_pascal_voc_tools.egg-info/
+-rw-rw-rw-   0        0        0     4391 2023-05-11 12:02:24.000000 express-pascal-voc-tools-0.6.1/express_pascal_voc_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-05-11 12:02:24.000000 express-pascal-voc-tools-0.6.1/express_pascal_voc_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 12:02:24.000000 express-pascal-voc-tools-0.6.1/express_pascal_voc_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-11 12:02:24.000000 express-pascal-voc-tools-0.6.1/express_pascal_voc_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 12:02:24.000000 express-pascal-voc-tools-0.6.1/express_pascal_voc_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 12:02:25.013587 express-pascal-voc-tools-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      959 2023-05-11 12:00:26.000000 express-pascal-voc-tools-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 12:02:24.991330 express-pascal-voc-tools-0.6.1/voc_tools/
+-rw-rw-rw-   0        0        0        0 2023-05-09 10:14:59.000000 express-pascal-voc-tools-0.6.1/voc_tools/__init__.py
+-rw-rw-rw-   0        0        0      102 2023-05-11 08:12:31.000000 express-pascal-voc-tools-0.6.1/voc_tools/constants.py
+-rw-rw-rw-   0        0        0     4733 2023-05-11 12:00:26.000000 express-pascal-voc-tools-0.6.1/voc_tools/reader.py
+drwxrwxrwx   0        0        0        0 2023-05-11 12:02:25.000338 express-pascal-voc-tools-0.6.1/voc_tools/unittest/
+-rw-rw-rw-   0        0        0        0 2023-05-09 12:15:29.000000 express-pascal-voc-tools-0.6.1/voc_tools/unittest/__init__.py
+-rw-rw-rw-   0        0        0     3126 2023-05-11 12:01:39.000000 express-pascal-voc-tools-0.6.1/voc_tools/unittest/reader_test.py
+-rw-rw-rw-   0        0        0     8750 2023-05-11 12:01:20.000000 express-pascal-voc-tools-0.6.1/voc_tools/utils.py
+-rw-rw-rw-   0        0        0      164 2023-05-11 08:37:02.000000 express-pascal-voc-tools-0.6.1/voc_tools/visulizer.py
+-rw-rw-rw-   0        0        0        2 2023-05-09 13:20:51.000000 express-pascal-voc-tools-0.6.1/voc_tools/writer.py
```

### Comparing `express-pascal-voc-tools-0.5.1/LICENSE` & `express-pascal-voc-tools-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `express-pascal-voc-tools-0.5.1/PKG-INFO` & `express-pascal-voc-tools-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: express-pascal-voc-tools
-Version: 0.5.1
+Version: 0.6.1
 Summary: A tool for creating, reading and visualizing Pascal VOC annotations
 Author: Soumen Sardar
 Author-email: soumensardarintmain@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `express-pascal-voc-tools-0.5.1/README.md` & `express-pascal-voc-tools-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `express-pascal-voc-tools-0.5.1/express_pascal_voc_tools.egg-info/PKG-INFO` & `express-pascal-voc-tools-0.6.1/express_pascal_voc_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: express-pascal-voc-tools
-Version: 0.5.1
+Version: 0.6.1
 Summary: A tool for creating, reading and visualizing Pascal VOC annotations
 Author: Soumen Sardar
 Author-email: soumensardarintmain@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `express-pascal-voc-tools-0.5.1/setup.py` & `express-pascal-voc-tools-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,10 +18,10 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=['lxml', 'numpy', 'opencv-python'],
     version_config=True,
-    version="0.5.1"
+    version="0.6.1"
     # setup_requires=["setuptools-git-versioning"]
 )
```

### Comparing `express-pascal-voc-tools-0.5.1/voc_tools/reader.py` & `express-pascal-voc-tools-0.6.1/voc_tools/reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,21 +83,24 @@
     for file_item in os.listdir(str(annotations_dir)):
         if fullpath:
             yield str(annotations_dir / file_item)
         else:
             yield (annotations_dir / file_item).name
 
 
-def from_dir(dir_path: str):
+def from_dir(dir_path: str, bulk=True):
     """
     Generate a list of Annotation object per file form a given PASCAL VOC directory
     """
     for xml_file in list_dir(dir_path):
-        for annotation in from_xml(xml_file):
-            yield annotation
+        if bulk:
+            yield list(from_xml(xml_file))
+        else:
+            for annotation in from_xml(xml_file):
+                yield annotation
 
 
 def caption_from_file(file_path: str, empty_placeholder="NULL"):
     """
     Generate a list of captions object per file form a given text file path directory
     """
     filename = pathlib.Path(file_path).name
@@ -110,14 +113,17 @@
                 yield caption
             if no_caption:
                 yield Caption(filename, empty_placeholder)
     except Exception as e:
         yield Caption(filename, "ERROR:{}".format(e))
 
 
-def caption_from_dir(dir_path: str):
+def caption_from_dir(dir_path: str, bulk=True):
     """
     Generate a list of captions object per file form a given directory
     """
     for file in list_dir(dir_path, dir_flag=VOC_CAPTIONS):
-        for caption in caption_from_file(file):
-            yield caption
+        if bulk:
+            yield list(caption_from_file(file))
+        else:
+            for caption in caption_from_file(file):
+                yield caption
```

### Comparing `express-pascal-voc-tools-0.5.1/voc_tools/unittest/reader_test.py` & `express-pascal-voc-tools-0.6.1/voc_tools/unittest/reader_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         "P00004.jpg,83,73,133,425,108.0,249.0,knife",
         "P00004.jpg,1,162,343,318,172.0,240.0,knife",
 
         for anno in voc_reader.from_file(r"sixray_data\train\JPEGImages\P00002.jpeg"):
             print(str(anno))
         for anno in voc_reader.from_file(r"sixray_data\train\Annotations\P00002.xml"):
             print(anno.csv())
-        for anno in voc_reader.from_dir(str(dataset_path / "train")):
+        for anno in voc_reader.from_dir(str(dataset_path / "train"), bulk=False):
             print(anno.csv())
         self.assertEqual("file,xmin,ymin,xmax,ymax,center_x,center_y,class_name", Annotation.csv_header())
 
         my_voc = VOCDataset(str(dataset_path))
         my_voc.train.load()
         my_voc.train.unload()
         my_voc.train.to_csv(str(dataset_path / "train.csv"))
@@ -53,10 +53,14 @@
         voc_caption_data.train.caption.to_csv(str(dataset_path / "captions.csv"))
         jpg = from_jpeg(r"sixray_data\train\JPEGImages\P00002.jpg")
         shape1 = jpg.image.shape
         shape2 = (482, 801, 3)
         self.assertEqual(shape1, shape2)
         # see_jpeg(r"sixray_data\train\JPEGImages\P00002.jpg")
 
+        # path = r"C:\Users\--\OneDrive - -- Group\Documents\Projects\Dataset\Sixray_easy"
+        # VOCDataset(path).train.to_csv("sixray_train.csv")
+        # VOCDataset(path).test.to_csv("sixray_test.csv")
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `express-pascal-voc-tools-0.5.1/voc_tools/utils.py` & `express-pascal-voc-tools-0.6.1/voc_tools/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,31 +172,31 @@
         ...
 
 
 class CaptionDataset(ABCDataset):
     def __init__(self, dataset_path):
         super().__init__(dataset_path)
 
-    def fetch(self):
+    def fetch(self, bulk=True):
         """
         Generate Caption object
         """
         from voc_tools.reader import caption_from_dir
 
-        for caption in caption_from_dir(self.dataset_path):
+        for caption in caption_from_dir(self.dataset_path, bulk=bulk):
             yield caption
 
     def to_csv(self, path_to_csv, write_mode="w"):
         """
         Generate csv file for given VOC dataset
         """
         from voc_tools.reader import caption_from_dir
         with open(path_to_csv, write_mode) as csv_fp:
             csv_fp.write("{}\n".format(Caption.csv_header()))
-            for caption in caption_from_dir(self.dataset_path):
+            for caption in caption_from_dir(self.dataset_path, bulk=False):
                 csv_fp.write("{}\n".format(caption.csv()))
         return self
 
 
 class Dataset(ABCDataset):
     def __init__(self, dataset_path, caption_support=False):
         super().__init__(dataset_path)
@@ -207,27 +207,27 @@
         self.loaded = False
         if caption_support:
             self.caption = CaptionDataset(dataset_path)
 
     def load(self):
         if not self.loaded:
             from voc_tools.reader import from_dir
-            self.meta = np.array([anno.raw() for anno in from_dir(self.dataset_path)], dtype='object')
+            self.meta = np.array([anno.raw() for anno in from_dir(self.dataset_path, bulk=False)], dtype='object')
             self.loaded = True
         return self
 
     def unload(self):
         del self.meta
         self.meta = np.array([], dtype='object')
         self.loaded = False
         return self
 
-    def fetch(self):
+    def fetch(self, bulk=True):
         from voc_tools.reader import from_dir
-        for anno in from_dir(self.dataset_path):
+        for anno in from_dir(self.dataset_path, bulk=False):
             yield anno, self.get_image(anno.filename)
 
     def class_names(self):
         if not self.loaded:
             self.load()
         class_name_idx = Annotation.raw_attributes().index('class_name')
         return tuple(set(self.meta[:, class_name_idx]))
@@ -246,15 +246,15 @@
         """
         Generate csv file for given VOC dataset
         """
         from voc_tools.reader import from_dir
         with open(path_to_csv, write_mode) as csv_fp:
             csv_fp.write("{}".format(Annotation.csv_header()))
             csv_fp.write("{}\n".format(JPEG.csv_header().replace("file", "")))
-            for anno in from_dir(self.dataset_path):
+            for anno in from_dir(self.dataset_path, bulk=False):
                 csv_fp.write("{},".format(anno.csv()))
                 csv_fp.write(",".join(self.get_image_meta(anno.filename)))
                 csv_fp.write("\n")
         return self
 
 
 class TrainDataset(Dataset):
```

