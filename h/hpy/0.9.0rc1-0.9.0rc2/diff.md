# Comparing `tmp/hpy-0.9.0rc1.tar.gz` & `tmp/hpy-0.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpy-0.9.0rc1.tar", last modified: Tue May  2 19:38:32 2023, max compression
+gzip compressed data, was "hpy-0.9.0rc2.tar", last modified: Thu May 11 11:14:32 2023, max compression
```

## Comparing `hpy-0.9.0rc1.tar` & `hpy-0.9.0rc2.tar`

### file list

```diff
@@ -1,324 +1,324 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.195921 hpy-0.9.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.163920 hpy-0.9.0rc1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.163920 hpy-0.9.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/.github/workflows/release-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/.github/workflows/valgrind-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-02 19:38:32.195921 hpy-0.9.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/README-gdb.md
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.163920 hpy-0.9.0rc1/c_test/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/c_test/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    60089 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/c_test/acutest.h
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/c_test/test_debug_handles.c
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/c_test/test_stacktrace.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.163920 hpy-0.9.0rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.163920 hpy-0.9.0rc1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/_static/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.163920 hpy-0.9.0rc1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/_templates/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.167920 hpy-0.9.0rc1/docs/api-reference/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/argument-parsing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/build-value.rst
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/builder.rst
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/formatting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/function-index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/helpers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/hpy-call.rst
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/hpy-ctx.rst
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/hpy-dict.rst
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/hpy-err.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/hpy-eval.rst
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/hpy-field.rst
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/hpy-gil.rst
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/hpy-global.rst
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/hpy-object.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/hpy-type.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/inline-helpers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/public-api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/structseq.rst
--rw-r--r--   0 runner    (1001) docker     (123)    25010 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.167920 hpy-0.9.0rc1/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/contributing/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/debug-mode.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.167920 hpy-0.9.0rc1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/debug-example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.167920 hpy-0.9.0rc1/docs/examples/hpytype-example/
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/hpytype-example/builtin_type.c
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/hpytype-example/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/hpytype-example/simple_type.c
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/hpytype-example/simple_type.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.167920 hpy-0.9.0rc1/docs/examples/mixed-example/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/mixed-example/mixed.c
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/mixed-example/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.167920 hpy-0.9.0rc1/docs/examples/quickstart/
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/quickstart/quickstart.c
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/quickstart/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.171920 hpy-0.9.0rc1/docs/examples/simple-example/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/simple-example/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/simple-example/simple.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.171920 hpy-0.9.0rc1/docs/examples/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/snippets/hpycall.c
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/snippets/hpyinit.c
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/snippets/hpyvarargs.c
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/snippets/legacyinit.c
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/snippets/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/snippets/snippets.c
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/trace-example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/leysin-2020-design-decisions.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.171920 hpy-0.9.0rc1/docs/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/misc/embedding.rst
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/misc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/module-state.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.171920 hpy-0.9.0rc1/docs/porting-example/
--rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.171920 hpy-0.9.0rc1/docs/porting-example/steps/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/setup00.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/setup01.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/setup02.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/setup03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/step_00_c_api.c
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/step_00_c_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/step_01_hpy_legacy.c
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/step_01_hpy_legacy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/step_02_hpy_legacy.c
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/step_02_hpy_legacy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/step_03_hpy_final.c
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/step_03_hpy_final.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/test_porting_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    40482 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/trace-mode.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/xxx-unsorted-notes.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/gdb-py.test
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.159920 hpy-0.9.0rc1/hpy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.175920 hpy-0.9.0rc1/hpy/debug/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/leakdetector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/pytest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.175920 hpy-0.9.0rc1/hpy/debug/src/
--rw-r--r--   0 runner    (1001) docker     (123)    14954 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/_debugmod.c
--rw-r--r--   0 runner    (1001) docker     (123)    18356 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/autogen_debug_ctx_call.i
--rw-r--r--   0 runner    (1001) docker     (123)    29310 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/autogen_debug_ctx_init.h
--rw-r--r--   0 runner    (1001) docker     (123)    59317 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/autogen_debug_wrappers.c
--rw-r--r--   0 runner    (1001) docker     (123)    22779 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/debug_ctx.c
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/debug_ctx_cpython.c
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/debug_ctx_not_cpython.c
--rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/debug_handles.c
--rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/debug_internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/dhqueue.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.175920 hpy-0.9.0rc1/hpy/debug/src/include/
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/include/hpy_debug.h
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/memprotect.c
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/stacktrace.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.175920 hpy-0.9.0rc1/hpy/devel/
--rw-r--r--   0 runner    (1001) docker     (123)    18442 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/abitag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.175920 hpy-0.9.0rc1/hpy/devel/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.179920 hpy-0.9.0rc1/hpy/devel/include/hpy/
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/autogen_hpyfunc_declare.h
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/autogen_hpyslot.h
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/cpy_types.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.179920 hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/
--rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/autogen_api_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/autogen_ctx.h
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/autogen_hpyfunc_trampolines.h
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/hpyfunc_trampolines.h
--rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/misc.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.179920 hpy-0.9.0rc1/hpy/devel/include/hpy/forbid_python_h/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/forbid_python_h/Python.h
--rw-r--r--   0 runner    (1001) docker     (123)    18148 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/hpydef.h
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/hpyexports.h
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/hpyfunc.h
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/hpymodule.h
--rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/hpytype.h
--rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/inline_helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/macros.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.179920 hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/argparse.h
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/buildvalue.h
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/ctx_funcs.h
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/ctx_module.h
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/ctx_type.h
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/format.h
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/structseq.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.179920 hpy-0.9.0rc1/hpy/devel/include/hpy/universal/
--rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/universal/autogen_ctx.h
--rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/universal/autogen_hpyfunc_trampolines.h
--rw-r--r--   0 runner    (1001) docker     (123)    23638 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/universal/autogen_trampolines.h
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/universal/hpyfunc_trampolines.h
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/universal/misc_trampolines.h
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-02 19:38:32.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/version.h
--rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.159920 hpy-0.9.0rc1/hpy/devel/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.183920 hpy-0.9.0rc1/hpy/devel/src/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)    26604 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/argparse.c
--rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/buildvalue.c
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_bytes.c
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_call.c
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_capsule.c
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_contextvar.c
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_err.c
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_eval.c
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_listbuilder.c
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_long.c
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_module.c
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_object.c
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_tracker.c
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_tuple.c
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_tuplebuilder.c
--rw-r--r--   0 runner    (1001) docker     (123)    57318 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_type.c
--rw-r--r--   0 runner    (1001) docker     (123)    22512 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/format.c
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/helpers.c
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/structseq.c
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-02 19:38:32.000000 hpy-0.9.0rc1/hpy/devel/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.183920 hpy-0.9.0rc1/hpy/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.183920 hpy-0.9.0rc1/hpy/tools/autogen/
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/autogen.h
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/autogenfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/hpyfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/hpyslot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8598 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    48452 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/public_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/pypy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.183920 hpy-0.9.0rc1/hpy/tools/autogen/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/testing/test_autogen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/testing/test_hpyfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/trampolines.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/include_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.183920 hpy-0.9.0rc1/hpy/tools/valgrind/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/valgrind/hpy.supp
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/valgrind/python.supp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.183920 hpy-0.9.0rc1/hpy/trace/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/trace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.183920 hpy-0.9.0rc1/hpy/trace/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/trace/src/_tracemod.c
--rw-r--r--   0 runner    (1001) docker     (123)    27287 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/trace/src/autogen_trace_ctx_init.h
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/trace/src/autogen_trace_func_table.c
--rw-r--r--   0 runner    (1001) docker     (123)    78016 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/trace/src/autogen_trace_wrappers.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.183920 hpy-0.9.0rc1/hpy/trace/src/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/trace/src/include/hpy_trace.h
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/trace/src/trace_ctx.c
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/trace/src/trace_internal.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.159920 hpy-0.9.0rc1/hpy/universal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.187920 hpy-0.9.0rc1/hpy/universal/src/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/api.h
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/autogen_ctx_call.i
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/autogen_ctx_def.h
--rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/autogen_ctx_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/ctx.c
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/ctx_meth.c
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/ctx_meth.h
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/ctx_misc.c
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/ctx_misc.h
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/handles.h
--rw-r--r--   0 runner    (1001) docker     (123)    24089 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/hpymodule.c
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/misc_win32.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.175920 hpy-0.9.0rc1/hpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-02 19:38:32.000000 hpy-0.9.0rc1/hpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-05-02 19:38:32.000000 hpy-0.9.0rc1/hpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:38:32.000000 hpy-0.9.0rc1/hpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-02 19:38:32.000000 hpy-0.9.0rc1/hpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 19:38:32.000000 hpy-0.9.0rc1/hpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 19:38:32.000000 hpy-0.9.0rc1/hpy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.187920 hpy-0.9.0rc1/microbench/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/microbench/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/microbench/_valgrind_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/microbench/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/microbench/pytest_valgrind.sh
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/microbench/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.187920 hpy-0.9.0rc1/microbench/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/microbench/src/cpy_simple.c
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/microbench/src/hpy_simple.c
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/microbench/test_microbench.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.187920 hpy-0.9.0rc1/proof-of-concept/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/proof-of-concept/pof.c
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/proof-of-concept/pofcpp.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.187920 hpy-0.9.0rc1/proof-of-concept/pofpackage/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/proof-of-concept/pofpackage/bar.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/proof-of-concept/pofpackage/foo.c
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/proof-of-concept/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/proof-of-concept/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/proof-of-concept/test_pof.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5000 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/proof-of-concept/test_pof.sh
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/requirements-autogen.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 19:38:32.195921 hpy-0.9.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.191920 hpy-0.9.0rc1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/check_py27_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.195921 hpy-0.9.0rc1/test/debug/
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/debug/test_builder_invalid.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/debug/test_charptr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/debug/test_context_reuse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/debug/test_handles_invalid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/debug/test_handles_leak.py
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/debug/test_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.195921 hpy-0.9.0rc1/test/hpy_devel/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/hpy_devel/test_abitag.py
--rw-r--r--   0 runner    (1001) docker     (123)    12635 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/hpy_devel/test_distutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/support.py
--rw-r--r--   0 runner    (1001) docker     (123)    19846 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_00_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    24280 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_call.py
--rw-r--r--   0 runner    (1001) docker     (123)    17094 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_capsule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_capsule_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_contextvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_cpy_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpybuildvalue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpybytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpydict.py
--rw-r--r--   0 runner    (1001) docker     (123)    29552 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpyerr.py
--rw-r--r--   0 runner    (1001) docker     (123)    14932 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpyfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpyglobal.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpyimport.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpylist.py
--rw-r--r--   0 runner    (1001) docker     (123)    16027 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpylong.py
--rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpymodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpyslice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpystructseq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpytuple.py
--rw-r--r--   0 runner    (1001) docker     (123)    60249 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpytype.py
--rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpytype_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    43142 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpyunicode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_importing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_legacy_forbidden.py
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    23728 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    28206 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_slots.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_slots_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.195921 hpy-0.9.0rc1/test/trace/
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/trace/test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.302524 hpy-0.9.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.246524 hpy-0.9.0rc2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.250524 hpy-0.9.0rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/.github/workflows/release-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/.github/workflows/valgrind-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-11 11:14:32.302524 hpy-0.9.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/README-gdb.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.250524 hpy-0.9.0rc2/c_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/c_test/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    60089 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/c_test/acutest.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/c_test/test_debug_handles.c
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/c_test/test_stacktrace.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.254524 hpy-0.9.0rc2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.254524 hpy-0.9.0rc2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/_static/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.254524 hpy-0.9.0rc2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/_templates/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.258524 hpy-0.9.0rc2/docs/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api-reference/argument-parsing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api-reference/build-value.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api-reference/builder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api-reference/formatting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api-reference/function-index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api-reference/helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api-reference/hpy-call.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api-reference/hpy-ctx.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api-reference/hpy-dict.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api-reference/hpy-err.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api-reference/hpy-eval.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api-reference/hpy-field.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api-reference/hpy-gil.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api-reference/hpy-global.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api-reference/hpy-object.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api-reference/hpy-type.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api-reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api-reference/inline-helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api-reference/public-api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api-reference/structseq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25010 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.258524 hpy-0.9.0rc2/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/contributing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/debug-mode.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.258524 hpy-0.9.0rc2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/examples/debug-example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.258524 hpy-0.9.0rc2/docs/examples/hpytype-example/
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/examples/hpytype-example/builtin_type.c
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/examples/hpytype-example/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/examples/hpytype-example/simple_type.c
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/examples/hpytype-example/simple_type.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.258524 hpy-0.9.0rc2/docs/examples/mixed-example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/examples/mixed-example/mixed.c
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/examples/mixed-example/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.262524 hpy-0.9.0rc2/docs/examples/quickstart/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/examples/quickstart/quickstart.c
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/examples/quickstart/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.262524 hpy-0.9.0rc2/docs/examples/simple-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/examples/simple-example/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/examples/simple-example/simple.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.262524 hpy-0.9.0rc2/docs/examples/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/examples/snippets/hpycall.c
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/examples/snippets/hpyinit.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/examples/snippets/hpyvarargs.c
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/examples/snippets/legacyinit.c
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/examples/snippets/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/examples/snippets/snippets.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/examples/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/examples/trace-example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/leysin-2020-design-decisions.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.266524 hpy-0.9.0rc2/docs/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/misc/embedding.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/misc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/module-state.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.266524 hpy-0.9.0rc2/docs/porting-example/
+-rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/porting-example/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.270524 hpy-0.9.0rc2/docs/porting-example/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/porting-example/steps/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/porting-example/steps/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/porting-example/steps/setup00.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/porting-example/steps/setup01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/porting-example/steps/setup02.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/porting-example/steps/setup03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/porting-example/steps/step_00_c_api.c
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/porting-example/steps/step_00_c_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/porting-example/steps/step_01_hpy_legacy.c
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/porting-example/steps/step_01_hpy_legacy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/porting-example/steps/step_02_hpy_legacy.c
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/porting-example/steps/step_02_hpy_legacy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/porting-example/steps/step_03_hpy_final.c
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/porting-example/steps/step_03_hpy_final.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/porting-example/steps/test_porting_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40482 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/porting-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/trace-mode.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/docs/xxx-unsorted-notes.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/gdb-py.test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.246524 hpy-0.9.0rc2/hpy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.270524 hpy-0.9.0rc2/hpy/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/debug/leakdetector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/debug/pytest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.274524 hpy-0.9.0rc2/hpy/debug/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    14954 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/debug/src/_debugmod.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18356 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/debug/src/autogen_debug_ctx_call.i
+-rw-r--r--   0 runner    (1001) docker     (123)    29310 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/debug/src/autogen_debug_ctx_init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    59317 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/debug/src/autogen_debug_wrappers.c
+-rw-r--r--   0 runner    (1001) docker     (123)    22779 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/debug/src/debug_ctx.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/debug/src/debug_ctx_cpython.c
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/debug/src/debug_ctx_not_cpython.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/debug/src/debug_handles.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/debug/src/debug_internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/debug/src/dhqueue.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.274524 hpy-0.9.0rc2/hpy/debug/src/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/debug/src/include/hpy_debug.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/debug/src/memprotect.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/debug/src/stacktrace.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.274524 hpy-0.9.0rc2/hpy/devel/
+-rw-r--r--   0 runner    (1001) docker     (123)    18636 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/abitag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.274524 hpy-0.9.0rc2/hpy/devel/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.278524 hpy-0.9.0rc2/hpy/devel/include/hpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/autogen_hpyfunc_declare.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/autogen_hpyslot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/cpy_types.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.278524 hpy-0.9.0rc2/hpy/devel/include/hpy/cpython/
+-rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/cpython/autogen_api_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/cpython/autogen_ctx.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/cpython/autogen_hpyfunc_trampolines.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/cpython/hpyfunc_trampolines.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/cpython/misc.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.278524 hpy-0.9.0rc2/hpy/devel/include/hpy/forbid_python_h/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/forbid_python_h/Python.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18148 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/hpydef.h
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/hpyexports.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/hpyfunc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/hpymodule.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/hpytype.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/inline_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/macros.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.278524 hpy-0.9.0rc2/hpy/devel/include/hpy/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/runtime/argparse.h
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/runtime/buildvalue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/runtime/ctx_funcs.h
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/runtime/ctx_module.h
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/runtime/ctx_type.h
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/runtime/format.h
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/runtime/helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/runtime/structseq.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.282524 hpy-0.9.0rc2/hpy/devel/include/hpy/universal/
+-rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/universal/autogen_ctx.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/universal/autogen_hpyfunc_trampolines.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23638 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/universal/autogen_trampolines.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/universal/hpyfunc_trampolines.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/universal/misc_trampolines.h
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 11:14:32.000000 hpy-0.9.0rc2/hpy/devel/include/hpy/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/include/hpy.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.242524 hpy-0.9.0rc2/hpy/devel/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.286524 hpy-0.9.0rc2/hpy/devel/src/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)    26604 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/src/runtime/argparse.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/src/runtime/buildvalue.c
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_bytes.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_call.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_capsule.c
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_contextvar.c
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_err.c
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_eval.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_listbuilder.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_long.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_module.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_object.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_tracker.c
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_tuple.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_tuplebuilder.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57318 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_type.c
+-rw-r--r--   0 runner    (1001) docker     (123)    22512 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/src/runtime/format.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/src/runtime/helpers.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/devel/src/runtime/structseq.c
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-11 11:14:32.000000 hpy-0.9.0rc2/hpy/devel/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.286524 hpy-0.9.0rc2/hpy/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.286524 hpy-0.9.0rc2/hpy/tools/autogen/
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/tools/autogen/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/tools/autogen/autogen.h
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/tools/autogen/autogenfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/tools/autogen/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/tools/autogen/ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/tools/autogen/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/tools/autogen/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/tools/autogen/hpyfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/tools/autogen/hpyslot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8598 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/tools/autogen/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48452 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/tools/autogen/public_api.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/tools/autogen/pypy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.290524 hpy-0.9.0rc2/hpy/tools/autogen/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/tools/autogen/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/tools/autogen/testing/test_autogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/tools/autogen/testing/test_hpyfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/tools/autogen/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/tools/autogen/trampolines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/tools/include_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.290524 hpy-0.9.0rc2/hpy/tools/valgrind/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/tools/valgrind/hpy.supp
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/tools/valgrind/python.supp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.290524 hpy-0.9.0rc2/hpy/trace/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/trace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.290524 hpy-0.9.0rc2/hpy/trace/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/trace/src/_tracemod.c
+-rw-r--r--   0 runner    (1001) docker     (123)    27287 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/trace/src/autogen_trace_ctx_init.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/trace/src/autogen_trace_func_table.c
+-rw-r--r--   0 runner    (1001) docker     (123)    78016 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/trace/src/autogen_trace_wrappers.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.290524 hpy-0.9.0rc2/hpy/trace/src/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/trace/src/include/hpy_trace.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/trace/src/trace_ctx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/trace/src/trace_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.246524 hpy-0.9.0rc2/hpy/universal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.290524 hpy-0.9.0rc2/hpy/universal/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/universal/src/api.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/universal/src/autogen_ctx_call.i
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/universal/src/autogen_ctx_def.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/universal/src/autogen_ctx_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/universal/src/ctx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/universal/src/ctx_meth.c
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/universal/src/ctx_meth.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/universal/src/ctx_misc.c
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/universal/src/ctx_misc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/universal/src/handles.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24089 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/universal/src/hpymodule.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/hpy/universal/src/misc_win32.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.270524 hpy-0.9.0rc2/hpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-11 11:14:32.000000 hpy-0.9.0rc2/hpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-05-11 11:14:32.000000 hpy-0.9.0rc2/hpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 11:14:32.000000 hpy-0.9.0rc2/hpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-11 11:14:32.000000 hpy-0.9.0rc2/hpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-11 11:14:32.000000 hpy-0.9.0rc2/hpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-11 11:14:32.000000 hpy-0.9.0rc2/hpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.294524 hpy-0.9.0rc2/microbench/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/microbench/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/microbench/_valgrind_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/microbench/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/microbench/pytest_valgrind.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/microbench/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.294524 hpy-0.9.0rc2/microbench/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/microbench/src/cpy_simple.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/microbench/src/hpy_simple.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/microbench/test_microbench.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.294524 hpy-0.9.0rc2/proof-of-concept/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/proof-of-concept/pof.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/proof-of-concept/pofcpp.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.294524 hpy-0.9.0rc2/proof-of-concept/pofpackage/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/proof-of-concept/pofpackage/bar.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/proof-of-concept/pofpackage/foo.c
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/proof-of-concept/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/proof-of-concept/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/proof-of-concept/test_pof.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5000 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/proof-of-concept/test_pof.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/requirements-autogen.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 11:14:32.302524 hpy-0.9.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.298524 hpy-0.9.0rc2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/check_py27_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.302524 hpy-0.9.0rc2/test/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/debug/test_builder_invalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/debug/test_charptr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/debug/test_context_reuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/debug/test_handles_invalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/debug/test_handles_leak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/debug/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.302524 hpy-0.9.0rc2/test/hpy_devel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/hpy_devel/test_abitag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12635 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/hpy_devel/test_distutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19846 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_00_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24280 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17094 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_capsule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_capsule_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_contextvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_cpy_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_hpybuildvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_hpybytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_hpydict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29552 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_hpyerr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14932 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_hpyfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_hpyglobal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_hpyimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_hpylist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16027 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_hpylong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_hpymodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_hpyslice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_hpystructseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_hpytuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60249 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_hpytype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_hpytype_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43142 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_hpyunicode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_legacy_forbidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23728 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28206 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_slots_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/test_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:14:32.302524 hpy-0.9.0rc2/test/trace/
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-11 11:14:23.000000 hpy-0.9.0rc2/test/trace/test_trace.py
```

### Comparing `hpy-0.9.0rc1/.github/workflows/ci.yml` & `hpy-0.9.0rc2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/.github/workflows/release-pypi.yml` & `hpy-0.9.0rc2/.github/workflows/release-pypi.yml`

 * *Files 3% similar despite different names*

```diff
@@ -122,20 +122,15 @@
     if: github.repository == 'hpyproject/hpy'
     steps:
     - uses: actions/download-artifact@v3
       with:
         name: artifact
         path: dist
 
