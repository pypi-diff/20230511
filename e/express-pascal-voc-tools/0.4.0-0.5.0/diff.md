# Comparing `tmp/express-pascal-voc-tools-0.4.0.tar.gz` & `tmp/express-pascal-voc-tools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "express-pascal-voc-tools-0.4.0.tar", last modified: Wed May 10 11:21:05 2023, max compression
+gzip compressed data, was "express-pascal-voc-tools-0.5.0.tar", last modified: Thu May 11 06:59:56 2023, max compression
```

## Comparing `express-pascal-voc-tools-0.4.0.tar` & `express-pascal-voc-tools-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 11:21:05.327085 express-pascal-voc-tools-0.4.0/
--rw-rw-rw-   0        0        0    35823 2023-05-09 09:49:08.000000 express-pascal-voc-tools-0.4.0/LICENSE
--rw-rw-rw-   0        0        0      897 2023-05-10 11:21:05.313229 express-pascal-voc-tools-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      413 2023-05-09 17:39:47.000000 express-pascal-voc-tools-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 11:21:05.161575 express-pascal-voc-tools-0.4.0/express_pascal_voc_tools.egg-info/
--rw-rw-rw-   0        0        0      897 2023-05-10 11:21:03.000000 express-pascal-voc-tools-0.4.0/express_pascal_voc_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-05-10 11:21:04.000000 express-pascal-voc-tools-0.4.0/express_pascal_voc_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 11:21:03.000000 express-pascal-voc-tools-0.4.0/express_pascal_voc_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-10 11:21:03.000000 express-pascal-voc-tools-0.4.0/express_pascal_voc_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-10 11:21:03.000000 express-pascal-voc-tools-0.4.0/express_pascal_voc_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 11:21:05.327762 express-pascal-voc-tools-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      942 2023-05-10 10:18:57.000000 express-pascal-voc-tools-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:21:05.245296 express-pascal-voc-tools-0.4.0/voc_tools/
--rw-rw-rw-   0        0        0        0 2023-05-09 10:14:59.000000 express-pascal-voc-tools-0.4.0/voc_tools/__init__.py
--rw-rw-rw-   0        0        0     4472 2023-05-10 10:14:01.000000 express-pascal-voc-tools-0.4.0/voc_tools/reader.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:21:05.287102 express-pascal-voc-tools-0.4.0/voc_tools/unittest/
--rw-rw-rw-   0        0        0        0 2023-05-09 12:15:29.000000 express-pascal-voc-tools-0.4.0/voc_tools/unittest/__init__.py
--rw-rw-rw-   0        0        0     2339 2023-05-10 09:45:35.000000 express-pascal-voc-tools-0.4.0/voc_tools/unittest/reader_test.py
--rw-rw-rw-   0        0        0     6062 2023-05-10 09:43:53.000000 express-pascal-voc-tools-0.4.0/voc_tools/utils.py
--rw-rw-rw-   0        0        0        0 2023-05-09 10:19:19.000000 express-pascal-voc-tools-0.4.0/voc_tools/visulizer.py
--rw-rw-rw-   0        0        0        2 2023-05-09 13:20:51.000000 express-pascal-voc-tools-0.4.0/voc_tools/writer.py
+drwxrwxrwx   0        0        0        0 2023-05-11 06:59:56.105770 express-pascal-voc-tools-0.5.0/
+-rw-rw-rw-   0        0        0    35823 2023-05-09 09:49:08.000000 express-pascal-voc-tools-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     4391 2023-05-11 06:59:56.101771 express-pascal-voc-tools-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3907 2023-05-11 06:57:01.000000 express-pascal-voc-tools-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 06:59:56.061217 express-pascal-voc-tools-0.5.0/express_pascal_voc_tools.egg-info/
+-rw-rw-rw-   0        0        0     4391 2023-05-11 06:59:55.000000 express-pascal-voc-tools-0.5.0/express_pascal_voc_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-05-11 06:59:55.000000 express-pascal-voc-tools-0.5.0/express_pascal_voc_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 06:59:55.000000 express-pascal-voc-tools-0.5.0/express_pascal_voc_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-11 06:59:55.000000 express-pascal-voc-tools-0.5.0/express_pascal_voc_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 06:59:55.000000 express-pascal-voc-tools-0.5.0/express_pascal_voc_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 06:59:56.105770 express-pascal-voc-tools-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      942 2023-05-11 06:59:24.000000 express-pascal-voc-tools-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 06:59:56.085772 express-pascal-voc-tools-0.5.0/voc_tools/
+-rw-rw-rw-   0        0        0        0 2023-05-09 10:14:59.000000 express-pascal-voc-tools-0.5.0/voc_tools/__init__.py
+-rw-rw-rw-   0        0        0     4472 2023-05-10 10:14:01.000000 express-pascal-voc-tools-0.5.0/voc_tools/reader.py
+drwxrwxrwx   0        0        0        0 2023-05-11 06:59:56.094771 express-pascal-voc-tools-0.5.0/voc_tools/unittest/
+-rw-rw-rw-   0        0        0        0 2023-05-09 12:15:29.000000 express-pascal-voc-tools-0.5.0/voc_tools/unittest/__init__.py
+-rw-rw-rw-   0        0        0     2415 2023-05-11 06:53:49.000000 express-pascal-voc-tools-0.5.0/voc_tools/unittest/reader_test.py
+-rw-rw-rw-   0        0        0     6207 2023-05-11 06:51:54.000000 express-pascal-voc-tools-0.5.0/voc_tools/utils.py
+-rw-rw-rw-   0        0        0        0 2023-05-09 10:19:19.000000 express-pascal-voc-tools-0.5.0/voc_tools/visulizer.py
+-rw-rw-rw-   0        0        0        2 2023-05-09 13:20:51.000000 express-pascal-voc-tools-0.5.0/voc_tools/writer.py
```

### Comparing `express-pascal-voc-tools-0.4.0/LICENSE` & `express-pascal-voc-tools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `express-pascal-voc-tools-0.4.0/setup.py` & `express-pascal-voc-tools-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,10 +18,10 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=['lxml', 'numpy'],
     version_config=True,
-    version="0.4.0"
+    version="0.5.0"
     # setup_requires=["setuptools-git-versioning"]
 )
```

