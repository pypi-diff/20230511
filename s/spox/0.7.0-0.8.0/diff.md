# Comparing `tmp/spox-0.7.0.tar.gz` & `tmp/spox-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spox-0.7.0.tar", last modified: Tue Apr  4 08:10:34 2023, max compression
+gzip compressed data, was "spox-0.8.0.tar", last modified: Thu May 11 10:38:01 2023, max compression
```

## Comparing `spox-0.7.0.tar` & `spox-0.8.0.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.216053 spox-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)      313 2023-04-04 08:10:26.000000 spox-0.7.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-04-04 08:10:26.000000 spox-0.7.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.204053 spox-0.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-04 08:10:26.000000 spox-0.7.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-04-04 08:10:26.000000 spox-0.7.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-04-04 08:10:26.000000 spox-0.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.204053 spox-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      947 2023-04-04 08:10:26.000000 spox-0.7.0/.github/workflows/build_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-04-04 08:10:26.000000 spox-0.7.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1331 2023-04-04 08:10:26.000000 spox-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      954 2023-04-04 08:10:26.000000 spox-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-04 08:10:26.000000 spox-0.7.0/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (122)      114 2023-04-04 08:10:26.000000 spox-0.7.0/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-04-04 08:10:26.000000 spox-0.7.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     4613 2023-04-04 08:10:26.000000 spox-0.7.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-04-04 08:10:26.000000 spox-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-04-04 08:10:34.216053 spox-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3074 2023-04-04 08:10:26.000000 spox-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.204053 spox-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-04-04 08:10:26.000000 spox-0.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     3160 2023-04-04 08:10:26.000000 spox-0.7.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.204053 spox-0.7.0/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (122)    15415 2023-04-04 08:10:26.000000 spox-0.7.0/docs/guides/advanced.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    11423 2023-04-04 08:10:26.000000 spox-0.7.0/docs/guides/converter.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    38133 2023-04-04 08:10:26.000000 spox-0.7.0/docs/guides/example-model-netron.png
--rw-r--r--   0 runner    (1001) docker     (122)    15822 2023-04-04 08:10:26.000000 spox-0.7.0/docs/guides/inference.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     9165 2023-04-04 08:10:26.000000 spox-0.7.0/docs/guides/inline.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    50579 2023-04-04 08:10:26.000000 spox-0.7.0/docs/guides/tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-04 08:10:26.000000 spox-0.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      793 2023-04-04 08:10:26.000000 spox-0.7.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.204053 spox-0.7.0/docs/manual/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-04-04 08:10:26.000000 spox-0.7.0/docs/manual/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (122)    11022 2023-04-04 08:10:26.000000 spox-0.7.0/docs/manual/operators.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5279 2023-04-04 08:10:26.000000 spox-0.7.0/docs/manual/overview.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7927 2023-04-04 08:10:26.000000 spox-0.7.0/docs/manual/unstable.rst
--rw-r--r--   0 runner    (1001) docker     (122)      436 2023-04-04 08:10:26.000000 spox-0.7.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-04-04 08:10:26.000000 spox-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-04 08:10:34.216053 spox-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.200053 spox-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.208053 spox-0.7.0/src/spox/
--rw-r--r--   0 runner    (1001) docker     (122)      877 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4185 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_adapt.py
--rw-r--r--   0 runner    (1001) docker     (122)     6644 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_attributes.py
--rw-r--r--   0 runner    (1001) docker     (122)    19064 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_build.py
--rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_debug.py
--rw-r--r--   0 runner    (1001) docker     (122)      926 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4004 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_fields.py
--rw-r--r--   0 runner    (1001) docker     (122)     7194 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_function.py
--rw-r--r--   0 runner    (1001) docker     (122)     6775 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_future.py
--rw-r--r--   0 runner    (1001) docker     (122)    18771 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     4913 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_inline.py
--rw-r--r--   0 runner    (1001) docker     (122)     8795 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_internal_op.py
--rw-r--r--   0 runner    (1001) docker     (122)    15250 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_node.py
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_patch_ref_impl.py
--rw-r--r--   0 runner    (1001) docker     (122)     8194 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_public.py
--rw-r--r--   0 runner    (1001) docker     (122)     3292 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_schemas.py
--rw-r--r--   0 runner    (1001) docker     (122)     7148 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_scope.py
--rw-r--r--   0 runner    (1001) docker     (122)     8460 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_shape.py
--rw-r--r--   0 runner    (1001) docker     (122)    10310 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_standard.py
--rw-r--r--   0 runner    (1001) docker     (122)     3237 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_traverse.py
--rw-r--r--   0 runner    (1001) docker     (122)     9434 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_type_system.py
--rw-r--r--   0 runner    (1001) docker     (122)     2191 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     6537 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_value_prop.py
--rw-r--r--   0 runner    (1001) docker     (122)     7478 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/_var.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.200053 spox-0.7.0/src/spox/opset/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.200053 spox-0.7.0/src/spox/opset/ai/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.208053 spox-0.7.0/src/spox/opset/ai/onnx/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.208053 spox-0.7.0/src/spox/opset/ai/onnx/ml/
--rw-r--r--   0 runner    (1001) docker     (122)    63324 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/opset/ai/onnx/ml/v3.py
--rw-r--r--   0 runner    (1001) docker     (122)   461188 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/opset/ai/onnx/v17.py
--rw-r--r--   0 runner    (1001) docker     (122)    93407 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/opset/ai/onnx/v18.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:26.000000 spox-0.7.0/src/spox/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.208053 spox-0.7.0/src/spox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-04-04 08:10:34.000000 spox-0.7.0/src/spox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3871 2023-04-04 08:10:34.000000 spox-0.7.0/src/spox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-04 08:10:34.000000 spox-0.7.0/src/spox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-04 08:10:34.000000 spox-0.7.0/src/spox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-04 08:10:34.000000 spox-0.7.0/src/spox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.212053 spox-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:26.000000 spox-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-04-04 08:10:26.000000 spox-0.7.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.212053 spox-0.7.0/tests/full/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:26.000000 spox-0.7.0/tests/full/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4623 2023-04-04 08:10:26.000000 spox-0.7.0/tests/full/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      918 2023-04-04 08:10:26.000000 spox-0.7.0/tests/full/test_brackets.py
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-04-04 08:10:26.000000 spox-0.7.0/tests/full/test_lifting.py
--rw-r--r--   0 runner    (1001) docker     (122)     5908 2023-04-04 08:10:26.000000 spox-0.7.0/tests/full/test_turing_completeness.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.212053 spox-0.7.0/tests/future/
--rw-r--r--   0 runner    (1001) docker     (122)     3662 2023-04-04 08:10:26.000000 spox-0.7.0/tests/future/test_var_operators.py
--rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-04-04 08:10:26.000000 spox-0.7.0/tests/test_adapt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-04-04 08:10:26.000000 spox-0.7.0/tests/test_attr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1914 2023-04-04 08:10:26.000000 spox-0.7.0/tests/test_broadcast.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-04-04 08:10:26.000000 spox-0.7.0/tests/test_constructors.py
--rw-r--r--   0 runner    (1001) docker     (122)     3036 2023-04-04 08:10:26.000000 spox-0.7.0/tests/test_custom_operator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-04-04 08:10:26.000000 spox-0.7.0/tests/test_equiv_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    10402 2023-04-04 08:10:26.000000 spox-0.7.0/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-04-04 08:10:26.000000 spox-0.7.0/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     1039 2023-04-04 08:10:26.000000 spox-0.7.0/tests/test_initializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5774 2023-04-04 08:10:26.000000 spox-0.7.0/tests/test_inline.py
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-04-04 08:10:26.000000 spox-0.7.0/tests/test_opsets.py
--rw-r--r--   0 runner    (1001) docker     (122)      427 2023-04-04 08:10:26.000000 spox-0.7.0/tests/test_optional.py
--rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-04-04 08:10:26.000000 spox-0.7.0/tests/test_public.py
--rw-r--r--   0 runner    (1001) docker     (122)     2111 2023-04-04 08:10:26.000000 spox-0.7.0/tests/test_standard_op.py
--rw-r--r--   0 runner    (1001) docker     (122)    11133 2023-04-04 08:10:26.000000 spox-0.7.0/tests/test_subgraphs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2043 2023-04-04 08:10:26.000000 spox-0.7.0/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (122)     2897 2023-04-04 08:10:26.000000 spox-0.7.0/tests/test_type_translation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4651 2023-04-04 08:10:26.000000 spox-0.7.0/tests/test_value_propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.216053 spox-0.7.0/tests/type_inference/
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-04-04 08:10:26.000000 spox-0.7.0/tests/type_inference/test_array_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-04-04 08:10:26.000000 spox-0.7.0/tests/type_inference/test_binarizer.py
--rw-r--r--   0 runner    (1001) docker     (122)      437 2023-04-04 08:10:26.000000 spox-0.7.0/tests/type_inference/test_category_mapper.py
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-04-04 08:10:26.000000 spox-0.7.0/tests/type_inference/test_compress.py
--rw-r--r--   0 runner    (1001) docker     (122)      947 2023-04-04 08:10:26.000000 spox-0.7.0/tests/type_inference/test_imputer.py
--rw-r--r--   0 runner    (1001) docker     (122)      907 2023-04-04 08:10:26.000000 spox-0.7.0/tests/type_inference/test_label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-04 08:10:26.000000 spox-0.7.0/tests/type_inference/test_linear_regressor.py
--rw-r--r--   0 runner    (1001) docker     (122)      418 2023-04-04 08:10:26.000000 spox-0.7.0/tests/type_inference/test_loop.py
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-04-04 08:10:26.000000 spox-0.7.0/tests/type_inference/test_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-04-04 08:10:26.000000 spox-0.7.0/tests/type_inference/test_one_hot.py
--rw-r--r--   0 runner    (1001) docker     (122)     1280 2023-04-04 08:10:26.000000 spox-0.7.0/tests/type_inference/test_one_hot_encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)      596 2023-04-04 08:10:26.000000 spox-0.7.0/tests/type_inference/test_scaler.py
--rw-r--r--   0 runner    (1001) docker     (122)      752 2023-04-04 08:10:26.000000 spox-0.7.0/tests/type_inference/test_tree_ensemble_classifier.py
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-04-04 08:10:26.000000 spox-0.7.0/tests/type_inference/test_tree_ensemble_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.216053 spox-0.7.0/tools/
--rw-r--r--   0 runner    (1001) docker     (122)    25288 2023-04-04 08:10:26.000000 spox-0.7.0/tools/generate_opset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.216053 spox-0.7.0/tools/templates/
--rw-r--r--   0 runner    (1001) docker     (122)     1698 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/class.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/construct.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)     1114 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/constructor.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/docstring.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.216053 spox-0.7.0/tools/templates/extras/
--rw-r--r--   0 runner    (1001) docker     (122)      278 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/extras/const.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      885 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/extras/promote.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/extras/xif.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/extras/xloop.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/inherit.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/preamble.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/summary.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.216053 spox-0.7.0/tools/templates/type_inference/
--rw-r--r--   0 runner    (1001) docker     (122)      576 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/type_inference/arrayfeatureextractor1.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)       74 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/type_inference/binarizer1.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      455 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/type_inference/categorymapper1.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      767 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/type_inference/compress11.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      627 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/type_inference/if16.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)     1021 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/type_inference/imputer1.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/type_inference/linearregressor1.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/type_inference/loop16-fix.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)     2523 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/type_inference/loop16.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/type_inference/normalizer1.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/type_inference/onehot11.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/type_inference/onehotencoder1.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/type_inference/scaler1.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      687 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/type_inference/treeensembleclassifier3.jinja2
--rw-r--r--   0 runner    (1001) docker     (122)      411 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/type_inference/treeensembleregressor3.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 08:10:34.216053 spox-0.7.0/tools/templates/value_propagation/
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-04-04 08:10:26.000000 spox-0.7.0/tools/templates/value_propagation/constant13.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.581310 spox-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      313 2023-05-11 10:37:53.000000 spox-0.8.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-05-11 10:37:53.000000 spox-0.8.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.565310 spox-0.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-11 10:37:53.000000 spox-0.8.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-11 10:37:53.000000 spox-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-05-11 10:37:53.000000 spox-0.8.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.565310 spox-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      947 2023-05-11 10:37:53.000000 spox-0.8.0/.github/workflows/build_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-05-11 10:37:53.000000 spox-0.8.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1331 2023-05-11 10:37:53.000000 spox-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      954 2023-05-11 10:37:53.000000 spox-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-11 10:37:53.000000 spox-0.8.0/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-05-11 10:37:53.000000 spox-0.8.0/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-05-11 10:37:53.000000 spox-0.8.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     5718 2023-05-11 10:37:53.000000 spox-0.8.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-05-11 10:37:53.000000 spox-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-05-11 10:38:01.581310 spox-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3074 2023-05-11 10:37:53.000000 spox-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.565310 spox-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-05-11 10:37:53.000000 spox-0.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     3160 2023-05-11 10:37:53.000000 spox-0.8.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.565310 spox-0.8.0/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (122)    15415 2023-05-11 10:37:53.000000 spox-0.8.0/docs/guides/advanced.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    11423 2023-05-11 10:37:53.000000 spox-0.8.0/docs/guides/converter.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    38133 2023-05-11 10:37:53.000000 spox-0.8.0/docs/guides/example-model-netron.png
+-rw-r--r--   0 runner    (1001) docker     (122)    15822 2023-05-11 10:37:53.000000 spox-0.8.0/docs/guides/inference.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     9165 2023-05-11 10:37:53.000000 spox-0.8.0/docs/guides/inline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    50579 2023-05-11 10:37:53.000000 spox-0.8.0/docs/guides/tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-05-11 10:37:53.000000 spox-0.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      793 2023-05-11 10:37:53.000000 spox-0.8.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.569310 spox-0.8.0/docs/manual/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-05-11 10:37:53.000000 spox-0.8.0/docs/manual/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11022 2023-05-11 10:37:53.000000 spox-0.8.0/docs/manual/operators.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5279 2023-05-11 10:37:53.000000 spox-0.8.0/docs/manual/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7928 2023-05-11 10:37:53.000000 spox-0.8.0/docs/manual/unstable.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      436 2023-05-11 10:37:53.000000 spox-0.8.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-05-11 10:37:53.000000 spox-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 10:38:01.581310 spox-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.565310 spox-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.569310 spox-0.8.0/src/spox/
+-rw-r--r--   0 runner    (1001) docker     (122)      877 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4193 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_adapt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6644 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19315 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (122)      926 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4004 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7117 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7285 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_future.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18828 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4750 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_inline.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8733 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_internal_op.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15132 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_node.py
+-rw-r--r--   0 runner    (1001) docker     (122)      993 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_patch_ref_impl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9767 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_public.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3292 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7148 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_scope.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8460 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_shape.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10455 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_standard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3237 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_traverse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9434 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_type_system.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2191 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6537 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_value_prop.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7478 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/_var.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.565310 spox-0.8.0/src/spox/opset/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.565310 spox-0.8.0/src/spox/opset/ai/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.573310 spox-0.8.0/src/spox/opset/ai/onnx/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.573310 spox-0.8.0/src/spox/opset/ai/onnx/ml/
+-rw-r--r--   0 runner    (1001) docker     (122)    63324 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/opset/ai/onnx/ml/v3.py
+-rw-r--r--   0 runner    (1001) docker     (122)   461188 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/opset/ai/onnx/v17.py
+-rw-r--r--   0 runner    (1001) docker     (122)    93407 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/opset/ai/onnx/v18.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 10:37:53.000000 spox-0.8.0/src/spox/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.569310 spox-0.8.0/src/spox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-05-11 10:38:01.000000 spox-0.8.0/src/spox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3871 2023-05-11 10:38:01.000000 spox-0.8.0/src/spox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 10:38:01.000000 spox-0.8.0/src/spox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-11 10:38:01.000000 spox-0.8.0/src/spox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-11 10:38:01.000000 spox-0.8.0/src/spox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.573310 spox-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 10:37:53.000000 spox-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-05-11 10:37:53.000000 spox-0.8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.573310 spox-0.8.0/tests/full/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 10:37:53.000000 spox-0.8.0/tests/full/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4623 2023-05-11 10:37:53.000000 spox-0.8.0/tests/full/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      918 2023-05-11 10:37:53.000000 spox-0.8.0/tests/full/test_brackets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-05-11 10:37:53.000000 spox-0.8.0/tests/full/test_lifting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5908 2023-05-11 10:37:53.000000 spox-0.8.0/tests/full/test_turing_completeness.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.573310 spox-0.8.0/tests/future/
+-rw-r--r--   0 runner    (1001) docker     (122)     3662 2023-05-11 10:37:53.000000 spox-0.8.0/tests/future/test_var_operators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3304 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_adapt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1914 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3036 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_custom_operator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_equiv_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10402 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1039 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6869 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_inline.py
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_opsets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_optional.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_public.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2111 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_standard_op.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12965 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_subgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2043 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2897 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_type_translation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4651 2023-05-11 10:37:53.000000 spox-0.8.0/tests/test_value_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.577310 spox-0.8.0/tests/type_inference/
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_array_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_binarizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_category_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_compress.py
+-rw-r--r--   0 runner    (1001) docker     (122)      947 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_imputer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      907 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_linear_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      418 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_loop.py
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_one_hot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1280 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_one_hot_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)      596 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_tree_ensemble_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-05-11 10:37:53.000000 spox-0.8.0/tests/type_inference/test_tree_ensemble_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.577310 spox-0.8.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)    25288 2023-05-11 10:37:53.000000 spox-0.8.0/tools/generate_opset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.577310 spox-0.8.0/tools/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     1698 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/class.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/construct.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)     1114 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/constructor.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/docstring.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.577310 spox-0.8.0/tools/templates/extras/
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/extras/const.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      885 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/extras/promote.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/extras/xif.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/extras/xloop.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/inherit.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/preamble.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/summary.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.581310 spox-0.8.0/tools/templates/type_inference/
+-rw-r--r--   0 runner    (1001) docker     (122)      576 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/arrayfeatureextractor1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/binarizer1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/categorymapper1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      767 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/compress11.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/if16.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)     1021 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/imputer1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/linearregressor1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/loop16-fix.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)     2523 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/loop16.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/normalizer1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/onehot11.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/onehotencoder1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/scaler1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/treeensembleclassifier3.jinja2
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/type_inference/treeensembleregressor3.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:38:01.581310 spox-0.8.0/tools/templates/value_propagation/
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-05-11 10:37:53.000000 spox-0.8.0/tools/templates/value_propagation/constant13.jinja2
```

### Comparing `spox-0.7.0/.github/workflows/build_and_publish.yml` & `spox-0.8.0/.github/workflows/build_and_publish.yml`

 * *Files 11% similar despite different names*

```diff
@@ -35,11 +35,11 @@
     if: github.event_name == 'release' && github.event.action == 'published'
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: artifact
           path: dist
 
