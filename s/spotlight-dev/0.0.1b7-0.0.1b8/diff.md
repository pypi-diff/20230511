# Comparing `tmp/spotlight-dev-0.0.1b7.tar.gz` & `tmp/spotlight-dev-0.0.1b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotlight-dev-0.0.1b7.tar", last modified: Tue May  9 20:53:26 2023, max compression
+gzip compressed data, was "spotlight-dev-0.0.1b8.tar", last modified: Thu May 11 20:26:25 2023, max compression
```

## Comparing `spotlight-dev-0.0.1b7.tar` & `spotlight-dev-0.0.1b8.tar`

### file list

```diff
@@ -1,131 +1,143 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.795951 spotlight-dev-0.0.1b7/
--rw-r--r--   0 root         (0) root         (0)     1413 2023-05-09 20:53:26.794951 spotlight-dev-0.0.1b7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      852 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 20:53:26.795951 spotlight-dev-0.0.1b7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1242 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.763949 spotlight-dev-0.0.1b7/spotlight/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.764949 spotlight-dev-0.0.1b7/spotlight/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.765949 spotlight-dev-0.0.1b7/spotlight/api/auth/
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1340 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/auth/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/auth/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1726 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/auth/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.766949 spotlight-dev-0.0.1b7/spotlight/api/job/
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/job/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/job/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2909 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/job/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/job/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2635 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/job/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.767949 spotlight-dev-0.0.1b7/spotlight/api/job/view/
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/job/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/job/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/job/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/job/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/job/view/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.768949 spotlight-dev-0.0.1b7/spotlight/api/organization/
--rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2503 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.770949 spotlight-dev-0.0.1b7/spotlight/api/organization/user/
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/user/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/user/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1876 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/user/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/user/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/user/model.py
--rw-rw-rw-   0 root         (0) root         (0)     1644 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/user/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.772950 spotlight-dev-0.0.1b7/spotlight/api/organization/view/
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      618 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/view/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.774950 spotlight-dev-0.0.1b7/spotlight/api/rule/
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/rule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/rule/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3809 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/rule/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      962 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/rule/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3434 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/rule/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.774950 spotlight-dev-0.0.1b7/spotlight/api/tag/
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1297 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/tag/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     4466 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/tag/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/tag/model.py
--rw-rw-rw-   0 root         (0) root         (0)     4008 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/tag/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.776950 spotlight-dev-0.0.1b7/spotlight/api/tag/view/
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/tag/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/tag/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/tag/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/tag/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      867 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/tag/view/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.777950 spotlight-dev-0.0.1b7/spotlight/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.779950 spotlight-dev-0.0.1b7/spotlight/core/common/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2648 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/base.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/base_enum.py
--rw-rw-rw-   0 root         (0) root         (0)     2712 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.780950 spotlight-dev-0.0.1b7/spotlight/core/common/date/
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/date/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2478 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/date/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.780950 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.781950 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/authorization/
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/authorization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/authorization/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3920 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/authorization/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3898 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/authorization/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.782950 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/data/
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/data/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/data/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1399 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/data/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/timeit.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     4794 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.783950 spotlight-dev-0.0.1b7/spotlight/core/common/metaclass/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/metaclass/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/metaclass/singleton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.784950 spotlight-dev-0.0.1b7/spotlight/core/common/requests/
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/requests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4689 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/requests/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3788 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/requests/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.784950 spotlight-dev-0.0.1b7/spotlight/core/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5958 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/decorator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.784950 spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.786951 spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/rule/
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/rule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2154 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/rule/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/rule/enum.py
--rw-rw-rw-   0 root         (0) root         (0)     1727 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/rule/sql_rule.py
--rw-rw-rw-   0 root         (0) root         (0)     3413 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.787951 spotlight-dev-0.0.1b7/spotlight/core/pipeline/model/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/model/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      282 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/model/rule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.787951 spotlight-dev-0.0.1b7/spotlight/core/pipeline/runner/
--rw-rw-rw-   0 root         (0) root         (0)     6327 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/runner/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.789951 spotlight-dev-0.0.1b7/spotlight/core/pipeline/runner/utils/
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/runner/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3573 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/runner/utils/asynchronously.py
--rw-rw-rw-   0 root         (0) root         (0)     3356 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/runner/utils/synchronously.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.790951 spotlight-dev-0.0.1b7/spotlight/pandas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/pandas/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/pandas/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     1750 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/pandas/runners.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.793951 spotlight-dev-0.0.1b7/spotlight_dev.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1413 2023-05-09 20:53:26.000000 spotlight-dev-0.0.1b7/spotlight_dev.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3859 2023-05-09 20:53:26.000000 spotlight-dev-0.0.1b7/spotlight_dev.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 20:53:26.000000 spotlight-dev-0.0.1b7/spotlight_dev.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-09 20:53:26.000000 spotlight-dev-0.0.1b7/spotlight_dev.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-09 20:53:26.000000 spotlight-dev-0.0.1b7/spotlight_dev.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.636672 spotlight-dev-0.0.1b8/
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-05-11 20:26:25.636672 spotlight-dev-0.0.1b8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      852 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 20:26:25.637672 spotlight-dev-0.0.1b8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1273 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.597669 spotlight-dev-0.0.1b8/spotlight/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.597669 spotlight-dev-0.0.1b8/spotlight/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.599669 spotlight-dev-0.0.1b8/spotlight/api/auth/
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/auth/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/auth/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/auth/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.600669 spotlight-dev-0.0.1b8/spotlight/api/job/
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/job/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/job/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2909 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/job/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/job/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2635 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/job/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.602669 spotlight-dev-0.0.1b8/spotlight/api/job/view/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/job/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/job/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/job/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/job/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/job/view/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.604669 spotlight-dev-0.0.1b8/spotlight/api/organization/
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/organization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/organization/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/organization/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/organization/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2503 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/organization/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.606670 spotlight-dev-0.0.1b8/spotlight/api/organization/user/
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/organization/user/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/organization/user/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1876 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/organization/user/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/organization/user/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/organization/user/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1644 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/organization/user/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.608670 spotlight-dev-0.0.1b8/spotlight/api/organization/view/
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/organization/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/organization/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      618 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/organization/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/organization/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/organization/view/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.610670 spotlight-dev-0.0.1b8/spotlight/api/rule/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/rule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/rule/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3809 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/rule/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/rule/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3434 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/rule/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.612670 spotlight-dev-0.0.1b8/spotlight/api/tag/
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1297 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/tag/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     4466 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/tag/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/tag/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4008 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/tag/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.614670 spotlight-dev-0.0.1b8/spotlight/api/tag/view/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/tag/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/tag/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/tag/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/tag/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      867 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/api/tag/view/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.614670 spotlight-dev-0.0.1b8/spotlight/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.617670 spotlight-dev-0.0.1b8/spotlight/core/common/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2648 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/base_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     2712 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.618671 spotlight-dev-0.0.1b8/spotlight/core/common/date/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/date/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2478 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/date/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.618671 spotlight-dev-0.0.1b8/spotlight/core/common/decorators/
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/decorators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.620671 spotlight-dev-0.0.1b8/spotlight/core/common/decorators/authorization/
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/decorators/authorization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/decorators/authorization/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3920 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/decorators/authorization/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3898 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/decorators/authorization/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.621671 spotlight-dev-0.0.1b8/spotlight/core/common/decorators/data/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/decorators/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/decorators/data/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/decorators/data/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/decorators/data/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/decorators/timeit.py
+-rw-rw-rw-   0 root         (0) root         (0)      423 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4794 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.622671 spotlight-dev-0.0.1b8/spotlight/core/common/metaclass/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/metaclass/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/metaclass/singleton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.623671 spotlight-dev-0.0.1b8/spotlight/core/common/requests/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/requests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4689 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/requests/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/requests/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/common/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.624671 spotlight-dev-0.0.1b8/spotlight/core/pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13108 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/decorator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.625671 spotlight-dev-0.0.1b8/spotlight/core/pipeline/execution/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.627671 spotlight-dev-0.0.1b8/spotlight/core/pipeline/execution/rule/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/execution/rule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2154 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/execution/rule/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/execution/rule/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/execution/rule/sql_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)     4295 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/execution/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.628671 spotlight-dev-0.0.1b8/spotlight/core/pipeline/model/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/model/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/model/rule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.628671 spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.629671 spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/batch/
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/batch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2312 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/batch/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3470 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/batch/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.630671 spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/stream/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/stream/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5877 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/stream/asynchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.631672 spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/stream/source/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/stream/source/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2039 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/stream/source/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/stream/source/decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5542 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/stream/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.632671 spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3665 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/utils/asynchronously.py
+-rw-rw-rw-   0 root         (0) root         (0)     3475 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/utils/synchronously.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.634672 spotlight-dev-0.0.1b8/spotlight/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3080 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/pandas/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/pandas/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-05-11 20:26:13.000000 spotlight-dev-0.0.1b8/spotlight/pandas/runners.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:26:25.636672 spotlight-dev-0.0.1b8/spotlight_dev.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-05-11 20:26:25.000000 spotlight-dev-0.0.1b8/spotlight_dev.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4342 2023-05-11 20:26:25.000000 spotlight-dev-0.0.1b8/spotlight_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 20:26:25.000000 spotlight-dev-0.0.1b8/spotlight_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      176 2023-05-11 20:26:25.000000 spotlight-dev-0.0.1b8/spotlight_dev.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-11 20:26:25.000000 spotlight-dev-0.0.1b8/spotlight_dev.egg-info/top_level.txt
```

### Comparing `spotlight-dev-0.0.1b7/PKG-INFO` & `spotlight-dev-0.0.1b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotlight-dev
-Version: 0.0.1b7
+Version: 0.0.1b8
 Summary: Spotlight Python SDK
 Home-page: https://alpha.dev
 Author: Spotlight
 Author-email: hello@spotlight.dev
 License: UNKNOWN
 Description: # Spotlight: The data quality platform for developers
