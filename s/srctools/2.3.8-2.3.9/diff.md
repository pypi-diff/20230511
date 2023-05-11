# Comparing `tmp/srctools-2.3.8.tar.gz` & `tmp/srctools-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srctools-2.3.8.tar", last modified: Sun Jan  8 07:48:34 2023, max compression
+gzip compressed data, was "srctools-2.3.9.tar", last modified: Thu Jan 19 06:44:11 2023, max compression
```

## Comparing `srctools-2.3.8.tar` & `srctools-2.3.9.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:48:34.486738 srctools-2.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-01-08 07:48:22.000000 srctools-2.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-01-08 07:48:22.000000 srctools-2.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-01-08 07:48:34.486738 srctools-2.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-01-08 07:48:22.000000 srctools-2.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-01-08 07:48:22.000000 srctools-2.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-08 07:48:34.486738 srctools-2.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-01-08 07:48:22.000000 srctools-2.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:48:34.470737 srctools-2.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:48:34.474738 srctools-2.3.8/src/libsquish/
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/alpha.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/alpha.h
--rw-r--r--   0 runner    (1001) docker     (123)    14421 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/clusterfit.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/clusterfit.h
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/colourblock.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/colourblock.h
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/colourfit.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/colourfit.h
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/colourset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/colourset.h
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/config.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:48:34.474738 srctools-2.3.8/src/libsquish/extra/
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/extra/squishgen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/extra/squishpng.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/extra/squishtest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/maths.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/maths.h
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/rangefit.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/rangefit.h
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/simd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/simd_float.h
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/simd_sse.h
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/simd_ve.h
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/singlecolourfit.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/singlecolourfit.h
--rw-r--r--   0 runner    (1001) docker     (123)    42650 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/singlecolourlookup.inl
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/squish.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-01-08 07:48:22.000000 srctools-2.3.8/src/libsquish/squish.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:48:34.474738 srctools-2.3.8/src/quickhull/
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-01-08 07:48:22.000000 srctools-2.3.8/src/quickhull/ConvexHull.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-01-08 07:48:22.000000 srctools-2.3.8/src/quickhull/HalfEdgeMesh.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-01-08 07:48:22.000000 srctools-2.3.8/src/quickhull/MathUtils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19273 2023-01-08 07:48:22.000000 srctools-2.3.8/src/quickhull/QuickHull.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-01-08 07:48:22.000000 srctools-2.3.8/src/quickhull/QuickHull.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:48:34.478738 srctools-2.3.8/src/quickhull/Structs/
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-01-08 07:48:22.000000 srctools-2.3.8/src/quickhull/Structs/Mesh.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-01-08 07:48:22.000000 srctools-2.3.8/src/quickhull/Structs/Plane.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-01-08 07:48:22.000000 srctools-2.3.8/src/quickhull/Structs/Pool.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-01-08 07:48:22.000000 srctools-2.3.8/src/quickhull/Structs/Ray.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-01-08 07:48:22.000000 srctools-2.3.8/src/quickhull/Structs/Vector3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-01-08 07:48:22.000000 srctools-2.3.8/src/quickhull/Structs/VertexDataSource.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:48:34.478738 srctools-2.3.8/src/quickhull/Tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10053 2023-01-08 07:48:22.000000 srctools-2.3.8/src/quickhull/Tests/QuickHullTests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-01-08 07:48:22.000000 srctools-2.3.8/src/quickhull/Tests/QuickHullTests.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-08 07:48:22.000000 srctools-2.3.8/src/quickhull/Tests/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:48:34.482738 srctools-2.3.8/src/srctools/
--rw-r--r--   0 runner    (1001) docker     (123)    17566 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30432 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/_class_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    33660 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/_cy_vtf_readwrite.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    15293 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/_engine_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    23788 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/_fgd_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/_math.pxd
--rw-r--r--   0 runner    (1001) docker     (123)   103694 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/_math.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    28662 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/_py_vtf_readwrite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:48:34.482738 srctools-2.3.8/src/srctools/_pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/_pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/_pyinstaller/hook-srctools.py
--rw-r--r--   0 runner    (1001) docker     (123)    37318 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/_shaderdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    43277 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/_tokenizer.pyx
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-08 07:48:34.000000 srctools-2.3.8/src/srctools/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/binformat.py
--rw-r--r--   0 runner    (1001) docker     (123)   118218 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/bsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/cmdseq.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    95296 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/dmx.py
--rw-r--r--   0 runner    (1001) docker     (123)   107220 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/fgd.lzma
--rw-r--r--   0 runner    (1001) docker     (123)    84506 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/fgd.py
--rw-r--r--   0 runner    (1001) docker     (123)    26480 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/filesys.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/game.py
--rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/instancing.py
--rw-r--r--   0 runner    (1001) docker     (123)    50001 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/keyvalues.py
--rw-r--r--   0 runner    (1001) docker     (123)    16048 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    96112 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    25066 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/mdl.py
--rw-r--r--   0 runner    (1001) docker     (123)    54979 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/packlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/particles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/property_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/quickhull.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:48:34.486738 srctools-2.3.8/src/srctools/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/scripts/collapse_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/scripts/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/scripts/dump_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/scripts/dump_proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/scripts/find_deps.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/scripts/make_model_folders.py
--rw-r--r--   0 runner    (1001) docker     (123)    27231 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/smd.py
--rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/sndscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/surfaceprop.py
--rw-r--r--   0 runner    (1001) docker     (123)    27376 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/vec.py
--rw-r--r--   0 runner    (1001) docker     (123)   117717 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/vmf.py
--rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/vmt.py
--rw-r--r--   0 runner    (1001) docker     (123)    25676 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/vpk.py
--rw-r--r--   0 runner    (1001) docker     (123)    37961 2023-01-08 07:48:22.000000 srctools-2.3.8/src/srctools/vtf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 07:48:34.482738 srctools-2.3.8/src/srctools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-01-08 07:48:34.000000 srctools-2.3.8/src/srctools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-01-08 07:48:34.000000 srctools-2.3.8/src/srctools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-08 07:48:34.000000 srctools-2.3.8/src/srctools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-01-08 07:48:34.000000 srctools-2.3.8/src/srctools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-08 07:48:34.000000 srctools-2.3.8/src/srctools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-08 07:48:34.000000 srctools-2.3.8/src/srctools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 06:44:11.995847 srctools-2.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-01-19 06:43:58.000000 srctools-2.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-01-19 06:43:58.000000 srctools-2.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-01-19 06:44:11.995847 srctools-2.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-01-19 06:43:58.000000 srctools-2.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-01-19 06:43:58.000000 srctools-2.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-19 06:44:11.995847 srctools-2.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-01-19 06:43:58.000000 srctools-2.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 06:44:11.979846 srctools-2.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 06:44:11.983847 srctools-2.3.9/src/libsquish/
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/alpha.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/alpha.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14421 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/clusterfit.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/clusterfit.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/colourblock.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/colourblock.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/colourfit.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/colourfit.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/colourset.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/colourset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/config.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 06:44:11.983847 srctools-2.3.9/src/libsquish/extra/
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/extra/squishgen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/extra/squishpng.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/extra/squishtest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/maths.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/maths.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/rangefit.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/rangefit.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/simd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/simd_float.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/simd_sse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/simd_ve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/singlecolourfit.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/singlecolourfit.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42650 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/singlecolourlookup.inl
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/squish.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-01-19 06:43:58.000000 srctools-2.3.9/src/libsquish/squish.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 06:44:11.983847 srctools-2.3.9/src/quickhull/
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-01-19 06:43:58.000000 srctools-2.3.9/src/quickhull/ConvexHull.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-01-19 06:43:58.000000 srctools-2.3.9/src/quickhull/HalfEdgeMesh.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-01-19 06:43:58.000000 srctools-2.3.9/src/quickhull/MathUtils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19273 2023-01-19 06:43:58.000000 srctools-2.3.9/src/quickhull/QuickHull.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-01-19 06:43:58.000000 srctools-2.3.9/src/quickhull/QuickHull.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 06:44:11.987847 srctools-2.3.9/src/quickhull/Structs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-01-19 06:43:58.000000 srctools-2.3.9/src/quickhull/Structs/Mesh.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-01-19 06:43:58.000000 srctools-2.3.9/src/quickhull/Structs/Plane.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-01-19 06:43:58.000000 srctools-2.3.9/src/quickhull/Structs/Pool.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-01-19 06:43:58.000000 srctools-2.3.9/src/quickhull/Structs/Ray.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-01-19 06:43:58.000000 srctools-2.3.9/src/quickhull/Structs/Vector3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-01-19 06:43:58.000000 srctools-2.3.9/src/quickhull/Structs/VertexDataSource.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 06:44:11.987847 srctools-2.3.9/src/quickhull/Tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10053 2023-01-19 06:43:58.000000 srctools-2.3.9/src/quickhull/Tests/QuickHullTests.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-01-19 06:43:58.000000 srctools-2.3.9/src/quickhull/Tests/QuickHullTests.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-19 06:43:58.000000 srctools-2.3.9/src/quickhull/Tests/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 06:44:11.991847 srctools-2.3.9/src/srctools/
+-rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30431 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/_class_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33660 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/_cy_vtf_readwrite.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    25894 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/_engine_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23767 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/_fgd_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/_math.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)   103695 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/_math.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    28662 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/_py_vtf_readwrite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 06:44:11.995847 srctools-2.3.9/src/srctools/_pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/_pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/_pyinstaller/hook-srctools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37318 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/_shaderdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43277 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/_tokenizer.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-19 06:44:11.000000 srctools-2.3.9/src/srctools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/binformat.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121931 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/bsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/cmdseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95099 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/dmx.py
+-rw-r--r--   0 runner    (1001) docker     (123)   839927 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/fgd.lzma
+-rw-r--r--   0 runner    (1001) docker     (123)    85509 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/fgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26480 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/filesys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22000 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/instancing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49792 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/keyvalues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16048 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96107 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25071 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/mdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54890 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/packlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/property_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/quickhull.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 06:44:11.995847 srctools-2.3.9/src/srctools/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/scripts/collapse_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/scripts/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/scripts/dump_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/scripts/dump_proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/scripts/find_deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/scripts/make_model_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27231 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/smd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/sndscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/surfaceprop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27376 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117804 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/vmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/vmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25780 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/vpk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37964 2023-01-19 06:43:58.000000 srctools-2.3.9/src/srctools/vtf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 06:44:11.995847 srctools-2.3.9/src/srctools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-01-19 06:44:11.000000 srctools-2.3.9/src/srctools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-01-19 06:44:11.000000 srctools-2.3.9/src/srctools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 06:44:11.000000 srctools-2.3.9/src/srctools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-01-19 06:44:11.000000 srctools-2.3.9/src/srctools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-19 06:44:11.000000 srctools-2.3.9/src/srctools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-19 06:44:11.000000 srctools-2.3.9/src/srctools.egg-info/top_level.txt
```

### Comparing `srctools-2.3.8/LICENSE` & `srctools-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/PKG-INFO` & `srctools-2.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srctools
-Version: 2.3.8
+Version: 2.3.9
 Summary: Modules for working with Valve's Source Engine file formats.
 Author-email: TeamSpen210 <spencerb21@live.com>
 License: MIT
 Project-URL: source, https://github.com/TeamSpen210/srctools
 Keywords: Valve,Source Engine
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
```

### Comparing `srctools-2.3.8/README.md` & `srctools-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/pyproject.toml` & `srctools-2.3.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -91,21 +91,14 @@
 	]
 stubPath = "src/"   # Use our module for stubs.
 # We want to do conversions when setting.
 reportPropertyTypeMismatch = false
 pythonVersion = "3.8"
 strictParameterNoneValue = false
 
-[tool.pytest.ini_options]
-filterwarnings = [
-	# Any warnings in srctools = error.
-	"error:::srctools[.*]",
-	"error:::tests[.*]",  # Same for tests themselves.
-]
-
 [tool.mypy]
 warn_unused_ignores = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_no_return = true
 
 disallow_incomplete_defs = true
```

### Comparing `srctools-2.3.8/setup.py` & `srctools-2.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/alpha.cpp` & `srctools-2.3.9/src/libsquish/alpha.cpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/alpha.h` & `srctools-2.3.9/src/libsquish/alpha.h`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/clusterfit.cpp` & `srctools-2.3.9/src/libsquish/clusterfit.cpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/clusterfit.h` & `srctools-2.3.9/src/libsquish/clusterfit.h`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/colourblock.cpp` & `srctools-2.3.9/src/libsquish/colourblock.cpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/colourblock.h` & `srctools-2.3.9/src/libsquish/colourblock.h`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/colourfit.cpp` & `srctools-2.3.9/src/libsquish/colourfit.cpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/colourfit.h` & `srctools-2.3.9/src/libsquish/colourfit.h`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/colourset.cpp` & `srctools-2.3.9/src/libsquish/colourset.cpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/colourset.h` & `srctools-2.3.9/src/libsquish/colourset.h`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/config.h` & `srctools-2.3.9/src/libsquish/config.h`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/extra/squishgen.cpp` & `srctools-2.3.9/src/libsquish/extra/squishgen.cpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/extra/squishpng.cpp` & `srctools-2.3.9/src/libsquish/extra/squishpng.cpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/extra/squishtest.cpp` & `srctools-2.3.9/src/libsquish/extra/squishtest.cpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/maths.cpp` & `srctools-2.3.9/src/libsquish/maths.cpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/maths.h` & `srctools-2.3.9/src/libsquish/maths.h`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/rangefit.cpp` & `srctools-2.3.9/src/libsquish/rangefit.cpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/rangefit.h` & `srctools-2.3.9/src/libsquish/rangefit.h`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/simd.h` & `srctools-2.3.9/src/libsquish/simd.h`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/simd_float.h` & `srctools-2.3.9/src/libsquish/simd_float.h`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/simd_sse.h` & `srctools-2.3.9/src/libsquish/simd_sse.h`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/simd_ve.h` & `srctools-2.3.9/src/libsquish/simd_ve.h`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/singlecolourfit.cpp` & `srctools-2.3.9/src/libsquish/singlecolourfit.cpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/singlecolourfit.h` & `srctools-2.3.9/src/libsquish/singlecolourfit.h`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/singlecolourlookup.inl` & `srctools-2.3.9/src/libsquish/singlecolourlookup.inl`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/squish.cpp` & `srctools-2.3.9/src/libsquish/squish.cpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/libsquish/squish.h` & `srctools-2.3.9/src/libsquish/squish.h`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/quickhull/ConvexHull.hpp` & `srctools-2.3.9/src/quickhull/ConvexHull.hpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/quickhull/HalfEdgeMesh.hpp` & `srctools-2.3.9/src/quickhull/HalfEdgeMesh.hpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/quickhull/MathUtils.hpp` & `srctools-2.3.9/src/quickhull/MathUtils.hpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/quickhull/QuickHull.cpp` & `srctools-2.3.9/src/quickhull/QuickHull.cpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/quickhull/QuickHull.hpp` & `srctools-2.3.9/src/quickhull/QuickHull.hpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/quickhull/Structs/Mesh.hpp` & `srctools-2.3.9/src/quickhull/Structs/Mesh.hpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/quickhull/Structs/Plane.hpp` & `srctools-2.3.9/src/quickhull/Structs/Plane.hpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/quickhull/Structs/Pool.hpp` & `srctools-2.3.9/src/quickhull/Structs/Pool.hpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/quickhull/Structs/Vector3.hpp` & `srctools-2.3.9/src/quickhull/Structs/Vector3.hpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/quickhull/Structs/VertexDataSource.hpp` & `srctools-2.3.9/src/quickhull/Structs/VertexDataSource.hpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/quickhull/Tests/QuickHullTests.cpp` & `srctools-2.3.9/src/quickhull/Tests/QuickHullTests.cpp`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/__init__.py` & `srctools-2.3.9/src/srctools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,14 +258,15 @@
         """EmptyMapping does not have any keys."""
         return False
 
     @overload
     def get(self, key: Any) -> None: ...
     @overload
     def get(self, key: Any, default: ValT) -> ValT: ...
