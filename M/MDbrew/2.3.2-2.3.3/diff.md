# Comparing `tmp/MDbrew-2.3.2.tar.gz` & `tmp/MDbrew-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MDbrew-2.3.2.tar", last modified: Mon May  8 12:17:25 2023, max compression
+gzip compressed data, was "MDbrew-2.3.3.tar", last modified: Thu May 11 12:13:06 2023, max compression
```

## Comparing `MDbrew-2.3.2.tar` & `MDbrew-2.3.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-08 12:17:25.644718 MDbrew-2.3.2/
--rw-r--r--   0 minu       (501) staff       (20)       25 2023-05-07 05:40:59.000000 MDbrew-2.3.2/MANIFEST.in
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-08 12:17:25.640618 MDbrew-2.3.2/MDbrew/
--rw-r--r--   0 minu       (501) staff       (20)      238 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/__init__.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-08 12:17:25.642027 MDbrew-2.3.2/MDbrew/analysis/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/analysis/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     4477 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/analysis/msd.py
--rw-r--r--   0 minu       (501) staff       (20)     5860 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/analysis/rdf.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-08 12:17:25.642364 MDbrew-2.3.2/MDbrew/application/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/application/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)    10054 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/application/brewcp2k.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-08 12:17:25.642806 MDbrew-2.3.2/MDbrew/main/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/main/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     5374 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/main/brewery.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-08 12:17:25.643835 MDbrew-2.3.2/MDbrew/main/filetype/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/main/filetype/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)      940 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/main/filetype/gro.py
--rw-r--r--   0 minu       (501) staff       (20)      860 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/main/filetype/lmps.py
--rw-r--r--   0 minu       (501) staff       (20)      777 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/main/filetype/pdb.py
--rw-r--r--   0 minu       (501) staff       (20)     4294 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/main/filetype/trr.py
--rw-r--r--   0 minu       (501) staff       (20)     1370 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/main/filetype/vasp.py
--rw-r--r--   0 minu       (501) staff       (20)      486 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/main/filetype/xyz.py
--rw-r--r--   0 minu       (501) staff       (20)     1163 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/main/opener.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-08 12:17:25.644563 MDbrew-2.3.2/MDbrew/tool/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/tool/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     3618 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/tool/colorfont.py
--rw-r--r--   0 minu       (501) staff       (20)     1578 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/tool/decorator.py
--rw-r--r--   0 minu       (501) staff       (20)      756 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/tool/doctor.py
--rw-r--r--   0 minu       (501) staff       (20)      619 2023-05-08 12:16:23.000000 MDbrew-2.3.2/MDbrew/tool/spacer.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-08 12:17:25.641566 MDbrew-2.3.2/MDbrew.egg-info/
--rw-r--r--   0 minu       (501) staff       (20)      340 2023-05-08 12:17:25.000000 MDbrew-2.3.2/MDbrew.egg-info/PKG-INFO
--rw-r--r--   0 minu       (501) staff       (20)      740 2023-05-08 12:17:25.000000 MDbrew-2.3.2/MDbrew.egg-info/SOURCES.txt
--rw-r--r--   0 minu       (501) staff       (20)        1 2023-05-08 12:17:25.000000 MDbrew-2.3.2/MDbrew.egg-info/dependency_links.txt
--rw-r--r--   0 minu       (501) staff       (20)        1 2023-05-08 12:17:25.000000 MDbrew-2.3.2/MDbrew.egg-info/not-zip-safe
--rw-r--r--   0 minu       (501) staff       (20)        7 2023-05-08 12:17:25.000000 MDbrew-2.3.2/MDbrew.egg-info/top_level.txt
--rw-r--r--   0 minu       (501) staff       (20)      340 2023-05-08 12:17:25.644803 MDbrew-2.3.2/PKG-INFO
--rw-r--r--   0 minu       (501) staff       (20)       62 2023-05-07 05:40:59.000000 MDbrew-2.3.2/requirement.txt
--rw-r--r--   0 minu       (501) staff       (20)       79 2023-05-08 12:17:25.645061 MDbrew-2.3.2/setup.cfg
--rw-r--r--   0 minu       (501) staff       (20)      664 2023-05-08 12:16:46.000000 MDbrew-2.3.2/setup.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-11 12:13:06.053016 MDbrew-2.3.3/
+-rw-r--r--   0 minu       (501) staff       (20)       25 2023-05-08 12:21:50.000000 MDbrew-2.3.3/MANIFEST.in
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-11 12:13:06.049231 MDbrew-2.3.3/MDbrew/
+-rw-r--r--   0 minu       (501) staff       (20)      182 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/__init__.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-11 12:13:06.050440 MDbrew-2.3.3/MDbrew/analysis/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/analysis/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     4477 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/analysis/msd.py
+-rw-r--r--   0 minu       (501) staff       (20)     5984 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/analysis/rdf.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-11 12:13:06.050992 MDbrew-2.3.3/MDbrew/application/
+-rw-r--r--   0 minu       (501) staff       (20)       30 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/application/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)    10054 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/application/cp2k2npy.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-11 12:13:06.051433 MDbrew-2.3.3/MDbrew/main/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/main/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     5142 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/main/brewery.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-11 12:13:06.052283 MDbrew-2.3.3/MDbrew/main/filetype/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/main/filetype/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)      940 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/main/filetype/gro.py
+-rw-r--r--   0 minu       (501) staff       (20)      904 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/main/filetype/lmps.py
+-rw-r--r--   0 minu       (501) staff       (20)      848 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/main/filetype/pdb.py
+-rw-r--r--   0 minu       (501) staff       (20)     4294 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/main/filetype/trr.py
+-rw-r--r--   0 minu       (501) staff       (20)     1414 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/main/filetype/vasp.py
+-rw-r--r--   0 minu       (501) staff       (20)      530 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/main/filetype/xyz.py
+-rw-r--r--   0 minu       (501) staff       (20)     1381 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/main/opener.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-11 12:13:06.052873 MDbrew-2.3.3/MDbrew/tool/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/tool/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     3618 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/tool/colorfont.py
+-rw-r--r--   0 minu       (501) staff       (20)     1578 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/tool/decorator.py
+-rw-r--r--   0 minu       (501) staff       (20)      765 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/tool/doctor.py
+-rw-r--r--   0 minu       (501) staff       (20)      619 2023-05-11 12:11:55.000000 MDbrew-2.3.3/MDbrew/tool/spacer.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-11 12:13:06.050024 MDbrew-2.3.3/MDbrew.egg-info/
+-rw-r--r--   0 minu       (501) staff       (20)      340 2023-05-11 12:13:05.000000 MDbrew-2.3.3/MDbrew.egg-info/PKG-INFO
+-rw-r--r--   0 minu       (501) staff       (20)      740 2023-05-11 12:13:05.000000 MDbrew-2.3.3/MDbrew.egg-info/SOURCES.txt
+-rw-r--r--   0 minu       (501) staff       (20)        1 2023-05-11 12:13:05.000000 MDbrew-2.3.3/MDbrew.egg-info/dependency_links.txt
+-rw-r--r--   0 minu       (501) staff       (20)        1 2023-05-11 12:13:05.000000 MDbrew-2.3.3/MDbrew.egg-info/not-zip-safe
+-rw-r--r--   0 minu       (501) staff       (20)        7 2023-05-11 12:13:05.000000 MDbrew-2.3.3/MDbrew.egg-info/top_level.txt
+-rw-r--r--   0 minu       (501) staff       (20)      340 2023-05-11 12:13:06.053073 MDbrew-2.3.3/PKG-INFO
+-rw-r--r--   0 minu       (501) staff       (20)       62 2023-05-08 12:21:50.000000 MDbrew-2.3.3/requirement.txt
+-rw-r--r--   0 minu       (501) staff       (20)       79 2023-05-11 12:13:06.053269 MDbrew-2.3.3/setup.cfg
+-rw-r--r--   0 minu       (501) staff       (20)      664 2023-05-11 12:12:27.000000 MDbrew-2.3.3/setup.py
```

### Comparing `MDbrew-2.3.2/MDbrew/analysis/msd.py` & `MDbrew-2.3.3/MDbrew/analysis/msd.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.2/MDbrew/analysis/rdf.py` & `MDbrew-2.3.3/MDbrew/analysis/rdf.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,52 +17,50 @@
         self,
         a,
         b,
         box_size=None,
         layer: int = 0,
         r_max: float = None,
         resolution: int = 1000,