```

### Comparing `spotlight-dev-0.0.1b7/README.md` & `spotlight-dev-0.0.1b8/README.md`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/setup.py` & `spotlight-dev-0.0.1b8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     tag = subprocess.getoutput('git tag --sort=version:refname | tail -n1')
     commits = subprocess.getoutput(f'git rev-list {tag}..HEAD --count')
     return f'{tag}.{commits}'
 
 
 setuptools.setup(
     name="spotlight-dev",
-    version="0.0.1b7",
+    version="0.0.1b8",
     author="Spotlight",
     author_email="hello@spotlight.dev",
     description="Spotlight Python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://alpha.dev",
     classifiers=[
@@ -40,10 +40,11 @@
         "pandas>=2.0.1",
         "duckdb>=0.7.1",
         "trycast>=1.0.0",
         "pydash>=7.0.3",
         "cachetools>=5.3.0",
         "pydantic>=1.10.7",
         "aiocache>=0.12.1",
-        "backoff>=2.2.1"
+        "backoff>=2.2.1",
+        "asyncstdlib>=3.10.7"
     ]
 )
```

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/auth/__util.py` & `spotlight-dev-0.0.1b8/spotlight/api/auth/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/auth/asynchronous.py` & `spotlight-dev-0.0.1b8/spotlight/api/auth/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/auth/synchronous.py` & `spotlight-dev-0.0.1b8/spotlight/api/auth/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/job/__util.py` & `spotlight-dev-0.0.1b8/spotlight/api/job/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/job/asynchronous.py` & `spotlight-dev-0.0.1b8/spotlight/api/job/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/job/model.py` & `spotlight-dev-0.0.1b8/spotlight/api/rule/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from typing import Optional, List
 
 from pydantic import Field
 
 from spotlight.core.common.base import Base
