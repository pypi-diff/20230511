# Comparing `tmp/lc_python-2023.5.1.tar.gz` & `tmp/lc_python-2023.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lc_python-2023.5.1.tar", max compression
+gzip compressed data, was "lc_python-2023.5.2.tar", max compression
```

## Comparing `lc_python-2023.5.1.tar` & `lc_python-2023.5.2.tar`

### file list

```diff
@@ -1,107 +1,107 @@
--rw-r--r--   0        0        0      526 2023-05-10 02:02:08.710582 lc_python-2023.5.1/LICENSE
--rw-r--r--   0        0        0     4391 2023-05-10 02:02:08.711582 lc_python-2023.5.1/README.md
--rw-r--r--   0        0        0     5353 2023-05-11 09:35:49.202770 lc_python-2023.5.1/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-05-11 02:59:35.246223 lc_python-2023.5.1/src/node_red/__init__.py
--rwxr-xr-x   0        0        0    13303 2023-05-11 02:59:35.247223 lc_python-2023.5.1/src/node_red/draw/graph_easy.py
--rwxr-xr-x   0        0        0     6259 2023-05-11 02:59:35.248222 lc_python-2023.5.1/src/node_red/draw/layout.py
--rwxr-xr-x   0        0        0     3196 2023-05-11 02:59:35.248222 lc_python-2023.5.1/src/node_red/http_api.py
--rwxr-xr-x   0        0        0    19061 2023-05-11 02:59:35.249223 lc_python-2023.5.1/src/node_red/js/nodered/.config.nodes.json
--rwxr-xr-x   0        0        0       95 2023-05-10 23:07:04.949424 lc_python-2023.5.1/src/node_red/js/nodered/.config.runtime.json
--rwxr-xr-x   0        0        0     1156 2023-05-10 23:50:22.817493 lc_python-2023.5.1/src/node_red/js/nodered/.config.users.json
--rwxr-xr-x   0        0        0       26 2023-05-10 23:07:04.949424 lc_python-2023.5.1/src/node_red/js/nodered/ax/LICENSE
--rwxr-xr-x   0        0        0       25 2023-05-10 23:07:04.949424 lc_python-2023.5.1/src/node_red/js/nodered/ax/README.md
--rwxr-xr-x   0        0        0     4227 2023-05-10 23:07:04.949424 lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-cond.html
--rwxr-xr-x   0        0        0      402 2023-05-10 23:07:04.949424 lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-cond.js
--rwxr-xr-x   0        0        0    11868 2023-05-10 23:07:04.949424 lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-func/ax-func.html
--rwxr-xr-x   0        0        0      360 2023-05-10 23:07:04.949424 lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-func/ax-func.js
--rwxr-xr-x   0        0        0      894 2023-05-10 23:07:04.949424 lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-hub.html
--rwxr-xr-x   0        0        0    33511 2023-05-10 23:07:04.956424 lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-hub.js
--rwxr-xr-x   0        0        0    10363 2023-05-10 23:07:04.956424 lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-join/ax-join.html
--rwxr-xr-x   0        0        0      360 2023-05-10 23:07:04.956424 lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-join/ax-join.js
--rwxr-xr-x   0        0        0    35086 2023-05-10 23:07:04.957424 lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-join/locales/en-US/ax-join.json
--rwxr-xr-x   0        0        0     7827 2023-05-10 23:07:04.957424 lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-op.html
--rwxr-xr-x   0        0        0      591 2023-05-10 23:07:04.958424 lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-op.js
--rwxr-xr-x   0        0        0       22 2023-05-10 23:07:04.958424 lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-snk.html
--rwxr-xr-x   0        0        0     1916 2023-05-10 23:07:04.958424 lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-snk.js
--rwxr-xr-x   0        0        0       22 2023-05-10 23:07:04.958424 lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-src.html
--rwxr-xr-x   0        0        0      810 2023-05-10 23:07:04.958424 lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-src.js
--rwxr-xr-x   0        0        0      287 2023-05-10 23:07:04.958424 lc_python-2023.5.1/src/node_red/js/nodered/ax/icons/ax.svg
--rwxr-xr-x   0        0        0      273 2023-05-10 23:07:04.958424 lc_python-2023.5.1/src/node_red/js/nodered/ax/icons/ax_fit.svg
--rwxr-xr-x   0        0        0      273 2023-05-10 23:07:04.958424 lc_python-2023.5.1/src/node_red/js/nodered/ax/icons/parse-tr069.svg
--rwxr-xr-x   0        0        0    35033 2023-05-10 23:07:04.959424 lc_python-2023.5.1/src/node_red/js/nodered/ax/messages.json
--rwxr-xr-x   0        0        0      491 2023-05-10 23:07:04.959424 lc_python-2023.5.1/src/node_red/js/nodered/ax/package.json
--rwxr-xr-x   0        0        0      315 2023-05-10 23:07:04.959424 lc_python-2023.5.1/src/node_red/js/nodered/ax/restart_on_change
--rwxr-xr-x   0        0        0      453 2023-05-10 23:07:04.959424 lc_python-2023.5.1/src/node_red/js/nodered/ax/sync_local_to_nodered
--rwxr-xr-x   0        0        0     4650 2023-05-10 23:07:04.959424 lc_python-2023.5.1/src/node_red/js/nodered/ax/test/ax-hub_spec.js
--rwxr-xr-x   0        0        0     3964 2023-05-10 23:07:04.959424 lc_python-2023.5.1/src/node_red/js/nodered/ax/test/py/README.adoc
--rwxr-xr-x   0        0        0     5622 2023-05-10 23:07:04.960424 lc_python-2023.5.1/src/node_red/js/nodered/ax/test/py/ax_tr_069.py
--rwxr-xr-x   0        0        0     2567 2023-05-10 23:07:04.960424 lc_python-2023.5.1/src/node_red/js/nodered/ax/test/py/cpe.py
--rwxr-xr-x   0        0        0     6877 2023-05-10 23:07:04.960424 lc_python-2023.5.1/src/node_red/js/nodered/ax/test/py/server_for_python_tests.js
--rwxr-xr-x   0        0        0     1413 2023-05-10 23:07:04.960424 lc_python-2023.5.1/src/node_red/js/nodered/ax/test/py/simple.py
--rwxr-xr-x   0        0        0   116456 2023-05-10 23:07:04.961424 lc_python-2023.5.1/src/node_red/js/nodered/flows.json
--rwxr-xr-x   0        0        0    64206 2023-05-10 23:07:04.963424 lc_python-2023.5.1/src/node_red/js/nodered/flows_lib/wstest.json
--rwxr-xr-x   0        0        0      909 2023-05-10 23:07:04.963424 lc_python-2023.5.1/src/node_red/js/nodered/package.json
--rwxr-xr-x   0        0        0    20273 2023-05-10 23:07:04.964424 lc_python-2023.5.1/src/node_red/js/nodered/settings.js
--rwxr-xr-x   0        0        0    16226 2023-05-10 23:07:04.965424 lc_python-2023.5.1/src/node_red/nr_config_builder.py
--rwxr-xr-x   0        0        0    12085 2023-05-10 23:07:04.965424 lc_python-2023.5.1/src/node_red/nr_node_arranger.py
--rwxr-xr-x   0        0        0    20758 2023-05-10 23:07:04.966424 lc_python-2023.5.1/src/node_red/nrclient.py
--rwxr-xr-x   0        0        0    14067 2023-05-10 23:07:04.967424 lc_python-2023.5.1/src/node_red/nrtesting.py
--rwxr-xr-x   0        0        0     5277 2023-05-11 09:27:56.665880 lc_python-2023.5.1/src/node_red/operations/resources.py
--rwxr-xr-x   0        0        0     6110 2023-05-11 02:59:35.250223 lc_python-2023.5.1/src/node_red/operations/rsc_node.py
--rwxr-xr-x   0        0        0     9015 2023-05-11 02:59:35.250223 lc_python-2023.5.1/src/node_red/testing.py
--rwxr-xr-x   0        0        0      707 2023-05-10 23:07:04.968424 lc_python-2023.5.1/src/node_red/tools.py
--rwxr-xr-x   0        0        0     1017 2023-05-11 02:59:35.250223 lc_python-2023.5.1/src/operators/__init__.py
--rwxr-xr-x   0        0        0     2806 2023-05-11 02:59:35.251222 lc_python-2023.5.1/src/operators/arch/client_bootstrap.py
--rwxr-xr-x   0        0        0    11168 2023-05-11 02:59:35.251222 lc_python-2023.5.1/src/operators/arch/doc.py
--rwxr-xr-x   0        0        0     5165 2023-05-11 02:59:35.252223 lc_python-2023.5.1/src/operators/arch/functions.py
--rwxr-xr-x   0        0        0    38789 2023-05-10 02:02:08.779582 lc_python-2023.5.1/src/operators/build.py
--rwxr-xr-x   0        0        0     1555 2023-05-11 02:59:35.252223 lc_python-2023.5.1/src/operators/caches.py
--rwxr-xr-x   0        0        0       70 2023-05-11 02:59:35.252223 lc_python-2023.5.1/src/operators/con/__init__.py
--rwxr-xr-x   0        0        0     6041 2023-05-11 02:59:35.253223 lc_python-2023.5.1/src/operators/con/connections.py
--rwxr-xr-x   0        0        0     9786 2023-05-11 02:59:35.258222 lc_python-2023.5.1/src/operators/con/elastic.py
--rwxr-xr-x   0        0        0     3769 2023-05-11 02:59:35.259223 lc_python-2023.5.1/src/operators/con/file.py
--rwxr-xr-x   0        0        0    11562 2023-05-11 02:59:35.259223 lc_python-2023.5.1/src/operators/con/http.py
--rwxr-xr-x   0        0        0     5077 2023-05-11 02:59:35.260223 lc_python-2023.5.1/src/operators/con/kafka.py
--rwxr-xr-x   0        0        0     7978 2023-05-11 02:59:35.261222 lc_python-2023.5.1/src/operators/con/mysql.py
--rwxr-xr-x   0        0        0     8524 2023-05-11 02:59:35.261222 lc_python-2023.5.1/src/operators/con/proc.py
--rwxr-xr-x   0        0        0     3974 2023-05-10 02:02:08.781582 lc_python-2023.5.1/src/operators/con/proc_kafka_consume.py
--rwxr-xr-x   0        0        0     9270 2023-05-11 02:59:35.262223 lc_python-2023.5.1/src/operators/con/redis.py
--rwxr-xr-x   0        0        0     7076 2023-05-11 02:59:35.263223 lc_python-2023.5.1/src/operators/con/sock.py
--rwxr-xr-x   0        0        0     1852 2023-05-11 02:59:35.263223 lc_python-2023.5.1/src/operators/const.py
--rwxr-xr-x   0        0        0    10945 2023-05-11 02:59:35.264222 lc_python-2023.5.1/src/operators/core.py
--rwxr-xr-x   0        0        0     4572 2023-05-11 02:59:35.264222 lc_python-2023.5.1/src/operators/dec_enc.py
--rwxr-xr-x   0        0        0     3843 2023-05-11 02:59:35.265223 lc_python-2023.5.1/src/operators/err_handling.py
--rwxr-xr-x   0        0        0     1407 2023-05-11 02:59:35.265223 lc_python-2023.5.1/src/operators/kv_tools.py
--rwxr-xr-x   0        0        0     5073 2023-05-11 02:59:35.265223 lc_python-2023.5.1/src/operators/misc_util.py
--rwxr-xr-x   0        0        0     2294 2023-05-11 02:59:35.266223 lc_python-2023.5.1/src/operators/operations/resources.py
--rwxr-xr-x   0        0        0     3905 2023-05-11 02:59:35.266223 lc_python-2023.5.1/src/operators/operations/rsc_mysql.py
--rwxr-xr-x   0        0        0        0 2023-05-10 02:02:08.782582 lc_python-2023.5.1/src/operators/ops/__init__.py
--rwxr-xr-x   0        0        0     2960 2023-05-10 02:02:08.782582 lc_python-2023.5.1/src/operators/ops/cond.py
--rwxr-xr-x   0        0        0     3606 2023-05-11 02:59:35.267223 lc_python-2023.5.1/src/operators/ops/exceptions.py
--rwxr-xr-x   0        0        0    14130 2023-05-11 02:59:35.267223 lc_python-2023.5.1/src/operators/ops/funcs.py
--rwxr-xr-x   0        0        0     3898 2023-05-10 02:02:08.783582 lc_python-2023.5.1/src/operators/ops/join.py
--rwxr-xr-x   0        0        0    10898 2023-05-10 02:02:08.783582 lc_python-2023.5.1/src/operators/ops/op.py
--rwxr-xr-x   0        0        0     2969 2023-05-10 02:02:08.783582 lc_python-2023.5.1/src/operators/ops/src.py
--rwxr-xr-x   0        0        0    21971 2023-05-11 03:00:06.107210 lc_python-2023.5.1/src/operators/ops/subflow.py
--rwxr-xr-x   0        0        0     5881 2023-05-10 02:02:08.784582 lc_python-2023.5.1/src/operators/ops/tools.py
--rwxr-xr-x   0        0        0     1370 2023-05-10 02:02:08.784582 lc_python-2023.5.1/src/operators/plugins/app_operators/client.py
--rwxr-xr-x   0        0        0     8957 2023-05-10 02:02:08.784582 lc_python-2023.5.1/src/operators/plugins/app_operators/flow_file_tools.py
--rwxr-xr-x   0        0        0    38506 2023-05-11 02:59:35.269223 lc_python-2023.5.1/src/operators/plugins/app_operators/parse_state_table.py
--rwxr-xr-x   0        0        0    24506 2023-05-11 02:59:35.270223 lc_python-2023.5.1/src/operators/plugins/app_operators/pp
--rwxr-xr-x   0        0        0     4421 2023-05-11 02:59:35.270223 lc_python-2023.5.1/src/operators/plugins/app_operators/pymod_templates/multi_instance.py
--rwxr-xr-x   0        0        0     1870 2023-05-10 02:02:08.784582 lc_python-2023.5.1/src/operators/plugins/app_operators/term_flow_inspector.py
--rwxr-xr-x   0        0        0     4979 2023-05-10 02:02:08.784582 lc_python-2023.5.1/src/operators/plugins/app_operators/test_tools.py
--rwxr-xr-x   0        0        0       27 2023-05-11 02:59:35.271222 lc_python-2023.5.1/src/operators/plugins/con_operators/docs/kafka.md
--rwxr-xr-x   0        0        0     6758 2023-05-11 02:59:35.272223 lc_python-2023.5.1/src/operators/plugins/con_operators/kafka.py
--rwxr-xr-x   0        0        0    87091 2023-05-11 02:59:35.274222 lc_python-2023.5.1/src/operators/plugins/con_operators/kafka_assets/load.py
--rwxr-xr-x   0        0        0     1083 2023-05-11 02:59:35.274222 lc_python-2023.5.1/src/operators/post_processors.py
--rwxr-xr-x   0        0        0     3092 2023-05-11 02:59:35.275223 lc_python-2023.5.1/src/operators/prometheus.py
--rwxr-xr-x   0        0        0     1645 2023-05-11 02:59:35.276223 lc_python-2023.5.1/src/operators/snk.py
--rwxr-xr-x   0        0        0     1719 2023-05-11 02:59:35.276223 lc_python-2023.5.1/src/operators/src.py
--rwxr-xr-x   0        0        0     8750 2023-05-11 02:59:35.277222 lc_python-2023.5.1/src/operators/testing/auto_docs.py
--rwxr-xr-x   0        0        0     3841 2023-05-11 02:59:35.277222 lc_python-2023.5.1/src/operators/testing/mkdocstrings_pytest.py
--rwxr-xr-x   0        0        0     1739 2023-05-11 02:59:35.278223 lc_python-2023.5.1/src/operators/testing/redis.py
--rwxr-xr-x   0        0        0    14019 2023-05-10 02:02:08.786582 lc_python-2023.5.1/src/operators/testing/tools.py
--rwxr-xr-x   0        0        0     3993 2023-05-11 02:59:35.278223 lc_python-2023.5.1/src/operators/tools.py
--rw-r--r--   0        0        0     8315 1970-01-01 00:00:00.000000 lc_python-2023.5.1/setup.py
--rw-r--r--   0        0        0     5900 1970-01-01 00:00:00.000000 lc_python-2023.5.1/PKG-INFO
+-rw-r--r--   0        0        0      526 2023-05-10 02:02:08.710582 lc_python-2023.5.2/LICENSE
+-rw-r--r--   0        0        0     4391 2023-05-10 02:02:08.711582 lc_python-2023.5.2/README.md
+-rw-r--r--   0        0        0     5353 2023-05-11 15:39:01.744730 lc_python-2023.5.2/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-05-11 02:59:35.246223 lc_python-2023.5.2/src/node_red/__init__.py
+-rwxr-xr-x   0        0        0    13303 2023-05-11 02:59:35.247223 lc_python-2023.5.2/src/node_red/draw/graph_easy.py
+-rwxr-xr-x   0        0        0     6259 2023-05-11 02:59:35.248222 lc_python-2023.5.2/src/node_red/draw/layout.py
+-rwxr-xr-x   0        0        0     3196 2023-05-11 02:59:35.248222 lc_python-2023.5.2/src/node_red/http_api.py
+-rwxr-xr-x   0        0        0    19061 2023-05-11 02:59:35.249223 lc_python-2023.5.2/src/node_red/js/nodered/.config.nodes.json
+-rwxr-xr-x   0        0        0       95 2023-05-10 23:07:04.949424 lc_python-2023.5.2/src/node_red/js/nodered/.config.runtime.json
+-rwxr-xr-x   0        0        0     1156 2023-05-10 23:50:22.817493 lc_python-2023.5.2/src/node_red/js/nodered/.config.users.json
+-rwxr-xr-x   0        0        0       26 2023-05-10 23:07:04.949424 lc_python-2023.5.2/src/node_red/js/nodered/ax/LICENSE
+-rwxr-xr-x   0        0        0       25 2023-05-10 23:07:04.949424 lc_python-2023.5.2/src/node_red/js/nodered/ax/README.md
+-rwxr-xr-x   0        0        0     4227 2023-05-10 23:07:04.949424 lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-cond.html
+-rwxr-xr-x   0        0        0      402 2023-05-10 23:07:04.949424 lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-cond.js
+-rwxr-xr-x   0        0        0    11868 2023-05-10 23:07:04.949424 lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-func/ax-func.html
+-rwxr-xr-x   0        0        0      360 2023-05-10 23:07:04.949424 lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-func/ax-func.js
+-rwxr-xr-x   0        0        0      894 2023-05-10 23:07:04.949424 lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-hub.html
+-rwxr-xr-x   0        0        0    33511 2023-05-10 23:07:04.956424 lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-hub.js
+-rwxr-xr-x   0        0        0    10363 2023-05-10 23:07:04.956424 lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-join/ax-join.html
+-rwxr-xr-x   0        0        0      360 2023-05-10 23:07:04.956424 lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-join/ax-join.js
+-rwxr-xr-x   0        0        0    35086 2023-05-10 23:07:04.957424 lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-join/locales/en-US/ax-join.json
+-rwxr-xr-x   0        0        0     7827 2023-05-10 23:07:04.957424 lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-op.html
+-rwxr-xr-x   0        0        0      591 2023-05-10 23:07:04.958424 lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-op.js
+-rwxr-xr-x   0        0        0       22 2023-05-10 23:07:04.958424 lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-snk.html
+-rwxr-xr-x   0        0        0     1916 2023-05-10 23:07:04.958424 lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-snk.js
+-rwxr-xr-x   0        0        0       22 2023-05-10 23:07:04.958424 lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-src.html
+-rwxr-xr-x   0        0        0      810 2023-05-10 23:07:04.958424 lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-src.js
+-rwxr-xr-x   0        0        0      287 2023-05-10 23:07:04.958424 lc_python-2023.5.2/src/node_red/js/nodered/ax/icons/ax.svg
+-rwxr-xr-x   0        0        0      273 2023-05-10 23:07:04.958424 lc_python-2023.5.2/src/node_red/js/nodered/ax/icons/ax_fit.svg
+-rwxr-xr-x   0        0        0      273 2023-05-10 23:07:04.958424 lc_python-2023.5.2/src/node_red/js/nodered/ax/icons/parse-tr069.svg
+-rwxr-xr-x   0        0        0    35033 2023-05-10 23:07:04.959424 lc_python-2023.5.2/src/node_red/js/nodered/ax/messages.json
+-rwxr-xr-x   0        0        0      491 2023-05-10 23:07:04.959424 lc_python-2023.5.2/src/node_red/js/nodered/ax/package.json
+-rwxr-xr-x   0        0        0      315 2023-05-10 23:07:04.959424 lc_python-2023.5.2/src/node_red/js/nodered/ax/restart_on_change
+-rwxr-xr-x   0        0        0      453 2023-05-10 23:07:04.959424 lc_python-2023.5.2/src/node_red/js/nodered/ax/sync_local_to_nodered
+-rwxr-xr-x   0        0        0     4650 2023-05-10 23:07:04.959424 lc_python-2023.5.2/src/node_red/js/nodered/ax/test/ax-hub_spec.js
+-rwxr-xr-x   0        0        0     3964 2023-05-10 23:07:04.959424 lc_python-2023.5.2/src/node_red/js/nodered/ax/test/py/README.adoc
+-rwxr-xr-x   0        0        0     5622 2023-05-10 23:07:04.960424 lc_python-2023.5.2/src/node_red/js/nodered/ax/test/py/ax_tr_069.py
+-rwxr-xr-x   0        0        0     2567 2023-05-10 23:07:04.960424 lc_python-2023.5.2/src/node_red/js/nodered/ax/test/py/cpe.py
+-rwxr-xr-x   0        0        0     6877 2023-05-10 23:07:04.960424 lc_python-2023.5.2/src/node_red/js/nodered/ax/test/py/server_for_python_tests.js
+-rwxr-xr-x   0        0        0     1413 2023-05-10 23:07:04.960424 lc_python-2023.5.2/src/node_red/js/nodered/ax/test/py/simple.py
+-rwxr-xr-x   0        0        0   116456 2023-05-10 23:07:04.961424 lc_python-2023.5.2/src/node_red/js/nodered/flows.json
+-rwxr-xr-x   0        0        0    64206 2023-05-10 23:07:04.963424 lc_python-2023.5.2/src/node_red/js/nodered/flows_lib/wstest.json
+-rwxr-xr-x   0        0        0      909 2023-05-10 23:07:04.963424 lc_python-2023.5.2/src/node_red/js/nodered/package.json
+-rwxr-xr-x   0        0        0    20273 2023-05-10 23:07:04.964424 lc_python-2023.5.2/src/node_red/js/nodered/settings.js
+-rwxr-xr-x   0        0        0    16226 2023-05-10 23:07:04.965424 lc_python-2023.5.2/src/node_red/nr_config_builder.py
+-rwxr-xr-x   0        0        0    12085 2023-05-10 23:07:04.965424 lc_python-2023.5.2/src/node_red/nr_node_arranger.py
+-rwxr-xr-x   0        0        0    20758 2023-05-10 23:07:04.966424 lc_python-2023.5.2/src/node_red/nrclient.py
+-rwxr-xr-x   0        0        0    14067 2023-05-10 23:07:04.967424 lc_python-2023.5.2/src/node_red/nrtesting.py
+-rwxr-xr-x   0        0        0     5277 2023-05-11 09:27:56.665880 lc_python-2023.5.2/src/node_red/operations/resources.py
+-rwxr-xr-x   0        0        0     6110 2023-05-11 02:59:35.250223 lc_python-2023.5.2/src/node_red/operations/rsc_node.py
+-rwxr-xr-x   0        0        0     9015 2023-05-11 02:59:35.250223 lc_python-2023.5.2/src/node_red/testing.py
+-rwxr-xr-x   0        0        0      707 2023-05-10 23:07:04.968424 lc_python-2023.5.2/src/node_red/tools.py
+-rwxr-xr-x   0        0        0     1017 2023-05-11 02:59:35.250223 lc_python-2023.5.2/src/operators/__init__.py
+-rwxr-xr-x   0        0        0     2806 2023-05-11 02:59:35.251222 lc_python-2023.5.2/src/operators/arch/client_bootstrap.py
+-rwxr-xr-x   0        0        0    11168 2023-05-11 02:59:35.251222 lc_python-2023.5.2/src/operators/arch/doc.py
+-rwxr-xr-x   0        0        0     5165 2023-05-11 02:59:35.252223 lc_python-2023.5.2/src/operators/arch/functions.py
+-rwxr-xr-x   0        0        0    38789 2023-05-10 02:02:08.779582 lc_python-2023.5.2/src/operators/build.py
+-rwxr-xr-x   0        0        0     1555 2023-05-11 02:59:35.252223 lc_python-2023.5.2/src/operators/caches.py
+-rwxr-xr-x   0        0        0       70 2023-05-11 02:59:35.252223 lc_python-2023.5.2/src/operators/con/__init__.py
+-rwxr-xr-x   0        0        0     6041 2023-05-11 02:59:35.253223 lc_python-2023.5.2/src/operators/con/connections.py
+-rwxr-xr-x   0        0        0     9786 2023-05-11 02:59:35.258222 lc_python-2023.5.2/src/operators/con/elastic.py
+-rwxr-xr-x   0        0        0     3769 2023-05-11 02:59:35.259223 lc_python-2023.5.2/src/operators/con/file.py
+-rwxr-xr-x   0        0        0    11562 2023-05-11 02:59:35.259223 lc_python-2023.5.2/src/operators/con/http.py
+-rwxr-xr-x   0        0        0     5077 2023-05-11 02:59:35.260223 lc_python-2023.5.2/src/operators/con/kafka.py
+-rwxr-xr-x   0        0        0     7978 2023-05-11 02:59:35.261222 lc_python-2023.5.2/src/operators/con/mysql.py
+-rwxr-xr-x   0        0        0     8524 2023-05-11 02:59:35.261222 lc_python-2023.5.2/src/operators/con/proc.py
+-rwxr-xr-x   0        0        0     3974 2023-05-10 02:02:08.781582 lc_python-2023.5.2/src/operators/con/proc_kafka_consume.py
+-rwxr-xr-x   0        0        0     9270 2023-05-11 02:59:35.262223 lc_python-2023.5.2/src/operators/con/redis.py
+-rwxr-xr-x   0        0        0     7076 2023-05-11 02:59:35.263223 lc_python-2023.5.2/src/operators/con/sock.py
+-rwxr-xr-x   0        0        0     1852 2023-05-11 02:59:35.263223 lc_python-2023.5.2/src/operators/const.py
+-rwxr-xr-x   0        0        0    10945 2023-05-11 02:59:35.264222 lc_python-2023.5.2/src/operators/core.py
+-rwxr-xr-x   0        0        0     4572 2023-05-11 02:59:35.264222 lc_python-2023.5.2/src/operators/dec_enc.py
+-rwxr-xr-x   0        0        0     3843 2023-05-11 02:59:35.265223 lc_python-2023.5.2/src/operators/err_handling.py
+-rwxr-xr-x   0        0        0     1407 2023-05-11 02:59:35.265223 lc_python-2023.5.2/src/operators/kv_tools.py
+-rwxr-xr-x   0        0        0     5073 2023-05-11 02:59:35.265223 lc_python-2023.5.2/src/operators/misc_util.py
+-rwxr-xr-x   0        0        0     2294 2023-05-11 02:59:35.266223 lc_python-2023.5.2/src/operators/operations/resources.py
+-rwxr-xr-x   0        0        0     3905 2023-05-11 02:59:35.266223 lc_python-2023.5.2/src/operators/operations/rsc_mysql.py
+-rwxr-xr-x   0        0        0        0 2023-05-10 02:02:08.782582 lc_python-2023.5.2/src/operators/ops/__init__.py
+-rwxr-xr-x   0        0        0     2960 2023-05-10 02:02:08.782582 lc_python-2023.5.2/src/operators/ops/cond.py
+-rwxr-xr-x   0        0        0     3606 2023-05-11 02:59:35.267223 lc_python-2023.5.2/src/operators/ops/exceptions.py
+-rwxr-xr-x   0        0        0    14130 2023-05-11 02:59:35.267223 lc_python-2023.5.2/src/operators/ops/funcs.py
+-rwxr-xr-x   0        0        0     3898 2023-05-10 02:02:08.783582 lc_python-2023.5.2/src/operators/ops/join.py
+-rwxr-xr-x   0        0        0    10898 2023-05-10 02:02:08.783582 lc_python-2023.5.2/src/operators/ops/op.py
+-rwxr-xr-x   0        0        0     2969 2023-05-10 02:02:08.783582 lc_python-2023.5.2/src/operators/ops/src.py
+-rwxr-xr-x   0        0        0    21971 2023-05-11 03:00:06.107210 lc_python-2023.5.2/src/operators/ops/subflow.py
+-rwxr-xr-x   0        0        0     5881 2023-05-10 02:02:08.784582 lc_python-2023.5.2/src/operators/ops/tools.py
+-rwxr-xr-x   0        0        0     1370 2023-05-10 02:02:08.784582 lc_python-2023.5.2/src/operators/plugins/app_operators/client.py
+-rwxr-xr-x   0        0        0     8957 2023-05-10 02:02:08.784582 lc_python-2023.5.2/src/operators/plugins/app_operators/flow_file_tools.py
+-rwxr-xr-x   0        0        0    38506 2023-05-11 02:59:35.269223 lc_python-2023.5.2/src/operators/plugins/app_operators/parse_state_table.py
+-rwxr-xr-x   0        0        0    24506 2023-05-11 02:59:35.270223 lc_python-2023.5.2/src/operators/plugins/app_operators/pp
+-rwxr-xr-x   0        0        0     4421 2023-05-11 02:59:35.270223 lc_python-2023.5.2/src/operators/plugins/app_operators/pymod_templates/multi_instance.py
+-rwxr-xr-x   0        0        0     1870 2023-05-10 02:02:08.784582 lc_python-2023.5.2/src/operators/plugins/app_operators/term_flow_inspector.py
+-rwxr-xr-x   0        0        0     4979 2023-05-10 02:02:08.784582 lc_python-2023.5.2/src/operators/plugins/app_operators/test_tools.py
+-rwxr-xr-x   0        0        0       27 2023-05-11 02:59:35.271222 lc_python-2023.5.2/src/operators/plugins/con_operators/docs/kafka.md
+-rwxr-xr-x   0        0        0     6758 2023-05-11 02:59:35.272223 lc_python-2023.5.2/src/operators/plugins/con_operators/kafka.py
+-rwxr-xr-x   0        0        0    87091 2023-05-11 02:59:35.274222 lc_python-2023.5.2/src/operators/plugins/con_operators/kafka_assets/load.py
+-rwxr-xr-x   0        0        0     1083 2023-05-11 02:59:35.274222 lc_python-2023.5.2/src/operators/post_processors.py
+-rwxr-xr-x   0        0        0     3092 2023-05-11 02:59:35.275223 lc_python-2023.5.2/src/operators/prometheus.py
+-rwxr-xr-x   0        0        0     1645 2023-05-11 02:59:35.276223 lc_python-2023.5.2/src/operators/snk.py
+-rwxr-xr-x   0        0        0     1719 2023-05-11 02:59:35.276223 lc_python-2023.5.2/src/operators/src.py
+-rwxr-xr-x   0        0        0     8750 2023-05-11 02:59:35.277222 lc_python-2023.5.2/src/operators/testing/auto_docs.py
+-rwxr-xr-x   0        0        0     3841 2023-05-11 02:59:35.277222 lc_python-2023.5.2/src/operators/testing/mkdocstrings_pytest.py
+-rwxr-xr-x   0        0        0     1739 2023-05-11 02:59:35.278223 lc_python-2023.5.2/src/operators/testing/redis.py
+-rwxr-xr-x   0        0        0    14019 2023-05-10 02:02:08.786582 lc_python-2023.5.2/src/operators/testing/tools.py
+-rwxr-xr-x   0        0        0     3993 2023-05-11 02:59:35.278223 lc_python-2023.5.2/src/operators/tools.py
+-rw-r--r--   0        0        0     8315 1970-01-01 00:00:00.000000 lc_python-2023.5.2/setup.py
+-rw-r--r--   0        0        0     5900 1970-01-01 00:00:00.000000 lc_python-2023.5.2/PKG-INFO
```

### Comparing `lc_python-2023.5.1/LICENSE` & `lc_python-2023.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/README.md` & `lc_python-2023.5.2/README.md`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/pyproject.toml` & `lc_python-2023.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "lc-python"
-version = "2023.05.01"
+version = "2023.05.02"
 description = "AX Low Code: Node-RED/AX Server and Python Client Reference Implementation"
 authors = ["Gunther Klessinger <gunther.klessinger@axiros.com>"]
 license = "AxirosCommercialLicense"
 readme = "README.md"
 repository = "https://gitlab.axiros.com/klessinger/lc-python"
 homepage = "http://klessinger.pages.axiros.com/lc-python"
```