-        max_frame: int = None,
         dtype: str = "float32",
     ):
         if type(a) == Brewery:
             self.is_Brewery_type = True
             self.a = a
             self.b = b
-            self.frame_num = max_frame
             self.a_number = a.atom_num
             self.b_number = b.atom_num
             self.box_size = a.box_size if box_size is None else box_size
             assert len(self.box_size), "plz set box_size"
         else:
             self.is_Brewery_type = False
             self.a = check_dimension(a, dim=3)
             self.b = check_dimension(b, dim=3)
-            self.frame_num = self.a.shape[0] if max_frame is None else max_frame
             self.a_number = self.a.shape[1]
             self.b_number = self.b.shape[1]
+            self.box_size = box_size
 
         self.box_size = np.array(self.box_size, dtype=dtype)
         self.half_box_size = self.box_size * 0.5
 
         self.layer_depth = layer
         self.layer = self.__make_layer()
 
         self.resolution = resolution
         self.r_max = np.max(self.half_box_size) * (2.0 * self.layer_depth + 1.0) if r_max is None else r_max
         self.dr = self.r_max / self.resolution
 
         self.hist_data = None
         self.radii = np.linspace(0.0, self.r_max, self.resolution)
 
-    def run(self):
+    def run(self, start=0, end=None, step=1):
         if self.is_Brewery_type:
-            self._cal_hist_data_with_generator()
+            self._cal_hist_data_with_generator(start=start, end=end, step=step)
         else:
-            self._cal_hist_data_with_iterator()
+            self._cal_hist_data_with_iterator(start=start, end=end, step=step)
         return self
 
     @property
     def result(self):
         if self.hist_data is None:
             self.run()
         return self.__cal_rdf_from_hist_data()
@@ -70,35 +68,37 @@
     @property
     def cn(self):
         if self.hist_data is None:
             self.run()
         return self.__cal_cn_from_hist_data()
 
     # Function for get hist
-    def _cal_hist_data_with_iterator(self):
+    def _cal_hist_data_with_iterator(self, start=0, end=None, step=1):
         self.hist_data = np.zeros(self.resolution)
         _apply_boundary_condition = self.__set_boundary_condition()
-        for frame in trange(self.frame_num, **self.kwrgs_trange):
+        self.frame_num = self.a.shape[0] if end is None else end - start + 1
+        for frame in trange(start=start, stop=end, step=step, **self.kwrgs_trange):
             a_unit = self.a[frame, ...]
             b_unit = self.b[frame, ...]
             diff_position = get_diff_position(a_unit[:, None, :], b_unit[None, :, :])
             diff_position = _apply_boundary_condition(diff_position=diff_position)
             distance = get_distance(diff_position=diff_position, axis=-1)
             idx_hist = self.__cal_idx_histogram(distance=distance)
             value, count = np.unique(idx_hist, return_counts=True)
             self.hist_data[value] += count
 
     # Function for get hist
-    def _cal_hist_data_with_generator(self):
+    def _cal_hist_data_with_generator(self, start=0, end=None, step=1):
         self.hist_data = np.zeros(self.resolution)
         _apply_boundary_condition = self.__set_boundary_condition()
         frame_num = 0
-        for _ in tqdm(zip(self.a.frange(), self.b.frange()), **self.kwrgs_trange):
-            if self.frame_num is not None and frame_num == self.frame_num:
-                break
+        for _ in tqdm(
+            zip(self.a.frange(start=start, end=end, step=step), self.b.frange(start=start, end=end, step=step)),
+            **self.kwrgs_trange,
+        ):
             frame_num += 1
             a_unit = self.a.coords
             b_unit = self.b.coords
             diff_position = get_diff_position(a_unit[:, None, :], b_unit[None, :, :])
             diff_position = _apply_boundary_condition(diff_position=diff_position)
             distance = get_distance(diff_position=diff_position, axis=-1)
             idx_hist = self.__cal_idx_histogram(distance=distance)
