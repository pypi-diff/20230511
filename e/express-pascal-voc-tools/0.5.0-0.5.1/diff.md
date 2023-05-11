# Comparing `tmp/express-pascal-voc-tools-0.5.0.tar.gz` & `tmp/express-pascal-voc-tools-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "express-pascal-voc-tools-0.5.0.tar", last modified: Thu May 11 06:59:56 2023, max compression
+gzip compressed data, was "express-pascal-voc-tools-0.5.1.tar", last modified: Thu May 11 10:16:52 2023, max compression
```

## Comparing `express-pascal-voc-tools-0.5.0.tar` & `express-pascal-voc-tools-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 06:59:56.105770 express-pascal-voc-tools-0.5.0/
--rw-rw-rw-   0        0        0    35823 2023-05-09 09:49:08.000000 express-pascal-voc-tools-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     4391 2023-05-11 06:59:56.101771 express-pascal-voc-tools-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3907 2023-05-11 06:57:01.000000 express-pascal-voc-tools-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 06:59:56.061217 express-pascal-voc-tools-0.5.0/express_pascal_voc_tools.egg-info/
--rw-rw-rw-   0        0        0     4391 2023-05-11 06:59:55.000000 express-pascal-voc-tools-0.5.0/express_pascal_voc_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-05-11 06:59:55.000000 express-pascal-voc-tools-0.5.0/express_pascal_voc_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 06:59:55.000000 express-pascal-voc-tools-0.5.0/express_pascal_voc_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-11 06:59:55.000000 express-pascal-voc-tools-0.5.0/express_pascal_voc_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-11 06:59:55.000000 express-pascal-voc-tools-0.5.0/express_pascal_voc_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 06:59:56.105770 express-pascal-voc-tools-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      942 2023-05-11 06:59:24.000000 express-pascal-voc-tools-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 06:59:56.085772 express-pascal-voc-tools-0.5.0/voc_tools/
--rw-rw-rw-   0        0        0        0 2023-05-09 10:14:59.000000 express-pascal-voc-tools-0.5.0/voc_tools/__init__.py
--rw-rw-rw-   0        0        0     4472 2023-05-10 10:14:01.000000 express-pascal-voc-tools-0.5.0/voc_tools/reader.py
-drwxrwxrwx   0        0        0        0 2023-05-11 06:59:56.094771 express-pascal-voc-tools-0.5.0/voc_tools/unittest/
--rw-rw-rw-   0        0        0        0 2023-05-09 12:15:29.000000 express-pascal-voc-tools-0.5.0/voc_tools/unittest/__init__.py
--rw-rw-rw-   0        0        0     2415 2023-05-11 06:53:49.000000 express-pascal-voc-tools-0.5.0/voc_tools/unittest/reader_test.py
--rw-rw-rw-   0        0        0     6207 2023-05-11 06:51:54.000000 express-pascal-voc-tools-0.5.0/voc_tools/utils.py
--rw-rw-rw-   0        0        0        0 2023-05-09 10:19:19.000000 express-pascal-voc-tools-0.5.0/voc_tools/visulizer.py
--rw-rw-rw-   0        0        0        2 2023-05-09 13:20:51.000000 express-pascal-voc-tools-0.5.0/voc_tools/writer.py
+drwxrwxrwx   0        0        0        0 2023-05-11 10:16:52.191170 express-pascal-voc-tools-0.5.1/
+-rw-rw-rw-   0        0        0    35823 2023-05-09 09:49:08.000000 express-pascal-voc-tools-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0     4391 2023-05-11 10:16:52.187016 express-pascal-voc-tools-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3907 2023-05-11 06:57:01.000000 express-pascal-voc-tools-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 10:16:52.139206 express-pascal-voc-tools-0.5.1/express_pascal_voc_tools.egg-info/
+-rw-rw-rw-   0        0        0     4391 2023-05-11 10:16:51.000000 express-pascal-voc-tools-0.5.1/express_pascal_voc_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-05-11 10:16:51.000000 express-pascal-voc-tools-0.5.1/express_pascal_voc_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 10:16:51.000000 express-pascal-voc-tools-0.5.1/express_pascal_voc_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-11 10:16:51.000000 express-pascal-voc-tools-0.5.1/express_pascal_voc_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 10:16:51.000000 express-pascal-voc-tools-0.5.1/express_pascal_voc_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 10:16:52.191170 express-pascal-voc-tools-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      959 2023-05-11 08:00:59.000000 express-pascal-voc-tools-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 10:16:52.172016 express-pascal-voc-tools-0.5.1/voc_tools/
+-rw-rw-rw-   0        0        0        0 2023-05-09 10:14:59.000000 express-pascal-voc-tools-0.5.1/voc_tools/__init__.py
+-rw-rw-rw-   0        0        0      102 2023-05-11 08:12:31.000000 express-pascal-voc-tools-0.5.1/voc_tools/constants.py
+-rw-rw-rw-   0        0        0     4536 2023-05-11 09:32:37.000000 express-pascal-voc-tools-0.5.1/voc_tools/reader.py
+drwxrwxrwx   0        0        0        0 2023-05-11 10:16:52.180017 express-pascal-voc-tools-0.5.1/voc_tools/unittest/
+-rw-rw-rw-   0        0        0        0 2023-05-09 12:15:29.000000 express-pascal-voc-tools-0.5.1/voc_tools/unittest/__init__.py
+-rw-rw-rw-   0        0        0     2900 2023-05-11 10:15:02.000000 express-pascal-voc-tools-0.5.1/voc_tools/unittest/reader_test.py
+-rw-rw-rw-   0        0        0     8669 2023-05-11 10:15:02.000000 express-pascal-voc-tools-0.5.1/voc_tools/utils.py
+-rw-rw-rw-   0        0        0      164 2023-05-11 08:37:02.000000 express-pascal-voc-tools-0.5.1/voc_tools/visulizer.py
+-rw-rw-rw-   0        0        0        2 2023-05-09 13:20:51.000000 express-pascal-voc-tools-0.5.1/voc_tools/writer.py
```

### Comparing `express-pascal-voc-tools-0.5.0/LICENSE` & `express-pascal-voc-tools-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `express-pascal-voc-tools-0.5.0/PKG-INFO` & `express-pascal-voc-tools-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: express-pascal-voc-tools
-Version: 0.5.0
+Version: 0.5.1
 Summary: A tool for creating, reading and visualizing Pascal VOC annotations
 Author: Soumen Sardar
 Author-email: soumensardarintmain@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `express-pascal-voc-tools-0.5.0/README.md` & `express-pascal-voc-tools-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `express-pascal-voc-tools-0.5.0/express_pascal_voc_tools.egg-info/PKG-INFO` & `express-pascal-voc-tools-0.5.1/express_pascal_voc_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: express-pascal-voc-tools
-Version: 0.5.0
+Version: 0.5.1
 Summary: A tool for creating, reading and visualizing Pascal VOC annotations
 Author: Soumen Sardar
 Author-email: soumensardarintmain@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `express-pascal-voc-tools-0.5.0/setup.py` & `express-pascal-voc-tools-0.5.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,12 +16,12 @@
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-    install_requires=['lxml', 'numpy'],
+    install_requires=['lxml', 'numpy', 'opencv-python'],
     version_config=True,