### Comparing `lc_python-2023.5.1/src/node_red/draw/graph_easy.py` & `lc_python-2023.5.2/src/node_red/draw/graph_easy.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/draw/layout.py` & `lc_python-2023.5.2/src/node_red/draw/layout.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/http_api.py` & `lc_python-2023.5.2/src/node_red/http_api.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/.config.nodes.json` & `lc_python-2023.5.2/src/node_red/js/nodered/.config.nodes.json`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/.config.users.json` & `lc_python-2023.5.2/src/node_red/js/nodered/.config.users.json`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-cond.html` & `lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-cond.html`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-func/ax-func.html` & `lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-func/ax-func.html`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-hub.html` & `lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-hub.html`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-hub.js` & `lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-hub.js`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-join/ax-join.html` & `lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-join/ax-join.html`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-join/locales/en-US/ax-join.json` & `lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-join/locales/en-US/ax-join.json`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-op.html` & `lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-op.html`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-op.js` & `lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-op.js`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-snk.js` & `lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-snk.js`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/ax/ax-src.js` & `lc_python-2023.5.2/src/node_red/js/nodered/ax/ax-src.js`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/ax/messages.json` & `lc_python-2023.5.2/src/node_red/js/nodered/ax/messages.json`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/ax/test/ax-hub_spec.js` & `lc_python-2023.5.2/src/node_red/js/nodered/ax/test/ax-hub_spec.js`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/ax/test/py/README.adoc` & `lc_python-2023.5.2/src/node_red/js/nodered/ax/test/py/README.adoc`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/ax/test/py/ax_tr_069.py` & `lc_python-2023.5.2/src/node_red/js/nodered/ax/test/py/ax_tr_069.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/ax/test/py/cpe.py` & `lc_python-2023.5.2/src/node_red/js/nodered/ax/test/py/cpe.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/ax/test/py/server_for_python_tests.js` & `lc_python-2023.5.2/src/node_red/js/nodered/ax/test/py/server_for_python_tests.js`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/ax/test/py/simple.py` & `lc_python-2023.5.2/src/node_red/js/nodered/ax/test/py/simple.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/flows.json` & `lc_python-2023.5.2/src/node_red/js/nodered/flows.json`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/flows_lib/wstest.json` & `lc_python-2023.5.2/src/node_red/js/nodered/flows_lib/wstest.json`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/package.json` & `lc_python-2023.5.2/src/node_red/js/nodered/package.json`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/js/nodered/settings.js` & `lc_python-2023.5.2/src/node_red/js/nodered/settings.js`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/nr_config_builder.py` & `lc_python-2023.5.2/src/node_red/nr_config_builder.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/nr_node_arranger.py` & `lc_python-2023.5.2/src/node_red/nr_node_arranger.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/nrclient.py` & `lc_python-2023.5.2/src/node_red/nrclient.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/nrtesting.py` & `lc_python-2023.5.2/src/node_red/nrtesting.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/operations/resources.py` & `lc_python-2023.5.2/src/node_red/operations/resources.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/operations/rsc_node.py` & `lc_python-2023.5.2/src/node_red/operations/rsc_node.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/testing.py` & `lc_python-2023.5.2/src/node_red/testing.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/node_red/tools.py` & `lc_python-2023.5.2/src/node_red/tools.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/__init__.py` & `lc_python-2023.5.2/src/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/arch/client_bootstrap.py` & `lc_python-2023.5.2/src/operators/arch/client_bootstrap.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/arch/doc.py` & `lc_python-2023.5.2/src/operators/arch/doc.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/arch/functions.py` & `lc_python-2023.5.2/src/operators/arch/functions.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/build.py` & `lc_python-2023.5.2/src/operators/build.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/caches.py` & `lc_python-2023.5.2/src/operators/caches.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/con/connections.py` & `lc_python-2023.5.2/src/operators/con/connections.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/con/elastic.py` & `lc_python-2023.5.2/src/operators/con/elastic.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/con/file.py` & `lc_python-2023.5.2/src/operators/con/file.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/con/http.py` & `lc_python-2023.5.2/src/operators/con/http.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/con/kafka.py` & `lc_python-2023.5.2/src/operators/con/kafka.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/con/mysql.py` & `lc_python-2023.5.2/src/operators/con/mysql.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/con/proc.py` & `lc_python-2023.5.2/src/operators/con/proc.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/con/proc_kafka_consume.py` & `lc_python-2023.5.2/src/operators/con/proc_kafka_consume.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/con/redis.py` & `lc_python-2023.5.2/src/operators/con/redis.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/con/sock.py` & `lc_python-2023.5.2/src/operators/con/sock.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/const.py` & `lc_python-2023.5.2/src/operators/const.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/core.py` & `lc_python-2023.5.2/src/operators/core.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/dec_enc.py` & `lc_python-2023.5.2/src/operators/dec_enc.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/err_handling.py` & `lc_python-2023.5.2/src/operators/err_handling.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/kv_tools.py` & `lc_python-2023.5.2/src/operators/kv_tools.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/misc_util.py` & `lc_python-2023.5.2/src/operators/misc_util.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/operations/resources.py` & `lc_python-2023.5.2/src/operators/operations/resources.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/operations/rsc_mysql.py` & `lc_python-2023.5.2/src/operators/operations/rsc_mysql.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/ops/cond.py` & `lc_python-2023.5.2/src/operators/ops/cond.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/ops/exceptions.py` & `lc_python-2023.5.2/src/operators/ops/exceptions.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/ops/funcs.py` & `lc_python-2023.5.2/src/operators/ops/funcs.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/ops/join.py` & `lc_python-2023.5.2/src/operators/ops/join.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/ops/op.py` & `lc_python-2023.5.2/src/operators/ops/op.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/ops/src.py` & `lc_python-2023.5.2/src/operators/ops/src.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/ops/subflow.py` & `lc_python-2023.5.2/src/operators/ops/subflow.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/ops/tools.py` & `lc_python-2023.5.2/src/operators/ops/tools.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/plugins/app_operators/client.py` & `lc_python-2023.5.2/src/operators/plugins/app_operators/client.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/plugins/app_operators/flow_file_tools.py` & `lc_python-2023.5.2/src/operators/plugins/app_operators/flow_file_tools.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/plugins/app_operators/parse_state_table.py` & `lc_python-2023.5.2/src/operators/plugins/app_operators/parse_state_table.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/plugins/app_operators/pp` & `lc_python-2023.5.2/src/operators/plugins/app_operators/pp`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/plugins/app_operators/pymod_templates/multi_instance.py` & `lc_python-2023.5.2/src/operators/plugins/app_operators/pymod_templates/multi_instance.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/plugins/app_operators/term_flow_inspector.py` & `lc_python-2023.5.2/src/operators/plugins/app_operators/term_flow_inspector.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/plugins/app_operators/test_tools.py` & `lc_python-2023.5.2/src/operators/plugins/app_operators/test_tools.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/plugins/con_operators/kafka.py` & `lc_python-2023.5.2/src/operators/plugins/con_operators/kafka.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/plugins/con_operators/kafka_assets/load.py` & `lc_python-2023.5.2/src/operators/plugins/con_operators/kafka_assets/load.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/post_processors.py` & `lc_python-2023.5.2/src/operators/post_processors.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/prometheus.py` & `lc_python-2023.5.2/src/operators/prometheus.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/snk.py` & `lc_python-2023.5.2/src/operators/snk.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/src.py` & `lc_python-2023.5.2/src/operators/src.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/testing/auto_docs.py` & `lc_python-2023.5.2/src/operators/testing/auto_docs.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/testing/mkdocstrings_pytest.py` & `lc_python-2023.5.2/src/operators/testing/mkdocstrings_pytest.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/testing/redis.py` & `lc_python-2023.5.2/src/operators/testing/redis.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/testing/tools.py` & `lc_python-2023.5.2/src/operators/testing/tools.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/src/operators/tools.py` & `lc_python-2023.5.2/src/operators/tools.py`

 * *Files identical despite different names*