-    - name: Checkout
-      uses: actions/checkout@v3
-      with:
-        ref: ${{ inputs.tag }}
-
     - name: Release
       uses: softprops/action-gh-release@v1
       with:
         files: dist/*
         # consider tags in form '*.*.*rc*' to indicate a pre-release
-        prerelease: ${{ contains(github.ref, 'rc') }}
+        prerelease: ${{ contains(inputs.tag, 'rc') }}
         draft: ${{ !inputs.official }}
         tag_name: ${{ inputs.tag }}
```

### Comparing `hpy-0.9.0rc1/.github/workflows/valgrind-tests.yml` & `hpy-0.9.0rc2/.github/workflows/valgrind-tests.yml`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/.gitignore` & `hpy-0.9.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/AUTHORS` & `hpy-0.9.0rc2/AUTHORS`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/CONTRIBUTING.md` & `hpy-0.9.0rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/LICENSE` & `hpy-0.9.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/Makefile` & `hpy-0.9.0rc2/Makefile`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/PKG-INFO` & `hpy-0.9.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpy
-Version: 0.9.0rc1
+Version: 0.9.0rc2
 Summary: A better C API for Python
 Home-page: https://hpyproject.org
 Author: The HPy team
 Author-email: hpy-dev@python.org
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `hpy-0.9.0rc1/README-gdb.md` & `hpy-0.9.0rc2/README-gdb.md`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/README.md` & `hpy-0.9.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/c_test/acutest.h` & `hpy-0.9.0rc2/c_test/acutest.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/c_test/test_debug_handles.c` & `hpy-0.9.0rc2/c_test/test_debug_handles.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/Makefile` & `hpy-0.9.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/api-reference/function-index.rst` & `hpy-0.9.0rc2/docs/api-reference/function-index.rst`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/api-reference/hpy-type.rst` & `hpy-0.9.0rc2/docs/api-reference/hpy-type.rst`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/api-reference/index.rst` & `hpy-0.9.0rc2/docs/api-reference/index.rst`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/api-reference/inline-helpers.rst` & `hpy-0.9.0rc2/docs/api-reference/inline-helpers.rst`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/api-reference/structseq.rst` & `hpy-0.9.0rc2/docs/api-reference/structseq.rst`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/api.rst` & `hpy-0.9.0rc2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/changelog.rst` & `hpy-0.9.0rc2/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/conf.py` & `hpy-0.9.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/contributing/index.rst` & `hpy-0.9.0rc2/docs/contributing/index.rst`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/debug-mode.rst` & `hpy-0.9.0rc2/docs/debug-mode.rst`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/examples/hpytype-example/builtin_type.c` & `hpy-0.9.0rc2/docs/examples/hpytype-example/builtin_type.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/examples/hpytype-example/simple_type.c` & `hpy-0.9.0rc2/docs/examples/hpytype-example/simple_type.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/examples/mixed-example/mixed.c` & `hpy-0.9.0rc2/docs/examples/mixed-example/mixed.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/examples/quickstart/quickstart.c` & `hpy-0.9.0rc2/docs/examples/quickstart/quickstart.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/examples/simple-example/simple.c` & `hpy-0.9.0rc2/docs/examples/simple-example/simple.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/examples/snippets/hpycall.c` & `hpy-0.9.0rc2/docs/examples/snippets/hpycall.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/examples/snippets/hpyvarargs.c` & `hpy-0.9.0rc2/docs/examples/snippets/hpyvarargs.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/examples/snippets/setup.py` & `hpy-0.9.0rc2/docs/examples/snippets/setup.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/examples/snippets/snippets.c` & `hpy-0.9.0rc2/docs/examples/snippets/snippets.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/examples/tests.py` & `hpy-0.9.0rc2/docs/examples/tests.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/index.rst` & `hpy-0.9.0rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/leysin-2020-design-decisions.md` & `hpy-0.9.0rc2/docs/leysin-2020-design-decisions.md`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/misc/embedding.rst` & `hpy-0.9.0rc2/docs/misc/embedding.rst`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/module-state.txt` & `hpy-0.9.0rc2/docs/module-state.txt`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/overview.rst` & `hpy-0.9.0rc2/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/porting-example/index.rst` & `hpy-0.9.0rc2/docs/porting-example/index.rst`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/porting-example/steps/conftest.py` & `hpy-0.9.0rc2/docs/porting-example/steps/conftest.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/porting-example/steps/step_00_c_api.c` & `hpy-0.9.0rc2/docs/porting-example/steps/step_00_c_api.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/porting-example/steps/step_01_hpy_legacy.c` & `hpy-0.9.0rc2/docs/porting-example/steps/step_01_hpy_legacy.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/porting-example/steps/step_02_hpy_legacy.c` & `hpy-0.9.0rc2/docs/porting-example/steps/step_02_hpy_legacy.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/porting-example/steps/step_03_hpy_final.c` & `hpy-0.9.0rc2/docs/porting-example/steps/step_03_hpy_final.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/porting-example/steps/test_porting_example.py` & `hpy-0.9.0rc2/docs/porting-example/steps/test_porting_example.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/porting-guide.rst` & `hpy-0.9.0rc2/docs/porting-guide.rst`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/quickstart.rst` & `hpy-0.9.0rc2/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/trace-mode.rst` & `hpy-0.9.0rc2/docs/trace-mode.rst`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/docs/xxx-unsorted-notes.txt` & `hpy-0.9.0rc2/docs/xxx-unsorted-notes.txt`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/debug/leakdetector.py` & `hpy-0.9.0rc2/hpy/debug/leakdetector.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/debug/pytest.py` & `hpy-0.9.0rc2/hpy/debug/pytest.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/debug/src/_debugmod.c` & `hpy-0.9.0rc2/hpy/debug/src/_debugmod.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/debug/src/autogen_debug_ctx_call.i` & `hpy-0.9.0rc2/hpy/debug/src/autogen_debug_ctx_call.i`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/debug/src/autogen_debug_ctx_init.h` & `hpy-0.9.0rc2/hpy/debug/src/autogen_debug_ctx_init.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/debug/src/autogen_debug_wrappers.c` & `hpy-0.9.0rc2/hpy/debug/src/autogen_debug_wrappers.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/debug/src/debug_ctx.c` & `hpy-0.9.0rc2/hpy/debug/src/debug_ctx.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/debug/src/debug_ctx_cpython.c` & `hpy-0.9.0rc2/hpy/debug/src/debug_ctx_cpython.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/debug/src/debug_ctx_not_cpython.c` & `hpy-0.9.0rc2/hpy/debug/src/debug_ctx_not_cpython.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/debug/src/debug_handles.c` & `hpy-0.9.0rc2/hpy/debug/src/debug_handles.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/debug/src/debug_internal.h` & `hpy-0.9.0rc2/hpy/debug/src/debug_internal.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/debug/src/dhqueue.c` & `hpy-0.9.0rc2/hpy/debug/src/dhqueue.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/debug/src/include/hpy_debug.h` & `hpy-0.9.0rc2/hpy/debug/src/include/hpy_debug.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/debug/src/memprotect.c` & `hpy-0.9.0rc2/hpy/debug/src/memprotect.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/debug/src/stacktrace.c` & `hpy-0.9.0rc2/hpy/debug/src/stacktrace.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/__init__.py` & `hpy-0.9.0rc2/hpy/devel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
             modes.
         """
         return list(map(str, [
             self.src_dir.joinpath('argparse.c'),
             self.src_dir.joinpath('buildvalue.c'),
             self.src_dir.joinpath('format.c'),
             self.src_dir.joinpath('helpers.c'),
+            self.src_dir.joinpath('structseq.c'),
         ]))
 
     def _scan_static_lib_dir(self):
         """ Scan the static library directory and build a dict for all
             available static libraries. The library directory contains
             subdirectories for each ABI and the ABI folders then contain
             the static libraries.
@@ -183,16 +184,19 @@
     if getattr(dist, 'hpydevel', None):
         return
 
     # add a global option --hpy-abi to setup.py
     dist.__class__.hpy_abi = DEFAULT_HPY_ABI
     dist.__class__.hpy_use_static_libs = False
     dist.__class__.global_options += [
-        ('hpy-abi=', None, 'Specify the HPy ABI mode (default: %s)' % DEFAULT_HPY_ABI),
-        ('hpy-no-static-libs', None, 'Compile context and extra sources with extension (default: False)')
+        ('hpy-abi=', None, 'Specify the HPy ABI mode (default: %s)'
+                           % DEFAULT_HPY_ABI),
+        ('hpy-use-static-libs', None, 'Use static library containing context '
+                                      'and helper functions for building '
+                                      'extensions (default: False)')
     ]
     hpydevel = HPyDevel()
     hpydevel.fix_distribution(dist)
 
 
 _HPY_UNIVERSAL_MODULE_STUB_TEMPLATE = """
 # DO NOT EDIT THIS FILE!
```

### Comparing `hpy-0.9.0rc1/hpy/devel/abitag.py` & `hpy-0.9.0rc2/hpy/devel/abitag.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/autogen_hpyfunc_declare.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/autogen_hpyfunc_declare.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/autogen_hpyslot.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/autogen_hpyslot.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/cpy_types.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/cpy_types.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/autogen_api_impl.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/cpython/autogen_api_impl.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/autogen_ctx.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/cpython/autogen_ctx.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/autogen_hpyfunc_trampolines.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/cpython/autogen_hpyfunc_trampolines.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/hpyfunc_trampolines.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/cpython/hpyfunc_trampolines.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/misc.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/cpython/misc.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/hpydef.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/hpydef.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/hpyfunc.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/hpyfunc.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/hpymodule.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/hpymodule.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/hpytype.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/hpytype.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/inline_helpers.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/inline_helpers.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/macros.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/macros.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/argparse.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/runtime/argparse.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/ctx_funcs.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/runtime/ctx_funcs.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/ctx_module.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/runtime/ctx_module.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/ctx_type.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/runtime/ctx_type.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/format.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/runtime/format.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/structseq.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/runtime/structseq.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/universal/autogen_ctx.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/universal/autogen_ctx.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/universal/autogen_hpyfunc_trampolines.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/universal/autogen_hpyfunc_trampolines.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/universal/autogen_trampolines.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/universal/autogen_trampolines.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/universal/hpyfunc_trampolines.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/universal/hpyfunc_trampolines.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy/universal/misc_trampolines.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy/universal/misc_trampolines.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/include/hpy.h` & `hpy-0.9.0rc2/hpy/devel/include/hpy.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/src/runtime/argparse.c` & `hpy-0.9.0rc2/hpy/devel/src/runtime/argparse.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/src/runtime/buildvalue.c` & `hpy-0.9.0rc2/hpy/devel/src/runtime/buildvalue.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_bytes.c` & `hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_bytes.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_call.c` & `hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_call.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_capsule.c` & `hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_capsule.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_eval.c` & `hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_eval.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_listbuilder.c` & `hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_listbuilder.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_long.c` & `hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_long.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_module.c` & `hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_module.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_object.c` & `hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_object.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_tracker.c` & `hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_tracker.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_tuplebuilder.c` & `hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_tuplebuilder.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_type.c` & `hpy-0.9.0rc2/hpy/devel/src/runtime/ctx_type.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/src/runtime/format.c` & `hpy-0.9.0rc2/hpy/devel/src/runtime/format.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/src/runtime/helpers.c` & `hpy-0.9.0rc2/hpy/devel/src/runtime/helpers.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/devel/src/runtime/structseq.c` & `hpy-0.9.0rc2/hpy/devel/src/runtime/structseq.c`

 * *Files 9% similar despite different names*

```diff
@@ -24,16 +24,18 @@
     }
 
     for (i = 0; desc->fields[i].name != NULL; i++) {
     }
 
 #ifndef HPY_ABI_CPYTHON
     HPyTracker ht;
-    HPy fields, args, kwds, defs, docstring, n_fields;
+    HPy fields, args, kwds, defs, docstring, n_fields, h_field, h_modname;
     HPy result = HPy_NULL;
+    const char *name, *s;
+    char *modname;
 
     HPy collections = HPyImport_ImportModule(ctx, "collections");
     if (HPy_IsNull(collections)) {
         return HPy_NULL;
     }
     HPy namedtuple = HPy_GetAttr_s(ctx, collections, "namedtuple");
     HPy_Close(ctx, collections);
@@ -52,16 +54,16 @@
     if (HPy_IsNull(h_name)) {
         goto error;
     }
     HPyTupleBuilder_Set(ctx, argsBuilder, 0, h_name);
     HPy_Close(ctx, h_name);
 
     i = 0;
-    for (const char* name = desc->fields[i].name; name != NULL; name = desc->fields[++i].name) {
-        HPy h_field = HPyUnicode_FromString(ctx, name);
+    for (name = desc->fields[i].name; name != NULL; name = desc->fields[++i].name) {
+        h_field = HPyUnicode_FromString(ctx, name);
         if (HPy_IsNull(h_field)) {
             HPyTupleBuilder_Cancel(ctx, argsBuilder);
             HPyTupleBuilder_Cancel(ctx, fieldsBuilder);
             HPyTupleBuilder_Cancel(ctx, defsBuilder);
             goto error;
         }
         HPyTupleBuilder_Set(ctx, fieldsBuilder, i, h_field);
@@ -126,16 +128,15 @@
     }
     HPyTracker_Add(ctx, ht, n_fields);
     if (HPy_SetAttr_s(ctx, result, "n_fields", n_fields) < 0) {
         goto error;
     }
 
     /* Set the type name and qualname */