-    version="0.5.0"
+    version="0.5.1"
     # setup_requires=["setuptools-git-versioning"]
 )
```

### Comparing `express-pascal-voc-tools-0.5.0/voc_tools/reader.py` & `express-pascal-voc-tools-0.5.1/voc_tools/reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import os
 import pathlib
 import xml.etree.ElementTree as ET
 
+from voc_tools.constants import VOC_XMLS, VOC_IMAGES, VOC_CAPTIONS
 from voc_tools.utils import Annotation, Caption
 
 
 def from_file(file: str):
     """
     Generate a list of Annotation objects for a given image or xml of a PASCAL VOC dataset.
     It also supports captions .txt files
     """
     if file.endswith(".xml"):
         return from_xml(file)
     elif file.endswith(".txt"):
         return caption_from_file(file)
-    elif file.endswith(".jpeg"):
+    elif file.endswith(".jpeg") or file.endswith(".jpg"):
         return from_image(file)
     else:
-        raise ValueError("Unsupported file format.")
+        raise ValueError("Unsupported file format")
 
 
 def from_image(image_file: str):
     """
     Generate a list of Annotation objects for a given image of a PASCAL VOC dataset
     """
     image_file = pathlib.Path(image_file)
     parent_path = image_file.parents[1] / "Annotations"