-      - uses: pypa/gh-action-pypi-publish@v1.8.5
+      - uses: pypa/gh-action-pypi-publish@v1.8.6
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `spox-0.7.0/.github/workflows/ci.yml` & `spox-0.8.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/.gitignore` & `spox-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/.pre-commit-config.yaml` & `spox-0.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/CHANGELOG.rst` & `spox-0.8.0/CHANGELOG.rst`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,29 @@
    * Update the major if you break the public API
    * Update the minor if you add new functionality
    * Update the patch if you fixed a bug
 
 Change log
 ==========
 
+0.8.0 (2023-05-11)
+------------------
+
+This version is intended as a release candidate for ``1.0.0``.
+
+**New feature**
+
+- Spox now explicitly sets a model's IR version (currently to version 8) rather than defaulting to the latest IR version supported by the installed onnx package. Increasing the IR version is not considered a breaking change going forward. The IR version will be increase once the ecosystem has adopted it more broadly.
+
+**Bug fixes**
+
+- Fix an issue with resolving scopes during the build process. They manifested with a ``KeyError`` in accessing variables in scope on graphs in complex dependencies between subgraphs.
+- ``inline`` now removes all symbolic dimensions from input/output shapes (i.e. ``N x 2`` becomes ``? x 2``) before inferring types to avoid inconsistent interactions. This is only a visual change of the output in some cases, as they are not compared strictly in ONNX.
+- ``inline`` now explicitly does not accept model with subgraphs and local functions. Attempting to use these would usually result in invalid models. Support for them will be added in the future.
+
 0.7.0 (2023-04-04)
 ------------------
 
 This version is intended as a release candidate for ``1.0.0``.
 
 **New features**