+
     def get(self, key: Any, default: Optional[ValT]=None) -> Optional[ValT]:
         """get() always returns the default item."""
         return default
 
     def __bool__(self) -> bool:
         """EmptyMapping is falsey."""
         return False
@@ -291,24 +292,26 @@
         return EmptyValuesView
 
     # Mutable functions
     @overload
     def setdefault(self, key: Any) -> None: ...
     @overload
     def setdefault(self, key: Any, default: ValT) -> ValT: ...
+
     def setdefault(self, key: Any, default: Optional[ValT] = None) -> Optional[ValT]:
         """setdefault() always returns the default item, but does not store it."""
         return default
 
     @overload
     def update(self, __m: _SupportsKeysAndGetItem, **kwargs: Any) -> None: ...
     @overload
     def update(self, __m: Iterable[Tuple[Any, Any]], **kwargs: Any) -> None: ...
     @overload
     def update(self, **kwargs: Any) -> None: ...
+
     def update(self, *args: Any, **kargs: Any) -> None:
         """Runs {}.update() on arguments."""
         # Check arguments are correct, and raise appropriately.
         # Also consume args[0] if an iterator - this raises if args > 1.
         {}.update(*args, **kargs)
 
     __marker: Final[Any] = object()
@@ -457,14 +460,15 @@
     clears the file.
     """
     @overload
     def __init__(
         self: 'AtomicWriter[io.BufferedWriter]', filename: StringPath,
         is_bytes: Literal[True],
     ) -> None: ...
+
     @overload
     def __init__(
         self: 'AtomicWriter[io.TextIOWrapper]', filename: StringPath,
         is_bytes: Literal[False]=False, encoding: str='utf8',
     ) -> None: ...
 
     def __init__(self, filename: StringPath, is_bytes: bool=False, encoding: str='utf8') -> None:
```

### Comparing `srctools-2.3.8/src/srctools/_class_resources.py` & `srctools-2.3.9/src/srctools/_class_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,14 @@
     """Inherits from func_button, but doesn't always use 'sounds'."""
     if conv_int(ent['spawnflags']) & 1024:  # USE_ACTIVATES
         yield button_sound(ent['sounds'])
     yield button_sound(ent['locked_sound'])
     yield button_sound(ent['unlocked_sound'])
 
 
-
 @cls_func
 def color_correction(ctx: ResourceCtx, ent: Entity) -> ResGen:
     """Pack the color correction file."""
     yield Resource(ent['filename'], FileType.GENERIC)
 
 
 # Index->sound lists for CBasePlatTrain in HL:Source.
@@ -447,15 +446,15 @@
     ("ar2.mdl", "ar2.mdl"),
     ("rockets.mdl", "rockets.mdl"),
     ("buckshot.mdl", "buckshot.mdl"),
     ("grenade.mdl", "grenade.mdl"),
     # Valve reused models for these three.
     ("smg1.mdl", "357.mdl"),
     ("smg1.mdl", "xbow.mdl"),
-    ("ar2.mdl",  "ar2alt.mdl"),
+    ("ar2.mdl", "ar2alt.mdl"),
 
     ("smg2.mdl", "smg2.mdl"),
     # Two added by mapbase.
     ("", "slam.mdl"),
     ("", "empty.mdl"),
 ]
 
@@ -566,14 +565,15 @@
     Resource.snd("NPC_Antlion.PoisonBurstScream"),
     Resource.snd("NPC_Antlion.PoisonBurstScreamSubmerged"),
     Resource.snd("NPC_Antlion.PoisonBurstExplode"),
     Resource.snd("NPC_Antlion.PoisonShoot"),
     Resource.snd("NPC_Antlion.PoisonBall"),
 ]
 
+
 @cls_func
 def npc_antlion(ctx: ResourceCtx, ent: Entity) -> ResGen:
     """Antlions require different resources for the worker version."""
     ez_variant = conv_int(ent['ezvariant'])
     spawnflags = conv_int(ent['spawnflags'])
     if spawnflags & (1 << 18):  # Is worker?
         if ez_variant == EZ_VARIANT_BLOOD:
```

### Comparing `srctools-2.3.8/src/srctools/_cy_vtf_readwrite.pyx` & `srctools-2.3.9/src/srctools/_cy_vtf_readwrite.pyx`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/_fgd_helpers.py` & `srctools-2.3.9/src/srctools/_fgd_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Implemenations of specific code for each FGD helper type."""
 from typing import (
-    TYPE_CHECKING, ClassVar, Collection, Iterable, Iterator, List, Optional, Tuple, Type,
-    TypeVar, Union,
+    ClassVar, Collection, Iterable, Iterator, List, Optional, Tuple, Type, TypeVar, Union,
 )
 
 import attrs
 
 from srctools.fgd import EntityDef, Helper, HelperTypes
 from srctools.math import Vec, parse_vec_str
 
@@ -321,15 +320,14 @@
         if isinstance(color, str):
             try:
                 r, g, b = color.split()
                 color = (float(r), float(g), float(b))
             except ValueError:
                 pass
 
-
         return cls(fov, nearz, farz, color, pitch)
 
     def export(self) -> List[str]:
         """Export back out frustrum() arguments."""
 
         if isinstance(self.color, tuple):
             color = '{:g} {:g} {:g}'.format(*self.color)
@@ -594,15 +592,14 @@
 
 
 class HelperModelLight(HelperModel):
     """Special model helper, with inverted pitch."""
     TYPE: ClassVar[HelperTypes] = HelperTypes.MODEL_NEG_PITCH
 
 
-
 class HelperInstance(Helper):
     """Specialized helper for func_instance."""
     TYPE: ClassVar[HelperTypes] = HelperTypes.ENT_INSTANCE
 
 
 class HelperDecal(Helper):
     """Specialized helper for infodecal."""
```

### Comparing `srctools-2.3.8/src/srctools/_math.pxd` & `srctools-2.3.9/src/srctools/_math.pxd`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/_math.pyx` & `srctools-2.3.9/src/srctools/_math.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1659,15 +1659,15 @@
         return (
             self.val.x * oth.x +
             self.val.y * oth.y +
             self.val.z * oth.z
         )
 
 
-    def join(self, delim: str=' ') -> str:
+    def join(self, delim: str=', ') -> str:
         """Return a string with all numbers joined by the passed delimiter.
 
         This strips off the .0 if no decimal portion exists.
         """
         return _join_triple(&self.val, delim)
 
     def __str__(self) -> str:
```

### Comparing `srctools-2.3.8/src/srctools/_py_vtf_readwrite.py` & `srctools-2.3.9/src/srctools/_py_vtf_readwrite.py`

 * *Files 0% similar despite different names*

```diff
@@ -700,16 +700,16 @@
                 block_off+8, block_wid,
                 block_x, block_y,
             )
             # Now add on the real alpha values.
             for off in range(8):
                 byte = data[block_off + off]
                 y, x = divmod(off * 2, 4)
-                pos = 16 * block_wid * (4 * block_y + y) + 4 * (4 * block_x  + x)
-                # Combine the values twice so we evenly cover the whole range.
+                pos = 16 * block_wid * (4 * block_y + y) + 4 * (4 * block_x + x)
+                # Combine the values twice, so we evenly cover the whole range.
                 pixels[pos + 3] = byte & 0b00001111 | (byte & 0b00001111) << 4
                 pixels[pos + 7] = byte & 0b11110000 | (byte & 0b11110000) >> 4
 
 
 def load_dxt5(pixels: Array, data: bytes, width: int, height: int) -> None:
     """Load compressed DXT5 data."""
     if width < 4 or height < 4:
```

### Comparing `srctools-2.3.8/src/srctools/_pyinstaller/hook-srctools.py` & `srctools-2.3.9/src/srctools/_pyinstaller/hook-srctools.py`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/_shaderdb.py` & `srctools-2.3.9/src/srctools/_shaderdb.py`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/_tokenizer.pyx` & `srctools-2.3.9/src/srctools/_tokenizer.pyx`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/binformat.py` & `srctools-2.3.9/src/srctools/binformat.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,39 +108,50 @@
         read_nullstr(file, off, encoding)
         for off in offsets
     ]
     file.seek(pos)
     return arr
 
 
-def read_array(fmt: str, data: bytes) -> List[int]:
+def read_array(fmt: Union[str, Struct], data: bytes) -> List[int]:
     """Read a buffer containing a stream of integers.
 
     The format string should be one of the integer format characters, optionally prefixed by an
      endianness indicator. As many integers as possible will then be read from the data.
     """
+
+    if isinstance(fmt, Struct):
+        # Since `struct.Struct` does not support writing arrays, we'll have to rebuild `fmt`.
+        # Turn it back into its original format string so we can figure out what it held.
+        fmt = fmt.format
+
     if len(fmt) == 2:
         endianness = fmt[0]
         fmt = fmt[1]
     else:
         endianness = ''
     try:
         item_size = SIZES[fmt]
     except KeyError:
         raise ValueError(f'Unknown format character {fmt!r}!')
     count = len(data) // item_size
     return list(Struct(endianness + fmt * count).unpack_from(data))
 
 
-def write_array(fmt: str, data: Collection[int]) -> bytes:
+def write_array(fmt: Union[str, Struct], data: Collection[int]) -> bytes:
     """Build a packed array of integers.
 
     The format string should be one of the integer format characters, optionally prefixed by an
     endianness indicator. The integers in the data will then be packed into a bytes buffer and returned.
      """
+    if isinstance(fmt, Struct):
+        # Since `struct.Struct` does not support writing arrays, we'll have to rebuild `fmt`.
+        # Turn it back into its original format string so we can figure out what it held.
+        fmt = fmt.format
+
     if len(fmt) == 2:
         endianness = fmt[0]
         fmt = fmt[1]
     else:
         endianness = ''
 
     return Struct(endianness + fmt * len(data)).pack(*data)
```