-    file_name = image_file.name.replace(".jpeg", ".xml")
+    file_name = image_file.name.replace(".jpeg", ".xml").replace(".jpg", ".xml")
     xml_file = str(parent_path / file_name)
     return from_xml(xml_file)
 
 
 def from_xml(xml_file: str, empty_placeholder="NULL"):
     """
     Generate a list of Annotation objects from a given VOC XML file
@@ -57,19 +58,14 @@
             yield single_annotation
         if no_threat:
             yield Annotation(filename, 0, 0, 0, 0, 0, 0, empty_placeholder)
     except Exception as e:
         yield Annotation(filename, 0, 0, 0, 0, 0, 0, "ERROR:{}".format(e))
 
 
-VOC_IMAGES = 1
-VOC_XMLS = 2
-VOC_CAPTIONS = 3
-
-
 def list_dir(dir_path: str, dir_flag=VOC_XMLS, images=False, fullpath=True):
     """
     Generate a list of XML files form a given PASCAL VOC directory
     Args:
         dir_path: A path to VOC dataset
         dir_flag: A flag which specify the subdirectory to list. Any typical
                     Pascal VOC dataset must contain Annotations, JPEGImages and text[optionsl] directories.
```

### Comparing `express-pascal-voc-tools-0.5.0/voc_tools/unittest/reader_test.py` & `express-pascal-voc-tools-0.5.1/voc_tools/unittest/reader_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pathlib
 import unittest
 
 from voc_tools import reader as voc_reader
 from voc_tools.utils import Annotation, VOCDataset
