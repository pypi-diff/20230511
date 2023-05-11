# Comparing `tmp/scikit-build-0.8.1.tar.gz` & `tmp/scikit-build-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scikit-build-0.8.1.tar", last modified: Wed Oct  3 13:44:40 2018, max compression
+gzip compressed data, was "dist/scikit-build-0.9.0.tar", last modified: Tue Mar  5 16:40:00 2019, max compression
```

## Comparing `scikit-build-0.8.1.tar` & `scikit-build-0.9.0.tar`

### file list

```diff
@@ -1,263 +1,352 @@
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    68611 2018-10-03 13:39:41.000000 scikit-build-0.8.1/versioneer.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      243 2018-10-03 13:44:40.000000 scikit-build-0.8.1/setup.cfg
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      201 2018-10-03 13:39:41.000000 scikit-build-0.8.1/requirements-dev.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3289 2018-10-03 13:39:41.000000 scikit-build-0.8.1/CONTRIBUTING.rst
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/docs/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     6466 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/make.bat
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1545 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/skbuild.platform_specifics.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       27 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/authors.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1304 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/index.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       27 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/changes.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       32 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/contributing.rst
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/docs/cmake-modules/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       76 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/cmake-modules/NumPy.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      165 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/cmake-modules/targetLinkLibrariesWithDynamicLookup.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       74 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/cmake-modules/F2PY.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      144 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/cmake-modules/Cython.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      109 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/cmake-modules/PythonExtensions.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    16707 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/usage.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4747 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/make_a_release.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1120 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/hacking.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       28 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/history.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      968 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/skbuild.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      611 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/cmake-modules.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2015 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/skbuild.command.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    17656 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/generators.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     6777 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/Makefile
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2118 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/installation.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     8981 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/conf.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       58 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/modules.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      133 2018-10-03 13:39:41.000000 scikit-build-0.8.1/docs/skbuild.utils.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       42 2018-10-03 13:39:41.000000 scikit-build-0.8.1/requirements.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      388 2018-10-03 13:39:41.000000 scikit-build-0.8.1/MANIFEST.in
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     5740 2018-10-03 13:42:26.000000 scikit-build-0.8.1/README.rst
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/scikit_build.egg-info/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        8 2018-10-03 13:44:40.000000 scikit-build-0.8.1/scikit_build.egg-info/top_level.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       43 2018-10-03 13:44:40.000000 scikit-build-0.8.1/scikit_build.egg-info/requires.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        1 2018-10-03 13:44:40.000000 scikit-build-0.8.1/scikit_build.egg-info/dependency_links.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        1 2018-10-03 13:44:40.000000 scikit-build-0.8.1/scikit_build.egg-info/not-zip-safe
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     9505 2018-10-03 13:44:40.000000 scikit-build-0.8.1/scikit_build.egg-info/SOURCES.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     7432 2018-10-03 13:44:40.000000 scikit-build-0.8.1/scikit_build.egg-info/PKG-INFO
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      213 2018-10-03 13:39:41.000000 scikit-build-0.8.1/HISTORY.rst
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2744 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_cmakelists_not_in_top_level_dir.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    34404 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_setup.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4005 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_platform.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1736 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_distribution.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4542 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_issue342_cmake_osx_args_in_setup.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4601 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_include_exclude_data.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      832 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_skbuild_variable.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     5126 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_broken_project.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1325 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_outside_project_root.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      194 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_issue334_configure_cmakelists_non_cp1252_encoding.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1935 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_hello_cython.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      813 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_issue274_support_one_package_without_package_dir.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3668 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_issue352_isolated_environment_support.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4867 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_skbuild.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2111 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_manifest_in.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     6363 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_hello_cpp.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/test-hide-listing/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      233 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-hide-listing/CMakeLists.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-hide-listing/bonjourModule.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/test-hide-listing/hello/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      116 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-hide-listing/hello/CMakeLists.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       31 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-hide-listing/hello/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       77 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-hide-listing/hello/__main__.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/test-hide-listing/bonjour/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-hide-listing/bonjour/__init__.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/test-hide-listing/bonjour/data/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        6 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-hide-listing/bonjour/data/soleil.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        5 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-hide-listing/bonjour/data/terre.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        4 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-hide-listing/bonjour/data/ciel.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      322 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-hide-listing/setup.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/cmakelists-not-in-top-level-dir/
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/cmakelists-not-in-top-level-dir/hello/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1553 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/cmakelists-not-in-top-level-dir/hello/_hello.cxx
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      217 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/cmakelists-not-in-top-level-dir/hello/CMakeLists.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/cmakelists-not-in-top-level-dir/hello/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       87 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/cmakelists-not-in-top-level-dir/hello/__main__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      262 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/cmakelists-not-in-top-level-dir/setup.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/hello2/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/hello2/hello2_include_from_manifest.txt
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/hello2/data2/
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/hello2/data2/subdata2/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       23 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/hello2/data2/subdata2/hello2_data1_include_from_manifest.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/hello2/data2/subdata2/hello2_data2_include_from_manifest.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/hello2/data2/subdata2/hello2_data3_include_from_manifest_and_exclude_from_manifest.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/hello2/data2/subdata2/hello2_data4_include_from_manifest_and_exclude_from_setup.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/hello2/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1965 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/CMakeLists.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      218 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/MANIFEST.in
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/hello/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/hello/hello_include_from_manifest.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/hello/__init__.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/hello/data/
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/hello/data/subdata/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/hello/data/subdata/hello_data3_include_from_manifest_and_exclude_from_manifest.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/hello/data/subdata/hello_data2_include_from_manifest.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/hello/data/subdata/hello_data4_include_from_manifest_and_exclude_from_setup.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       23 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/hello/data/subdata/hello_data1_include_from_manifest.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      360 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data/setup.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/fail-with-syntax-error-cmakelists/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      227 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/fail-with-syntax-error-cmakelists/CMakeLists.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      302 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/fail-with-syntax-error-cmakelists/setup.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/manifest-in/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       35 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/manifest-in/MANIFEST.in
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/manifest-in/hello/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/manifest-in/hello/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      224 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/manifest-in/setup.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       45 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/manifest-in/not_included.txt
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/fail-outside-project-root/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      833 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/fail-outside-project-root/CMakeLists.txt
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/fail-outside-project-root/other_project/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      127 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/fail-outside-project-root/other_project/CMakeLists.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/fail-outside-project-root/dummy
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      301 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/fail-outside-project-root/setup.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/fail-unless-skbuild-set/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      227 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/fail-unless-skbuild-set/CMakeLists.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      264 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/fail-unless-skbuild-set/setup.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/issue-274-support-one-package-without-package-dir/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      294 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/issue-274-support-one-package-without-package-dir/CMakeLists.txt
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/issue-274-support-one-package-without-package-dir/hello_tests/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      448 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/issue-274-support-one-package-without-package-dir/hello_tests/__init__.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/issue-274-support-one-package-without-package-dir/hello/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       31 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/issue-274-support-one-package-without-package-dir/hello/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      228 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/issue-274-support-one-package-without-package-dir/setup.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/hello-pure/
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/hello-pure/hello/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-pure/hello/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      204 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-pure/setup.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/src/
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/src/hello2/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/src/hello2/hello2_include_from_manifest.txt
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/src/hello2/data2/
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/src/hello2/data2/subdata2/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       23 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/src/hello2/data2/subdata2/hello2_data1_include_from_manifest.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/src/hello2/data2/subdata2/hello2_data2_include_from_manifest.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/src/hello2/data2/subdata2/hello2_data3_include_from_manifest_and_exclude_from_manifest.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/src/hello2/data2/subdata2/hello2_data4_include_from_manifest_and_exclude_from_setup.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/src/hello2/__init__.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/src/hello/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/src/hello/hello_include_from_manifest.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/src/hello/__init__.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/src/hello/data/
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/src/hello/data/subdata/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/src/hello/data/subdata/hello_data3_include_from_manifest_and_exclude_from_manifest.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/src/hello/data/subdata/hello_data2_include_from_manifest.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/src/hello/data/subdata/hello_data4_include_from_manifest_and_exclude_from_setup.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       23 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/src/hello/data/subdata/hello_data1_include_from_manifest.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1979 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/CMakeLists.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      238 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/MANIFEST.in
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      398 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/setup.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/hello-cython/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      157 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-cython/CMakeLists.txt
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/hello-cython/hello/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      151 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-cython/hello/CMakeLists.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      229 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-cython/hello/_hello.pyx
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-cython/hello/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       87 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-cython/hello/__main__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      353 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-cython/setup.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/fail-hello-with-compile-error/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      120 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/fail-hello-with-compile-error/CMakeLists.txt
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/fail-hello-with-compile-error/hello/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1613 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/fail-hello-with-compile-error/hello/_hello.cxx
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      121 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/fail-hello-with-compile-error/hello/CMakeLists.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/fail-hello-with-compile-error/hello/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       87 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/fail-hello-with-compile-error/hello/__main__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      309 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/fail-hello-with-compile-error/setup.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/issue-334-configure-cmakelist-non-cp1252-encoding/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      265 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/issue-334-configure-cmakelist-non-cp1252-encoding/CMakeLists.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      191 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/issue-334-configure-cmakelist-non-cp1252-encoding/setup.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/issue-274-support-default-package-dir/
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/issue-274-support-default-package-dir/src/
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/issue-274-support-default-package-dir/src/hello/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       31 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/issue-274-support-default-package-dir/src/hello/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      298 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/issue-274-support-default-package-dir/CMakeLists.txt
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/issue-274-support-default-package-dir/hello_tests/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      448 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/issue-274-support-default-package-dir/hello_tests/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      257 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/issue-274-support-default-package-dir/setup.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/fail-with-fatal-error-cmakelists/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      204 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/fail-with-fatal-error-cmakelists/CMakeLists.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      305 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/fail-with-fatal-error-cmakelists/setup.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/issue-335-support-cmake-source-dir/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      599 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/issue-335-support-cmake-source-dir/CMakeLists.txt
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/issue-335-support-cmake-source-dir/wrapping/
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/issue-335-support-cmake-source-dir/wrapping/python/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      243 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/issue-335-support-cmake-source-dir/wrapping/python/CMakeLists.txt
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/issue-335-support-cmake-source-dir/wrapping/python/hello/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/issue-335-support-cmake-source-dir/wrapping/python/hello/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      289 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/issue-335-support-cmake-source-dir/wrapping/python/setup.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/hello-no-language/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      129 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-no-language/CMakeLists.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      186 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-no-language/setup.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/hello-cpp/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      551 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-cpp/CMakeLists.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-cpp/bonjourModule.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/hello-cpp/hello/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1553 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-cpp/hello/_hello.cxx
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      238 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-cpp/hello/CMakeLists.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-cpp/hello/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       87 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-cpp/hello/__main__.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/hello-cpp/bonjour/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-cpp/bonjour/__init__.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/tests/samples/hello-cpp/bonjour/data/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        6 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-cpp/bonjour/data/soleil.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        5 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-cpp/bonjour/data/terre.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        4 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-cpp/bonjour/data/ciel.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      322 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/samples/hello-cpp/setup.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     6053 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_utils.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1052 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_issue335_support_cmake_source_dir.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      789 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_issue274_support_default_package_dir.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    11192 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4668 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_command_line.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     6105 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_cmaker.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2608 2018-10-03 13:39:41.000000 scikit-build-0.8.1/tests/test_hello_pure.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/skbuild/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      373 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/exceptions.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    35404 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/setuptools_wrap.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      497 2018-10-03 13:44:40.000000 scikit-build-0.8.1/skbuild/_version.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/skbuild/platform_specifics/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      466 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/platform_specifics/unix.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      227 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/platform_specifics/bsd.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      827 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/platform_specifics/platform_factory.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      303 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/platform_specifics/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      623 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/platform_specifics/osx.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2903 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/platform_specifics/linux.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     8685 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/platform_specifics/abstract.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     6994 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/platform_specifics/windows.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/skbuild/command/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3170 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/command/generate_source_manifest.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3858 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/command/build_py.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      958 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/command/install.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3252 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/command/bdist_wheel.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1065 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/command/clean.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      719 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/command/install_lib.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      416 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/command/bdist.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1465 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/command/sdist.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      640 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/command/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1916 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/command/egg_info.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      483 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/command/test.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      739 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/command/install_scripts.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      416 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/command/build.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    19111 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/cmaker.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      918 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/constants.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      800 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/compat.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/skbuild/utils/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     8051 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/utils/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      458 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/__init__.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/skbuild/resources/
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2018-10-03 13:44:40.000000 scikit-build-0.8.1/skbuild/resources/cmake/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3139 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/resources/cmake/FindF2PY.cmake
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    21390 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/resources/cmake/FindPythonExtensions.cmake
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2638 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/resources/cmake/FindCython.cmake
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    13678 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/resources/cmake/UseCython.cmake
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4075 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/resources/cmake/FindNumPy.cmake
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    16669 2018-10-03 13:39:41.000000 scikit-build-0.8.1/skbuild/resources/cmake/targetLinkLibrariesWithDynamicLookup.cmake
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      129 2018-10-03 13:39:41.000000 scikit-build-0.8.1/AUTHORS.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2764 2018-10-03 13:39:41.000000 scikit-build-0.8.1/LICENSE
--rwxrwxr-x   0 jcfr      (1000) jcfr      (1000)     2285 2018-10-03 13:39:41.000000 scikit-build-0.8.1/setup.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     7432 2018-10-03 13:44:40.000000 scikit-build-0.8.1/PKG-INFO
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    68611 2018-08-06 03:59:14.000000 scikit-build-0.9.0/versioneer.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      222 2019-03-05 16:40:00.000000 scikit-build-0.9.0/setup.cfg
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      201 2018-10-03 13:41:06.000000 scikit-build-0.9.0/requirements-dev.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3289 2018-07-14 22:29:55.000000 scikit-build-0.9.0/CONTRIBUTING.rst
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/docs/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     6466 2016-09-13 08:20:34.000000 scikit-build-0.9.0/docs/make.bat
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1545 2018-07-14 22:29:55.000000 scikit-build-0.9.0/docs/skbuild.platform_specifics.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       27 2016-09-13 08:20:34.000000 scikit-build-0.9.0/docs/authors.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1304 2018-08-06 04:44:00.000000 scikit-build-0.9.0/docs/index.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       27 2018-07-14 22:29:55.000000 scikit-build-0.9.0/docs/changes.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       32 2016-09-13 08:20:34.000000 scikit-build-0.9.0/docs/contributing.rst
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/docs/cmake-modules/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       76 2018-07-14 22:29:55.000000 scikit-build-0.9.0/docs/cmake-modules/NumPy.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      165 2018-07-14 22:29:55.000000 scikit-build-0.9.0/docs/cmake-modules/targetLinkLibrariesWithDynamicLookup.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       74 2018-07-14 22:29:55.000000 scikit-build-0.9.0/docs/cmake-modules/F2PY.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      144 2018-07-14 22:29:55.000000 scikit-build-0.9.0/docs/cmake-modules/Cython.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      109 2018-07-14 22:29:55.000000 scikit-build-0.9.0/docs/cmake-modules/PythonExtensions.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    16708 2019-01-09 22:28:39.000000 scikit-build-0.9.0/docs/usage.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4801 2018-10-03 14:31:59.000000 scikit-build-0.9.0/docs/make_a_release.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1120 2018-07-14 22:29:55.000000 scikit-build-0.9.0/docs/hacking.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       28 2016-09-13 08:20:34.000000 scikit-build-0.9.0/docs/history.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      968 2019-01-08 21:05:21.000000 scikit-build-0.9.0/docs/skbuild.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      611 2018-07-14 22:29:55.000000 scikit-build-0.9.0/docs/cmake-modules.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2015 2018-07-14 22:29:55.000000 scikit-build-0.9.0/docs/skbuild.command.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    17656 2018-08-03 07:41:14.000000 scikit-build-0.9.0/docs/generators.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     6777 2016-12-20 10:05:21.000000 scikit-build-0.9.0/docs/Makefile
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2118 2018-08-03 07:41:14.000000 scikit-build-0.9.0/docs/installation.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     8981 2019-01-08 21:06:38.000000 scikit-build-0.9.0/docs/conf.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       58 2019-01-08 21:05:21.000000 scikit-build-0.9.0/docs/modules.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      133 2018-07-14 22:29:55.000000 scikit-build-0.9.0/docs/skbuild.utils.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       42 2018-07-14 22:29:55.000000 scikit-build-0.9.0/requirements.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      388 2018-08-06 03:59:14.000000 scikit-build-0.9.0/MANIFEST.in
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     5740 2019-03-05 16:38:22.000000 scikit-build-0.9.0/README.rst
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/scikit_build.egg-info/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        8 2019-03-05 16:40:00.000000 scikit-build-0.9.0/scikit_build.egg-info/top_level.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       43 2019-03-05 16:40:00.000000 scikit-build-0.9.0/scikit_build.egg-info/requires.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        1 2019-03-05 16:40:00.000000 scikit-build-0.9.0/scikit_build.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        1 2019-03-05 16:40:00.000000 scikit-build-0.9.0/scikit_build.egg-info/not-zip-safe
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    16371 2019-03-05 16:40:00.000000 scikit-build-0.9.0/scikit_build.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     7432 2019-03-05 16:40:00.000000 scikit-build-0.9.0/scikit_build.egg-info/PKG-INFO
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      213 2016-11-01 15:00:02.000000 scikit-build-0.9.0/HISTORY.rst
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2744 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/test_cmakelists_not_in_top_level_dir.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    34432 2019-01-09 22:28:39.000000 scikit-build-0.9.0/tests/test_setup.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4005 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/test_platform.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1736 2018-10-03 13:41:06.000000 scikit-build-0.9.0/tests/test_distribution.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4542 2019-01-08 20:18:26.000000 scikit-build-0.9.0/tests/test_issue342_cmake_osx_args_in_setup.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4601 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/test_include_exclude_data.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      832 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/test_skbuild_variable.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     5126 2018-08-03 07:41:14.000000 scikit-build-0.9.0/tests/test_broken_project.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1325 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/test_outside_project_root.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      194 2018-07-15 05:13:31.000000 scikit-build-0.9.0/tests/test_issue334_configure_cmakelists_non_cp1252_encoding.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1935 2018-07-15 14:53:07.000000 scikit-build-0.9.0/tests/test_hello_cython.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      813 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/test_issue274_support_one_package_without_package_dir.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    76627 2018-08-03 06:58:40.000000 scikit-build-0.9.0/tests/.coverage
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      464 2019-01-10 18:39:56.000000 scikit-build-0.9.0/tests/test_issue284_build_ext_inplace.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3670 2019-01-09 22:28:39.000000 scikit-build-0.9.0/tests/test_issue352_isolated_environment_support.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4869 2019-03-05 16:35:18.000000 scikit-build-0.9.0/tests/test_skbuild.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    64366 2019-01-10 03:26:40.000000 scikit-build-0.9.0/tests/coverage.xml
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2111 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/test_manifest_in.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     6381 2019-01-09 22:28:39.000000 scikit-build-0.9.0/tests/test_hello_cpp.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/test-hide-listing/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      233 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-hide-listing/CMakeLists.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-hide-listing/bonjourModule.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/test-hide-listing/hello/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      116 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-hide-listing/hello/CMakeLists.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       31 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-hide-listing/hello/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       77 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-hide-listing/hello/__main__.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/test-hide-listing/bonjour/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-hide-listing/bonjour/__init__.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/test-hide-listing/bonjour/data/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        6 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-hide-listing/bonjour/data/soleil.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        5 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-hide-listing/bonjour/data/terre.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        4 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-hide-listing/bonjour/data/ciel.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      322 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-hide-listing/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/cmakelists-not-in-top-level-dir/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/cmakelists-not-in-top-level-dir/hello/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1553 2018-05-28 18:15:28.000000 scikit-build-0.9.0/tests/samples/cmakelists-not-in-top-level-dir/hello/_hello.cxx
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      217 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/cmakelists-not-in-top-level-dir/hello/CMakeLists.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-05-28 18:15:28.000000 scikit-build-0.9.0/tests/samples/cmakelists-not-in-top-level-dir/hello/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       87 2018-05-28 18:15:28.000000 scikit-build-0.9.0/tests/samples/cmakelists-not-in-top-level-dir/hello/__main__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      262 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/cmakelists-not-in-top-level-dir/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      234 2019-01-10 18:39:56.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/CMakeLists.txt
+-rwxrwxr-x   0 jcfr      (1000) jcfr      (1000)    23144 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_hello_ext.cpython-35m-x86_64-linux-gnu.so
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/hello/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1573 2019-01-10 18:39:56.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/hello/_hello_ext.cxx
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1568 2019-01-10 18:39:56.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/hello/_hello_sk.cxx
+-rw-r--r--   0 jcfr      (1000) jcfr      (1000)     8736 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/hello/_hello_sk.cpython-35m-x86_64-linux-gnu.so
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2019-01-10 18:39:56.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/hello/__init__.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/setuptools/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/setuptools/lib.linux-x86_64-3.5/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/setuptools/lib.linux-x86_64-3.5/papa/
+-rwxrwxr-x   0 jcfr      (1000) jcfr      (1000)    23144 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/setuptools/lib.linux-x86_64-3.5/papa/_hello_ext.cpython-35m-x86_64-linux-gnu.so
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/setuptools/temp.linux-x86_64-3.5/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/setuptools/temp.linux-x86_64-3.5/hello/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    30648 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/setuptools/temp.linux-x86_64-3.5/hello/_hello_ext.o
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      162 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/install_manifest.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      237 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/.ninja_log
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/src/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       98 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/src/counter.h
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      668 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/src/CMakeLists.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      149 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/src/counter.c
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1168 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/src/main.c
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      157 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/src/number.c
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      136 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/src/number.h
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/build/
+-rwxrwxr-x   0 jcfr      (1000) jcfr      (1000)     7936 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/build/libnumber.so
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      396 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/build/.ninja_log
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/build/CMakeFiles/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       85 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/build/CMakeFiles/cmake.check_cache
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      955 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/build/CMakeFiles/TargetDirectories.txt
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/build/CMakeFiles/main.dir/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2384 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/build/CMakeFiles/main.dir/main.c.o
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/build/CMakeFiles/number.dir/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1496 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/build/CMakeFiles/number.dir/number.c.o
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/build/CMakeFiles/counter.dir/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1488 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/build/CMakeFiles/counter.dir/counter.c.o
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3380 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/build/rules.ninja
+-rwxrwxr-x   0 jcfr      (1000) jcfr      (1000)     8896 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/build/main
+-rwxrwxr-x   0 jcfr      (1000) jcfr      (1000)     7952 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/build/counter.so
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1776 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/build/cmake_install.cmake
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    11325 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/build/build.ninja
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      184 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/build/.ninja_deps
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    10048 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeTmp/link_flags/gnu_ld_ignore/MODULE/SHARED/build/CMakeCache.txt
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    10011 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/feature_tests.cxx
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       85 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/cmake.check_cache
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      991 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/TargetDirectories.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      688 2019-01-10 13:53:05.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/feature_tests.c
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       39 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/_hello_sk-version-script.map
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/_hello_sk.dir/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/_hello_sk.dir/hello/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3416 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/_hello_sk.dir/hello/_hello_sk.cxx.o
+-rwxrwxr-x   0 jcfr      (1000) jcfr      (1000)    12616 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/feature_tests.bin
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/3.10.0/
+-rwxrwxr-x   0 jcfr      (1000) jcfr      (1000)     8568 2019-01-10 13:53:05.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/3.10.0/CMakeDetermineCompilerABI_CXX.bin
+-rwxrwxr-x   0 jcfr      (1000) jcfr      (1000)     8560 2019-01-10 13:53:05.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/3.10.0/CMakeDetermineCompilerABI_C.bin
+-rw-r--r--   0 jcfr      (1000) jcfr      (1000)     2219 2019-01-10 13:53:05.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/3.10.0/CMakeCCompiler.cmake
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/3.10.0/CompilerIdC/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    18076 2019-01-10 13:53:05.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/3.10.0/CompilerIdC/CMakeCCompilerId.c
+-rwxrwxr-x   0 jcfr      (1000) jcfr      (1000)     8720 2019-01-10 13:53:05.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/3.10.0/CompilerIdC/a.out
+-rw-r--r--   0 jcfr      (1000) jcfr      (1000)      398 2019-01-10 13:53:05.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/3.10.0/CMakeSystem.cmake
+-rw-r--r--   0 jcfr      (1000) jcfr      (1000)     4849 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/3.10.0/CMakeCXXCompiler.cmake
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/3.10.0/CompilerIdCXX/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    17631 2019-01-10 13:53:05.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/3.10.0/CompilerIdCXX/CMakeCXXCompilerId.cpp
+-rwxrwxr-x   0 jcfr      (1000) jcfr      (1000)     8728 2019-01-10 13:53:05.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/3.10.0/CompilerIdCXX/a.out
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    38747 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeFiles/CMakeOutput.log
+-rwxrwxr-x   0 jcfr      (1000) jcfr      (1000)     8736 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/_hello_sk.cpython-35m-x86_64-linux-gnu.so
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2117 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/rules.ninja
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      155 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeSpec.json
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2839 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/cmake_install.cmake
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    25703 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/build.ninja
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     8308 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/.ninja_deps
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    15202 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-build/CMakeCache.txt
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-install/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-install/hello/
+-rw-r--r--   0 jcfr      (1000) jcfr      (1000)     8736 2019-01-10 13:53:06.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/_skbuild/linux-x86_64-3.5/cmake-install/hello/_hello_sk.cpython-35m-x86_64-linux-gnu.so
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      364 2019-01-10 18:39:56.000000 scikit-build-0.9.0/tests/samples/issue-284-build-ext-inplace/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/hello2/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/hello2/hello2_include_from_manifest.txt
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/hello2/data2/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/hello2/data2/subdata2/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       23 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/hello2/data2/subdata2/hello2_data1_include_from_manifest.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/hello2/data2/subdata2/hello2_data2_include_from_manifest.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/hello2/data2/subdata2/hello2_data3_include_from_manifest_and_exclude_from_manifest.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/hello2/data2/subdata2/hello2_data4_include_from_manifest_and_exclude_from_setup.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/hello2/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1965 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/CMakeLists.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      218 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/MANIFEST.in
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/hello/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/hello/hello_include_from_manifest.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/hello/__init__.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/hello/data/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/hello/data/subdata/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/hello/data/subdata/hello_data3_include_from_manifest_and_exclude_from_manifest.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/hello/data/subdata/hello_data2_include_from_manifest.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/hello/data/subdata/hello_data4_include_from_manifest_and_exclude_from_setup.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       23 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/hello/data/subdata/hello_data1_include_from_manifest.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      360 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/fail-with-syntax-error-cmakelists/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      227 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/fail-with-syntax-error-cmakelists/CMakeLists.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      302 2018-05-11 12:09:33.000000 scikit-build-0.9.0/tests/samples/fail-with-syntax-error-cmakelists/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/manifest-in/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       35 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/manifest-in/MANIFEST.in
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/manifest-in/hello/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/manifest-in/hello/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      224 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/manifest-in/setup.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       45 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/manifest-in/not_included.txt
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/fail-outside-project-root/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      833 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/fail-outside-project-root/CMakeLists.txt
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/fail-outside-project-root/other_project/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      127 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/fail-outside-project-root/other_project/CMakeLists.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2016-09-13 08:20:34.000000 scikit-build-0.9.0/tests/samples/fail-outside-project-root/dummy
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      301 2018-05-11 12:09:42.000000 scikit-build-0.9.0/tests/samples/fail-outside-project-root/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/fail-unless-skbuild-set/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      227 2016-09-13 08:20:34.000000 scikit-build-0.9.0/tests/samples/fail-unless-skbuild-set/CMakeLists.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      264 2018-05-11 12:09:40.000000 scikit-build-0.9.0/tests/samples/fail-unless-skbuild-set/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-274-support-one-package-without-package-dir/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      294 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/issue-274-support-one-package-without-package-dir/CMakeLists.txt
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-274-support-one-package-without-package-dir/hello_tests/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      448 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/issue-274-support-one-package-without-package-dir/hello_tests/__init__.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-274-support-one-package-without-package-dir/hello/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       31 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/issue-274-support-one-package-without-package-dir/hello/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      228 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/issue-274-support-one-package-without-package-dir/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/hello-pure/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/hello-pure/hello/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2016-09-26 22:55:53.000000 scikit-build-0.9.0/tests/samples/hello-pure/hello/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      204 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/hello-pure/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/src/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/src/hello2/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/src/hello2/hello2_include_from_manifest.txt
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/src/hello2/data2/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/src/hello2/data2/subdata2/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       23 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/src/hello2/data2/subdata2/hello2_data1_include_from_manifest.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/src/hello2/data2/subdata2/hello2_data2_include_from_manifest.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/src/hello2/data2/subdata2/hello2_data3_include_from_manifest_and_exclude_from_manifest.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/src/hello2/data2/subdata2/hello2_data4_include_from_manifest_and_exclude_from_setup.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/src/hello2/__init__.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/src/hello/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/src/hello/hello_include_from_manifest.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/src/hello/__init__.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/src/hello/data/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/src/hello/data/subdata/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/src/hello/data/subdata/hello_data3_include_from_manifest_and_exclude_from_manifest.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/src/hello/data/subdata/hello_data2_include_from_manifest.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/src/hello/data/subdata/hello_data4_include_from_manifest_and_exclude_from_setup.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       23 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/src/hello/data/subdata/hello_data1_include_from_manifest.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1979 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/CMakeLists.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      238 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/MANIFEST.in
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      398 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/hello-cython/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      157 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/hello-cython/CMakeLists.txt
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/hello-cython/hello/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      151 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/hello-cython/hello/CMakeLists.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      229 2016-09-13 08:20:34.000000 scikit-build-0.9.0/tests/samples/hello-cython/hello/_hello.pyx
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2016-09-24 23:30:36.000000 scikit-build-0.9.0/tests/samples/hello-cython/hello/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       87 2016-09-24 23:30:36.000000 scikit-build-0.9.0/tests/samples/hello-cython/hello/__main__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      353 2018-08-03 07:41:14.000000 scikit-build-0.9.0/tests/samples/hello-cython/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/fail-hello-with-compile-error/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      120 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/fail-hello-with-compile-error/CMakeLists.txt
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/fail-hello-with-compile-error/hello/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1613 2016-09-26 22:55:53.000000 scikit-build-0.9.0/tests/samples/fail-hello-with-compile-error/hello/_hello.cxx
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      121 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/fail-hello-with-compile-error/hello/CMakeLists.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2016-09-26 22:55:53.000000 scikit-build-0.9.0/tests/samples/fail-hello-with-compile-error/hello/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       87 2016-09-26 22:55:53.000000 scikit-build-0.9.0/tests/samples/fail-hello-with-compile-error/hello/__main__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      309 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/fail-hello-with-compile-error/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-334-configure-cmakelist-non-cp1252-encoding/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      265 2018-07-15 05:13:31.000000 scikit-build-0.9.0/tests/samples/issue-334-configure-cmakelist-non-cp1252-encoding/CMakeLists.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      191 2018-07-15 05:13:31.000000 scikit-build-0.9.0/tests/samples/issue-334-configure-cmakelist-non-cp1252-encoding/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-274-support-default-package-dir/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-274-support-default-package-dir/src/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-274-support-default-package-dir/src/hello/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       31 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/issue-274-support-default-package-dir/src/hello/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      298 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/issue-274-support-default-package-dir/CMakeLists.txt
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-274-support-default-package-dir/hello_tests/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      448 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/issue-274-support-default-package-dir/hello_tests/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      257 2018-07-30 05:55:52.000000 scikit-build-0.9.0/tests/samples/issue-274-support-default-package-dir/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/fail-with-fatal-error-cmakelists/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      204 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/fail-with-fatal-error-cmakelists/CMakeLists.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      305 2018-05-11 12:09:37.000000 scikit-build-0.9.0/tests/samples/fail-with-fatal-error-cmakelists/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-335-support-cmake-source-dir/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      599 2018-07-15 14:53:07.000000 scikit-build-0.9.0/tests/samples/issue-335-support-cmake-source-dir/CMakeLists.txt
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-335-support-cmake-source-dir/wrapping/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-335-support-cmake-source-dir/wrapping/python/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      243 2018-07-15 14:53:07.000000 scikit-build-0.9.0/tests/samples/issue-335-support-cmake-source-dir/wrapping/python/CMakeLists.txt
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/issue-335-support-cmake-source-dir/wrapping/python/hello/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-15 14:53:07.000000 scikit-build-0.9.0/tests/samples/issue-335-support-cmake-source-dir/wrapping/python/hello/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      289 2018-07-15 14:53:07.000000 scikit-build-0.9.0/tests/samples/issue-335-support-cmake-source-dir/wrapping/python/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/hello-no-language/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      129 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/hello-no-language/CMakeLists.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      186 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/hello-no-language/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/hello-cpp/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      551 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/hello-cpp/CMakeLists.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/hello-cpp/bonjourModule.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/hello-cpp/hello/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1553 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/hello-cpp/hello/_hello.cxx
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      238 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/hello-cpp/hello/CMakeLists.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/hello-cpp/hello/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       87 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/hello-cpp/hello/__main__.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/hello-cpp/bonjour/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/hello-cpp/bonjour/__init__.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/tests/samples/hello-cpp/bonjour/data/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        6 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/hello-cpp/bonjour/data/soleil.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        5 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/hello-cpp/bonjour/data/terre.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        4 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/hello-cpp/bonjour/data/ciel.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      322 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/samples/hello-cpp/setup.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     6053 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/test_utils.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1052 2018-07-15 14:53:07.000000 scikit-build-0.9.0/tests/test_issue335_support_cmake_source_dir.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      789 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/test_issue274_support_default_package_dir.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    11416 2019-01-09 22:28:39.000000 scikit-build-0.9.0/tests/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4668 2018-07-14 22:29:55.000000 scikit-build-0.9.0/tests/test_command_line.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     6117 2019-01-09 22:28:39.000000 scikit-build-0.9.0/tests/test_cmaker.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2612 2019-01-09 22:28:39.000000 scikit-build-0.9.0/tests/test_hello_pure.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/skbuild/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      373 2018-07-14 22:29:55.000000 scikit-build-0.9.0/skbuild/exceptions.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    36889 2019-01-10 18:39:56.000000 scikit-build-0.9.0/skbuild/setuptools_wrap.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      497 2019-03-05 16:40:00.000000 scikit-build-0.9.0/skbuild/_version.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/skbuild/platform_specifics/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      466 2018-07-14 22:29:55.000000 scikit-build-0.9.0/skbuild/platform_specifics/unix.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      227 2018-07-14 22:29:55.000000 scikit-build-0.9.0/skbuild/platform_specifics/bsd.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      827 2018-07-14 22:29:55.000000 scikit-build-0.9.0/skbuild/platform_specifics/platform_factory.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      303 2018-07-14 22:29:55.000000 scikit-build-0.9.0/skbuild/platform_specifics/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      623 2018-07-14 22:29:55.000000 scikit-build-0.9.0/skbuild/platform_specifics/osx.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2903 2018-07-14 22:29:55.000000 scikit-build-0.9.0/skbuild/platform_specifics/linux.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     8685 2018-08-21 15:45:59.000000 scikit-build-0.9.0/skbuild/platform_specifics/abstract.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     6994 2019-03-05 16:35:18.000000 scikit-build-0.9.0/skbuild/platform_specifics/windows.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/skbuild/command/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3129 2019-01-09 22:28:39.000000 scikit-build-0.9.0/skbuild/command/generate_source_manifest.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1930 2019-01-10 18:39:56.000000 scikit-build-0.9.0/skbuild/command/build_ext.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3862 2019-01-10 02:58:49.000000 scikit-build-0.9.0/skbuild/command/build_py.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      958 2018-07-14 22:29:55.000000 scikit-build-0.9.0/skbuild/command/install.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3304 2019-01-09 22:28:39.000000 scikit-build-0.9.0/skbuild/command/bdist_wheel.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1071 2019-01-09 22:28:39.000000 scikit-build-0.9.0/skbuild/command/clean.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      719 2018-07-14 22:29:55.000000 scikit-build-0.9.0/skbuild/command/install_lib.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      416 2018-07-14 22:29:55.000000 scikit-build-0.9.0/skbuild/command/bdist.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1465 2018-07-14 22:29:55.000000 scikit-build-0.9.0/skbuild/command/sdist.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      642 2019-01-09 22:28:39.000000 scikit-build-0.9.0/skbuild/command/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1918 2019-01-09 22:28:39.000000 scikit-build-0.9.0/skbuild/command/egg_info.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      483 2018-07-14 22:29:55.000000 scikit-build-0.9.0/skbuild/command/test.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      739 2018-07-14 22:29:55.000000 scikit-build-0.9.0/skbuild/command/install_scripts.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      416 2018-07-14 22:29:55.000000 scikit-build-0.9.0/skbuild/command/build.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    19149 2019-01-09 22:28:39.000000 scikit-build-0.9.0/skbuild/cmaker.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1916 2019-01-09 22:28:39.000000 scikit-build-0.9.0/skbuild/constants.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      800 2018-07-14 22:29:55.000000 scikit-build-0.9.0/skbuild/compat.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/skbuild/utils/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     8051 2018-10-02 22:24:38.000000 scikit-build-0.9.0/skbuild/utils/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      458 2018-08-06 03:59:14.000000 scikit-build-0.9.0/skbuild/__init__.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/skbuild/resources/
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2019-03-05 16:40:00.000000 scikit-build-0.9.0/skbuild/resources/cmake/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     3139 2018-07-14 22:29:55.000000 scikit-build-0.9.0/skbuild/resources/cmake/FindF2PY.cmake
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    21440 2019-01-09 16:38:57.000000 scikit-build-0.9.0/skbuild/resources/cmake/FindPythonExtensions.cmake
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2638 2018-07-14 22:29:55.000000 scikit-build-0.9.0/skbuild/resources/cmake/FindCython.cmake
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    13678 2018-07-30 08:05:04.000000 scikit-build-0.9.0/skbuild/resources/cmake/UseCython.cmake
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     4075 2018-07-14 22:29:55.000000 scikit-build-0.9.0/skbuild/resources/cmake/FindNumPy.cmake
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    16669 2018-07-14 22:29:55.000000 scikit-build-0.9.0/skbuild/resources/cmake/targetLinkLibrariesWithDynamicLookup.cmake
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      129 2016-09-13 08:20:34.000000 scikit-build-0.9.0/AUTHORS.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2764 2016-09-13 08:20:34.000000 scikit-build-0.9.0/LICENSE
+-rwxrwxr-x   0 jcfr      (1000) jcfr      (1000)     2279 2019-02-27 14:47:01.000000 scikit-build-0.9.0/setup.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     7432 2019-03-05 16:40:00.000000 scikit-build-0.9.0/PKG-INFO
```

### Comparing `scikit-build-0.8.1/versioneer.py` & `scikit-build-0.9.0/versioneer.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/CONTRIBUTING.rst` & `scikit-build-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/docs/make.bat` & `scikit-build-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/docs/skbuild.platform_specifics.rst` & `scikit-build-0.9.0/docs/skbuild.platform_specifics.rst`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/docs/index.rst` & `scikit-build-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/docs/usage.rst` & `scikit-build-0.9.0/docs/usage.rst`

 * *Files 1% similar despite different names*

