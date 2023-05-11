# Comparing `tmp/sarus_data_spec_public-3.2.1.dev2.tar.gz` & `tmp/sarus_data_spec_public-3.2.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus_data_spec_public-3.2.1.dev2.tar", last modified: Tue May  9 08:13:15 2023, max compression
+gzip compressed data, was "sarus_data_spec_public-3.2.1.dev3.tar", last modified: Thu May 11 13:08:16 2023, max compression
```

## Comparing `sarus_data_spec_public-3.2.1.dev2.tar` & `sarus_data_spec_public-3.2.1.dev3.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.868536 sarus_data_spec_public-3.2.1.dev2/
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      436 2023-05-09 08:13:15.868536 sarus_data_spec_public-3.2.1.dev2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.811532 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/
--rwxrwxrwx   0 root         (0) root         (0)      830 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.813532 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5582 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/admin_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/array.py
--rw-rw-rw-   0 root         (0) root         (0)     3172 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/pandas_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6260 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    10408 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/type.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/attribute.py
--rw-rw-rw-   0 root         (0) root         (0)     4618 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1488 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.814532 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/config/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1727 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/config/privacy_properties.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3622 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.815532 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/context/
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/context/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/context/public.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/context/state.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/context/typing.py
--rw-rw-rw-   0 root         (0) root         (0)    18711 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.817532 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_rewriter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_rewriter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_rewriter/base.py
--rw-rw-rw-   0 root         (0) root         (0)    13030 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_rewriter/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_rewriter/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.819532 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11044 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3882 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/parameter_kind.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/privacy_limit.py
--rw-rw-rw-   0 root         (0) root         (0)    19230 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/signature.py
--rw-rw-rw-   0 root         (0) root         (0)     2710 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     4492 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     8849 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8679 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/json_serialisation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.821533 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7230 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/async_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    28802 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.821533 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8823 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.823533 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/local/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/local/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2172 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/local/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.823533 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/remote/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/remote/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3302 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/remote/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.824533 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3640 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.825533 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.829533 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11465 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/external_op.py
--rw-rw-rw-   0 root         (0) root         (0)     3047 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/imblearn.py
--rw-rw-rw-   0 root         (0) root         (0)     7943 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.830533 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas/
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    73352 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
--rw-rw-rw-   0 root         (0) root         (0)    26225 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
--rw-rw-rw-   0 root         (0) root         (0)     2819 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.835533 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21085 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
--rw-rw-rw-   0 root         (0) root         (0)     1914 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
--rw-rw-rw-   0 root         (0) root         (0)    38861 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
--rw-rw-rw-   0 root         (0) root         (0)     2096 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
--rw-rw-rw-   0 root         (0) root         (0)     6920 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
--rw-rw-rw-   0 root         (0) root         (0)    12822 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     6057 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     4382 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     2657 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
--rw-rw-rw-   0 root         (0) root         (0)     2896 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/skopt.py
--rw-rw-rw-   0 root         (0) root         (0)    18360 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/std.py
--rw-rw-rw-   0 root         (0) root         (0)     2716 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6107 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/xgboost.py
--rw-rw-rw-   0 root         (0) root         (0)    10560 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.840534 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14040 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/extract.py
--rw-rw-rw-   0 root         (0) root         (0)    11996 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/filter.py
--rw-rw-rw-   0 root         (0) root         (0)    11180 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/get_item.py
--rw-rw-rw-   0 root         (0) root         (0)    11214 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/project.py
--rw-rw-rw-   0 root         (0) root         (0)     6820 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/sample.py
--rw-rw-rw-   0 root         (0) root         (0)     4290 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/select_sql.py
--rw-rw-rw-   0 root         (0) root         (0)     2480 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/shuffle.py
--rw-rw-rw-   0 root         (0) root         (0)    10320 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/standard_op.py
--rw-rw-rw-   0 root         (0) root         (0)    11292 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/synthetic.py
--rw-rw-rw-   0 root         (0) root         (0)    27153 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.841534 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/source/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/source/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/source/privacy_params.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/source/random_seed.py
--rw-rw-rw-   0 root         (0) root         (0)     2596 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/source/routing.py
--rw-rw-rw-   0 root         (0) root         (0)    10235 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/marginals.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/multiplicity.py
--rw-rw-rw-   0 root         (0) root         (0)     3127 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/path.py
--rw-rw-rw-   0 root         (0) root         (0)     3004 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/predicate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.864535 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/
--rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/attribute.proto
--rw-r--r--   0 root         (0) root         (0)     5552 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/attribute_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/attribute_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/bounds.proto
--rw-r--r--   0 root         (0) root         (0)     6306 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/bounds_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/bounds_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/constraint.proto
--rw-r--r--   0 root         (0) root         (0)     8070 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/constraint_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/constraint_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1233 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/dataset.proto
--rw-r--r--   0 root         (0) root         (0)    24833 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/dataset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8880 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/dataset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/links.proto
--rw-r--r--   0 root         (0) root         (0)    11282 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/links_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4193 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/links_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/manager.proto
--rw-r--r--   0 root         (0) root         (0)     4572 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/manager_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/manager_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/marginals.proto
--rw-r--r--   0 root         (0) root         (0)     6408 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/marginals_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2177 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/marginals_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/multiplicity.proto
--rw-r--r--   0 root         (0) root         (0)     6521 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/multiplicity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2186 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/multiplicity_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/path.proto
--rw-r--r--   0 root         (0) root         (0)     4998 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/path_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/path_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/predicate.proto
--rw-r--r--   0 root         (0) root         (0)    13369 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/predicate_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4859 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/predicate_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/proto_container.proto
--rw-r--r--   0 root         (0) root         (0)     5086 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/proto_container_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/proto_container_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/relation.proto
--rw-r--r--   0 root         (0) root         (0)     5982 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/relation_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/relation_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3044 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/scalar.proto
--rw-r--r--   0 root         (0) root         (0)    32882 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/scalar_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14459 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/scalar_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/schema.proto
--rw-r--r--   0 root         (0) root         (0)    12546 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/schema_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/schema_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/size.proto
--rw-r--r--   0 root         (0) root         (0)     6233 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/size_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2162 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/size_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3909 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/statistics.proto
--rw-r--r--   0 root         (0) root         (0)    91981 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/statistics_pb2.py
--rw-r--r--   0 root         (0) root         (0)    32903 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/statistics_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/status.proto
--rw-r--r--   0 root         (0) root         (0)    18816 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     5640 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/transform.proto
--rw-r--r--   0 root         (0) root         (0)   107770 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/transform_pb2.py
--rw-r--r--   0 root         (0) root         (0)    38135 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/transform_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4567 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/type.proto
--rw-r--r--   0 root         (0) root         (0)    74241 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/type_pb2.py
--rw-r--r--   0 root         (0) root         (0)    29134 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/type_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3914 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/utilities.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    10599 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/scalar.py
--rw-rw-rw-   0 root         (0) root         (0)     4555 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1467 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/size.py
--rw-rw-rw-   0 root         (0) root         (0)    43542 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)    16850 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.865536 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11812 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/storage/local.py
--rw-rw-rw-   0 root         (0) root         (0)     5153 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/storage/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3078 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/storage/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    31051 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/transform.py
--rw-rw-rw-   0 root         (0) root         (0)   136116 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/type.py
--rw-rw-rw-   0 root         (0) root         (0)    35669 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3983 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/variant_constraint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.868536 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec_public.egg-info/
--rw-r--r--   0 root         (0) root         (0)      436 2023-05-09 08:13:15.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec_public.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7837 2023-05-09 08:13:15.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec_public.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 08:13:15.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec_public.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 08:13:15.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec_public.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-09 08:13:15.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec_public.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-09 08:13:15.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec_public.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     5833 2023-05-09 08:13:15.869536 sarus_data_spec_public-3.2.1.dev2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1191 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.372045 sarus_data_spec_public-3.2.1.dev3/
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      436 2023-05-11 13:08:16.372045 sarus_data_spec_public-3.2.1.dev3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.318041 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/
+-rwxrwxrwx   0 root         (0) root         (0)      830 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.320042 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/arrow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5679 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/arrow/admin_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/arrow/array.py
+-rw-rw-rw-   0 root         (0) root         (0)     3172 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/arrow/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/arrow/pandas_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6260 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/arrow/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    10408 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/arrow/type.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)     4618 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.321042 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/config/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/config/privacy_properties.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3712 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.322042 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/context/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/context/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/context/public.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/context/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/context/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    18711 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.324042 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_rewriter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_rewriter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_rewriter/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    13030 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_rewriter/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_rewriter/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.326042 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_validator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_validator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11237 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_validator/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3882 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_validator/parameter_kind.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_validator/privacy_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)    20331 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_validator/signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     2710 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_validator/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4492 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_validator/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8849 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/deprecation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8679 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/json_serialisation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.328042 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7230 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/async_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    29039 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.328042 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/computations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/computations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8793 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/computations/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.329042 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/computations/local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/computations/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/computations/local/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2311 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/computations/local/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.330042 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/computations/remote/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/computations/remote/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/computations/remote/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.331042 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3640 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.332042 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.335043 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11451 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/external_op.py
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/imblearn.py
+-rw-rw-rw-   0 root         (0) root         (0)     7943 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.336043 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    73380 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
+-rw-rw-rw-   0 root         (0) root         (0)    26225 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2819 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.341043 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21085 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
+-rw-rw-rw-   0 root         (0) root         (0)     1914 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
+-rw-rw-rw-   0 root         (0) root         (0)    38717 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2096 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
+-rw-rw-rw-   0 root         (0) root         (0)     6920 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    12822 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     6057 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4382 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2896 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/skopt.py
+-rw-rw-rw-   0 root         (0) root         (0)    18437 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/std.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6107 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/xgboost.py
+-rw-rw-rw-   0 root         (0) root         (0)    10560 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.346043 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14040 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/extract.py
+-rw-rw-rw-   0 root         (0) root         (0)    11996 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11180 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/get_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    11214 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     6820 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     4290 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/select_sql.py
+-rw-rw-rw-   0 root         (0) root         (0)     2480 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/shuffle.py
+-rw-rw-rw-   0 root         (0) root         (0)    10332 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/standard_op.py
+-rw-rw-rw-   0 root         (0) root         (0)    11292 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/synthetic.py
+-rw-rw-rw-   0 root         (0) root         (0)    27153 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.347043 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/source/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/source/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/source/privacy_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/source/random_seed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2596 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/source/routing.py
+-rw-rw-rw-   0 root         (0) root         (0)    10235 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/marginals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/multiplicity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3580 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/predicate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.369045 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/attribute.proto
+-rw-r--r--   0 root         (0) root         (0)     5552 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/attribute_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/attribute_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/bounds.proto
+-rw-r--r--   0 root         (0) root         (0)     6306 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/bounds_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/bounds_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/constraint.proto
+-rw-r--r--   0 root         (0) root         (0)     8070 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/constraint_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/constraint_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/dataset.proto
+-rw-r--r--   0 root         (0) root         (0)    24833 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/dataset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8880 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/dataset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/links.proto
+-rw-r--r--   0 root         (0) root         (0)    11282 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/links_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4193 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/links_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/manager.proto
+-rw-r--r--   0 root         (0) root         (0)     4572 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/manager_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/manager_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/marginals.proto
+-rw-r--r--   0 root         (0) root         (0)     6408 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/marginals_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2177 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/marginals_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/multiplicity.proto
+-rw-r--r--   0 root         (0) root         (0)     6521 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/multiplicity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/multiplicity_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/path.proto
+-rw-r--r--   0 root         (0) root         (0)     4998 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/path_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/path_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/predicate.proto
+-rw-r--r--   0 root         (0) root         (0)    13369 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/predicate_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4859 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/predicate_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/proto_container.proto
+-rw-r--r--   0 root         (0) root         (0)     5086 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/proto_container_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/proto_container_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/relation.proto
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/relation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/relation_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3044 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/scalar.proto
+-rw-r--r--   0 root         (0) root         (0)    32882 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/scalar_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14459 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/scalar_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/schema.proto
+-rw-r--r--   0 root         (0) root         (0)    12546 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/schema_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/schema_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/size.proto
+-rw-r--r--   0 root         (0) root         (0)     6233 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/size_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/size_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3909 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/statistics.proto
+-rw-r--r--   0 root         (0) root         (0)    91981 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/statistics_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    32903 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/statistics_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/status.proto
+-rw-r--r--   0 root         (0) root         (0)    18816 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     5640 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/transform.proto
+-rw-r--r--   0 root         (0) root         (0)   107770 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/transform_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    38135 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/transform_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4567 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/type.proto
+-rw-r--r--   0 root         (0) root         (0)    74241 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/type_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    29134 2023-05-11 13:08:05.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/type_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3914 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/utilities.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    10599 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/scalar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4555 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/size.py
+-rw-rw-rw-   0 root         (0) root         (0)    43542 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)    16850 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.370045 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11812 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/storage/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     5153 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/storage/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3078 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/storage/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    31051 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)   136116 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/type.py
+-rw-rw-rw-   0 root         (0) root         (0)    35688 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4107 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/variant_constraint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:08:16.372045 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec_public.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      436 2023-05-11 13:08:16.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec_public.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7837 2023-05-11 13:08:16.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec_public.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 13:08:16.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec_public.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 13:08:16.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec_public.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-11 13:08:16.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec_public.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-11 13:08:16.000000 sarus_data_spec_public-3.2.1.dev3/sarus_data_spec_public.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5833 2023-05-11 13:08:16.373045 sarus_data_spec_public-3.2.1.dev3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1191 2023-05-11 13:07:53.000000 sarus_data_spec_public-3.2.1.dev3/setup.py
```

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/__init__.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sarus_data_spec.transform import Transform
 from sarus_data_spec.variant_constraint import VariantConstraint
 
 """A library to manage Sarus datasets"""
 # pylint: disable=unused-variable
 
 PACKAGE_NAME: Final[str] = 'sarus_data_spec'
-VERSION: Final[str] = '3.2.1.dev2'
+VERSION: Final[str] = '3.2.1.dev3'
 
 try:
     import sarus_data_spec.context.worker as sw
 
     push_global_context(sw.WorkerContext())
 except ModuleNotFoundError as exception:
     if exception.name == 'sarus_data_spec.context.worker':
```

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/admin_utils.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/arrow/admin_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,14 +141,17 @@
 
 
 def validate_admin_data(
     admin_data: t.List[pa.Table],
 ) -> pa.Table:
     """Check that all admin data are equal."""
     # If we reach this part then there should be only one input admin data