```

### Comparing `spox-0.7.0/LICENSE` & `spox-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/PKG-INFO` & `spox-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spox
-Version: 0.7.0
+Version: 0.8.0
 Summary: A framework for constructing ONNX computational graphs.
 Author-email: Jakub Bachurski <kbachurski@gmail.com>, Christian Bourjau <christian.bourjau@quantco.com>
 Maintainer-email: Jakub Bachurski <kbachurski@gmail.com>, Christian Bourjau <christian.bourjau@quantco.com>
 Project-URL: Source, https://github.com/quantco/spox
 Keywords: machine-learning,onnx
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `spox-0.7.0/README.md` & `spox-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/docs/Makefile` & `spox-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/docs/conf.py` & `spox-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/docs/guides/advanced.ipynb` & `spox-0.8.0/docs/guides/advanced.ipynb`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/docs/guides/converter.ipynb` & `spox-0.8.0/docs/guides/converter.ipynb`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/docs/guides/example-model-netron.png` & `spox-0.8.0/docs/guides/example-model-netron.png`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/docs/guides/inference.ipynb` & `spox-0.8.0/docs/guides/inference.ipynb`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/docs/guides/inline.ipynb` & `spox-0.8.0/docs/guides/inline.ipynb`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/docs/guides/tutorial.ipynb` & `spox-0.8.0/docs/guides/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/docs/index.rst` & `spox-0.8.0/docs/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 .. toctree::
    :maxdepth: 1
    :caption: API Listing
 
    API Reference <api/modules>
    Operator constructors for the ai.onnx domain version 17 <api/spox.opset.ai.onnx.v17>
+   Operator constructors for the ai.onnx domain version 18 <api/spox.opset.ai.onnx.v18>
    Operator constructors for the ai.onnx.ml domain version 3 <api/spox.opset.ai.onnx.ml.v3>
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
```

### Comparing `spox-0.7.0/docs/make.bat` & `spox-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/docs/manual/operators.rst` & `spox-0.8.0/docs/manual/operators.rst`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/docs/manual/overview.rst` & `spox-0.8.0/docs/manual/overview.rst`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/docs/manual/unstable.rst` & `spox-0.8.0/docs/manual/unstable.rst`

 * *Files 0% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 
 Initializers
 ============
 
 Initializers are an ONNX mechanism for expressing constant tensor values in the model. Spox provides a function to create them:
 
 ..  code:: python
+
     def initializer(value: ArrayLike, dtype: DTypeLike = None) -> Var:
         ...
 
 This is a mechanism alternative to the ``ai.onnx::Constant`` operator. In our experience initializers sometimes have worse support, which is why they remain unstable. Additionally, both methods essentially achieve the same result.
 
 
 Operator overloading
```

### Comparing `spox-0.7.0/pyproject.toml` & `spox-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/src/spox/__init__.py` & `spox-0.8.0/src/spox/__init__.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/src/spox/_adapt.py` & `spox-0.8.0/src/spox/_adapt.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     if source_version != target_version:
         target_model = onnx.version_converter.convert_version(
             node.model, target_version
         )
         base_model = node.model
         try:
             node.model = target_model