### Comparing `srctools-2.3.8/src/srctools/bsp.py` & `srctools-2.3.9/src/srctools/bsp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Read and write parts of Source BSP files.
 
 Data from a read BSP is lazily parsed when each section is accessed.
 """
 from typing import (
     Any, Callable, ClassVar, Dict, Generator, Generic, Hashable, Iterator, List, Mapping,
-    Optional, Sequence, Set, Tuple, Type, TypeVar, Union, cast, overload,
+    Optional, Sequence, Set, Tuple, Type, TypeVar, Union, cast, overload
 )
+from typing_extensions import TypedDict
 from enum import Enum, Flag
 from io import BytesIO
 from weakref import WeakKeyDictionary
 from zipfile import ZipFile
 import contextlib
 import inspect
 import itertools
@@ -97,14 +98,15 @@
     CS_GO = 21
     DEAR_ESTHER = 21
     STANLEY_PARABLE = 21
 
     INFRA = 22
     DOTA2 = 22
     CONTAGION = 23
+    CHAOSSOURCE = 25  # Chaos' limit increased BSPs.
 
     DESOLATION_OLD = 42  # Old version.
     VITAMINSOURCE = 43  # Desolation's expanded map format.
 
     def __eq__(self, other: object) -> bool:
         """Versions are equal to their integer value."""
         return self.value == other
@@ -217,14 +219,92 @@
     MAP_FLAGS = 59
     OVERLAY_FADES = 60
     OVERLAY_SYSTEM_LEVELS = 61
     PHYSLEVEL = 62
     DISP_MULTIBLEND = 63
 
 
+class LumpDataLayout(TypedDict):
+    """Container dictionary for lump layouts."""
+    FACE: struct.Struct
+    FACEID: struct.Struct
+    EDGE: struct.Struct
+    PRIMITIVE: struct.Struct
+    PRIMINDEX: struct.Struct
+    NODE: struct.Struct
+    LEAF: struct.Struct
+    LEAFFACE: struct.Struct
+    LEAFBRUSH: struct.Struct
+    LEAF_AREA_OFFSET: int
+    LEAFWATERDATA: struct.Struct
+    BRUSHSIDE: struct.Struct
+    STATICPROPLEAF: struct.Struct
+
+
+# Version specific lump data layout description
+LUMP_LAYOUT_STANDARD: LumpDataLayout = {
+    "FACE":             struct.Struct('<H??i4h4sif5iHHI'),
+    "FACEID":           struct.Struct('<H'),
+    "EDGE":             struct.Struct('<HH'),
+    "PRIMITIVE":        struct.Struct('<HHHHH'),
+    "PRIMINDEX":        struct.Struct('<H'),
+    "NODE":             struct.Struct('<iii6hHHh2x'),
+    "LEAF":             struct.Struct('<ihh6h4Hh2x'),  # Version 1
+    "LEAFFACE":         struct.Struct('<H'),
+    "LEAFBRUSH":        struct.Struct('<H'),
+    "LEAF_AREA_OFFSET": 7,
+    "LEAFWATERDATA":    struct.Struct('<ffH2x'),
+    "BRUSHSIDE":        struct.Struct('<HhhH'),
+    "STATICPROPLEAF":   struct.Struct('<H'),
+}
+
+
+LUMP_LAYOUT_V19: LumpDataLayout = {
+    # See https://github.com/python/mypy/issues/9408
+    **LUMP_LAYOUT_STANDARD,  # type: ignore[misc]
+    "LEAF":             struct.Struct('<ihh6h4Hh24s2x'), # Version 0
+}
+
+LUMP_LAYOUT_INFRA: LumpDataLayout = {
+    **LUMP_LAYOUT_STANDARD,  # type: ignore[misc]
+    # INFRA seems to have a different lump. It's 16 bytes, it seems to be:
+    # char type;
+    # int first_ind, ind_count;
+    # short vert_ind, vert_count;
+    # Then the type is promoted to int for structure alignment.
+    "PRIMITIVE": struct.Struct('<IIIHH'),
+}
+
+LUMP_LAYOUT_VITAMIN: LumpDataLayout = {
+    **LUMP_LAYOUT_STANDARD,  # type: ignore[misc]
+    "LEAF": struct.Struct('<ihh6I4HhBx'),
+    "FACE": struct.Struct('<5i4iB3x'),
+    "BRUSHSIDE": struct.Struct('<IIhBB'),
+    "NODE": struct.Struct('<iii6iHHh2x'),
+}
+
+# https://chaosinitiative.github.io/Wiki/docs/Reference/bsp-v25/
+LUMP_LAYOUT_CHAOS: LumpDataLayout = {
+    **LUMP_LAYOUT_STANDARD,  # type: ignore[misc]
+    "FACE":             struct.Struct('<I??xx5i4sif5i3I'),
+    "FACEID":           struct.Struct('<I'),
+    "EDGE":             struct.Struct('<II'),
+    "PRIMITIVE":        struct.Struct('<IIIII'),
+    "PRIMINDEX":        struct.Struct('<I'),
+    "NODE":             struct.Struct('<iii6fIIhxx'),
+    "LEAF":             struct.Struct('<iii6f4Ii'),  # Version 2
+    "LEAFFACE":         struct.Struct('<I'),
+    "LEAFBRUSH":        struct.Struct('<I'),
+    "LEAF_AREA_OFFSET": 17,
+    "LEAFWATERDATA":    struct.Struct('<ffI'),
+    "BRUSHSIDE":        struct.Struct('<IiiHxx'),
+    "STATICPROPLEAF":   struct.Struct('<I'),
+}
+
+
 LUMP_COUNT = max(lump.value for lump in BSP_LUMPS) + 1  # 64 normally
 
 # Special-case the packfile lump, put it at the end.
 # This way the BSP can be opened by generic zip programs.
 LUMP_WRITE_ORDER = list(BSP_LUMPS)
 LUMP_WRITE_ORDER.remove(BSP_LUMPS.PAKFILE)
 LUMP_WRITE_ORDER.append(BSP_LUMPS.PAKFILE)
@@ -318,14 +398,16 @@
     # Source 2013, also appears with version 7 but is identical.
     # Based on v6, adds lightmapped props.
     # Despite the actual versions, more like v6.
     V_LIGHTMAP_v7 = (7, 72)
     V_LIGHTMAP_v10 = (10, 72)
     V_LIGHTMAP_MESA = (11, 80, 'Mesa')  # Adds rendercolor to V10
 
+    V_CHAOS = (12, 80)  # Changes the leaf list from uint16 to uint32
+
     # V6_WNAME = (5, 188)  # adds targetname, used by The Ship and Bloody Good Time.
     UNKNOWN = (0, 0, 'unknown')  # Before prop is read.
     # All games should recognise this, so switch to this if set to unknown.
     DEFAULT = V5
 
     @property
     def is_lightmap(self) -> bool:
@@ -752,15 +834,15 @@
     size: int = 0
 
     @property
     def resolution(self) -> int:
         """Return the actual image size."""
         if self.size == 0:
             return 32
-        res =  2 ** (self.size - 1)
+        res = 2 ** (self.size - 1)
         assert isinstance(res, int), self.size
         return res
 
 
 @attrs.define(eq=False)
 class Overlay:
     """An overlay embedded in the map."""
@@ -1138,14 +1220,15 @@
     # Parsed lump -> func which remakes the raw data. Any = ParsedLump's T, but
     # that can't bind here.
     _save_funcs: ClassVar[Dict[
         Union[bytes, BSP_LUMPS],
         Callable[['BSP', Any], Union[bytes, Generator[bytes, None, None]]]
     ]] = {}
     version: Union[VERSIONS, int]
+    lump_layout: LumpDataLayout
 
     def __init__(self, filename: StringPath, version: Optional[VERSIONS] = None) -> None:
         self.filename = filename
         self.map_revision = -1  # The map's revision count
         self.lumps: Dict[BSP_LUMPS, Lump] = {}
         self._parsed_lumps: Dict[Union[bytes, BSP_LUMPS], Any] = {}
         self.game_lumps: Dict[bytes, GameLump] = {}
@@ -1157,14 +1240,17 @@
         self.out_comma_sep: Optional[bool] = None
         self.static_prop_version: StaticPropVersion = StaticPropVersion.UNKNOWN
         # This internally stores the texdata values texinfo refers to. Users
         # don't interact directly, instead they use the create_texinfo / texinfo.set()
         # methods that create the data as required.
         self._texdata: Dict[str, TexData] = {}
 
+        # lump_layout holds version specific struct formats for lumps
+        self.lump_layout = LUMP_LAYOUT_STANDARD
+        
         self.read()
 
     # The first lump is the main one this reads/writes to, any additional are simpler lumps it
     # reads and includes all the data for.
     pakfile: ParsedLump[ZipFile] = ParsedLump(BSP_LUMPS.PAKFILE)
     ents: ParsedLump[VMF] = ParsedLump(BSP_LUMPS.ENTITIES)
     textures: ParsedLump[List[str]] = ParsedLump(
@@ -1224,24 +1310,40 @@
                 raise ValueError('File is not a BSP file!')
 
             if self.version is None:
                 try:
                     self.version = VERSIONS(bsp_version)
                 except ValueError:
                     self.version = bsp_version
+                    LOGGER.warning(f'Unknown BSP Version \"{bsp_version}\"!')
             else:
                 if bsp_version != self.version:
                     raise ValueError(
                         f'Unexpected BSP version {self.version!r}, expected {bsp_version!r}!'
                     )
 
             if magic_name == VITAMIN_MAGIC and self.version is not VERSIONS.VITAMINSOURCE:
                 raise ValueError('VitaminSource uses a different version number.')
 
-            lump_offsets = {}
+            if self.version is VERSIONS.CHAOSSOURCE:
+                # Change the expected structure for lumps to fit chaos' increased limits
+                self.lump_layout = LUMP_LAYOUT_CHAOS
+            elif self.version is VERSIONS.VITAMINSOURCE:
+                # Change the expected structure for lumps to fit vitamin's rad new format
+                self.lump_layout = LUMP_LAYOUT_VITAMIN
+            elif self.version is VERSIONS.INFRA:
+                self.lump_layout = LUMP_LAYOUT_INFRA
+            elif self.version <= 19:
+                self.lump_layout = LUMP_LAYOUT_V19
+
+            lump_offsets: Dict[BSP_LUMPS, Tuple[int, int, int]] = {}
+            offset: int
+            length: int
+            version: int
+            uncomp_size: int
 
             # Read the index describing each BSP lump.
             for index in range(LUMP_COUNT):
                 # The 4th value here is originally the fourCC identity, but is
                 # instead used to indicate the unpacked size if compressed.
                 offset, length, version, uncomp_size = struct_read(HEADER_LUMP, file)
                 lump_id = BSP_LUMPS(index)
@@ -1267,43 +1369,40 @@
 
             game_lump = self.lumps[BSP_LUMPS.GAME_LUMP]
 
             self.game_lumps.clear()
 
             [lump_count] = struct.unpack_from('<i', game_lump.data)
             lump_offset = 4
-            gm_lump_offsets = {}
-            gm_lump_sizes = {}
+            gm_lump_offsets: Dict[bytes, Tuple[int, int]] = {}
+            gm_lump_sizes: Dict[bytes, int] = {}
             prev_game_lump = b''
             prev_lump_offset = 0
             for _ in range(lump_count):
                 game_lump_id: bytes
                 flags: int
                 glump_version: int
                 file_off: int
-                file_len: int
                 (
                     game_lump_id,
                     flags,
                     glump_version,
                     file_off,
                     uncomp_size,
                 ) = GameLump.ST.unpack_from(game_lump.data, lump_offset)
                 lump_offset += GameLump.ST.size
                 # The lump ID is backward..
                 game_lump_id = game_lump_id[::-1]
 
                 gm_lump_offsets[game_lump_id] = file_off, uncomp_size
 
-                # Determine the size of the lump by comparing offsets.
-                # This is necessary for compressed lumps, but still works
-                # normally. To allow this BSPs have an extra dummy entry with
-                # this ID which should have an offset value, but it's also
-                # just zero so it's useless. Skip that and use the size of the
-                # lump itself.
+                # Determine the size of the lump by comparing offsets. This is necessary for
+                # compressed lumps, but still works normally. To allow this BSPs have an extra
+                # dummy entry with this ID which should have an offset value, but it's also just
+                # zero and therefore useless. Skip that and use the size of the lump itself.
                 if game_lump_id == b'\x00\x00\x00\x00':
                     continue
 
                 if prev_game_lump:
                     gm_lump_sizes[prev_game_lump] = file_off - prev_lump_offset - 1
                 prev_game_lump = game_lump_id
                 prev_lump_offset = file_off
@@ -1642,15 +1741,15 @@
     def _lmp_write_vertexes(self, vertexes: List[Vec]) -> bytes:
         return b''.join([struct.pack('<fff', pos.x, pos.y, pos.z) for pos in vertexes])
 
     def _lmp_read_surfedges(self, edge_inds: bytes) -> Iterator[Edge]:
         verts: List[Vec] = self.vertexes
         edges = [
             Edge(verts[a], verts[b])
-            for a, b in struct.iter_unpack('<HH', self.lumps[BSP_LUMPS.EDGES].data)
+            for a, b in self.lump_layout['EDGE'].iter_unpack(self.lumps[BSP_LUMPS.EDGES].data)
         ]
         for [ind] in struct.iter_unpack('i', edge_inds):
             if ind < 0:  # If negative, the vertexes are reversed order.
                 yield edges[-ind].opposite
             else:
                 yield edges[ind]
 
@@ -1680,64 +1779,60 @@
                 ind = -add_edge(edge.opposite)
             else:
                 ind = add_edge(edge)
             surf_buf.write(struct.pack('i', ind))
 
         for edge in edges:
             assert not isinstance(edge, RevEdge), edge
-            edge_buf.write(struct.pack('<HH', add_vert(edge.a), add_vert(edge.b)))
+            edge_buf.write(self.lump_layout['EDGE'].pack(add_vert(edge.a), add_vert(edge.b)))
 
         self.lumps[BSP_LUMPS.EDGES].data = edge_buf.getvalue()
         return surf_buf.getvalue()
 
     def _lmp_read_primitives(self, data: bytes) -> Iterator['Primitive']:
         """Parse the primitives lumps."""
         if self.is_vitamin:
             # VitaminSource no longer uses primitives.
             return
 
         verts = list(map(Vec, struct.iter_unpack('<fff', self.lumps[BSP_LUMPS.PRIMVERTS].data)))
-        indices = read_array('<H', self.lumps[BSP_LUMPS.PRIMINDICES].data)
-        # INFRA seems to have a different lump. It's 16 bytes, it seems to be:
-        # char type;
-        # int first_ind, ind_count;
-        # short vert_ind, vert_count;
-        # Then the type is promoted to int for structure alignment.
-        fmt = '<IIIHH' if self.version is VERSIONS.INFRA else '<HHHHH'
+        indices = read_array(self.lump_layout['PRIMINDEX'], self.lumps[BSP_LUMPS.PRIMINDICES].data)
+
+        fmt = self.lump_layout['PRIMITIVE']
         for (
             prim_type,
             first_ind, ind_count,
             first_vert, vert_count,
-        ) in struct.iter_unpack(fmt, data):
+        ) in fmt.iter_unpack(data):
             yield Primitive(
                 prim_type,
                 indices[first_ind: first_ind + ind_count],
                 verts[first_vert: first_vert + vert_count],
             )
 
     def _lmp_write_primitives(self, prims: List['Primitive']) -> Iterator[bytes]:
         if self.is_vitamin:
             # VitaminSource no longer uses primitives.
             return
 
         verts: List[bytes] = []
         indices: List[int] = []
 
-        fmt = struct.Struct('<IIIHH' if self.version is VERSIONS.INFRA else '<HHHHH')
+        fmt = self.lump_layout['PRIMITIVE']
         for prim in prims:
             vert_loc = len(verts)
             index_loc = len(indices)
             verts += [struct.pack('<fff', pos.x, pos.y, pos.z) for pos in prim.verts]
             indices.extend(prim.indexed_verts)
             yield fmt.pack(
                 prim.is_tristrip,
                 index_loc, len(prim.indexed_verts),
                 vert_loc, len(prim.verts),
             )
-        self.lumps[BSP_LUMPS.PRIMINDICES].data = write_array('<H', indices)
+        self.lumps[BSP_LUMPS.PRIMINDICES].data = write_array(self.lump_layout['PRIMINDEX'], indices)
         self.lumps[BSP_LUMPS.PRIMVERTS].data = b''.join(verts)
 
     def _read_faces_common(self, data: bytes, orig_faces: Optional[List['Face']]) -> Iterator['Face']:
         """Read one of the faces arrays.
 
         For ORIG_FACES, _orig_faces is None and that entry is ignored.
         For the others, that is the parsed orig faces lump, which each face