```diff
@@ -422,15 +422,15 @@
 Optimized incremental build
 ---------------------------
 
 To optimize the developer workflow, scikit-build reconfigures the CMake project only when
 needed. It caches the environment associated with the generator as well as the CMake execution
 properties.
 
-The CMake properties are saved in a :const:`CMake spec file <skbuild.constants.CMAKE_SPEC_FILE>` responsible
+The CMake properties are saved in a :func:`CMake spec file <skbuild.constants.CMAKE_SPEC_FILE()>` responsible
 to store the CMake executable path, the CMake configuration arguments, the CMake version as well as the
 environment variables ``PYTHONNOUSERSITE`` and ``PYTHONPATH``.
 
 If there are no ``CMakeCache.txt`` file or if any of the CMake properties changes, scikit-build will
 explicitly reconfigure the project calling :meth:`skbuild.cmaker.CMaker.configure`.
 
 If a file is added to the CMake build system by updating one of the ``CMakeLists.txt`` file, scikit-build
```

### Comparing `scikit-build-0.8.1/docs/make_a_release.rst` & `scikit-build-0.9.0/docs/make_a_release.rst`

 * *Files 2% similar despite different names*

```diff
@@ -115,34 +115,35 @@
       git commit -m "Scikit-build ${release}"
 
 
 7. Tag the release
 
   .. code::
 
-    $ git tag --sign -m "Scikit-build ${release}" ${release} origin/master
+    $ git tag --sign -m "Scikit-build ${release}" ${release} master
 
   .. warning::
 
       We recommend using a `GPG signing key <https://help.github.com/articles/generating-a-new-gpg-key/>`_
       to sign the tag.
 
 
 8. Create the source distribution and wheel
 
   .. code::
 
     $ python setup.py sdist bdist_wheel
 
 