+    if len(admin_data) == 0:
+        raise ValueError("The list of input admin data is empty.")
+
     pe = next(iter(admin_data), None)
     if pe is None:
         raise ValueError(
             "The dataset was infered PEP but has no input admin data"
         )
 
     if not all([candidate.equals(pe) for candidate in admin_data]):
```

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/array.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/arrow/array.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/conversion.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/arrow/conversion.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/pandas_utils.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/arrow/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/schema.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/arrow/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/type.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/arrow/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/attribute.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/attribute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/base.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/bounds.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/bounds.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/config/privacy_properties.yaml` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/config/privacy_properties.yaml`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/constants.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -100,14 +100,16 @@
 QB_TASK = 'query_builder'
 LINKS_TASK = 'links_statistics'
 SYNTHETIC_TASK = 'synthetic'
 
 
 # Privacy
 PEP_TOKEN = "pep_token"
+NO_TOKEN = "no_token"
+IS_PUBLIC = "is_public"
 PRIVACY_LIMIT = "privacy_limit"
 CONSTRAINT_KIND = "constraint_kind"
 BEST_ALTERNATIVE = "best_alternative"
 
 # QUERYBUILDER
 QUERIES = 'queries'
 
@@ -136,12 +138,13 @@
     "mssql": st.SQLDialect.SQL_SERVER,
     "mysql": st.SQLDialect.MY_SQL,
     "sqlite": st.SQLDialect.SQLLITE,
     "oracle": st.SQLDialect.ORACLE,
     "bigquery": st.SQLDialect.BIG_QUERY,
     "redshift": st.SQLDialect.REDSHIFT,
     "hive": st.SQLDialect.HIVE,
+    "databricks": st.SQLDialect.DATABRICKS,
 }
 
 # Possible values
 POSSIBLE_VALUES_LENGTH = 'possible_values_length'
 POSSIBLE_VALUES = 'possible_values'
```

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/context/public.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/context/public.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/context/typing.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/context/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataset.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_rewriter/base.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_rewriter/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_rewriter/simple_rules.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_rewriter/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_rewriter/typing.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_rewriter/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/base.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_validator/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from __future__ import annotations
 
 from typing import Collection, List, Optional, cast
 import json
 import logging
 
 from sarus_data_spec.attribute import attach_properties