+from voc_tools.visulizer import from_jpeg, see_jpeg
 
 
 class MyTestCase(unittest.TestCase):
     def test_something(self):
         dataset_path = pathlib.Path(r"sixray_data")
 
         self.assertEqual(list(voc_reader.list_dir(str(dataset_path / "train"), fullpath=False)),
@@ -30,21 +31,32 @@
             print(str(anno))
         for anno in voc_reader.from_file(r"sixray_data\train\Annotations\P00002.xml"):
             print(anno.csv())
         for anno in voc_reader.from_dir(str(dataset_path / "train")):
             print(anno.csv())
         self.assertEqual("file,xmin,ymin,xmax,ymax,center_x,center_y,class_name", Annotation.csv_header())
 
-        print(VOCDataset(str(dataset_path)).train.load().to_csv(str(dataset_path / "train.csv")).class_names())
+        my_voc = VOCDataset(str(dataset_path))
+        my_voc.train.load()
+        my_voc.train.unload()
+        my_voc.train.to_csv(str(dataset_path / "train.csv"))
+        classes1 = my_voc.train.class_names()
+        classes2 = "knife",
+        self.assertEqual(classes2, classes1)
 
         voc_caption_data = VOCDataset(str(dataset_path), caption_support=True)
         for caption in voc_caption_data.train.caption.fetch():
             print(caption)
 
-        for anno in voc_caption_data.train.fetch():
-            print(anno)
+        for anno, jpeg in voc_caption_data.train.fetch():
+            print(anno, jpeg)
 
         voc_caption_data.train.caption.to_csv(str(dataset_path / "captions.csv"))
+        jpg = from_jpeg(r"sixray_data\train\JPEGImages\P00002.jpg")
+        shape1 = jpg.image.shape
+        shape2 = (482, 801, 3)
+        self.assertEqual(shape1, shape2)
+        # see_jpeg(r"sixray_data\train\JPEGImages\P00002.jpg")
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `express-pascal-voc-tools-0.5.0/voc_tools/utils.py` & `express-pascal-voc-tools-0.5.1/voc_tools/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,38 @@
 import os
+import pathlib
 from abc import ABC, abstractmethod
 
+import cv2
 import numpy as np
 
+from voc_tools.constants import VOC_IMAGES, VOC_CAPTIONS, VOC_XMLS
+
+
+def path_convert(file: str, converter_flag: int):
+    """
+    Convert any file path to a required file path
+    :param file: A path to xml, jpeg or txt file
+    :param converter_flag:
+    :return: Converted path
+    """
+    assert file.endswith(".xml") or file.endswith(".txt") or file.endswith(".jpeg") or file.endswith(".jpg"), (
+        "Unsupported file format")
+    assert converter_flag in [VOC_IMAGES, VOC_CAPTIONS, VOC_XMLS], "Unsupported converter_flag"
+    file = pathlib.Path(file)
+    filename = file.name
+    parent_path = file.parents[1]
+    if converter_flag == VOC_IMAGES:
+        path = parent_path / "JPEGImages" / filename
+    if converter_flag == VOC_XMLS:
+        path = parent_path / "Annotations" / filename
+    if converter_flag == VOC_CAPTIONS:
+        path = parent_path / "text" / filename
+    return str(path)
+
 
 # ################################################
 # Python classes to hold annotation and captions #
 # ################################################
 class Atomic:
     def __str__(self):
         s = ""
@@ -31,14 +57,41 @@
     @classmethod
     @abstractmethod
     def raw_attributes(cls):
         """Return raw tuple of strings(to be used as key per values). A single method instance is required per class"""
         ...
 
 
+class JPEG(Atomic):
+
+    def raw(self):
+        return self._filename, *self._cv_image.shape
+
+    @classmethod
+    def raw_attributes(cls):
+        return "file", "height", "width", "channels"
+
+    def __init__(self, filename):
+        filename = path_convert(filename, VOC_IMAGES)
+        self._filename = pathlib.Path(filename).name
+        self._cv_image = cv2.imread(filename)
+
+    @property
+    def filename(self):
+        return self._filename
+
+    @property
+    def image(self):
+        return self._cv_image
+
+    def see(self):
+        cv2.imshow(self.filename, self._cv_image)
+        cv2.waitKey(-1)
+
+
 class Annotation(Atomic):
     def __init__(self, filename, xmin, ymin, xmax, ymax, center_x, center_y, class_name):
         self._xmin, self._ymin, self._xmax, self._ymax, self._center_x, self._center_y, self._class_name = (
             xmin, ymin, xmax,
             ymax, center_x,
             center_y,
             class_name)
@@ -146,45 +199,65 @@
 
 class Dataset(ABCDataset):
     def __init__(self, dataset_path, caption_support=False):
         super().__init__(dataset_path)
         self.dataset_path = dataset_path
         self.caption_support = caption_support
         self.meta = np.array([], dtype='object')
+        self.image_cache: JPEG = None
+        self.loaded = False
         if caption_support:
             self.caption = CaptionDataset(dataset_path)
 
     def load(self):
-        from voc_tools.reader import from_dir
-        self.meta = np.array([anno.raw() for anno in from_dir(self.dataset_path)], dtype='object')
+        if not self.loaded:
+            from voc_tools.reader import from_dir
+            self.meta = np.array([anno.raw() for anno in from_dir(self.dataset_path)], dtype='object')
+            self.loaded = True
         return self
 
     def unload(self):
         del self.meta
         self.meta = np.array([], dtype='object')
+        self.loaded = False
         return self
 
     def fetch(self):
         from voc_tools.reader import from_dir
         for anno in from_dir(self.dataset_path):
-            yield anno
+            yield anno, self.get_image(anno.filename)
 
     def class_names(self):
+        if not self.loaded:
+            self.load()
         class_name_idx = Annotation.raw_attributes().index('class_name')
-        return set(self.meta[:, class_name_idx])
+        return tuple(set(self.meta[:, class_name_idx]))
+
+    def get_image(self, filename):
+        return JPEG(os.path.join(self.dataset_path, "JPEGImages", filename))
+
+    def get_image_meta(self, filename):
+        if self.image_cache is None or filename != self.image_cache.filename:
+            # save the image
+            self.image_cache = self.get_image(filename)
+            # if a newer appear, re
+        return self.image_cache.csv().split(",")[1:]
 
     def to_csv(self, path_to_csv, write_mode="w"):
         """
         Generate csv file for given VOC dataset
         """
         from voc_tools.reader import from_dir
         with open(path_to_csv, write_mode) as csv_fp:
-            csv_fp.write("{}\n".format(Annotation.csv_header()))
+            csv_fp.write("{}".format(Annotation.csv_header()))
+            csv_fp.write("{}\n".format(JPEG.csv_header().replace("file", "")))
             for anno in from_dir(self.dataset_path):
-                csv_fp.write("{}\n".format(anno.csv()))
+                csv_fp.write("{},".format(anno.csv()))
+                csv_fp.write(",".join(self.get_image_meta(anno.filename)))
+                csv_fp.write("\n")
         return self
 
 
 class TrainDataset(Dataset):
     def __init__(self, dataset_path, caption_support=False):
         super().__init__(dataset_path, caption_support=caption_support)
```

