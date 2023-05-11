# Comparing `tmp/fastsweep-0.1.1.tar.gz` & `tmp/fastsweep-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastsweep-0.1.1.tar", last modified: Wed Sep 28 08:43:29 2022, max compression
+gzip compressed data, was "fastsweep-0.1.2.tar", last modified: Thu May 11 18:05:18 2023, max compression
```

## Comparing `fastsweep-0.1.1.tar` & `fastsweep-0.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 08:43:29.657127 fastsweep-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-09-28 08:43:15.000000 fastsweep-0.1.1/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 08:43:29.653127 fastsweep-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 08:43:29.657127 fastsweep-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-09-28 08:43:15.000000 fastsweep-0.1.1/.github/workflows/macOS_arm64_toolchain.cmake
--rwxr-xr-x   0 runner    (1001) docker     (121)     2493 2022-09-28 08:43:15.000000 fastsweep-0.1.1/.github/workflows/tag_wheel_manylinux.py
--rw-r--r--   0 runner    (1001) docker     (121)     3420 2022-09-28 08:43:15.000000 fastsweep-0.1.1/.github/workflows/wheels.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2152 2022-09-28 08:43:15.000000 fastsweep-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 08:43:15.000000 fastsweep-0.1.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-09-28 08:43:15.000000 fastsweep-0.1.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3465 2022-09-28 08:43:15.000000 fastsweep-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4425 2022-09-28 08:43:29.657127 fastsweep-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4113 2022-09-28 08:43:15.000000 fastsweep-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 08:43:29.657127 fastsweep-0.1.1/cmake-defaults/
--rw-r--r--   0 runner    (1001) docker     (121)    12690 2022-09-28 08:43:15.000000 fastsweep-0.1.1/cmake-defaults/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 08:43:29.657127 fastsweep-0.1.1/kernels/
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-09-28 08:43:15.000000 fastsweep-0.1.1/kernels/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     3057 2022-09-28 08:43:15.000000 fastsweep-0.1.1/kernels/cuda_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (121)    30671 2022-09-28 08:43:15.000000 fastsweep-0.1.1/kernels/cuda_kernels.h
--rw-r--r--   0 runner    (1001) docker     (121)     6038 2022-09-28 08:43:15.000000 fastsweep-0.1.1/kernels/cuda_kernels.ptx
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-09-28 08:43:15.000000 fastsweep-0.1.1/kernels/vec.h
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-09-28 08:43:15.000000 fastsweep-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 08:43:29.657127 fastsweep-0.1.1/python/
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2022-09-28 08:43:15.000000 fastsweep-0.1.1/python/example.py
--rw-r--r--   0 runner    (1001) docker     (121)     9234 2022-09-28 08:43:15.000000 fastsweep-0.1.1/python/pure_python_impl.py
--rw-r--r--   0 runner    (1001) docker     (121)    39945 2022-09-28 08:43:15.000000 fastsweep-0.1.1/redistancing.svg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-28 08:43:29.657127 fastsweep-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1405 2022-09-28 08:43:15.000000 fastsweep-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 08:43:29.657127 fastsweep-0.1.1/src/
--rw-r--r--   0 runner    (1001) docker     (121)     3111 2022-09-28 08:43:15.000000 fastsweep-0.1.1/src/cuda_helpers.h
--rw-r--r--   0 runner    (1001) docker     (121)    14656 2022-09-28 08:43:15.000000 fastsweep-0.1.1/src/distance_marcher.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-09-28 08:43:15.000000 fastsweep-0.1.1/src/distance_marcher.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 08:43:29.657127 fastsweep-0.1.1/src/fastsweep/
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-09-28 08:43:15.000000 fastsweep-0.1.1/src/fastsweep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 08:43:29.657127 fastsweep-0.1.1/src/fastsweep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4425 2022-09-28 08:43:29.000000 fastsweep-0.1.1/src/fastsweep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-09-28 08:43:29.000000 fastsweep-0.1.1/src/fastsweep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-28 08:43:29.000000 fastsweep-0.1.1/src/fastsweep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-28 08:43:29.000000 fastsweep-0.1.1/src/fastsweep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-28 08:43:29.000000 fastsweep-0.1.1/src/fastsweep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-09-28 08:43:15.000000 fastsweep-0.1.1/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 08:43:29.657127 fastsweep-0.1.1/src/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-09-28 08:43:15.000000 fastsweep-0.1.1/src/tests/test_redistancing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:18.428388 fastsweep-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-11 18:05:06.000000 fastsweep-0.1.2/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:18.424388 fastsweep-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:18.424388 fastsweep-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-11 18:05:06.000000 fastsweep-0.1.2/.github/workflows/macOS_arm64_toolchain.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2493 2023-05-11 18:05:06.000000 fastsweep-0.1.2/.github/workflows/tag_wheel_manylinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-11 18:05:06.000000 fastsweep-0.1.2/.github/workflows/wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-11 18:05:06.000000 fastsweep-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:06.000000 fastsweep-0.1.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-11 18:05:06.000000 fastsweep-0.1.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-11 18:05:06.000000 fastsweep-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-05-11 18:05:18.428388 fastsweep-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-11 18:05:06.000000 fastsweep-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:18.424388 fastsweep-0.1.2/cmake-defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-05-11 18:05:06.000000 fastsweep-0.1.2/cmake-defaults/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:18.428388 fastsweep-0.1.2/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-11 18:05:06.000000 fastsweep-0.1.2/kernels/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-11 18:05:06.000000 fastsweep-0.1.2/kernels/cuda_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    30671 2023-05-11 18:05:06.000000 fastsweep-0.1.2/kernels/cuda_kernels.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-05-11 18:05:06.000000 fastsweep-0.1.2/kernels/cuda_kernels.ptx
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-11 18:05:06.000000 fastsweep-0.1.2/kernels/vec.h
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-11 18:05:06.000000 fastsweep-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:18.428388 fastsweep-0.1.2/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-11 18:05:06.000000 fastsweep-0.1.2/python/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-05-11 18:05:06.000000 fastsweep-0.1.2/python/pure_python_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39945 2023-05-11 18:05:06.000000 fastsweep-0.1.2/redistancing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 18:05:18.428388 fastsweep-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-11 18:05:06.000000 fastsweep-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:18.428388 fastsweep-0.1.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-11 18:05:06.000000 fastsweep-0.1.2/src/cuda_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-05-11 18:05:06.000000 fastsweep-0.1.2/src/distance_marcher.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-11 18:05:06.000000 fastsweep-0.1.2/src/distance_marcher.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:18.428388 fastsweep-0.1.2/src/fastsweep/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-11 18:05:06.000000 fastsweep-0.1.2/src/fastsweep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:18.428388 fastsweep-0.1.2/src/fastsweep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-05-11 18:05:18.000000 fastsweep-0.1.2/src/fastsweep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-11 18:05:18.000000 fastsweep-0.1.2/src/fastsweep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:05:18.000000 fastsweep-0.1.2/src/fastsweep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 18:05:18.000000 fastsweep-0.1.2/src/fastsweep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 18:05:18.000000 fastsweep-0.1.2/src/fastsweep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-11 18:05:06.000000 fastsweep-0.1.2/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:18.428388 fastsweep-0.1.2/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-11 18:05:06.000000 fastsweep-0.1.2/src/tests/test_redistancing.py
```

### Comparing `fastsweep-0.1.1/.clang-format` & `fastsweep-0.1.2/.clang-format`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.1/.github/workflows/tag_wheel_manylinux.py` & `fastsweep-0.1.2/.github/workflows/tag_wheel_manylinux.py`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.1/.github/workflows/wheels.yml` & `fastsweep-0.1.2/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.1/.gitignore` & `fastsweep-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.1/CMakeLists.txt` & `fastsweep-0.1.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.1/LICENSE` & `fastsweep-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.1/PKG-INFO` & `fastsweep-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastsweep
-Version: 0.1.1
+Version: 0.1.2
 Summary: Eikonal solver using parallel fast sweeping
 Home-page: https://github.com/rgl-epfl/fastsweep
 Author: Delio Vicini
 Author-email: delio.vicini@gmail.com
 License: BSD
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `fastsweep-0.1.1/README.md` & `fastsweep-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.1/cmake-defaults/CMakeLists.txt` & `fastsweep-0.1.2/cmake-defaults/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.1/kernels/cuda_kernels.cu` & `fastsweep-0.1.2/kernels/cuda_kernels.cu`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.1/kernels/cuda_kernels.h` & `fastsweep-0.1.2/kernels/cuda_kernels.h`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.1/kernels/cuda_kernels.ptx` & `fastsweep-0.1.2/kernels/cuda_kernels.ptx`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.1/pyproject.toml` & `fastsweep-0.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools", "wheel", "scikit-build", "cmake", "ninja", "pybind11", "drjit>=0.2.0"]
+requires = ["setuptools", "wheel", "scikit-build", "cmake", "ninja", "pybind11", "drjit>=0.4.2"]
 
 build-backend = "setuptools.build_meta"
 
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
```

### Comparing `fastsweep-0.1.1/python/example.py` & `fastsweep-0.1.2/python/example.py`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.1/python/pure_python_impl.py` & `fastsweep-0.1.2/python/pure_python_impl.py`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.1/redistancing.svg` & `fastsweep-0.1.2/redistancing.svg`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.1/setup.py` & `fastsweep-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 fastsweep_cmake_toolchain_file = os.environ.get("FASTSWEEP_CMAKE_TOOLCHAIN_FILE", "")
 fastsweep_drjit_cmake_dir = os.environ.get("FASTSWEEP_DRJIT_CMAKE_DIR", "")
 
-VERSION = "0.1.1"
+VERSION = "0.1.2"
 
 setup(
     name="fastsweep",
     version=VERSION,
     description="Eikonal solver using parallel fast sweeping",
     author="Delio Vicini",
     author_email="delio.vicini@gmail.com",
```