-from sarus_data_spec.constants import PEP_TOKEN, PRIVATE_QUERY
+from sarus_data_spec.constants import (
+    IS_PUBLIC,
+    NO_TOKEN,
+    PEP_TOKEN,
+    PRIVATE_QUERY,
+)
 from sarus_data_spec.dataspec_validator.privacy_limit import DeltaEpsilonLimit
 from sarus_data_spec.manager.async_utils import sync
 from sarus_data_spec.manager.ops.processor import routing
 from sarus_data_spec.protobuf.utilities import dejson
 from sarus_data_spec.protobuf.utilities import json as proto_to_json
 from sarus_data_spec.storage.typing import Storage
 from sarus_data_spec.variant_constraint import (
@@ -162,15 +167,15 @@
         public_context: Collection[str] = []
         privacy_limit = DeltaEpsilonLimit({0.0: 0.0})
         kind = st.ConstraintKind.PUBLIC
 
         # Does any saved constraint yet verifies that the Dataspec is public
         for constraint in self.verified_constraints(dataspec):
             if self.verifies(constraint, kind, public_context, privacy_limit):
-                return True
+                return constraint.properties()[IS_PUBLIC] == str(True)
 
         # Determine is the Dataspec is public
         if dataspec.is_transformed():
             # Returns true if the DataSpec derives only from public
             args_parents, kwargs_parents = dataspec.parents()
             is_public = all(
                 [self.is_public(ds) for ds in args_parents]
@@ -184,16 +189,15 @@
                 or scalar.is_synthetic_model()
             )
             is_public = True
         else:
             is_public = False
 
         # save variant constraint
-        if is_public:
-            public_constraint(dataspec)
+        public_constraint(dataspec, is_public)
 
         return is_public
 
     def pep_token(self, dataspec: st.DataSpec) -> Optional[str]:
         """Return a token if the dataspec is PEP, otherwise return None.
 
         DataSpec.pep_token() returns a PEP token if the dataset is PEP and None
@@ -220,32 +224,35 @@
         public_context: Collection[str] = []
         privacy_limit = DeltaEpsilonLimit({0.0: 0.0})
         kind = st.ConstraintKind.PEP
 
         # Does any constraint yet verifies that the Dataset is PEP
         for constraint in self.verified_constraints(dataset):
             if self.verifies(constraint, kind, public_context, privacy_limit):
-                return constraint.properties()[PEP_TOKEN]
+                stored_token = constraint.properties()[PEP_TOKEN]
+                return None if stored_token == NO_TOKEN else stored_token
 
         # Compute the PEP token
         if not dataset.is_transformed():
             return None
 
         transform = dataset.transform()
         _, StaticChecker = routing.get_dataset_op(transform)
         pep_token = StaticChecker(dataset).pep_token(public_context)
-        if pep_token is not None:
-            pep_constraint(
-                dataspec=dataset,
-                token=pep_token,
-                required_context=[],
-                privacy_limit=privacy_limit,
-            )
+        if pep_token is None:
+            pep_token = NO_TOKEN
+
+        pep_constraint(
+            dataspec=dataset,
+            token=pep_token,
+            required_context=[],
+            privacy_limit=privacy_limit,
+        )
 
-        return pep_token
+        return None if pep_token == NO_TOKEN else pep_token
 
     def private_queries(self, dataspec: st.DataSpec) -> List[st.PrivateQuery]:
         """Return the list of PrivateQueries used in a Dataspec's transform.
 
         It represents the privacy loss associated with the current computation.
 
         It can be used by Sarus when a user (Access object) reads a DP dataspec
```

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/parameter_kind.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_validator/parameter_kind.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/privacy_limit.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_validator/privacy_limit.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/signature.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_validator/signature.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
 from enum import Enum, auto
+import logging
+import time
 import typing as t
 
 import pyarrow as pa
 
 from sarus_data_spec.arrow.admin_utils import (
     async_admin_data,
     validate_admin_data,
@@ -20,14 +22,16 @@
 )
 from sarus_data_spec.manager.ops.processor.external.utils import (
     static_arguments,
 )
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 
+logger = logging.getLogger(__name__)
+
 
 class DefautValue(Enum):
     NO_DEFAULT = auto()
 
 
 class SarusParameter:
     def __init__(
@@ -94,24 +98,28 @@
             predicate=predicate,
         )
 
 
 class SarusSignature:
     """A Signature is a list of Parameters."""
 
-    def __init__(self, *parameters: SarusParameter):
+    def __init__(self, *parameters: SarusParameter, name: str = ""):
         self._parameters = list(parameters)
         self._parameter_map = {param.name: param for param in parameters}
+        self._name = name
 
     def parameters(self) -> t.List[SarusParameter]:
         return self._parameters
 
     def __getitem__(self, name: str) -> SarusParameter:
         return self._parameter_map[name]
 
+    def name(self) -> str:
+        return self._name
+
     def _bind_external(
         self,
         transform: st.Transform,
         *ds_args: st.DataSpec,
         **ds_kwargs: st.DataSpec,
     ) -> SarusBoundSignature:
         # Deserialize arguments
@@ -233,15 +241,15 @@
         # reorder arguments
         if not has_param_array and not has_param_mapping:
             arg_map = {arg.name(): arg for arg in bound_arguments}
             bound_arguments = [
                 arg_map[param.name] for param in self.parameters()
             ]
 
-        return SarusBoundSignature(bound_arguments)
+        return SarusBoundSignature(bound_arguments, name=self.name())
 
     def bind_dataspec(self, dataspec: st.DataSpec) -> SarusBoundSignature:
         if not dataspec.is_transformed():
             raise ValueError("Cannot bind a non transformed dataspec.")
 
         transform = dataspec.transform()
         ds_args, ds_kwargs = dataspec.parents()
@@ -312,14 +320,17 @@
         self._value = value
         self.kind = kind
         self.positional_only = positional_only
 
     def name(self) -> str:
         return self.parameter.name
 
+    def __repr__(self) -> str:
+        return f"<BoundArgument {self.name()} {repr(self.static_value())}>"
+
     def static_value(self) -> t.Any:
         return self._value
 
     def python_type(self) -> t.Optional[str]:
         return self.kind
 
     def parameter_kind(self) -> ParameterCondition:
@@ -407,35 +418,53 @@
             return self.static_value()
 
     async def admin_data(self) -> t.Optional[pa.Table]:
         if not self.is_pep():
             return None
 
         dataset = t.cast(st.Dataset, self.static_value())
-        return await async_admin_data(dataset)
+        admin_data = await async_admin_data(dataset)
+        if admin_data is None:
+            raise ValueError(
+                f"The dataset {dataset.uuid()} was"
+                " inferred PEP but has no admin data."
+            )
+        return admin_data
 
 
 class SarusBoundSignature:
     """A BoundSignature is a list of BoundArguments."""
 
-    def __init__(self, arguments: t.List[SarusBoundArgument]):
+    def __init__(self, arguments: t.List[SarusBoundArgument], name: str):
         self.arguments = arguments
         self._argument_map = {arg.name(): arg for arg in self.arguments}
-        self.static_validation()
+        self._name = name
+
+    def name(self) -> str:
+        return self._name
+
+    def __repr__(self) -> str:
+        return (
+            f"{self.name()}"
+            f"({', '.join([arg.name() for arg in self.arguments])})"
+        )
 
     def is_dp(self) -> bool:
         return "budget" in self._argument_map and "seed" in self._argument_map
 
     def __getitem__(self, name: str) -> SarusBoundArgument:
         return self._argument_map[name]
 
     def static_validation(self) -> None:
         """Check that the arguments have the correct dataspec type."""
+        start = time.perf_counter()
         for arg in self.arguments:
             arg.static_validation()
+        end = time.perf_counter()
+        logger.debug(f"STATIC VALIDATION {self} ({end-start:.2f}s)")
 
     async def dynamic_validation(self) -> None:
         """Compare the values with the annotations.
 
         TODO: Not used yet. Annotations needs to be curated to
         remove ForwardRefs.
         """
@@ -530,27 +559,37 @@
             have the same token
         """
         if not all(
             [arg.is_public() or arg.is_pep() for arg in self.arguments]
         ):
             return None
 
-        tokens = [arg.pep_token() for arg in self.arguments]
-        unique_tokens = set([token for token in tokens if token is not None])
+        pep_args = [arg for arg in self.arguments if arg.is_pep()]
+        if len(pep_args) == 0:
+            return None
+
+        tokens = [arg.pep_token() for arg in pep_args]
+        unique_tokens = set(tokens)
         if len(unique_tokens) != 1:
             return None
         else:
             return unique_tokens.pop()
 
     async def admin_data(self) -> pa.Table:
         """Return the admin data of the inputs."""
-        protected_entities = [
+        admin_data = [
             await arg.admin_data() for arg in self.arguments if arg.is_pep()
         ]
-        return validate_admin_data(protected_entities)
+        if len(admin_data) == 0:
+            raise ValueError(
+                "The list of input admin data is empty "
+                f"among arguments {self.arguments}"
+            )
+
+        return validate_admin_data(admin_data)
 
 
 def extended_is_instance(obj: t.Any, kind: t.Type) -> bool:
     """Extended version of isinstance that also checks composite types."""
     if t.get_origin(kind) is None:
         if isinstance(kind, t.ForwardRef):
             return False
```

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/simple_rules.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_validator/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/typing.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/dataspec_validator/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/deprecation.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/deprecation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/factory.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/factory.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/json_serialisation.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/json_serialisation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/async_utils.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/async_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/base.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from uuid import UUID
 import asyncio
 import hashlib
 import logging
 import os
+import time
 import typing as t
 import warnings
 
 import pandas as pd
 import pyarrow as pa
 
 from sarus_data_spec.arrow.admin_utils import async_to_arrow_extract_data_only
@@ -32,14 +33,15 @@
 )
 from sarus_data_spec.manager.typing import Computation
 from sarus_data_spec.protobuf.utilities import copy
 from sarus_data_spec.protobuf.utilities import json as utilities_json
 from sarus_data_spec.scalar import Scalar
 from sarus_data_spec.schema import Schema
 from sarus_data_spec.status import error_aggregation