-            target_nodes = node.to_onnx(Scope.of(*var_names.items()), node_name)
+            target_nodes = node.to_onnx(Scope.of((node, node_name), *var_names.items()))
         finally:
             node.model = base_model
         return target_nodes
     return protos
 
 
 def adapt_best_effort(
```

### Comparing `spox-0.7.0/src/spox/_attributes.py` & `spox-0.8.0/src/spox/_attributes.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/src/spox/_build.py` & `spox-0.8.0/src/spox/_build.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,87 +118,92 @@
         By the second rule, the parent scope of a given scope is ``scope_of[subgraph_of[graph]]``.
 
         We may find that the first constraint is sometimes not satisfied. Then we set the scope of a node to the
         parent scope of its current scope, as many times as possible. This turns out to be computable with LCA
         (lowest common ancestor), which is a common operation on trees.
         """
 
-        subgraph_of: Dict["Graph", Node]
+        subgraph_owner: Dict["Graph", Node]
         scope_of: Dict[Node, "Graph"]
 
         def __init__(self):
-            self.subgraph_of = {}
+            self.subgraph_owner = {}
             self.scope_of = {}
 
         def parent(self, graph: "Graph") -> "Graph":
             """
             Return the parent of a scope in the represented scope tree.
 
             A scope must be the child of the scope of the node that holds this scope (subgraph)
             If there is no parent (the main graph is not a subgraph of anything), the scope itself is returned.
             """
             return (
-                self.scope_of[self.subgraph_of[graph]]
-                if graph in self.subgraph_of
+                self.scope_of[self.subgraph_owner[graph]]
+                if graph in self.subgraph_owner
                 else graph
             )
 
         def lca(self, a: "Graph", b: "Graph") -> "Graph":
             """
             A simple LCA algorithm without preprocessing that only accesses the parents.
 
-            The algorithm is simple - we keep going up one step with both nodes
-            Whenever we hit a node that was already visited, it must be the lowest common ancestor
+            The algorithm is simple - we keep going up one step alternating between the nodes.
+            Whenever we hit a node that was already visited, it must be the lowest common ancestor.
             - as it is definitely a common ancestor, and it required the least steps up.
 
             Time and space complexity in the length of the path between a, b in the tree.
             """
-            if a is b:
-                return a
-            vis = set()
-            while True:
-                if a in vis:
-                    return a
-                if b in vis:
-                    return b
-                vis.add(a)
-                vis.add(b)
-                a, b = self.parent(a), self.parent(b)
+            vis_a, vis_b = {a}, {b}
+            while a not in vis_b:
+                vis_a.add(a)
+                a = self.parent(a)
+                a, b = b, a
+                vis_a, vis_b = vis_b, vis_a
+            return a
 
     # Graphs needed in the build
     main: "Graph"
     graphs: Set["Graph"]
+    graph_topo: List["Graph"]
     # Arguments, results
     arguments_of: Dict["Graph", List[Var]]
     results_of: Dict["Graph", List[Var]]
     source_of: Dict["Graph", Node]
     # Arguments found by traversal
     all_arguments_in: Dict["Graph", Set[Var]]
     claimed_arguments_in: Dict["Graph", Set[Var]]
     # Scopes
     scope_tree: ScopeTree
     scope_own: Dict["Graph", List[Node]]
 
     def __init__(self, main: "Graph"):
         self.main = main
         self.graphs = set()
+        self.graph_topo = list()
         self.arguments_of = {}
         self.results_of = {}
         self.source_of = {}
         self.all_arguments_in = {}
         self.claimed_arguments_in = {}
         self.scope_tree = self.ScopeTree()
         self.scope_own = {}
 
     def build_main(self) -> BuildResult:
+        # Discovery
         self.discover(self.main)
+        self.graph_topo.reverse()
         if not self.graphs == set(self.arguments_of) == set(self.results_of):
             raise BuildError("Some graphs have missing build data.")
-        self.update_scope_tree(self.main)
+
+        # Resolving scopes
+        for graph in self.graph_topo:
+            self.update_scope_tree(graph)
         self.resolve_scopes()
+
+        # Compilation
         return self.compile_graph(self.main, Scope())
 
     @staticmethod
     def get_intro_results(
         request_results: Dict[str, Var], set_names: bool
     ) -> List[Var]:
         """
@@ -212,15 +217,16 @@
         for key, var in zip(request_results, vars):
             if set_names:
                 var._rename(key)
         return vars
 
     def discover(self, graph: "Graph") -> Tuple[Set[Var], Set[Var]]:
         """
-        Run the discover step of the build process. Resolves arguments and results for the involved graphs.
+        Run the discovery step of the build process. Resolves arguments and results for the involved graphs.
+        Finds the topological ordering between (sub)graphs and sets their owners (nodes of which they are attributes).
 
         The time complexity of this step is in the order of the sum over the counts of intermediate nodes
         for all subgraphs (scopes). With number of scopes `s` and number of nodes `n`, worst-case is `O(ns) = O(n^2)`.
 
         The bottleneck is in rediscovering the same argument nodes many times. This could be avoided if used arguments
         (the basis) were stored in the Node itself and computed during construction time.
 
@@ -253,20 +259,27 @@
             nonlocal all_arguments, claimed_arguments
             if isinstance(nd, Argument):
                 all_arguments.add(nd.outputs.arg)
             for subgraph in nd.subgraphs:
                 all_arguments_sub, claimed_arguments_sub = self.discover(subgraph)
                 all_arguments |= all_arguments_sub
                 claimed_arguments |= claimed_arguments_sub
+                if subgraph not in self.scope_tree.subgraph_owner:
+                    self.scope_tree.subgraph_owner[subgraph] = nd
+                if self.scope_tree.subgraph_owner[subgraph] != nd:
+                    raise BuildError(
+                        "Subgraph has multiple owners (the Graph instance was reused)."
+                    )
 
         iterative_dfs(
             [self.source_of[graph]],
             lambda nd: (a._op for a in nd.dependencies),
             collect_arguments,
         )
+        self.graph_topo.append(graph)
 
         # Now we resolve which arguments we should get.
         if graph.requested_arguments is None:
             # If there's no request, we take all arguments
             self.arguments_of[graph] = list(all_arguments - claimed_arguments)
         else:
             # If there is a request, we may not have found it by traversal if an argument was unused.
@@ -288,37 +301,32 @@
 
         The algorithm is based on a relaxation of the scopes when a constraint requires it.
         - When a new node is found, by default it is assigned to the scope of the graph it is found in.
         - If a node was already in the graph and had a scope assigned, that scope has to be accessible to the
           graph that we are in (as this is an indirect result to this graph).
           In this case we update the scope to the LCA of this graph's scope and the existing scope.
         - This cannot break the input-scope (1st) constraint (as we only expose more values to scopes),
-          and the 2nd constraint is not moved.
-        - We may recursively descend into subgraphs found by traversing this graph. This will serve to update the scope
-          tree and satisfy that subgraph's constraints.
+          and the 2nd constraint is not affected.
 
         Pessimistically an LCA constraint update may be O(s), and all n nodes may be visited in all s scopes.
-        However, a node may be pushed up in the scope tree at most O(s) time, so the complexity is amortised to O(ns).
+        However, a node may be pushed up in the scope tree at most O(s) times, so the complexity is amortised to O(ns).
+
+        It is expected that subgraphs reachable from the source of ``graph`` have already been resolved.
+        This method is called for all graphs in topological ordering, which ensures the scope tree
+        is completed 'bottom-up'.
         """
 
         def satisfy_constraints(node):
             # By default, a node is bound to the scope it is found in.
-            if node not in self.scope_tree.scope_of:
-                self.scope_tree.scope_of[node] = graph
+            self.scope_tree.scope_of.setdefault(node, graph)
             # Bring up the scope of its node to its ancestors if it is too low to be accessible in the current graph.
             self.scope_tree.scope_of[node] = self.scope_tree.lca(
                 graph, self.scope_tree.scope_of[node]
             )
-            # For every subgraph, if we didn't apply its constraints yet apply a recursive traversal.
-            for sub in node.subgraphs:
-                if sub not in self.scope_tree.subgraph_of:
-                    self.scope_tree.subgraph_of[sub] = node
-                    self.update_scope_tree(sub)
 
-        # Visit from the source (result) of this graph. Traverse only input edges for the first constraint.
         iterative_dfs(
             [self.source_of[graph]],
             lambda nd: (a._op for a in nd.dependencies),
             satisfy_constraints,
         )
 
     def resolve_scopes(self) -> None:
```

### Comparing `spox-0.7.0/src/spox/_debug.py` & `spox-0.8.0/src/spox/_debug.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/src/spox/_exceptions.py` & `spox-0.8.0/src/spox/_exceptions.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/src/spox/_fields.py` & `spox-0.8.0/src/spox/_fields.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/src/spox/_function.py` & `spox-0.8.0/src/spox/_function.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import inspect
 import itertools
 from dataclasses import dataclass, make_dataclass
 from typing import TYPE_CHECKING, Callable, Dict, Iterable, Tuple, TypeVar
 
 import onnx
-from typing_extensions import TypeAlias
 
 from . import _attributes
 from ._fields import BaseAttributes, BaseInputs, BaseOutputs
 from ._internal_op import _InternalNode
 from ._node import Node, OpType
 from ._type_system import Type
 from ._var import Var
 
 if TYPE_CHECKING:
     from . import _graph
 
 DEFAULT_FUNCTION_DOMAIN = "spox.default"
 
-Constructor: TypeAlias = Callable[..., Iterable[Var]]
-ConstructorT = TypeVar("ConstructorT", bound=Constructor)
+ConstructorT = TypeVar("ConstructorT", bound=Callable[..., Iterable[Var]])
 
 
 class Function(_InternalNode):
     """
     Type of ``Node`` that is defined in terms of its abstract ``constructor``, which may invoke standard operators.
     Can be built into an ONNX function, and when a full model is built all instances inheriting from Function
     are converted to ONNX functions and stored alongside the built graph.
```

### Comparing `spox-0.7.0/src/spox/_future.py` & `spox-0.8.0/src/spox/_future.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,23 +9,43 @@
 import spox._node
 import spox._value_prop
 from spox._graph import initializer as _initializer
 from spox._type_system import Tensor
 from spox._var import Var
 
 TypeWarningLevel = spox._node.TypeWarningLevel
-set_type_warning_level = spox._node.set_type_warning_level
+
+
+def set_type_warning_level(level: TypeWarningLevel) -> None:
+    spox._node._TYPE_WARNING_LEVEL = level
+
+
+@contextmanager
+def type_warning_level(level: TypeWarningLevel):
+    prev_level = spox._node._TYPE_WARNING_LEVEL
+    set_type_warning_level(level)
+    yield
+    set_type_warning_level(prev_level)
+
 
 ValuePropBackend = spox._value_prop.ValuePropBackend
 
 
 def set_value_prop_backend(backend: ValuePropBackend) -> None:
     spox._value_prop._VALUE_PROP_BACKEND = backend
 
 
+@contextmanager
+def value_prop_backend(backend: ValuePropBackend):
+    prev_backend = spox._value_prop._VALUE_PROP_BACKEND
+    set_value_prop_backend(backend)
+    yield
+    set_value_prop_backend(prev_backend)
+
+
 def initializer(value: npt.ArrayLike, dtype: npt.DTypeLike = None) -> Var:
     """
     Create a Var with a constant value.
 
     Parameters
     ----------
     value
@@ -185,15 +205,17 @@
     Var._operator_dispatcher = prev_dispatcher
 
 
 __all__ = [
     # Type warning levels
     "TypeWarningLevel",
     "set_type_warning_level",
+    "type_warning_level",
     # Initializer-backed constants
     "initializer",
     # Value propagation backend
     "ValuePropBackend",
     "set_value_prop_backend",
+    "value_prop_backend",
     # Operator overloading on Var
     "operator_overloading",
 ]
```

### Comparing `spox-0.7.0/src/spox/_graph.py` & `spox-0.8.0/src/spox/_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,19 +345,20 @@
             result_info,
             initializer_tensors,
             self._doc_string,
         )
 
     def to_onnx_model(
         self,
+        *,
         producer_name: str = "spox",
         model_doc_string: str = "",
         infer_shapes: bool = False,
         check_model: Union[Literal[0], Literal[1], Literal[2]] = 1,
-        *,
+        ir_version=8,
         concrete: bool = True,
     ) -> onnx.ModelProto:
         """
         Internally, this function first obtains a GraphProto from ``.to_onnx()``. Additionally:
 
         - Function definitions are collected and built into FunctionProtos.
         - Opset requirements are collected (consistency policy is to use the highest version).
@@ -409,14 +410,15 @@
             producer_name=producer_name,
             doc_string=model_doc_string,
             functions=list(function_protos.values()),
             opset_imports=[
                 onnx.helper.make_operatorsetid(domain, version)
                 for domain, version in opsets.items()
             ],
+            ir_version=ir_version,
         )
 
         if infer_shapes:
             model = onnx.shape_inference.infer_shapes(model)
         if check_model:
             onnx.checker.check_model(model, full_check=check_model >= 2)
         return model
```

### Comparing `spox-0.7.0/src/spox/_inline.py` & `spox-0.8.0/src/spox/_inline.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
     def infer_output_types(self) -> Dict[str, Type]:
         # First, type check that we match the ModelProto type requirements
         for i, var in zip(self.graph.input, self.inputs.inputs):
             if var.type is not None and not (
                 var.type._subtype(Type._from_onnx(i.type))
             ):
                 raise TypeError(
-                    f"Embedded model input {i.name} type {var.type} "
-                    f"does not match expected {Type._from_onnx(i.type)}."
+                    f"Input '{i.name}' to inlined model got type {var.type}, "
+                    f"expected {Type._from_onnx(i.type)}."
                 )
         # If we do, take the types as declared in the model
         return {
             f"outputs_{k}": Type._from_onnx(o.type)
             for k, o in enumerate(self.graph.output)
         }
 
@@ -82,31 +82,29 @@
             for k, (o, var) in enumerate(zip(self.graph.output, self.outputs.outputs))
         }
 
     def to_onnx(
         self, scope: Scope, doc_string: Optional[str] = None, build_subgraph=None
     ) -> List[onnx.NodeProto]:
         # Prefix all names in the graph to try and avoid name clashes
-        name = scope.node[self] if self in scope.node else None
-        if name is not None:
-            graph = onnx.GraphProto()
-            graph.CopyFrom(self.graph)
-            # FIXME: This is a bug upstream - when add_prefix_graph has rename_edges,
-            #        unused inputs are not renamed. We apply identities to use the inputs.
-            for i in graph.input:
-                graph.node.append(
-                    onnx.helper.make_node(
-                        "Identity", [i.name], [f"__{i.name}_Identity_dummy_use"]
-                    )
+        name = scope.node[self]
+        graph = onnx.GraphProto()
+        graph.CopyFrom(self.graph)
+        # FIXME: This is a bug upstream - when add_prefix_graph has rename_edges,
+        #        unused inputs are not renamed. We apply identities to use the inputs.
+        for i in graph.input:
+            graph.node.append(
+                onnx.helper.make_node(
+                    "Identity", [i.name], [f"__{i.name}_Identity_dummy_use"]
                 )
-            graph = onnx.compose.add_prefix_graph(graph, f"{name}__")
-            for _ in graph.input:
-                graph.node.pop()
-        else:
-            graph = self.graph
+            )
+        graph = onnx.compose.add_prefix_graph(graph, f"{name}__")
+        for _ in graph.input:
+            graph.node.pop()
+
         nodes: List[onnx.NodeProto] = []
         # Move initializers to Constant nodes
         input_names = {i.name for i in graph.input}
         nodes.extend(
             onnx.helper.make_node("Constant", [], [i.name], value=i)
             for i in graph.initializer
             if i.name not in input_names
```

### Comparing `spox-0.7.0/src/spox/_internal_op.py` & `spox-0.8.0/src/spox/_internal_op.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,22 +170,22 @@
 
     def to_onnx(
         self, scope: Scope, doc_string: Optional[str] = None, build_subgraph=None
     ) -> List[onnx.NodeProto]:
         assert len(self.inputs.inputs) == len(self.outputs.outputs)
         # Just create a renaming identity from what we forwarded into our actual output
         protos = []
-        name = scope.node[self] if self in scope.node else None
+        name = scope.node[self]
         for i in range(len(self.inputs.inputs)):
             protos.append(
                 onnx.helper.make_node(
                     "Identity",
                     [scope.var[self.inputs.inputs[i]]],
                     [scope.var[self.outputs.outputs[i]]],
-                    name + f"_id{i}" if name is not None else None,
+                    name + f"_id{i}",
                     doc_string,
                 )
             )
         return protos
 
 
 def intros(*args: Var) -> Sequence[Var]:
```

### Comparing `spox-0.7.0/src/spox/_node.py` & `spox-0.8.0/src/spox/_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,14 @@
     INITIAL = 2
     OUTPUTS = 3
 
 
 _TYPE_WARNING_LEVEL: TypeWarningLevel = TypeWarningLevel.INITIAL
 
 
-def set_type_warning_level(level: TypeWarningLevel):
-    global _TYPE_WARNING_LEVEL
-    _TYPE_WARNING_LEVEL = level
-
-
 @dataclass(frozen=True)
 class OpType:
     """Stores information on an ONNX operator, like its identifier and domain."""
 
     identifier: str
     domain: str
     version: int
```

### Comparing `spox-0.7.0/src/spox/_patch_ref_impl.py` & `spox-0.8.0/src/spox/_patch_ref_impl.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/src/spox/_public.py` & `spox-0.8.0/src/spox/_public.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Module implementing the main public interface functions in Spox."""
 
 import contextlib
