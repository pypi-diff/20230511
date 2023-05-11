# Comparing `tmp/PyNucSeg-0.0.7.tar.gz` & `tmp/PyNucSeg-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNucSeg-0.0.7.tar", last modified: Wed Mar  1 01:35:13 2023, max compression
+gzip compressed data, was "PyNucSeg-0.0.8.tar", last modified: Mon May  8 22:11:38 2023, max compression
```

## Comparing `PyNucSeg-0.0.7.tar` & `PyNucSeg-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-01 01:35:13.097825 PyNucSeg-0.0.7/
--rw-rw-rw-   0        0        0     1527 2023-02-28 22:32:05.000000 PyNucSeg-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      837 2023-03-01 01:35:13.097825 PyNucSeg-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      445 2023-02-28 22:32:05.000000 PyNucSeg-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-03-01 01:35:13.097825 PyNucSeg-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      817 2023-03-01 01:35:07.000000 PyNucSeg-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-01 01:35:13.083644 PyNucSeg-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-03-01 01:35:13.096813 PyNucSeg-0.0.7/src/PyNucSeg.egg-info/
--rw-rw-rw-   0        0        0      837 2023-03-01 01:35:12.000000 PyNucSeg-0.0.7/src/PyNucSeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-03-01 01:35:12.000000 PyNucSeg-0.0.7/src/PyNucSeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-01 01:35:12.000000 PyNucSeg-0.0.7/src/PyNucSeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-03-01 01:35:12.000000 PyNucSeg-0.0.7/src/PyNucSeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-01 01:35:12.000000 PyNucSeg-0.0.7/src/PyNucSeg.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-01 01:35:13.097825 PyNucSeg-0.0.7/src/pynucseg/
--rw-rw-rw-   0        0        0       83 2023-03-01 01:34:20.000000 PyNucSeg-0.0.7/src/pynucseg/__init__.py
--rw-rw-rw-   0        0        0    15729 2023-02-28 21:54:55.000000 PyNucSeg-0.0.7/src/pynucseg/base.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:11:38.766075 PyNucSeg-0.0.8/
+-rw-rw-rw-   0        0        0     1527 2023-02-28 22:32:05.000000 PyNucSeg-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      837 2023-05-08 22:11:38.756416 PyNucSeg-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2023-02-28 22:32:05.000000 PyNucSeg-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 22:11:38.767659 PyNucSeg-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      830 2023-05-08 22:04:59.000000 PyNucSeg-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:11:38.698727 PyNucSeg-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 22:11:38.738026 PyNucSeg-0.0.8/src/PyNucSeg.egg-info/
+-rw-rw-rw-   0        0        0      837 2023-05-08 22:11:37.000000 PyNucSeg-0.0.8/src/PyNucSeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-05-08 22:11:37.000000 PyNucSeg-0.0.8/src/PyNucSeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 22:11:37.000000 PyNucSeg-0.0.8/src/PyNucSeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-08 22:11:37.000000 PyNucSeg-0.0.8/src/PyNucSeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-08 22:11:37.000000 PyNucSeg-0.0.8/src/PyNucSeg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 22:11:38.751283 PyNucSeg-0.0.8/src/pynucseg/
+-rw-rw-rw-   0        0        0       83 2023-05-08 22:04:53.000000 PyNucSeg-0.0.8/src/pynucseg/__init__.py
+-rw-rw-rw-   0        0        0    16859 2023-05-08 21:52:20.000000 PyNucSeg-0.0.8/src/pynucseg/base.py
```

### Comparing `PyNucSeg-0.0.7/LICENSE` & `PyNucSeg-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNucSeg-0.0.7/PKG-INFO` & `PyNucSeg-0.0.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNucSeg
-Version: 0.0.7
+Version: 0.0.8
 Summary: Segment fluorescent nucleus, and measure the area, and the mean intensity per nucleus.
 Home-page: https://github.com/pganes/PyNucSeg
 Author: Ganesh Pandey
 Author-email: gpande3@uic.edu
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `PyNucSeg-0.0.7/setup.py` & `PyNucSeg-0.0.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md","r") as fh:
     long_description = fh.read()
 
 setup(
     name='PyNucSeg',
-    version='0.0.7',
+    version='0.0.8',
     author="Ganesh Pandey",
     author_email="gpande3@uic.edu",
     description='Segment fluorescent nucleus, and measure the area, and the mean intensity per nucleus.',
     long_description=long_description,
     long_description_content_type="text/markdown", 
     url="https://github.com/pganes/PyNucSeg",
     packages=['pynucseg'],
@@ -19,14 +19,15 @@
     ],
     install_requires=[
     "numpy",
     "stardist",
     "napari",
     "scikit-image",
     "tensorflow",
+    "pyqt5"
     ],
     extras_require ={
     "dev": [
     "pytest>=3.7",
     "twine",
     ]
     },
```