+from sarus_data_spec.transform import transform_id
 import sarus_data_spec.dataspec_rewriter.typing as sdrt
 import sarus_data_spec.dataspec_validator.typing as sdvt
 import sarus_data_spec.manager.typing as manager_typing
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.status as stt
 import sarus_data_spec.storage.typing as storage_typing
 import sarus_data_spec.typing as st
@@ -634,14 +636,15 @@
         transform: st.Transform,
         *arguments: st.DataSpec,
         **named_arguments: st.DataSpec,
     ) -> t.Any:
         """Compute the mock value of an external transform applied on
         Dataspecs.
         """
+        start = time.perf_counter()
         assert transform.is_external()
         mock_args = [arg.variant(st.ConstraintKind.MOCK) for arg in arguments]
         named_mock_args = {
             name: arg.variant(st.ConstraintKind.MOCK)
             for name, arg in named_arguments.items()
         }
 
@@ -664,14 +667,19 @@
                 async_compute_external_value(
                     transform, *typed_mock_args, **typed_named_mock_args
                 )
             )
         except Exception as e:
             raise e
 
+        end = time.perf_counter()
+        logger.debug(
+            f"MOCK VALUE {transform_id(transform)} ({end-start:.2f}s)"
+        )
+
         return mock_value
 
     async def async_value_op(self, scalar: st.Scalar) -> t.Any:
         raise NotImplementedError
 
     async def async_to_arrow_op(
         self, dataset: st.Dataset, batch_size: int
```

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/base.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/computations/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,18 +186,17 @@
         status with relaunch=true exists. it creates
         a new status without the task in question
         and calls launch task"""
         status = self.status(dataspec=dataspec)
         if status is not None:
             stage = status.task(self.task_name)
             assert stage
-            should_clear = status_error_policy(stage=stage)
-            if should_clear:
+            if stage.error() and status_error_policy(stage=stage):
                 status.clear_task(self.task_name)
-                self.launch_task(dataspec=dataspec)
+        self.launch_task(dataspec=dataspec)
 
 
 class ErrorCatchingAsyncIterator:
     """Wrap an AsyncIterator and catches potential errors.
 
     When an error occurs, this sets the Dataspec status to error
     accordingly.
```

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/local/base.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/computations/local/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/local/schema.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/computations/local/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import time
 import traceback
 import typing as t
 
 from sarus_data_spec import typing as st
 from sarus_data_spec.constants import SCHEMA_TASK
 from sarus_data_spec.dataset import Dataset
 from sarus_data_spec.manager.computations.local.base import LocalComputation
@@ -16,14 +17,15 @@
     """Class responsible to compute schemas"""
 
     task_name = SCHEMA_TASK
 
     async def prepare(self, dataspec: st.DataSpec) -> None:
         try:
             logger.debug(f'STARTED SCHEMA {dataspec.uuid()}')
+            start = time.perf_counter()
             schema = await self.computing_manager().async_schema_op(
                 dataset=t.cast(Dataset, dataspec)
             )
 
         except DataSpecErrorStatus as exception:
             error(
                 dataspec=dataspec,
@@ -43,15 +45,18 @@
                 properties={
                     "message": traceback.format_exc(),
                     'relaunch': str(False),
                 },
             )
             raise DataSpecErrorStatus((False, traceback.format_exc()))
         else:
-            logger.debug(f'FINISHED SCHEMA {dataspec.uuid()}')
+            end = time.perf_counter()
+            logger.debug(
+                f'FINISHED SCHEMA {dataspec.uuid()} ({end-start:.2f}s)'
+            )
             ready(
                 dataspec=dataspec,
                 manager=self.computing_manager(),
                 task=self.task_name,
                 properties={'uuid': schema.uuid()},
             )
```

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/remote/base.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/computations/remote/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/base.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/__init__.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/external_op.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/external_op.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         self, batch_size: int
     ) -> t.AsyncIterator[pa.RecordBatch]:
         transform = self.dataset.transform()
         implementation = external_implementation(transform)
         bound_signature = implementation.signature().bind_dataspec(
             self.dataset
         )
-        await bound_signature.dynamic_validation()
+        bound_signature.static_validation()
 
         if self.dataset.is_pep():
             result = await implementation.call(bound_signature)
             ds_result = t.cast(st.DatasetCastable, result)
             admin_data = await bound_signature.admin_data()
             output_admin_data = compute_admin_data(admin_data, ds_result)
             data_table = to_pyarrow_table(ds_result)
@@ -203,15 +203,15 @@
       - for computing a Mock value and inferring if the result is
         a Scalar or a Dataset.
     """
     implementation = external_implementation(transform)
     bound_signature = implementation.signature().bind(
         transform, *ds_args, **ds_kwargs
     )
-    await bound_signature.dynamic_validation()
+    bound_signature.static_validation()
 
     if implementation.is_dp(bound_signature):
         data = await implementation.call(bound_signature)
 
     else:
         data = await implementation.call(bound_signature)
```

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/imblearn.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/imblearn.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/numpy.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/numpy.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py`

 * *Files 0% similar despite different names*

```diff
@@ -892,14 +892,15 @@
             default=False,
         ),
         SarusParameter(
             name="method",
             annotation=Literal['pad', 'ffill', 'bfill'],
             default=lib.no_default,
         ),
