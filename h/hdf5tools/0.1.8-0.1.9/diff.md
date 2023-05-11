# Comparing `tmp/hdf5tools-0.1.8.tar.gz` & `tmp/hdf5tools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdf5tools-0.1.8.tar", last modified: Wed Nov  9 22:20:47 2022, max compression
+gzip compressed data, was "hdf5tools-0.1.9.tar", last modified: Sun Nov 13 22:32:34 2022, max compression
```

## Comparing `hdf5tools-0.1.8.tar` & `hdf5tools-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-09 22:20:47.758199 hdf5tools-0.1.8/
--rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2022-11-04 04:18:51.000000 hdf5tools-0.1.8/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)      552 2022-11-09 22:20:47.758199 hdf5tools-0.1.8/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      452 2022-11-04 04:18:51.000000 hdf5tools-0.1.8/README.rst
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-09 22:20:47.758199 hdf5tools-0.1.8/hdf5tools/
--rw-rw-r--   0 mike      (1000) mike      (1000)       70 2022-11-09 22:20:34.000000 hdf5tools-0.1.8/hdf5tools/__init__.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-09 22:20:47.758199 hdf5tools-0.1.8/hdf5tools/datasets/
--rw-rw-r--   0 mike      (1000) mike      (1000)      906 2022-11-04 04:18:51.000000 hdf5tools-0.1.8/hdf5tools/datasets/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    18819 2022-11-09 22:19:00.000000 hdf5tools-0.1.8/hdf5tools/main.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    26110 2022-11-07 01:55:19.000000 hdf5tools-0.1.8/hdf5tools/utils.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-09 22:20:47.758199 hdf5tools-0.1.8/hdf5tools.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)      552 2022-11-09 22:20:47.000000 hdf5tools-0.1.8/hdf5tools.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      306 2022-11-09 22:20:47.000000 hdf5tools-0.1.8/hdf5tools.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2022-11-09 22:20:47.000000 hdf5tools-0.1.8/hdf5tools.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       64 2022-11-09 22:20:47.000000 hdf5tools-0.1.8/hdf5tools.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       10 2022-11-09 22:20:47.000000 hdf5tools-0.1.8/hdf5tools.egg-info/top_level.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      104 2022-11-04 04:18:51.000000 hdf5tools-0.1.8/pyproject.toml
--rw-rw-r--   0 mike      (1000) mike      (1000)       67 2022-11-09 22:20:47.758199 hdf5tools-0.1.8/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     7261 2022-11-09 22:19:51.000000 hdf5tools-0.1.8/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-13 22:32:34.511180 hdf5tools-0.1.9/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2022-11-04 04:18:51.000000 hdf5tools-0.1.9/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)      552 2022-11-13 22:32:34.511180 hdf5tools-0.1.9/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      452 2022-11-04 04:18:51.000000 hdf5tools-0.1.9/README.rst
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-13 22:32:34.511180 hdf5tools-0.1.9/hdf5tools/
+-rw-rw-r--   0 mike      (1000) mike      (1000)       70 2022-11-09 22:20:34.000000 hdf5tools-0.1.9/hdf5tools/__init__.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-13 22:32:34.511180 hdf5tools-0.1.9/hdf5tools/datasets/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      906 2022-11-04 04:18:51.000000 hdf5tools-0.1.9/hdf5tools/datasets/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    18690 2022-11-13 22:13:25.000000 hdf5tools-0.1.9/hdf5tools/main.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    26703 2022-11-13 22:31:40.000000 hdf5tools-0.1.9/hdf5tools/utils.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-13 22:32:34.511180 hdf5tools-0.1.9/hdf5tools.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      552 2022-11-13 22:32:34.000000 hdf5tools-0.1.9/hdf5tools.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      306 2022-11-13 22:32:34.000000 hdf5tools-0.1.9/hdf5tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2022-11-13 22:32:34.000000 hdf5tools-0.1.9/hdf5tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       64 2022-11-13 22:32:34.000000 hdf5tools-0.1.9/hdf5tools.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       10 2022-11-13 22:32:34.000000 hdf5tools-0.1.9/hdf5tools.egg-info/top_level.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      104 2022-11-04 04:18:51.000000 hdf5tools-0.1.9/pyproject.toml
+-rw-rw-r--   0 mike      (1000) mike      (1000)       67 2022-11-13 22:32:34.511180 hdf5tools-0.1.9/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7261 2022-11-13 22:04:36.000000 hdf5tools-0.1.9/setup.py
```

### Comparing `hdf5tools-0.1.8/LICENSE` & `hdf5tools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hdf5tools-0.1.8/PKG-INFO` & `hdf5tools-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdf5tools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python hdf5 tools
 Home-page: https://github.com/tethys-ts/hdf5tools
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: tethys
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hdf5tools-0.1.8/hdf5tools/datasets/__init__.py` & `hdf5tools-0.1.9/hdf5tools/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hdf5tools-0.1.8/hdf5tools/main.py` & `hdf5tools-0.1.9/hdf5tools/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,18 +112,15 @@
                     data_vars[k] = (v['dims'], np.empty(v['shape'], dtype=np.dtype('datetime64[ns]')))
                 else:
                     data_vars[k] = (v['dims'], np.empty(v['shape'], dtype=v['dtype_decoded']))
 
             coords = {}
             for k, v in self._coords_dict.items():
                 if k in all_data_coords:
-                    if 'datetime' in v.dtype.name:
-                        coords[k] = v.astype('datetime64[ns]')
-                    else:
-                        coords[k] = v
+                    coords[k] = utils.decode_data(v, **self._encodings[k])
 
             xr_ds = xr.Dataset(data_vars=data_vars, coords=coords, attrs=self._global_attrs)
 
             for ds_name, attr in self._attrs.items():
                 if ds_name in xr_ds:
                     xr_ds[ds_name].attrs = attr
             for ds_name, enc in self._encodings.items():
@@ -165,15 +162,15 @@
         Returns
         -------
         H5 instance
         """
         c = self.copy()
         if selection is not None:
             files = utils.open_files(self._files, self._group)
-            utils.filter_coords(files, c._coords_dict, selection)
+            utils.filter_coords(files, c._coords_dict, selection, self._encodings)
             vars_dict = utils.index_variables(files, c._coords_dict, c._encodings)
 
             c._data_vars_dict = vars_dict
 
             ## Close files
             utils.close_files(files)
 
@@ -319,28 +316,28 @@
                 else:
                     nf1 = nf
 
                 ## Add the coords as datasets
                 for coord, arr in self._coords_dict.items():
                     # if coord == 'time':
                     #     break
-                    enc_arr = utils.encode_data(arr, **self._encodings[coord])
-                    shape = enc_arr.shape
+                    shape = arr.shape
+                    dtype = self._encodings[coord]['dtype']
 
                     maxshape = tuple([s if s not in unlimited_dims else None for s in shape])
 
-                    chunks1 = utils.guess_chunk(shape, maxshape, enc_arr.dtype)
+                    chunks1 = utils.guess_chunk(shape, maxshape, dtype)
 
                     if isinstance(chunks, dict):
                         if coord in chunks:
                             chunks1 = chunks[coord]
 
-                    ds = nf1.create_dataset(coord, shape, chunks=chunks1, maxshape=maxshape, dtype=enc_arr.dtype, **compressor)
+                    ds = nf1.create_dataset(coord, shape, chunks=chunks1, maxshape=maxshape, dtype=dtype, **compressor)
 
-                    ds[:] = enc_arr
+                    ds[:] = arr
 
                     ds.make_scale(coord)
 
                 ## Add the variables as datasets
                 vars_dict = copy.deepcopy(self._data_vars_dict)
 
                 for var_name in vars_dict:
```

### Comparing `hdf5tools-0.1.8/hdf5tools/utils.py` & `hdf5tools-0.1.9/hdf5tools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,16 @@
     """
 
     """
     if 'datetime64' in data.dtype.name:
         data = encode_datetime(data, units, calendar)
 
     elif isinstance(scale_factor, (int, float, np.number)):
-        data = (data - add_offset)/scale_factor
+        # precision = int(np.abs(np.log10(val['scale_factor'])))
+        data = np.round((data - add_offset)/scale_factor)
 
         if isinstance(missing_value, (int, np.number)):
             data[np.isnan(data)] = missing_value
 
     if (data.dtype != dtype) or (data.dtype.name == 'object'):
         data = data.astype(dtype)
 
@@ -103,18 +104,18 @@
         data = data.astype(dtype_decoded)
 
         if isinstance(missing_value, (int, np.number)):
             data[data == missing_value] = np.nan
 
         data = (data * scale_factor) + add_offset
 
-    elif (data.dtype.name == 'object'):
-        data = data.astype(str).astype(dtype_decoded)
+    # elif (data.dtype.name == 'object'):
+    #     data = data.astype(str).astype(dtype_decoded)
 
-    elif (data.dtype != dtype_decoded):
+    elif (data.dtype != dtype_decoded) or (data.dtype.name == 'object'):
         data = data.astype(dtype_decoded)
 
     return data
 
 
 def get_encoding(data):
     """
@@ -144,14 +145,16 @@
         encoding['dtype'] = np.dtype('int64')
         if 'units' not in encoding:
             encoding['units'] = 'seconds since 1970-01-01 00:00:00'
         encoding['missing_value'] = missing_value_dict['int64']
         encoding['_FillValue'] = encoding['missing_value']
 
     if 'dtype' not in encoding:
+        if np.issubdtype(data.dtype, np.floating):
+            raise ValueError('float dtypes must have encoding data to encode to int.')
         encoding['dtype'] = data.dtype
     elif isinstance(encoding['dtype'], str):
         encoding['dtype'] = np.dtype(encoding['dtype'])
 
     if 'scale_factor' in encoding:
         if not isinstance(encoding['scale_factor'], (int, float, np.number)):
             raise TypeError('scale_factor must be an int or float.')