### Comparing `PyNucSeg-0.0.7/src/PyNucSeg.egg-info/PKG-INFO` & `PyNucSeg-0.0.8/src/PyNucSeg.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNucSeg
-Version: 0.0.7
+Version: 0.0.8
 Summary: Segment fluorescent nucleus, and measure the area, and the mean intensity per nucleus.
 Home-page: https://github.com/pganes/PyNucSeg
 Author: Ganesh Pandey
 Author-email: gpande3@uic.edu
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `PyNucSeg-0.0.7/src/pynucseg/base.py` & `PyNucSeg-0.0.8/src/pynucseg/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         # 
         ReferenceImage.all_fovs.append(self)
     
     def show_image_names(self):
         print(list(self.image.keys()))
         return 
         
-    def view_on_napari(self, return_viewer:bool=False)->napari.Viewer:
+    def view_on_napari(self,pixel_length_um=0.1, return_viewer:bool=False)->napari.Viewer:
         """Displays the availlable images in napari viewer.
 
         If no image is found, no viewer object will be returned.
 
         Parameters
         ----------
         return_viewer : bool, optional
@@ -107,18 +107,20 @@
         if len(self.image) == 0:
             print(f"Image not found!!")
             return
         else:
             viewer = napari.Viewer()
             for image_name,image in self.image.items():
                 if 'label' in image_name:
-                    viewer.add_labels(image, name=image_name)
+                    # viewer.add_labels(image, name=image_name))
+                    viewer.add_labels(image, name=image_name,scale=(pixel_length_um,pixel_length_um))
                 else:
-                    viewer.add_image(image, name=image_name)
-                    
+                    viewer.add_image(image, name=image_name,scale=(pixel_length_um,pixel_length_um))
+            viewer.scale_bar.visible = True
+            viewer.scale_bar.unit="um"       
             if return_viewer:
                 return viewer
             else:
                 return
     
 
     def smoothing(self,image_name:str=None,sigma:int=8,return_image:bool=False):
@@ -302,15 +304,34 @@
             filtared_labels[mask] = i+1
 
         self.image['boundary_filtered_labels'] = filtared_labels
         if return_results:
             return self.image['boundary_filtered_labels'], self.closedcontours,\
                 self.n_closedcontours
         
-    
+    def filterout_nuclei_by_area(self,
+                                 a_pixel_area:float=0.01,
+                                 area_threshold:list = [50,150]):
+        # Store area of each nucleus and mean intensity per pixel
+        area_per_nuclus = np.zeros((self.n_closedcontours,2))  
+        for i, label in enumerate(self.closedcontours):
+            mask = self.image['labels'] == label+1
+            area_per_nuclus[i,0] = label
+            area_per_nuclus[i,1] = len(np.where(mask==True)[0]) # area in terms of pixel
+
+        # convert unit of area to um^2
+        area_per_nuclus[:,1] = area_per_nuclus[:,1] * a_pixel_area
+        
+        # remove the very small and very big nuclei
+        true_nuclei_ind = np.where((area_per_nuclus[:,1] >= area_threshold[0]) &
+                               (area_per_nuclus[:,1] <= area_threshold[1]))[0]
+        
+        # 
+
+
     def get_cell_info(
             self,
             probe_names:list[str]=["PolII"],
             return_results:bool=False,
             a_pixel_area:float=0.01):
         """Adds `area_n_ADU` attribute that contains background subtracted
         mean intensity and the area of each nucleus and another attrubute
```