+        name=_transform_id,
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
         this, kwargs = await signature.collect_kwargs_method()
         return this.replace(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
```

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,19 +56,14 @@
             default="SAMME.R",
         ),
         SarusParameter(
             name="random_state",
             annotation=Optional[Union[int, np.random.RandomState]],
             default=None,
         ),
-        SarusParameter(
-            name="base_estimator",
-            annotation=Optional[BaseEstimator],
-            default=None,
-        ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
         kwargs = await signature.collect_kwargs()
         return ensemble.AdaBoostClassifier(**kwargs)
```

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/skopt.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/skopt.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/std.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/std.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,15 @@
             name="this",
             annotation=Any,
         ),
         SarusParameter(
             name="key",
             annotation=Any,
         ),
+        name=_transform_id,
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
         this, key = await signature.collect_args()
         return this[key]
 
 
@@ -198,14 +199,15 @@
             name="key",
             annotation=Any,
         ),
         SarusParameter(
             name="value",
             annotation=Any,
         ),
+        name=_transform_id,
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
         this, key, value = await signature.collect_args()
         this[key] = value
         return this
 
@@ -649,14 +651,15 @@
 class sudo(ExternalOpImplementation):
     _transform_id = "std.SUDO"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Any,
         ),
+        name="sudo",
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
         (this,) = await signature.collect_args()
         return this