-from spotlight.core.common.enum import Status
+from spotlight.core.common.enum import Severity, ThresholdType
 
 
-class JobRequest(Base):
+class RuleRequest(Base):
     name: str
-    status: Status
-    tag_ids: Optional[List[str]] = Field(default=None)
-    start_time: Optional[int] = Field(default=None)
-    end_time: Optional[int] = Field(default=None)
-    metadata: Optional[dict] = Field(default=None)
+    predicate: str
+    description: Optional[str] = Field(default=None)
+    threshold: Optional[float] = Field(default=None)
+    threshold_type: Optional[ThresholdType] = Field(default=ThresholdType.TOTAL)
+    severity: Optional[Severity] = Field(default=Severity.ERROR)
+    sampling_fields: Optional[List[str]] = Field(default=None)
 
 
-class JobResponse(Base):
+class RuleResponse(Base):
     id: str
     name: str
-    status: Status
-    start_time: Optional[int]
-    end_time: Optional[int]
-    metadata: dict
+    description: Optional[str]
+    predicate: str
+    threshold: float
+    threshold_type: ThresholdType
+    severity: Severity
+    sampling_fields: List[str]
     created_by: str
     created_at: int
     updated_by: Optional[str]
     updated_at: Optional[int]
 
 
-class JobTagResponse(Base):
+class RuleTagResponse(Base):
     tag_id: str
     rule_id: str
     created_by: str
     created_at: int