@@ -1745,24 +1840,23 @@
         In VitaminSource, we only have the regular faces lump.
         """
         is_vitamin = self.is_vitamin
 
         # The non-original faces have the Hammer ID value, which is an array
         # in the same order. But some versions don't define it as anything...
         if orig_faces is not None or is_vitamin:
-            hammer_ids = read_array('<H', self.lumps[BSP_LUMPS.FACEIDS].data)
+            hammer_ids = read_array(self.lump_layout['FACEID'], self.lumps[BSP_LUMPS.FACEIDS].data)
         else:
             hammer_ids = []
 
         hammer_id: Optional[int]
 
-        for i, face_data in enumerate(struct.iter_unpack(
-            '<5i4iB3x' if self.is_vitamin else '<H??i4h4sif5iHHI',
-            data,
-        )):
+        for i, face_data in enumerate(
+            self.lump_layout['FACE'].iter_unpack(data),
+        ):
             if is_vitamin:
                 (
                     plane_num,
                     texinfo_ind,
                     dispinfo,
                     first_edge, num_edges,
                     lightmap_mins_x, lightmap_mins_y,
@@ -1885,16 +1979,15 @@
                 prim_count = len(face.primitives)
                 if prim_count > 0x7fff:
                     raise ValueError(f'Too many primitives: {prim_count} in {orig_ind}')
                 if not face.dynamic_shadows:
                     prim_count |= 0x8000
 
                 # noinspection PyProtectedMember
-                face_buf.write(struct.pack(
-                    '<H??i4h4sif5iHHI',
+                face_buf.write(self.lump_layout['FACE'].pack(
                     add_plane(face.plane),
                     face.same_dir_as_plane,
                     face.on_node,
                     add_edges(face.edges), len(face.edges),
                     texinfo,
                     face._dispinfo_ind,
                     face.surf_fog_volume_id,
@@ -1904,15 +1997,15 @@
                     *face.lightmap_mins, *face.lightmap_size,
                     orig_ind,
                     prim_count,
                     add_prims(face.primitives),
                     face.smoothing_groups,
                 ))
             if hammer_ids:
-                self.lumps[BSP_LUMPS.FACEIDS].data = write_array('<H', hammer_ids)
+                self.lumps[BSP_LUMPS.FACEIDS].data = write_array(self.lump_layout['FACEID'], hammer_ids)
         return face_buf.getvalue()
 
     def _lmp_read_orig_faces(self, data: bytes) -> Iterator['Face']:
         """Parse the unsplit faces lump."""
         if self.is_vitamin:
             return iter(())  # Unused
         else:
@@ -1956,21 +2049,21 @@
     def _lmp_read_brushes(self, data: bytes) -> Iterator['Brush']:
         """Parse brush definitions, along with the sides."""
         # The bevel param should be a bool, but randomly has other bits set?
         if self.is_vitamin:
             sides = [
                 BrushSide(self.planes[plane_num], self.texinfo[texinfo], dispinfo, bevel, extra)
                 for (plane_num, texinfo, dispinfo, bevel, extra)
-                in struct.iter_unpack('<IIhBB', self.lumps[BSP_LUMPS.BRUSHSIDES].data)
+                in self.lump_layout['BRUSHSIDE'].iter_unpack(self.lumps[BSP_LUMPS.BRUSHSIDES].data)
             ]
         else:
             sides = [
                 BrushSide(self.planes[plane_num], self.texinfo[texinfo], dispinfo, bool(bevel & 1), bevel & ~1)
                 for (plane_num, texinfo, dispinfo, bevel)
-                in struct.iter_unpack('<HhhH', self.lumps[BSP_LUMPS.BRUSHSIDES].data)
+                in self.lump_layout['BRUSHSIDE'].iter_unpack(self.lumps[BSP_LUMPS.BRUSHSIDES].data)
             ]
         for first_side, side_count, contents in struct.iter_unpack('<iii', data):
             yield Brush(BrushContents(contents), sides[first_side:first_side+side_count])
 
     def _lmp_write_brushes(self, brushes: List['Brush']) -> bytes:
         sides: List[BrushSide] = []
         add_plane = _find_or_insert(self.planes)
@@ -1982,76 +2075,67 @@
         for brush in brushes:
             brush_buf.write(struct.pack(
                 '<iii',
                 add_sides(brush.sides), len(brush.sides),
                 brush.contents.value,
             ))
 
+        side_struct = self.lump_layout['BRUSHSIDE']
         if self.is_vitamin:
             for side in sides:
-                side_struct = struct.Struct('<IIhBB')
                 sides_buf.write(side_struct.pack(
                     add_plane(side.plane),
                     add_texinfo(side.texinfo),
                     side._dispinfo,
                     side.is_bevel_plane,
                     side._unknown_bevel_bits,
                 ))
         else:
             for side in sides:
-                side_struct = struct.Struct('<HhhH')
                 sides_buf.write(side_struct.pack(
                     add_plane(side.plane),
                     add_texinfo(side.texinfo),
                     side._dispinfo,
                     side.is_bevel_plane | side._unknown_bevel_bits,
                 ))
         self.lumps[BSP_LUMPS.BRUSHSIDES].data = sides_buf.getvalue()
         return brush_buf.getvalue()
 
     def _lmp_read_water_leaf_info(self, data: bytes) -> Iterator[LeafWaterInfo]:
         """Parse data associated with visleafs containing water."""
         texinfo = self.texinfo
-        for surf_z, min_z, texinfo_ind in struct.iter_unpack('<ffH2x', data):
+        for surf_z, min_z, texinfo_ind in self.lump_layout['LEAFWATERDATA'].iter_unpack(data):
             yield LeafWaterInfo(surf_z, min_z, texinfo[texinfo_ind])
 
     def _lmp_write_water_leaf_info(self, data: List[LeafWaterInfo]) -> Iterator[bytes]:
         """Write data associated with visleafs containing water."""
         add_texinfo = _find_or_insert(self.texinfo)
         for info in self.water_leaf_info:
-            yield struct.pack('<ffH2x', info.surface_z, info.min_z, add_texinfo(info.surface_texinfo))
+            yield self.lump_layout['LEAFWATERDATA'].pack(info.surface_z, info.min_z, add_texinfo(info.surface_texinfo))
 
     def _lmp_read_visleafs(self, data: bytes) -> Iterator[VisLeaf]:
         """Parse the leafs of the visleaf/bsp tree."""
         # There's an indirection through these index arrays.
         leaf_brushes = list(map(
             self.brushes.__getitem__,
-            read_array('<H', self.lumps[BSP_LUMPS.LEAFBRUSHES].data),
+            read_array(self.lump_layout['LEAFBRUSH'], self.lumps[BSP_LUMPS.LEAFBRUSHES].data),
         ))
         leaf_faces = list(map(
             self.faces.__getitem__,
-            read_array('<H', self.lumps[BSP_LUMPS.LEAFFACES].data),
+            read_array(self.lump_layout['LEAFFACE'], self.lumps[BSP_LUMPS.LEAFFACES].data),
         ))
         # Another lump which is just an array of ints - no point being separate.
         dist_to_water = read_array('<H', self.lumps[BSP_LUMPS.LEAFMINDISTTOWATER].data)
 
         is_vitamin = self.is_vitamin
-        if is_vitamin:
-            leaf_fmt = '<ihh6I4HhBx'
-            has_ambient = False
-        else:
-            leaf_fmt = '<ihh6h4Hh'
-            has_ambient = False
-            # Some extra ambient light data.
-            if self.version <= 19:
-                has_ambient = True
-                leaf_fmt += '24s'
-            leaf_fmt += '2x'
+        leaf_fmt = self.lump_layout['LEAF']
+        # Some extra ambient light data.
+        has_ambient = not is_vitamin and self.version <= 19
 
-        for leaf_data, water_dist in zip(struct.iter_unpack(leaf_fmt, data), dist_to_water):
+        for leaf_data, water_dist in zip(leaf_fmt.iter_unpack(data), dist_to_water):
             if is_vitamin:
                 # VitaminSource moves the flags into its own block.
                 (
                     contents,
                     cluster_ind, area,
                     min_x, min_y, min_z,
                     max_x, max_y, max_z,
@@ -2079,16 +2163,16 @@
                         max_x, max_y, max_z,
                         first_face, num_faces,
                         first_brush, num_brushes,
                         water_ind,
                     ) = leaf_data
                     # bytes(24), but can constant fold.
                     ambient = b'\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0'
-                area = area_and_flags >> 7
-                flags = area_and_flags & 0b1111111
+                area = area_and_flags >> self.lump_layout['LEAF_AREA_OFFSET']
+                flags = area_and_flags & ((1 << self.lump_layout['LEAF_AREA_OFFSET']) - 1)
             yield VisLeaf(
                 BrushContents(contents), cluster_ind, area, VisLeafFlags(flags),
                 Vec(min_x, min_y, min_z),
                 Vec(max_x, max_y, max_z),
                 leaf_faces[first_face:first_face+num_faces],
                 leaf_brushes[first_brush:first_brush+num_brushes],
                 water_ind, ambient, water_dist,
@@ -2100,18 +2184,15 @@
         nodes: List[Tuple[VisTree, int, int]] = []
 
         for (
             plane_ind, neg_ind, pos_ind,
             min_x, min_y, min_z,
             max_x, max_y, max_z,
             first_face, face_count, area_ind,
-        ) in struct.iter_unpack(
-            '<iii6iHHh2x' if self.is_vitamin else '<iii6hHHh2x',
-            data,
-        ):
+        ) in self.lump_layout['NODE'].iter_unpack(data):
             nodes.append((VisTree(
                 self.planes[plane_ind],
                 Vec(min_x, min_y, min_z),
                 Vec(max_x, max_y, max_z),
                 self.faces[first_face:first_face+face_count],
                 area_ind,
             ), neg_ind, pos_ind))
@@ -2143,16 +2224,15 @@
             else:
                 pos_ind = add_node(node.child_pos)
             if isinstance(node.child_neg, VisLeaf):
                 neg_ind = -(add_leaf(node.child_neg) + 1)
             else:
                 neg_ind = add_node(node.child_neg)
 
-            buf.write(struct.pack(
-                '<iii6iHHh2x' if self.is_vitamin else '<iii6hHHh2x',
+            buf.write(self.lump_layout['NODE'].pack(
                 add_plane(node.plane), neg_ind, pos_ind,
                 int(node.mins.x), int(node.mins.y), int(node.mins.z),
                 int(node.maxes.x), int(node.maxes.y), int(node.maxes.z),
                 add_faces(node.faces), len(node.faces), node.area_ind,
             ))
 
         return buf.getvalue()
@@ -2165,49 +2245,52 @@
 
         add_face = _find_or_insert(self.faces)
         add_brush = _find_or_insert(self.brushes)
 
         buf = BytesIO()
         is_vitamin = self.is_vitamin
 
+        # Some extra ambient light data.
+        has_ambient = self.version <= 19
+
         for leaf in visleafs:
             # Do not deduplicate these, engine assumes they aren't when allocating memory.
             face_ind = len(leaf_faces)
             brush_ind = len(leaf_brushes)
             leaf_faces.extend(map(add_face, leaf.faces))
             leaf_brushes.extend(map(add_brush, leaf.brushes))
             min_water_dists.append(leaf.min_water_dist)
 
             if is_vitamin:
-                buf.write(struct.pack(
-                    '<ihh6I4HhBx',
+                buf.write(self.lump_layout['LEAF'].pack(
                     leaf.contents.value, leaf.cluster_id, leaf.area,
                     int(leaf.mins.x), int(leaf.mins.y), int(leaf.mins.z),
                     int(leaf.maxes.x), int(leaf.maxes.y), int(leaf.maxes.z),
                     face_ind, len(leaf.faces),
                     brush_ind, len(leaf.brushes),
                     leaf.water_id, leaf.flags.value,
                 ))
             else:
-                buf.write(struct.pack(
-                    '<ihh6h4Hh',
+                leafdata: Tuple[Union[int, bytes], ...] = (
                     leaf.contents.value, leaf.cluster_id,
-                    (leaf.area << 7 | leaf.flags.value),
+                    (leaf.area << self.lump_layout['LEAF_AREA_OFFSET'] | leaf.flags.value),
                     int(leaf.mins.x), int(leaf.mins.y), int(leaf.mins.z),
                     int(leaf.maxes.x), int(leaf.maxes.y), int(leaf.maxes.z),
                     face_ind, len(leaf.faces),
                     brush_ind, len(leaf.brushes),
-                    leaf.water_id,
-                ))
-                if self.version <= 19:
-                    buf.write(leaf._ambient)
-                buf.write(b'\x00\x00')  # Padding.
+                    leaf.water_id)
+                
+                # Older leaf lumps include some ambient light data at the end.
+                if has_ambient:
+                    leafdata = leafdata + (leaf._ambient,)
+
+                buf.write(self.lump_layout['LEAF'].pack(*leafdata))
 
-        self.lumps[BSP_LUMPS.LEAFFACES].data = write_array('<H', leaf_faces)
-        self.lumps[BSP_LUMPS.LEAFBRUSHES].data = write_array('<H', leaf_brushes)
+        self.lumps[BSP_LUMPS.LEAFFACES].data = write_array(self.lump_layout['LEAFFACE'], leaf_faces)
+        self.lumps[BSP_LUMPS.LEAFBRUSHES].data = write_array(self.lump_layout['LEAFBRUSH'], leaf_brushes)
         self.lumps[BSP_LUMPS.LEAFMINDISTTOWATER].data = write_array('<H', min_water_dists)
         return buf.getvalue()
 
     def read_texture_names(self) -> Iterator[str]:
         """Iterate through all brush textures in the map."""
         warnings.warn('Access bsp.textures', DeprecationWarning, stacklevel=2)
         return iter(self.textures)
@@ -2732,29 +2815,29 @@
         Deprecated, bsp.props is stored and resaved.
         """
         warnings.warn('Assign to BSP.props', DeprecationWarning, stacklevel=2)
         self.props = props
 
     def _lmp_read_props(self, vers_num: int, data: bytes) -> Iterator['StaticProp']:
         # The version of the static prop format - different features.