### Comparing `express-pascal-voc-tools-0.4.0/voc_tools/reader.py` & `express-pascal-voc-tools-0.5.0/voc_tools/reader.py`

 * *Files identical despite different names*

### Comparing `express-pascal-voc-tools-0.4.0/voc_tools/unittest/reader_test.py` & `express-pascal-voc-tools-0.5.0/voc_tools/unittest/reader_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,13 +34,17 @@
             print(anno.csv())
         self.assertEqual("file,xmin,ymin,xmax,ymax,center_x,center_y,class_name", Annotation.csv_header())
 
         print(VOCDataset(str(dataset_path)).train.load().to_csv(str(dataset_path / "train.csv")).class_names())
 
         voc_caption_data = VOCDataset(str(dataset_path), caption_support=True)
         for caption in voc_caption_data.train.caption.fetch():
-            print(caption.csv())
+            print(caption)
+
+        for anno in voc_caption_data.train.fetch():
+            print(anno)
+
         voc_caption_data.train.caption.to_csv(str(dataset_path / "captions.csv"))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `express-pascal-voc-tools-0.4.0/voc_tools/utils.py` & `express-pascal-voc-tools-0.5.0/voc_tools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,19 @@
         return self
 
     def unload(self):
         del self.meta
         self.meta = np.array([], dtype='object')
         return self
 
+    def fetch(self):
+        from voc_tools.reader import from_dir
+        for anno in from_dir(self.dataset_path):
+            yield anno
+
     def class_names(self):
         class_name_idx = Annotation.raw_attributes().index('class_name')
         return set(self.meta[:, class_name_idx])
 
     def to_csv(self, path_to_csv, write_mode="w"):
         """
         Generate csv file for given VOC dataset
```