```

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/job/synchronous.py` & `spotlight-dev-0.0.1b8/spotlight/api/job/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/job/view/asynchronous.py` & `spotlight-dev-0.0.1b8/spotlight/api/job/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/organization/__util.py` & `spotlight-dev-0.0.1b8/spotlight/api/organization/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/organization/asynchronous.py` & `spotlight-dev-0.0.1b8/spotlight/api/organization/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/organization/synchronous.py` & `spotlight-dev-0.0.1b8/spotlight/api/organization/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/organization/user/__util.py` & `spotlight-dev-0.0.1b8/spotlight/api/organization/user/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/organization/user/asynchronous.py` & `spotlight-dev-0.0.1b8/spotlight/api/organization/user/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/organization/user/model.py` & `spotlight-dev-0.0.1b8/spotlight/api/organization/user/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/organization/user/synchronous.py` & `spotlight-dev-0.0.1b8/spotlight/api/organization/user/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/organization/view/asynchronous.py` & `spotlight-dev-0.0.1b8/spotlight/api/organization/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/organization/view/synchronous.py` & `spotlight-dev-0.0.1b8/spotlight/api/organization/view/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/rule/__util.py` & `spotlight-dev-0.0.1b8/spotlight/api/rule/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/rule/asynchronous.py` & `spotlight-dev-0.0.1b8/spotlight/api/rule/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/rule/synchronous.py` & `spotlight-dev-0.0.1b8/spotlight/api/rule/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/tag/__util.py` & `spotlight-dev-0.0.1b8/spotlight/api/tag/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/tag/asynchronous.py` & `spotlight-dev-0.0.1b8/spotlight/api/tag/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/tag/synchronous.py` & `spotlight-dev-0.0.1b8/spotlight/api/tag/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/tag/view/asynchronous.py` & `spotlight-dev-0.0.1b8/spotlight/api/tag/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/api/tag/view/synchronous.py` & `spotlight-dev-0.0.1b8/spotlight/api/tag/view/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/common/base.py` & `spotlight-dev-0.0.1b8/spotlight/core/common/base.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/common/config.py` & `spotlight-dev-0.0.1b8/spotlight/core/common/config.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/common/date/function.py` & `spotlight-dev-0.0.1b8/spotlight/core/common/date/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/common/decorators/authorization/__util.py` & `spotlight-dev-0.0.1b8/spotlight/core/common/decorators/authorization/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/common/decorators/authorization/asynchronous.py` & `spotlight-dev-0.0.1b8/spotlight/core/common/decorators/authorization/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/common/decorators/authorization/synchronous.py` & `spotlight-dev-0.0.1b8/spotlight/core/common/decorators/authorization/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/common/decorators/data/__util.py` & `spotlight-dev-0.0.1b8/spotlight/core/common/decorators/data/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/common/decorators/data/asynchronous.py` & `spotlight-dev-0.0.1b8/spotlight/core/common/decorators/data/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/common/decorators/data/synchronous.py` & `spotlight-dev-0.0.1b8/spotlight/core/common/decorators/data/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/common/decorators/timeit.py` & `spotlight-dev-0.0.1b8/spotlight/core/common/decorators/timeit.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/common/errors.py` & `spotlight-dev-0.0.1b8/spotlight/core/common/errors.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/common/function.py` & `spotlight-dev-0.0.1b8/spotlight/core/common/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/common/metaclass/singleton.py` & `spotlight-dev-0.0.1b8/spotlight/core/common/metaclass/singleton.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/common/requests/asynchronous.py` & `spotlight-dev-0.0.1b8/spotlight/core/common/requests/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/common/requests/synchronous.py` & `spotlight-dev-0.0.1b8/spotlight/core/common/requests/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/pipeline/abstract.py` & `spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/stream/asynchronous.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,156 +1,148 @@
-from abc import ABC, abstractmethod
-from typing import Any, Optional, List
+import logging
+import asyncstdlib as a
+from typing import Any, List, Optional, Callable, Awaitable, Type
 
 from spotlight.api.job.model import JobResponse
-from spotlight.core.pipeline.execution.rule.abstract import AbstractRule
+from spotlight.core.common.enum import JobType, Status
+from spotlight.core.pipeline.execution.rule import AbstractRule
+from spotlight.core.pipeline.execution import ApplyRule, execute_pipeline
 from spotlight.core.pipeline.model.pipeline import PipelineResult
-from spotlight.core.pipeline.model.rule import RuleResult
-from spotlight.core.pipeline.runner import (
-    pipeline_runner,
-    async_pipeline_runner,
-    offline_pipeline_runner,
+from spotlight.core.pipeline.runner.stream.source.abstract import (
+    AbstractAsyncDataSource,
 )
+from spotlight.core.pipeline.runner.utils import async_stop_job, async_start_job
 
+logger = logging.getLogger(__name__)
 
-class AbstractPipeline(ABC):
-    @classmethod
-    @abstractmethod
-    def apply_rule(cls, data: Any, rule: AbstractRule) -> RuleResult:
-        """
-        This method applies a rule to the data provided
-
-        Args:
-            data (Any): The data associated with the plugin
-            rule (AbstractRule): The rule being run on the data
-
-        Returns:
-            RuleResult: The result of the rule run
-        """
-        pass
-
-    @classmethod
-    def run(
-        cls,
-        data: Any,
-        job_name: str,
-        *,
-        tag_names: Optional[List[str]] = None,
-        tag_ids: Optional[List[str]] = None,
-        additional_rules: Optional[List[AbstractRule]] = None,
-        metadata: Optional[dict] = None,
-        multi_processing: bool = False,
-        processes: int = 5,
-    ) -> JobResponse:
-        """
-        Runs data through the pipeline.
-
-        NOTE: You must provide the tag names and/or the tag ids for this method to run.
-        NOTE: The number of rules run in parallel is dependent on the number of processes.
-
-        Args:
-            data (Any): Data that is run through the pipeline
-            job_name (str): Name assigned to the job created from running this pipeline
-            tag_names (Optional[List[str]]): List of tag names to use with the pipeline
-            tag_ids (Optional[List[str]]): List of tag ids to use with the pipeline
-            additional_rules (List[AbstractRule]): additional rules to run on the pipeline (specifically rules that aren't
-            supported in the API i.e. AbstractCustomCodeRules)
-            metadata (Optional[dict]): Metadata added to the job information
-            multi_processing (bool): Optional flag to run the rules over the data concurrently
-            processes (int): Optional number of process to spin up when running the rules concurrently
-
-        Returns:
-            JobResponse: The job response with all the information from the run
-        """
-        return pipeline_runner(
-            data=data,
-            job_name=job_name,
-            apply_rule=cls.apply_rule,
-            tag_names=tag_names,
-            tag_ids=tag_ids,
-            additional_rules=additional_rules,
-            metadata=metadata,
-            multi_processing=multi_processing,
-            processes=processes,
-        )
-
-    @classmethod
-    async def async_run(
-        cls,
-        data: Any,
-        job_name: str,
-        *,
-        tag_names: Optional[List[str]] = None,
-        tag_ids: Optional[List[str]] = None,
-        additional_rules: Optional[List[AbstractRule]] = None,
-        metadata: Optional[dict] = None,
-        multi_processing: bool = False,
-        processes: int = 5,
-    ) -> JobResponse:
-        """
-        Asynchronously runs data through a pipeline.
-
-        NOTE: You must provide the tag names and/or the tag ids for this method to run.
-        NOTE: The number of rules run in parallel is dependent on the number of processes.
-
-        Args:
-            data (Any): Data that is run through the pipeline
-            job_name (str): Name assigned to the job created from running this pipeline
-            tag_names (Optional[List[str]]): List of tag names to use with the pipeline
-            tag_ids (Optional[List[str]]): List of tag ids to use with the pipeline
-            additional_rules (List[AbstractRule]): additional rules to run on the pipeline (specifically rules that aren't
-            supported in the API i.e. AbstractCustomCodeRules)
-            metadata (Optional[dict]): Metadata added to the job information
-            multi_processing (bool): Optional flag to run the rules over the data concurrently
-            processes (int): Optional number of process to spin up when running the rules concurrently
-
-        Returns:
-            JobResponse: The job response with all the information from the run
-        """
-        result = await async_pipeline_runner(
-            data=data,
-            job_name=job_name,
-            apply_rule=cls.apply_rule,
-            tag_names=tag_names,
-            tag_ids=tag_ids,
-            additional_rules=additional_rules,
-            metadata=metadata,
-            multi_processing=multi_processing,
-            processes=processes,
-        )
-        return result
-
-    @classmethod
-    def offline_run(
-        cls,
-        job_name: str,
-        data: Any,
-        rules: List[AbstractRule],
-        *,
-        multi_processing: bool = False,
-        processes: int = 5,
-    ) -> PipelineResult:
-        """
-        Runs data through the pipeline.
-
-        NOTE: This pipeline will run locally and the results will NOT be synced to the API making the results
-        unavailable in the UI
-        NOTE: The number of rules run in parallel is dependent on the number of processes.
-
-        Args:
-            job_name (str): Name for the test job
-            data (Any): Data that is run through the pipeline
-            rules (List[RuleRequest]): A list of the rules to run on the pipeline
-            multi_processing (bool): Optional flag to run the rules over the data concurrently
-            processes (int): Optional number of process to spin up when running the rules concurrently
-
-        Returns:
-            PipelineResult: The result of the pipeline
-        """
-        return offline_pipeline_runner(
-            job_name=job_name,
-            data=data,
-            apply_rule=cls.apply_rule,
-            rules=rules,
-            multi_processing=multi_processing,
-            processes=processes,
-        )
+
+async def __async_process_stream(
+    data_source: AbstractAsyncDataSource,
+    job_name: str,
+    apply_rule: ApplyRule,
+    rules: List[AbstractRule],
+    multi_processing: bool = False,
+    processes: int = 5,
+    on_failure: Callable[[PipelineResult], Awaitable[Any]] = lambda x: None,
+) -> List[PipelineResult]:
+    """
+    This helper asynchronously processes each message in the stream and runs it through a data pipeline
+
+     Args:
+        data_source (AbstractAsyncDataSource): Streaming data source
+        job_name (str): Name assigned to the job created from running this pipeline
+        apply_rule (ApplyRule): function for applying the rule(s) to the data provided
+        rules (List[AbstractRule]): The rules being run on the data
+        multi_processing (bool): Optional flag to run the rules over the data concurrently
+        processes (int): Optional number of process to spin up when running the rules concurrently
+        on_failure (Callable[[PipelineResult], Awaitable[Any]]): Optional function that is called when a message fails
+        thh pipeline
+
+    Returns:
+        List[PipelineResult]: All the results from each pipeline iteration ran
+    """
+    results = []
+    try:
+        async for idx, data in a.enumerate(data_source):
+            logger.debug(f"Processing message in stream {idx=}: {data}")
+            result = execute_pipeline(
+                data, job_name, apply_rule, rules, multi_processing, processes
+            )
+            results.append(result)
+            if result.status != Status.SUCCESS:
+                logger.info(f"Message failed: {idx=}")
+                logger.debug(f"Message failed {idx=}: {result}")
+                await on_failure(result)
+    finally:
+        logger.debug("Shutting down stream processor...")
+        await data_source.teardown()
+    return results
+
+
+async def async_stream_pipeline_runner(
+    data_source: AbstractAsyncDataSource,
+    job_name: str,
+    apply_rule: ApplyRule,
+    *,
+    tag_names: Optional[List[str]] = None,
+    tag_ids: Optional[List[str]] = None,
+    additional_rules: Optional[List[AbstractRule]] = None,
+    metadata: Optional[dict] = None,
+    multi_processing: bool = False,
+    processes: int = 5,
+) -> JobResponse:
+    """
+    Asynchronously processes stream messages through a pipeline
+
+    NOTE: You must provide the tag names and/or the tag ids for this method to run.
+    NOTE: The number of rules run in parallel is dependent on the number of processes.
+
+    Args:
+        data_source (AbstractAsyncDataSource): Streaming data source
+        job_name (str): Name assigned to the job created from running this pipeline
+        apply_rule (ApplyRule): function for applying the rule(s) to the data provided
+        tag_names (Optional[List[str]]): List of tag names to use with the pipeline
+        tag_ids (Optional[List[str]]): List of tag ids to use with the pipeline
+        additional_rules (List[AbstractRule]): additional rules to run on the pipeline (specifically rules that aren't
+        supported in the API i.e. AbstractCustomCodeRules)
+        metadata (Optional[dict]): Metadata added to the job information
+        multi_processing (bool): Optional flag to run the rules over the data concurrently
+        processes (int): Optional number of process to spin up when running the rules concurrently
+
+    Returns:
+        JobResponse: The job response for the stream job
+    """
+    job, rules = await async_start_job(
+        job_name=job_name,
+        tag_names=tag_names,
+        tag_ids=tag_ids,
+        job_type=JobType.STREAM,
+        metadata=metadata,
+    )
+    rules.extend(additional_rules or [])
+
+    async def on_failure(result: PipelineResult):
+        await async_stop_job(job, result)
+
+    results = await __async_process_stream(
+        data_source,
+        job.name,
+        apply_rule,
+        rules,
+        multi_processing,
+        processes,
+        on_failure,
+    )
+    return job
+
+
+async def async_offline_stream_pipeline_runner(
+    data_source: AbstractAsyncDataSource,
+    job_name: str,
+    apply_rule: ApplyRule,
+    rules: List[AbstractRule],
+    *,
+    multi_processing: bool = False,
+    processes: int = 5,
+) -> List[PipelineResult]:
+    """
+    Asynchronously streams data through a pipeline.
+
+    NOTE: This pipeline will run locally and the results will NOT be synced to the API making the results
+    unavailable in the UI
+    NOTE: The number of rules run in parallel is dependent on the number of processes.
+
+    Args:
+        data_source (AbstractAsyncDataSource): Streaming data source
+        job_name (str): Name for the test job
+        apply_rule (ApplyRule): function for applying the rule(s) to the data provided
+        rules (List[RuleRequest]): A list of the rules to run on the pipeline
+        multi_processing (bool): Optional flag to run the rules over the data concurrently
+        processes (int): Optional number of process to spin up when running the rules concurrently
+
+    Returns:
+        List[PipelineResult]: A list of all the results from each iterator of data emitted from the data source
+    """
+    results = await __async_process_stream(
+        data_source, job_name, apply_rule, rules, multi_processing, processes
+    )
+    return results
```

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/pipeline/decorator.py` & `spotlight-dev-0.0.1b8/spotlight/core/pipeline/decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import Any, Type
+from typing import Any, Type, Callable
 
 from spotlight.core.pipeline.abstract import AbstractPipeline
 from spotlight.core.pipeline.execution.rule import AbstractRule
 from spotlight.core.pipeline.execution.synchronous import ApplyRule
 from spotlight.core.pipeline.model.rule import RuleResult
 
 
 def pipeline(
     apply_rule: ApplyRule = None,
     *,
     name: str = "Unnamed",
-) -> Type[AbstractPipeline]:
+) -> Callable[[Any], Type[AbstractPipeline]]:
     """
-    This is a decorator to create a plugin from the apply method
+    This is a decorator to create a plugin from the apply_rule method
 
     Args:
         apply_rule (Callable[[Any, Any], RuleResult]): The apply rule method for a plugin
         name (str): Name of the plugin
     """
 
     def wrap(fxn):