### Comparing `lc_python-2023.5.1/setup.py` & `lc_python-2023.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
  'wsaccel>=0.6.2,<0.7.0']
 
 entry_points = \
 {'console_scripts': ['con = devapp.plugin_tools:main']}
 
 setup_kwargs = {
     'name': 'lc-python',
-    'version': '2023.5.1',
+    'version': '2023.5.2',
     'description': 'AX Low Code: Node-RED/AX Server and Python Client Reference Implementation',
     'long_description': '# This package\n\n<!-- badges -->\n\n[![docs pages][docs pages_img]][docs pages] [![gh-ci][gh-ci_img]][gh-ci] [![pkg][pkg_img]][pkg] [![code_style][code_style_img]][code_style]\n\n[docs pages]: http://klessinger.pages.axiros.com/lc-python\n[docs pages_img]: ./img/badge_docs.svg\n[gh-ci]: https://gitlab.axiros.com/klessinger/lc-python/actions/workflows/ci.yml\n[gh-ci_img]: https://gitlab.axiros.com/klessinger/lc-python/actions/workflows/ci.yml/badge.svg\n[pkg]: https://artifacts.axiros.com/artifactory/pypi-ax-sources/lc-python/2021.6.2/lc-python-2021.6.2.tar.gz\n[pkg_img]: ./img/badge_pypi.svg\n[code_style]: https://pypi.org/project/axblack/\n[code_style_img]: ./img/badge_axblack.svg\n\n<!-- badges -->\n\n[![docs][img_docs]][lnk_docs]&nbsp; [![package][img_package]][lnk_package]&nbsp; [![discuss][img_discuss]][lnk_discuss]&nbsp; [![pipeline][img_pipeline]][lnk_pipeline]&nbsp; [![code style][img_code style]][lnk_code style]\n\n[lnk_docs]: http://devapps.pages.axiros.com/lc-python\n[img_docs]: https://axchange.axiros.com/scm/hg/noauth/badges/raw-file/a2d5751cb09c/lc-python/documentation.svg\n[lnk_package]: https://artifacts.axiros.com/artifactory/pypi-ax-sources/lc-python/2020.12.09/lc-python-2020.12.09.tar.gz\n[img_package]: https://axchange.axiros.com/scm/hg/noauth/badges/raw-file/a2d5751cb09c/lc-python/pypi_package.svg\n[lnk_discuss]: https://join.skype.com/krSNYZqvEmJm\n[img_discuss]: https://axchange.axiros.com/scm/hg/noauth/badges/raw-file/a2d5751cb09c/lc-python/discuss.svg\n[lnk_pipeline]: https://gitlab.axiros.com/devapps/lc-python/-/commits/master\n[img_pipeline]: https://axchange.axiros.com/scm/hg/noauth/badges/raw-file/a2d5751cb09c/lc-python/pipeline.svg\n[lnk_code style]: https://github.com/axiros/axblack\n[img_code style]: https://axchange.axiros.com/scm/hg/noauth/badges/raw-file/a2d5751cb09c/lc-python/code_style_ax_black.svg\n\n## About\n![](img/page-teaser.png){: style="width:1550px"}\n\nAxiros Low Code Platform (AX/LC) allows for the building of complex data processing pipelines, from\n\n- an extendable set of small building blocks (operator functions)\n- a declarative, composable description file, which can be editted e.g. visually.\n\n> An often drawn analogy to that approach is the one with Lego, which also allows to build complex designs, based on a set of generic and some design specifig blocks, plus a manual, describing how to put them together - while still allowing customization to a large extent.\n\n### This Package\n\nThis is the core package for the Axiros Low Code Platform.\n\nIt contains:\n\n- The base platform ops and dev command line tools\n- The python reference implementation of the AX/LC data pipeline building protocol\n- The `ax.core` operator namespace, containing basic generic building blocks\n- The javascript running within Node-RED, enabling the AX/LC pipeline building protocol on Node-RED side.\n\n---\n\nLast modified: Fri Dec 18 17:10:06 2020\n\n<!-- pre_proc_marker -->\n\n---\n\n??? warning "Documentation was built with development versions of libs!"\n\n    - [lc-python](git@gitlab.axiros.com:devapps/lc-python.git)\n    ```\n    commit d06dbfa5a40cf8c0564a6eb26a43e81b4888a7ab\n    Author: Gunther Klessinger <gk@axiros.com>\n    Date:   Sat Jan 30 16:25:17 2021 +0100\n\n        ci: trigger CI (empty commit)\n\n    commit 23bdaa68dacb7d040414eff41a158ce3504e960e\n    Author: Gunther Klessinger <gk@axiros.com>\n    Date:   Sat Jan 30 15:54:00 2021 +0100\n\n        fix: No capture at tests\n    ```\n\n    - [lc-devapp](git@gitlab.axiros.com:devapps/lc-devapp.git)\n    ```\n    commit 520081be6a9c5181c60c80fa27f090edeb438ea7\n    Author: Gunther Klessinger <gk@axiros.com>\n    Date:   Sat Jan 30 18:16:42 2021 +0100\n\n        feat: ops lc can now kill services of other processes\n\n        ...and also supports s for start\n\n    commit 8b55380fe7ec718ec78358bcda0792686884a526\n    Author: Gunther Klessinger <gk@axiros.com>\n    Date:   Sat Jan 30 12:45:23 2021 +0100\n\n        chore: better output\n    ```\n\n    - [lc-doctools](git@gitlab.axiros.com:devapps/lc-doctools.git)\n    ```\n    commit ad5dd751b688d1a64d7eb4534f0a393f14c9d89c\n    Author: Gunther Klessinger <gk@axiros.com>\n    Date:   Thu Jan 21 11:05:21 2021 +0100\n\n        fix: flow -flows\n\n    commit 161cfd0b0ceb63889687ef897a9aa357352408fc\n    Author: Gunther Klessinger <gk@axiros.com>\n    Date:   Wed Jan 20 23:43:46 2021 +0100\n\n        fix: keep path in tmux\n    ```\n\nLast modified: Sun Jan 31 00:59:16 2021\n',
     'author': 'Gunther Klessinger',
     'author_email': 'gunther.klessinger@axiros.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'http://klessinger.pages.axiros.com/lc-python',
```

### Comparing `lc_python-2023.5.1/PKG-INFO` & `lc_python-2023.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lc-python
-Version: 2023.5.1
+Version: 2023.5.2
 Summary: AX Low Code: Node-RED/AX Server and Python Client Reference Implementation
 Home-page: http://klessinger.pages.axiros.com/lc-python
 License: AxirosCommercialLicense
 Author: Gunther Klessinger
 Author-email: gunther.klessinger@axiros.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