@@ -331,18 +334,20 @@
         else:
             ds_list = [ds_name for ds_name in file.keys() if is_scale(file[ds_name])]
 
         for ds_name in ds_list:
             ds = file[ds_name]
 
             if isinstance(file, xr.Dataset):
-                # data = decode_data(ds.values, **encodings[ds_name])
-                data = ds.values
+                data = encode_data(ds.values, **encodings[ds_name])
             else:
-                data = decode_data(ds[:], **encodings[ds_name])
+                if ds.dtype.name == 'object':
+                    data = ds[:].astype(str).astype(h5py.string_dtype())
+                else:
+                    data = ds[:]
 
             if ds_name in coords_dict:
                 coords_dict[ds_name] = np.union1d(coords_dict[ds_name], data)
             else:
                 coords_dict[ds_name] = data
 
     return coords_dict
@@ -351,14 +356,16 @@
 def index_variables(files, coords_dict, encodings):
     """
 
     """
     vars_dict = {}
 
     for i, file in enumerate(files):
+        # if i == 77:
+        #     break
 
         if isinstance(file, xr.Dataset):
             ds_list = list(file.data_vars)
         else:
             ds_list = [ds_name for ds_name in file.keys() if not is_scale(file[ds_name])]
 
         for ds_name in ds_list:
@@ -370,22 +377,27 @@
             global_index = []
             local_index = []
             remove_ds = False
 
             for dim in ds.dims:
                 if isinstance(file, xr.Dataset):
                     dim_name = dim
-                    # dim_data = decode_data(ds[dim_name].values, **encodings[dim_name])
-                    dim_data = ds[dim_name].values
+                    dim_data = encode_data(ds[dim_name].values, **encodings[dim_name])
                 else:
                     dim_name = dim[0].name.split('/')[-1]
-                    dim_data = decode_data(dim[0][:], **encodings[dim_name])
+                    if dim[0].dtype.name == 'object':
+                        dim_data = dim[0][:].astype(str).astype(h5py.string_dtype())
+                    else:
+                        dim_data = dim[0][:]
 
                 dims.append(dim_name)
 
+                # if dim_name == 'lon':
+                #     break
+
                 global_arr_index = np.where(np.isin(coords_dict[dim_name], dim_data))[0]
                 local_arr_index = np.where(np.isin(dim_data, coords_dict[dim_name]))[0]
 
                 if len(global_arr_index) > 0:
 
                     if is_regular_index(global_arr_index):
                         slice1 = slice(global_arr_index.min(), global_arr_index.max() + 1)
@@ -492,23 +504,23 @@
 #             slice_index = slice(None, None)
 
 #         index_coords_dict[coord] = slice_index
 
 #     return index_coords_dict
 
 
-def filter_coords(files, coords_dict, selection):
+def filter_coords(files, coords_dict, selection, encodings):
     """
 
     """
     for coord, sel in selection.items():
         if coord not in coords_dict:
             raise ValueError(coord + ' one of the coordinates.')
 
-        coord_data = coords_dict[coord]
+        coord_data = decode_data(coords_dict[coord], **encodings[coord])
 
         if isinstance(sel, slice):
             if 'datetime64' in coord_data.dtype.name:
                 if not isinstance(sel.start, (str, np.datetime64)):
                     raise TypeError('Input for datetime selection should be either a datetime string or np.datetime64.')
                 start = np.datetime64(sel.start, 's')
                 end = np.datetime64(sel.stop, 's')
@@ -528,15 +540,15 @@
             if sel1.dtype.name == 'bool':
                 if sel1.shape[0] != coord_data.shape[0]:
                     raise ValueError('The boolean array does not have the same length as the coord array.')
                 bool_index = sel1
             else:
                 bool_index = np.in1d(coord_data, sel1)
 
-        new_coord_data = coord_data[bool_index]
+        new_coord_data = encode_data(coord_data[bool_index], **encodings[coord])
 
         coords_dict[coord] = new_coord_data
```

### Comparing `hdf5tools-0.1.8/hdf5tools.egg-info/PKG-INFO` & `hdf5tools-0.1.9/hdf5tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdf5tools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python hdf5 tools
 Home-page: https://github.com/tethys-ts/hdf5tools
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: tethys
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hdf5tools-0.1.8/setup.py` & `hdf5tools-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # General parameters
 name = 'hdf5tools'
 main_package = 'hdf5tools'
 datasets = 'datasets'
-version = '0.1.8'
+version = '0.1.9'
 descrip = 'Python hdf5 tools'
 
 # The below code is for readthedocs. To have sphinx/readthedocs interact with
 # the contained package, readthedocs needs to build the package. But the dependencies
 # should be installed via the conda yml env file rather than during the package build.
 if os.environ.get('READTHEDOCS', False) == 'True':
     INSTALL_REQUIRES = []
```