```

### Comparing `MDbrew-2.3.2/MDbrew/application/brewcp2k.py` & `MDbrew-2.3.3/MDbrew/application/cp2k2npy.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from tqdm import tqdm
 from scipy import constants
 from ..main.brewery import Brewery
 from ..tool.colorfont import color
 from ..tool.decorator import color_print
 
 
-class BrewCP2K(object):
+class CP2K2NPY(object):
     tqmd_option = {"ascii": " #"}
     printing_option = {
         "2array": f" #CONVERT  {color.font_yellow}List2Array{color.reset}",
         "2a.u": f" #CONVERT  {color.font_yellow}Atomic Unit{color.reset}",
         "save": f" #SAVE  {color.font_yellow}THE DATA{color.reset}",
         "kind2type": f" #CONVERT  {color.font_yellow}KIND2TYPE{color.reset}",
     }
```

### Comparing `MDbrew-2.3.2/MDbrew/main/brewery.py` & `MDbrew-2.3.3/MDbrew/main/brewery.py`

 * *Files 12% similar despite different names*

```diff
@@ -123,26 +123,20 @@
 
     def _check_path(self, path, **kwrgs):
         path = os.path.join(os.getcwd(), path)
         assert os.path.isfile(path=path), f"Check your path || not {path}"
         return path
 
     def frange(self, start: int = 0, end: int = None, step: int = 1):
-        self.reset()
-        assert start >= 0, ValueError("Frame start idx should be positive")
-        i = 0
-        while i < start:
-            max_frame = i
-            try:
-                self.next_frame
-                i += 1
-            except:
-                raise ValueError(f"start idx should be lower than {max_frame}")
+        self.move_frame(num=start)
         while True:
             try:
                 if self.frame == end:
                     break
                 if not (self.frame - start) % step:
                     yield self.frame
                 self.next_frame
             except:
                 break
+
+    def move_frame(self, num):
+        self._opener.skip_frame(num=num)
```

### Comparing `MDbrew-2.3.2/MDbrew/main/filetype/gro.py` & `MDbrew-2.3.3/MDbrew/main/filetype/gro.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.2/MDbrew/main/filetype/lmps.py` & `MDbrew-2.3.3/MDbrew/main/filetype/lmps.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
     def _make_one_frame_data(self, file):
         self.skip_line(file=file, num=3)
         atom_num = int(file.readline().split()[0])
         self.skip_line(file=file, num=1)
         self.box_size = [sum([abs(float(box_length)) for box_length in file.readline().split()]) for _ in range(3)]
         self.column = file.readline().split()[2:]
+        self.total_line_num = 9 + atom_num
         return [self.str2float_list(file.readline().split()) for _ in range(atom_num)]
 
     def skip_line(self, file, num):
         for _ in range(num):
             file.readline()
 
     def str2float_list(self, str_list):
```

### Comparing `MDbrew-2.3.2/MDbrew/main/filetype/pdb.py` & `MDbrew-2.3.3/MDbrew/main/filetype/pdb.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,13 +10,15 @@
         super().gen_db()
 
     def _make_one_frame_data(self, file):
         first__loop_line = file.readline()
         second_loop_line = file.readline()
         self.box_size = [float(box_length) for box_length in second_loop_line.split()[1:4]]
         one_frame_data = []
+        self.total_line_num = 3
         while True:
             line = file.readline()
             if "END" in line:
                 break
+            self.total_line_num += 1
             one_frame_data.append(line.split())
         return one_frame_data
```

### Comparing `MDbrew-2.3.2/MDbrew/main/filetype/trr.py` & `MDbrew-2.3.3/MDbrew/main/filetype/trr.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.2/MDbrew/main/filetype/vasp.py` & `MDbrew-2.3.3/MDbrew/main/filetype/vasp.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
         self._set_box_and_atom(path=path)
         super().gen_db()
 
     def _make_one_frame_data(self, file):
         first_loop_line = file.readline()
         step = first_loop_line.split()[-1]
         num_atom = sum(self.atom_kind_num)
+        self.total_line_num = num_atom + 1
         database = []
         c_atom_num = 0
         pointer = 0
         for _ in range(num_atom):
             if c_atom_num >= self.atom_kind_num[pointer]:
                 pointer += 1
                 c_atom_num = 0
