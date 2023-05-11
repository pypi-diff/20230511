# Comparing `tmp/express-pascal-voc-tools-0.6.1.tar.gz` & `tmp/express-pascal-voc-tools-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "express-pascal-voc-tools-0.6.1.tar", last modified: Thu May 11 12:02:25 2023, max compression
+gzip compressed data, was "express-pascal-voc-tools-0.6.2.tar", last modified: Thu May 11 13:02:11 2023, max compression
```

## Comparing `express-pascal-voc-tools-0.6.1.tar` & `express-pascal-voc-tools-0.6.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 12:02:25.012596 express-pascal-voc-tools-0.6.1/
--rw-rw-rw-   0        0        0    35823 2023-05-09 09:49:08.000000 express-pascal-voc-tools-0.6.1/LICENSE
--rw-rw-rw-   0        0        0     4391 2023-05-11 12:02:25.007587 express-pascal-voc-tools-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     3907 2023-05-11 06:57:01.000000 express-pascal-voc-tools-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 12:02:24.958784 express-pascal-voc-tools-0.6.1/express_pascal_voc_tools.egg-info/
--rw-rw-rw-   0        0        0     4391 2023-05-11 12:02:24.000000 express-pascal-voc-tools-0.6.1/express_pascal_voc_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-05-11 12:02:24.000000 express-pascal-voc-tools-0.6.1/express_pascal_voc_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 12:02:24.000000 express-pascal-voc-tools-0.6.1/express_pascal_voc_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-11 12:02:24.000000 express-pascal-voc-tools-0.6.1/express_pascal_voc_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-11 12:02:24.000000 express-pascal-voc-tools-0.6.1/express_pascal_voc_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 12:02:25.013587 express-pascal-voc-tools-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0      959 2023-05-11 12:00:26.000000 express-pascal-voc-tools-0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 12:02:24.991330 express-pascal-voc-tools-0.6.1/voc_tools/
--rw-rw-rw-   0        0        0        0 2023-05-09 10:14:59.000000 express-pascal-voc-tools-0.6.1/voc_tools/__init__.py
--rw-rw-rw-   0        0        0      102 2023-05-11 08:12:31.000000 express-pascal-voc-tools-0.6.1/voc_tools/constants.py
--rw-rw-rw-   0        0        0     4733 2023-05-11 12:00:26.000000 express-pascal-voc-tools-0.6.1/voc_tools/reader.py
-drwxrwxrwx   0        0        0        0 2023-05-11 12:02:25.000338 express-pascal-voc-tools-0.6.1/voc_tools/unittest/
--rw-rw-rw-   0        0        0        0 2023-05-09 12:15:29.000000 express-pascal-voc-tools-0.6.1/voc_tools/unittest/__init__.py
--rw-rw-rw-   0        0        0     3126 2023-05-11 12:01:39.000000 express-pascal-voc-tools-0.6.1/voc_tools/unittest/reader_test.py
--rw-rw-rw-   0        0        0     8750 2023-05-11 12:01:20.000000 express-pascal-voc-tools-0.6.1/voc_tools/utils.py
--rw-rw-rw-   0        0        0      164 2023-05-11 08:37:02.000000 express-pascal-voc-tools-0.6.1/voc_tools/visulizer.py
--rw-rw-rw-   0        0        0        2 2023-05-09 13:20:51.000000 express-pascal-voc-tools-0.6.1/voc_tools/writer.py
+drwxrwxrwx   0        0        0        0 2023-05-11 13:02:11.557399 express-pascal-voc-tools-0.6.2/
+-rw-rw-rw-   0        0        0    35823 2023-05-09 09:49:08.000000 express-pascal-voc-tools-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0     4900 2023-05-11 13:02:11.553400 express-pascal-voc-tools-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4416 2023-05-11 13:01:05.000000 express-pascal-voc-tools-0.6.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 13:02:11.504953 express-pascal-voc-tools-0.6.2/express_pascal_voc_tools.egg-info/
+-rw-rw-rw-   0        0        0     4900 2023-05-11 13:02:10.000000 express-pascal-voc-tools-0.6.2/express_pascal_voc_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-05-11 13:02:11.000000 express-pascal-voc-tools-0.6.2/express_pascal_voc_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 13:02:10.000000 express-pascal-voc-tools-0.6.2/express_pascal_voc_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-11 13:02:10.000000 express-pascal-voc-tools-0.6.2/express_pascal_voc_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 13:02:10.000000 express-pascal-voc-tools-0.6.2/express_pascal_voc_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 13:02:11.558066 express-pascal-voc-tools-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0      959 2023-05-11 12:55:55.000000 express-pascal-voc-tools-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 13:02:11.538739 express-pascal-voc-tools-0.6.2/voc_tools/
+-rw-rw-rw-   0        0        0        0 2023-05-09 10:14:59.000000 express-pascal-voc-tools-0.6.2/voc_tools/__init__.py
+-rw-rw-rw-   0        0        0      102 2023-05-11 08:12:31.000000 express-pascal-voc-tools-0.6.2/voc_tools/constants.py
+-rw-rw-rw-   0        0        0     4733 2023-05-11 12:00:26.000000 express-pascal-voc-tools-0.6.2/voc_tools/reader.py
+drwxrwxrwx   0        0        0        0 2023-05-11 13:02:11.546739 express-pascal-voc-tools-0.6.2/voc_tools/unittest/
+-rw-rw-rw-   0        0        0        0 2023-05-09 12:15:29.000000 express-pascal-voc-tools-0.6.2/voc_tools/unittest/__init__.py
+-rw-rw-rw-   0        0        0     3126 2023-05-11 12:01:39.000000 express-pascal-voc-tools-0.6.2/voc_tools/unittest/reader_test.py
+-rw-rw-rw-   0        0        0     8858 2023-05-11 12:09:35.000000 express-pascal-voc-tools-0.6.2/voc_tools/utils.py
+-rw-rw-rw-   0        0        0      164 2023-05-11 08:37:02.000000 express-pascal-voc-tools-0.6.2/voc_tools/visulizer.py
+-rw-rw-rw-   0        0        0        2 2023-05-09 13:20:51.000000 express-pascal-voc-tools-0.6.2/voc_tools/writer.py
```

### Comparing `express-pascal-voc-tools-0.6.1/LICENSE` & `express-pascal-voc-tools-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `express-pascal-voc-tools-0.6.1/PKG-INFO` & `express-pascal-voc-tools-0.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: express-pascal-voc-tools
-Version: 0.6.1
+Version: 0.6.2
 Summary: A tool for creating, reading and visualizing Pascal VOC annotations
 Author: Soumen Sardar
 Author-email: soumensardarintmain@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -81,17 +81,20 @@
 from voc_tools.utils import VOCDataset
 
 dataset_path = "/my_dataset"
 
 # initialize a dataset
 my_dataset = VOCDataset(dataset_path)
 
+# fetch annotation bulk
+for annotations, jpeg in my_dataset.train.fetch():
+    print(annotations[0].filename, jpeg.image.shape)
 # fetch annotation
-for anno in my_dataset.train.fetch():
-    print(anno)
+for anno, jpeg in my_dataset.train.fetch(bulk=False):
+    print(anno, jpeg.image.shape)
 
 # parse the annotations into memory for train dataset
 my_dataset.train.load()
 my_dataset.test.load()
 
 # returns a list of class names in train dataset
 my_dataset.train.class_names()
@@ -146,21 +149,36 @@
 
 ```python
 from voc_tools.utils import VOCDataset
 
 dataset_path = "/my_dataset"
 voc_caption_data = VOCDataset(dataset_path, caption_support=True)  # init dataset with caption
 