-9. Publish the release tag
+9. Publish the both release tag and the master branch
 
   .. code::
 
-    $ git push origin ${release}
+    $ git push origin ${release} && \
+      git push origin master
 
 
 10. Upload the distributions on `PyPI`_
 
   .. code::
 
     twine upload dist/*
```

### Comparing `scikit-build-0.8.1/docs/hacking.rst` & `scikit-build-0.9.0/docs/hacking.rst`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/docs/skbuild.rst` & `scikit-build-0.9.0/docs/skbuild.rst`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/docs/cmake-modules.rst` & `scikit-build-0.9.0/docs/cmake-modules.rst`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/docs/skbuild.command.rst` & `scikit-build-0.9.0/docs/skbuild.command.rst`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/docs/generators.rst` & `scikit-build-0.9.0/docs/generators.rst`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/docs/Makefile` & `scikit-build-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/docs/installation.rst` & `scikit-build-0.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/docs/conf.py` & `scikit-build-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/README.rst` & `scikit-build-0.9.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 --------------
 
 .. table::
 
   +-----------------------------------------------------------------------------+-------------------------------------------------------------------------------+
   | Versions                                                                    | Downloads                                                                     |
   +=============================================================================+===============================================================================+
-  | .. image:: https://img.shields.io/pypi/v/scikit-build.svg                   | .. image:: https://img.shields.io/badge/downloads-54k%20total-green.svg       |
+  | .. image:: https://img.shields.io/pypi/v/scikit-build.svg                   | .. image:: https://img.shields.io/badge/downloads-95k%20total-green.svg       |
   |     :target: https://pypi.python.org/pypi/scikit-build                      |     :target: https://pypi.python.org/pypi/scikit-build                        |
   +-----------------------------------------------------------------------------+-------------------------------------------------------------------------------+
   | .. image:: https://anaconda.org/conda-forge/scikit-build/badges/version.svg | .. image:: https://anaconda.org/conda-forge/scikit-build/badges/downloads.svg |
   |     :target: https://anaconda.org/conda-forge/scikit-build                  |     :target: https://anaconda.org/conda-forge/scikit-build                    |
   +-----------------------------------------------------------------------------+-------------------------------------------------------------------------------+
```

### Comparing `scikit-build-0.8.1/scikit_build.egg-info/PKG-INFO` & `scikit-build-0.9.0/scikit_build.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scikit-build
-Version: 0.8.1
+Version: 0.9.0
 Summary: Improved build system generator for Python C/C++/Fortran/Cython extensions
 Home-page: https://github.com/scikit-build/scikit-build
 Author: The scikit-build team
 Author-email: scikit-build@googlegroups.com
 License: MIT
 Description: ===============================
         scikit-build
@@ -26,15 +26,15 @@
         --------------
         
         .. table::
         
           +-----------------------------------------------------------------------------+-------------------------------------------------------------------------------+
           | Versions                                                                    | Downloads                                                                     |
           +=============================================================================+===============================================================================+
-          | .. image:: https://img.shields.io/pypi/v/scikit-build.svg                   | .. image:: https://img.shields.io/badge/downloads-54k%20total-green.svg       |
+          | .. image:: https://img.shields.io/pypi/v/scikit-build.svg                   | .. image:: https://img.shields.io/badge/downloads-95k%20total-green.svg       |
           |     :target: https://pypi.python.org/pypi/scikit-build                      |     :target: https://pypi.python.org/pypi/scikit-build                        |
           +-----------------------------------------------------------------------------+-------------------------------------------------------------------------------+
           | .. image:: https://anaconda.org/conda-forge/scikit-build/badges/version.svg | .. image:: https://anaconda.org/conda-forge/scikit-build/badges/downloads.svg |
           |     :target: https://anaconda.org/conda-forge/scikit-build                  |     :target: https://anaconda.org/conda-forge/scikit-build                    |
           +-----------------------------------------------------------------------------+-------------------------------------------------------------------------------+
```

### Comparing `scikit-build-0.8.1/tests/test_cmakelists_not_in_top_level_dir.py` & `scikit-build-0.9.0/tests/test_cmakelists_not_in_top_level_dir.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/test_setup.py` & `scikit-build-0.9.0/tests/test_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         is_pure = False
         cmakelists_txt = tmpdir.join("CMakeLists.txt")
         cmakelists_txt.write(
             """
             cmake_minimum_required(VERSION 3.5.0)
             project(test NONE)
             install(CODE "execute_process(
-              COMMAND \${CMAKE_COMMAND} -E sleep 0)")
+              COMMAND \\${CMAKE_COMMAND} -E sleep 0)")
             """
         )
     else:
         raise Exception(
             "Unknown distribution_type: {}".format(distribution_type))
 
     platform = get_platform()
@@ -116,15 +116,15 @@
     tmp_dir.join('CMakeLists.txt').write(textwrap.dedent(
         """
         cmake_minimum_required(VERSION 3.5.0)
         project(test NONE)
         message(STATUS "VAR[${VAR}]")
         message(STATUS "VAR_WITH_SPACE[${VAR_WITH_SPACE}]")
         install(CODE "execute_process(
-          COMMAND \${CMAKE_COMMAND} -E sleep 0)")
+          COMMAND \\${CMAKE_COMMAND} -E sleep 0)")
         """
     ))
 
     with execute_setup_py(tmp_dir, ['build'] + cmake_args, disable_languages_test=True):
         pass
 
     out, _ = capfd.readouterr()
@@ -216,21 +216,21 @@
     out, _ = capsys.readouterr()
 
     assert failed == expected_failed
     if failed:
         if error_code_type == str:
             assert message == "error: package directory " \
                               "'{}' does not exist".format(
-                                    os.path.join(CMAKE_INSTALL_DIR, 'banana'))
+                                    os.path.join(CMAKE_INSTALL_DIR(), 'banana'))
         else:
             assert message.strip().startswith(
                 "setup parameter 'cmake_install_dir' "
                 "is set to an absolute path.")
     else:
-        init_py = to_platform_path("{}/banana/__init__.py".format(CMAKE_INSTALL_DIR))
+        init_py = to_platform_path("{}/banana/__init__.py".format(CMAKE_INSTALL_DIR()))
         assert "copying {}".format(init_py) in out
 
 
 @pytest.mark.parametrize("cmake_with_sdist", [True, False])
 def test_cmake_with_sdist_keyword(cmake_with_sdist, capfd):
     tmp_dir = _tmpdir('cmake_with_sdist')
 
@@ -248,15 +248,15 @@
         """.format(cmake_with_sdist=cmake_with_sdist)
     ))
     tmp_dir.join('CMakeLists.txt').write(textwrap.dedent(
         """
         cmake_minimum_required(VERSION 3.5.0)
         project(test NONE)
         install(CODE "execute_process(
-          COMMAND \${CMAKE_COMMAND} -E sleep 0)")
+          COMMAND \\${CMAKE_COMMAND} -E sleep 0)")
         """
     ))
 
     initialize_git_repo_and_commit(tmp_dir)
 
     with execute_setup_py(tmp_dir, ['sdist'], disable_languages_test=True):
         pass
@@ -286,15 +286,15 @@
         """
     ))
     tmp_dir.join('CMakeLists.txt').write(textwrap.dedent(
         """
         cmake_minimum_required(VERSION 3.5.0)
         project(test NONE)
         install(CODE "execute_process(
-          COMMAND \${CMAKE_COMMAND} -E sleep 0)")
+          COMMAND \\${CMAKE_COMMAND} -E sleep 0)")
         """
     ))
 
     try:
         with execute_setup_py(tmp_dir, ['build'], disable_languages_test=True):
             pass
     except SystemExit as e:
@@ -333,15 +333,15 @@
         """.format(setup_requires=",".join(["'%s'" % package for package in setup_requires]))
     ))
     tmp_dir.join('CMakeLists.txt').write(textwrap.dedent(
         """
         cmake_minimum_required(VERSION 3.5.0)
         project(test NONE)
         install(CODE "execute_process(
-          COMMAND \${CMAKE_COMMAND} -E sleep 0)")
+          COMMAND \\${CMAKE_COMMAND} -E sleep 0)")
         """
     ))
 
     with execute_setup_py(tmp_dir, ['build'], disable_languages_test=True):
         assert mock_setup.call_count == 1
         setup_kw = mock_setup.call_args[1]
         assert setup_kw['setup_requires'] == setup_requires
@@ -409,24 +409,24 @@
                 DESTINATION "."
                 )
             """
         ))
 
         messages = [
             "copying {}/{}.py -> "
-            "{}/setuptools/scripts-".format(CMAKE_INSTALL_DIR, module, SKBUILD_DIR)
+            "{}/setuptools/scripts-".format(CMAKE_INSTALL_DIR(), module, SKBUILD_DIR())
             for module in ['foo', 'bar']]
 
     elif distribution_type == 'pure':
         tmp_dir.join('foo.py').write("# foo.py")
         tmp_dir.join('bar.py').write("# bar.py")
 
         messages = [
             "copying {}.py -> "
-            "{}/setuptools/scripts-".format(module, SKBUILD_DIR)
+            "{}/setuptools/scripts-".format(module, SKBUILD_DIR())
             for module in ['foo', 'bar']]
 
     with execute_setup_py(tmp_dir, ['build'], disable_languages_test=True):
         pass
 
     out, _ = capsys.readouterr()
     for message in messages:
@@ -489,24 +489,24 @@
                 DESTINATION "."
                 )
             """
         ))
 
         messages = [
             "copying {}/{}.py -> "
-            "{}/setuptools/lib".format(CMAKE_INSTALL_DIR, module, SKBUILD_DIR)
+            "{}/setuptools/lib".format(CMAKE_INSTALL_DIR(), module, SKBUILD_DIR())
             for module in ['foo', 'bar']]
 
     elif distribution_type == 'pure':
         tmp_dir.join('foo.py').write("# foo.py")
         tmp_dir.join('bar.py').write("# bar.py")
 
         messages = [
             "copying {}.py -> "
-            "{}/setuptools/lib".format(module, SKBUILD_DIR)
+            "{}/setuptools/lib".format(module, SKBUILD_DIR())
             for module in ['foo', 'bar']]
 
     with execute_setup_py(tmp_dir, ['build'], disable_languages_test=True):
         pass
 
     out, _ = capsys.readouterr()
     for message in messages:
@@ -828,15 +828,15 @@
             expected_packages += ['hybrid.hybrid_2_pure', 'pure']
 
         _pprint('expected_packages', expected_packages)
         _pprint('packages')
 
         # package dir
         expected_package_dir = {
-            package: (os.path.join(CMAKE_INSTALL_DIR,
+            package: (os.path.join(CMAKE_INSTALL_DIR(),
                       package_base,
                       package.replace('.', '/')))
             for package in expected_packages
             }
         _pprint('expected_package_dir', expected_package_dir)
         _pprint('package_dir')
 
@@ -1014,15 +1014,15 @@
     tmp_dir.ensure('fruits/__init__.py')
 
     with execute_setup_py(tmp_dir, ['build'], disable_languages_test=True):
         pass
 
     messages = [
         "copying {}/{} -> "
-        "{}/setuptools/lib".format(CMAKE_INSTALL_DIR, module, SKBUILD_DIR)
+        "{}/setuptools/lib".format(CMAKE_INSTALL_DIR(), module, SKBUILD_DIR())
         for module in [
             'fruits/__init__.py',
             'fruits/apple.py',
             'fruits/banana.py',
             'fruits/data/apple.dat',
             'fruits/data/banana.dat',
         ]]
@@ -1057,15 +1057,15 @@
         """.format(setup_kwarg=setup_kwarg)
     ))
     tmp_dir.join('CMakeLists.txt').write(textwrap.dedent(
         """
         cmake_minimum_required(VERSION 3.5.0)
         project(test NONE)
         install(CODE "execute_process(
-          COMMAND \${CMAKE_COMMAND} -E sleep 0)")
+          COMMAND \\${CMAKE_COMMAND} -E sleep 0)")
         """
     ))
 
     with execute_setup_py(tmp_dir, ['build'], disable_languages_test=True):
         pass
 
     assert mock_setup.call_count == 1
```

### Comparing `scikit-build-0.8.1/tests/test_platform.py` & `scikit-build-0.9.0/tests/test_platform.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/test_distribution.py` & `scikit-build-0.9.0/tests/test_distribution.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/test_issue342_cmake_osx_args_in_setup.py` & `scikit-build-0.9.0/tests/test_issue342_cmake_osx_args_in_setup.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/test_include_exclude_data.py` & `scikit-build-0.9.0/tests/test_include_exclude_data.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/test_skbuild_variable.py` & `scikit-build-0.9.0/tests/test_skbuild_variable.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/test_broken_project.py` & `scikit-build-0.9.0/tests/test_broken_project.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/test_outside_project_root.py` & `scikit-build-0.9.0/tests/test_outside_project_root.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/test_hello_cython.py` & `scikit-build-0.9.0/tests/test_hello_cython.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/test_issue274_support_one_package_without_package_dir.py` & `scikit-build-0.9.0/tests/test_issue274_support_one_package_without_package_dir.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/test_issue352_isolated_environment_support.py` & `scikit-build-0.9.0/tests/test_issue352_isolated_environment_support.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     ))
 
     #
     # mock configure
     #
     def fake_configure(*args, **kwargs):
         # Simulate a successful configuration creating a CMakeCache.txt
-        tmp_dir.ensure(CMAKE_BUILD_DIR, dir=1).join('CMakeCache.txt').write(textwrap.dedent(
+        tmp_dir.ensure(CMAKE_BUILD_DIR(), dir=1).join('CMakeCache.txt').write(textwrap.dedent(
             """
             //Name of generator.
             CMAKE_GENERATOR:INTERNAL=Ninja
             """
         ))
 
     # Skip real configuration creating the CMakeCache.txt expected by
```

### Comparing `scikit-build-0.8.1/tests/test_skbuild.py` & `scikit-build-0.9.0/tests/test_skbuild.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
     @project_setup_py_test("hello-cpp", ["build"])
     def run_build():
         pass
 
     with push_env(CMAKE_GENERATOR=generator):
         tmp_dir = run_build()[0]
-        cmakecache = tmp_dir.join(CMAKE_BUILD_DIR).join("CMakeCache.txt")
+        cmakecache = tmp_dir.join(CMAKE_BUILD_DIR()).join("CMakeCache.txt")
         assert cmakecache.exists()
         variables = get_cmakecache_variables(str(cmakecache))
         make_program = (variables["CMAKE_MAKE_PROGRAM"][1]
                         if "CMAKE_MAKE_PROGRAM" in variables else "")
         assert make_program.endswith(expected_make_program) or \
             make_program.endswith("%s.exe" % expected_make_program)
```

### Comparing `scikit-build-0.8.1/tests/test_manifest_in.py` & `scikit-build-0.9.0/tests/test_manifest_in.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/test_hello_cpp.py` & `scikit-build-0.9.0/tests/test_hello_cpp.py`

 * *Files 14% similar despite different names*

```diff
@@ -103,22 +103,22 @@
     def build_wheel():
         whls = glob.glob('dist/*.whl')
         assert len(whls) == 1
         check_wheel_content(whls[0], expected_distribution_name, expected_content)
         os.remove(whls[0])
         assert not os.path.exists(whls[0])
 
-        assert os.path.exists(os.path.join(CMAKE_BUILD_DIR, "CMakeCache.txt"))
-        os.remove(os.path.join(CMAKE_BUILD_DIR, "CMakeCache.txt"))
+        assert os.path.exists(os.path.join(CMAKE_BUILD_DIR(), "CMakeCache.txt"))
+        os.remove(os.path.join(CMAKE_BUILD_DIR(), "CMakeCache.txt"))
 
     tmp_dir = build_wheel()[0]
 
     @project_setup_py_test("hello-cpp", ["--skip-cmake", "bdist_wheel"], tmp_dir=tmp_dir)
     def build_wheel_skip_cmake():
-        assert not os.path.exists(os.path.join(CMAKE_BUILD_DIR, "CMakeCache.txt"))
+        assert not os.path.exists(os.path.join(CMAKE_BUILD_DIR(), "CMakeCache.txt"))
         whls = glob.glob('dist/*.whl')
         assert len(whls) == 1
         check_wheel_content(whls[0], expected_distribution_name, expected_content)
 
     build_wheel_skip_cmake()
 
 
@@ -130,15 +130,15 @@
 
         @project_setup_py_test("hello-cpp", ["build"])
         def run_build():
             pass
 
         tmp_dir = run_build()[0]
 
-        assert tmp_dir.join(SKBUILD_DIR).exists()
+        assert tmp_dir.join(SKBUILD_DIR()).exists()
 
         # XXX Since using capfd.disabled() context manager prevents
         # the output from being captured atfer it exits, we display
         # a separator allowing to differentiate the build and clean output.
         print("<<-->>")
 
         clean_args = ["clean"]
@@ -148,17 +148,17 @@
         @project_setup_py_test("hello-cpp", clean_args, tmp_dir=tmp_dir)
         def run_clean():
             pass
 
         run_clean()
 
         if not dry_run:
-            assert not tmp_dir.join(SKBUILD_DIR).exists()
+            assert not tmp_dir.join(SKBUILD_DIR()).exists()
         else:
-            assert tmp_dir.join(SKBUILD_DIR).exists()
+            assert tmp_dir.join(SKBUILD_DIR()).exists()
 
         build_out, clean_out = capfd.readouterr()[0].split('<<-->>')
         assert 'Build files have been written to' in build_out
         assert 'Build files have been written to' not in clean_out
 
 
 def test_hello_cleans(capfd):
@@ -186,17 +186,17 @@
     _, clean1_out, clean2_out = \
         capfd.readouterr()[0].split('<<-->>')
 
     clean1_out = clean1_out.strip()
     clean2_out = clean2_out.strip()
 
     assert "running clean" == clean1_out.splitlines()[0]
-    assert "removing '{}'".format(CMAKE_INSTALL_DIR) == clean1_out.splitlines()[1]
-    assert "removing '{}'".format(CMAKE_BUILD_DIR) == clean1_out.splitlines()[2]
-    assert "removing '{}'".format(SKBUILD_DIR) == clean1_out.splitlines()[3]
+    assert "removing '{}'".format(CMAKE_INSTALL_DIR()) == clean1_out.splitlines()[1]
+    assert "removing '{}'".format(CMAKE_BUILD_DIR()) == clean1_out.splitlines()[2]
+    assert "removing '{}'".format(SKBUILD_DIR()) == clean1_out.splitlines()[3]
 
     assert "running clean" == clean2_out
 
 
 @project_setup_py_test("hello-cpp", ["develop"])
 def test_hello_develop():
     for expected_file in [
```

### Comparing `scikit-build-0.8.1/tests/samples/cmakelists-not-in-top-level-dir/hello/_hello.cxx` & `scikit-build-0.9.0/tests/samples/cmakelists-not-in-top-level-dir/hello/_hello.cxx`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/samples/test-include-exclude-data/CMakeLists.txt` & `scikit-build-0.9.0/tests/samples/test-include-exclude-data/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/samples/fail-outside-project-root/CMakeLists.txt` & `scikit-build-0.9.0/tests/samples/fail-outside-project-root/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/samples/test-include-exclude-data-with-base/CMakeLists.txt` & `scikit-build-0.9.0/tests/samples/test-include-exclude-data-with-base/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/samples/fail-hello-with-compile-error/hello/_hello.cxx` & `scikit-build-0.9.0/tests/samples/fail-hello-with-compile-error/hello/_hello.cxx`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/samples/issue-335-support-cmake-source-dir/CMakeLists.txt` & `scikit-build-0.9.0/tests/samples/issue-335-support-cmake-source-dir/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/samples/hello-cpp/CMakeLists.txt` & `scikit-build-0.9.0/tests/samples/hello-cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/samples/hello-cpp/hello/_hello.cxx` & `scikit-build-0.9.0/tests/samples/hello-cpp/hello/_hello.cxx`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/test_utils.py` & `scikit-build-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/test_issue335_support_cmake_source_dir.py` & `scikit-build-0.9.0/tests/test_issue335_support_cmake_source_dir.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/test_issue274_support_default_package_dir.py` & `scikit-build-0.9.0/tests/test_issue274_support_default_package_dir.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/__init__.py` & `scikit-build-0.9.0/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 def _tmpdir(basename):
     """This function returns a temporary directory similar to the one
     returned by the ``tmpdir`` pytest fixture.
     The difference is that the `basetemp` is not configurable using
     the pytest settings."""
 
     # Adapted from _pytest.tmpdir.tmpdir()
-    basename = re.sub("[\W]", "_", basename)
+    basename = re.sub(r"[\W]", "_", basename)
     max_val = 30
     if len(basename) > max_val:
         basename = basename[:max_val]
 
     # Adapted from _pytest.tmpdir.TempdirFactory.getbasetemp()
     try:
         basetemp = _tmpdir._basetemp
@@ -197,14 +197,19 @@
     It yields after changing the current working directory
     to ``project_dir``.
     """
 
     # See https://stackoverflow.com/questions/9160227/dir-util-copy-tree-fails-after-shutil-rmtree
     distutils.dir_util._path_created = {}
 
+    # Clear _PYTHON_HOST_PLATFORM to ensure value sets in skbuild.setuptools_wrap.setup() does not
+    # influence other tests.
+    if '_PYTHON_HOST_PLATFORM' in os.environ:
+        del os.environ['_PYTHON_HOST_PLATFORM']
+
     with push_dir(str(project_dir)), push_argv(["setup.py"] + setup_args), prepend_sys_path([str(project_dir)]):
 
         # Restore master working set that is reset following call to "python setup.py test"
         # See function "project_on_sys_path()" in setuptools.command.test
         pkg_resources._initialize_master_working_set()
 
         with open("setup.py", "r") as fp:
```

### Comparing `scikit-build-0.8.1/tests/test_command_line.py` & `scikit-build-0.9.0/tests/test_command_line.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/tests/test_cmaker.py` & `scikit-build-0.9.0/tests/test_cmaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     with push_dir(str(src_dir)), pytest.raises(SKBuildError) as excinfo:
         CMaker().make()
     assert "Did you forget to run configure before make" in str(excinfo.value)
 
 
 def test_make_without_configure_fails(capfd):
     src_dir = _tmpdir('test_make_without_configure_fails')
-    src_dir.ensure(CMAKE_BUILD_DIR, dir=1)
+    src_dir.ensure(CMAKE_BUILD_DIR(), dir=1)
     with push_dir(str(src_dir)), pytest.raises(SKBuildError) as excinfo:
         CMaker().make()
     _, err = capfd.readouterr()
     assert "An error occurred while building with CMake." in str(excinfo.value)
     assert "Error: could not load cache" in err
 
 
@@ -88,15 +88,15 @@
             file(WRITE "${CMAKE_BINARY_DIR}/foo.txt" "# foo")
             install(FILES "${CMAKE_BINARY_DIR}/foo.txt" DESTINATION ".")
             install(CODE "message(STATUS \\"Project has been installed\\")")
             message(STATUS "CMAKE_SOURCE_DIR:${CMAKE_SOURCE_DIR}")
             message(STATUS "CMAKE_BINARY_DIR:${CMAKE_BINARY_DIR}")
             """
         ))
-        src_dir.ensure(CMAKE_BUILD_DIR, dir=1)
+        src_dir.ensure(CMAKE_BUILD_DIR(), dir=1)
 
         with push_dir(str(src_dir)
                       if not configure_with_cmake_source_dir
                       else str(tmp_dir.ensure('BUILD', dir=1))):
             cmkr = CMaker()
             config_kwargs = {}
             if configure_with_cmake_source_dir:
@@ -105,22 +105,22 @@
             cmkr.make(env=env)
 
         messages = ["Project has been installed"]
 
         if configure_with_cmake_source_dir:
             messages += [
                 "/SRC",
-                "/BUILD/{}".format(to_unix_path(CMAKE_BUILD_DIR)),
-                "/BUILD/{}/./foo.txt".format(to_unix_path(CMAKE_INSTALL_DIR))
+                "/BUILD/{}".format(to_unix_path(CMAKE_BUILD_DIR())),
+                "/BUILD/{}/./foo.txt".format(to_unix_path(CMAKE_INSTALL_DIR()))
             ]
         else:
             messages += [
                 "/SRC",
-                "/SRC/{}".format(to_unix_path(CMAKE_BUILD_DIR)),
-                "/SRC/{}/./foo.txt".format(to_unix_path(CMAKE_INSTALL_DIR)),
+                "/SRC/{}".format(to_unix_path(CMAKE_BUILD_DIR())),
+                "/SRC/{}/./foo.txt".format(to_unix_path(CMAKE_INSTALL_DIR())),
             ]
 
         out, _ = capfd.readouterr()
         for message in messages:
             assert message in out
```

### Comparing `scikit-build-0.8.1/tests/test_hello_pure.py` & `scikit-build-0.9.0/tests/test_hello_pure.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,19 +77,19 @@
 
         @project_setup_py_test("hello-pure", ["build"], disable_languages_test=True)
         def run_build():
             pass
 
         tmp_dir = run_build()[0]
 
-        assert tmp_dir.join(SKBUILD_DIR).exists()
+        assert tmp_dir.join(SKBUILD_DIR()).exists()
 
         @project_setup_py_test("hello-pure", ["clean"], tmp_dir=tmp_dir, disable_languages_test=True)
         def run_clean():
             pass
 
         run_clean()
 
-        assert not tmp_dir.join(SKBUILD_DIR).exists()
+        assert not tmp_dir.join(SKBUILD_DIR()).exists()
 
         out = capfd.readouterr()[0]
         assert 'Build files have been written to' not in out
```

### Comparing `scikit-build-0.8.1/skbuild/setuptools_wrap.py` & `scikit-build-0.9.0/skbuild/setuptools_wrap.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,21 +33,23 @@
 except ImportError:
     from .compat import which
 
 from setuptools import setup as upstream_setup
 from setuptools.dist import Distribution as upstream_Distribution
 
 from . import cmaker
-from .command import (build, build_py, clean,
+from .command import (build, build_ext, build_py, clean,
                       install, install_lib, install_scripts,
                       bdist, bdist_wheel, egg_info,
                       sdist, generate_source_manifest, test)
 from .constants import (CMAKE_DEFAULT_EXECUTABLE,
                         CMAKE_INSTALL_DIR,
-                        CMAKE_SPEC_FILE)
+                        CMAKE_SPEC_FILE,
+                        set_skbuild_plat_name,
+                        skbuild_plat_name)
 from .exceptions import SKBuildError, SKBuildGeneratorNotFoundError
 from .utils import (mkdir_p, parse_manifestin, PythonModuleFinder, to_platform_path, to_unix_path)
 
 
 def create_skbuild_argparser():
     """Create and return a scikit-build argument parser.
     """
@@ -137,30 +139,31 @@
         out[1] = out[1].getvalue()
 
 
 def _parse_setuptools_arguments(setup_attrs):
     """This function instantiates a Distribution object and
     parses the command line arguments.
 
-    It returns the tuple
-        ``(display_only, help_commands, commands,
-        hide_listing, force_cmake, skip_cmake, plat_name)``
+    It returns the tuple ``(display_only, help_commands, commands, hide_listing, force_cmake, skip_cmake, plat_name)``
     where
+
     - display_only is a boolean indicating if an argument like '--help',
       '--help-commands' or '--author' was passed.
     - help_commands is a boolean indicating if argument '--help-commands'
       was passed.
     - commands contains the list of commands that were passed.
     - hide_listing is a boolean indicating if the list of files being included
       in the distribution is displayed or not.
     - force_cmake a boolean indicating that CMake should always be executed.
     - skip_cmake is a boolean indicating if the execution of CMake should
       explicitly be skipped.
     - plat_name is a string identifying the platform name to embed in generated
       filenames. It defaults to ``distutils.util.get_platform()``.
+    - build_ext_inplace is a boolean indicating if ``build_ext`` command was
+      specified along with the --inplace argument.
 
     Otherwise it raises DistutilsArgError exception if there are
     any error on the command-line, and it raises DistutilsGetoptError
     if there any error in the command 'options' attribute.
 
     The code has been adapted from the setup() function available
     in distutils/core.py.
@@ -212,17 +215,19 @@
     if not plat_names:
         plat_names.add(None)
     elif len(plat_names) > 1:
         raise SKBuildError(
             "--plat-name is ambiguous: %s" % ", ".join(plat_names))
     plat_name = list(plat_names)[0]
 
+    build_ext_inplace = dist.get_command_obj('build_ext').inplace
+
     return (display_only, dist.help_commands, dist.commands,
             dist.hide_listing, dist.force_cmake, dist.skip_cmake,
-            plat_name)
+            plat_name, build_ext_inplace)
 
 
 def _check_skbuild_parameters(skbuild_kw):
     cmake_install_dir = skbuild_kw['cmake_install_dir']
     if os.path.isabs(cmake_install_dir):
         raise SKBuildError((
             "\n  setup parameter 'cmake_install_dir' is set to "
@@ -291,14 +296,15 @@
 
 
 def _should_run_cmake(commands, cmake_with_sdist):
     """Return True if at least one command requiring ``cmake`` to run
     is found in ``commands``."""
     for expected_command in [
         "build",
+        "build_ext",
         "develop",
         "install",
         "install_lib",
         "bdist",
         "bdist_dumb",
         "bdist_egg"
         "bdist_rpm",
@@ -313,49 +319,50 @@
     return False
 
 
 def _save_cmake_spec(args):
     """Save the CMake spec to disk"""
     # We use JSON here because readability is more important than performance
     try:
-        os.makedirs(os.path.dirname(CMAKE_SPEC_FILE))
+        os.makedirs(os.path.dirname(CMAKE_SPEC_FILE()))
     except OSError:
         pass
 
-    with open(CMAKE_SPEC_FILE, 'w+') as fp:
+    with open(CMAKE_SPEC_FILE(), 'w+') as fp:
         json.dump(args, fp)
 
 
 def _load_cmake_spec():
     """Load and return the CMake spec from disk"""
     try:
-        with open(CMAKE_SPEC_FILE) as fp:
+        with open(CMAKE_SPEC_FILE()) as fp:
             return json.load(fp)
     except (OSError, IOError, ValueError):
         return None
 
 
 # pylint:disable=too-many-locals, too-many-branches
 def setup(*args, **kw):  # noqa: C901
     """This function wraps setup() so that we can run cmake, make,
     CMake build, then proceed as usual with setuptools, appending the
     CMake-generated output as necessary.
 
     The CMake project is re-configured only if needed. This is achieved by (1) retrieving the environment mapping
     associated with the generator set in the ``CMakeCache.txt`` file, (2) saving the CMake configure arguments and
-    version in :const:`skbuild.constants.CMAKE_SPEC_FILE`: and (3) re-configuring only if either the generator or
+    version in :func:`skbuild.constants.CMAKE_SPEC_FILE()`: and (3) re-configuring only if either the generator or
     the CMake specs change.
     """
     sys.argv, cmake_executable, skip_generator_test, cmake_args, make_args = parse_args()
 
     # work around https://bugs.python.org/issue1011113
     # (patches provided, but no updates since 2014)
     cmdclass = kw.get('cmdclass', {})
     cmdclass['build'] = cmdclass.get('build', build.build)
     cmdclass['build_py'] = cmdclass.get('build_py', build_py.build_py)
+    cmdclass['build_ext'] = cmdclass.get('build_ext', build_ext.build_ext)
     cmdclass['install'] = cmdclass.get('install', install.install)
     cmdclass['install_lib'] = cmdclass.get('install_lib',
                                            install_lib.install_lib)
     cmdclass['install_scripts'] = cmdclass.get('install_scripts',
                                                install_scripts.install_scripts)
     cmdclass['clean'] = cmdclass.get('clean', clean.clean)
     cmdclass['sdist'] = cmdclass.get('sdist', sdist.sdist)
@@ -410,15 +417,15 @@
     # * no CMakeLists.txt if found
     display_only = has_invalid_arguments = help_commands = False
     force_cmake = skip_cmake = False
     commands = []
     try:
         (display_only, help_commands, commands,
          hide_listing, force_cmake, skip_cmake,
-         plat_name) = \
+         plat_name, build_ext_inplace) = \
             _parse_setuptools_arguments(kw)
     except (DistutilsArgError, DistutilsGetoptError):
         has_invalid_arguments = True
 
     has_cmakelists = os.path.exists(
         os.path.join(cmake_source_dir, "CMakeLists.txt"))
     if not has_cmakelists:
@@ -444,15 +451,15 @@
             print('Arguments following a "--" are passed directly to CMake '
                   '(e.g. -DMY_VAR:BOOL=TRUE).')
             print('Arguments following a second "--" are passed directly to '
                   ' the build tool.')
             print('')
         return upstream_setup(*args, **kw)
 
-    developer_mode = "develop" in commands or "test" in commands
+    developer_mode = "develop" in commands or "test" in commands or build_ext_inplace
 
     packages = kw.get('packages', [])
     package_dir = kw.get('package_dir', {})
     package_data = copy.deepcopy(kw.get('package_data', {}))
 
     py_modules = kw.get('py_modules', [])
     new_py_modules = {py_module: False for py_module in py_modules}
@@ -466,22 +473,42 @@
     }
 
     # Since CMake arguments provided through the command line have more
     # weight and when CMake is given multiple times a argument, only the last
     # one is considered, let's prepend the one provided in the setup call.
     cmake_args = skbuild_kw['cmake_args'] + cmake_args
 
-    # Set CMAKE_OSX_DEPLOYMENT_TARGET and CMAKE_OSX_ARCHITECTURES if not already
-    # specified
     if sys.platform == 'darwin':
+        # Set plat-name based on CMAKE_OSX_* arguments
         if plat_name is None:
-            # The following code is duplicated in bdist_wheel.finalize_options()
-            plat_name = "macosx-10.6-x86_64"
+            # These default values are duplicated in bdist_wheel.finalize_options()
+            version = '10.6'
+            machine = 'x86_64'
+        else:
+            (_, version, machine) = plat_name.split('-')
 
-        (_, version, machine) = plat_name.split('-')
+        # The loop here allows for CMAKE_OSX_* command line arguments to overload
+        # values passed with either the ``--plat-name`` command-line argument
+        # or the ``cmake_args`` setup option.
+        for cmake_arg in cmake_args:
+            if 'CMAKE_OSX_DEPLOYMENT_TARGET' in cmake_arg:
+                version = cmake_arg.split('=')[1]
+            if 'CMAKE_OSX_ARCHITECTURES' in cmake_arg:
+                machine = cmake_arg.split('=')[1]
+
+        set_skbuild_plat_name("macosx-{}-{}".format(version, machine))
+
+        # Set platform env. variable so that commands (e.g. bdist_wheel)
+        # uses this information. The _PYTHON_HOST_PLATFORM env. variable is
+        # used in distutils.util.get_platform() function.
+        os.environ['_PYTHON_HOST_PLATFORM'] = skbuild_plat_name()
+
+        # Set CMAKE_OSX_DEPLOYMENT_TARGET and CMAKE_OSX_ARCHITECTURES if not already
+        # specified
+        (_, version, machine) = skbuild_plat_name().split('-')
         if not cmaker.has_cmake_cache_arg(
                 cmake_args, 'CMAKE_OSX_DEPLOYMENT_TARGET'):
             cmake_args.append(
                 '-DCMAKE_OSX_DEPLOYMENT_TARGET:STRING=%s' % version
             )
         if not cmaker.has_cmake_cache_arg(
                 cmake_args, 'CMAKE_OSX_ARCHITECTURES'):
@@ -581,50 +608,52 @@
     if kw.get("include_package_data", False):
         original_manifestin_data_files = parse_manifestin(os.path.join(os.getcwd(), "MANIFEST.in"))
         for path in original_manifestin_data_files:
             _classify_file(path, package_data, package_prefixes,
                            py_modules, new_py_modules,
                            scripts, new_scripts,
                            data_files)
+
     if developer_mode:
         # Copy packages
         for package, package_file_list in package_data.items():
             for package_file in package_file_list:
                 package_file = os.path.join(package_dir[package], package_file)
-                cmake_file = os.path.join(CMAKE_INSTALL_DIR, package_file)
+                cmake_file = os.path.join(CMAKE_INSTALL_DIR(), package_file)
                 if os.path.exists(cmake_file):
                     _copy_file(cmake_file, package_file, hide_listing)
+
         # Copy modules
         for py_module in py_modules:
             package_file = py_module + ".py"
-            cmake_file = os.path.join(CMAKE_INSTALL_DIR, package_file)
+            cmake_file = os.path.join(CMAKE_INSTALL_DIR(), package_file)
             if os.path.exists(cmake_file):
                 _copy_file(cmake_file, package_file, hide_listing)
     else:
         _consolidate_package_modules(
             cmake_source_dir, packages, package_dir, py_modules, package_data, hide_listing)
 
         original_package_data = kw.get('package_data', {}).copy()
         _consolidate_package_data_files(original_package_data, package_prefixes, hide_listing)
 
         for data_file in original_manifestin_data_files:
-            dest_data_file = os.path.join(CMAKE_INSTALL_DIR, data_file)
+            dest_data_file = os.path.join(CMAKE_INSTALL_DIR(), data_file)
             _copy_file(data_file, dest_data_file, hide_listing)
 
     kw['package_data'] = package_data
     kw['package_dir'] = {
         package: (
-            os.path.join(CMAKE_INSTALL_DIR, prefix)
-            if os.path.exists(os.path.join(CMAKE_INSTALL_DIR, prefix))
+            os.path.join(CMAKE_INSTALL_DIR(), prefix)
+            if os.path.exists(os.path.join(CMAKE_INSTALL_DIR(), prefix))
             else prefix)
         for prefix, package in package_prefixes
     }
 
     kw['scripts'] = [
-        os.path.join(CMAKE_INSTALL_DIR, script) if mask else script
+        os.path.join(CMAKE_INSTALL_DIR(), script) if mask else script
         for script, mask in new_scripts.items()
     ]
 
     kw['data_files'] = [
         (parent_dir, list(file_set))
         for parent_dir, file_set in data_files.items()
     ]
@@ -655,23 +684,25 @@
     matched with their immediate parent package, instead of any of that
     package's ancestors.
 
     For example, consider the project structure below.  Assume that the
     setup call was made with a package list featuring "top" and "top.bar", but
     not "top.not_a_subpackage".
 
-    top/                -> top/
-      __init__.py       -> top/__init__.py                 (parent: top)
-      foo.py            -> top/foo.py                      (parent: top)
-      bar/              -> top/bar/                        (parent: top)
-        __init__.py     -> top/bar/__init__.py             (parent: top.bar)
-
-      not_a_subpackage/ -> top/not_a_subpackage/           (parent: top)
-        data_0.txt      -> top/not_a_subpackage/data_0.txt (parent: top)
-        data_1.txt      -> top/not_a_subpackage/data_1.txt (parent: top)
+    ::
+
+        top/                -> top/
+          __init__.py       -> top/__init__.py                 (parent: top)
+          foo.py            -> top/foo.py                      (parent: top)
+          bar/              -> top/bar/                        (parent: top)
+            __init__.py     -> top/bar/__init__.py             (parent: top.bar)
+
+          not_a_subpackage/ -> top/not_a_subpackage/           (parent: top)
+            data_0.txt      -> top/not_a_subpackage/data_0.txt (parent: top)
+            data_1.txt      -> top/not_a_subpackage/data_1.txt (parent: top)
 
     The paths in the generated install manifest are matched to packages
     according to the parents indicated on the right.  Only packages that are
     specified in the setup() call are considered.  Because of the sort order,
     the data files on the bottom would have been mapped to
     "top.not_a_subpackage" instead of "top", proper -- had such a package been
     specified.
@@ -690,27 +721,27 @@
                               py_modules, new_py_modules,
                               scripts, new_scripts,
                               data_files,
                               cmake_source_dir, cmake_install_dir):
     assert not os.path.isabs(cmake_source_dir)
     assert cmake_source_dir != "."
 
-    install_root = os.path.join(os.getcwd(), CMAKE_INSTALL_DIR)
+    install_root = os.path.join(os.getcwd(), CMAKE_INSTALL_DIR())
     for path in install_paths:
         # if this installed file is not within the project root, complain and
         # exit
-        if not to_platform_path(path).startswith(CMAKE_INSTALL_DIR):
+        if not to_platform_path(path).startswith(CMAKE_INSTALL_DIR()):
             raise SKBuildError((
                 "\n  CMake-installed files must be within the project root.\n"
                 "    Project Root  : {}\n"
                 "    Violating File: {}\n").format(
                     install_root, to_platform_path(path)))
 
         # peel off the 'skbuild' prefix
-        path = to_unix_path(os.path.relpath(path, CMAKE_INSTALL_DIR))
+        path = to_unix_path(os.path.relpath(path, CMAKE_INSTALL_DIR()))
 
         _classify_file(path, package_data, package_prefixes,
                        py_modules, new_py_modules,
                        scripts, new_scripts,
                        data_files)
 
 
@@ -770,15 +801,15 @@
     # not part of a package, not a module, nor a script.  Without any other
     # information, we can only treat it as a generic data file.
     parent_dir = os.path.dirname(path)
     file_set = data_files.get(parent_dir)
     if file_set is None:
         file_set = set()
         data_files[parent_dir] = file_set
-    file_set.add(os.path.join(CMAKE_INSTALL_DIR, path))
+    file_set.add(os.path.join(CMAKE_INSTALL_DIR(), path))
 
 
 def _copy_file(src_file, dest_file, hide_listing=True):
     """Copy ``src_file`` to ``dest_file`` ensuring parent directory exists.
 
     By default, message like `creating directory /path/to/package` and
     `copying directory /src/path/to/package -> path/to/package` are displayed
@@ -803,40 +834,40 @@
         cmake_source_dir, packages, package_dir, py_modules, package_data,
         hide_listing
 ):
     """This function consolidates packages having modules located in
     both the source tree and the CMake install tree into one location.
 
     The one location is the CMake install tree
-    (see data::`.constants.CMAKE_INSTALL_DIR`).
+    (see :func:`.constants.CMAKE_INSTALL_DIR()`).
 
     Why ? This is a necessary evil because ``Setuptools`` keeps track of
     packages and modules files to install using a dictionary of lists where
     the key are package names (e.g ``foo.bar``) and the values are lists of
     module files (e.g ``['__init__.py', 'baz.py']``. Since this doesn't allow
     to "split" files associated with a given module in multiple location, one
     location is selected, and files are copied over.
 
     How? It currently searches for modules across both locations using
     the :class:`.utils.PythonModuleFinder`. then with the help
     of :func:`_package_data_contain_module`, it identifies which
     one are either already included or missing from the distribution.
 
     Once a module has been identified as ``missing``, it is both copied
-    into the data::`.constants.CMAKE_INSTALL_DIR` and added to the
+    into the :func:`.constants.CMAKE_INSTALL_DIR()` and added to the
     ``package_data`` dictionary so that it can be considered by
     the upstream setup function.
     """
 
     try:
         # Search for python modules in both the current directory
         # and cmake install tree.
         modules = PythonModuleFinder(
             packages, package_dir, py_modules,
-            alternative_build_base=CMAKE_INSTALL_DIR
+            alternative_build_base=CMAKE_INSTALL_DIR()
         ).find_all_modules()
     except DistutilsError as msg:
         raise SystemExit("error: {}".format(str(msg)))
 
     print("")
 
     for entry in modules:
@@ -845,15 +876,15 @@
         if _package_data_contain_module(entry, package_data):
             continue
 
         (package, _, src_module_file) = entry
 
         # Copy missing module file
         if os.path.exists(src_module_file):
-            dest_module_file = os.path.join(CMAKE_INSTALL_DIR, src_module_file)
+            dest_module_file = os.path.join(CMAKE_INSTALL_DIR(), src_module_file)
             _copy_file(src_module_file, dest_module_file, hide_listing)
 
         # Since the mapping in package_data expects the package to be associated
         # with a list of files relative to the directory containing the package,
         # the following section makes sure to strip the redundant part of the
         # module file path.
         # The redundant part should be stripped for both cmake_source_dir and
@@ -870,35 +901,35 @@
             package_data[package].append(stripped_module_file)
         except KeyError:
             package_data[package] = [stripped_module_file]
 
 
 def _consolidate_package_data_files(original_package_data, package_prefixes, hide_listing):
     """This function copies package data files specified using the ``package_data`` keyword
-    into data::`.constants.CMAKE_INSTALL_DIR`.
+    into :func:`.constants.CMAKE_INSTALL_DIR()`.
 
     ::
 
         setup(...,
             packages=['mypkg'],
             package_dir={'mypkg': 'src/mypkg'},
             package_data={'mypkg': ['data/*.dat']},
             )
 
     Considering that (1) the packages associated with modules located in both the source tree and
     the CMake install tree are consolidated into the CMake install tree, and (2) the consolidated
     package path set in the ``package_dir`` dictionary and later used by setuptools to package
-    (or install) modules and data files is data::`.constants.CMAKE_INSTALL_DIR`, copying the data files
+    (or install) modules and data files is :func:`.constants.CMAKE_INSTALL_DIR()`, copying the data files
     is required to ensure setuptools can find them when it uses the package directory.
     """
     project_root = os.getcwd()
     for prefix, package in package_prefixes:
         if package not in original_package_data:
             continue
         raw_patterns = original_package_data[package]
         for pattern in raw_patterns:
             expanded_package_dir = os.path.join(project_root, prefix, pattern)
             for src_data_file in glob(expanded_package_dir):
                 full_prefix_length = len(os.path.join(project_root, prefix)) + 1
                 data_file = src_data_file[full_prefix_length:]
-                dest_data_file = os.path.join(CMAKE_INSTALL_DIR, prefix, data_file)
+                dest_data_file = os.path.join(CMAKE_INSTALL_DIR(), prefix, data_file)
                 _copy_file(src_data_file, dest_data_file, hide_listing)
```

### Comparing `scikit-build-0.8.1/skbuild/platform_specifics/platform_factory.py` & `scikit-build-0.9.0/skbuild/platform_specifics/platform_factory.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/skbuild/platform_specifics/osx.py` & `scikit-build-0.9.0/skbuild/platform_specifics/osx.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/skbuild/platform_specifics/linux.py` & `scikit-build-0.9.0/skbuild/platform_specifics/linux.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/skbuild/platform_specifics/abstract.py` & `scikit-build-0.9.0/skbuild/platform_specifics/abstract.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/skbuild/platform_specifics/windows.py` & `scikit-build-0.9.0/skbuild/platform_specifics/windows.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/skbuild/command/generate_source_manifest.py` & `scikit-build-0.9.0/skbuild/command/generate_source_manifest.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 import os
 import subprocess
 import sys
 
 from distutils.cmd import Command
 
 from . import set_build_base_mixin
-from ..constants import SKBUILD_DIR
+from ..constants import SKBUILD_DIR, SKBUILD_MARKER_FILE
 from ..utils import new_style
 
-SKBUILD_MARKER_FILE = os.path.join(SKBUILD_DIR, "_skbuild_MANIFEST")
-
 
 class generate_source_manifest(set_build_base_mixin, new_style(Command)):
     """Custom setuptools command generating a `MANIFEST` file if
     not already provided."""
 
     description = "generate source MANIFEST"
 
@@ -41,15 +39,15 @@
             # with the project's manifest.
             not os.path.exists('MANIFEST.in')
 
             # otherwise, we check to see that there is no MANIFEST, ...
             and not os.path.exists('MANIFEST')  # ... or ...
 
             # ... (if there is one,) that we created it
-            or os.path.exists(SKBUILD_MARKER_FILE)
+            or os.path.exists(SKBUILD_MARKER_FILE())
         )
 
         if do_generate:
 
             try:
                 with open('MANIFEST', 'wb') as manifest_file:
                     # Since Git < 2.11 does not support --recurse-submodules option, fallback to
@@ -70,16 +68,16 @@
                     'automatically, but could not because it could not '
                     'determine which source files to include.\n\n'
                     'The command used was "git ls-files"\n'
                     '\n\n'
                 )
                 raise
 
-            if not os.path.exists(SKBUILD_DIR):
-                os.makedirs(SKBUILD_DIR)
+            if not os.path.exists(SKBUILD_DIR()):
+                os.makedirs(SKBUILD_DIR())
 
-            with open(SKBUILD_MARKER_FILE, 'w'):  # touch
+            with open(SKBUILD_MARKER_FILE(), 'w'):  # touch
                 pass
 
     def finalize_options(self, *args, **kwargs):
         """Set final values for all the options that this command supports."""
         pass
```

### Comparing `scikit-build-0.8.1/skbuild/command/build_py.py` & `scikit-build-0.9.0/skbuild/command/build_py.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,16 +86,16 @@
             # XXX perhaps we should also check for just .pyc files
             # (so greedy closed-source bastards can distribute Python
             # modules too)
             module_file = os.path.join(package_dir, module_base + ".py")
 
             # skbuild: prepend CMAKE_INSTALL_DIR if file exists in the
             # CMake install tree.
-            if os.path.exists(os.path.join(CMAKE_INSTALL_DIR, module_file)):
-                module_file = os.path.join(CMAKE_INSTALL_DIR, module_file)
+            if os.path.exists(os.path.join(CMAKE_INSTALL_DIR(), module_file)):
+                module_file = os.path.join(CMAKE_INSTALL_DIR(), module_file)
 
             if not self.check_module(module, module_file):
                 continue
 
             modules.append((package, module_base, module_file))
 
         return modules
```

### Comparing `scikit-build-0.8.1/skbuild/command/install.py` & `scikit-build-0.9.0/skbuild/command/install.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/skbuild/command/bdist_wheel.py` & `scikit-build-0.9.0/skbuild/command/bdist_wheel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module defines custom implementation of ``bdist_wheel`` setuptools
 command."""
 
+import os
 import sys
 
 try:
     from wheel.wheelfile import WheelFile
     _USE_WHEELFILE = True
 except ImportError:
     from wheel import archive as _wheel_archive  # Not available with wheel >= 0.32.0
@@ -56,20 +57,20 @@
 
             try:
                 super(bdist_wheel, self).run(*args, **kwargs)
             finally:
                 _wheel_archive.make_wheelfile_inner = old_make_wheelfile_inner
 
     def finalize_options(self, *args, **kwargs):
-        """Ensure MacOSX wheels include ``x86_64`` instead of ``intel``."""
+        """Ensure MacOSX wheels include the expected platform information."""
         # pylint:disable=attribute-defined-outside-init,access-member-before-definition
         if sys.platform == 'darwin' and self.plat_name is None and self.distribution.has_ext_modules():
-            # The following code is duplicated in setuptools_wrap
+            # The default value is duplicated in setuptools_wrap
             # pylint:disable=access-member-before-definition
-            self.plat_name = "macosx-10.6-x86_64"
+            self.plat_name = os.environ.get('_PYTHON_HOST_PLATFORM', 'macosx-10.6-x86_64')
         super(bdist_wheel, self).finalize_options(*args, **kwargs)
 
     def write_wheelfile(self, wheelfile_base, _=None):
         """Write ``skbuild <version>`` as a wheel generator.
         See `PEP-0427 <https://www.python.org/dev/peps/pep-0427/#file-contents>`_ for more details.
         """
         from .. import __version__ as skbuild_version
```

### Comparing `scikit-build-0.8.1/skbuild/command/clean.py` & `scikit-build-0.9.0/skbuild/command/clean.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,14 @@
 
 class clean(set_build_base_mixin, new_style(_clean)):
     """Custom implementation of ``clean`` setuptools command."""
     def run(self):
         """After calling the super class implementation, this function removes
         the directories specific to scikit-build."""
         super(clean, self).run()
-        for dir_ in (CMAKE_INSTALL_DIR,
-                     CMAKE_BUILD_DIR,
-                     SKBUILD_DIR):
+        for dir_ in (CMAKE_INSTALL_DIR(),
+                     CMAKE_BUILD_DIR(),
+                     SKBUILD_DIR()):
             if os.path.exists(dir_):
                 log.info("removing '%s'", dir_)
             if not self.dry_run and os.path.exists(dir_):
                 rmtree(dir_)
```

### Comparing `scikit-build-0.8.1/skbuild/command/install_lib.py` & `scikit-build-0.9.0/skbuild/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/skbuild/command/sdist.py` & `scikit-build-0.9.0/skbuild/command/sdist.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/skbuild/command/__init__.py` & `scikit-build-0.9.0/skbuild/command/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,12 +9,12 @@
     """Mixin allowing to override distutils and setuptools commands.
     """
     def finalize_options(self, *args, **kwargs):
         """Override built-in function and set a new `build_base`.
         """
         try:
             if not self.build_base or self.build_base == 'build':
-                self.build_base = cmaker.SETUPTOOLS_INSTALL_DIR
+                self.build_base = cmaker.SETUPTOOLS_INSTALL_DIR()
         except AttributeError:
             pass
 
         super(set_build_base_mixin, self).finalize_options(*args, **kwargs)
```

### Comparing `scikit-build-0.8.1/skbuild/command/egg_info.py` & `scikit-build-0.9.0/skbuild/command/egg_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             if self.distribution.package_dir is not None and len(self.distribution.package_dir) == 1:
                 # Recover directory specified in setup() function
                 # using `package_dir={'':<egg_base>}`
                 # This is required to successfully update the python path when
                 # running the test command.
                 package_name = list(self.distribution.package_dir.keys())[0]
                 egg_base = to_unix_path(list(self.distribution.package_dir.values())[0])
-                cmake_install_dir = to_unix_path(CMAKE_INSTALL_DIR)
+                cmake_install_dir = to_unix_path(CMAKE_INSTALL_DIR())
                 if egg_base.startswith(cmake_install_dir):
                     egg_base = egg_base[len(cmake_install_dir) + 1:]
                 if package_name and egg_base.endswith(package_name):
                     egg_base = egg_base[:-len(package_name) - 1]
                 if egg_base == "":
                     egg_base = "."
                 # pylint:disable=attribute-defined-outside-init
```

### Comparing `scikit-build-0.8.1/skbuild/command/install_scripts.py` & `scikit-build-0.9.0/skbuild/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/skbuild/cmaker.py` & `scikit-build-0.9.0/skbuild/cmaker.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,20 +91,20 @@
 
     def __init__(self, cmake_executable=CMAKE_DEFAULT_EXECUTABLE):
         self.cmake_executable = cmake_executable
         self.cmake_version = get_cmake_version(self.cmake_executable)
         self.platform = get_platform()
 
     def get_cached_generator_name(self):
-        """Reads and returns the cached generator from the :const:`skbuild.constants.CMAKE_BUILD_DIR`:.
+        """Reads and returns the cached generator from the :func:`skbuild.constants.CMAKE_BUILD_DIR()`:.
         Returns None if not found.
         """
         try:
             cmake_generator = 'CMAKE_GENERATOR:INTERNAL='
-            with open(os.path.join(CMAKE_BUILD_DIR, 'CMakeCache.txt')) as fp:
+            with open(os.path.join(CMAKE_BUILD_DIR(), 'CMakeCache.txt')) as fp:
                 for line in fp:
                     if line.startswith(cmake_generator):
                         return line[len(cmake_generator):].strip()
         except (OSError, IOError):
             pass
 
         return None
@@ -136,15 +136,15 @@
             is skipped.
 
         cmake_source_dir: string
             Path to source tree containing a ``CMakeLists.txt``
 
         cmake_install_dir: string
             Relative directory to append
-            to :const:`skbuild.constants.CMAKE_INSTALL_DIR`.
+            to :func:`skbuild.constants.CMAKE_INSTALL_DIR()`.
 
         languages: tuple
             List of languages required to configure the project and expected to
             be supported by the compiler. The language identifier that can be specified
             in the list corresponds to the one recognized by CMake.
 
         cleanup: bool
@@ -170,33 +170,33 @@
         # use the generator returned from the platform, with the current
         # generator_name as a suggestion
         generator = self.platform.get_best_generator(
             generator_name, skip_generator_test=skip_generator_test,
             cmake_executable=self.cmake_executable, cmake_args=clargs,
             languages=languages, cleanup=cleanup)
 
-        if not os.path.exists(CMAKE_BUILD_DIR):
-            os.makedirs(CMAKE_BUILD_DIR)
+        if not os.path.exists(CMAKE_BUILD_DIR()):
+            os.makedirs(CMAKE_BUILD_DIR())
 
-        if not os.path.exists(CMAKE_INSTALL_DIR):
-            os.makedirs(CMAKE_INSTALL_DIR)
+        if not os.path.exists(CMAKE_INSTALL_DIR()):
+            os.makedirs(CMAKE_INSTALL_DIR())
 
-        if not os.path.exists(SETUPTOOLS_INSTALL_DIR):
-            os.makedirs(SETUPTOOLS_INSTALL_DIR)
+        if not os.path.exists(SETUPTOOLS_INSTALL_DIR()):
+            os.makedirs(SETUPTOOLS_INSTALL_DIR())
 
         python_version = CMaker.get_python_version()
         python_include_dir = CMaker.get_python_include_dir(python_version)
         python_library = CMaker.get_python_library(python_version)
 
         cmake_source_dir = os.path.abspath(cmake_source_dir)
         cmd = [
             self.cmake_executable, cmake_source_dir, '-G', generator.name,
             ("-DCMAKE_INSTALL_PREFIX:PATH=" +
                 os.path.abspath(
-                    os.path.join(CMAKE_INSTALL_DIR, cmake_install_dir))),
+                    os.path.join(CMAKE_INSTALL_DIR(), cmake_install_dir))),
             ("-DPYTHON_EXECUTABLE:FILEPATH=" +
                 sys.executable),
             ("-DPYTHON_VERSION_STRING:STRING=" +
                 sys.version.split(' ')[0]),
             ("-DPYTHON_INCLUDE_DIR:PATH=" +
                 python_include_dir),
             ("-DPYTHON_LIBRARY:FILEPATH=" +
@@ -212,28 +212,28 @@
         cmd.extend(
             filter(bool,
                    shlex.split(os.environ.get("SKBUILD_CONFIGURE_OPTIONS", "")))
         )
 
         # changes dir to cmake_build and calls cmake's configure step
         # to generate makefile
-        rtn = subprocess.call(cmd, cwd=CMAKE_BUILD_DIR, env=generator.env)
+        rtn = subprocess.call(cmd, cwd=CMAKE_BUILD_DIR(), env=generator.env)
         if rtn != 0:
             raise SKBuildError(
                 "An error occurred while configuring with CMake.\n"
                 "  Command:\n"
                 "    {}\n"
                 "  Source directory:\n"
                 "    {}\n"
                 "  Working directory:\n"
                 "    {}\n"
                 "Please see CMake's output for more information.".format(
                     self._formatArgsForDisplay(cmd),
                     os.path.abspath(cmake_source_dir),
-                    os.path.abspath(CMAKE_BUILD_DIR)))
+                    os.path.abspath(CMAKE_BUILD_DIR())))
 
         CMaker.check_for_bad_installs()
 
         return generator.env
 
     @staticmethod
     def get_python_version():
@@ -404,24 +404,24 @@
     @staticmethod
     def check_for_bad_installs():
         """This function tries to catch files that are meant to be installed
         outside the project root before they are actually installed.
 
         Indeed, we can not wait for the manifest, so we try to extract the
         information (install destination) from the CMake build files
-        ``*.cmake`` found in :const:`skbuild.constants.CMAKE_BUILD_DIR`.
+        ``*.cmake`` found in :func:`skbuild.constants.CMAKE_BUILD_DIR()`.
 
         It raises :class:`skbuild.exceptions.SKBuildError` if it found install destination outside of
-        :const:`skbuild.constants.CMAKE_INSTALL_DIR`.
+        :func:`skbuild.constants.CMAKE_INSTALL_DIR()`.
         """
 
         bad_installs = []
-        install_dir = os.path.join(os.getcwd(), CMAKE_INSTALL_DIR)
+        install_dir = os.path.join(os.getcwd(), CMAKE_INSTALL_DIR())
 
-        for root, _, file_list in os.walk(CMAKE_BUILD_DIR):
+        for root, _, file_list in os.walk(CMAKE_BUILD_DIR()):
             for filename in file_list:
                 if os.path.splitext(filename)[1] != ".cmake":
                     continue
 
                 for line in io.open(os.path.join(root, filename), encoding="utf-8"):
                     match = RE_FILE_INSTALL.match(line)
                     if match is None:
@@ -449,51 +449,51 @@
                     ("      " + _install) for _install in bad_installs)
             )))
 
     def make(self, clargs=(), config="Release", source_dir=".", env=None):
         """Calls the system-specific make program to compile code.
         """
         clargs, config = pop_arg('--config', clargs, config)
-        if not os.path.exists(CMAKE_BUILD_DIR):
+        if not os.path.exists(CMAKE_BUILD_DIR()):
             raise SKBuildError(("CMake build folder ({}) does not exist. "
                                 "Did you forget to run configure before "
-                                "make?").format(CMAKE_BUILD_DIR))
+                                "make?").format(CMAKE_BUILD_DIR()))
 
         cmd = [self.cmake_executable, "--build", source_dir,
                "--target", "install", "--config", config, "--"]
         cmd.extend(clargs)
         cmd.extend(
             filter(bool,
                    shlex.split(os.environ.get("SKBUILD_BUILD_OPTIONS", "")))
         )
 
-        rtn = subprocess.call(cmd, cwd=CMAKE_BUILD_DIR, env=env)
+        rtn = subprocess.call(cmd, cwd=CMAKE_BUILD_DIR(), env=env)
         if rtn != 0:
             raise SKBuildError(
                 "An error occurred while building with CMake.\n"
                 "  Command:\n"
                 "    {}\n"
                 "  Source directory:\n"
                 "    {}\n"
                 "  Working directory:\n"
                 "    {}\n"
                 "Please see CMake's output for more information.".format(
                     self._formatArgsForDisplay(cmd),
                     os.path.abspath(source_dir),
-                    os.path.abspath(CMAKE_BUILD_DIR)))
+                    os.path.abspath(CMAKE_BUILD_DIR())))
 
     def install(self):
         """Returns a list of file paths to install via setuptools that is
         compatible with the data_files keyword argument.
         """
         return self._parse_manifests()
 
     def _parse_manifests(self):
         paths = \
-            glob.glob(os.path.join(CMAKE_BUILD_DIR, "install_manifest*.txt"))
+            glob.glob(os.path.join(CMAKE_BUILD_DIR(), "install_manifest*.txt"))
         try:
             return [self._parse_manifest(path) for path in paths][0]
         except IndexError:
             return []
 
     @staticmethod
     def _parse_manifest(install_manifest_path):
```

### Comparing `scikit-build-0.8.1/skbuild/compat.py` & `scikit-build-0.9.0/skbuild/compat.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/skbuild/utils/__init__.py` & `scikit-build-0.9.0/skbuild/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/skbuild/resources/cmake/FindF2PY.cmake` & `scikit-build-0.9.0/skbuild/resources/cmake/FindF2PY.cmake`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/skbuild/resources/cmake/FindPythonExtensions.cmake` & `scikit-build-0.9.0/skbuild/resources/cmake/FindPythonExtensions.cmake`

 * *Files 1% similar despite different names*

```diff
@@ -328,23 +328,23 @@
     set(_modinit_prefix "init")
   endif()
   message("_modinit_prefix:${_modinit_prefix}")
   if("${CMAKE_C_COMPILER_ID}" STREQUAL "MSVC")
     set_target_properties(${_target} PROPERTIES LINK_FLAGS 
         "/EXPORT:${_modinit_prefix}${_target}"
     )
-  elseif("${CMAKE_C_COMPILER_ID}" STREQUAL "GNU")
+  elseif("${CMAKE_C_COMPILER_ID}" STREQUAL "GNU" AND NOT ${CMAKE_SYSTEM_NAME} MATCHES "Darwin")
     set(_script_path
       ${CMAKE_CURRENT_BINARY_DIR}/CMakeFiles/${_target}-version-script.map
     )
     file(WRITE ${_script_path} 
                "{global: ${_modinit_prefix}${_target}; local: *; };"
     )
     set_property(TARGET ${_target} APPEND_STRING PROPERTY LINK_FLAGS
-        " -Wl,--version-script=${_script_path}"
+        " -Wl,--version-script=\"${_script_path}\""
     )
   endif()
 endfunction()
 
 function(python_extension_module _target)
   set(one_ops LINKED_MODULES_VAR FORWARD_DECL_MODULES_VAR MODULE_SUFFIX)
   cmake_parse_arguments(_args "" "${one_ops}" "" ${ARGN})
```

### Comparing `scikit-build-0.8.1/skbuild/resources/cmake/FindCython.cmake` & `scikit-build-0.9.0/skbuild/resources/cmake/FindCython.cmake`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/skbuild/resources/cmake/UseCython.cmake` & `scikit-build-0.9.0/skbuild/resources/cmake/UseCython.cmake`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/skbuild/resources/cmake/FindNumPy.cmake` & `scikit-build-0.9.0/skbuild/resources/cmake/FindNumPy.cmake`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/skbuild/resources/cmake/targetLinkLibrariesWithDynamicLookup.cmake` & `scikit-build-0.9.0/skbuild/resources/cmake/targetLinkLibrariesWithDynamicLookup.cmake`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/LICENSE` & `scikit-build-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-build-0.8.1/setup.py` & `scikit-build-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 with open('requirements.txt', 'r') as fp:
     requirements = list(filter(bool, (line.strip() for line in fp)))
 
 with open('requirements-dev.txt', 'r') as fp:
     dev_requirements = list(filter(bool, (line.strip() for line in fp)))
 
 # Require pytest-runner only when running tests
-pytest_runner = (['pytest-runner>=2.0,<3dev']
+pytest_runner = (['pytest-runner>=2.9']
                  if any(arg in sys.argv for arg in ('pytest', 'test'))
                  else [])
 
 setup_requires = pytest_runner
 
 setup(
     name='scikit-build',
```

### Comparing `scikit-build-0.8.1/PKG-INFO` & `scikit-build-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scikit-build
-Version: 0.8.1
+Version: 0.9.0
 Summary: Improved build system generator for Python C/C++/Fortran/Cython extensions
 Home-page: https://github.com/scikit-build/scikit-build
 Author: The scikit-build team
 Author-email: scikit-build@googlegroups.com
 License: MIT
 Description: ===============================
         scikit-build
@@ -26,15 +26,15 @@
         --------------
         
         .. table::
         
           +-----------------------------------------------------------------------------+-------------------------------------------------------------------------------+
           | Versions                                                                    | Downloads                                                                     |
           +=============================================================================+===============================================================================+
-          | .. image:: https://img.shields.io/pypi/v/scikit-build.svg                   | .. image:: https://img.shields.io/badge/downloads-54k%20total-green.svg       |
+          | .. image:: https://img.shields.io/pypi/v/scikit-build.svg                   | .. image:: https://img.shields.io/badge/downloads-95k%20total-green.svg       |
           |     :target: https://pypi.python.org/pypi/scikit-build                      |     :target: https://pypi.python.org/pypi/scikit-build                        |
           +-----------------------------------------------------------------------------+-------------------------------------------------------------------------------+
           | .. image:: https://anaconda.org/conda-forge/scikit-build/badges/version.svg | .. image:: https://anaconda.org/conda-forge/scikit-build/badges/downloads.svg |
           |     :target: https://anaconda.org/conda-forge/scikit-build                  |     :target: https://anaconda.org/conda-forge/scikit-build                    |
           +-----------------------------------------------------------------------------+-------------------------------------------------------------------------------+
```