```

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/typing.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/utils.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/xgboost.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/external/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/routing.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/routing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/extract.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/extract.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/filter.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/filter.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/get_item.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/get_item.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/project.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/project.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/sample.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/select_sql.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/select_sql.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/shuffle.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/shuffle.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/standard_op.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/standard_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     DatasetImplementation,
     DatasetStaticChecker,
     DataspecStaticChecker,
     ScalarImplementation,
 )
 
 try:
-    from sarus_data_spec.manager.ops.sql_mapping import (
+    from sarus_data_spec.manager.ops.sql_utils.table_mapping import (
         name_encoder,
         table_mapping,
     )
 except ModuleNotFoundError:
     warnings.warn('table_mapping not found. Cannot send sql queries.')
 from sarus_data_spec.scalar import Scalar
 import sarus_data_spec.typing as st
```

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/synthetic.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/synthetic.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/source/routing.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/ops/source/routing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/typing.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/marginals.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/marginals.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/multiplicity.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/multiplicity.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/path.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/path.py`

 * *Files 17% similar despite different names*

```diff
@@ -91,15 +91,32 @@
     return Path(
         sp.Path(label=label, paths=[element.protobuf() for element in paths])
     )
 
 
 def straight_path(nodes: t.List[str]) -> Path:
     """Returns linear path between elements in the list"""