+# read caption bulk
+for captions in voc_caption_data.train.caption.fetch():
+    print(captions[0].raw())
+
 # read caption one by one
-for caption in voc_caption_data.train.caption.fetch():
+for caption in voc_caption_data.train.caption.fetch(bulk=False):
     print(caption.raw())
 # save captions to a CSV
 voc_caption_data.train.caption.to_csv("train_captions.csv")
 ```
 
+### Visualize
+
+```python
+from voc_tools.visulizer import from_jpeg, see_jpeg
+
+jpeg = from_jpeg(r"sixray_data\train\JPEGImages\P00002.jpg")
+jpeg.see()
+# OR
+see_jpeg(r"sixray_data\train\JPEGImages\P00002.jpg")
+```
+
 # Collaborate
 
 GitHub: [https://github.com/Redcof/pascal_voc_tools.git](https://github.com/Redcof/pascal_voc_tools.git)
 
 **Build and Publish**
 
 1. `python setup.py sdist bdist_wheel`
```

### Comparing `express-pascal-voc-tools-0.6.1/README.md` & `express-pascal-voc-tools-0.6.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -68,17 +68,20 @@
 from voc_tools.utils import VOCDataset
 
 dataset_path = "/my_dataset"
 
 # initialize a dataset
 my_dataset = VOCDataset(dataset_path)
 
+# fetch annotation bulk
+for annotations, jpeg in my_dataset.train.fetch():
+    print(annotations[0].filename, jpeg.image.shape)
 # fetch annotation
-for anno in my_dataset.train.fetch():
-    print(anno)
+for anno, jpeg in my_dataset.train.fetch(bulk=False):
+    print(anno, jpeg.image.shape)
 
 # parse the annotations into memory for train dataset
 my_dataset.train.load()
 my_dataset.test.load()
 
 # returns a list of class names in train dataset
 my_dataset.train.class_names()
@@ -133,21 +136,36 @@
 
 ```python
 from voc_tools.utils import VOCDataset
 
 dataset_path = "/my_dataset"
 voc_caption_data = VOCDataset(dataset_path, caption_support=True)  # init dataset with caption
 
+# read caption bulk
+for captions in voc_caption_data.train.caption.fetch():
+    print(captions[0].raw())
+
 # read caption one by one
-for caption in voc_caption_data.train.caption.fetch():
+for caption in voc_caption_data.train.caption.fetch(bulk=False):
     print(caption.raw())
 # save captions to a CSV
 voc_caption_data.train.caption.to_csv("train_captions.csv")
 ```
 
