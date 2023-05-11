# Comparing `tmp/tensorcircuit-nightly-0.9.0.dev20230509.tar.gz` & `tmp/tensorcircuit-nightly-0.9.0.dev20230510.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorcircuit-nightly-0.9.0.dev20230509.tar", last modified: Tue May  9 13:19:37 2023, max compression
+gzip compressed data, was "tensorcircuit-nightly-0.9.0.dev20230510.tar", last modified: Wed May 10 12:40:11 2023, max compression
```

## Comparing `tensorcircuit-nightly-0.9.0.dev20230509.tar` & `tensorcircuit-nightly-0.9.0.dev20230510.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.266651 tensorcircuit-nightly-0.9.0.dev20230509/
--rw-r--r--   0 runner    (1001) docker     (122)    24079 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    20682 2023-05-09 13:19:37.266651 tensorcircuit-nightly-0.9.0.dev20230509/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    18300 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     6048 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/README_cn.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.254651 tensorcircuit-nightly-0.9.0.dev20230509/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.258651 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/advance.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/cnconf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6397 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/contribution.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/generate_rst.py
--rw-r--r--   0 runner    (1001) docker     (122)     2985 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8695 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/infras.rst
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/modules.rst.backup
--rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/sharpbits.rst
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/textbooktoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/tutorial_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/whitepapertoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/whitepapertoc_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-09 13:19:37.266651 tensorcircuit-nightly-0.9.0.dev20230509/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-09 13:19:30.000000 tensorcircuit-nightly-0.9.0.dev20230509/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.258651 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-09 13:19:30.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/about.py
--rw-r--r--   0 runner    (1001) docker     (122)    39188 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/abstractcircuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.262651 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/dqas.py
--rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/graphdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/vags.py
--rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/van.py
--rw-r--r--   0 runner    (1001) docker     (122)    23156 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/vqes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/asciiart.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.262651 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/abstract_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/backend_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/cupy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/jax_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/jax_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/pytorch_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/pytorch_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    31112 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/tf_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/basecircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.262651 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/abstraction.py
--rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/apis.py
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/quafu_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)    14212 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/tencent.py
--rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7968 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.262651 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/compiler/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2945 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/compiler/composed_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     6032 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/compiler/qiskit_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     7791 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/compiler/simple_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    29573 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cons.py
--rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/densitymatrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/gates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.262651 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/numpy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/scipy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/tensortrans.py
--rw-r--r--   0 runner    (1001) docker     (122)     5030 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/torch.py
--rw-r--r--   0 runner    (1001) docker     (122)    10126 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/keras.py
--rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/mps_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    34350 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/quantum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.262651 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/results/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/results/counts.py
--rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/results/readout_mitigation.py
--rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/simplify.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.262651 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/chems.py
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/graphs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/measurements.py
--rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/translation.py
--rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.266651 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    20682 2023-05-09 13:19:36.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3561 2023-05-09 13:19:36.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 13:19:36.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-09 13:19:36.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-09 13:19:36.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.266651 tensorcircuit-nightly-0.9.0.dev20230509/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    33394 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_calibrating.py
--rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    46467 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     4204 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_dmcircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_miscs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_qaoa.py
--rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_quantum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_quantum_attr.py
--rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_van.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:40:11.444956 tensorcircuit-nightly-0.9.0.dev20230510/
+-rw-r--r--   0 runner    (1001) docker     (122)    24112 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    20682 2023-05-10 12:40:11.444956 tensorcircuit-nightly-0.9.0.dev20230510/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    18300 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     6048 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/README_cn.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:40:11.408954 tensorcircuit-nightly-0.9.0.dev20230510/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:40:11.420955 tensorcircuit-nightly-0.9.0.dev20230510/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/docs/source/advance.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/docs/source/cnconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6397 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/docs/source/contribution.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/docs/source/generate_rst.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2985 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8695 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/docs/source/infras.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/docs/source/modules.rst.backup
+-rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/docs/source/sharpbits.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/docs/source/textbooktoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/docs/source/tutorial_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/docs/source/whitepapertoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/docs/source/whitepapertoc_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-10 12:40:11.444956 tensorcircuit-nightly-0.9.0.dev20230510/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-10 12:40:04.000000 tensorcircuit-nightly-0.9.0.dev20230510/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:40:11.424955 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-10 12:40:04.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/about.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39188 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/abstractcircuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:40:11.428955 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/applications/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/applications/dqas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/applications/graphdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/applications/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/applications/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/applications/vags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/applications/van.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23156 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/applications/vqes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/asciiart.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:40:11.432955 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/abstract_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/backend_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/cupy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/jax_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/jax_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/pytorch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/pytorch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31112 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/tf_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/basecircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:40:11.436956 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/cloud/abstraction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/cloud/apis.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/cloud/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/cloud/quafu_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14212 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/cloud/tencent.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7787 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/cloud/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:40:11.436956 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/compiler/composed_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6032 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/compiler/qiskit_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9230 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/compiler/simple_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29573 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/cons.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/densitymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/gates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:40:11.436956 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/interfaces/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/interfaces/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/interfaces/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/interfaces/tensortrans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5030 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/interfaces/torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10126 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/mps_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34350 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/quantum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:40:11.440956 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/results/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/results/counts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/results/readout_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/simplify.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:40:11.440956 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/templates/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/templates/chems.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/templates/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/templates/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/templates/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/templates/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/translation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:40:11.440956 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    20682 2023-05-10 12:40:11.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3561 2023-05-10 12:40:11.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 12:40:11.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-10 12:40:11.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-10 12:40:11.000000 tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:40:11.444956 tensorcircuit-nightly-0.9.0.dev20230510/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33394 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_calibrating.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46467 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4204 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_dmcircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_miscs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_quantum_attr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-05-10 12:17:05.000000 tensorcircuit-nightly-0.9.0.dev20230510/tests/test_van.py
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/CHANGELOG.md` & `tensorcircuit-nightly-0.9.0.dev20230510/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 - Add simplecompiler module to assite qiskit compile for better performance when targeting rz native basis
 
 ### Changed
 
 - Add compiler and cloud namespace to the global tensorcircuit namespace
 