-    const char *s = strrchr(desc->name, '.');
-    char *modname;
+    s = strrchr(desc->name, '.');
     if (s == NULL) {
         s = desc->name;
         modname = NULL;
     }
     else {
         /* TODO: Replace this by using 'HPyUnicode_FromStringAndSize' or similar
            once available. */
@@ -159,15 +160,15 @@
     HPyTracker_Add(ctx, ht, h_name);
     if (HPy_SetAttr_s(ctx, result, "__name__", h_name) < 0 ||
             HPy_SetAttr_s(ctx, result, "__qualname__", h_name) < 0) {
         goto error;
     }
 
     if (modname != NULL) {
-        HPy h_modname = HPyUnicode_FromString(ctx, modname);
+        h_modname = HPyUnicode_FromString(ctx, modname);
         free(modname);
         if (HPy_IsNull(h_modname)) {
             goto error;
         }
         HPyTracker_Add(ctx, ht, h_modname);
         if (HPy_SetAttr_s(ctx, result, "__module__", h_modname) < 0) {
             goto error;
@@ -187,15 +188,15 @@
 #if PY_VERSION_HEX < 0x03090000
         // In Python 3.8.x or earlier, the docstring MUST NOT be NULL
         .doc = (desc->doc != NULL ? desc->doc : ""),
 #else
         .doc = desc->doc,
 #endif
         .fields = (PyStructSequence_Field *)desc->fields,
-        .n_in_sequence = i
+        .n_in_sequence = (int)i
     };
     return _py2h((PyObject*) PyStructSequence_NewType(&d));
 #endif
 }
 
 HPyAPI_HELPER HPy
 HPyStructSequence_New(HPyContext *ctx, HPy type, HPy_ssize_t nargs, HPy *args)
@@ -212,37 +213,40 @@
     if (HPy_IsNull(tuple)) {
         return HPy_NULL;
     }
     HPy result = HPy_CallTupleDict(ctx, type, tuple, HPy_NULL);
     HPy_Close(ctx, tuple);
     return result;
 #else
-    PyTypeObject *tp = (PyTypeObject *)_h2py(type);
+    PyTypeObject *tp;
+    PyObject *name, *v, *seq, *item;
+    Py_ssize_t n_fields, i;
+
+    tp = (PyTypeObject *)_h2py(type);
+    name = PyUnicode_FromStringAndSize(s_n_fields, sizeof(s_n_fields));
     // CPython also accesses the dict directly
-    PyObject *name = PyUnicode_FromStringAndSize(s_n_fields, sizeof(s_n_fields));
-    PyObject *v = PyDict_GetItemWithError(tp->tp_dict, name);
+    v = PyDict_GetItemWithError(tp->tp_dict, name);
     Py_DECREF(name);
     if (v == NULL && !PyErr_Occurred()) {
         goto type_error;
     }
-    Py_ssize_t n_fields = PyLong_AsSsize_t(v);
-    PyObject *seq = PyStructSequence_New(tp);
+    n_fields = PyLong_AsSsize_t(v);
+    seq = PyStructSequence_New(tp);
     if (seq == NULL) {
         goto type_error;
     }
     if (n_fields != nargs) {
         PyErr_Format(PyExc_TypeError,
                      "expected exactly %d arguments but got %d",
                      n_fields, nargs);
         Py_DECREF(seq);
         goto error;
     }
 
-    PyObject *item;
-    for (Py_ssize_t i = 0; i < nargs; i++) {
+    for (i = 0; i < nargs; i++) {
         item = _h2py(args[i]);
         Py_INCREF(item);
         PyStructSequence_SetItem(seq, i, item);
     }
     return _py2h(seq);
 
 type_error:
```

### Comparing `hpy-0.9.0rc1/hpy/tools/autogen/__main__.py` & `hpy-0.9.0rc2/hpy/tools/autogen/__main__.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/tools/autogen/autogen.h` & `hpy-0.9.0rc2/hpy/tools/autogen/autogen.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/tools/autogen/autogenfile.py` & `hpy-0.9.0rc2/hpy/tools/autogen/autogenfile.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/tools/autogen/conf.py` & `hpy-0.9.0rc2/hpy/tools/autogen/conf.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/tools/autogen/ctx.py` & `hpy-0.9.0rc2/hpy/tools/autogen/ctx.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/tools/autogen/debug.py` & `hpy-0.9.0rc2/hpy/tools/autogen/debug.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/tools/autogen/doc.py` & `hpy-0.9.0rc2/hpy/tools/autogen/doc.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/tools/autogen/hpyfunc.py` & `hpy-0.9.0rc2/hpy/tools/autogen/hpyfunc.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/tools/autogen/hpyslot.py` & `hpy-0.9.0rc2/hpy/tools/autogen/hpyslot.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/tools/autogen/parse.py` & `hpy-0.9.0rc2/hpy/tools/autogen/parse.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/tools/autogen/public_api.h` & `hpy-0.9.0rc2/hpy/tools/autogen/public_api.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/tools/autogen/pypy.py` & `hpy-0.9.0rc2/hpy/tools/autogen/pypy.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/tools/autogen/testing/test_autogen.py` & `hpy-0.9.0rc2/hpy/tools/autogen/testing/test_autogen.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/tools/autogen/testing/test_hpyfunc.py` & `hpy-0.9.0rc2/hpy/tools/autogen/testing/test_hpyfunc.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/tools/autogen/trace.py` & `hpy-0.9.0rc2/hpy/tools/autogen/trace.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/tools/autogen/trampolines.py` & `hpy-0.9.0rc2/hpy/tools/autogen/trampolines.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/tools/valgrind/hpy.supp` & `hpy-0.9.0rc2/hpy/tools/valgrind/hpy.supp`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/tools/valgrind/python.supp` & `hpy-0.9.0rc2/hpy/tools/valgrind/python.supp`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/trace/src/_tracemod.c` & `hpy-0.9.0rc2/hpy/trace/src/_tracemod.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/trace/src/autogen_trace_ctx_init.h` & `hpy-0.9.0rc2/hpy/trace/src/autogen_trace_ctx_init.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/trace/src/autogen_trace_func_table.c` & `hpy-0.9.0rc2/hpy/trace/src/autogen_trace_func_table.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/trace/src/autogen_trace_wrappers.c` & `hpy-0.9.0rc2/hpy/trace/src/autogen_trace_wrappers.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/trace/src/include/hpy_trace.h` & `hpy-0.9.0rc2/hpy/trace/src/include/hpy_trace.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/trace/src/trace_ctx.c` & `hpy-0.9.0rc2/hpy/trace/src/trace_ctx.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/trace/src/trace_internal.h` & `hpy-0.9.0rc2/hpy/trace/src/trace_internal.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/universal/src/autogen_ctx_call.i` & `hpy-0.9.0rc2/hpy/universal/src/autogen_ctx_call.i`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/universal/src/autogen_ctx_def.h` & `hpy-0.9.0rc2/hpy/universal/src/autogen_ctx_def.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/universal/src/autogen_ctx_impl.h` & `hpy-0.9.0rc2/hpy/universal/src/autogen_ctx_impl.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/universal/src/ctx_meth.c` & `hpy-0.9.0rc2/hpy/universal/src/ctx_meth.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/universal/src/ctx_misc.c` & `hpy-0.9.0rc2/hpy/universal/src/ctx_misc.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/universal/src/ctx_misc.h` & `hpy-0.9.0rc2/hpy/universal/src/ctx_misc.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/universal/src/handles.h` & `hpy-0.9.0rc2/hpy/universal/src/handles.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/universal/src/hpymodule.c` & `hpy-0.9.0rc2/hpy/universal/src/hpymodule.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy/universal/src/misc_win32.h` & `hpy-0.9.0rc2/hpy/universal/src/misc_win32.h`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/hpy.egg-info/PKG-INFO` & `hpy-0.9.0rc2/hpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpy
-Version: 0.9.0rc1
+Version: 0.9.0rc2
 Summary: A better C API for Python
 Home-page: https://hpyproject.org
 Author: The HPy team
 Author-email: hpy-dev@python.org
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `hpy-0.9.0rc1/hpy.egg-info/SOURCES.txt` & `hpy-0.9.0rc2/hpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/microbench/README.md` & `hpy-0.9.0rc2/microbench/README.md`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/microbench/_valgrind_build.py` & `hpy-0.9.0rc2/microbench/_valgrind_build.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/microbench/conftest.py` & `hpy-0.9.0rc2/microbench/conftest.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/microbench/src/cpy_simple.c` & `hpy-0.9.0rc2/microbench/src/cpy_simple.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/microbench/src/hpy_simple.c` & `hpy-0.9.0rc2/microbench/src/hpy_simple.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/microbench/test_microbench.py` & `hpy-0.9.0rc2/microbench/test_microbench.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/proof-of-concept/pof.c` & `hpy-0.9.0rc2/proof-of-concept/pof.c`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/proof-of-concept/pofcpp.cpp` & `hpy-0.9.0rc2/proof-of-concept/pofcpp.cpp`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/proof-of-concept/pofpackage/bar.cpp` & `hpy-0.9.0rc2/proof-of-concept/pofpackage/bar.cpp`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/proof-of-concept/setup.py` & `hpy-0.9.0rc2/proof-of-concept/setup.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/proof-of-concept/test_pof.py` & `hpy-0.9.0rc2/proof-of-concept/test_pof.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/proof-of-concept/test_pof.sh` & `hpy-0.9.0rc2/proof-of-concept/test_pof.sh`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/setup.py` & `hpy-0.9.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/check_py27_compat.py` & `hpy-0.9.0rc2/test/check_py27_compat.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/conftest.py` & `hpy-0.9.0rc2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/debug/test_builder_invalid.py` & `hpy-0.9.0rc2/test/debug/test_builder_invalid.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/debug/test_charptr.py` & `hpy-0.9.0rc2/test/debug/test_charptr.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/debug/test_context_reuse.py` & `hpy-0.9.0rc2/test/debug/test_context_reuse.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/debug/test_handles_invalid.py` & `hpy-0.9.0rc2/test/debug/test_handles_invalid.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/debug/test_handles_leak.py` & `hpy-0.9.0rc2/test/debug/test_handles_leak.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/debug/test_misc.py` & `hpy-0.9.0rc2/test/debug/test_misc.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/hpy_devel/test_abitag.py` & `hpy-0.9.0rc2/test/hpy_devel/test_abitag.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/hpy_devel/test_distutils.py` & `hpy-0.9.0rc2/test/hpy_devel/test_distutils.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/support.py` & `hpy-0.9.0rc2/test/support.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_00_basic.py` & `hpy-0.9.0rc2/test/test_00_basic.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_argparse.py` & `hpy-0.9.0rc2/test/test_argparse.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_call.py` & `hpy-0.9.0rc2/test/test_call.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_capsule.py` & `hpy-0.9.0rc2/test/test_capsule.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_capsule_legacy.py` & `hpy-0.9.0rc2/test/test_capsule_legacy.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_contextvar.py` & `hpy-0.9.0rc2/test/test_contextvar.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_cpy_compat.py` & `hpy-0.9.0rc2/test/test_cpy_compat.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_eval.py` & `hpy-0.9.0rc2/test/test_eval.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_helpers.py` & `hpy-0.9.0rc2/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_hpybuildvalue.py` & `hpy-0.9.0rc2/test/test_hpybuildvalue.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_hpybytes.py` & `hpy-0.9.0rc2/test/test_hpybytes.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_hpydict.py` & `hpy-0.9.0rc2/test/test_hpydict.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_hpyerr.py` & `hpy-0.9.0rc2/test/test_hpyerr.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_hpyfield.py` & `hpy-0.9.0rc2/test/test_hpyfield.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_hpyglobal.py` & `hpy-0.9.0rc2/test/test_hpyglobal.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_hpyimport.py` & `hpy-0.9.0rc2/test/test_hpyimport.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_hpylist.py` & `hpy-0.9.0rc2/test/test_hpylist.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_hpylong.py` & `hpy-0.9.0rc2/test/test_hpylong.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_hpymodule.py` & `hpy-0.9.0rc2/test/test_hpymodule.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_hpyslice.py` & `hpy-0.9.0rc2/test/test_hpyslice.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_hpystructseq.py` & `hpy-0.9.0rc2/test/test_hpystructseq.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_hpytuple.py` & `hpy-0.9.0rc2/test/test_hpytuple.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_hpytype.py` & `hpy-0.9.0rc2/test/test_hpytype.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_hpytype_legacy.py` & `hpy-0.9.0rc2/test/test_hpytype_legacy.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_hpyunicode.py` & `hpy-0.9.0rc2/test/test_hpyunicode.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_importing.py` & `hpy-0.9.0rc2/test/test_importing.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_legacy_forbidden.py` & `hpy-0.9.0rc2/test/test_legacy_forbidden.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_number.py` & `hpy-0.9.0rc2/test/test_number.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_object.py` & `hpy-0.9.0rc2/test/test_object.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_slots.py` & `hpy-0.9.0rc2/test/test_slots.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_slots_legacy.py` & `hpy-0.9.0rc2/test/test_slots_legacy.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_support.py` & `hpy-0.9.0rc2/test/test_support.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/test_tracker.py` & `hpy-0.9.0rc2/test/test_tracker.py`

 * *Files identical despite different names*

### Comparing `hpy-0.9.0rc1/test/trace/test_trace.py` & `hpy-0.9.0rc2/test/trace/test_trace.py`

 * *Files identical despite different names*