+import itertools
 from typing import Dict, Optional, Protocol
 
 import numpy as np
 import onnx
 from onnx.numpy_helper import to_array
 
 from . import _internal_op
 from ._attributes import AttrType
 from ._graph import Argument, initializer, results
 from ._inline import _Inline
+from ._standard import _strip_dim_symbol
 from ._type_system import Type
 from ._var import Var
 
 
 def argument(typ: Type) -> Var:
     """
     Create an argument variable which may be used as a model input.
@@ -137,14 +139,20 @@
         Returns
         -------
         Dict[str, Var]
             Variables representing the inlined model's outputs.
         """
 
 
+def _copy_model(model: onnx.ModelProto) -> onnx.ModelProto:
+    copied = onnx.ModelProto()
+    copied.CopyFrom(model)
+    return copied
+
+
 def inline(model: onnx.ModelProto) -> _InlineCall:
     """Inline an existing ONNX model, taking and producing ``Var``.
 
     Any valid model may be inlined. The behaviour of the ``model`` is
     replicated, its metadata (docstring, annotations) may be stripped.
     The opset imports of the target model are significant and the
     model itself may be adapted if its version is inconsistent.
@@ -190,24 +198,53 @@
     insertion point in the topological ordering.  Prefixing is applied
     (with the build system name) to attempt to avoid collisions.
 
     Initializers present in the model are replaced with Constant nodes,
     unless they are used as a default argument value. In this case
     they are also built as initializers.
 
+    Symbolic dimensions in input and output shapes are stripped from
+    the model and ignored, to avoid handling them inconsistently.
+
     Build behaviour should be treated as an implementation detail and
     may change.
 
+    Currently, inlining models with subgraphs or functions is not supported
+    as it cannot be performed in most cases due to lack of upstream support.
     """
     in_names = [i.name for i in model.graph.input]
     in_defaults = {i.name: i for i in model.graph.initializer}
     out_names = [o.name for o in model.graph.output]
     _defaults_msg = f" (defaults {list(in_defaults.keys())})"
     _signature_msg = f"signature {in_names}{_defaults_msg} -> {out_names}"
 
