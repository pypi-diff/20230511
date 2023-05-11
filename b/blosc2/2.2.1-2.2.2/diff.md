# Comparing `tmp/blosc2-2.2.1.tar.gz` & `tmp/blosc2-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blosc2-2.2.1.tar", last modified: Wed May 10 12:11:11 2023, max compression
+gzip compressed data, was "blosc2-2.2.2.tar", last modified: Thu May 11 11:48:51 2023, max compression
```

## Comparing `blosc2-2.2.1.tar` & `blosc2-2.2.2.tar`

### file list

```diff
@@ -1,1146 +1,1146 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.442915 blosc2-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 12:08:59.000000 blosc2-2.2.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.786908 blosc2-2.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-10 12:08:59.000000 blosc2-2.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.786908 blosc2-2.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-10 12:08:59.000000 blosc2-2.2.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-05-10 12:08:59.000000 blosc2-2.2.1/.github/workflows/cibuildwheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-10 12:08:59.000000 blosc2-2.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-10 12:08:59.000000 blosc2-2.2.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-10 12:08:59.000000 blosc2-2.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-10 12:08:59.000000 blosc2-2.2.1/ANNOUNCE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-10 12:08:59.000000 blosc2-2.2.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-10 12:08:59.000000 blosc2-2.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-05-10 12:11:11.442915 blosc2-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-05-10 12:08:59.000000 blosc2-2.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-10 12:08:59.000000 blosc2-2.2.1/README_DEVELOPERS.md
--rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-05-10 12:08:59.000000 blosc2-2.2.1/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-10 12:08:59.000000 blosc2-2.2.1/RELEASING.rst
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-10 12:08:59.000000 blosc2-2.2.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.790908 blosc2-2.2.1/bench/
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-10 12:08:59.000000 blosc2-2.2.1/bench/compress_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-10 12:08:59.000000 blosc2-2.2.1/bench/get_slice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.794909 blosc2-2.2.1/bench/ndarray/
--rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-05-10 12:08:59.000000 blosc2-2.2.1/bench/ndarray/compare_getslice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-10 12:08:59.000000 blosc2-2.2.1/bench/ndarray/copy_postfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-10 12:08:59.000000 blosc2-2.2.1/bench/ndarray/download_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.798909 blosc2-2.2.1/bench/ndarray/era5-pds/
--rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-05-10 12:08:59.000000 blosc2-2.2.1/bench/ndarray/era5-pds/measurements-i10k.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-05-10 12:08:59.000000 blosc2-2.2.1/bench/ndarray/era5-pds/measurements-i13k-always-split.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    16476 2023-05-10 12:08:59.000000 blosc2-2.2.1/bench/ndarray/era5-pds/measurements-i13k-never-split.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-05-10 12:08:59.000000 blosc2-2.2.1/bench/ndarray/era5-pds/measurements-i13k.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-05-10 12:08:59.000000 blosc2-2.2.1/bench/ndarray/era5-pds/measurements-m1.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-05-10 12:08:59.000000 blosc2-2.2.1/bench/ndarray/era5-pds/measurements-ryzen3.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    10749 2023-05-10 12:08:59.000000 blosc2-2.2.1/bench/ndarray/plot_transcode_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-10 12:08:59.000000 blosc2-2.2.1/bench/ndarray/transcode_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-10 12:08:59.000000 blosc2-2.2.1/bench/pack_compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-10 12:08:59.000000 blosc2-2.2.1/bench/pack_large.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-10 12:08:59.000000 blosc2-2.2.1/bench/pack_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-10 12:08:59.000000 blosc2-2.2.1/bench/set_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-10 12:08:59.000000 blosc2-2.2.1/bench/sum_postfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.802909 blosc2-2.2.1/blosc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-10 12:08:59.000000 blosc2-2.2.1/blosc2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-05-10 12:08:59.000000 blosc2-2.2.1/blosc2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86462 2023-05-10 12:08:59.000000 blosc2-2.2.1/blosc2/blosc2_ext.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.822909 blosc2-2.2.1/blosc2/c-blosc2/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.822909 blosc2-2.2.1/blosc2/c-blosc2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.822909 blosc2-2.2.1/blosc2/c-blosc2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.822909 blosc2-2.2.1/blosc2/c-blosc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/.github/workflows/cmake.yml
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/.github/workflows/fuzz.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/ANNOUNCE.md
--rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/COMPILING_WITH_WHEELS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/DEVELOPING-GUIDE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/FAQ.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.826909 blosc2-2.2.1/blosc2/c-blosc2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/LICENSES/BITSHUFFLE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/LICENSES/FASTLZ.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/LICENSES/LZ4.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/LICENSES/SNAPPY.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/LICENSES/STDINT.txt
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/LICENSES/ZLIB.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16474 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15951 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/README_ARM.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/README_B2ND_METALAYER.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13926 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/README_CFRAME_FORMAT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/README_CHUNK_FORMAT.rst
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/README_FUZZER.md
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/README_SFRAME_FORMAT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/README_THREADED.rst
--rw-r--r--   0 runner    (1001) docker     (123)    25030 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/RELEASING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/ROADMAP.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/THANKS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/TODO-refactorization.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.834909 blosc2-2.2.1/blosc2/c-blosc2/bench/
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/Makefile.mingw
--rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/b2bench.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.834909 blosc2-2.2.1/blosc2/c-blosc2/bench/b2nd/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/b2nd/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/b2nd/bench_get_slice.c
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/b2nd/bench_zfp_getitem.c
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/create_frame.c
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/delta_schunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/plot-speeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/plot-sum_openmp-results.py
--rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/rainfall-grid-150x150.bin
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/read-grid-150x150.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.838909 blosc2-2.2.1/blosc2/c-blosc2/bench/results-corex/
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/results-corex/blosclz-cl1-sum_openmp-corex.out
--rw-r--r--   0 runner    (1001) docker     (123)    29803 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/results-corex/blosclz-suite-corex.out
--rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/results-corex/lz4-cl1-sum_openmp-corex.out
--rw-r--r--   0 runner    (1001) docker     (123)    29683 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/results-corex/lz4-suite-corex.out
--rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/results-corex/lz4hc-cl1-sum_openmp-corex.out
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/results-corex/zlib-cl1-sum_openmp-corex.out
--rw-r--r--   0 runner    (1001) docker     (123)    11248 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/results-corex/zstd-cl1-sum_openmp-corex.out
--rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/sframe_bench.c
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/sum_openmp.c
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/trunc_prec_schunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/bench/zero_runlen.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.870909 blosc2-2.2.1/blosc2/c-blosc2/blosc/
--rw-r--r--   0 runner    (1001) docker     (123)    12565 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    64093 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/b2nd.c
--rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/b2nd_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/b2nd_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)    21571 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/bitshuffle-altivec.c
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/bitshuffle-altivec.h
--rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/bitshuffle-avx2.c
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/bitshuffle-avx2.h
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/bitshuffle-generic.c
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/bitshuffle-generic.h
--rw-r--r--   0 runner    (1001) docker     (123)    49599 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/bitshuffle-neon.c
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/bitshuffle-neon.h
--rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/bitshuffle-sse2.c
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/bitshuffle-sse2.h
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/blosc-private.h
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/blosc2-stdio.c
--rw-r--r--   0 runner    (1001) docker     (123)   148248 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/blosc2.c
--rw-r--r--   0 runner    (1001) docker     (123)    24299 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/blosclz.c
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/blosclz.h
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/config.h.in
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/context.h
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/delta.c
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/delta.h
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/directories.c
--rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/fastcopy.c
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/fastcopy.h
--rw-r--r--   0 runner    (1001) docker     (123)   115970 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/frame.c
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/frame.h
--rw-r--r--   0 runner    (1001) docker     (123)    56594 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/schunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/sframe.c
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/sframe.h
--rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle-altivec.c
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle-altivec.h
--rw-r--r--   0 runner    (1001) docker     (123)    31608 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle-avx2.c
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle-avx2.h
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle-generic.c
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle-generic.h
--rw-r--r--   0 runner    (1001) docker     (123)    21980 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle-neon.c
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle-neon.h
--rw-r--r--   0 runner    (1001) docker     (123)    26137 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle-sse2.c
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle-sse2.h
--rw-r--r--   0 runner    (1001) docker     (123)    19497 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle.c
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle.h
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/stune.c
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/stune.h
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/timestamp.c
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/transpose-altivec.h
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/trunc-prec.c
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/trunc-prec.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.874909 blosc2-2.2.1/blosc2/c-blosc2/blosc/win32/
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/win32/pthread.c
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/win32/pthread.h
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc/win32/stdint-windows.h
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/blosc2.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.878909 blosc2-2.2.1/blosc2/c-blosc2/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/cmake/FindIPP.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/cmake/FindLZ4.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/cmake/FindSIMD.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/cmake/FindZLIB_NG.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/cmake/FindZSTD.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/cmake/toolchain-aarch64.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/cmake/toolchain-armhf.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/cmake/toolchain-armsf.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/code_of_conduct.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.902910 blosc2-2.2.1/blosc2/c-blosc2/compat/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26736 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.11.1-blosclz.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    33610 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.11.1-lz4.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    32485 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.11.1-lz4hc.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.11.1-zlib.cdata
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.11.1-zstd.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    36256 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.14.0-blosclz.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    36267 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.14.0-lz4.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    36263 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.14.0-lz4hc.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    20530 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.14.0-zlib.cdata
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.14.0-zstd.cdata
--rw-r--r--   0 runner    (1001) docker     (123)   141205 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle4-memcpy.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    22760 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle8-nomemcpy.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    27787 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle4-memcpy.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    22760 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle8-nomemcpy.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    36349 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.3.0-blosclz.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    36267 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.3.0-lz4.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    31963 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.3.0-lz4hc.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    14956 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.3.0-zlib.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    36394 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.7.0-blosclz.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    36267 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.7.0-lz4.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    31963 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.7.0-lz4hc.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    14956 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.7.0-zlib.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    15763 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle4-memcpy.cdata
--rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle8-nomemcpy.cdata
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/compat/filegen.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.902910 blosc2-2.2.1/blosc2/c-blosc2/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.766908 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.906910 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6974 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test1.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    23072 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test16.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     8642 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test2.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    11457 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test4.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    14436 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test8.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.906910 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10706 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    16818 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.906910 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     4846 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.906910 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2262 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     7896 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle
--rwxr-xr-x   0 runner    (1001) docker     (123)     7574 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.906910 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3708 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     7910 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.910910 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5792 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    11472 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.910910 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8199 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    24719 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.910910 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1376 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     4233 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.914910 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2214 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     7559 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.914910 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3616 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    13037 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.914910 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4479 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    15834 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.766908 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.918910 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/Test/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10906 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test16.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2162 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test2.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2769 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test4.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     6545 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test8.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.922910 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     7713 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_bucle.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     4630 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     8365 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.922910 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2577 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.922910 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)      756 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2997 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.926910 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2268 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     4883 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_bucle.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2711 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     6813 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt_bucle.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2010 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     5787 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.930910 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3949 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     7649 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_bucle.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     4177 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     7353 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.930910 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)      656 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2212 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.934910 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle4_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)      770 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle4_neon/unshuffle4_neon.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.934910 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2279 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     5550 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_bucle.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2737 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     4987 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.938910 blosc2-2.2.1/blosc2/c-blosc2/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.938910 blosc2-2.2.1/blosc2/c-blosc2/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/_static/blosc-logo_256.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.938910 blosc2-2.2.1/blosc2/c-blosc2/doc/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/c-blosc2.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.938910 blosc2-2.2.1/blosc2/c-blosc2/doc/development/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/development/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/development/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/development/releasing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/development/roadmap.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.942910 blosc2-2.2.1/blosc2/c-blosc2/doc/format/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/format/cframe_format.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/format/chunk_format.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/format/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/format/sframe_format.rst
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.958910 blosc2-2.2.1/blosc2/c-blosc2/doc/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/reference/b2nd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/reference/blosc1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/reference/context.rst
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/reference/metalayers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/reference/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/reference/schunk.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/reference/utility.rst
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.966910 blosc2-2.2.1/blosc2/c-blosc2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.970910 blosc2-2.2.1/blosc2/c-blosc2/examples/b2nd/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/b2nd/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/b2nd/example_empty_shape.c
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/b2nd/example_frame_generator.c
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/b2nd/example_oindex.c
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/b2nd/example_plainbuffer.c
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/b2nd/example_plugins_codecs.c
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/b2nd/example_plugins_filters.c
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/b2nd/example_print_meta.c
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/b2nd/example_serialize.c
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/compress_file.c
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/contexts.c
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/delta_schunk_ex.c
--rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/find_roots.c
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/frame_backed_schunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/frame_big.c
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/frame_metalayers.c
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/frame_offset.c
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/frame_roundtrip.c
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/frame_simple.c
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/frame_vlmetalayers.c
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/get_set_slice.c
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/instrument_codec.c
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/many_compressors.c
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/multithread.c
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/noinit.c
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/schunk_postfilter.c
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/schunk_simple.c
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/sframe_simple.c
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/simple.c
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/urcodecs.c
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/urfilters.c
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/win-dynamic-linking.c
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/examples/zstd_dict.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.974910 blosc2-2.2.1/blosc2/c-blosc2/images/
--rw-r--r--   0 runner    (1001) docker     (123)   116429 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/images/Complete-Write-Read-B2ND.png
--rw-r--r--   0 runner    (1001) docker     (123)   113029 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/images/Read-Partial-Slices-B2ND.png
--rw-r--r--   0 runner    (1001) docker     (123)   314966 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/images/b2nd-2level-parts.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.974910 blosc2-2.2.1/blosc2/c-blosc2/include/
--rw-r--r--   0 runner    (1001) docker     (123)    19667 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/include/b2nd.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.978910 blosc2-2.2.1/blosc2/c-blosc2/include/blosc2/
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/include/blosc2/blosc2-common.h
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/include/blosc2/blosc2-export.h
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/include/blosc2/blosc2-stdio.h
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/include/blosc2/codecs-registry.h
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/include/blosc2/filters-registry.h
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/include/blosc2/plugins-utils.h
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/include/blosc2/tunes-registry.h
--rw-r--r--   0 runner    (1001) docker     (123)    93522 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/include/blosc2.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.770908 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.014911 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)   113390 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.c
--rw-r--r--   0 runner    (1001) docker     (123)    43263 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.h
--rw-r--r--   0 runner    (1001) docker     (123)    70129 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.c
--rw-r--r--   0 runner    (1001) docker     (123)    20179 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.062911 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/.shellcheckrc
--rw-r--r--   0 runner    (1001) docker     (123)    53620 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/FAQ.zlib
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/INDEX.md
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    13120 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/PORTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32.c
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32_p.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.062911 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.066911 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/adler32_neon.c
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/arm.h
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/armfeature.c
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/chunkset_neon.c
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/crc32_acle.c
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/ctzl.h
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/insert_string_acle.c
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/slide_neon.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.066911 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/generic/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/generic/Makefile.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.070911 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/adler32_power8.c
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/power.c
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/power.h
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/slide_hash_power8.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.074911 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.c
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.h
--rw-r--r--   0 runner    (1001) docker     (123)    15189 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.c
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.h
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_detail.h
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.c
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.074911 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.service
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.766908 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.766908 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.074911 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      991 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/actions-runner
--rwxr-xr-x   0 runner    (1001) docker     (123)      740 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/entrypoint
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/qemu-user-static.service
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.082912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/INDEX.md
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_avx.c
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_ssse3.c
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_avx.c
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_sse.c
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_avx.c
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_sse.c
--rw-r--r--   0 runner    (1001) docker     (123)    16308 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.c
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.h
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/insert_string_sse.c
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_avx.c
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_sse.c
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/x86.c
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/x86.h
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset.c
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset_tpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.090911 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.c
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-coverage.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-install-dirs.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-sanitizer.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-compare.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-redirect.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-compress.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-aarch64.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-arm.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-armhf.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-i686.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-x86_64.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64le.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-s390x.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-sparc64.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compare258.c
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compress.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    63492 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/configure
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32.c
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb.c
--rw-r--r--   0 runner    (1001) docker     (123)    13676 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl._h
--rw-r--r--   0 runner    (1001) docker     (123)    13676 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl.h
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_p.h
--rw-r--r--   0 runner    (1001) docker     (123)    26517 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl._h
--rw-r--r--   0 runner    (1001) docker     (123)    26517 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl.h
--rw-r--r--   0 runner    (1001) docker     (123)    69027 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.c
--rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.h
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_fast.c
--rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_medium.c
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_p.h
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_quick.c
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_slow.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.094912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/algorithm.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20502 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1950.txt
--rw-r--r--   0 runner    (1001) docker     (123)    36944 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1951.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25040 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1952.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/txtvsbin.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/fallback_builtins.h
--rw-r--r--   0 runner    (1001) docker     (123)    14849 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.c
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.h
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzguts.h
--rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzlib.c
--rw-r--r--   0 runner    (1001) docker     (123)    20278 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzread.c
--rw-r--r--   0 runner    (1001) docker     (123)    16106 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzwrite.c
--rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/infback.c
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.c
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.h
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl._h
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl.h
--rw-r--r--   0 runner    (1001) docker     (123)    48765 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.c
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.h
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate_p.h
--rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.c
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.h
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string.c
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string_tpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/match_tpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.106912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.110912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2002-0059/
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2002-0059/test.gz
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2003-0107.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.110912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2004-0797/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2004-0797/test.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.110912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-1849/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-1849/test.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.110912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-2096/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-2096/test.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.110912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/
--rw-r--r--   0 runner    (1001) docker     (123)    48192 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/default.txt
--rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/fixed.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.114912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-361/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-361/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.114912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-364/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-364/test.bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.114912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-382/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-382/defneg3.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.114912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-751/
--rw-r--r--   0 runner    (1001) docker     (123)   180001 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-751/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.114912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-979/
--rw-r--r--   0 runner    (1001) docker     (123)   106840 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-979/pigz-2.6.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.118912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/ignore
--rw-r--r--   0 runner    (1001) docker     (123)    14893 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-arm-linux-gnueabihf.abi
--rw-r--r--   0 runner    (1001) docker     (123)    90251 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-x86_64-linux-gnu.abi
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     4281 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)    35507 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/adler32_test.c
--rw-r--r--   0 runner    (1001) docker     (123)    14167 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/crc32_test.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.122912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)   123093 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/fireworks.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   419233 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/lcet10.txt
--rw-r--r--   0 runner    (1001) docker     (123)   102400 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/paper-100k.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_bi_valid.c
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_block_open.c
--rw-r--r--   0 runner    (1001) docker     (123)    33965 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/example.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.126912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/checksum_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/compress_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_dict_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_flush_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_large_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_small_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/minigzip_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/standalone_fuzz_target_runner.c
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/gh1235.c
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/hash_head_0.c
--rw-r--r--   0 runner    (1001) docker     (123)    26273 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/infcover.c
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/inflate_adler32.c
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minideflate.c
--rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minigzip.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.130912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pigz/
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pigz/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pkgcheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/switchlevels.c
--rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/testCVEinputs.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.130912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/codecov-upload.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      678 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/config.sub
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makecrct.c
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makefixed.c
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/maketrees.c
--rw-r--r--   0 runner    (1001) docker     (123)    31487 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.c
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.h
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_emit.h
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl._h
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/uncompr.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.138912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/
--rw-r--r--   0 runner    (1001) docker     (123)    17920 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/DLL_FAQ.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.a64
--rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.arm
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.msc
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/README-WIN32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng.def
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng1.rc
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib.def
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib1.rc
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlibcompat.def
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zbuild.h
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf-ng.h.in
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.in
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.included
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zendian.h
--rw-r--r--   0 runner    (1001) docker     (123)    94727 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.h
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.map
--rw-r--r--   0 runner    (1001) docker     (123)    94178 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.h
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.map
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.pc.cmakein
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.c
--rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.h
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil_p.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.142912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/BUCK
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.158912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/allocations.h
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bits.h
--rw-r--r--   0 runner    (1001) docker     (123)    17522 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bitstream.h
--rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/compiler.h
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/cpu.h
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.c
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.h
--rw-r--r--   0 runner    (1001) docker     (123)    13308 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/entropy_common.c
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.c
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.h
--rw-r--r--   0 runner    (1001) docker     (123)    30110 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse.h
--rw-r--r--   0 runner    (1001) docker     (123)    12152 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/huf.h
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/mem.h
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.c
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.h
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/portability_macros.h
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.c
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.h
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.c
--rw-r--r--   0 runner    (1001) docker     (123)   212896 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.h
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_common.c
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_deps.h
--rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_trace.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.178912 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/clevels.h
--rw-r--r--   0 runner    (1001) docker     (123)    24096 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/fse_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.c
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.h
--rw-r--r--   0 runner    (1001) docker     (123)    57710 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/huf_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)   312776 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)    64416 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.c
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.h
--rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.c
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.h
--rw-r--r--   0 runner    (1001) docker     (123)    28499 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.c
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.h
--rw-r--r--   0 runner    (1001) docker     (123)    27872 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_cwksp.h
--rw-r--r--   0 runner    (1001) docker     (123)    34479 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.c
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.h
--rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.c
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.h
--rw-r--r--   0 runner    (1001) docker     (123)   101952 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.c
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.h
--rw-r--r--   0 runner    (1001) docker     (123)    28437 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.c
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.h
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm_geartab.h
--rw-r--r--   0 runner    (1001) docker     (123)    67459 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.c
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.h
--rw-r--r--   0 runner    (1001) docker     (123)    81334 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.186913 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/
--rw-r--r--   0 runner    (1001) docker     (123)    73701 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress_amd64.S
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.c
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.h
--rw-r--r--   0 runner    (1001) docker     (123)    99701 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)    99641 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.c
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.h
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_internal.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.190913 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/
--rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff.h
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_common.c
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_decompress.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.194913 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/
--rw-r--r--   0 runner    (1001) docker     (123)    42898 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.c
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.h
--rw-r--r--   0 runner    (1001) docker     (123)    54649 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.h
--rw-r--r--   0 runner    (1001) docker     (123)    28561 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/fastcover.c
--rw-r--r--   0 runner    (1001) docker     (123)    44008 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/zdict.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.770908 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.194913 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.sln
--rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.vcxproj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.210913 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)    14318 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_legacy.h
--rw-r--r--   0 runner    (1001) docker     (123)    69465 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.c
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.h
--rw-r--r--   0 runner    (1001) docker     (123)   125639 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.c
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.h
--rw-r--r--   0 runner    (1001) docker     (123)   111749 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.c
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.h
--rw-r--r--   0 runner    (1001) docker     (123)   132791 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.c
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.h
--rw-r--r--   0 runner    (1001) docker     (123)   153658 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.c
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.h
--rw-r--r--   0 runner    (1001) docker     (123)   163699 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.c
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.h
--rw-r--r--   0 runner    (1001) docker     (123)   182559 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.c
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.h
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/libzstd.mk
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/libzstd.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/module.modulemap
--rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zdict.h
--rw-r--r--   0 runner    (1001) docker     (123)   171378 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd_errors.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.210913 blosc2-2.2.1/blosc2/c-blosc2/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.214913 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/codecs-registry.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.218913 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz-private.h
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.c
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.h
--rw-r--r--   0 runner    (1001) docker     (123)    22831 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.c
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.h
--rw-r--r--   0 runner    (1001) docker     (123)    19036 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.c
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.h
--rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/test_ndlz.c
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.c
--rw-r--r--   0 runner    (1001) docker     (123)   205061 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.230913 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    26401 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.c
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.230913 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/include/
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/include/bitstream.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.234913 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/macros.h
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/system.h
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/types.h
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/version.h
--rw-r--r--   0 runner    (1001) docker     (123)    34968 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.254913 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/bitstream.c
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/block1.h
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/block2.h
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/block3.h
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/block4.h
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1d.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1f.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1i.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1l.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2d.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2f.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2i.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2l.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3d.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3f.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3i.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3l.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4d.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4f.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4i.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4l.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1d.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1f.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1i.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1l.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2d.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2f.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2i.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2l.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3d.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3f.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3i.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3l.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4d.c
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4f.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4i.c
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4l.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.258913 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/
--rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/bitstream.c
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/inline.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.258913 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/share/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/share/omp.c
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/share/parallel.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.278913 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec.c
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec.h
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec1.c
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec2.c
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec3.c
--rw-r--r--   0 runner    (1001) docker     (123)     9466 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec4.c
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codecf.c
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/compress.c
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode.c
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode1.c
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode2.c
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode3.c
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode4.c
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decodef.c
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decodei.c
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode.c
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode1.c
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode2.c
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode3.c
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode4.c
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodef.c
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodei.c
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/ompcompress.c
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revcodecf.c
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode.c
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode1.c
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode2.c
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode3.c
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode4.c
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecodef.c
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode.c
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode1.c
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode2.c
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode3.c
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode4.c
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencodef.c
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/template.h
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsd.h
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsf.h
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsi.h
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsl.h
--rw-r--r--   0 runner    (1001) docker     (123)    32747 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/zfp.c
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_acc_float.c
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_prec_float.c
--rw-r--r--   0 runner    (1001) docker     (123)    10268 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_float.c
--rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_getitem.c
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/zfp-private.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.278913 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.282914 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/bytedelta/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/bytedelta/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.c
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.h
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/bytedelta/test_bytedelta.c
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/filters-registry.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.286913 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndcell/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndcell/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndcell/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.c
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.h
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndcell/test_ndcell.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.286913 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndmean/
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndmean/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndmean/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.c
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.h
--rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_mean.c
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_repart.c
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/plugin_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/plugin_utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.290914 blosc2-2.2.1/blosc2/c-blosc2/plugins/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/test_data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/test_data/example_day_month_temp.b2nd
--rw-r--r--   0 runner    (1001) docker     (123)   141455 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/test_data/example_item_prices.b2nd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.290914 blosc2-2.2.1/blosc2/c-blosc2/plugins/tunes/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/tunes/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/plugins/tunes/tunes-registry.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.330914 blosc2-2.2.1/blosc2/c-blosc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.342914 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/cutest.h
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_append.c
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_copy.c
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_delete.c
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_full.c
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice.c
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice_buffer.c
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_insert.c
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_metalayers.c
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_open_offset.c
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_persistency.c
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_resize.c
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_roundtrip.c
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_save.c
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_serialize.c
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_set_slice_buffer.c
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze.c
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze_index.c
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_uninit.c
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_zeros.c
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_common.h
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/cutest.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.350914 blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.354914 blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/corpus/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/corpus/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    33187 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-blosclz.b2frame
--rw-r--r--   0 runner    (1001) docker     (123)    41393 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4.b2frame
--rw-r--r--   0 runner    (1001) docker     (123)    24087 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4hc.b2frame
--rw-r--r--   0 runner    (1001) docker     (123)    21570 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zlib.b2frame
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zstd.b2frame
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/fuzz_compress_chunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/fuzz_compress_frame.c
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_chunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_frame.c
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/generate_inputs_corpus.c
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/standalone.c
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/gcc-segfault-issue.c
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/print_versions.c
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_all.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_api.c
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_bitshuffle_leftovers.c
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_blosc1_compat.c
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_change_nthreads_append.c
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_common.h
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_compress_roundtrip.c
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_compress_roundtrip.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_compressor.c
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_contexts.c
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_copy.c
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_delete_chunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_delta.c
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_delta_schunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_dict_schunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_empty_buffer.c
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_fill_special.c
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_frame.c
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_frame_get_offsets.c
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_frame_offset.c
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_get_slice_buffer.c
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_getitem.c
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_getitem.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_getitem_delta.c
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_insert_chunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_lazychunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_lazychunk_memcpyed.c
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_maskout.c
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_maxout.c
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_noinit.c
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_nolock.c
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_nthreads.c
--rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_postfilter.c
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_prefilter.c
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_reorder_offsets.c
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_schunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_schunk_frame.c
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_schunk_header.c
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_set_slice_buffer.c
--rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_sframe.c
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_sframe_lazychunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.c
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.c
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.c
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.c
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.c
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_small_chunks.c
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_udio.c
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_update_chunk.c
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_urcodecs.c
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_urfilters.c
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-10 12:09:00.000000 blosc2-2.2.1/blosc2/c-blosc2/tests/test_zero_runlen.c
--rw-r--r--   0 runner    (1001) docker     (123)    45909 2023-05-10 12:08:59.000000 blosc2-2.2.1/blosc2/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-10 12:08:59.000000 blosc2-2.2.1/blosc2/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    19583 2023-05-10 12:08:59.000000 blosc2-2.2.1/blosc2/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    29890 2023-05-10 12:08:59.000000 blosc2-2.2.1/blosc2/schunk.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 12:11:10.000000 blosc2-2.2.1/blosc2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.806909 blosc2-2.2.1/blosc2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-05-10 12:11:10.000000 blosc2-2.2.1/blosc2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    52219 2023-05-10 12:11:10.000000 blosc2-2.2.1/blosc2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:11:10.000000 blosc2-2.2.1/blosc2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 12:11:10.000000 blosc2-2.2.1/blosc2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 12:11:10.000000 blosc2-2.2.1/blosc2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-10 12:08:59.000000 blosc2-2.2.1/code_of_conduct.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.354914 blosc2-2.2.1/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.358914 blosc2-2.2.1/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/_static/blosc-logo_128.png
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/_static/blosc-logo_256.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.358914 blosc2-2.2.1/doc/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/python-blosc2.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.362914 blosc2-2.2.1/doc/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:10.770908 blosc2-2.2.1/doc/reference/autofiles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.374915 blosc2-2.2.1/doc/reference/autofiles/schunk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.382915 blosc2-2.2.1/doc/reference/autofiles/schunk/attributes/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.blocksize.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.cbytes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.chunkshape.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.chunksize.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.contiguous.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.cparams.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.cratio.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.dparams.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.nbytes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.typesize.rst
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.urlpath.rst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/attributes/meta.rst
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/attributes/vlmeta.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.__getitem__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.__setitem__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.append_data.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.decompress_chunk.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.delete_chunk.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.filler.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.get_chunk.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.get_slice.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.insert_chunk.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.insert_data.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.iterchunks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.postfilter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.prefilter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.remove_postfilter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.remove_prefilter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.to_cframe.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.update_chunk.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.update_data.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.386915 blosc2-2.2.1/doc/reference/autofiles/top_level/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/top_level/blosc2.Codec.rst
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/top_level/blosc2.Filter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/top_level/blosc2.SplitMode.rst
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/autofiles/top_level/blosc2.nthreads.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/ndarray_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/schunk_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/top_level.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/reference/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.386915 blosc2-2.2.1/doc/release_notes/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-10 12:08:59.000000 blosc2-2.2.1/doc/release_notes/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.394915 blosc2-2.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/compress2_decompress2.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/compress_decompress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/filler.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/gil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.398915 blosc2-2.2.1/examples/images/
--rw-r--r--   0 runner    (1001) docker     (123)   335474 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/images/blosc2-pipeline.png
--rw-r--r--   0 runner    (1001) docker     (123)    46143 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/images/blosc2-pipeline.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.406915 blosc2-2.2.1/examples/images/ucodecs-filters/
--rw-r--r--   0 runner    (1001) docker     (123)   107624 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/images/ucodecs-filters/backward.png
--rw-r--r--   0 runner    (1001) docker     (123)    38548 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/images/ucodecs-filters/backward.svg
--rw-r--r--   0 runner    (1001) docker     (123)    31483 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/images/ucodecs-filters/decoder.svg
--rw-r--r--   0 runner    (1001) docker     (123)    35540 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/images/ucodecs-filters/decoder2.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23248 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/images/ucodecs-filters/encoder.svg
--rw-r--r--   0 runner    (1001) docker     (123)    24481 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/images/ucodecs-filters/encoder2.svg
--rw-r--r--   0 runner    (1001) docker     (123)   110817 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/images/ucodecs-filters/forward.png
--rw-r--r--   0 runner    (1001) docker     (123)    41521 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/images/ucodecs-filters/forward.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.410915 blosc2-2.2.1/examples/ndarray/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/ndarray/asarray.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/ndarray/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/ndarray/bytedelta_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/ndarray/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/ndarray/empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/ndarray/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/ndarray/getitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/ndarray/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/ndarray/ndmean.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/ndarray/persistency.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/ndarray/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/ndarray/work_with_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/ndarray/zfp_codec.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/pack_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/pack_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/postfilter1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/postfilter2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/postfilter3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/postfilters.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/prefilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/prefilters.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/save_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/schunk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/schunk_roundtrip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/slicing_and_beyond.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/tutorial-basics.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/ucodecs-ufilters.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (123)     2114 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/ucodecs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/ufilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-10 12:08:59.000000 blosc2-2.2.1/examples/vlmeta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.418915 blosc2-2.2.1/images/
--rw-r--r--   0 runner    (1001) docker     (123)   116429 2023-05-10 12:08:59.000000 blosc2-2.2.1/images/Complete-Write-Read-B2ND.png
--rw-r--r--   0 runner    (1001) docker     (123)    64898 2023-05-10 12:08:59.000000 blosc2-2.2.1/images/M1-i386-vs-arm64-pack.png
--rw-r--r--   0 runner    (1001) docker     (123)    62528 2023-05-10 12:08:59.000000 blosc2-2.2.1/images/M1-i386-vs-arm64-unpack.png
--rw-r--r--   0 runner    (1001) docker     (123)   113029 2023-05-10 12:08:59.000000 blosc2-2.2.1/images/Read-Partial-Slices-B2ND.png
--rw-r--r--   0 runner    (1001) docker     (123)   314966 2023-05-10 12:08:59.000000 blosc2-2.2.1/images/b2nd-2level-parts.png
--rw-r--r--   0 runner    (1001) docker     (123)    77813 2023-05-10 12:08:59.000000 blosc2-2.2.1/images/linspace-compress.png
--rw-r--r--   0 runner    (1001) docker     (123)    24888 2023-05-10 12:08:59.000000 blosc2-2.2.1/images/linspace-decompress.png
--rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-05-10 12:08:59.000000 blosc2-2.2.1/images/pack-array-cratios.png
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-10 12:08:59.000000 blosc2-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-10 12:08:59.000000 blosc2-2.2.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 12:08:59.000000 blosc2-2.2.1/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-10 12:08:59.000000 blosc2-2.2.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-10 12:08:59.000000 blosc2-2.2.1/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 12:08:59.000000 blosc2-2.2.1/requirements-runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 12:08:59.000000 blosc2-2.2.1/requirements-test-wheels.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-10 12:08:59.000000 blosc2-2.2.1/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:11:11.442915 blosc2-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-10 12:08:59.000000 blosc2-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.434915 blosc2-2.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:11:11.442915 blosc2-2.2.1/tests/ndarray/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/ndarray/persistency.cat
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/ndarray/test_auto_parts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/ndarray/test_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/ndarray/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/ndarray/test_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/ndarray/test_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/ndarray/test_getitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/ndarray/test_lossy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/ndarray/test_metalayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/ndarray/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/ndarray/test_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/ndarray/test_persistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/ndarray/test_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/ndarray/test_setitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/ndarray/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/ndarray/test_squeeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/ndarray/test_struct_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/ndarray/test_zeros.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_bytes_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_comp_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_compress2.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_compression_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_compressors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_decompress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_iterchunks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_postfilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_prefilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_python_blosc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_schunk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_schunk_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_schunk_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_schunk_get_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_schunk_insert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_schunk_set_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_schunk_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_ucodecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_ufilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-10 12:08:59.000000 blosc2-2.2.1/tests/test_vlmeta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.427007 blosc2-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-11 11:46:32.000000 blosc2-2.2.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.079001 blosc2-2.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-11 11:46:32.000000 blosc2-2.2.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.079001 blosc2-2.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-11 11:46:32.000000 blosc2-2.2.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-11 11:46:32.000000 blosc2-2.2.2/.github/workflows/cibuildwheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-11 11:46:32.000000 blosc2-2.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-11 11:46:32.000000 blosc2-2.2.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-11 11:46:32.000000 blosc2-2.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-11 11:46:32.000000 blosc2-2.2.2/ANNOUNCE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-11 11:46:32.000000 blosc2-2.2.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-11 11:46:32.000000 blosc2-2.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-05-11 11:48:51.427007 blosc2-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-05-11 11:46:32.000000 blosc2-2.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-11 11:46:32.000000 blosc2-2.2.2/README_DEVELOPERS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-05-11 11:46:32.000000 blosc2-2.2.2/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-11 11:46:32.000000 blosc2-2.2.2/RELEASING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 11:46:32.000000 blosc2-2.2.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.083001 blosc2-2.2.2/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-11 11:46:32.000000 blosc2-2.2.2/bench/compress_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-11 11:46:32.000000 blosc2-2.2.2/bench/get_slice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.083001 blosc2-2.2.2/bench/ndarray/
+-rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-05-11 11:46:32.000000 blosc2-2.2.2/bench/ndarray/compare_getslice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-11 11:46:32.000000 blosc2-2.2.2/bench/ndarray/copy_postfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-11 11:46:32.000000 blosc2-2.2.2/bench/ndarray/download_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.087001 blosc2-2.2.2/bench/ndarray/era5-pds/
+-rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-05-11 11:46:32.000000 blosc2-2.2.2/bench/ndarray/era5-pds/measurements-i10k.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-05-11 11:46:32.000000 blosc2-2.2.2/bench/ndarray/era5-pds/measurements-i13k-always-split.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    16476 2023-05-11 11:46:32.000000 blosc2-2.2.2/bench/ndarray/era5-pds/measurements-i13k-never-split.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-05-11 11:46:32.000000 blosc2-2.2.2/bench/ndarray/era5-pds/measurements-i13k.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-05-11 11:46:32.000000 blosc2-2.2.2/bench/ndarray/era5-pds/measurements-m1.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-05-11 11:46:32.000000 blosc2-2.2.2/bench/ndarray/era5-pds/measurements-ryzen3.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    10749 2023-05-11 11:46:32.000000 blosc2-2.2.2/bench/ndarray/plot_transcode_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-11 11:46:32.000000 blosc2-2.2.2/bench/ndarray/transcode_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-11 11:46:32.000000 blosc2-2.2.2/bench/pack_compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-11 11:46:32.000000 blosc2-2.2.2/bench/pack_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-11 11:46:32.000000 blosc2-2.2.2/bench/pack_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-11 11:46:32.000000 blosc2-2.2.2/bench/set_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-11 11:46:32.000000 blosc2-2.2.2/bench/sum_postfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.091001 blosc2-2.2.2/blosc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-11 11:46:32.000000 blosc2-2.2.2/blosc2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-05-11 11:46:32.000000 blosc2-2.2.2/blosc2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86462 2023-05-11 11:46:32.000000 blosc2-2.2.2/blosc2/blosc2_ext.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.099002 blosc2-2.2.2/blosc2/c-blosc2/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.099002 blosc2-2.2.2/blosc2/c-blosc2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.099002 blosc2-2.2.2/blosc2/c-blosc2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.103002 blosc2-2.2.2/blosc2/c-blosc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/.github/workflows/cmake.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/.github/workflows/fuzz.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/ANNOUNCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/COMPILING_WITH_WHEELS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/DEVELOPING-GUIDE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/FAQ.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.103002 blosc2-2.2.2/blosc2/c-blosc2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/LICENSES/BITSHUFFLE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/LICENSES/FASTLZ.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/LICENSES/LZ4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/LICENSES/SNAPPY.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/LICENSES/STDINT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/LICENSES/ZLIB.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16474 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15951 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/README_ARM.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/README_B2ND_METALAYER.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13926 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/README_CFRAME_FORMAT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/README_CHUNK_FORMAT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/README_FUZZER.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/README_SFRAME_FORMAT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/README_THREADED.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25030 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/RELEASING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/ROADMAP.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/THANKS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/TODO-refactorization.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.107002 blosc2-2.2.2/blosc2/c-blosc2/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/Makefile.mingw
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/b2bench.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.111002 blosc2-2.2.2/blosc2/c-blosc2/bench/b2nd/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/b2nd/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/b2nd/bench_get_slice.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/b2nd/bench_zfp_getitem.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/create_frame.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/delta_schunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/plot-speeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/plot-sum_openmp-results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/rainfall-grid-150x150.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/read-grid-150x150.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.111002 blosc2-2.2.2/blosc2/c-blosc2/bench/results-corex/
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/results-corex/blosclz-cl1-sum_openmp-corex.out
+-rw-r--r--   0 runner    (1001) docker     (123)    29803 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/results-corex/blosclz-suite-corex.out
+-rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/results-corex/lz4-cl1-sum_openmp-corex.out
+-rw-r--r--   0 runner    (1001) docker     (123)    29683 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/results-corex/lz4-suite-corex.out
+-rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/results-corex/lz4hc-cl1-sum_openmp-corex.out
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/results-corex/zlib-cl1-sum_openmp-corex.out
+-rw-r--r--   0 runner    (1001) docker     (123)    11248 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/results-corex/zstd-cl1-sum_openmp-corex.out
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/sframe_bench.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/sum_openmp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/trunc_prec_schunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/bench/zero_runlen.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.131002 blosc2-2.2.2/blosc2/c-blosc2/blosc/
+-rw-r--r--   0 runner    (1001) docker     (123)    12565 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    64093 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/b2nd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/b2nd_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/b2nd_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21571 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/bitshuffle-altivec.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/bitshuffle-altivec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/bitshuffle-avx2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/bitshuffle-avx2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/bitshuffle-generic.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/bitshuffle-generic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    49599 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/bitshuffle-neon.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/bitshuffle-neon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/bitshuffle-sse2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/bitshuffle-sse2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/blosc-private.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/blosc2-stdio.c
+-rw-r--r--   0 runner    (1001) docker     (123)   148248 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/blosc2.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24299 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/blosclz.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/blosclz.h
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/config.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/context.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/delta.c
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/delta.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/directories.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/fastcopy.c
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/fastcopy.h
+-rw-r--r--   0 runner    (1001) docker     (123)   115970 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/frame.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/frame.h
+-rw-r--r--   0 runner    (1001) docker     (123)    56594 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/schunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/sframe.c
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/sframe.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle-altivec.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle-altivec.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31608 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle-avx2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle-avx2.h
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle-generic.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle-generic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21980 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle-neon.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle-neon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26137 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle-sse2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle-sse2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19497 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/stune.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/stune.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/timestamp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/transpose-altivec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/trunc-prec.c
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/trunc-prec.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.131002 blosc2-2.2.2/blosc2/c-blosc2/blosc/win32/
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/win32/pthread.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/win32/pthread.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc/win32/stdint-windows.h
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/blosc2.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.135002 blosc2-2.2.2/blosc2/c-blosc2/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/cmake/FindIPP.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/cmake/FindLZ4.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/cmake/FindSIMD.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/cmake/FindZLIB_NG.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/cmake/FindZSTD.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/cmake/toolchain-aarch64.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/cmake/toolchain-armhf.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/cmake/toolchain-armsf.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/code_of_conduct.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.147002 blosc2-2.2.2/blosc2/c-blosc2/compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26736 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.11.1-blosclz.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    33610 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.11.1-lz4.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    32485 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.11.1-lz4hc.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.11.1-zlib.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.11.1-zstd.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    36256 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.14.0-blosclz.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    36267 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.14.0-lz4.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    36263 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.14.0-lz4hc.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    20530 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.14.0-zlib.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.14.0-zstd.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)   141205 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle4-memcpy.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    22760 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle8-nomemcpy.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    27787 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle4-memcpy.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    22760 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle8-nomemcpy.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    36349 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.3.0-blosclz.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    36267 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.3.0-lz4.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    31963 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.3.0-lz4hc.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    14956 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.3.0-zlib.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    36394 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.7.0-blosclz.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    36267 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.7.0-lz4.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    31963 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.7.0-lz4hc.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    14956 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.7.0-zlib.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    15763 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle4-memcpy.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle8-nomemcpy.cdata
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/compat/filegen.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.147002 blosc2-2.2.2/blosc2/c-blosc2/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.067001 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.151003 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6974 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test1.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23072 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test16.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8642 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test2.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11457 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test4.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14436 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test8.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.151003 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10706 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16818 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.151003 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4846 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.155002 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2262 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7896 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7574 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.155002 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3708 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7910 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.155002 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5792 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11472 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.155002 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8199 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24719 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.155002 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1376 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4233 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.159003 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2214 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7559 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.159003 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3616 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13037 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.159003 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4479 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15834 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.067001 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.159003 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/Test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10906 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test16.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2162 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test2.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2769 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test4.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6545 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test8.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.163003 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7713 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_bucle.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4630 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8365 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.163003 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2577 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.163003 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      756 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2997 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.167003 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2268 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4883 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_bucle.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2711 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6813 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt_bucle.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2010 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5787 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.167003 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3949 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7649 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_bucle.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4177 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7353 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.167003 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      656 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2212 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.167003 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle4_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      770 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle4_neon/unshuffle4_neon.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.171003 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2279 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5550 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_bucle.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2737 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4987 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.171003 blosc2-2.2.2/blosc2/c-blosc2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.171003 blosc2-2.2.2/blosc2/c-blosc2/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/_static/blosc-logo_256.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.171003 blosc2-2.2.2/blosc2/c-blosc2/doc/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/c-blosc2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.175003 blosc2-2.2.2/blosc2/c-blosc2/doc/development/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/development/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/development/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/development/releasing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/development/roadmap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.175003 blosc2-2.2.2/blosc2/c-blosc2/doc/format/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/format/cframe_format.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/format/chunk_format.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/format/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/format/sframe_format.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.175003 blosc2-2.2.2/blosc2/c-blosc2/doc/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/reference/b2nd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/reference/blosc1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/reference/context.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/reference/metalayers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/reference/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/reference/schunk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/reference/utility.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.183003 blosc2-2.2.2/blosc2/c-blosc2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.187003 blosc2-2.2.2/blosc2/c-blosc2/examples/b2nd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/b2nd/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/b2nd/example_empty_shape.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/b2nd/example_frame_generator.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/b2nd/example_oindex.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/b2nd/example_plainbuffer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/b2nd/example_plugins_codecs.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/b2nd/example_plugins_filters.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/b2nd/example_print_meta.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/b2nd/example_serialize.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/compress_file.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/contexts.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/delta_schunk_ex.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/find_roots.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/frame_backed_schunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/frame_big.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/frame_metalayers.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/frame_offset.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/frame_roundtrip.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/frame_simple.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/frame_vlmetalayers.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/get_set_slice.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/instrument_codec.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/many_compressors.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/multithread.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/noinit.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/schunk_postfilter.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/schunk_simple.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/sframe_simple.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/simple.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/urcodecs.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/urfilters.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/win-dynamic-linking.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/examples/zstd_dict.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.191003 blosc2-2.2.2/blosc2/c-blosc2/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   116429 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/images/Complete-Write-Read-B2ND.png
+-rw-r--r--   0 runner    (1001) docker     (123)   113029 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/images/Read-Partial-Slices-B2ND.png
+-rw-r--r--   0 runner    (1001) docker     (123)   314966 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/images/b2nd-2level-parts.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.191003 blosc2-2.2.2/blosc2/c-blosc2/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    19667 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/include/b2nd.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.195003 blosc2-2.2.2/blosc2/c-blosc2/include/blosc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/include/blosc2/blosc2-common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/include/blosc2/blosc2-export.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/include/blosc2/blosc2-stdio.h
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/include/blosc2/codecs-registry.h
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/include/blosc2/filters-registry.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/include/blosc2/plugins-utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/include/blosc2/tunes-registry.h
+-rw-r--r--   0 runner    (1001) docker     (123)    93522 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/include/blosc2.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.071001 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.195003 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)   113390 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43263 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.h
+-rw-r--r--   0 runner    (1001) docker     (123)    70129 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20179 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.223003 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/.shellcheckrc
+-rw-r--r--   0 runner    (1001) docker     (123)    53620 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/FAQ.zlib
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/INDEX.md
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13120 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/PORTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32_p.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.223003 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.223003 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/adler32_neon.c
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/arm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/armfeature.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/chunkset_neon.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/crc32_acle.c
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/ctzl.h
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/insert_string_acle.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/slide_neon.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.223003 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/generic/Makefile.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.227004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/adler32_power8.c
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/power.c
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/power.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/slide_hash_power8.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.227004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15189 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_detail.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.231004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.service
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.071001 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.071001 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.231004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      991 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/actions-runner
+-rwxr-xr-x   0 runner    (1001) docker     (123)      740 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/entrypoint
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/qemu-user-static.service
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.235004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/INDEX.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_avx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_ssse3.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_avx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_sse.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_avx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_sse.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16308 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.c
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/insert_string_sse.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_avx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_sse.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/x86.c
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/x86.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset_tpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.239004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-coverage.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-install-dirs.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-sanitizer.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-compare.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-redirect.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-compress.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-aarch64.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-arm.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-armhf.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-i686.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-x86_64.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64le.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-s390x.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-sparc64.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compare258.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compress.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    63492 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/configure
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13676 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl._h
+-rw-r--r--   0 runner    (1001) docker     (123)    13676 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl.h
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_p.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26517 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl._h
+-rw-r--r--   0 runner    (1001) docker     (123)    26517 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    69027 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_fast.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_medium.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_p.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_quick.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_slow.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.243004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/algorithm.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20502 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1950.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    36944 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1951.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25040 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1952.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/txtvsbin.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/fallback_builtins.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14849 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzguts.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzlib.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20278 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzread.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16106 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzwrite.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/infback.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.c
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl._h
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48765 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate_p.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.h
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string_tpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/match_tpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.247004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.247004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2002-0059/
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2002-0059/test.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2003-0107.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.247004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2004-0797/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2004-0797/test.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.247004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-1849/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-1849/test.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.247004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-2096/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-2096/test.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.251004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/
+-rw-r--r--   0 runner    (1001) docker     (123)    48192 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/default.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/fixed.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.251004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-361/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-361/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.251004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-364/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-364/test.bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.251004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-382/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-382/defneg3.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.251004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-751/
+-rw-r--r--   0 runner    (1001) docker     (123)   180001 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-751/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.251004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-979/
+-rw-r--r--   0 runner    (1001) docker     (123)   106840 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-979/pigz-2.6.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.255004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/ignore
+-rw-r--r--   0 runner    (1001) docker     (123)    14893 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-arm-linux-gnueabihf.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    90251 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-x86_64-linux-gnu.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4281 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    35507 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/adler32_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14167 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/crc32_test.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.259004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   123093 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/fireworks.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   419233 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/lcet10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   102400 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/paper-100k.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_bi_valid.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_block_open.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33965 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/example.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.259004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/checksum_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/compress_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_dict_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_flush_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_large_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_small_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/minigzip_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/standalone_fuzz_target_runner.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/gh1235.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/hash_head_0.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26273 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/infcover.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/inflate_adler32.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minideflate.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minigzip.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.259004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pigz/
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pigz/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pkgcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/switchlevels.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/testCVEinputs.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.263004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/codecov-upload.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      678 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/config.sub
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makecrct.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makefixed.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/maketrees.c
+-rw-r--r--   0 runner    (1001) docker     (123)    31487 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_emit.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl._h
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/uncompr.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.263004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/
+-rw-r--r--   0 runner    (1001) docker     (123)    17920 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/DLL_FAQ.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.a64
+-rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.arm
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.msc
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/README-WIN32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng.def
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng1.rc
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib.def
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib1.rc
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlibcompat.def
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zbuild.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf-ng.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.included
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zendian.h
+-rw-r--r--   0 runner    (1001) docker     (123)    94727 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.map
+-rw-r--r--   0 runner    (1001) docker     (123)    94178 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.map
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.pc.cmakein
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil_p.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.267004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/BUCK
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.279004 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/allocations.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bits.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17522 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bitstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/compiler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/cpu.h
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13308 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/entropy_common.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30110 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12152 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/huf.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/mem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/portability_macros.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.h
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.c
+-rw-r--r--   0 runner    (1001) docker     (123)   212896 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_common.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_deps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_trace.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.291005 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/clevels.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24096 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/fse_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57710 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/huf_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)   312776 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    64416 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28499 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27872 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_cwksp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34479 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.h
+-rw-r--r--   0 runner    (1001) docker     (123)   101952 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28437 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm_geartab.h
+-rw-r--r--   0 runner    (1001) docker     (123)    67459 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    81334 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.295005 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/
+-rw-r--r--   0 runner    (1001) docker     (123)    73701 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress_amd64.S
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.h
+-rw-r--r--   0 runner    (1001) docker     (123)    99701 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    99641 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.295005 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_common.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_decompress.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.299005 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)    42898 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.h
+-rw-r--r--   0 runner    (1001) docker     (123)    54649 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28561 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/fastcover.c
+-rw-r--r--   0 runner    (1001) docker     (123)    44008 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/zdict.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.071001 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.299005 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.sln
+-rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.vcxproj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.307005 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)    14318 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_legacy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    69465 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.h
+-rw-r--r--   0 runner    (1001) docker     (123)   125639 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.h
+-rw-r--r--   0 runner    (1001) docker     (123)   111749 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.h
+-rw-r--r--   0 runner    (1001) docker     (123)   132791 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.h
+-rw-r--r--   0 runner    (1001) docker     (123)   153658 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.h
+-rw-r--r--   0 runner    (1001) docker     (123)   163699 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.h
+-rw-r--r--   0 runner    (1001) docker     (123)   182559 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/libzstd.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/libzstd.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/module.modulemap
+-rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zdict.h
+-rw-r--r--   0 runner    (1001) docker     (123)   171378 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd_errors.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.311005 blosc2-2.2.2/blosc2/c-blosc2/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.311005 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/codecs-registry.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.315005 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz-private.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.c
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22831 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19036 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/test_ndlz.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.c
+-rw-r--r--   0 runner    (1001) docker     (123)   205061 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.319005 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26401 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.319005 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/include/bitstream.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.319005 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/macros.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/system.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34968 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.331005 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/bitstream.c
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/block1.h
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/block2.h
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/block3.h
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/block4.h
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1d.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1f.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1i.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1l.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2d.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2f.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2i.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2l.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3d.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3f.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3i.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3l.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4d.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4f.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4i.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4l.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1d.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1f.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1i.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1l.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2d.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2f.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2i.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2l.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3d.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3f.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3i.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3l.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4d.c
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4f.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4i.c
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4l.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.331005 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/
+-rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/bitstream.c
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/inline.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.331005 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/share/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/share/omp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/share/parallel.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.343006 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec.c
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec.h
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec1.c
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec3.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9466 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec4.c
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codecf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode3.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode4.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decodef.c
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decodei.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode3.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode4.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodef.c
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodei.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/ompcompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revcodecf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode.c
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode1.c
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode2.c
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode3.c
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode4.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecodef.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode.c
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode1.c
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode2.c
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode3.c
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode4.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencodef.c
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/template.h
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsd.h
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsi.h
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32747 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/zfp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_acc_float.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_prec_float.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10268 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_float.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_getitem.c
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/zfp-private.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.343006 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.343006 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/bytedelta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/bytedelta/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.c
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/bytedelta/test_bytedelta.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/filters-registry.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.347005 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndcell/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndcell/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndcell/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.c
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndcell/test_ndcell.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.347005 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndmean/
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndmean/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndmean/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.c
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_mean.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_repart.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/plugin_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/plugin_utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.347005 blosc2-2.2.2/blosc2/c-blosc2/plugins/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/test_data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/test_data/example_day_month_temp.b2nd
+-rw-r--r--   0 runner    (1001) docker     (123)   141455 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/test_data/example_item_prices.b2nd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.351006 blosc2-2.2.2/blosc2/c-blosc2/plugins/tunes/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/tunes/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/plugins/tunes/tunes-registry.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.367006 blosc2-2.2.2/blosc2/c-blosc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.375006 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/cutest.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_append.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_copy.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_delete.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_full.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_insert.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_metalayers.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_open_offset.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_persistency.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_resize.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_roundtrip.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_save.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_serialize.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_set_slice_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze_index.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_uninit.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_zeros.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/cutest.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.375006 blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.379006 blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/corpus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/corpus/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    33187 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-blosclz.b2frame
+-rw-r--r--   0 runner    (1001) docker     (123)    41393 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4.b2frame
+-rw-r--r--   0 runner    (1001) docker     (123)    24087 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4hc.b2frame
+-rw-r--r--   0 runner    (1001) docker     (123)    21570 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zlib.b2frame
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zstd.b2frame
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/fuzz_compress_chunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/fuzz_compress_frame.c
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_chunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_frame.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/generate_inputs_corpus.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/standalone.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/gcc-segfault-issue.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/print_versions.c
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_all.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_api.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_bitshuffle_leftovers.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_blosc1_compat.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_change_nthreads_append.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_compress_roundtrip.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_compress_roundtrip.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_compressor.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_contexts.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_copy.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_delete_chunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_delta.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_delta_schunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_dict_schunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_empty_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_fill_special.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_frame.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_frame_get_offsets.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_frame_offset.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_get_slice_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_getitem.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_getitem.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_getitem_delta.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_insert_chunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_lazychunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_lazychunk_memcpyed.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_maskout.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_maxout.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_noinit.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_nolock.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_nthreads.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_postfilter.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_prefilter.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_reorder_offsets.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_schunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_schunk_frame.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_schunk_header.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_set_slice_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_sframe.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_sframe_lazychunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_small_chunks.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_udio.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_update_chunk.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_urcodecs.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_urfilters.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-11 11:46:33.000000 blosc2-2.2.2/blosc2/c-blosc2/tests/test_zero_runlen.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45909 2023-05-11 11:46:32.000000 blosc2-2.2.2/blosc2/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-11 11:46:32.000000 blosc2-2.2.2/blosc2/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19583 2023-05-11 11:46:32.000000 blosc2-2.2.2/blosc2/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29890 2023-05-11 11:46:32.000000 blosc2-2.2.2/blosc2/schunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-11 11:48:50.000000 blosc2-2.2.2/blosc2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.091001 blosc2-2.2.2/blosc2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-05-11 11:48:51.000000 blosc2-2.2.2/blosc2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    52219 2023-05-11 11:48:51.000000 blosc2-2.2.2/blosc2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 11:48:51.000000 blosc2-2.2.2/blosc2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 11:48:51.000000 blosc2-2.2.2/blosc2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 11:48:51.000000 blosc2-2.2.2/blosc2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-11 11:46:32.000000 blosc2-2.2.2/code_of_conduct.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.379006 blosc2-2.2.2/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.379006 blosc2-2.2.2/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/_static/blosc-logo_128.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/_static/blosc-logo_256.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.379006 blosc2-2.2.2/doc/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/python-blosc2.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.383006 blosc2-2.2.2/doc/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.075001 blosc2-2.2.2/doc/reference/autofiles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.387006 blosc2-2.2.2/doc/reference/autofiles/schunk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.391006 blosc2-2.2.2/doc/reference/autofiles/schunk/attributes/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.blocksize.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.cbytes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.chunkshape.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.chunksize.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.contiguous.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.cparams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.cratio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.dparams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.nbytes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.typesize.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.urlpath.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/attributes/meta.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/attributes/vlmeta.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.__getitem__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.__setitem__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.append_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.decompress_chunk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.delete_chunk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.filler.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.get_chunk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.get_slice.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.insert_chunk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.insert_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.iterchunks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.postfilter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.prefilter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.remove_postfilter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.remove_prefilter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.to_cframe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.update_chunk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.update_data.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.395006 blosc2-2.2.2/doc/reference/autofiles/top_level/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/top_level/blosc2.Codec.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/top_level/blosc2.Filter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/top_level/blosc2.SplitMode.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/autofiles/top_level/blosc2.nthreads.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/ndarray_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/schunk_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/top_level.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/reference/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.395006 blosc2-2.2.2/doc/release_notes/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-11 11:46:32.000000 blosc2-2.2.2/doc/release_notes/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.399006 blosc2-2.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/compress2_decompress2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/compress_decompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/filler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/gil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.403006 blosc2-2.2.2/examples/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   335474 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/images/blosc2-pipeline.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46143 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/images/blosc2-pipeline.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.407006 blosc2-2.2.2/examples/images/ucodecs-filters/
+-rw-r--r--   0 runner    (1001) docker     (123)   107624 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/images/ucodecs-filters/backward.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38548 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/images/ucodecs-filters/backward.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    31483 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/images/ucodecs-filters/decoder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    35540 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/images/ucodecs-filters/decoder2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23248 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/images/ucodecs-filters/encoder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    24481 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/images/ucodecs-filters/encoder2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   110817 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/images/ucodecs-filters/forward.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41521 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/images/ucodecs-filters/forward.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.411007 blosc2-2.2.2/examples/ndarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/ndarray/asarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/ndarray/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/ndarray/bytedelta_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/ndarray/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/ndarray/empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/ndarray/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/ndarray/getitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/ndarray/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/ndarray/ndmean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/ndarray/persistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/ndarray/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/ndarray/work_with_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/ndarray/zfp_codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/pack_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/pack_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/postfilter1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/postfilter2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/postfilter3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/postfilters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/prefilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/prefilters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/save_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/schunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/schunk_roundtrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/slicing_and_beyond.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/tutorial-basics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/ucodecs-ufilters.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2114 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/ucodecs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/ufilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-11 11:46:32.000000 blosc2-2.2.2/examples/vlmeta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.415006 blosc2-2.2.2/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   116429 2023-05-11 11:46:32.000000 blosc2-2.2.2/images/Complete-Write-Read-B2ND.png
+-rw-r--r--   0 runner    (1001) docker     (123)    64898 2023-05-11 11:46:32.000000 blosc2-2.2.2/images/M1-i386-vs-arm64-pack.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62528 2023-05-11 11:46:32.000000 blosc2-2.2.2/images/M1-i386-vs-arm64-unpack.png
+-rw-r--r--   0 runner    (1001) docker     (123)   113029 2023-05-11 11:46:32.000000 blosc2-2.2.2/images/Read-Partial-Slices-B2ND.png
+-rw-r--r--   0 runner    (1001) docker     (123)   314966 2023-05-11 11:46:32.000000 blosc2-2.2.2/images/b2nd-2level-parts.png
+-rw-r--r--   0 runner    (1001) docker     (123)    77813 2023-05-11 11:46:32.000000 blosc2-2.2.2/images/linspace-compress.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24888 2023-05-11 11:46:32.000000 blosc2-2.2.2/images/linspace-decompress.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-05-11 11:46:32.000000 blosc2-2.2.2/images/pack-array-cratios.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-11 11:46:32.000000 blosc2-2.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-11 11:46:32.000000 blosc2-2.2.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 11:46:32.000000 blosc2-2.2.2/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-11 11:46:32.000000 blosc2-2.2.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 11:46:32.000000 blosc2-2.2.2/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 11:46:32.000000 blosc2-2.2.2/requirements-runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 11:46:32.000000 blosc2-2.2.2/requirements-test-wheels.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-11 11:46:32.000000 blosc2-2.2.2/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 11:48:51.427007 blosc2-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-11 11:46:32.000000 blosc2-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.423007 blosc2-2.2.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:48:51.427007 blosc2-2.2.2/tests/ndarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/ndarray/persistency.cat
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/ndarray/test_auto_parts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/ndarray/test_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/ndarray/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/ndarray/test_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/ndarray/test_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/ndarray/test_getitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/ndarray/test_lossy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/ndarray/test_metalayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/ndarray/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/ndarray/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/ndarray/test_persistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/ndarray/test_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/ndarray/test_setitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/ndarray/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/ndarray/test_squeeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/ndarray/test_struct_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/ndarray/test_zeros.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_bytes_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_comp_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_compress2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_compression_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_compressors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_decompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_iterchunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_postfilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_prefilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_python_blosc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_schunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_schunk_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_schunk_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_schunk_get_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_schunk_insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_schunk_set_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_schunk_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_ucodecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_ufilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-11 11:46:32.000000 blosc2-2.2.2/tests/test_vlmeta.py
```

### Comparing `blosc2-2.2.1/.github/workflows/build.yml` & `blosc2-2.2.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/.github/workflows/cibuildwheels.yml` & `blosc2-2.2.2/.github/workflows/cibuildwheels.yml`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,14 @@
           CIBW_BUILD: 'cp38-* cp39-* cp310-* cp311-*'
           CIBW_SKIP: '*-manylinux*_i686 *-musllinux_* ${{ env.CIBW_SKIP}}'
           CIBW_ARCHS_LINUX: ${{ matrix.arch }}
           CIBW_TEST_REQUIRES: pytest
           CIBW_TEST_COMMAND: python -m pytest -m "not heavy" {project}/tests
           CIBW_BUILD_VERBOSITY: 1
           CIBW_ARCHS_MACOS: "x86_64 arm64"
-          CIBW_MANYLINUX_X86_64_IMAGE: quay.io/pypa/manylinux2014_x86_64:2023-03-05-271004f
 
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           path: ./wheelhouse/*.whl
 
 
@@ -130,15 +129,15 @@
           python -m pip install --upgrade pip
           python -m pip install -r requirements-build.txt
           python -m pip install -r requirements-tests.txt
           python -m pip install -r requirements-runtime.txt
 
       - name: Build sdist
         run: |
-          python setup.py sdist
+          python -m build --sdist
 
       - name: Upload sdist package
         uses: actions/upload-artifact@v3
         with:
           path: dist/*.tar.gz
 
       - name: Build building extension from sdist package
```