-    built_path = path(label=nodes.pop(-1))
-    while len(nodes) > 0:
-        built_path = path(label=nodes.pop(-1), paths=[built_path])
-    return built_path
+    if len(nodes) == 0:
+        raise ValueError('At least one node must be provided')
+    curr_sub_path: t.List[st.Path] = []
+    for el in reversed(nodes):
+        update = path(label=el, paths=curr_sub_path)
+        curr_sub_path = [update]
+    return update
+
+
+def append_to_straight_path(
+    curr_path: t.Optional[st.Path], new_element: str
+) -> st.Path:
+    if curr_path is None:
+        return straight_path([new_element])
+    else:
+        return straight_path(
+            [
+                *(element for element in curr_path.to_strings_list()[0]),
+                new_element,
+            ]
+        )
 
 
 if t.TYPE_CHECKING:
     test_path: st.Path = Path(sp.Path())
```

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/predicate.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/predicate.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/__init__.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/attribute_pb2.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/attribute_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/attribute_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/attribute_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/bounds_pb2.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/bounds_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/bounds_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/bounds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/constraint_pb2.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/constraint_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/constraint_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/constraint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/dataset.proto` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/dataset.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/dataset_pb2.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/dataset_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/links_pb2.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/links_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/links_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/manager_pb2.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/manager_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/marginals_pb2.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/marginals_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/marginals_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/marginals_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/multiplicity_pb2.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/multiplicity_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/multiplicity_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/multiplicity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/path_pb2.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/path_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/path_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/path_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/predicate.proto` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/predicate.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/predicate_pb2.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/predicate_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/predicate_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/predicate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/proto_container_pb2.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/proto_container_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/proto_container_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/proto_container_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/relation.proto` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/relation.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/relation_pb2.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/relation_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/relation_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/relation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/scalar.proto` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/scalar.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/scalar_pb2.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/scalar_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/scalar_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/scalar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/schema.proto` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/schema.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/schema_pb2.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/schema_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/size_pb2.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/size_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/size_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/size_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/statistics.proto` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/statistics.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/statistics_pb2.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/statistics_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/statistics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/status.proto` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/status.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/status_pb2.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/status_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/status_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/transform.proto` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/transform.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/transform_pb2.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/transform_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/transform_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/transform_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/type.proto` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/type.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/type_pb2.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/type_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/type_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/typing.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/utilities.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/protobuf/utilities.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/scalar.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/scalar.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/schema.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/size.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/size.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/statistics.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/statistics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/status.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/status.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/storage/local.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/storage/local.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/storage/typing.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/storage/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/storage/utils.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/storage/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/transform.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/transform.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/type.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/typing.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/typing.py`

 * *Files 0% similar despite different names*

```diff
@@ -901,14 +901,15 @@
     SQL_SERVER = 2
     MY_SQL = 3
     SQLLITE = 4
     ORACLE = 5
     BIG_QUERY = 6
     REDSHIFT = 7
     HIVE = 8