### Comparing `fastsweep-0.1.1/src/cuda_helpers.h` & `fastsweep-0.1.2/src/cuda_helpers.h`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.1/src/distance_marcher.cpp` & `fastsweep-0.1.2/src/distance_marcher.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Vec3i block_size(16, 16, 1);
     if (total_num_threads < 256)
         block_size = Vec3i(x_res, y_res, 1);
     Vec3i grid_size(int_div_up(x_res, block_size.x), int_div_up(y_res, block_size.y), 1);
     return {grid_size, block_size};
 }
 
-template <typename T> std::tuple<T, T, T> meshgrid(const T &x, const T &y, const T &z) {
+template <typename T> std::tuple<T, T, T> meshgrid3d(const T &x, const T &y, const T &z) {
     uint32_t sizes[3] = { (uint32_t) x.size(), (uint32_t) y.size(), (uint32_t) z.size() };
     dr::Array<T, 3> args(x, y, z);
     uint32_t size               = sizes[0] * sizes[1] * sizes[2];
     dr::uint32_array_t<T> index = dr::arange<dr::uint32_array_t<T>>(size);
     dr::Array<T, 3> result;
     for (size_t i = 0; i < 3; i++) {
         size         = size / sizes[i];
@@ -58,15 +58,15 @@
     using Vector3f = dr::Array<Float, 3>;
 
     // The implementation follows the code in https://github.com/scikit-fmm/scikit-fmm
     ScalarVector3i shape_in(
         init_distance.shape()[0], init_distance.shape()[1], init_distance.shape()[2]);
     ScalarVector3i shape = shape_in + 2 * BORDER_SIZE;
 
-    auto [z, y, x] = meshgrid(
+    auto [z, y, x] = meshgrid3d(
         dr::arange<Int32>(shape[0]), dr::arange<Int32>(shape[1]), dr::arange<Int32>(shape[2]));
     Vector3i coord(x, y, z);
 
     Vector3f ldistance(dr::Infinity<Float>);
 
     // Assume SDF is in [0,1]
     Bool active = dr::all((coord >= BORDER_SIZE) & (coord < shape - BORDER_SIZE));
@@ -300,17 +300,17 @@
         cuda_load_kernels();
 
     auto [distance, frozen] = initialize_distance(init_distance);
     dr::eval(distance, frozen);
     fast_sweep<Float>(distance, frozen);
 
     // Remove border passing and multiply by sign of the input
-    auto [z, y, x] = meshgrid(dr::arange<Int32>(init_distance.shape()[0]) + BORDER_SIZE,
-                              dr::arange<Int32>(init_distance.shape()[1]) + BORDER_SIZE,
-                              dr::arange<Int32>(init_distance.shape()[2]) + BORDER_SIZE);
+    auto [z, y, x] = meshgrid3d(dr::arange<Int32>(init_distance.shape()[0]) + BORDER_SIZE,
+                                dr::arange<Int32>(init_distance.shape()[1]) + BORDER_SIZE,
+                                dr::arange<Int32>(init_distance.shape()[2]) + BORDER_SIZE);
     Float result   = dr::gather<Float64>(
         distance.array(),
         z * distance.shape()[0] * distance.shape()[1] + y * distance.shape()[0] + x);
     return dr::Tensor<Float>(result * dr::sign(init_distance), 3, init_distance.shape().data());
 }
 
 template dr::Tensor<dr::CUDAArray<float>> redistance(const dr::Tensor<dr::CUDAArray<float>> &);
```

### Comparing `fastsweep-0.1.1/src/fastsweep.egg-info/PKG-INFO` & `fastsweep-0.1.2/src/fastsweep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastsweep
-Version: 0.1.1
+Version: 0.1.2
 Summary: Eikonal solver using parallel fast sweeping
 Home-page: https://github.com/rgl-epfl/fastsweep
 Author: Delio Vicini
 Author-email: delio.vicini@gmail.com
 License: BSD
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `fastsweep-0.1.1/src/fastsweep.egg-info/SOURCES.txt` & `fastsweep-0.1.2/src/fastsweep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.1/src/main.cpp` & `fastsweep-0.1.2/src/main.cpp`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.1/src/tests/test_redistancing.py` & `fastsweep-0.1.2/src/tests/test_redistancing.py`

 * *Files identical despite different names*