### Comparing `blosc2-2.2.1/.gitignore` & `blosc2-2.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/ANNOUNCE.rst` & `blosc2-2.2.2/ANNOUNCE.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-Announcing Python-Blosc2 2.2.1
+Announcing Python-Blosc2 2.2.2
 ==============================
 
-We have updated to latest C-Blosc2 2.9.1.
+Wheels are not including blosc2.pc (pkgconfig) anymore.  For details see:
+https://github.com/Blosc/python-blosc2/pull/111
+Thanks to @bnavigator for the PR.
 
 For more info, you can have a look at the release notes in:
 
 https://github.com/Blosc/python-blosc2/releases
 
 More docs and examples are available in the documentation site:
```

### Comparing `blosc2-2.2.1/CMakeLists.txt` & `blosc2-2.2.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/LICENSE.txt` & `blosc2-2.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/PKG-INFO` & `blosc2-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: blosc2
-Version: 2.2.1
-Summary: Python wrapper for the C-Blosc2 library.
-Home-page: https://github.com/Blosc/python-blosc2
-Author: Blosc Development Team
-Author-email: blosc@blosc.org
-Maintainer: Blosc Development Team
-Maintainer-email: blosc@blosc.org
-License: https://opensource.org/licenses/BSD-3-Clause
-Platform: any
+Version: 2.2.2
+Summary: Python wrapper for the C-Blosc2 library
+Author-email: Blosc Development Team <blosc@blosc.org>
+Maintainer-email: Blosc Development Team <blosc@blosc.org>
+License: BSD-3-Clause
+Project-URL: homepage, https://github.com/Blosc/python-blosc2
+Project-URL: documentation, https://www.blosc.org/python-blosc2/python-blosc2.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8, <4
+Requires-Python: <4,>=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 =============
 Python-Blosc2
 =============
 