+### Visualize
+
+```python
+from voc_tools.visulizer import from_jpeg, see_jpeg
+
+jpeg = from_jpeg(r"sixray_data\train\JPEGImages\P00002.jpg")
+jpeg.see()
+# OR
+see_jpeg(r"sixray_data\train\JPEGImages\P00002.jpg")
+```
+
 # Collaborate
 
 GitHub: [https://github.com/Redcof/pascal_voc_tools.git](https://github.com/Redcof/pascal_voc_tools.git)
 
 **Build and Publish**
 
 1. `python setup.py sdist bdist_wheel`
```

### Comparing `express-pascal-voc-tools-0.6.1/express_pascal_voc_tools.egg-info/PKG-INFO` & `express-pascal-voc-tools-0.6.2/express_pascal_voc_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: express-pascal-voc-tools
-Version: 0.6.1
+Version: 0.6.2
 Summary: A tool for creating, reading and visualizing Pascal VOC annotations
 Author: Soumen Sardar
 Author-email: soumensardarintmain@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -81,17 +81,20 @@
 from voc_tools.utils import VOCDataset
 
 dataset_path = "/my_dataset"
 
 # initialize a dataset
 my_dataset = VOCDataset(dataset_path)
 
+# fetch annotation bulk
+for annotations, jpeg in my_dataset.train.fetch():
+    print(annotations[0].filename, jpeg.image.shape)
 # fetch annotation
-for anno in my_dataset.train.fetch():
-    print(anno)
+for anno, jpeg in my_dataset.train.fetch(bulk=False):
+    print(anno, jpeg.image.shape)
 
 # parse the annotations into memory for train dataset
 my_dataset.train.load()
 my_dataset.test.load()
 
 # returns a list of class names in train dataset
 my_dataset.train.class_names()
@@ -146,21 +149,36 @@
 
 ```python
 from voc_tools.utils import VOCDataset
 
 dataset_path = "/my_dataset"
 voc_caption_data = VOCDataset(dataset_path, caption_support=True)  # init dataset with caption
 
+# read caption bulk
+for captions in voc_caption_data.train.caption.fetch():
+    print(captions[0].raw())
+
 # read caption one by one
-for caption in voc_caption_data.train.caption.fetch():
+for caption in voc_caption_data.train.caption.fetch(bulk=False):
     print(caption.raw())
 # save captions to a CSV
 voc_caption_data.train.caption.to_csv("train_captions.csv")
 ```
 
+### Visualize
+
+```python
+from voc_tools.visulizer import from_jpeg, see_jpeg
+
+jpeg = from_jpeg(r"sixray_data\train\JPEGImages\P00002.jpg")
+jpeg.see()
+# OR
+see_jpeg(r"sixray_data\train\JPEGImages\P00002.jpg")
+```
+
 # Collaborate
 
 GitHub: [https://github.com/Redcof/pascal_voc_tools.git](https://github.com/Redcof/pascal_voc_tools.git)
 
 **Build and Publish**
 
 1. `python setup.py sdist bdist_wheel`
```

### Comparing `express-pascal-voc-tools-0.6.1/setup.py` & `express-pascal-voc-tools-0.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,10 +18,10 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=['lxml', 'numpy', 'opencv-python'],
     version_config=True,
-    version="0.6.1"
+    version="0.6.2"
     # setup_requires=["setuptools-git-versioning"]
 )
```

### Comparing `express-pascal-voc-tools-0.6.1/voc_tools/reader.py` & `express-pascal-voc-tools-0.6.2/voc_tools/reader.py`

 * *Files identical despite different names*

### Comparing `express-pascal-voc-tools-0.6.1/voc_tools/unittest/reader_test.py` & `express-pascal-voc-tools-0.6.2/voc_tools/unittest/reader_test.py`

 * *Files identical despite different names*

### Comparing `express-pascal-voc-tools-0.6.1/voc_tools/utils.py` & `express-pascal-voc-tools-0.6.2/voc_tools/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,16 +219,20 @@
         del self.meta
         self.meta = np.array([], dtype='object')
         self.loaded = False
         return self
 
     def fetch(self, bulk=True):
         from voc_tools.reader import from_dir
-        for anno in from_dir(self.dataset_path, bulk=False):
-            yield anno, self.get_image(anno.filename)
+        for anno in from_dir(self.dataset_path, bulk=bulk):
+            if bulk:
+                yield anno, self.get_image(anno[0].filename)
+            else:
+                yield anno, self.get_image(anno.filename)
+
 
     def class_names(self):
         if not self.loaded:
             self.load()
         class_name_idx = Annotation.raw_attributes().index('class_name')
         return tuple(set(self.meta[:, class_name_idx]))
```