```

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/rule/abstract.py` & `spotlight-dev-0.0.1b8/spotlight/core/pipeline/execution/rule/abstract.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/rule/sql_rule.py` & `spotlight-dev-0.0.1b8/spotlight/core/pipeline/execution/rule/sql_rule.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/pipeline/model/pipeline.py` & `spotlight-dev-0.0.1b8/spotlight/core/pipeline/model/pipeline.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/pipeline/runner/__init__.py` & `spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/stream/synchronous.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,174 +1,141 @@
 import logging
-from typing import Any, List, Optional
+from typing import Any, List, Optional, Callable, Type
 
 from spotlight.api.job.model import JobResponse
-from spotlight.core.common.date.function import current_timestamp
-from spotlight.core.pipeline.execution import execute_pipeline
+from spotlight.core.common.enum import JobType, Status
 from spotlight.core.pipeline.execution.rule import AbstractRule
-from spotlight.core.pipeline.execution.synchronous import ApplyRule
+from spotlight.core.pipeline.execution import ApplyRule, execute_pipeline
 from spotlight.core.pipeline.model.pipeline import PipelineResult
-from spotlight.core.pipeline.runner.utils import (
-    async_start_job,
-    async_stop_job,
-    start_job,
-    stop_job,
-)
+from spotlight.core.pipeline.runner.stream.source.abstract import AbstractDataSource
+from spotlight.core.pipeline.runner.utils import start_job, stop_job
 
 logger = logging.getLogger(__name__)
 
 
-def __run_pipeline(
-    data: Any,
+def __process_stream(
+    data_source: AbstractDataSource,
     job_name: str,
     apply_rule: ApplyRule,
     rules: List[AbstractRule],
     multi_processing: bool = False,
     processes: int = 5,
-):
-    start_time = current_timestamp()
-    logger.info(f"Starting data quality pipeline [{job_name=}, {start_time=}]")
-    rule_results = execute_pipeline(
-        data, rules, apply_rule, multi_processing=multi_processing, processes=processes
-    )
-    end_time = current_timestamp()
-    result = PipelineResult.build_result(job_name, start_time, end_time, rule_results)
-    logger.debug(f"Data quality pipeline result: {result}")
-    logger.info(
-        f"Data quality pipeline finished [{job_name=}, {end_time=}]: {result.status}"
-    )
-    return result
-
-
-def pipeline_runner(
-    data: Any,
-    job_name: str,
-    apply_rule: ApplyRule,
-    *,
-    tag_names: Optional[List[str]] = None,
-    tag_ids: Optional[List[str]] = None,
-    additional_rules: Optional[List[AbstractRule]] = None,
-    metadata: Optional[dict] = None,
-    multi_processing: bool = False,
-    processes: int = 5,
-) -> JobResponse:
+    on_failure: Callable[[PipelineResult], Any] = lambda x: None,
+) -> List[PipelineResult]:
     """
-    Runs data through a data quality pipeline.
+    This helper processes each message in the stream and runs it through a data pipeline
 
-    NOTE: You must provide the tag names and/or the tag ids for this method to run.
-    NOTE: The number of rules run in parallel is dependent on the number of processes.
-
-    Args:
-        data (Any): Data that is run through the pipeline
+     Args:
+        data_source (AbstractDataSource): Streaming data source
         job_name (str): Name assigned to the job created from running this pipeline
         apply_rule (ApplyRule): function for applying the rule(s) to the data provided
-        tag_names (Optional[List[str]]): List of tag names to use with the pipeline
-        tag_ids (Optional[List[str]]): List of tag ids to use with the pipeline
-        additional_rules (List[AbstractRule]): additional rules to run on the pipeline (specifically rules that aren't
-        supported in the API i.e. AbstractCustomCodeRules)
-        metadata (Optional[dict]): Metadata added to the job information
+        rules (List[AbstractRule]): The rules being run on the data
         multi_processing (bool): Optional flag to run the rules over the data concurrently
         processes (int): Optional number of process to spin up when running the rules concurrently
+        on_failure (Callable[[PipelineResult], Any]): Optional function that is called when a message fails teh pipeline
 
     Returns:
-        JobResponse: The job response with all the information from the run
+        List[PipelineResult]: All the results from each pipeline iteration ran
     """
-    job, rules = start_job(
-        job_name=job_name,
-        tag_names=tag_names,
-        tag_ids=tag_ids,
-        metadata=metadata,
-    )
-    rules.extend(additional_rules or [])
-    result = __run_pipeline(
-        data, job.name, apply_rule, rules, multi_processing, processes
-    )
-
-    job = stop_job(
-        job=job,
-        pipeline_result=result,
-    )
-    return job
+    results = []
+    try:
+        for idx, data in enumerate(data_source):
+            logger.debug(f"Processing message in stream {idx=}: {data}")
+            result = execute_pipeline(
+                data, job_name, apply_rule, rules, multi_processing, processes
+            )
+            results.append(result)
+            if result.status != Status.SUCCESS:
+                logger.info(f"Message failed: {idx=}")
+                logger.debug(f"Message failed {idx=}: {result}")
+                on_failure(result)
+    finally:
+        logger.debug("Shutting down stream processor...")
+        data_source.teardown()
+    return results
 
 
-async def async_pipeline_runner(
-    data: Any,
+def stream_pipeline_runner(
+    data_source: AbstractDataSource,
     job_name: str,
     apply_rule: ApplyRule,
     *,
     tag_names: Optional[List[str]] = None,
     tag_ids: Optional[List[str]] = None,
     additional_rules: Optional[List[AbstractRule]] = None,
     metadata: Optional[dict] = None,
     multi_processing: bool = False,
     processes: int = 5,
 ) -> JobResponse:
     """
-    Asynchronously runs data through a data quality pipeline.
+    Processes stream messages through a pipeline
 
     NOTE: You must provide the tag names and/or the tag ids for this method to run.
     NOTE: The number of rules run in parallel is dependent on the number of processes.
 
     Args:
-        data (Any): Data that is run through the pipeline
+        data_source (AbstractDataSource): Streaming data source
         job_name (str): Name assigned to the job created from running this pipeline
         apply_rule (ApplyRule): function for applying the rule(s) to the data provided
         tag_names (Optional[List[str]]): List of tag names to use with the pipeline
         tag_ids (Optional[List[str]]): List of tag ids to use with the pipeline
         additional_rules (List[AbstractRule]): additional rules to run on the pipeline (specifically rules that aren't
         supported in the API i.e. AbstractCustomCodeRules)
         metadata (Optional[dict]): Metadata added to the job information
         multi_processing (bool): Optional flag to run the rules over the data concurrently
         processes (int): Optional number of process to spin up when running the rules concurrently
 
     Returns:
-        JobResponse: The job response with all the information from the run
+        JobResponse: The job response for the stream job
     """
-    job, rules = await async_start_job(
+    job, rules = start_job(
         job_name=job_name,
         tag_names=tag_names,
         tag_ids=tag_ids,
+        job_type=JobType.STREAM,
         metadata=metadata,
     )
     rules.extend(additional_rules or [])
-    result = __run_pipeline(
-        data, job.name, apply_rule, rules, multi_processing, processes
-    )
 
-    job = await async_stop_job(
-        job=job,
-        pipeline_result=result,
+    __process_stream(
+        data_source,
+        job.name,
+        apply_rule,
+        rules,
+        multi_processing,
+        processes,
+        lambda result: stop_job(job, result),
     )
     return job
 
 
-def offline_pipeline_runner(
+def offline_stream_pipeline_runner(
+    data_source: AbstractDataSource,
     job_name: str,
-    data: Any,
     apply_rule: ApplyRule,
     rules: List[AbstractRule],
     *,
     multi_processing: bool = False,
     processes: int = 5,
-) -> PipelineResult:
+) -> List[PipelineResult]:
     """
-    Runs data through a data quality pipeline.
+    Streams data through a pipeline.
 
-    NOTE: This pipeline will run locally and the results will NOT be synced to the API making the results unavailable in
-    the UI
+    NOTE: This pipeline will run locally and the results will NOT be synced to the API making the results
+    unavailable in the UI
     NOTE: The number of rules run in parallel is dependent on the number of processes.
 
     Args:
+        data_source (AbstractDataSource): Streaming data source
         job_name (str): Name for the test job
-        data (Any): Data that is run through the pipeline
         apply_rule (ApplyRule): function for applying the rule(s) to the data provided
         rules (List[RuleRequest]): A list of the rules to run on the pipeline
         multi_processing (bool): Optional flag to run the rules over the data concurrently
         processes (int): Optional number of process to spin up when running the rules concurrently
 
     Returns:
-        PipelineResult: The result of the pipeline
+        List[PipelineResult]: A list of all the results from each iterator of data emitted from the data source
     """
-    result = __run_pipeline(
-        data, job_name, apply_rule, rules, multi_processing, processes
+    results = __process_stream(
+        data_source, job_name, apply_rule, rules, multi_processing, processes
     )
-    return result
+    return results
```

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/pipeline/runner/utils/asynchronously.py` & `spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/utils/asynchronously.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     async_create_job,
     async_update_job,
 )
 from spotlight.api.job.model import JobRequest, JobResponse
 from spotlight.api.rule.asynchronous import async_get_rules_by_tags
 from spotlight.api.rule.model import RuleResponse
 from spotlight.api.model import LookupRequest