+    model = _copy_model(model)
+    # FIXME: Renaming does not work on subgraphs as of ONNX 1.13/1.14.
+    for node in model.graph.node:
+        for attr in node.attribute:
+            if attr.HasField("g") or attr.graphs:
+                raise ValueError(
+                    "Inlining models with subgraphs is not supported due to "
+                    "lack of upstream support for renaming values in subgraphs."
+                )
+    # FIXME: Support for functions is a bit involved, as it interacts with build.
+    if model.functions:
+        raise ValueError(
+            "Inlining models with functions is not supported. "
+            "Consider removing or inlining the function definitions "
+            "(if that preserves the model validity)."
+        )
+    # Handling symbolic dimensions is difficult and not particularly useful, so strip them
+    for info in itertools.chain(
+        model.graph.input, model.graph.output, model.graph.value_info
+    ):
+        info.type.CopyFrom(
+            _strip_dim_symbol(Type._from_onnx(info.type), lambda x: True)._to_onnx()
+        )
+
     def inline_inner(*args: Var, **kwargs: Var) -> Dict[str, Var]:
         for name, arg in zip(in_names, args):
             if name in kwargs:
                 raise TypeError(
                     f"inline callback got multiple values for argument '{name}', {_signature_msg}."
                 )
             kwargs[name] = arg
```

### Comparing `spox-0.7.0/src/spox/_schemas.py` & `spox-0.8.0/src/spox/_schemas.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/src/spox/_scope.py` & `spox-0.8.0/src/spox/_scope.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/src/spox/_shape.py` & `spox-0.8.0/src/spox/_shape.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/src/spox/_standard.py` & `spox-0.8.0/src/spox/_standard.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Module implementing a base for standard ONNX operators, which use the functionality of ONNX node-level inference."""
 import logging
-import typing
-from typing import Dict, Tuple
+from typing import TYPE_CHECKING, Callable, Dict, Tuple
 
 import numpy
 import onnx
 import onnx.reference
 import onnx.shape_inference
 from onnx.defs import OpSchema
 
@@ -15,15 +14,15 @@
 from ._schemas import SCHEMAS
 from ._scope import Scope
 from ._shape import SimpleShape
 from ._type_system import Optional, Sequence, Tensor, Type
 from ._utils import from_array
 from ._value_prop import PropValueType
 
-if typing.TYPE_CHECKING:
+if TYPE_CHECKING:
     from ._graph import Graph
 
 
 class StandardNode(Node):
     """
     Base type for a Node which has a known reference Schema (``self.schema``), extracted based on the ``op_type``.
     Implements ``infer_output_types_onnx``, which is used for type inference.
@@ -146,15 +145,18 @@
         # Recover the types from protobuf, ignoring empty protobuf objects for failing/unimplemented type inference.
         results = {
             info.name: Type._from_onnx(info.type)
             for info in typed_model.graph.output
             if info.type != onnx.TypeProto()
         }
         # Strips some unuseful type data (unknown dimensions become global-scoped dimension parameters).
-        return {key: _strip_unk_param(type_) for key, type_ in results.items()}
+        return {
+            key: _strip_dim_symbol(type_, lambda x: x.startswith("unk__"))
+            for key, type_ in results.items()
+        }
 
     def propagate_values_onnx(self) -> Dict[str, PropValueType]:
         """Perform value propagation by evaluating singleton model.
 
         The backend used for the propagation can be configured with the `spox._standard.ValuePropBackend` variable.
         """
         # Cannot do propagation when some inputs were not propagated/inferred
@@ -195,33 +197,35 @@
 
     def propagate_values(self) -> Dict[str, PropValueType]:
         if _value_prop._VALUE_PROP_BACKEND != _value_prop.ValuePropBackend.NONE:
             return self.propagate_values_onnx()
         return {}
 
 
-def _strip_unk_param_shape(shape: SimpleShape) -> SimpleShape:
+def _strip_dim_symbol_shape(
+    shape: SimpleShape, pred: Callable[[str], bool]
+) -> SimpleShape:
     """
     Remove all instances all ``unk__`` dimension parameters from a shape -- created when running
     ONNX shape inference and no parameter to use existed. It is stripped to avoid conflicts (due to global scoping).
     """
     if shape is None:
         return shape