@@ -232,9 +230,7 @@
 =======
 
 Please follow `@Blosc2 <https://twitter.com/Blosc2>`_ to get informed about the latest developments.
 
 ----
 
   **Enjoy data!**
-
-
```

### Comparing `blosc2-2.2.1/README.rst` & `blosc2-2.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/RELEASE_NOTES.md` & `blosc2-2.2.2/RELEASE_NOTES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Release notes
 
+## Changes from 2.2.1 to 2.2.2
+
+* Wheels are not including blosc2.pc (pkgconfig) anymore.  For details see:
+  https://github.com/Blosc/python-blosc2/pull/111
+  Thanks to @bnavigator for the PR.
+
+
 ## Changes from 2.2.0 to 2.2.1
 
 * Updated to latest C-Blosc2 2.9.1.
 
 
 ## Changes from 2.1.1 to 2.2.0
```

### Comparing `blosc2-2.2.1/RELEASING.rst` & `blosc2-2.2.2/RELEASING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 * Double check that the supported Python versions for the wheels are the correct ones
   (`.github/workflows/cibuildwheels.yml`).  Add/remove Python version if needed.
   Also, update the `classifiers` field for the supported Python versions.
 
 * Check that the metainfo for the package is correct::
 
-    python setup.py sdist
+    python -m build --sdist 
     twine check dist/*
 
 
 Tagging
 -------
 
 * Create a (signed, if possible) tag ``X.Y.Z`` from ``main``.  Use the next message::
```

### Comparing `blosc2-2.2.1/bench/compress_numpy.py` & `blosc2-2.2.2/bench/compress_numpy.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/bench/get_slice.py` & `blosc2-2.2.2/bench/get_slice.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/bench/ndarray/compare_getslice.py` & `blosc2-2.2.2/bench/ndarray/compare_getslice.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/bench/ndarray/copy_postfilter.py` & `blosc2-2.2.2/bench/ndarray/copy_postfilter.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/bench/ndarray/download_data.py` & `blosc2-2.2.2/bench/ndarray/download_data.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/bench/ndarray/era5-pds/measurements-i10k.parquet` & `blosc2-2.2.2/bench/ndarray/era5-pds/measurements-i10k.parquet`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/bench/ndarray/era5-pds/measurements-i13k-always-split.parquet` & `blosc2-2.2.2/bench/ndarray/era5-pds/measurements-i13k-always-split.parquet`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/bench/ndarray/era5-pds/measurements-i13k-never-split.parquet` & `blosc2-2.2.2/bench/ndarray/era5-pds/measurements-i13k-never-split.parquet`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/bench/ndarray/era5-pds/measurements-i13k.parquet` & `blosc2-2.2.2/bench/ndarray/era5-pds/measurements-i13k.parquet`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/bench/ndarray/era5-pds/measurements-m1.parquet` & `blosc2-2.2.2/bench/ndarray/era5-pds/measurements-m1.parquet`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/bench/ndarray/era5-pds/measurements-ryzen3.parquet` & `blosc2-2.2.2/bench/ndarray/era5-pds/measurements-ryzen3.parquet`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/bench/ndarray/plot_transcode_data.ipynb` & `blosc2-2.2.2/bench/ndarray/plot_transcode_data.ipynb`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/bench/ndarray/transcode_data.py` & `blosc2-2.2.2/bench/ndarray/transcode_data.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/bench/pack_compress.py` & `blosc2-2.2.2/bench/pack_compress.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/bench/pack_large.py` & `blosc2-2.2.2/bench/pack_large.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/bench/pack_tensor.py` & `blosc2-2.2.2/bench/pack_tensor.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/bench/set_slice.py` & `blosc2-2.2.2/bench/set_slice.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/bench/sum_postfilter.py` & `blosc2-2.2.2/bench/sum_postfilter.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/CMakeLists.txt` & `blosc2-2.2.2/blosc2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/__init__.py` & `blosc2-2.2.2/blosc2/__init__.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/blosc2_ext.pyx` & `blosc2-2.2.2/blosc2/blosc2_ext.pyx`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/.github/ISSUE_TEMPLATE/bug_report.md` & `blosc2-2.2.2/blosc2/c-blosc2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/.github/workflows/cmake.yml` & `blosc2-2.2.2/blosc2/c-blosc2/.github/workflows/cmake.yml`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/.github/workflows/fuzz.yml` & `blosc2-2.2.2/blosc2/c-blosc2/.github/workflows/fuzz.yml`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/.readthedocs.yaml` & `blosc2-2.2.2/blosc2/c-blosc2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/ANNOUNCE.md` & `blosc2-2.2.2/blosc2/c-blosc2/ANNOUNCE.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/CMakeLists.txt` & `blosc2-2.2.2/blosc2/c-blosc2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/COMPILING_WITH_WHEELS.rst` & `blosc2-2.2.2/blosc2/c-blosc2/COMPILING_WITH_WHEELS.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/CONTRIBUTING.rst` & `blosc2-2.2.2/blosc2/c-blosc2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/DEVELOPING-GUIDE.rst` & `blosc2-2.2.2/blosc2/c-blosc2/DEVELOPING-GUIDE.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/FAQ.md` & `blosc2-2.2.2/blosc2/c-blosc2/FAQ.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/LICENSE.txt` & `blosc2-2.2.2/blosc2/c-blosc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/LICENSES/BITSHUFFLE.txt` & `blosc2-2.2.2/blosc2/c-blosc2/LICENSES/BITSHUFFLE.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/LICENSES/FASTLZ.txt` & `blosc2-2.2.2/blosc2/c-blosc2/LICENSES/FASTLZ.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/LICENSES/LZ4.txt` & `blosc2-2.2.2/blosc2/c-blosc2/LICENSES/LZ4.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/LICENSES/SNAPPY.txt` & `blosc2-2.2.2/blosc2/c-blosc2/LICENSES/SNAPPY.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/LICENSES/STDINT.txt` & `blosc2-2.2.2/blosc2/c-blosc2/LICENSES/STDINT.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/LICENSES/ZLIB.txt` & `blosc2-2.2.2/blosc2/c-blosc2/LICENSES/ZLIB.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/README.rst` & `blosc2-2.2.2/blosc2/c-blosc2/README.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/README_ARM.rst` & `blosc2-2.2.2/blosc2/c-blosc2/README_ARM.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/README_B2ND_METALAYER.rst` & `blosc2-2.2.2/blosc2/c-blosc2/README_B2ND_METALAYER.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/README_CFRAME_FORMAT.rst` & `blosc2-2.2.2/blosc2/c-blosc2/README_CFRAME_FORMAT.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/README_CHUNK_FORMAT.rst` & `blosc2-2.2.2/blosc2/c-blosc2/README_CHUNK_FORMAT.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/README_FUZZER.md` & `blosc2-2.2.2/blosc2/c-blosc2/README_FUZZER.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/README_SFRAME_FORMAT.rst` & `blosc2-2.2.2/blosc2/c-blosc2/README_SFRAME_FORMAT.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/README_THREADED.rst` & `blosc2-2.2.2/blosc2/c-blosc2/README_THREADED.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/RELEASE_NOTES.md` & `blosc2-2.2.2/blosc2/c-blosc2/RELEASE_NOTES.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/RELEASING.rst` & `blosc2-2.2.2/blosc2/c-blosc2/RELEASING.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/ROADMAP.rst` & `blosc2-2.2.2/blosc2/c-blosc2/ROADMAP.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/THANKS.rst` & `blosc2-2.2.2/blosc2/c-blosc2/THANKS.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/CMakeLists.txt` & `blosc2-2.2.2/blosc2/c-blosc2/bench/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/Makefile` & `blosc2-2.2.2/blosc2/c-blosc2/bench/Makefile`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/Makefile.mingw` & `blosc2-2.2.2/blosc2/c-blosc2/bench/Makefile.mingw`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/b2bench.c` & `blosc2-2.2.2/blosc2/c-blosc2/bench/b2bench.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/b2nd/CMakeLists.txt` & `blosc2-2.2.2/blosc2/c-blosc2/bench/b2nd/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/b2nd/bench_get_slice.c` & `blosc2-2.2.2/blosc2/c-blosc2/bench/b2nd/bench_get_slice.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/b2nd/bench_zfp_getitem.c` & `blosc2-2.2.2/blosc2/c-blosc2/bench/b2nd/bench_zfp_getitem.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/create_frame.c` & `blosc2-2.2.2/blosc2/c-blosc2/bench/create_frame.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/delta_schunk.c` & `blosc2-2.2.2/blosc2/c-blosc2/bench/delta_schunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/plot-speeds.py` & `blosc2-2.2.2/blosc2/c-blosc2/bench/plot-speeds.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/plot-sum_openmp-results.py` & `blosc2-2.2.2/blosc2/c-blosc2/bench/plot-sum_openmp-results.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/rainfall-grid-150x150.bin` & `blosc2-2.2.2/blosc2/c-blosc2/bench/rainfall-grid-150x150.bin`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/read-grid-150x150.py` & `blosc2-2.2.2/blosc2/c-blosc2/bench/read-grid-150x150.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/results-corex/blosclz-cl1-sum_openmp-corex.out` & `blosc2-2.2.2/blosc2/c-blosc2/bench/results-corex/blosclz-cl1-sum_openmp-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/results-corex/blosclz-suite-corex.out` & `blosc2-2.2.2/blosc2/c-blosc2/bench/results-corex/blosclz-suite-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/results-corex/lz4-cl1-sum_openmp-corex.out` & `blosc2-2.2.2/blosc2/c-blosc2/bench/results-corex/lz4-cl1-sum_openmp-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/results-corex/lz4-suite-corex.out` & `blosc2-2.2.2/blosc2/c-blosc2/bench/results-corex/lz4-suite-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/results-corex/lz4hc-cl1-sum_openmp-corex.out` & `blosc2-2.2.2/blosc2/c-blosc2/bench/results-corex/lz4hc-cl1-sum_openmp-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/results-corex/zlib-cl1-sum_openmp-corex.out` & `blosc2-2.2.2/blosc2/c-blosc2/bench/results-corex/zlib-cl1-sum_openmp-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/results-corex/zstd-cl1-sum_openmp-corex.out` & `blosc2-2.2.2/blosc2/c-blosc2/bench/results-corex/zstd-cl1-sum_openmp-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/sframe_bench.c` & `blosc2-2.2.2/blosc2/c-blosc2/bench/sframe_bench.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/sum_openmp.c` & `blosc2-2.2.2/blosc2/c-blosc2/bench/sum_openmp.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/trunc_prec_schunk.c` & `blosc2-2.2.2/blosc2/c-blosc2/bench/trunc_prec_schunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/bench/zero_runlen.c` & `blosc2-2.2.2/blosc2/c-blosc2/bench/zero_runlen.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/CMakeLists.txt` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/b2nd.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/b2nd.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/b2nd_utils.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/b2nd_utils.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/b2nd_utils.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/b2nd_utils.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/bitshuffle-altivec.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/bitshuffle-altivec.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/bitshuffle-altivec.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/bitshuffle-altivec.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/bitshuffle-avx2.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/bitshuffle-avx2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/bitshuffle-avx2.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/bitshuffle-avx2.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/bitshuffle-generic.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/bitshuffle-generic.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/bitshuffle-generic.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/bitshuffle-generic.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/bitshuffle-neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/bitshuffle-neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/bitshuffle-neon.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/bitshuffle-neon.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/bitshuffle-sse2.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/bitshuffle-sse2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/bitshuffle-sse2.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/bitshuffle-sse2.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/blosc-private.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/blosc-private.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/blosc2-stdio.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/blosc2-stdio.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/blosc2.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/blosc2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/blosclz.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/blosclz.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/blosclz.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/blosclz.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/context.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/context.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/delta.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/delta.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/delta.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/delta.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/directories.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/directories.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/fastcopy.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/fastcopy.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/fastcopy.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/fastcopy.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/frame.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/frame.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/frame.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/frame.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/schunk.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/schunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/sframe.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/sframe.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/sframe.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/sframe.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle-altivec.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle-altivec.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle-altivec.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle-altivec.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle-avx2.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle-avx2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle-avx2.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle-avx2.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle-generic.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle-generic.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle-generic.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle-generic.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle-neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle-neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle-neon.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle-neon.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle-sse2.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle-sse2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle-sse2.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle-sse2.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/shuffle.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/shuffle.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/stune.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/stune.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/stune.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/stune.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/timestamp.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/timestamp.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/transpose-altivec.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/transpose-altivec.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/trunc-prec.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/trunc-prec.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/trunc-prec.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/trunc-prec.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/win32/pthread.c` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/win32/pthread.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/win32/pthread.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/win32/pthread.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/blosc/win32/stdint-windows.h` & `blosc2-2.2.2/blosc2/c-blosc2/blosc/win32/stdint-windows.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/cmake/FindIPP.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/cmake/FindIPP.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/cmake/FindSIMD.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/cmake/FindSIMD.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/cmake/FindZLIB_NG.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/cmake/FindZLIB_NG.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/cmake/toolchain-aarch64.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/cmake/toolchain-aarch64.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/cmake/toolchain-armhf.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/cmake/toolchain-armhf.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/cmake/toolchain-armsf.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/cmake/toolchain-armsf.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/cmake_uninstall.cmake.in` & `blosc2-2.2.2/blosc2/c-blosc2/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/CMakeLists.txt` & `blosc2-2.2.2/blosc2/c-blosc2/compat/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.11.1-blosclz.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.11.1-blosclz.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.11.1-lz4.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.11.1-lz4.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.11.1-lz4hc.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.11.1-lz4hc.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.11.1-zlib.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.11.1-zlib.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.11.1-zstd.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.11.1-zstd.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.14.0-blosclz.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.14.0-blosclz.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.14.0-lz4.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.14.0-lz4.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.14.0-lz4hc.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.14.0-lz4hc.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.14.0-zlib.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.14.0-zlib.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.14.0-zstd.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.14.0-zstd.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle4-memcpy.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle4-memcpy.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle8-nomemcpy.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle8-nomemcpy.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle4-memcpy.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle4-memcpy.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle8-nomemcpy.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle8-nomemcpy.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.3.0-blosclz.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.3.0-blosclz.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.3.0-lz4.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.3.0-lz4.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.3.0-lz4hc.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.3.0-lz4hc.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.3.0-zlib.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.3.0-zlib.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.7.0-blosclz.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.7.0-blosclz.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.7.0-lz4.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.7.0-lz4.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.7.0-lz4hc.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.7.0-lz4hc.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-1.7.0-zlib.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-1.7.0-zlib.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle4-memcpy.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle4-memcpy.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle8-nomemcpy.cdata` & `blosc2-2.2.2/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle8-nomemcpy.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/compat/filegen.c` & `blosc2-2.2.2/blosc2/c-blosc2/compat/filegen.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test1.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test1.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test16.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test16.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test2.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test4.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test8.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test8.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test16.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test16.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test2.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test4.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test8.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test8.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle4_neon/unshuffle4_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle4_neon/unshuffle4_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx_bucle.c` & `blosc2-2.2.2/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/doc/_static/blosc-logo_256.png` & `blosc2-2.2.2/blosc2/c-blosc2/doc/_static/blosc-logo_256.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/doc/_static/css/custom.css` & `blosc2-2.2.2/blosc2/c-blosc2/doc/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/doc/conf.py` & `blosc2-2.2.2/blosc2/c-blosc2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/doc/reference/b2nd.rst` & `blosc2-2.2.2/blosc2/c-blosc2/doc/reference/b2nd.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/doc/reference/blosc1.rst` & `blosc2-2.2.2/blosc2/c-blosc2/doc/reference/blosc1.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/doc/reference/context.rst` & `blosc2-2.2.2/blosc2/c-blosc2/doc/reference/context.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/doc/reference/index.rst` & `blosc2-2.2.2/blosc2/c-blosc2/doc/reference/index.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/doc/reference/metalayers.rst` & `blosc2-2.2.2/blosc2/c-blosc2/doc/reference/metalayers.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/doc/reference/plugins.rst` & `blosc2-2.2.2/blosc2/c-blosc2/doc/reference/plugins.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/doc/reference/schunk.rst` & `blosc2-2.2.2/blosc2/c-blosc2/doc/reference/schunk.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/doc/reference/utility.rst` & `blosc2-2.2.2/blosc2/c-blosc2/doc/reference/utility.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/CMakeLists.txt` & `blosc2-2.2.2/blosc2/c-blosc2/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/README.rst` & `blosc2-2.2.2/blosc2/c-blosc2/examples/README.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/b2nd/CMakeLists.txt` & `blosc2-2.2.2/blosc2/c-blosc2/examples/b2nd/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/b2nd/example_empty_shape.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/b2nd/example_empty_shape.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/b2nd/example_frame_generator.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/b2nd/example_frame_generator.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/b2nd/example_oindex.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/b2nd/example_oindex.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/b2nd/example_plainbuffer.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/b2nd/example_plainbuffer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/b2nd/example_plugins_codecs.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/b2nd/example_plugins_codecs.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/b2nd/example_plugins_filters.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/b2nd/example_plugins_filters.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/b2nd/example_print_meta.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/b2nd/example_print_meta.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/b2nd/example_serialize.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/b2nd/example_serialize.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/compress_file.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/compress_file.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/contexts.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/contexts.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/delta_schunk_ex.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/delta_schunk_ex.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/find_roots.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/find_roots.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/frame_backed_schunk.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/frame_backed_schunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/frame_big.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/frame_big.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/frame_metalayers.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/frame_metalayers.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/frame_offset.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/frame_offset.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/frame_roundtrip.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/frame_roundtrip.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/frame_simple.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/frame_simple.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/frame_vlmetalayers.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/frame_vlmetalayers.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/get_set_slice.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/get_set_slice.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/instrument_codec.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/instrument_codec.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/many_compressors.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/many_compressors.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/multithread.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/multithread.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/noinit.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/noinit.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/schunk_postfilter.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/schunk_postfilter.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/schunk_simple.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/schunk_simple.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/sframe_simple.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/sframe_simple.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/simple.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/simple.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/urcodecs.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/urcodecs.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/urfilters.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/urfilters.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/win-dynamic-linking.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/win-dynamic-linking.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/examples/zstd_dict.c` & `blosc2-2.2.2/blosc2/c-blosc2/examples/zstd_dict.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/images/Complete-Write-Read-B2ND.png` & `blosc2-2.2.2/blosc2/c-blosc2/images/Complete-Write-Read-B2ND.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/images/Read-Partial-Slices-B2ND.png` & `blosc2-2.2.2/blosc2/c-blosc2/images/Read-Partial-Slices-B2ND.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/images/b2nd-2level-parts.png` & `blosc2-2.2.2/blosc2/c-blosc2/images/b2nd-2level-parts.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/include/b2nd.h` & `blosc2-2.2.2/blosc2/c-blosc2/include/b2nd.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/include/blosc2/blosc2-common.h` & `blosc2-2.2.2/blosc2/c-blosc2/include/blosc2/blosc2-common.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/include/blosc2/blosc2-export.h` & `blosc2-2.2.2/blosc2/c-blosc2/include/blosc2/blosc2-export.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/include/blosc2/blosc2-stdio.h` & `blosc2-2.2.2/blosc2/c-blosc2/include/blosc2/blosc2-stdio.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/include/blosc2/codecs-registry.h` & `blosc2-2.2.2/blosc2/c-blosc2/include/blosc2/codecs-registry.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/include/blosc2/filters-registry.h` & `blosc2-2.2.2/blosc2/c-blosc2/include/blosc2/filters-registry.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/include/blosc2/plugins-utils.h` & `blosc2-2.2.2/blosc2/c-blosc2/include/blosc2/plugins-utils.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/include/blosc2/tunes-registry.h` & `blosc2-2.2.2/blosc2/c-blosc2/include/blosc2/tunes-registry.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/include/blosc2.h` & `blosc2-2.2.2/blosc2/c-blosc2/include/blosc2.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/.shellcheckrc` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/.shellcheckrc`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/CMakeLists.txt` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/FAQ.zlib` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/FAQ.zlib`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/INDEX.md` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/INDEX.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/LICENSE.md` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/Makefile.in` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/Makefile.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/PORTING.md` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/PORTING.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/README.md` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32_p.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32_p.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/Makefile.in` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/Makefile.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/adler32_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/adler32_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/armfeature.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/armfeature.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/chunkset_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/chunkset_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/crc32_acle.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/crc32_acle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/insert_string_acle.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/insert_string_acle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/slide_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/slide_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/Makefile.in` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/Makefile.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/adler32_power8.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/adler32_power8.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/slide_hash_power8.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/slide_hash_power8.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/Makefile.in` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/Makefile.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/README.md` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_detail.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_detail.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.Dockerfile` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.Dockerfile`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.service` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.service`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/actions-runner` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/actions-runner`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/entrypoint` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/Makefile.in` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/Makefile.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_avx.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_avx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_ssse3.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_ssse3.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_avx.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_avx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_sse.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_sse.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_avx.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_avx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_sse.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_sse.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/insert_string_sse.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/insert_string_sse.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_avx.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_avx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_sse.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_sse.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/x86.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/x86.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset_tpl.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset_tpl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-coverage.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-coverage.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-install-dirs.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-install-dirs.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-sanitizer.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-sanitizer.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-compare.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-compare.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-redirect.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-redirect.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-compress.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-compress.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-tools.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-tools.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-aarch64.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-aarch64.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-arm.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-arm.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-armhf.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-armhf.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-i686.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-i686.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-x86_64.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-x86_64.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64le.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64le.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-s390x.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-s390x.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-sparc64.cmake` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-sparc64.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compare258.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compare258.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compress.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/configure` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/configure`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl._h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl._h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl._h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl._h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_fast.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_fast.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_medium.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_medium.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_p.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_p.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_quick.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_quick.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_slow.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_slow.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/algorithm.txt` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/algorithm.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1950.txt` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1950.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1951.txt` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1951.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1952.txt` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1952.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/txtvsbin.txt` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/txtvsbin.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/fallback_builtins.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/fallback_builtins.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzguts.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzguts.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzlib.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzlib.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzread.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzread.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzwrite.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzwrite.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/infback.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/infback.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl._h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl._h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate_p.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate_p.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string_tpl.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string_tpl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/match_tpl.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/match_tpl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2002-0059/test.gz` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2002-0059/test.gz`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/default.txt` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/default.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/fixed.txt` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/fixed.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-979/pigz-2.6.tar.gz` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-979/pigz-2.6.tar.gz`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/Makefile.in` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/Makefile.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/README.md` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-arm-linux-gnueabihf.abi` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-arm-linux-gnueabihf.abi`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-x86_64-linux-gnu.abi` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-x86_64-linux-gnu.abi`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.md` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.sh` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.sh`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/adler32_test.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/adler32_test.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/crc32_test.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/crc32_test.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/fireworks.jpg` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/fireworks.jpg`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/lcet10.txt` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/lcet10.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/paper-100k.pdf` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/paper-100k.pdf`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_bi_valid.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_bi_valid.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_block_open.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_block_open.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/example.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/example.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/checksum_fuzzer.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/checksum_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/compress_fuzzer.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/compress_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_dict_fuzzer.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_dict_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_flush_fuzzer.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_flush_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_large_fuzzer.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_large_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_small_fuzzer.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_small_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/minigzip_fuzzer.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/minigzip_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/standalone_fuzz_target_runner.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/standalone_fuzz_target_runner.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/gh1235.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/gh1235.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/hash_head_0.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/hash_head_0.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/infcover.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/infcover.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/inflate_adler32.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/inflate_adler32.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minideflate.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minideflate.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minigzip.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minigzip.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pigz/CMakeLists.txt` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pigz/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pkgcheck.sh` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pkgcheck.sh`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/switchlevels.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/switchlevels.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/testCVEinputs.sh` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/testCVEinputs.sh`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/config.sub` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/config.sub`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makecrct.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makecrct.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makefixed.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makefixed.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/maketrees.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/maketrees.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_emit.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_emit.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl._h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl._h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/uncompr.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/uncompr.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/DLL_FAQ.txt` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/DLL_FAQ.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.a64` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.a64`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.arm` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.arm`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.msc` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.msc`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/README-WIN32.txt` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/README-WIN32.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng.def` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng.def`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng1.rc` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng1.rc`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib.def` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib.def`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib1.rc` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib1.rc`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlibcompat.def` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlibcompat.def`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zbuild.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zbuild.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf-ng.h.in` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf-ng.h.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.in` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.included` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.included`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zendian.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zendian.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.map` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.map`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.map` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.map`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil_p.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil_p.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/BUCK` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/BUCK`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/Makefile` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/Makefile`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/README.md` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/allocations.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/allocations.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bits.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bits.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bitstream.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bitstream.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/compiler.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/compiler.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/cpu.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/cpu.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/entropy_common.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/entropy_common.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse_decompress.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/huf.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/huf.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/mem.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/mem.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/portability_macros.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/portability_macros.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_common.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_common.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_deps.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_deps.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_internal.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_internal.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_trace.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_trace.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/clevels.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/clevels.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/fse_compress.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/fse_compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/huf_compress.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/huf_compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_internal.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_internal.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_cwksp.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_cwksp.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm_geartab.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm_geartab.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress_amd64.S` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress_amd64.S`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_internal.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_internal.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_common.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_common.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_compress.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_decompress.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_decompress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/fastcover.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/fastcover.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/zdict.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/zdict.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/Makefile` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/Makefile`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/README.md` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.sln` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.sln`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.vcxproj` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_legacy.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_legacy.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.c` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/libzstd.mk` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/libzstd.mk`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/module.modulemap` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/module.modulemap`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zdict.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zdict.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd_errors.h` & `blosc2-2.2.2/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd_errors.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/README.md` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/codecs-registry.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/codecs-registry.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/CMakeLists.txt` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/README.md` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz-private.h` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz-private.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.h` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.h` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.h` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/test_ndlz.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/test_ndlz.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.h` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/CMakeLists.txt` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/README.md` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.h` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/include/bitstream.h` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/include/bitstream.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/system.h` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/system.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/types.h` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/types.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/version.h` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/version.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp.h` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/bitstream.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/bitstream.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/share/omp.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/share/omp.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/share/parallel.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/share/parallel.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec2.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec3.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec3.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec4.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codecf.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codecf.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/compress.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode1.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode1.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode2.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode3.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode3.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode4.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decodef.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decodef.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decompress.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decompress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode1.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode1.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode2.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode3.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode3.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode4.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodef.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodef.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodei.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodei.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/ompcompress.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/ompcompress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode3.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode3.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode4.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecodef.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecodef.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode3.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode3.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode4.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencodef.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencodef.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsd.h` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsd.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsf.h` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsf.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/src/zfp.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/src/zfp.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_acc_float.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_acc_float.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_prec_float.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_prec_float.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_float.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_float.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_getitem.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_getitem.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/codecs/zfp/zfp-private.h` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/codecs/zfp/zfp-private.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/bytedelta/CMakeLists.txt` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/bytedelta/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.h` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/bytedelta/test_bytedelta.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/bytedelta/test_bytedelta.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/filters-registry.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/filters-registry.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndcell/CMakeLists.txt` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndcell/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndcell/README.md` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndcell/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.h` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndcell/test_ndcell.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndcell/test_ndcell.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndmean/CMakeLists.txt` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndmean/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndmean/README.md` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndmean/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.h` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_mean.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_mean.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_repart.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_repart.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/plugin_utils.c` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/plugin_utils.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/test_data/README.md` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/test_data/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/test_data/example_day_month_temp.b2nd` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/test_data/example_day_month_temp.b2nd`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/plugins/test_data/example_item_prices.b2nd` & `blosc2-2.2.2/blosc2/c-blosc2/plugins/test_data/example_item_prices.b2nd`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/CMakeLists.txt` & `blosc2-2.2.2/blosc2/c-blosc2/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/Makefile` & `blosc2-2.2.2/blosc2/c-blosc2/tests/Makefile`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/CMakeLists.txt` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/cutest.h` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/cutest.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_append.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_append.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_copy.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_copy.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_delete.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_delete.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_full.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_full.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice_buffer.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice_buffer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_insert.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_insert.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_metalayers.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_metalayers.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_open_offset.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_open_offset.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_persistency.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_persistency.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_resize.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_resize.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_roundtrip.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_roundtrip.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_save.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_save.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_serialize.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_serialize.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_set_slice_buffer.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_set_slice_buffer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze_index.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze_index.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_uninit.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_uninit.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_zeros.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_b2nd_zeros.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/b2nd/test_common.h` & `blosc2-2.2.2/blosc2/c-blosc2/tests/b2nd/test_common.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/cutest.h` & `blosc2-2.2.2/blosc2/c-blosc2/tests/cutest.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/CMakeLists.txt` & `blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/README.md` & `blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/corpus/README.md` & `blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/corpus/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-blosclz.b2frame` & `blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-blosclz.b2frame`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4.b2frame` & `blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4.b2frame`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4hc.b2frame` & `blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4hc.b2frame`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zlib.b2frame` & `blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zlib.b2frame`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zstd.b2frame` & `blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zstd.b2frame`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/fuzz_compress_chunk.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/fuzz_compress_chunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/fuzz_compress_frame.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/fuzz_compress_frame.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_chunk.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_chunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_frame.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_frame.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/generate_inputs_corpus.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/generate_inputs_corpus.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/fuzz/standalone.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/fuzz/standalone.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/gcc-segfault-issue.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/gcc-segfault-issue.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/print_versions.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/print_versions.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_api.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_api.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_bitshuffle_leftovers.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_bitshuffle_leftovers.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_blosc1_compat.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_blosc1_compat.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_change_nthreads_append.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_change_nthreads_append.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_common.h` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_common.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_compress_roundtrip.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_compress_roundtrip.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_compress_roundtrip.csv` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_compress_roundtrip.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_compressor.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_compressor.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_contexts.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_contexts.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_copy.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_copy.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_delete_chunk.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_delete_chunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_delta.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_delta.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_delta_schunk.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_delta_schunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_dict_schunk.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_dict_schunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_empty_buffer.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_empty_buffer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_fill_special.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_fill_special.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_frame.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_frame.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_frame_get_offsets.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_frame_get_offsets.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_frame_offset.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_frame_offset.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_get_slice_buffer.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_get_slice_buffer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_getitem.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_getitem.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_getitem.csv` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_getitem.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_getitem_delta.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_getitem_delta.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_insert_chunk.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_insert_chunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_lazychunk.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_lazychunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_lazychunk_memcpyed.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_lazychunk_memcpyed.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_maskout.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_maskout.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_maxout.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_maxout.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_noinit.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_noinit.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_nolock.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_nolock.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_nthreads.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_nthreads.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_postfilter.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_postfilter.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_prefilter.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_prefilter.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_reorder_offsets.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_reorder_offsets.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_schunk.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_schunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_schunk_frame.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_schunk_frame.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_schunk_header.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_schunk_header.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_set_slice_buffer.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_set_slice_buffer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_sframe.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_sframe.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_sframe_lazychunk.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_sframe_lazychunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.csv` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.csv` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.csv` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.csv` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.csv` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_small_chunks.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_small_chunks.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_udio.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_udio.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_update_chunk.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_update_chunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_urcodecs.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_urcodecs.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_urfilters.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_urfilters.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/c-blosc2/tests/test_zero_runlen.c` & `blosc2-2.2.2/blosc2/c-blosc2/tests/test_zero_runlen.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/core.py` & `blosc2-2.2.2/blosc2/core.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/info.py` & `blosc2-2.2.2/blosc2/info.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/ndarray.py` & `blosc2-2.2.2/blosc2/ndarray.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2/schunk.py` & `blosc2-2.2.2/blosc2/schunk.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/blosc2.egg-info/PKG-INFO` & `blosc2-2.2.2/blosc2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: blosc2
-Version: 2.2.1
-Summary: Python wrapper for the C-Blosc2 library.
-Home-page: https://github.com/Blosc/python-blosc2
-Author: Blosc Development Team
-Author-email: blosc@blosc.org
-Maintainer: Blosc Development Team
-Maintainer-email: blosc@blosc.org
-License: https://opensource.org/licenses/BSD-3-Clause
-Platform: any
+Version: 2.2.2
+Summary: Python wrapper for the C-Blosc2 library
+Author-email: Blosc Development Team <blosc@blosc.org>
+Maintainer-email: Blosc Development Team <blosc@blosc.org>
+License: BSD-3-Clause
+Project-URL: homepage, https://github.com/Blosc/python-blosc2
+Project-URL: documentation, https://www.blosc.org/python-blosc2/python-blosc2.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8, <4
+Requires-Python: <4,>=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 =============
 Python-Blosc2
 =============
 
@@ -232,9 +230,7 @@
 =======
 
 Please follow `@Blosc2 <https://twitter.com/Blosc2>`_ to get informed about the latest developments.
 
 ----
 
   **Enjoy data!**
-
-
```

### Comparing `blosc2-2.2.1/blosc2.egg-info/SOURCES.txt` & `blosc2-2.2.2/blosc2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/doc/_static/blosc-logo_128.png` & `blosc2-2.2.2/doc/_static/blosc-logo_128.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/doc/_static/blosc-logo_256.png` & `blosc2-2.2.2/doc/_static/blosc-logo_256.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/doc/_static/css/custom.css` & `blosc2-2.2.2/doc/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/doc/conf.py` & `blosc2-2.2.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/doc/reference/autofiles/schunk/attributes/meta.rst` & `blosc2-2.2.2/doc/reference/autofiles/schunk/attributes/meta.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/doc/reference/autofiles/schunk/attributes/vlmeta.rst` & `blosc2-2.2.2/doc/reference/autofiles/schunk/attributes/vlmeta.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/doc/reference/ndarray_api.rst` & `blosc2-2.2.2/doc/reference/ndarray_api.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/doc/reference/schunk_api.rst` & `blosc2-2.2.2/doc/reference/schunk_api.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/doc/reference/top_level.rst` & `blosc2-2.2.2/doc/reference/top_level.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/compress2_decompress2.py` & `blosc2-2.2.2/examples/compress2_decompress2.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/compress_decompress.py` & `blosc2-2.2.2/examples/compress_decompress.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/filler.py` & `blosc2-2.2.2/examples/filler.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/images/blosc2-pipeline.png` & `blosc2-2.2.2/examples/images/blosc2-pipeline.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/images/blosc2-pipeline.svg` & `blosc2-2.2.2/examples/images/blosc2-pipeline.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/images/ucodecs-filters/backward.png` & `blosc2-2.2.2/examples/images/ucodecs-filters/backward.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/images/ucodecs-filters/backward.svg` & `blosc2-2.2.2/examples/images/ucodecs-filters/backward.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/images/ucodecs-filters/decoder.svg` & `blosc2-2.2.2/examples/images/ucodecs-filters/decoder.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/images/ucodecs-filters/decoder2.svg` & `blosc2-2.2.2/examples/images/ucodecs-filters/decoder2.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/images/ucodecs-filters/encoder.svg` & `blosc2-2.2.2/examples/images/ucodecs-filters/encoder.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/images/ucodecs-filters/encoder2.svg` & `blosc2-2.2.2/examples/images/ucodecs-filters/encoder2.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/images/ucodecs-filters/forward.png` & `blosc2-2.2.2/examples/images/ucodecs-filters/forward.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/images/ucodecs-filters/forward.svg` & `blosc2-2.2.2/examples/images/ucodecs-filters/forward.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/ndarray/asarray.py` & `blosc2-2.2.2/examples/ndarray/asarray.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/ndarray/buffer.py` & `blosc2-2.2.2/examples/ndarray/buffer.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/ndarray/bytedelta_filter.py` & `blosc2-2.2.2/examples/ndarray/bytedelta_filter.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/ndarray/copy.py` & `blosc2-2.2.2/examples/ndarray/copy.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/ndarray/empty.py` & `blosc2-2.2.2/examples/ndarray/empty.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/ndarray/formats.py` & `blosc2-2.2.2/examples/ndarray/formats.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/ndarray/getitem.py` & `blosc2-2.2.2/examples/ndarray/getitem.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/ndarray/meta.py` & `blosc2-2.2.2/examples/ndarray/meta.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/ndarray/ndmean.py` & `blosc2-2.2.2/examples/ndarray/ndmean.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/ndarray/persistency.py` & `blosc2-2.2.2/examples/ndarray/persistency.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/ndarray/resize.py` & `blosc2-2.2.2/examples/ndarray/resize.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/ndarray/work_with_numpy.py` & `blosc2-2.2.2/examples/ndarray/work_with_numpy.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/ndarray/zfp_codec.py` & `blosc2-2.2.2/examples/ndarray/zfp_codec.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/pack_array.py` & `blosc2-2.2.2/examples/pack_array.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/pack_tensor.py` & `blosc2-2.2.2/examples/pack_tensor.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/postfilter1.py` & `blosc2-2.2.2/examples/postfilter1.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/postfilter2.py` & `blosc2-2.2.2/examples/postfilter2.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/postfilter3.py` & `blosc2-2.2.2/examples/postfilter3.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/postfilters.ipynb` & `blosc2-2.2.2/examples/postfilters.ipynb`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/prefilter.py` & `blosc2-2.2.2/examples/prefilter.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/prefilters.ipynb` & `blosc2-2.2.2/examples/prefilters.ipynb`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/save_tensor.py` & `blosc2-2.2.2/examples/save_tensor.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/schunk.py` & `blosc2-2.2.2/examples/schunk.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/schunk_roundtrip.py` & `blosc2-2.2.2/examples/schunk_roundtrip.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/slicing_and_beyond.ipynb` & `blosc2-2.2.2/examples/slicing_and_beyond.ipynb`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/tutorial-basics.ipynb` & `blosc2-2.2.2/examples/tutorial-basics.ipynb`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/ucodecs-ufilters.ipynb` & `blosc2-2.2.2/examples/ucodecs-ufilters.ipynb`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/ucodecs.py` & `blosc2-2.2.2/examples/ucodecs.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/ufilters.py` & `blosc2-2.2.2/examples/ufilters.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/examples/vlmeta.py` & `blosc2-2.2.2/examples/vlmeta.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/images/Complete-Write-Read-B2ND.png` & `blosc2-2.2.2/images/Complete-Write-Read-B2ND.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/images/M1-i386-vs-arm64-pack.png` & `blosc2-2.2.2/images/M1-i386-vs-arm64-pack.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/images/M1-i386-vs-arm64-unpack.png` & `blosc2-2.2.2/images/M1-i386-vs-arm64-unpack.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/images/Read-Partial-Slices-B2ND.png` & `blosc2-2.2.2/images/Read-Partial-Slices-B2ND.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/images/b2nd-2level-parts.png` & `blosc2-2.2.2/images/b2nd-2level-parts.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/images/linspace-compress.png` & `blosc2-2.2.2/images/linspace-compress.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/images/linspace-decompress.png` & `blosc2-2.2.2/images/linspace-decompress.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/images/pack-array-cratios.png` & `blosc2-2.2.2/images/pack-array-cratios.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/ndarray/test_auto_parts.py` & `blosc2-2.2.2/tests/ndarray/test_auto_parts.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/ndarray/test_buffer.py` & `blosc2-2.2.2/tests/ndarray/test_buffer.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/ndarray/test_copy.py` & `blosc2-2.2.2/tests/ndarray/test_copy.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/ndarray/test_empty.py` & `blosc2-2.2.2/tests/ndarray/test_empty.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/ndarray/test_full.py` & `blosc2-2.2.2/tests/ndarray/test_full.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/ndarray/test_getitem.py` & `blosc2-2.2.2/tests/ndarray/test_getitem.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/ndarray/test_lossy.py` & `blosc2-2.2.2/tests/ndarray/test_lossy.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/ndarray/test_metalayers.py` & `blosc2-2.2.2/tests/ndarray/test_metalayers.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/ndarray/test_mode.py` & `blosc2-2.2.2/tests/ndarray/test_mode.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/ndarray/test_numpy.py` & `blosc2-2.2.2/tests/ndarray/test_numpy.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/ndarray/test_persistency.py` & `blosc2-2.2.2/tests/ndarray/test_persistency.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/ndarray/test_resize.py` & `blosc2-2.2.2/tests/ndarray/test_resize.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/ndarray/test_setitem.py` & `blosc2-2.2.2/tests/ndarray/test_setitem.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/ndarray/test_slice.py` & `blosc2-2.2.2/tests/ndarray/test_slice.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/ndarray/test_squeeze.py` & `blosc2-2.2.2/tests/ndarray/test_squeeze.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/ndarray/test_struct_dtype.py` & `blosc2-2.2.2/tests/ndarray/test_struct_dtype.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/ndarray/test_zeros.py` & `blosc2-2.2.2/tests/ndarray/test_zeros.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_bytes_array.py` & `blosc2-2.2.2/tests/test_bytes_array.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_comp_info.py` & `blosc2-2.2.2/tests/test_comp_info.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_compress2.py` & `blosc2-2.2.2/tests/test_compress2.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_compression_parameters.py` & `blosc2-2.2.2/tests/test_compression_parameters.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_compressors.py` & `blosc2-2.2.2/tests/test_compressors.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_decompress.py` & `blosc2-2.2.2/tests/test_decompress.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_iterchunks.py` & `blosc2-2.2.2/tests/test_iterchunks.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_open.py` & `blosc2-2.2.2/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_postfilters.py` & `blosc2-2.2.2/tests/test_postfilters.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_prefilters.py` & `blosc2-2.2.2/tests/test_prefilters.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_python_blosc.py` & `blosc2-2.2.2/tests/test_python_blosc.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_schunk.py` & `blosc2-2.2.2/tests/test_schunk.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_schunk_constructor.py` & `blosc2-2.2.2/tests/test_schunk_constructor.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_schunk_delete.py` & `blosc2-2.2.2/tests/test_schunk_delete.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_schunk_get_slice.py` & `blosc2-2.2.2/tests/test_schunk_get_slice.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_schunk_insert.py` & `blosc2-2.2.2/tests/test_schunk_insert.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_schunk_set_slice.py` & `blosc2-2.2.2/tests/test_schunk_set_slice.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_schunk_update.py` & `blosc2-2.2.2/tests/test_schunk_update.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_tensor.py` & `blosc2-2.2.2/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_ucodecs.py` & `blosc2-2.2.2/tests/test_ucodecs.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_ufilters.py` & `blosc2-2.2.2/tests/test_ufilters.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.2.1/tests/test_vlmeta.py` & `blosc2-2.2.2/tests/test_vlmeta.py`

 * *Files identical despite different names*