```

### Comparing `MDbrew-2.3.2/MDbrew/main/opener.py` & `MDbrew-2.3.3/MDbrew/main/opener.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-import abc
+from abc import abstractmethod
 
 
 class Opener(object):
     skip_head = 0
     read_mode = "r"
     is_require_gro = False
+    total_line_num = 0
 
     def __init__(self, path: str, *args, **kwrgs) -> None:
         self.path = path
         self.column = []
         self.box_size = []
         self._atom_keyword = "atom"
 
-    def gen_db(self):
-        self.frame = -1
+    def gen_db(self, frame=0):
+        self.frame = frame - 1
         self._database = self._generate_database()
         self.next_frame()
 
     def reset(self):
         self.gen_db()
 
     @property
@@ -27,22 +28,27 @@
     @property
     def data(self):
         return self._data
 
     def next_frame(self):
         self._data = next(self._database)
 
-    @abc.abstractmethod
+    @abstractmethod
     def _make_one_frame_data(self, file):
         pass
 
     # Generation database
     def _generate_database(self):
         with open(file=self.path, mode=self.read_mode) as file:
             for _ in range(self.skip_head):
                 file.readline()
             while True:
                 try:
                     self.frame += 1
                     yield self._make_one_frame_data(file=file)
                 except:
                     break
+
+    def skip_frame(self, num):
+        total_skip_line = self.total_line_num * num
+        self.skip_head += total_skip_line
+        self.gen_db(frame=num)
```

### Comparing `MDbrew-2.3.2/MDbrew/tool/colorfont.py` & `MDbrew-2.3.3/MDbrew/tool/colorfont.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.2/MDbrew/tool/decorator.py` & `MDbrew-2.3.3/MDbrew/tool/decorator.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.2/MDbrew/tool/doctor.py` & `MDbrew-2.3.3/MDbrew/tool/doctor.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,13 +13,13 @@
     atom_info = mb.atom_info
     order1 = mb.order(what="type == 1")
     order2 = mb.order(what="type == 2")
     print(sep_line)
     position = order1.coords
     ixiyiz = order1.brew(cols=["ix", "iy", "iz"])
     unwrapped_position = [position + ixiyiz for _ in order1.frange()]
-    rdf = RDF(order1, order2, mb.box_size, max_frame=100).run()
+    rdf = RDF(order1, order2, mb.box_size).run(start=2, end=100, step=2)
     rdf.result
     msd = MSD(unwrapped_position).run()
     msd.result
     print(sep_line)
     print(mb)
```

### Comparing `MDbrew-2.3.2/MDbrew/tool/spacer.py` & `MDbrew-2.3.3/MDbrew/tool/spacer.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.2/MDbrew.egg-info/SOURCES.txt` & `MDbrew-2.3.3/MDbrew.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 MDbrew.egg-info/dependency_links.txt
 MDbrew.egg-info/not-zip-safe
 MDbrew.egg-info/top_level.txt
 MDbrew/analysis/__init__.py
 MDbrew/analysis/msd.py
 MDbrew/analysis/rdf.py
 MDbrew/application/__init__.py
-MDbrew/application/brewcp2k.py
+MDbrew/application/cp2k2npy.py
 MDbrew/main/__init__.py
 MDbrew/main/brewery.py
 MDbrew/main/opener.py
 MDbrew/main/filetype/__init__.py
 MDbrew/main/filetype/gro.py
 MDbrew/main/filetype/lmps.py
 MDbrew/main/filetype/pdb.py
```

### Comparing `MDbrew-2.3.2/setup.py` & `MDbrew-2.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="MDbrew",
-    version="2.3.2",
+    version="2.3.3",
     author="Knu",
     author_email="minu928@snu.ac.kr",
     url="https://github.com/MyKnu/MDbrew",
-    download_url="https://github.com/MyKnu/MDbrew/install_file/MDbrew-2.3.2.tar.gz",
+    download_url="https://github.com/MyKnu/MDbrew/install_file/MDbrew-2.3.3.tar.gz",
     install_requies=[
         "numpy>=1.0.0",
         "pandas>=1.0.0",
         "matplotlib>=1.0.0",
         "tqdm>=1.0.0",
     ],
     description="Postprocessing tools for the MD simulation results (ex. lammps)",
```