-    xs = [None if isinstance(x, str) and x.startswith("unk__") else x for x in shape]
+    xs = [None if isinstance(x, str) and pred(x) else x for x in shape]
     return tuple(xs)
 
 
-def _strip_unk_param(typ: Type) -> Type:
+def _strip_dim_symbol(typ: Type, pred: Callable[[str], bool]) -> Type:
     """Apply ``_strip_unk_param_shape`` to all shapes present in this ``Type``."""
     if isinstance(typ, Tensor):
-        return Tensor(typ.dtype, _strip_unk_param_shape(typ.shape))
+        return Tensor(typ.dtype, _strip_dim_symbol_shape(typ.shape, pred))
     elif isinstance(typ, Sequence):
-        return Sequence(_strip_unk_param(typ.elem_type))
+        return Sequence(_strip_dim_symbol(typ.elem_type, pred))
     elif isinstance(typ, Optional):
-        return Optional(_strip_unk_param(typ.elem_type))
+        return Optional(_strip_dim_symbol(typ.elem_type, pred))
     else:
         return typ
 
 
 def _make_dummy_subgraph(_node: Node, key: str, graph: "Graph") -> onnx.GraphProto:
     """
     Make a dummy GraphProto that has inputs and outputs typed like Graph, without a graph body.
```

### Comparing `spox-0.7.0/src/spox/_traverse.py` & `spox-0.8.0/src/spox/_traverse.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/src/spox/_type_system.py` & `spox-0.8.0/src/spox/_type_system.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/src/spox/_utils.py` & `spox-0.8.0/src/spox/_utils.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/src/spox/_value_prop.py` & `spox-0.8.0/src/spox/_value_prop.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/src/spox/_var.py` & `spox-0.8.0/src/spox/_var.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/src/spox/opset/ai/onnx/ml/v3.py` & `spox-0.8.0/src/spox/opset/ai/onnx/ml/v3.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/src/spox/opset/ai/onnx/v17.py` & `spox-0.8.0/src/spox/opset/ai/onnx/v17.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/src/spox/opset/ai/onnx/v18.py` & `spox-0.8.0/src/spox/opset/ai/onnx/v18.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/src/spox.egg-info/PKG-INFO` & `spox-0.8.0/src/spox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spox
-Version: 0.7.0
+Version: 0.8.0
 Summary: A framework for constructing ONNX computational graphs.
 Author-email: Jakub Bachurski <kbachurski@gmail.com>, Christian Bourjau <christian.bourjau@quantco.com>
 Maintainer-email: Jakub Bachurski <kbachurski@gmail.com>, Christian Bourjau <christian.bourjau@quantco.com>
 Project-URL: Source, https://github.com/quantco/spox
 Keywords: machine-learning,onnx
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `spox-0.7.0/src/spox.egg-info/SOURCES.txt` & `spox-0.8.0/src/spox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/conftest.py` & `spox-0.8.0/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 
 import numpy
 import onnxruntime
 import pytest
 
 from spox import _value_prop
 from spox._debug import show_construction_tracebacks
+from spox._future import set_type_warning_level
 from spox._graph import Graph
-from spox._node import TypeWarningLevel, set_type_warning_level
+from spox._node import TypeWarningLevel
 
 set_type_warning_level(TypeWarningLevel.CRITICAL)
 _value_prop.VALUE_PROP_STRICT_CHECK = True
 
 
 class ONNXRuntimeHelper:
     _build_cache: Dict[Graph, bytes]
```

### Comparing `spox-0.7.0/tests/full/conftest.py` & `spox-0.8.0/tests/full/conftest.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/full/test_brackets.py` & `spox-0.8.0/tests/full/test_brackets.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/full/test_lifting.py` & `spox-0.8.0/tests/full/test_lifting.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/full/test_turing_completeness.py` & `spox-0.8.0/tests/full/test_turing_completeness.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/future/test_var_operators.py` & `spox-0.8.0/tests/future/test_var_operators.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/test_adapt.py` & `spox-0.8.0/tests/test_adapt.py`

 * *Files 21% similar despite different names*

```diff
@@ -29,14 +29,30 @@
     B = Squeeze<axes: floats = [0]>(A)
 }
 """
     )
 
 
 @pytest.fixture
+def old_identity() -> onnx.ModelProto:
+    return onnx.parser.parse_model(
+        """
+<
+ ir_version: 8,
+ opset_import: ["" : 13]
+>
+agraph (float[N] A) => (float[N] B)
+{
+    B = Identity(A)
+}
+    """
+    )
+
+
+@pytest.fixture
 def inline_old_squeeze_graph(old_squeeze):
     (data,) = arguments(
         data=Tensor(
             numpy.float32,
             (
                 1,
                 None,
@@ -44,14 +60,22 @@
         )
     )
     (result,) = inline(old_squeeze)(A=data).values()
     return results(final=result).with_opset(("ai.onnx", 17))
 
 
 @pytest.fixture
+def inline_old_identity_twice_graph(old_identity):
+    (x,) = arguments(data=Tensor(numpy.float32, (None,)))
+    (y,) = inline(old_identity)(A=x).values()
+    (z,) = inline(old_identity)(A=y).values()
+    return results(final=z).with_opset(("ai.onnx", 17))
+
+
+@pytest.fixture
 def old_squeeze_graph(old_squeeze):
     class Squeeze11(StandardNode):
         @dataclass
         class Attributes(BaseAttributes):
             axes: AttrInt64s
 
         @dataclass
@@ -93,14 +117,25 @@
             "final",
             data=numpy.array([[1, 2, 3, 4]], dtype=numpy.float32),
         ),
         [1, 2, 3, 4],
     )
 
 
+def test_adapts_inline_old_identity_twice(onnx_helper, inline_old_identity_twice_graph):
+    onnx_helper.assert_close(
+        onnx_helper.run(
+            inline_old_identity_twice_graph,
+            "final",
+            data=numpy.array([1, 2, 3, 4], dtype=numpy.float32),
+        ),
+        [1, 2, 3, 4],
+    )
+
+
 def test_adapts_singleton_old_squeeze(onnx_helper, old_squeeze_graph):
     onnx_helper.assert_close(
         onnx_helper.run(
             old_squeeze_graph,
             "final",
             data=numpy.array([[1, 2, 3, 4]], dtype=numpy.float32),
         ),
```

### Comparing `spox-0.7.0/tests/test_attr.py` & `spox-0.8.0/tests/test_attr.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/test_broadcast.py` & `spox-0.8.0/tests/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/test_constructors.py` & `spox-0.8.0/tests/test_constructors.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/test_custom_operator.py` & `spox-0.8.0/tests/test_custom_operator.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/test_equiv_types.py` & `spox-0.8.0/tests/test_equiv_types.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/test_function.py` & `spox-0.8.0/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/test_graph.py` & `spox-0.8.0/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/test_initializer.py` & `spox-0.8.0/tests/test_initializer.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/test_inline.py` & `spox-0.8.0/tests/test_inline.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pytest
 
 import spox.opset.ai.onnx.v17 as op
 from spox._graph import arguments, results
 from spox._public import inline
 from spox._type_system import Tensor
 from spox._utils import from_array
+from spox._var import Var
 
 
 @pytest.fixture
 def add_proto() -> onnx.ModelProto:
     return onnx.parser.parse_model(
         """
 <
@@ -89,14 +90,25 @@
     c = Identity(b)
 }
 """
     )
 
 
 @pytest.fixture
+def relu_proto() -> onnx.ModelProto:
+    (x,) = arguments(c=Tensor(float, ()))
+    (y,) = op.if_(
+        op.less(x, op.const(0.0)),
+        then_branch=lambda: (op.const(0.0),),
+        else_branch=lambda: (x,),
+    )
+    return results(y=y).with_arguments(x).to_onnx_model()
+
+
+@pytest.fixture
 def min_graph(lin_fun_proto):
     first, second = arguments(
         first=Tensor(numpy.float32, (None,)), second=Tensor(numpy.float32, (None,))
     )
     (result,) = inline(lin_fun_proto)(
         A=first, X=op.constant(value_float=1.0), B=second
     ).values()
@@ -226,7 +238,29 @@
 
     x, y = arguments(a=Tensor(float, ("N",)), b=Tensor(float, ("N",)))
     graph = results(c=proj(y, proj(x, y)))
 
     onnx_helper.assert_close(
         onnx_helper.run(graph, "c", a=numpy.array([1.0]), b=numpy.array([2.0])), 2
     )
+
+
+def test_relu_inline_subgraph_warns(onnx_helper, relu_proto):
+    (a,) = arguments(a=Tensor(float, ()))
+    with pytest.raises(ValueError):
+        inline(relu_proto)(a).values()
+
+
+@pytest.mark.skip("Inlining subgraphs requires reimplementing renaming in graphs.")
+def test_relu_inline_subgraph(onnx_helper, relu_proto):
+    (a,) = arguments(a=Tensor(float, ()))
+    (b,) = inline(relu_proto)(a).values()
+    graph = results(b=b).with_arguments(a)
+
+    onnx_helper.assert_close(onnx_helper.run(graph, "b", a=numpy.array([1.0])), 1.0)
+    onnx_helper.assert_close(onnx_helper.run(graph, "b", a=numpy.array([-1.0])), 0.0)
+
+
+def test_symbolic_dim_stripped(add4_graph):
+    x: Var
+    (x,) = add4_graph.requested_results.values()
+    assert x.unwrap_tensor().shape == (None,)
```

### Comparing `spox-0.7.0/tests/test_opsets.py` & `spox-0.8.0/tests/test_opsets.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/test_public.py` & `spox-0.8.0/tests/test_public.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/test_standard_op.py` & `spox-0.8.0/tests/test_standard_op.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/test_subgraphs.py` & `spox-0.8.0/tests/test_subgraphs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+from typing import Callable
+
 import numpy
 import pytest
 
 import spox.opset.ai.onnx.v17 as op
+from spox import Var
 from spox._future import initializer
 from spox._graph import arguments, results
 from spox._type_system import Sequence, Tensor
 
 
 def test_subgraph(onnx_helper):
     (e,) = arguments(e=Tensor(numpy.int64, ()))
@@ -329,14 +332,72 @@
             xs=[numpy.array([1]), numpy.array([2]), numpy.array([3])],
             ys=[numpy.array([-1]), numpy.array([0]), numpy.array([1])],
         ),
         [numpy.array([-2]), numpy.array([0]), numpy.array([6])],
     )
 
 