-- Refactor composed compiler pipeline interface to include simple_compiler (breaking)
+- Refactor composed compiler pipeline interface to include simple_compiler, using `DefaultCompiler` for now (breaking)
 
 ## 0.9.0
 
 ### Added
 
 - Cloud module for Tencent QCloud is now merged into the master branch and ready to release
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/HISTORY.md` & `tensorcircuit-nightly-0.9.0.dev20230510/HISTORY.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/LICENSE` & `tensorcircuit-nightly-0.9.0.dev20230510/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/PKG-INFO` & `tensorcircuit-nightly-0.9.0.dev20230510/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.0.dev20230509
+Version: 0.9.0.dev20230510
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/README.md` & `tensorcircuit-nightly-0.9.0.dev20230510/README.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/README_cn.md` & `tensorcircuit-nightly-0.9.0.dev20230510/README_cn.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/advance.rst` & `tensorcircuit-nightly-0.9.0.dev20230510/docs/source/advance.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/cnconf.py` & `tensorcircuit-nightly-0.9.0.dev20230510/docs/source/cnconf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/conf.py` & `tensorcircuit-nightly-0.9.0.dev20230510/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/contribution.rst` & `tensorcircuit-nightly-0.9.0.dev20230510/docs/source/contribution.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/faq.rst` & `tensorcircuit-nightly-0.9.0.dev20230510/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/generate_rst.py` & `tensorcircuit-nightly-0.9.0.dev20230510/docs/source/generate_rst.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/index.rst` & `tensorcircuit-nightly-0.9.0.dev20230510/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/infras.rst` & `tensorcircuit-nightly-0.9.0.dev20230510/docs/source/infras.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/modules.rst` & `tensorcircuit-nightly-0.9.0.dev20230510/docs/source/modules.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/modules.rst.backup` & `tensorcircuit-nightly-0.9.0.dev20230510/docs/source/modules.rst.backup`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/quickstart.rst` & `tensorcircuit-nightly-0.9.0.dev20230510/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/sharpbits.rst` & `tensorcircuit-nightly-0.9.0.dev20230510/docs/source/sharpbits.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/tutorial.rst` & `tensorcircuit-nightly-0.9.0.dev20230510/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/tutorial_cn.rst` & `tensorcircuit-nightly-0.9.0.dev20230510/docs/source/tutorial_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/whitepapertoc_cn.rst` & `tensorcircuit-nightly-0.9.0.dev20230510/docs/source/whitepapertoc_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/setup.py` & `tensorcircuit-nightly-0.9.0.dev20230510/setup.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/__init__.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.0.dev20230509"
+__version__ = "0.9.0.dev20230510"
 __author__ = "TensorCircuit Authors"
 __creator__ = "refraction-ray"
 
 from .utils import gpu_memory_share
 
 gpu_memory_share()
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/about.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/about.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/abstractcircuit.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/abstractcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/dqas.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/applications/dqas.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/graphdata.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/applications/graphdata.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/layers.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/applications/layers.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/utils.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/applications/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/vags.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/applications/vags.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/van.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/applications/van.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/vqes.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/applications/vqes.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/asciiart.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/asciiart.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/abstract_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/backend_factory.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/backend_factory.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/cupy_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/cupy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/jax_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/jax_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/jax_ops.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/jax_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/numpy_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/pytorch_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/pytorch_ops.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/pytorch_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/tensorflow_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/tf_ops.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/backends/tf_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/basecircuit.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/basecircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/channels.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/circuit.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/abstraction.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/cloud/abstraction.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/apis.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/cloud/apis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/local.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/cloud/local.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/quafu_provider.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/cloud/quafu_provider.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/tencent.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/cloud/tencent.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/utils.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/wrapper.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/cloud/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from ..circuit import Circuit
 from ..results import counts
 from ..results.readout_mitigation import ReadoutMit
 from ..utils import is_sequence
 from ..cons import backend
 from ..quantum import ps2xyz
-from ..compiler.qiskit_compiler import qiskit_compile
+from ..compiler import DefaultCompiler
 from .apis import submit_task, get_device
 from .abstraction import Device
 
 
 logger = logging.getLogger(__name__)
 Tensor = Any
 
@@ -133,38 +133,36 @@
         else:
             return backend.real(backend.sum([w * r for w, r in zip(ws, results)]))
     cs = []
     infos = []
     exps = []
     if isinstance(device, str):
         device = get_device(device)
+
+    dc = DefaultCompiler(
+        {
+            "coupling_map": device.topology(),
+        }
+    )
     for ps in pss:
         # TODO(@refraction-ray): Pauli string grouping
         # https://docs.pennylane.ai/en/stable/_modules/pennylane/pauli/grouping/group_observables.html
         c1 = Circuit.from_qir(c.to_qir())
         exp = []
         for j, i in enumerate(ps):
             if i == 1:
                 c1.H(j)  # type: ignore
                 exp.append(j)
             elif i == 2:
                 c1.rx(j, theta=np.pi / 2)  # type: ignore
                 exp.append(j)
             elif i == 3:
                 exp.append(j)
-        c1, info = qiskit_compile(
-            c1,
-            compiled_options={
-                "basis_gates": device.native_gates() + ["cx"],
-                # whether + "cx" here?
-                "optimization_level": 2,
-                "coupling_map": device.topology(),
-            },
-        )
-        # change the compiler to DefaultCompiler when it matures
+        c1, info = dc(c1)
+        # TODO(@refraction-ray): two steps compiling with pre compilation
         cs.append(c1)
         infos.append(info)
         exps.append(exp)
 
     reduced_cs = []
     reduced_dict = {}
     recover_dict = {}
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/compiler/composed_compiler.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/compiler/composed_compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 object oriented compiler pipeline
 """
 
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from ..utils import is_sequence
 from ..abstractcircuit import AbstractCircuit
 from .qiskit_compiler import qiskit_compile
 from .simple_compiler import simple_compile
 
 
@@ -68,7 +68,17 @@
         # rz target is bad for qiskit
         if qiskit_compiled_options:
             compiled_options.update(qiskit_compiled_options)
         super().__init__(
             [qiskit_compile, simple_compile],
             [compiled_options, None],  # type: ignore
         )
+
+
+def default_compile(
+    circuit: AbstractCircuit,
+    info: Optional[Dict[str, Any]] = None,
+    compiled_options: Optional[Dict[str, Any]] = None,
+) -> Tuple[AbstractCircuit, Dict[str, Any]]:
+    dc = DefaultCompiler(compiled_options)
+    c, info = dc(circuit, info)
+    return c, info  # type: ignore
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/compiler/qiskit_compiler.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/compiler/qiskit_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/compiler/simple_compiler.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/compiler/simple_compiler.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Very simple transformations that qiskit may even fail or hard to control
 """
 
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple, Union
 from copy import copy
 
 import numpy as np
 
 from ..abstractcircuit import AbstractCircuit
 from ..cons import backend
 from ..quantum import QuOperator
@@ -89,38 +89,69 @@
                 c.apply_general_variable_gate_delayed(
                     d["gatef"], d["name"], mpo=d["mpo"]
                 )(c, *d["index"], **d["parameters"], split=d["split"])
 
     return c  # type: ignore
 
 
+def _get_matrix(qir_item: Dict[str, Any]) -> Any:
+    if "gate" in qir_item:
+        op = qir_item["gate"]
+    else:
+        op = qir_item["gatef"](**qir_item["parameters"])
+    if isinstance(op, QuOperator):
+        m = backend.numpy(op.eval_matrix())
+    else:
+        m = backend.numpy(backend.reshapem(op.tensor))
+    return m
+
+
 def prune(
-    circuit: AbstractCircuit, rtol: float = 1e-3, atol: float = 1e-3, **kws: Any
-) -> AbstractCircuit:
-    qir = circuit.to_qir()
-    c = type(circuit)(**circuit.circuit_param)
-    for d in qir:
-        if isinstance(d["gate"], QuOperator):
-            m = backend.numpy(d["gate"].eval_matrix())
-        else:
-            m = backend.numpy(backend.reshapem(d["gate"].tensor))
-        if not np.allclose(
-            m / (m[0, 0] + 1e-8), np.eye(m.shape[0]), rtol=rtol, atol=atol
-        ):
-            # upto a phase
-            if "parameters" not in d:
-                c.apply_general_gate_delayed(d["gatef"], d["name"], mpo=d["mpo"])(
-                    c, *d["index"], split=d["split"]
-                )
-            else:
-                c.apply_general_variable_gate_delayed(
-                    d["gatef"], d["name"], mpo=d["mpo"]
-                )(c, *d["index"], **d["parameters"], split=d["split"])
+    circuit: Union[AbstractCircuit, List[Dict[str, Any]]],
+    rtol: float = 1e-3,
+    atol: float = 1e-3,
+    **kws: Any
+) -> Any:
+    if isinstance(circuit, list):
+        qir = circuit
+        output = "qir"
+    else:
+        qir = circuit.to_qir()
+        output = "tc"
+    if output in ["tc", "circuit"]:
+        c: Any = type(circuit)(**circuit.circuit_param)  # type: ignore
+        for d in qir:
+            m = _get_matrix(d)
 
-    return c
+            if not np.allclose(
+                m / (m[0, 0] + 1e-8), np.eye(m.shape[0]), rtol=rtol, atol=atol
+            ):
+                # upto a phase
+                if "parameters" not in d:
+                    c.apply_general_gate_delayed(d["gatef"], d["name"], mpo=d["mpo"])(
+                        c, *d["index"], split=d["split"]
+                    )
+                else:
+                    c.apply_general_variable_gate_delayed(
+                        d["gatef"], d["name"], mpo=d["mpo"]
+                    )(c, *d["index"], **d["parameters"], split=d["split"])
+        return c
+
+    elif output in ["qir"]:
+        nqir = []
+        for d in qir:
+            m = _get_matrix(d)
+
+            if not np.allclose(
+                m / (m[0, 0] + 1e-8), np.eye(m.shape[0]), rtol=rtol, atol=atol
+            ):
+                nqir.append(d)
+                # upto a phase
+
+        return nqir
 
 
 # upto global phase
 default_merge_rules = {
     ("s", "s"): "z",
     ("sd", "sd"): "z",
     ("t", "t"): "s",
@@ -147,16 +178,19 @@
     ("cnot", "cnot"): "i",
     ("cz", "cz"): "i",
     ("cy", "cy"): "i",
 }
 
 
 def _find_next(qir: List[Dict[str, Any]], i: int) -> Optional[int]:
+    # if qir[i] is None:
+    # return None
     index = qir[i]["index"]
     for j, item in enumerate(qir[i + 1 :]):
+        # if item is not None:
         if item["index"] == index:
             return j + i + 1
         for ind in item["index"]:
             if ind in index:
                 return None
     return None
 
@@ -168,79 +202,98 @@
     return theta  # type: ignore
 
 
 def _merge(
     qir: List[Dict[str, Any]], rules: Dict[Tuple[str, ...], str]
 ) -> Tuple[List[Dict[str, Any]], bool]:
     i = 0
+    flg = False
     while i < len(qir) - 1:
         j = _find_next(qir, i)
 
         if j is not None:
             if (qir[i]["gatef"].n, qir[j]["gatef"].n) in rules:
                 nn = rules[(qir[i]["gatef"].n, qir[j]["gatef"].n)]
                 if nn == "i":
                     del qir[i]
                     del qir[j - 1]
+                    # qir[i] = None
+                    # qir[j] = None
                 else:
                     param = {}
                     if nn.startswith("r") or nn.startswith("cr"):
                         param = {"theta": _get_theta(qir[i]) + _get_theta(qir[j])}
                     qir[i] = {
                         "gatef": getattr(gates, nn),
                         "name": nn,
                         "mpo": False,
                         "split": False,
                         "parameters": param,
                         "index": qir[i]["index"],
                     }
                     del qir[j]
-                return qir, True
+                    # qir[j] = None
+                flg = True
+                # return qir, flg
             elif (
                 qir[i]["gatef"].n == qir[j]["gatef"].n + "d"
                 or qir[i]["gatef"].n + "d" == qir[j]["gatef"].n
             ):
                 del qir[i]
                 del qir[j - 1]
-                return qir, True
+                # qir[i] = None
+                # qir[j] = None
+                flg = True
+                # return qir, True
         i += 1
-    return qir, False
+    return qir, flg
 
 
 def merge(
-    circuit: AbstractCircuit,
+    circuit: Union[AbstractCircuit, List[Dict[str, Any]]],
     rules: Optional[Dict[Tuple[str, ...], str]] = None,
     **kws: Any
-) -> AbstractCircuit:
+) -> Any:
     merge_rules = copy(default_merge_rules)
     if rules is not None:
         merge_rules.update(rules)  # type: ignore
-
-    qir = circuit.to_qir()
+    if isinstance(circuit, list):
+        qir = circuit
+        output = "qir"
+    else:
+        qir = circuit.to_qir()
+        output = "tc"
     flg = True
     while flg:
         qir, flg = _merge(qir, merge_rules)  # type: ignore
-    c = type(circuit).from_qir(qir, circuit.circuit_param)
-    return c
+    if output in ["qir"]:
+        return qir
+    elif output in ["tc", "circuit"]:
+        c: Any = type(circuit).from_qir(qir, circuit.circuit_param)  # type: ignore
+        return c
 
 
 def simple_compile(
     circuit: Any,
     info: Optional[Dict[str, Any]] = None,
     output: str = "tc",
     compiled_options: Optional[Dict[str, Any]] = None,
 ) -> Any:
     if compiled_options is None:
         compiled_options = {}
     c = replace_r(circuit, **compiled_options)
     c = replace_u(circuit, **compiled_options)
-    qasm = c.to_openqasm()
-    c = merge(c, **compiled_options)
-    c = prune(c, **compiled_options)
-    qasm1 = c.to_openqasm()
-    while qasm1 != qasm:
-        qasm = qasm1
-        c = merge(c, **compiled_options)
-        c = prune(c, **compiled_options)
-        qasm1 = c.to_openqasm()
+    qir = c.to_qir()
+    len0 = len(qir)
+    qir = merge(qir, **compiled_options)
+    qir = prune(qir, **compiled_options)
+    len1 = len(qir)
+    while len1 != len0:
+        len0 = len1
+        qir = merge(qir, **compiled_options)
+        if len(qir) == len0:
+            break
+        qir = prune(qir, **compiled_options)
+        len1 = len(qir)
 
+    c = type(circuit).from_qir(qir, circuit.circuit_param)
     return (c, info)
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cons.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/cons.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/densitymatrix.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/experimental.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/experimental.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/gates.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/numpy.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/interfaces/numpy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/scipy.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/interfaces/scipy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/tensorflow.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/interfaces/tensorflow.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/tensortrans.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/interfaces/tensortrans.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/torch.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/interfaces/torch.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/keras.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/mps_base.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/mps_base.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/mpscircuit.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/noisemodel.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/quantum.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/results/counts.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/results/counts.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/results/readout_mitigation.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/results/readout_mitigation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/simplify.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/blocks.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/templates/blocks.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/chems.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/templates/chems.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/dataset.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/templates/dataset.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/ensemble.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/templates/ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/graphs.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/templates/graphs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/measurements.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/templates/measurements.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/torchnn.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/translation.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/translation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/utils.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/vis.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit/vis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit_nightly.egg-info/PKG-INFO` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.0.dev20230509
+Version: 0.9.0.dev20230510
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit_nightly.egg-info/SOURCES.txt` & `tensorcircuit-nightly-0.9.0.dev20230510/tensorcircuit_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/conftest.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_backends.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_calibrating.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_calibrating.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_channels.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_circuit.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_cloud.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_compiler.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_dmcircuit.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_dmcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_ensemble.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_gates.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_interfaces.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_keras.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_miscs.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_miscs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_mpscircuit.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_noisemodel.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_qaoa.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_qaoa.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_quantum.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_quantum_attr.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_quantum_attr.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_results.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_simplify.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_templates.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_torchnn.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_van.py` & `tensorcircuit-nightly-0.9.0.dev20230510/tests/test_van.py`

 * *Files identical despite different names*