-from spotlight.core.common.enum import Status
+from spotlight.core.common.enum import Status, JobType
 from spotlight.core.pipeline.execution.rule import SQLRule
 from spotlight.core.pipeline.model.pipeline import PipelineResult
 
 
 async def __async_get_rule_and_tag_info(
     tag_names: Optional[List[str]] = None, tag_ids: Optional[List[str]] = None
 ) -> Tuple[List[TagResponse], List[RuleResponse]]:
@@ -42,25 +42,27 @@
 
 
 async def async_start_job(
     job_name: str,
     *,
     tag_names: Optional[List[str]] = None,
     tag_ids: Optional[List[str]] = None,
+    job_type: JobType = JobType.BATCH,
     metadata: Optional[dict] = None,
 ) -> Tuple[JobResponse, List[SQLRule]]:
     """
     Asynchronously creates the job with the starting information.
 
     NOTE: You must provide the tag_name or tag_id but not both.
 
     Args:
         job_name (str): Name assigned to the job created from running this pipeline
         tag_names (Optional[List[str]]): The name of rule tags
         tag_ids (Optional[List[str]]): The id of the rule tags
+        job_type (JobType): The type of job
         metadata (Optional[dict]): Metadata added to the job information
 
     Returns:
         Tuple[JobResponse, List[Rule]]: The created job and the rules used in the job
     """
     tags, rules = await __async_get_rule_and_tag_info(
         tag_names=tag_names, tag_ids=tag_ids
```

### Comparing `spotlight-dev-0.0.1b7/spotlight/core/pipeline/runner/utils/synchronously.py` & `spotlight-dev-0.0.1b8/spotlight/core/pipeline/runner/utils/synchronously.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from spotlight.api.tag.model import TagResponse
 from spotlight.api.tag.synchronous import get_tags_by_lookup
 from spotlight.api.job import create_job, update_job
 from spotlight.api.job.model import JobRequest, JobResponse
 from spotlight.api.rule.model import RuleResponse
 from spotlight.api.model import LookupRequest
 from spotlight.api.rule.synchronous import get_rules_by_tags
-from spotlight.core.common.enum import Status
+from spotlight.core.common.enum import Status, JobType
 from spotlight.core.pipeline.execution.rule import SQLRule
 from spotlight.core.pipeline.model.pipeline import PipelineResult
 
 
 def __get_rule_and_tag_info(
     tag_names: Optional[List[str]] = None, tag_ids: Optional[List[str]] = None
 ) -> Tuple[List[TagResponse], List[RuleResponse]]:
@@ -39,32 +39,35 @@
 
 
 def start_job(
     job_name: str,
     *,
     tag_names: Optional[List[str]] = None,
     tag_ids: Optional[List[str]] = None,
+    job_type: JobType = JobType.BATCH,
     metadata: Optional[dict] = None,
 ) -> Tuple[JobResponse, List[SQLRule]]:
     """
     Creates the job with the starting information.
 
     Args:
         job_name (str): Name assigned to the job created from running this pipeline
         tag_names (Optional[List[str]]): List of tag names to use with the pipeline
         tag_ids (Optional[List[str]]): List of tag ids to use with the pipeline
+        job_type (JobType): The type of job
         metadata (Optional[dict]): Metadata added to the job information
 
     Returns:
         Tuple[JobResponse, List[Rule]]: The created job and the rules used in the job
     """
     tags, rules = __get_rule_and_tag_info(tag_names=tag_names, tag_ids=tag_ids)
     request = JobRequest(
         name=job_name,
         status=Status.IN_PROGRESS,
+        job_type=job_type,
         tag_ids=[tag.id for tag in tags],
         metadata=metadata,
     )
     response = create_job(request)
     job = JobResponse(**response)
     return job, [SQLRule.from_rule_response(rule) for rule in rules]
```

### Comparing `spotlight-dev-0.0.1b7/spotlight/pandas/__util.py` & `spotlight-dev-0.0.1b8/spotlight/pandas/__util.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,11 +91,11 @@
     """
     Helper method for extracting a sample from the failed results
     """
     fields = set(rule.sampling_fields) if rule.sampling_fields else set()
     if fields == set():
         return []
 
-    schema = list(results.columns)
+    schema = set(results.columns)
     fields = schema if fields == {"*"} else fields.intersection(set(schema))
-    sample = results[fields][:10]
+    sample = results[list(fields)][:10]
     return sample.to_dict("records")
```

### Comparing `spotlight-dev-0.0.1b7/spotlight/pandas/pipeline.py` & `spotlight-dev-0.0.1b8/spotlight/pandas/pipeline.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight/pandas/runners.py` & `spotlight-dev-0.0.1b8/spotlight/pandas/runners.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b7/spotlight_dev.egg-info/PKG-INFO` & `spotlight-dev-0.0.1b8/spotlight_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotlight-dev
-Version: 0.0.1b7
+Version: 0.0.1b8
 Summary: Spotlight Python SDK
 Home-page: https://alpha.dev
 Author: Spotlight
 Author-email: hello@spotlight.dev
 License: UNKNOWN
 Description: # Spotlight: The data quality platform for developers
```

### Comparing `spotlight-dev-0.0.1b7/spotlight_dev.egg-info/SOURCES.txt` & `spotlight-dev-0.0.1b8/spotlight_dev.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -83,14 +83,23 @@
 spotlight/core/pipeline/execution/rule/abstract.py
 spotlight/core/pipeline/execution/rule/enum.py
 spotlight/core/pipeline/execution/rule/sql_rule.py
 spotlight/core/pipeline/model/__init__.py
 spotlight/core/pipeline/model/pipeline.py
 spotlight/core/pipeline/model/rule.py
 spotlight/core/pipeline/runner/__init__.py
+spotlight/core/pipeline/runner/batch/__init__.py
+spotlight/core/pipeline/runner/batch/asynchronous.py
+spotlight/core/pipeline/runner/batch/synchronous.py
+spotlight/core/pipeline/runner/stream/__init__.py
+spotlight/core/pipeline/runner/stream/asynchronous.py
+spotlight/core/pipeline/runner/stream/synchronous.py
+spotlight/core/pipeline/runner/stream/source/__init__.py
+spotlight/core/pipeline/runner/stream/source/abstract.py
+spotlight/core/pipeline/runner/stream/source/decorator.py
 spotlight/core/pipeline/runner/utils/__init__.py
 spotlight/core/pipeline/runner/utils/asynchronously.py
 spotlight/core/pipeline/runner/utils/synchronously.py
 spotlight/pandas/__init__.py
 spotlight/pandas/__util.py
 spotlight/pandas/pipeline.py
 spotlight/pandas/runners.py
```