+def test_subgraph_result_depends_on_result(onnx_helper):
+    b, x = arguments(b=Tensor(numpy.bool_, ()), x=Tensor(numpy.int64, ()))
+    x = op.mul(x, op.const(2))
+    x1 = op.add(x, op.const(1))
+    z1, z2 = op.if_(b, then_branch=lambda: (x, x1), else_branch=lambda: (x1, x))
+    graph = results(z1=z1, z2=z2)
+    onnx_helper.assert_close(
+        onnx_helper.run(graph, "z1", b=numpy.array(True), x=numpy.array(5)),
+        [10],
+    )
+    onnx_helper.assert_close(
+        onnx_helper.run(graph, "z2", b=numpy.array(True), x=numpy.array(5)),
+        [11],
+    )
+
+
+@pytest.mark.parametrize("f3", ["fwd", "nest", "tee", "clone"])
+@pytest.mark.parametrize("f2", ["fwd", "nest", "tee", "clone"])
+@pytest.mark.parametrize("f1", ["fwd", "nest", "tee", "clone"])
+def test_complex_scope_trees_on_subgraph_argument(onnx_helper, f1, f2, f3):
+    def ident(arg: Callable[[], Var], fork) -> Var:
+        if fork == "clone":
+            fst, snd = arg(), arg()
+        else:
+            fst = snd = arg()
+        (ret,) = (
+            op.if_(
+                op.const(True),
+                then_branch=lambda: (fst,),
+                else_branch=lambda: (snd,) if fork != "nest" else (op.const(-1),),
+            )
+            if fork != "fwd"
+            else (fst,)
+        )
+        return ret
+
+    (_a,) = op.loop(
+        v_initial=[op.const(0)],
+        body=lambda _i, _c, a: (
+            op.const(False),
+            ident(
+                lambda: ident(
+                    lambda: ident(
+                        lambda: a,
+                        fork=f3,
+                    ),
+                    fork=f2,
+                ),
+                fork=f1,
+            ),
+        ),
+    )
+
+    (x,) = arguments(x=Tensor(int, ()))
+
+    results(_=_a).with_arguments(x).to_onnx_model()
+
+
 def test_subgraph_not_callback_raises():
     with pytest.raises(TypeError):
         op.if_(
             op.const(True),
             then_branch=[op.const(0)],  # type: ignore
             else_branch=[op.const(1)],  # type: ignore
         )
```

### Comparing `spox-0.7.0/tests/test_tensor.py` & `spox-0.8.0/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/test_type_translation.py` & `spox-0.8.0/tests/test_type_translation.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/test_value_propagation.py` & `spox-0.8.0/tests/test_value_propagation.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/type_inference/test_array_feature_extractor.py` & `spox-0.8.0/tests/type_inference/test_array_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/type_inference/test_compress.py` & `spox-0.8.0/tests/type_inference/test_compress.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/type_inference/test_imputer.py` & `spox-0.8.0/tests/type_inference/test_imputer.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/type_inference/test_label_encoder.py` & `spox-0.8.0/tests/type_inference/test_label_encoder.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/type_inference/test_linear_regressor.py` & `spox-0.8.0/tests/type_inference/test_linear_regressor.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/type_inference/test_one_hot.py` & `spox-0.8.0/tests/type_inference/test_one_hot.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/type_inference/test_one_hot_encoder.py` & `spox-0.8.0/tests/type_inference/test_one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/type_inference/test_scaler.py` & `spox-0.8.0/tests/type_inference/test_scaler.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tests/type_inference/test_tree_ensemble_classifier.py` & `spox-0.8.0/tests/type_inference/test_tree_ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tools/generate_opset.py` & `spox-0.8.0/tools/generate_opset.py`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tools/templates/class.jinja2` & `spox-0.8.0/tools/templates/class.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tools/templates/construct.jinja2` & `spox-0.8.0/tools/templates/construct.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tools/templates/constructor.jinja2` & `spox-0.8.0/tools/templates/constructor.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tools/templates/docstring.jinja2` & `spox-0.8.0/tools/templates/docstring.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tools/templates/extras/promote.jinja2` & `spox-0.8.0/tools/templates/extras/promote.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tools/templates/extras/xif.jinja2` & `spox-0.8.0/tools/templates/extras/xif.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tools/templates/extras/xloop.jinja2` & `spox-0.8.0/tools/templates/extras/xloop.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tools/templates/preamble.jinja2` & `spox-0.8.0/tools/templates/preamble.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tools/templates/type_inference/arrayfeatureextractor1.jinja2` & `spox-0.8.0/tools/templates/type_inference/arrayfeatureextractor1.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tools/templates/type_inference/compress11.jinja2` & `spox-0.8.0/tools/templates/type_inference/compress11.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tools/templates/type_inference/if16.jinja2` & `spox-0.8.0/tools/templates/type_inference/if16.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tools/templates/type_inference/imputer1.jinja2` & `spox-0.8.0/tools/templates/type_inference/imputer1.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tools/templates/type_inference/loop16.jinja2` & `spox-0.8.0/tools/templates/type_inference/loop16.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tools/templates/type_inference/onehot11.jinja2` & `spox-0.8.0/tools/templates/type_inference/onehot11.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tools/templates/type_inference/scaler1.jinja2` & `spox-0.8.0/tools/templates/type_inference/scaler1.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tools/templates/type_inference/treeensembleclassifier3.jinja2` & `spox-0.8.0/tools/templates/type_inference/treeensembleclassifier3.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.7.0/tools/templates/value_propagation/constant13.jinja2` & `spox-0.8.0/tools/templates/value_propagation/constant13.jinja2`

 * *Files identical despite different names*