+    DATABRICKS = 9
 
 
 class InferredDistributionName(Enum):
     UNIFORM = "Uniform"
     NORMAL = "Normal"
     EXPONENTIAL = "Exponential"
     GAMMA = "Gamma"
```

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/variant_constraint.py` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec/variant_constraint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import List, Optional, Type, cast
 import json
 
 from sarus_data_spec.base import Referring
-from sarus_data_spec.constants import PEP_TOKEN, PRIVACY_LIMIT
+from sarus_data_spec.constants import IS_PUBLIC, PEP_TOKEN, PRIVACY_LIMIT
 from sarus_data_spec.dataspec_validator.privacy_limit import DeltaEpsilonLimit
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 
 
 class VariantConstraint(Referring[sp.VariantConstraint]):
     def __init__(
@@ -42,20 +42,25 @@
             st.DataSpec, self.storage().referrable(self.protobuf().dataspec)
         )
 
 
 # Builders
 
 
-def public_constraint(dataspec: st.DataSpec) -> VariantConstraint:
+def public_constraint(
+    dataspec: st.DataSpec, is_public: bool = True
+) -> VariantConstraint:
     """Create a variant constraint specifying a dataspec is Public."""
     return VariantConstraint(
         sp.VariantConstraint(
             dataspec=dataspec.uuid(),
             constraint_kind=sp.ConstraintKind.PUBLIC,
+            properties={
+                IS_PUBLIC: str(is_public),
+            },
         )
     )
 
 
 def dp_constraint(
     dataspec: st.DataSpec,
     required_context: List[str],
```

### Comparing `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec_public.egg-info/SOURCES.txt` & `sarus_data_spec_public-3.2.1.dev3/sarus_data_spec_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/setup.cfg` & `sarus_data_spec_public-3.2.1.dev3/setup.cfg`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev2/setup.py` & `sarus_data_spec_public-3.2.1.dev3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 
     def run(self):
         generate_proto_code()
         build_py.run(self)
 
 
 if __name__ == '__main__':
-    setup(version='3.2.1.dev2')
+    setup(version='3.2.1.dev3')
```