-        if vers_num > 11:
+        if vers_num > 12:
             raise ValueError(f'Unknown version ({vers_num})!')
         if vers_num < 4:
             # Predates HL2, no game produces these.
             raise ValueError(f'Static prop version {vers_num} is too old!')
 
         static_lump = BytesIO(data)
 
         # Array of model filenames.
         model_dict = list(self._read_static_props_models(static_lump))
 
         [visleaf_count] = struct_read('<i', static_lump)
         visleaf_list = list(map(
             self.visleafs.__getitem__,
-            struct_read('H' * visleaf_count, static_lump),
+            struct_read(self.lump_layout['STATICPROPLEAF'].format[1] * visleaf_count, static_lump),
         ))
 
         [prop_count] = struct_read('<i', static_lump)
 
         if prop_count == 0:
             # No props, following code will divide by zero, also no point anyway.
             # Use the 'standard' version for the given version number.
@@ -2926,15 +3009,15 @@
         # Now write out the sections.
         prop_lump = BytesIO()
         prop_lump.write(struct.pack('<i', len(model_list)))
         for name in model_list:
             prop_lump.write(struct.pack('<128s', name.encode('ascii')))
 
         prop_lump.write(struct.pack('<i', len(leaf_array)))
-        prop_lump.write(write_array('<H', leaf_array))
+        prop_lump.write(write_array(self.lump_layout['STATICPROPLEAF'], leaf_array))
 
         prop_lump.write(struct.pack('<i', len(props)))
         for (leaf_off, model_ind), prop in zip(indexes, props):
             start = prop_lump.tell()
             prop_lump.write(struct.pack(
                 '<3f3fH',
                 prop.origin.x,
```

### Comparing `srctools-2.3.8/src/srctools/cmdseq.py` & `srctools-2.3.9/src/srctools/cmdseq.py`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/const.py` & `srctools-2.3.9/src/srctools/const.py`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/dmx.py` & `srctools-2.3.9/src/srctools/dmx.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,24 +215,15 @@
     List[Quaternion],
     List[FrozenMatrix],
     List[_Element],
 ]
 # Additional values we convert to valid types.
 ConvValue: TypeAlias = Union[Value, Vec, Matrix, Angle]
 
-ValueT = TypeVar(
-    'ValueT',
-    int, float, bool, str, bytes,
-    Color, Time,
-    Vec2, FrozenVec, Vec4,
-    FrozenAngle,
-    Quaternion,
-    FrozenMatrix,
-    _Element,
-)
+ValueT = TypeVar('ValueT', bound=Value)
 
 # [from, to] -> conversion.
 # Implementation at the end of the file.
 # Unfortunately we can't show the ValueType -> Value match to the type checker.
 ConvertMap: TypeAlias = Dict[Tuple[ValueType, ValueType], Callable[[Value], Value]]
 TYPE_CONVERT: ConvertMap
 
@@ -289,22 +280,22 @@
         if from_typ is not ValueType.STRING and from_typ is not ValueType.BINARY:
             sizes[from_typ] = ns['_struct_' + from_typ.name.casefold()].size
         convert[from_typ] = ns.pop(f'_conv_{from_typ.name.casefold()}')
 
     return type_conv, convert, sizes
 
 
-def _make_val_prop(val_type: ValueType, typ: Type[Value]) -> property:
+def _make_val_prop(val_type: ValueType, typ: Type[ValueT]) -> property:
     """Build the properties for each type."""
 
-    def setter(self: '_ValProps', value: ValueT) -> None:
+    def setter(self: '_ValProps', value: Value) -> None:
         self._write_val(val_type, value)
 
-    def getter(self: '_ValProps') -> ValueT:
-        return self._read_val(val_type)  # type: ignore
+    def getter(self: '_ValProps') -> Value:
+        return self._read_val(val_type)
 
     if val_type.name[0].casefold() in 'aeiou':
         desc = f'an {val_type.name.lower()}.'
     else:
         desc = f'a {val_type.name.lower()}.'
     getter.__doc__ = 'Return the value as ' + desc
     setter.__doc__ = 'Convert the value to ' + desc
@@ -998,15 +989,15 @@
     def append(self, value: ConvValue) -> None:
         """Append an item to the array.
 
         If not already an array, it is converted to one
         holding the existing value.
         """
         if not isinstance(self._value, list):
-            self._value = cast('List[ValueT]', [self._value])
+            self._value = [self._value]
         [val_type, result] = deduce_type_single(value)
         if val_type is not self._typ:
             # Try converting.
             try:
                 func = cast('Callable[[Value], ValueT]', TYPE_CONVERT[val_type, self._typ])
             except KeyError:
                 raise ValueError(f'Cannot convert ({val_type}) to {self._typ} type!')
@@ -1017,15 +1008,15 @@
     def extend(self, values: Iterable[ConvValue]) -> None:
         """Append multiple values to the array.
 
         If not already an array, it is converted to one
         holding the existing value.
         """
         if not isinstance(self._value, list):
-            self._value = cast('List[ValueT]', [self._value])
+            self._value = [self._value]
         for value in values:
             [val_type, result] = deduce_type_single(value)
             if val_type is not self._typ:
                 # Try converting.
                 try:
                     func = cast('Callable[[Value], ValueT]', TYPE_CONVERT[val_type, self._typ])
                 except KeyError:
@@ -2396,9 +2387,10 @@
 
 
 def _conv_element(value: Element) -> Element:
     if not isinstance(value, Element):
         raise ValueError('Expected element, got: ' + repr(value))
     return value
 
+
 # Gather all these functions, add to the dicts.
 TYPE_CONVERT, CONVERSIONS, SIZES = _get_converters()
```

### Comparing `srctools-2.3.8/src/srctools/fgd.py` & `srctools-2.3.9/src/srctools/fgd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Parse FGD files, used to describe Hammer entities."""
 from typing import (
     IO, TYPE_CHECKING, AbstractSet, Any, Callable, ClassVar, Collection, Container, Dict,
     FrozenSet, Generic, Iterable, Iterator, List, Mapping, Optional, Sequence, Set, TextIO,
     Tuple, Type, TypeVar, Union, cast,
 )
-from typing_extensions import TypeAlias, overload
+from typing_extensions import Protocol, TypeAlias, overload
 from collections import ChainMap, defaultdict
 from copy import deepcopy
 from enum import Enum
 from importlib_resources import files
 from pathlib import PurePosixPath
 import io
 import itertools
@@ -41,22 +41,23 @@
     'HelperSize', 'HelperSphere', 'HelperSprite',
     'HelperSweptPlayerHull', 'HelperTrack', 'HelperTypes',
     'HelperVecLine', 'HelperWorldText',
 
     'HelperExtAppliesTo', 'HelperExtAutoVisgroups', 'HelperExtOrderBy',
 ]
 
-# Cached result of FGD.engine_dbase().
-_ENGINE_FGD: Optional['FGD'] = None
 T = TypeVar('T')
 FileSysT = TypeVar('FileSysT', bound=FileSystem[Any])
 _fake_vmf = VMF(preserve_ids=False)
 # Collections of tags.
 TagsSet: TypeAlias = FrozenSet[str]
 
+# Cached engine DB parsing functions.
+_ENGINE_DB: Optional['_EngineDBProto'] = None
+
 
 class FGDParseError(TokenSyntaxError):
     """Raised if the FGD contains invalid syntax."""
 
 
 class ValueTypes(Enum):
     """Types which can be applied to a KeyValue."""
@@ -278,29 +279,33 @@
 
     @property
     def extension(self) -> bool:
         """Is this an extension to the format?"""
         return self.name.startswith('EXT_')
 
 
-def _load_engine_db() -> 'FGD':
+def _load_engine_db() -> '_EngineDBProto':
     """Load our engine database."""
     # It's pretty expensive to parse, so keep the original privately,
     # returning a deep-copy.
-    global _ENGINE_FGD
-    if _ENGINE_FGD is None:
-        from lzma import LZMAFile
-
+    global _ENGINE_DB
+    if _ENGINE_DB is None:
         from ._engine_db import unserialise
-        comp: IO[bytes]
         # On 3.8, importlib_resources doesn't have the right stubs.
-        with cast(Any, files(srctools) / 'fgd.lzma').open('rb') as comp:
-            with LZMAFile(comp) as f:
-                _ENGINE_FGD = unserialise(f)
-    return _ENGINE_FGD
+        with cast(Any, files(srctools) / 'fgd.lzma').open('rb') as f:
+            _ENGINE_DB = unserialise(f)
+    return _ENGINE_DB
+
+
+def _engine_db_stats() -> str:
+    """Return information about how much of the engine database has been parsed."""
+    if _ENGINE_DB is None:
+        return '<not loaded>'
+    else:
+        return _ENGINE_DB.stats()
 
 
 def read_colon_list(tok: BaseTokenizer, had_colon: bool = False) -> Tuple[List[str], Token]:
     """Read strings seperated by colons, up to the end of the line.
 
     The token found at the end is returned.
     """
@@ -478,75 +483,14 @@
 
     @classmethod
     def part(cls, filename: str, tags: TagsSet = frozenset()) -> 'Resource':
         """Create a resource definition for a particle system."""
         return cls(filename, FileType.PARTICLE_SYSTEM, tags)
 
 
-_GetFGDFunc = Callable[[str], 'EntityDef']
-
-
-@attrs.frozen(init=False)
-class ResourceCtx:
-    """Map information passed to :attr:`FileType.ENTCLASS_FUNC` functions."""
-    tags: TagsSet
-    fsys: FileSystem[Any]
-    #: The BSP/VMF map name, like what is passed to :command:`map` in-game.
-    mapname: str
-    get_entdef: Callable[[str], 'EntityDef']
-
-    # For use of get_resources() only.
-    _functions: Mapping[str, Callable[
-        ['ResourceCtx', Entity],
-        Iterator[Union[Resource, Entity]]
-    ]]
-
-    def __init__(
-        self,
-        tags: Iterable[str] = (),
-        fsys: FileSystem[Any] = VirtualFileSystem({}),
-        fgd: Union['FGD', Mapping[str, 'EntityDef'], _GetFGDFunc] = srctools.EmptyMapping,
-        mapname: str = '',
-        funcs: Mapping[str, Callable[
-            ['ResourceCtx', Entity],
-            Iterator[Union[Resource, Entity]]
-        ]] = srctools.EmptyMapping,
-    ) -> None:
-        """
-        :param fgd: Used to look up dependent entities. May either be the :py:class:`FGD` itself, \
-        an equivalent :external:term:`mapping`, or a callable returning the :py:class:`EntityDef`.
-        :param tags: Various string tags used to indicate what engine branch is being used. This \
-        allows handling Episodic differences, or enhancements by Mapbase.
-        :param fsys: A :py:class:`~srctools.FileSystem`
-        :param mapname:
-        :param funcs: Mapping of names to entclass functions to call. A builtin set of functions is
-        accessed, if not present in this
-        """
-        from srctools._class_resources import CLASS_FUNCS
-        if funcs is srctools.EmptyMapping:
-            funcs = CLASS_FUNCS
-        else:
-            # ChainMap itself is mutable and so can't accept Mapping.
-            # We're immediately casting to Mapping, so it's not dangerous.
-            funcs = ChainMap(funcs, CLASS_FUNCS)  # type: ignore[arg-type]
-
-        # Strip extension, and normalise folder separators.
-        if mapname.casefold().endswith(('.bsp', '.vmf', '.vmm', '.vmx')):
-            mapname = mapname[:-4]
-        self.__attrs_init__(  # pyright: ignore
-            frozenset(map(str.upper, tags)),
-            fsys,
-            mapname.replace('\\', '/'),
-            # If this is an FGD or Mapping __getitem__ is the appropriate callable, otherwise
-            # it must already be callable.
-            getattr(fgd, '__getitem__', cast(_GetFGDFunc, fgd)),
-            funcs,
-        )
-
-
 class Helper:
     """Base class for representing helper() commands in the header of an entity.
 
     These mainly add visual widgets in Hammer's views for manipulating and
     previewing keyvalues.
 
     This should not be instantiated, only subclasses in _fgd_helpers.
@@ -596,14 +540,15 @@
             return NotImplemented
         return self.TYPE is not other.TYPE or vars(self) != vars(other)
 
 
 class UnknownHelper(Helper):
     """Represents an unknown helper."""
     TYPE: ClassVar[Optional[HelperTypes]] = None
+
     def __init__(self, name: str, args: List[str]) -> None:
         """Unknown helpers have a name attribute."""
         self.name = name
         self.args = args
 
     def export(self) -> List[str]:
         """Produce the argument text to recreate this helper type."""
@@ -1359,21 +1304,21 @@
         """Return the specified entity from an internal copy of the Hammer Addons database.
 
         This can be used to identify the kind of keys/inputs/outputs present on an entity, as well
         as resources the entity requires/:external:cpp:func:`!Precache()`\\ es.
 
         :raises KeyError: If the classname is not found in the database.
         """
-        return deepcopy(_load_engine_db()[classname])  # Or KeyError if not found.
+        return deepcopy(_load_engine_db().get_ent(classname))  # Or KeyError if not found.
 
     @classmethod
     def engine_classes(cls) -> AbstractSet[str]:
         """Return a set of known entity classnames, from the Hammer Addons database."""
         # This is immutable, so we don't need to copy.
-        return _load_engine_db().entities.keys()
+        return _load_engine_db().get_classnames()
 
     def __repr__(self) -> str:
         if self.type is EntityTypes.BASE:
             return f'<Entity Base "{self.classname}">'
         else:
             return f'<Entity {self.classname}>'
 
@@ -1454,15 +1399,15 @@
         else:
             for helper in self.helpers:
                 if helper.TYPE == typ.TYPE:
                     yield helper
 
     def get_resources(
         self,
-        ctx: ResourceCtx,
+        ctx: 'ResourceCtx',
         *,
         ent: Optional[Entity],
         on_error: Callable[[str], object] = lambda err: None,
     ) -> Iterator[Tuple[FileType, str]]:
         """Recursively fetch all the resources this entity may use, simulating ``Precache()``.
 
         :param ent: A specific entity to evaluate against. If not provided, functions will
@@ -1746,15 +1691,15 @@
                         )
                     ) from None
 
     def sorted_ents(self) -> Iterator[EntityDef]:
         """Yield all entities in sorted order.
 
         This ensures only all bases for an entity are yielded before the entity.
-        Otherwise entities are ordered in alphabetical order.
+        Otherwise, entities are ordered in alphabetical order.
         """
         # We need to do a topological sort.
         todo: Set[EntityDef] = set(self)
         done: Set[EntityDef] = set()
         cls_getter = operator.attrgetter('classname')
         while todo:
             deferred: Set[EntityDef] = set()
@@ -1788,15 +1733,15 @@
                 raise ValueError(
                     f"Loop in bases! \n Problematic entities:\n"
                     f"{[ent.classname for ent in deferred]}"
                 )
 
             todo = deferred.difference(done)
 
-    def collapse_bases(self) -> None:
+    def collapse_bases(self, ignore_aliases: bool = True) -> None:
         """Collapse all bases into the entities that use them.
 
         This operates in-place, and clears all the base attributes as a result.
         """
         # We need to do a topological sort effectively, to ensure we do
         # parents before children.
         for ent in self.sorted_ents():
@@ -2071,15 +2016,15 @@
     def engine_dbase(cls) -> 'FGD':
         """Load and return a database of entity keyvalues and I/O.
 
         This can be used to identify the kind of keys present on an entity. If you only need
         specific entities, use :py:func:`EntityDef.engine_def()` instead to avoid needing to fetch
         all the entities.
         """
-        return deepcopy(_load_engine_db())
+        return _load_engine_db().get_fgd()
 
     def __getitem__(self, classname: str) -> EntityDef:
         """Lookup entities by classname."""
         try:
             return self.entities[classname.casefold()]
         except KeyError:
             raise KeyError(f'No class "{classname}"!') from None
@@ -2122,14 +2067,76 @@
                 if poss_name not in self.entities:
                     base.classname = poss_name
                     self.entities[poss_name] = base
                     break
             self._fix_missing_bases(base)
 
 
+_GetFGDFunc: TypeAlias = Callable[[str], EntityDef]
+
+
+@attrs.frozen(init=False)
+class ResourceCtx:
+    """Map information passed to :attr:`FileType.ENTCLASS_FUNC` functions."""
+    tags: TagsSet
+    fsys: FileSystem[Any]
+    #: The BSP/VMF map name, like what is passed to :command:`map` in-game.
+    mapname: str
+    get_entdef: Callable[[str], 'EntityDef']
+
+    # For use of get_resources() only.
+    _functions: Mapping[str, Callable[
+        ['ResourceCtx', Entity],
+        Iterator[Union[Resource, Entity]]
+    ]]
+
+    def __init__(
+        self,
+        tags: Iterable[str] = (),
+        fsys: FileSystem[Any] = VirtualFileSystem({}),
+        fgd: Union[FGD, Mapping[str, EntityDef], _GetFGDFunc] = EntityDef.engine_def,
+        mapname: str = '',
+        funcs: Mapping[str, Callable[
+            ['ResourceCtx', Entity],
+            Iterator[Union[Resource, Entity]]
+        ]] = srctools.EmptyMapping,
+    ) -> None:
+        """
+        :param fgd: Used to look up dependent entities. May either be the :py:class:`FGD` itself, \
+        an equivalent :external:term:`mapping`, or a callable returning the :py:class:`EntityDef`.
+        If unset the internal database will be used.
+        :param tags: Various string tags used to indicate what engine branch is being used. This \
+        allows handling Episodic differences, enhancements by Mapbase, and other things like that.
+        :param fsys: A :py:class:`~srctools.FileSystem`, used to read scripts and other files.
+        :param mapname: The name of the map, used to handle some entities that used this to pick variants.
+        :param funcs: Mapping of names to entclass functions to call. A builtin set of functions is
+        accessed, if not present in this.
+        """
+        from srctools._class_resources import CLASS_FUNCS
+        if funcs is srctools.EmptyMapping:
+            funcs = CLASS_FUNCS
+        else:
+            # ChainMap itself is mutable and so can't accept Mapping.
+            # We're immediately casting to Mapping, so it's not dangerous.
+            funcs = ChainMap(funcs, CLASS_FUNCS)  # type: ignore[arg-type]
+
+        # Strip extension, and normalise folder separators.
+        if mapname.casefold().endswith(('.bsp', '.vmf', '.vmm', '.vmx')):
+            mapname = mapname[:-4]
+        self.__attrs_init__(  # pyright: ignore
+            frozenset(map(str.upper, tags)),
+            fsys,
+            mapname.replace('\\', '/'),
+            # If this is an FGD or Mapping __getitem__ is the appropriate callable, otherwise
+            # it must already be callable.
+            getattr(fgd, '__getitem__', cast(_GetFGDFunc, fgd)),
+            funcs,
+        )
+
+
 def _init_helper_impl() -> None:
     """Import and register the helper implementations."""
     # noinspection PyProtectedMember
     from srctools import _fgd_helpers as helper_mod
     for helper_type in vars(helper_mod).values():
         if isinstance(helper_type, type) and issubclass(helper_type, Helper):
             if helper_type.TYPE is not None:
@@ -2137,14 +2144,34 @@
 
     for helper in HelperTypes:
         if helper not in HELPER_IMPL:
             raise ValueError(
                 f'Missing helper implementation for {helper}! : {HELPER_IMPL}'
             )
 
+
+class _EngineDBProto(Protocol):
+    """Unserialised database, which will be parsed progressively as required."""
+    def get_classnames(self) -> AbstractSet[str]:
+        """Get the classnames in the database."""
+        raise NotImplementedError
+
+    def get_ent(self, classname: str) -> EntityDef:
+        """Fetch the specified entity."""
+        raise NotImplementedError
+
+    def get_fgd(self) -> FGD:
+        """Parse all the blocks and make an FGD."""
+        raise NotImplementedError
+
+    def stats(self) -> str:
+        """Return usage statistics for the database."""
+        raise NotImplementedError
+
+
 # Each helper type -> the class implementing them.
 HELPER_IMPL: Dict[HelperTypes, Type[Helper]] = {}
 
 # If we're importing, make sure _fgd_helpers is imported fresh. Otherwise, if the module is
 # reloaded it'll be using the old classes, breaking our registration.
 try:
     del sys.modules['srctools._fgd_helpers']
```

### Comparing `srctools-2.3.8/src/srctools/filesys.py` & `srctools-2.3.9/src/srctools/filesys.py`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/game.py` & `srctools-2.3.9/src/srctools/game.py`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/instancing.py` & `srctools-2.3.9/src/srctools/instancing.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     node_ids: Dict[int, int]
     visgroup_ids: Dict[int, int]
     def __init__(
         self,
         name: str,
         filename: str,
         pos: Vec, orient: Matrix,
-        fixup_type: FixupStyle,
+        fixup_type: FixupStyle = FixupStyle.PREFIX,
         outputs: Iterable[Output] = (),
         fixup: Iterable[FixupValue] = (),
     ) -> None:
         self.name = name
         self.filename = filename
         self.pos = pos
         self.orient = orient
@@ -100,15 +100,15 @@
             ent.fixup.copy_values(),
         )
         inst.recur_count = getattr(ent, RECUR_COUNT_ATTR, 0)
         return inst
 
     def fixup_name(self, name: str) -> str:
         """Apply the name fixup rules to this name."""
-        if name.startswith(('@', '!')):
+        if not name or name.startswith(('@', '!')):
             return name
         if self.fixup_type is FixupStyle.NONE:
             return name
         elif self.fixup_type is FixupStyle.PREFIX:
             return f'{self.name}-{name}'
         elif self.fixup_type is FixupStyle.SUFFIX:
             return f'{name}-{self.name}'
@@ -160,22 +160,26 @@
             try:
                 old_id = int(value)
             except (ValueError, TypeError):
                 return value  # Skip.
             try:
                 value = str(self.node_ids[old_id])
             except KeyError:
-                self.node_ids[old_id] = new_id = vmf.node_id.get_id()
+                self.node_ids[old_id] = new_id = vmf.node_id.get_id(old_id)
                 value = str(new_id)
         elif type is ValueTypes.VEC_AXIS:
             # Two positions seperated by commas.
             first_str, second_str = value.split(',')
             first = Vec.from_str(first_str) @ self.orient + self.pos
             second = Vec.from_str(second_str) @ self.orient + self.pos
             value = f'{first}, {second}'
+        elif type is ValueTypes.ANGLE_NEG_PITCH or type is ValueTypes.EXT_ANGLE_PITCH:
+            raise ValueError(f'"{type.name}" keyvalue type must be fixed up on the instance as a whole!')
+        elif type is ValueTypes.CHOICES:
+            raise ValueError('choices keyvalue type is not meaningful, it should be swapped with another type!')
         # All others = no change required.
         return value
 
 
 class Manifest(Instance):
     """Additional options set in VMM manifests."""
     def __init__(
@@ -294,15 +298,15 @@
             break
     return fsys
 
 
 def reset_keyvalue_warnings() -> None:
     """If an unknown keyvalue is encountered during collapsing, a log message is produced only once.
 
-    This resets the internal tracker so the messages will be repeated again.
+    This resets the internal tracker so the messages will be repeated.
     """
     _UNKNOWN_KV.clear()
 
 
 def collapse_one(
     vmf: VMF,
     inst: Instance,
@@ -439,14 +443,21 @@
             setattr(new_ent, RECUR_COUNT_ATTR, inst.recur_count + 1)
 
         # Now keyvalues.
         # First extract a rotated angles value, handling the special "pitch" and "yaw" keys.
         angles = Angle.from_str(new_ent['angles'])
         if 'pitch' in new_ent:
             angles.pitch = srctools.conv_float(new_ent['pitch'])
+            try:
+                kv = ent_type.kv['pitch']
+            except KeyError:
+                pass
+            else:
+                if kv.type is ValueTypes.ANGLE_NEG_PITCH:
+                    angles.pitch = -angles.pitch
         if 'yaw' in new_ent:
             angles.yaw = srctools.conv_float(new_ent['yaw'])
         angles @= orient
 
         for key, value in new_ent.items():
             folded = key.casefold()
             value = inst.fixup.substitute(value, '')
@@ -456,15 +467,15 @@
                 continue
             elif folded == 'angles':
                 new_ent['angles'] = str(angles)
                 continue
             elif folded == 'yaw':
                 new_ent['yaw'] = format_float(angles.yaw)
                 continue
-            elif folded in ('classname', 'hammerid', 'spawnflags', 'nodeid'):
+            elif folded in {'classname', 'hammerid', 'spawnflags'}:
                 continue
 
             try:
                 kv = ent_type.kv[folded]
             except KeyError:
                 if folded.startswith('$') and classname == 'func_instance':
                     # Dummy fixup names Hammer provides for convenience, ignore.
```

### Comparing `srctools-2.3.8/src/srctools/keyvalues.py` & `srctools-2.3.9/src/srctools/keyvalues.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 Handling `\\\\n`, `\\\\t`, `\\\\"`, and `\\\\\\\\` escape characters can be enabled.
 """
 from typing import (
     Any, Callable, Dict, Iterable, Iterator, List, Mapping, Optional, Tuple, Type, TypeVar,
     Union, cast,
 )
-from typing_extensions import Final, overload
+from typing_extensions import Final, TypeAlias, overload
 import builtins  # Keyvalues.bool etc shadows these.
 import keyword
 import os
 import sys
 import types
 import warnings
 
@@ -78,19 +78,15 @@
 
 __all__ = ['KeyValError', 'NoKeyError', 'Keyvalues']
 
 # Sentinel value to indicate that no default was given to find_key()
 _NO_KEY_FOUND = cast(str, object())
 
 _KV_Value = Union[List['Keyvalues'], str, Any]
-# We don't have recursive definitions, just go deep enough it should be fine.
-_As_Dict_Ret = Union[str, Dict[str, Union[str, Dict[str, Union[str, Dict[str,
-               Union[str, Dict[str, Union[str, Dict[str, Union[str, Dict[str,
-               Union[str, Dict[str, Union[str, Dict[str, Union[str, Dict[str,
-               Any]]]]]]]]]]]]]]]]]]
+_As_Dict_Ret: TypeAlias = Union[str, Dict[str, '_As_Dict_Ret']]
 
 T = TypeVar('T')
 
 # Various [flags] used after keyvalues names in some Valve files.
 # See https://github.com/ValveSoftware/source-sdk-2013/blob/master/sp/src/tier1/KeyValues.cpp#L2055
 FLAGS_DEFAULT = {
     # We know we're not on a console...
@@ -247,20 +243,26 @@
         newline_keys: bool = False,
         newline_values: bool = True,
         allow_escapes: bool=True,
         single_line: bool=False,
     ) -> "Keyvalues":
         """Returns a Keyvalues tree parsed from given text.
 
-        :param file_contents: should be an iterable of strings or a single string. Alternatively, file_contents may be an already created tokenizer. In this case ``allow_escapes`` is ignored.
-        :param filename: If set this should be the source of the text for debug purposes. If not supplied, ``file_contents.name`` will be used if present.
+        :param file_contents: should be an iterable of strings or a single string. Alternatively, \
+        file_contents may be an already created tokenizer. In this case ``allow_escapes`` is ignored.
+        :param filename: If set this should be the source of the text for debug purposes. If not \
+        supplied, ``file_contents.name`` will be used if present.
         :param flags: This should be a mapping for additional ``[flag]`` suffixes to accept.
         :param allow_escapes: This allows choosing if ``\\t`` or similar escapes are parsed.
-        :param single_line: If this is set, allow multiple properties to be on the same line. This means unterminated strings will be caught late (if at all), but it allows parsing some 'internal' data blocks.
-        :param newline_keys: This specifies if newline characters are allowed in keys. Keys are prohibited by default, since this is fairly useless, but if quote characters are mismatched it'll catch the mistake early.
+        :param single_line: If this is set, allow multiple properties to be on the same line. \
+        This means unterminated strings will be caught late (if at all), but it allows parsing \
+        some 'internal' data blocks.
+        :param newline_keys: This specifies if newline characters are allowed in keys. \
+        Keys are prohibited by default, since this is fairly useless, but if quote characters are \
+        mismatched it'll catch the mistake early.
         :param newline_values: This specifies if newline characters are allowed in string values.
         """
         # The block we are currently adding to.
 
         # The special name 'None' marks it as the root keyvalue, which
         # just outputs its children when exported. This way we can handle
         # multiple root blocks in the file, while still returning a single
@@ -513,14 +515,15 @@
         for block in self.find_all(*keys):
             yield from block
 
     @overload
     def find_key(self, key: str, *, or_blank: bool) -> 'Keyvalues': ...
     @overload
     def find_key(self, key: str, def_: str=...) -> 'Keyvalues': ...
+
     def find_key(self, key: str, def_: str=_NO_KEY_FOUND, *, or_blank: bool=False) -> 'Keyvalues':
         """Obtain the child Keyvalue with a given name.
 
         - If no child is found with the given name, this will return the
           default value wrapped in a Keyvalue. If or_blank is set,
           it will be a blank block instead. If neither default is provided
           this will raise NoKeyError.
@@ -588,14 +591,15 @@
         else:
             return def_
 
     @overload
     def int(self, key: str) -> builtins.int: ...
     @overload
     def int(self, key: str, def_: T) -> Union[builtins.int, T]: ...
+
     def int(self, key: str, def_: Union[builtins.int, T]=0) -> Union[builtins.int, T]:
         """Return the value of an integer key.
 
         Equivalent to int(prop[key]), but with a default value if missing or
         invalid.
         If multiple keys with the same name are present, this will use the
         last only.
@@ -607,14 +611,15 @@
         except (NoKeyError, ValueError, TypeError):
             return def_
 
     @overload
     def float(self, key: str) -> builtins.float: ...
     @overload
     def float(self, key: str, def_: T) -> Union[builtins.float, T]: ...
+
     def float(self, key: str, def_: Union[builtins.float, T]=0.0) -> Union[builtins.float, T]:
         """Return the value of an integer key.
 
         Equivalent to float(prop[key]), but with a default value if missing or
         invalid.
         If multiple keys with the same name are present, this will use the
         last only.
@@ -626,14 +631,15 @@
         except (NoKeyError, ValueError, TypeError):
             return def_
 
     @overload
     def bool(self, key: str) -> builtins.bool: ...
     @overload
     def bool(self, key: str, def_: T) -> Union[builtins.bool, T]: ...
+
     def bool(self, key: str, def_: Union[builtins.bool, T]=False) -> Union[builtins.bool, T]:
         """Return the value of an boolean key.
 
         The value may be case-insensitively 'true', 'false', '1', '0', 'T',
         'F', 'y', 'n', 'yes', or 'no'.
         If multiple keys with the same name are present, this will use the
         last only.
@@ -720,14 +726,15 @@
         else:
             return self._value
 
     @overload
     def as_array(self) -> List[str]: ...
     @overload
     def as_array(self, *, conv: Callable[[str], T]) -> List[T]: ...
+
     def as_array(self, *, conv: Callable[[str], T]=cast(Callable[[str], T], str)) -> Union[List[T], List[str]]:
         """Convert a keyvalue block into a list of values.
 
         If the keyvalue is a single keyvalue, the single value will be
         yielded. Otherwise, each child must be a single value and each
         of those will be yielded. The name is ignored.
         """
```

### Comparing `srctools-2.3.8/src/srctools/logger.py` & `srctools-2.3.9/src/srctools/logger.py`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/math.py` & `srctools-2.3.9/src/srctools/math.py`

 * *Files 0% similar despite different names*

```diff
@@ -2475,15 +2475,15 @@
     >> Vec(range(0, 270, 90))  # Any 1,2 or 3 long iterable
     Vec(0, 90, 180)
     >>> Vec(1, 2, 3) @ Angle(0, 0, 45)
     Vec(1, -0.707107, 3.53553)
     >>> Angle.from_str('(45 90 0)')  # Parse strings.
     Angle(45, 90, 0)
 
-    Addition and subtraction can be performed 
+    Addition and subtraction can be performed
     between angles, while division/multiplication must be between an angle and scalar (to scale).
 
     Like vectors, each axis can be accessed by getting/setting ``pitch``/``yaw`` and ``roll`` attributes.
     In addition, the following indexes are allowed (case-insensitive):
 
     * ``0``, ``1``, ``2``
     * ``"p"``, ``"y"``, ``r``
@@ -2532,15 +2532,15 @@
     def __reduce__(self) -> Tuple[Callable[[float, float, float], 'Angle'], Tuple3]:
         """Pickling support.
 
         This redirects to a global function, so C/Python versions
         interoperate.
         """
         return _mk_ang, (self._pitch, self._yaw, self._roll)
-    
+
     def freeze(self) -> FrozenAngle:
         """Return an immutable copy of this angle."""
         ang = Py_FrozenAngle.__new__(Py_FrozenAngle)
         ang._pitch = self._pitch
         ang._yaw = self._yaw
         ang._roll = self._roll
         return ang
```

### Comparing `srctools-2.3.8/src/srctools/mdl.py` & `srctools-2.3.9/src/srctools/mdl.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     cast_texture_shadows = 1 << 18
 
     add_unknown(locals())
 
 
 class AnimEventTypes(FlagEnum):
     """Categories of animation events."""
-    NONE = 0
+    NONE      = 0
     SERVER    = 1 << 0
     SCRIPTED  = 1 << 1
     SHARED    = 1 << 2
     WEAPON    = 1 << 3
     CLIENT    = 1 << 4
     FACEPOSER = 1 << 5
     add_unknown(locals())
```

### Comparing `srctools-2.3.8/src/srctools/packlist.py` & `srctools-2.3.9/src/srctools/packlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,16 @@
 def load_fgd() -> FGD:
     """Extract the local copy of FGD data.
 
     This allows the analysis to not depend on local files.
     """
     import warnings
     warnings.warn(
-        'Use FGD.engine_dbase() instead, '
-        'this has been moved there.',
+        'Use EntityDef.engine_def() instead if possible, or FGD.engine_dbase() '
+        'if all entities are required.',
         DeprecationWarning,
         stacklevel=2,
     )
     return FGD.engine_dbase()
 
 
 def strip_extension(filename: str) -> str:
@@ -816,53 +816,60 @@
             # Static props obviously only use one skin.
             self.pack_file(prop.model, FileType.MODEL, skinset={prop.skin})
 
         # These are all the materials the BSP references, including brushes and overlays.
         for mat in bsp.textures:
             self.pack_file('materials/{}.vmt'.format(mat.lower()), FileType.MATERIAL)
 
-    def pack_fgd(
+    def pack_fgd(self, vmf: VMF, fgd: FGD, mapname: str='', tags: Iterable[str]=()) -> None:
+        warnings.warn(
+            "The provided FGD is no longer used, call pack_with_ents instead.",
+            DeprecationWarning, stacklevel=2,
+        )
+        self.pack_from_ents(vmf, mapname, tags)
+
+    def pack_from_ents(
         self,
         vmf: VMF,
-        fgd: FGD,
         mapname: str='',
         tags: Iterable[str]=(),
     ) -> None:
-        """Analyse the map to pack files. We use the FGD to easily handle this."""
+        """Analyse the map to pack files, using an internal database of keyvalues."""
         # Don't show the same keyvalue warning twice, it's just noise.
         unknown_keys: Set[Tuple[str, str]] = set()
 
         # Definitions for the common keyvalues on all entities.
-        try:
-            base_entity = fgd['_CBaseEntity_']
-        except KeyError:
-            LOGGER.warning('No CBaseEntity definition!')
-            base_entity = EntityDef(EntityTypes.BASE)
+        base_entity = EntityDef.engine_def('_CBaseEntity_')
 
         res_ctx = ResourceCtx(
-            fgd=fgd,
+            fgd=EntityDef.engine_def,
             fsys=self.fsys,
             mapname=mapname,
             tags=tags,
         )
 
+        cache: Dict[str, EntityDef] = {}
+
         for ent in vmf.entities:
             # Allow opting out packing specific entities.
             if conv_bool(ent.pop('srctools_nopack', '')):
                 continue
 
             classname = ent['classname']
             try:
-                ent_class = fgd[classname]
+                ent_class = cache[classname]
             except KeyError:
-                if (classname, '') not in unknown_keys:
-                    LOGGER.warning('Unknown class "{}"!', classname)
-                    unknown_keys.add((classname, ''))
-                # Fall back to generic keyvalues.
-                ent_class = base_entity
+                try:
+                    ent_class = cache[classname] = EntityDef.engine_def(classname)
+                except KeyError:
+                    if (classname, '') not in unknown_keys:
+                        LOGGER.warning('Unknown class "{}"!', classname)
+                        unknown_keys.add((classname, ''))
+                    # Fall back to generic keyvalues.
+                    ent_class = base_entity
 
             skinset: Optional[Set[int]]
             if ent['skinset'] != '':
                 # Special key for us - if set this is a list of skins this
                 # entity is pledging it will restrict itself to.
                 skinset = {
                     int(x)
@@ -1265,63 +1272,44 @@
                 filename = prefix + arg.decode('utf8')
             except UnicodeDecodeError:
                 LOGGER.warning("Can't read filename in VScript:", exc_info=True)
                 continue
             self.pack_file(filename, param_type, optional=file.optional)
 
 
-_engine_fgd: Optional[FGD] = None
-
-
-def _get_engine_fgd() -> FGD:
-    """Fetch and cache the engine FGD database."""
-    global _engine_fgd
-    if _engine_fgd is None:
-        _engine_fgd = FGD.engine_dbase()
-    return _engine_fgd
-
-
 def entclass_resources(classname: str) -> Iterable[Tuple[str, FileType]]:
     """Fetch a list of resources this entity class is known to use in code.
 
-    :deprecated: Use :py:func:`EntityDef.engine_cls()` then :py:func:`EntityDef.get_resources()`.
+    :deprecated: Use :py:meth:`EntityDef.engine_def() <srctools.fgd.EntityDef.engine_def>` \
+    then :py:meth:`EntityDef.get_resources() <srctools.fgd.EntityDef.get_resources>`.
     """
     warnings.warn(
-        'Using entclass_resources() is deprecated, access FGD.engine_db() and then '
+        'Using entclass_resources() is deprecated, access EntityDef.engine_cls() and then '
         'EntityDef.get_resources() instead.',
         DeprecationWarning, stacklevel=2,
     )
-    fgd = _get_engine_fgd()
-    try:
-        ent_def = fgd[classname]
-    except KeyError:
-        raise KeyError(classname) from None
-
-    for filetype, filename in ent_def.get_resources(ResourceCtx(fgd=fgd), ent=None):
+    ent_def = EntityDef.engine_def(classname)
+    for filetype, filename in ent_def.get_resources(ResourceCtx(), ent=None):
         yield (filename, filetype)
 
 
 def entclass_canonicalise(classname: str) -> str:
     """Canonicalise classnames - some ents have old classnames for compatibility and the like.
 
-    For example func_movelinear was originally momentary_door. This doesn't include names which
-    have observably different behaviour, like prop_physics_override.
+    For example ``func_movelinear`` was originally ``momentary_door``. This doesn't include names
+    which have observably different behaviour, like ``prop_physics_override``.
 
-    :deprecated: Use :py:func:`FGD.engine_db()`, then check if the entity is an alias.
+    :deprecated: Use :py:meth:`EntityDef.engine_def() <srctools.fgd.EntityDef.engine_def>`, then \
+    check if the entity is an alias.
     """
     warnings.warn(
-        f'Using entclass_packfun() is deprecated, access FGD.engine_db() and then '
-        f'EntityDef.get_resources() instead.',
+        'Using entclass_canonicalise() is deprecated, access EntityDef.engine_def() instead.',
         DeprecationWarning, stacklevel=2,
     )
-    fgd = _get_engine_fgd()
-    try:
-        ent_def = fgd[classname]
-    except KeyError:
-        return classname
+    ent_def = EntityDef.engine_def(classname)
     if ent_def.is_alias:
         try:
             [base] = ent_def.bases
             return base.classname if isinstance(base, EntityDef) else base
         except ValueError:
             pass
     return classname
@@ -1338,24 +1326,19 @@
     :deprecated: Use :py:func:`EntityDef.engine_cls()` then :py:func:`EntityDef.get_resources()`.
     """
     warnings.warn(
         'Using entclass_packfunc() is deprecated, access FGD.engine_db() and then '
         'EntityDef.get_resources() instead.',
         DeprecationWarning, stacklevel=2,
     )
-    fgd = _get_engine_fgd()
-    try:
-        ent_def = fgd[classname]
-    except KeyError:
-        raise KeyError(classname) from None
+    ent_def = EntityDef.engine_def(classname)
 
     def pack_shim(packlist: PackList, ent: Entity) -> None:
         """Translate to old parameters."""
         for filetype, filename in ent_def.get_resources(ResourceCtx(
-            fgd=fgd,
             fsys=packlist.fsys,
         ), ent=ent):
             packlist.pack_file(filename, filetype)
     return pack_shim
 
 
 def entclass_iter() -> Collection[str]:
@@ -1363,12 +1346,8 @@
 
     :deprecated: Use :py:func:`FGD.engine_db()` instead.
     """
     warnings.warn(
         'Using entclass_iter() is deprecated, access FGD.engine_db() instead.',
         DeprecationWarning, stacklevel=2,
     )
-    return [
-        ent.classname
-        for ent in _get_engine_fgd().entities.values()
-        if not isinstance(ent.resources, tuple)
-    ]
+    return EntityDef.engine_classes()
```

### Comparing `srctools-2.3.8/src/srctools/particles.py` & `srctools-2.3.9/src/srctools/particles.py`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/property_parser.py` & `srctools-2.3.9/src/srctools/property_parser.py`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/quickhull.pxd` & `srctools-2.3.9/src/srctools/quickhull.pxd`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/run.py` & `srctools-2.3.9/src/srctools/run.py`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/scripts/collapse_manifest.py` & `srctools-2.3.9/src/srctools/scripts/collapse_manifest.py`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/scripts/diff.py` & `srctools-2.3.9/src/srctools/scripts/diff.py`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/scripts/dump_parms.py` & `srctools-2.3.9/src/srctools/scripts/dump_parms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Dump all the shader parameters from the Source SDK code.
 
 Run with a list of paths pointing to the materialsystem/ folders in the SDK.
 This produces _shaderdb.py
 """
-from typing import Dict, List, Optional, Set
+from typing import Dict, FrozenSet, List, Optional, Set, Union
 from collections import defaultdict
 import ast
 import collections
 import glob
 import sys
 
 import attrs
@@ -19,31 +19,31 @@
 class Var:
     """A shader var."""
     name: str
     type: VarType
     default: object
     help: object
     flags: str
-    filename: str
+    filename: Union[str, FrozenSet[str]]
 
 
 VARS: Dict[str, Var] = {}
 CONFLICTS: Dict[str, Set[Var]] = collections.defaultdict(set)
 
 # Overrides for some vars that have mismatches.
 OVERRIDES: Dict[str, VarType] = {
     'bluramount': VarType.FLOAT,  # Conflict, also int.
     'bloomamount': VarType.VEC4,  # Conflicted, also float.
     # On unlitgeneric is a >dx9 bool, on lightmappedgeneric it's 80, 81, 90, etc.
     'envmapoptional': VarType.INT,
     'color': VarType.COLOR,  # Randomly made vec3 in some shaders.
     'clearcolor': VarType.VEC3,  # Int and vec
     'noisescale': VarType.VEC4,  # Float and Vec4
-    'phongexponent': VarType.FLOAT, # Float and int.
-    # Defined as float in engine_post, but immediately casted to int.
+    'phongexponent': VarType.FLOAT,  # Float and int.
+    # Defined as float in engine_post, but immediately cast to int.
     'num_lookups': VarType.INT,
     'selfillumfresnelminmaxexp': VarType.VEC4,  # 3 or 4 values depending on shader.
     # 4 floats in Character shader, float in lightmappedgeneric
     'detailscale': VarType.VEC4,
     # Generic parameter, int in weapondecal but that's unused.
     'alpha': VarType.FLOAT,
 
@@ -122,30 +122,31 @@
         if var.type == other.type:
             # If the default is different, note that.
             # but we don't care about help etc.
             if var.default != other.default:
                 if isinstance(other.default, frozenset):
                     var = attrs.evolve(var, default=other.default | {var.default})
                 else:
-                    var = attrs.evolve(var, default=frozenset({var.default, other.default}))
+                    var = attrs.evolve(var, default=frozenset({other.default, var.default}))
 
                 if isinstance(other.filename, frozenset):
-                    var = attrs.evolve(var, filename=other.filename | {var.filename})
+                    var = attrs.evolve(var, filename=other.filename | {filename})
                 else:
-                    var = attrs.evolve(var, filename=frozenset({var.filename, other.filename}))
+                    var = attrs.evolve(var, filename=frozenset({other.filename, filename}))
         else:
             # Different types, major issue.
             CONFLICTS[name].add(var)
     VARS[name] = var
 
 
 def dump(folder: str) -> None:
     """Process the materialsystem/ folder from a game repro."""
     for file in glob.iglob(folder + '/**/*'):
-        if not file.endswith(('.h', '.cpp', '.c')): continue
+        if not file.endswith(('.h', '.cpp', '.c')):
+            continue
         with open(file, errors='ignore') as f:
             for line in f:
                 if line.strip() == 'BEGIN_SHADER_PARAMS':
                     break
             else:  # No shader params in this file...
                 continue
```

### Comparing `srctools-2.3.8/src/srctools/scripts/dump_proxies.py` & `srctools-2.3.9/src/srctools/scripts/dump_proxies.py`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/scripts/find_deps.py` & `srctools-2.3.9/src/srctools/scripts/find_deps.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 """Finds dependencies used by resources or maps."""
 from typing import List
 import argparse
 import os
 import sys
 
 from srctools.bsp import BSP
-from srctools.fgd import FGD
 from srctools.filesys import FileSystemChain, RawFileSystem
 from srctools.game import Game
 from srctools.keyvalues import Keyvalues
 from srctools.packlist import PackList
 from srctools.vmf import VMF
 
 
-fgd = FGD.engine_dbase()
-
-
 def main(args: List[str]) -> None:
     """Main script."""
     parser = argparse.ArgumentParser(description=__doc__)
 
     parser.add_argument(
         "-f", "--filter",
         help="filter output to only display resources in this subfolder. "
@@ -84,23 +80,23 @@
         files = [fsys[file_path]]
     for file in files:
         ext = file.path[-4:].casefold()
         if ext == '.vmf':
             with file.open_str() as f:
                 vmf_props = Keyvalues.parse(f)
                 vmf = VMF.parse(vmf_props)
-            packlist.pack_fgd(vmf, fgd)
+            packlist.pack_from_ents(vmf)
             del vmf, vmf_props  # Hefty, don't want to keep.
         elif ext == '.bsp':
             child_sys = fsys.get_system(file)
             if not isinstance(child_sys, RawFileSystem):
                 raise ValueError('Cannot inspect BSPs in VPKs!')
             bsp = BSP(os.path.join(child_sys.path, file.path))
             packlist.pack_from_bsp(bsp)
-            packlist.pack_fgd(bsp.ents, fgd)
+            packlist.pack_from_ents(bsp.ents)
             del bsp
         else:
             packlist.pack_file(file.path)
     print('Evaluating dependencies...')
     packlist.eval_dependencies()
     print('Done.')
```

### Comparing `srctools-2.3.8/src/srctools/scripts/make_model_folders.py` & `srctools-2.3.9/src/srctools/scripts/make_model_folders.py`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/smd.py` & `srctools-2.3.9/src/srctools/smd.py`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/sndscript.py` & `srctools-2.3.9/src/srctools/sndscript.py`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/surfaceprop.py` & `srctools-2.3.9/src/srctools/surfaceprop.py`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/tokenizer.py` & `srctools-2.3.9/src/srctools/tokenizer.py`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/vec.py` & `srctools-2.3.9/src/srctools/vec.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 if TYPE_CHECKING:
     from srctools.math import (
         Angle as Angle, Matrix as Matrix, Vec as Vec, Vec_tuple as Vec_tuple, lerp as lerp,
         parse_vec_str as parse_vec_str, to_matrix as to_matrix,
     )
 else:
     from srctools import math
+
     def __getattr__(name: str) -> object:
         if name in __all__:
             warnings.warn(
                 f'srctools.vec.{name} is renamed to srctools.math.{name}',
                 DeprecationWarning,
                 stacklevel=2,
             )
```

### Comparing `srctools-2.3.8/src/srctools/vmf.py` & `srctools-2.3.9/src/srctools/vmf.py`

 * *Files 0% similar despite different names*

```diff
@@ -598,19 +598,21 @@
         return map_obj
 
     @overload
     def export(
         self, *,
         inc_version: bool=True, minimal: bool=False, disp_multiblend: bool = True,
     ) -> str: ...
+
     @overload
     def export(
         self, dest_file: IO[str], *,
         inc_version: bool=True, minimal: bool=False, disp_multiblend: bool = True,
     ) -> None: ...
+
     def export(
         self,
         dest_file: Optional[IO[str]] = None, *,
         inc_version: bool = True,
         minimal: bool = False,
         disp_multiblend: bool = True,
     ) -> Optional[str]:
@@ -2105,15 +2107,15 @@
 
     scale = property(fset=_scale_setter, doc='Set both scale attributes easily.')
     offset = property(fset=_offset_setter, doc='Set both offset attributes easily.')
     del _scale_setter, _offset_setter
 
 
 class _KeyDict(Dict[str, str]):
-    """Temporary class to allow the Entity.keys dict to be accessed directly, as well as call keys()."""
+    """Temporary class to allow the `Entity.keys` dict to be accessed directly, as well as call keys()."""
     def __call__(self) -> KeysView[str]:
         return self.keys()
 
 
 class Entity(MutableMapping[str, str]):
     """A representation of either a point or brush entity.
 
@@ -2172,26 +2174,28 @@
         self.visgroup_ids = set(vis_ids)
         self.vis_shown = vis_shown
         self.vis_auto_shown = vis_auto_shown
         self.editor_color = Vec(editor_color)
         self.logical_pos = logical_pos or f'[0 {self.id}]'
         self.comments = comments
 
-    @property
-    def keys(self) -> _KeyDict:
-        """Access the internal keyvalues dict.
-
-        This use is deprecated, the entity is a MutableMapping. It can also be called to get
-        a keys view, as with other mappings.
-        """
-        warnings.warn('This is private, use the entity as a mapping.', DeprecationWarning, stacklevel=2)
-        return self._keys
+    if TYPE_CHECKING:
+        # To type checkers, treat as a regular method.
+        def keys(self) -> KeysView[str]: ...
+    else:
+        @property
+        def keys(self) -> _KeyDict:
+            """Access the internal keyvalues dict.
+
+            This use is deprecated, the entity is a MutableMapping. It can also be called to get
+            a keys view, as with other mappings.
+            """
+            warnings.warn('This is private, use the entity as a mapping.', DeprecationWarning, stacklevel=2)
+            return self._keys
 
-    if not TYPE_CHECKING:  # Show as readonly.
-        # noinspection PyDeprecation
         @keys.setter
         def keys(self, value: Dict[str, ValidKVs]) -> None:
             """Deprecated method to replace all keys."""
             warnings.warn('This is private, call .clear_keys() and update().', DeprecationWarning, stacklevel=2)
             self.clear_keys()
             self.update(value)
 
@@ -2495,14 +2499,15 @@
         """Iteration iterates over all keyvalues."""
         return iter(self._keys)
 
     @overload
     def __getitem__(self, key: str) -> str: ...
     @overload
     def __getitem__(self, key: Tuple[str, T]) -> Union[str, T]: ...
+
     def __getitem__(self, key: Union[str, Tuple[str, T]]) -> Union[str, T]:
         """Allow using [] syntax to search for keyvalues.
 
         - This will return '' if the value is not present.
         - It ignores case-matching, but will use the first given version
           of a key.
         - If used via Entity.get() the default argument is available.
@@ -2772,16 +2777,18 @@
 
     def __len__(self) -> int:
         """Return the number of defined keys."""
         return len(self._fixup)
 
     @overload
     def __getitem__(self, key: str) -> str: ...
+
     @overload
     def __getitem__(self, key: Tuple[str, T]) -> Union[str, T]: ...
+
     def __getitem__(self, key: Union[Tuple[str, T], str]) -> Union[str, T]:
         """Retrieve keys via fixup[key] or fixup[key, default].
 
         See EntityFixup.get().
         """
         if isinstance(key, tuple):
             return self.get(key[0], default=key[1])
```

### Comparing `srctools-2.3.8/src/srctools/vmt.py` & `srctools-2.3.9/src/srctools/vmt.py`

 * *Files identical despite different names*

### Comparing `srctools-2.3.8/src/srctools/vpk.py` & `srctools-2.3.9/src/srctools/vpk.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,30 +244,33 @@
     """The VPK filename, without ``_dir.vpk``."""
 
     # fileinfo[extension][directory][filename]
     _fileinfo: Dict[str, Dict[str, Dict[str, FileInfo]]]
 
     mode: OpenModes
     """How the file was opened.
-    
+
     - Read mode, the file will not be modified and it must already exist.
     - Write mode will create the directory if needed.
     - Append mode will also create the directory, but not wipe the file.
     """
 
     dir_limit: Optional[int]
     """
-    The maximum amount of data for files saved to the dir file. 
-    
+    The maximum amount of data for files saved to the dir file.
+
     - :external:py:data:`None`: No limit.
     - ``0``: Save all to a data file.
     """
 
     footer_data: bytes
-    """The block of data after the header, which contains the file data for files stored in the ``_dir`` file, not numeric files."""
+    """
+    The block of data after the header, which contains the file data for files stored in the
+    ``_dir`` file, not numeric files.
+    """
 
     version: int
     """The VPK version, 1 or 2."""
 
     def __init__(
         self,
         dir_file: Union[str, 'os.PathLike[str]'],
@@ -720,15 +723,17 @@
                 if os.path.exists(arch_filename) and os.stat(arch_filename).st_size > arch_len:
                     current_arch += 1
                     arch_filename = get_arch_filename(vpk_name_base, current_arch)
 
 
 # This function requires accumulating a character at a time, parsing the VPK
 # is very slow without a speedup.
+_Py_iter_nullstr = _Cy_iter_nullstr = iter_nullstr
 try:
-    from srctools._tokenizer import _VPK_IterNullstr as iter_nullstr  # type: ignore
+    from srctools._tokenizer import _VPK_IterNullstr as _Cy_iter_nullstr  # type: ignore  # noqa
+    iter_nullstr = _Cy_iter_nullstr
 except ImportError:
     pass
 
 if __name__ == '__main__':
     import sys
     script_write(sys.argv[1:])
```

### Comparing `srctools-2.3.8/src/srctools/vtf.py` & `srctools-2.3.9/src/srctools/vtf.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,14 +351,15 @@
 
         If the VTF is saved, this will be generated from the larger mipmaps.
         """
         self._data = self._fileinfo = None
 
     @overload
     def copy_from(self, source: 'Frame') -> None: ...
+
     @overload
     def copy_from(
         self,
         source: Union[bytes, bytearray, 'array[int]', memoryview],
         format: ImageFormats = ImageFormats.RGBA8888,
     ) -> None: ...
 
@@ -374,15 +375,15 @@
         if isinstance(source, Frame):
             if self.width != source.width or self.height != source.height:
                 raise ValueError("Tried copying from a frame of a different size!")
             source.load()
             assert source._data is not None
             if self._data is None:  # Duplicate the other array
                 self._data = source._data[:]
-            else: # Copy the other array onto us
+            else:  # Copy the other array onto us
                 self._data[:] = source._data
         else:
             if self._data is None:
                 self._data = _BLANK_PIXEL * (self.width * self.height)
             view = memoryview(source)
             # For efficiency, our functions assume the view is contiguous.
             # If it isn't, make a copy to force that.
@@ -1090,13 +1091,13 @@
                 seq_num,
                 seq.clamp,
                 len(seq.frames),
                 seq.duration,
             ))
             for i, (duration, tex_a, tex_b, tex_c, tex_d) in enumerate(seq.frames):
                 file.write(struct.pack('<f4f', duration, *tex_a))
-                if version == 1: # We have an additional 3 coords.
+                if version == 1:  # We have an additional 3 coords.
                     file.write(struct.pack('<4f', *tex_b))
                     file.write(struct.pack('<4f', *tex_c))
                     file.write(struct.pack('<4f', *tex_d))
 
         return file.getvalue()
```

### Comparing `srctools-2.3.8/src/srctools.egg-info/PKG-INFO` & `srctools-2.3.9/src/srctools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srctools
-Version: 2.3.8
+Version: 2.3.9
 Summary: Modules for working with Valve's Source Engine file formats.
 Author-email: TeamSpen210 <spencerb21@live.com>
 License: MIT
 Project-URL: source, https://github.com/TeamSpen210/srctools
 Keywords: Valve,Source Engine
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
```

### Comparing `srctools-2.3.8/src/srctools.egg-info/SOURCES.txt` & `srctools-2.3.9/src/srctools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

