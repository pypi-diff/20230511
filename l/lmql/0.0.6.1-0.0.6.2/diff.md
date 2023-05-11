# Comparing `tmp/lmql-0.0.6.1.tar.gz` & `tmp/lmql-0.0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmql-0.0.6.1.tar", last modified: Wed May  3 14:15:35 2023, max compression
+gzip compressed data, was "lmql-0.0.6.2.tar", last modified: Thu May 11 15:00:40 2023, max compression
```

## Comparing `lmql-0.0.6.1.tar` & `lmql-0.0.6.2.tar`

### file list

```diff
@@ -1,249 +1,256 @@
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.871245 lmql-0.0.6.1/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.847245 lmql-0.0.6.1/.github/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.847245 lmql-0.0.6.1/.github/workflows/
--rw-rw-r--   0 luca      (1000) luca      (1000)     1594 2023-05-01 11:40:25.000000 lmql-0.0.6.1/.github/workflows/lmql-web.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)     2743 2023-05-01 11:40:25.000000 lmql-0.0.6.1/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.6.1/LICENSE
--rw-rw-r--   0 luca      (1000) luca      (1000)      140 2023-04-17 14:44:31.000000 lmql-0.0.6.1/MANIFEST.in
--rw-rw-r--   0 luca      (1000) luca      (1000)     4969 2023-05-03 14:15:35.871245 lmql-0.0.6.1/PKG-INFO
--rw-rw-r--   0 luca      (1000) luca      (1000)     4538 2023-05-03 11:12:24.000000 lmql-0.0.6.1/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)       75 2023-04-17 14:44:31.000000 lmql-0.0.6.1/TODO.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/
--rw-rw-r--   0 luca      (1000) luca      (1000)      638 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/Makefile
--rw-rw-r--   0 luca      (1000) luca      (1000)      444 2023-03-14 15:27:49.000000 lmql-0.0.6.1/docs/RELEASE.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      799 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/make.bat
--rw-rw-r--   0 luca      (1000) luca      (1000)       81 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/requirements.txt
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/source/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/source/_ext/
--rw-rw-r--   0 luca      (1000) luca      (1000)     5526 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/_ext/lmql_snippets.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.847245 lmql-0.0.6.1/docs/source/_static/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/source/_static/css/
--rw-rw-r--   0 luca      (1000) luca      (1000)     5883 2023-04-20 08:07:08.000000 lmql-0.0.6.1/docs/source/_static/css/lmql-docs.css
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/source/_static/images/
--rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/_static/images/lmql.svg
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/source/_static/js/
--rw-rw-r--   0 luca      (1000) luca      (1000)     2191 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/_static/js/lmql-playground.js
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/source/_templates/
--rw-rw-r--   0 luca      (1000) luca      (1000)      292 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/_templates/layout.html
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/source/blog/
--rw-rw-r--   0 luca      (1000) luca      (1000)     4591 2023-05-01 11:40:25.000000 lmql-0.0.6.1/docs/source/blog/release-0.0.5.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     8976 2023-05-01 11:40:25.000000 lmql-0.0.6.1/docs/source/blog/release-0.0.6.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     1167 2023-04-17 14:48:56.000000 lmql-0.0.6.1/docs/source/conf.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1293 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/dev-setup.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     2780 2023-05-02 15:32:22.000000 lmql-0.0.6.1/docs/source/index.rst
--rw-rw-r--   0 luca      (1000) luca      (1000)     2484 2023-04-18 06:55:18.000000 lmql-0.0.6.1/docs/source/installation.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/source/language/
--rw-rw-r--   0 luca      (1000) luca      (1000)     7435 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/language/constraints.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     4067 2023-04-17 14:48:56.000000 lmql-0.0.6.1/docs/source/language/decoders.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     7850 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/language/functions.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     8252 2023-05-02 15:32:22.000000 lmql-0.0.6.1/docs/source/language/models.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     8507 2023-04-18 06:55:18.000000 lmql-0.0.6.1/docs/source/language/overview.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     3676 2023-04-18 06:55:18.000000 lmql-0.0.6.1/docs/source/language/scripted_prompts.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/lmql.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)    28444 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/logo.png
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/source/python/
--rw-rw-r--   0 luca      (1000) luca      (1000)       11 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/python/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    10831 2023-04-18 06:55:18.000000 lmql-0.0.6.1/docs/source/python/langchain.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     6681 2023-04-30 16:34:02.000000 lmql-0.0.6.1/docs/source/python/llama_index.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)    75148 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/python/lmql.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)     7458 2023-05-02 15:32:22.000000 lmql-0.0.6.1/docs/source/python/output.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     9592 2023-04-20 08:07:08.000000 lmql-0.0.6.1/docs/source/python/pandas.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     8847 2023-04-19 15:28:18.000000 lmql-0.0.6.1/docs/source/python/python.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     3135 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/quickstart.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/source/releases/
--rw-rw-r--   0 luca      (1000) luca      (1000)     2263 2023-05-02 15:32:22.000000 lmql-0.0.6.1/docs/source/releases/misc-snippets.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      321 2023-04-17 14:48:56.000000 lmql-0.0.6.1/docs/source/releases/release-0.0.5.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      257 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/todo.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      137 2023-03-14 15:27:49.000000 lmql-0.0.6.1/pyproject.toml
--rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-04-17 14:44:31.000000 lmql-0.0.6.1/requirements.txt
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/scripts/
--rw-rw-r--   0 luca      (1000) luca      (1000)      295 2023-04-17 14:44:31.000000 lmql-0.0.6.1/scripts/activate-dev.sh
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/scripts/conda/
--rw-rw-r--   0 luca      (1000) luca      (1000)      210 2023-04-19 15:28:18.000000 lmql-0.0.6.1/scripts/conda/requirements-no-gpu.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)      344 2023-04-19 15:28:18.000000 lmql-0.0.6.1/scripts/conda/requirements.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)      486 2023-03-14 15:27:49.000000 lmql-0.0.6.1/scripts/pypi-release.sh
--rw-rw-r--   0 luca      (1000) luca      (1000)      817 2023-03-14 15:27:49.000000 lmql-0.0.6.1/scripts/wheel.sh
--rw-rw-r--   0 luca      (1000) luca      (1000)      828 2023-05-03 14:15:35.871245 lmql-0.0.6.1/setup.cfg
--rw-rw-r--   0 luca      (1000) luca      (1000)       37 2023-03-14 15:27:49.000000 lmql-0.0.6.1/setup.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/src/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/src/lmql/
--rw-rw-r--   0 luca      (1000) luca      (1000)     5586 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/__init__.py
--rwxrwxr-x   0 luca      (1000) luca      (1000)     7998 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/cli.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1577 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/demo.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1531 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/http.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.855245 lmql-0.0.6.1/src/lmql/language/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/language/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    21499 2023-05-03 14:14:45.000000 lmql-0.0.6.1/src/lmql/language/compiler.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    10194 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/language/fragment_parser.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      979 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/language/qstrings.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1804 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/language/validator.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.855245 lmql-0.0.6.1/src/lmql/model/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/model/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    24468 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/model/async_generation_utils.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1299 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/model/local_client.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    18118 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/model/serve.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     8052 2023-05-02 15:48:30.000000 lmql-0.0.6.1/src/lmql/model/served_model.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.855245 lmql-0.0.6.1/src/lmql/ops/
--rw-rw-r--   0 luca      (1000) luca      (1000)       93 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ops/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     7542 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/ops/follow_map.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    39574 2023-05-03 14:14:45.000000 lmql-0.0.6.1/src/lmql/ops/ops.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    21044 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/ops/token_set.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.855245 lmql-0.0.6.1/src/lmql/output/
--rw-rw-r--   0 luca      (1000) luca      (1000)       57 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/output/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2313 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/output/http.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1889 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/output/sse.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2282 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/output/ws.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.855245 lmql-0.0.6.1/src/lmql/runtime/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/runtime/__init__.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.855245 lmql-0.0.6.1/src/lmql/runtime/bopenai/
--rw-rw-r--   0 luca      (1000) luca      (1000)     2236 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/runtime/bopenai/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    28384 2023-05-03 14:14:45.000000 lmql-0.0.6.1/src/lmql/runtime/bopenai/batched_openai.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    17221 2023-05-03 11:12:24.000000 lmql-0.0.6.1/src/lmql/runtime/bopenai/openai_api.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.855245 lmql-0.0.6.1/src/lmql/runtime/dclib/
--rw-rw-r--   0 luca      (1000) luca      (1000)      494 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/runtime/dclib/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    18631 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_array.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    26433 2023-05-03 14:14:45.000000 lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_cache.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      538 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_global.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    21721 2023-05-02 16:00:00.000000 lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_model.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     8589 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_rewrite.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    30560 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_seq.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    20722 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/runtime/dclib/decoders.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4144 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/runtime/dclib/trie_cache.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3176 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/runtime/hf_integration.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    34019 2023-05-03 11:12:24.000000 lmql-0.0.6.1/src/lmql/runtime/interpreter.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      250 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/runtime/interrupt.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1084 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/runtime/langchain.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     6367 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/runtime/lmql_runtime.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1186 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/runtime/maiohttp.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1726 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/runtime/masks.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      732 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/runtime/model_registry.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     5835 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/runtime/multi_head_interpretation.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    42592 2023-05-03 11:12:24.000000 lmql-0.0.6.1/src/lmql/runtime/openai_integration.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1971 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/runtime/openai_secret.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4042 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/runtime/output_writer.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.859245 lmql-0.0.6.1/src/lmql/runtime/postprocessing/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/runtime/postprocessing/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3530 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/runtime/postprocessing/conditional_prob.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      152 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/runtime/postprocessing/group_by.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1980 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/runtime/program_state.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1317 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/runtime/stats.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     9327 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/runtime/tokenizer.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.859245 lmql-0.0.6.1/src/lmql/tests/
--rw-rw-r--   0 luca      (1000) luca      (1000)      319 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/tests/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     5188 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/expr_test_utils.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.859245 lmql-0.0.6.1/src/lmql/tests/outdated/
--rw-rw-r--   0 luca      (1000) luca      (1000)     1611 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/outdated/mask_product_test.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2789 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/outdated/monotonicity.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      546 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/outdated/one_of_tests.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      758 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/outdated/sentences_op.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      984 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/outdated/starts_with_op_test.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1236 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/outdated/stops_at.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      537 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/outdated/str_in_str_tests.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4738 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/outdated/test_multi_head.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3036 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/outdated/token_set_test.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.859245 lmql-0.0.6.1/src/lmql/tests/system/
--rw-rw-r--   0 luca      (1000) luca      (1000)     3402 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/tests/system/basic_use_cases.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      971 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/tail_token_set.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      788 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/tests/test_back2back_caching.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2481 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/test_sample_queries.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.859245 lmql-0.0.6.1/src/lmql/ui/
--rw-rw-r--   0 luca      (1000) luca      (1000)       27 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/__init__.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.859245 lmql-0.0.6.1/src/lmql/ui/live/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/live/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     6747 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/live/live.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     3346 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/ui/live/live.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3885 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/live/livelib.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      349 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/live/package.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    33701 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/live/yarn.lock
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.859245 lmql-0.0.6.1/src/lmql/ui/playground/
--rw-rw-r--   0 luca      (1000) luca      (1000)       31 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/.dockerignore
--rw-rw-r--   0 luca      (1000) luca      (1000)       34 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/.env
--rw-rw-r--   0 luca      (1000) luca      (1000)      310 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)      354 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/Dockerfile
--rw-rw-r--   0 luca      (1000) luca      (1000)     3359 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     1327 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/package.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.859245 lmql-0.0.6.1/src/lmql/ui/playground/public/
--rw-rw-r--   0 luca      (1000) luca      (1000)       90 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/_headers
--rw-rw-r--   0 luca      (1000) luca      (1000)     3870 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/favicon.ico
--rw-rw-r--   0 luca      (1000) luca      (1000)     1678 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/index.html
--rw-rw-r--   0 luca      (1000) luca      (1000)     2817 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/lmql.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)      306 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/manifest.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.867245 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/
--rw-rw-r--   0 luca      (1000) luca      (1000)  1227728 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/calc.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   295285 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/chat.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   160153 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/cot.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    81768 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/distribution.json
--rw-rw-r--   0 luca      (1000) luca      (1000)     5221 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/hello.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    89531 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/joke.json
--rw-rw-r--   0 luca      (1000) luca      (1000)  1710847 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/kv.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    52748 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/list.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   628184 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/meta.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   264768 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/translation.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   215050 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/wiki.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       67 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/robots.txt
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.867245 lmql-0.0.6.1/src/lmql/ui/playground/public/snippets/
--rw-rw-r--   0 luca      (1000) luca      (1000)   381736 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   184008 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/snippets/json-parsing.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       62 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/ref.py
--rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/run-in-docker.sh
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.867245 lmql-0.0.6.1/src/lmql/ui/playground/src/
--rw-rw-r--   0 luca      (1000) luca      (1000)    69135 2023-05-03 14:14:45.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/App.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      246 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/App.test.js
--rw-rw-r--   0 luca      (1000) luca      (1000)    29983 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/CodeScreenshot.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      807 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/Configuration.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     1174 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/DataListView.js
--rw-rw-r--   0 luca      (1000) luca      (1000)    21319 2023-05-03 11:12:24.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/DecoderGraph.js
--rw-rw-r--   0 luca      (1000) luca      (1000)      329 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/DecodingTree.js
--rw-rw-r--   0 luca      (1000) luca      (1000)       89 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/Embed.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)     9601 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/Explore.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      675 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/SharedState.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     3868 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/State.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     5763 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/ValidationGraph.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)     9360 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/browser_process.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     1163 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/build_info.js
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.867245 lmql-0.0.6.1/src/lmql/ui/playground/src/editor/
--rw-rw-r--   0 luca      (1000) luca      (1000)     8696 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     4758 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/editor/theme.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      889 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/explore.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     1345 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/graph-layout.css
--rw-rw-r--   0 luca      (1000) luca      (1000)     1698 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/index.css
--rw-rw-r--   0 luca      (1000) luca      (1000)      489 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/index.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     2632 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/logo.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     8104 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/queries.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     5990 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/remote_process.js
--rw-rw-r--   0 luca      (1000) luca      (1000)      362 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/reportWebVitals.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     9520 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/screenshot.css
--rw-rw-r--   0 luca      (1000) luca      (1000)      241 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/setupTests.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     3466 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/spinner.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     2949 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/tagged-model-result.js
--rw-rw-r--   0 luca      (1000) luca      (1000)   449905 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/yarn.lock
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.871245 lmql-0.0.6.1/src/lmql/ui/vscode/
--rw-rw-r--   0 luca      (1000) luca      (1000)       76 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/vscode/.gitattributes
--rw-rw-r--   0 luca      (1000) luca      (1000)       19 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/vscode/.gitignore
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.871245 lmql-0.0.6.1/src/lmql/ui/vscode/.vscode/
--rw-rw-r--   0 luca      (1000) luca      (1000)      540 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/vscode/.vscode/launch.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       66 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/vscode/.vscodeignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/ui/vscode/LICENSE
--rw-rw-r--   0 luca      (1000) luca      (1000)      357 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/ui/vscode/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      959 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/vscode/language-configuration.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    11532 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/ui/vscode/lmql-vscode.png
--rw-rw-r--   0 luca      (1000) luca      (1000)     1214 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/ui/vscode/package.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.871245 lmql-0.0.6.1/src/lmql/ui/vscode/syntaxes/
--rw-rw-r--   0 luca      (1000) luca      (1000)      518 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      642 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      853 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/vscode/syntaxes/pylmql.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.871245 lmql-0.0.6.1/src/lmql/utils/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/utils/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2402 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/utils/docstring_parser.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     5384 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/utils/graph.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2402 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/utils/nputil.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      115 2023-05-03 14:15:30.000000 lmql-0.0.6.1/src/lmql/version.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.855245 lmql-0.0.6.1/src/lmql.egg-info/
--rw-rw-r--   0 luca      (1000) luca      (1000)     4969 2023-05-03 14:15:35.000000 lmql-0.0.6.1/src/lmql.egg-info/PKG-INFO
--rw-rw-r--   0 luca      (1000) luca      (1000)     6969 2023-05-03 14:15:35.000000 lmql-0.0.6.1/src/lmql.egg-info/SOURCES.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)        1 2023-05-03 14:15:35.000000 lmql-0.0.6.1/src/lmql.egg-info/dependency_links.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)       39 2023-05-03 14:15:35.000000 lmql-0.0.6.1/src/lmql.egg-info/entry_points.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-05-03 14:15:35.000000 lmql-0.0.6.1/src/lmql.egg-info/requires.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)        5 2023-05-03 14:15:35.000000 lmql-0.0.6.1/src/lmql.egg-info/top_level.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)   115785 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql.svg
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.332651 lmql-0.0.6.2/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.308651 lmql-0.0.6.2/.github/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/.github/workflows/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2285 2023-05-09 13:19:22.000000 lmql-0.0.6.2/.github/workflows/lmql-web.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2743 2023-05-01 11:40:25.000000 lmql-0.0.6.2/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.6.2/LICENSE
+-rw-rw-r--   0 luca      (1000) luca      (1000)      140 2023-04-17 14:44:31.000000 lmql-0.0.6.2/MANIFEST.in
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4988 2023-05-11 15:00:40.332651 lmql-0.0.6.2/PKG-INFO
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4538 2023-05-03 11:12:24.000000 lmql-0.0.6.2/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)       75 2023-04-17 14:44:31.000000 lmql-0.0.6.2/TODO.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      638 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/Makefile
+-rw-rw-r--   0 luca      (1000) luca      (1000)      444 2023-03-14 15:27:49.000000 lmql-0.0.6.2/docs/RELEASE.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      799 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/make.bat
+-rw-rw-r--   0 luca      (1000) luca      (1000)       81 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/requirements.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/source/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/source/_ext/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5526 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/_ext/lmql_snippets.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.308651 lmql-0.0.6.2/docs/source/_static/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/source/_static/css/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5883 2023-04-20 08:07:08.000000 lmql-0.0.6.2/docs/source/_static/css/lmql-docs.css
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/source/_static/images/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/_static/images/lmql.svg
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/source/_static/js/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2191 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/_static/js/lmql-playground.js
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/source/_templates/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      292 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/_templates/layout.html
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/source/blog/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4591 2023-05-01 11:40:25.000000 lmql-0.0.6.2/docs/source/blog/release-0.0.5.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1444 2023-05-04 19:03:37.000000 lmql-0.0.6.2/docs/source/blog/release-0.0.6.1.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8976 2023-05-01 11:40:25.000000 lmql-0.0.6.2/docs/source/blog/release-0.0.6.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1167 2023-04-17 14:48:56.000000 lmql-0.0.6.2/docs/source/conf.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1293 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/dev-setup.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2780 2023-05-02 15:32:22.000000 lmql-0.0.6.2/docs/source/index.rst
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2484 2023-04-18 06:55:18.000000 lmql-0.0.6.2/docs/source/installation.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/source/language/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7435 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/language/constraints.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4067 2023-04-17 14:48:56.000000 lmql-0.0.6.2/docs/source/language/decoders.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7850 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/language/functions.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8252 2023-05-02 15:32:22.000000 lmql-0.0.6.2/docs/source/language/models.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8507 2023-04-18 06:55:18.000000 lmql-0.0.6.2/docs/source/language/overview.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3676 2023-04-18 06:55:18.000000 lmql-0.0.6.2/docs/source/language/scripted_prompts.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/lmql.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)    28444 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/logo.png
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/source/python/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       11 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/python/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    10831 2023-04-18 06:55:18.000000 lmql-0.0.6.2/docs/source/python/langchain.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6681 2023-04-30 16:34:02.000000 lmql-0.0.6.2/docs/source/python/llama_index.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)    75148 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/python/lmql.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7458 2023-05-02 15:32:22.000000 lmql-0.0.6.2/docs/source/python/output.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9592 2023-04-20 08:07:08.000000 lmql-0.0.6.2/docs/source/python/pandas.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8847 2023-04-19 15:28:18.000000 lmql-0.0.6.2/docs/source/python/python.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3135 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/quickstart.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/source/releases/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2263 2023-05-02 15:32:22.000000 lmql-0.0.6.2/docs/source/releases/misc-snippets.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      321 2023-04-17 14:48:56.000000 lmql-0.0.6.2/docs/source/releases/release-0.0.5.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      257 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/todo.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      137 2023-03-14 15:27:49.000000 lmql-0.0.6.2/pyproject.toml
+-rw-rw-r--   0 luca      (1000) luca      (1000)       74 2023-05-10 09:23:13.000000 lmql-0.0.6.2/requirements.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/scripts/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      295 2023-04-17 14:44:31.000000 lmql-0.0.6.2/scripts/activate-dev.sh
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.316651 lmql-0.0.6.2/scripts/conda/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      198 2023-05-10 09:22:47.000000 lmql-0.0.6.2/scripts/conda/requirements-no-gpu.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)      332 2023-05-10 09:22:44.000000 lmql-0.0.6.2/scripts/conda/requirements.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)      486 2023-03-14 15:27:49.000000 lmql-0.0.6.2/scripts/pypi-release.sh
+-rw-rw-r--   0 luca      (1000) luca      (1000)      817 2023-03-14 15:27:49.000000 lmql-0.0.6.2/scripts/wheel.sh
+-rw-rw-r--   0 luca      (1000) luca      (1000)      866 2023-05-11 15:00:40.332651 lmql-0.0.6.2/setup.cfg
+-rw-rw-r--   0 luca      (1000) luca      (1000)       37 2023-05-10 14:35:25.000000 lmql-0.0.6.2/setup.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.316651 lmql-0.0.6.2/src/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.316651 lmql-0.0.6.2/src/lmql/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6208 2023-05-09 13:19:22.000000 lmql-0.0.6.2/src/lmql/__init__.py
+-rwxrwxr-x   0 luca      (1000) luca      (1000)     8142 2023-05-04 19:03:37.000000 lmql-0.0.6.2/src/lmql/cli.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1577 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/demo.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1531 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/http.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.316651 lmql-0.0.6.2/src/lmql/language/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/language/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    24147 2023-05-09 13:19:22.000000 lmql-0.0.6.2/src/lmql/language/compiler.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    10194 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/language/fragment_parser.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      979 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/language/qstrings.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1804 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/language/validator.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.316651 lmql-0.0.6.2/src/lmql/model/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/model/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    24468 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/model/async_generation_utils.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1299 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/model/local_client.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    18118 2023-05-10 08:09:52.000000 lmql-0.0.6.2/src/lmql/model/serve.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8052 2023-05-02 15:48:30.000000 lmql-0.0.6.2/src/lmql/model/served_model.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.316651 lmql-0.0.6.2/src/lmql/ops/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       93 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ops/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7542 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/ops/follow_map.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    41664 2023-05-09 13:19:22.000000 lmql-0.0.6.2/src/lmql/ops/ops.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    20831 2023-05-10 08:09:02.000000 lmql-0.0.6.2/src/lmql/ops/token_set.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.316651 lmql-0.0.6.2/src/lmql/output/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       57 2023-05-02 15:32:22.000000 lmql-0.0.6.2/src/lmql/output/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2334 2023-05-10 08:08:53.000000 lmql-0.0.6.2/src/lmql/output/http.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1889 2023-05-02 15:32:22.000000 lmql-0.0.6.2/src/lmql/output/sse.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2282 2023-05-02 15:32:22.000000 lmql-0.0.6.2/src/lmql/output/ws.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.316651 lmql-0.0.6.2/src/lmql/runtime/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/runtime/__init__.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.320651 lmql-0.0.6.2/src/lmql/runtime/bopenai/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2236 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/runtime/bopenai/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    28384 2023-05-03 14:14:45.000000 lmql-0.0.6.2/src/lmql/runtime/bopenai/batched_openai.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    17221 2023-05-03 11:12:24.000000 lmql-0.0.6.2/src/lmql/runtime/bopenai/openai_api.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1906 2023-05-10 08:09:02.000000 lmql-0.0.6.2/src/lmql/runtime/caching.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.320651 lmql-0.0.6.2/src/lmql/runtime/dclib/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      494 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/runtime/dclib/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    18631 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_array.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    27728 2023-05-10 08:08:53.000000 lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_cache.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      538 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_global.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    21721 2023-05-02 16:00:00.000000 lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_model.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8589 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_rewrite.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    30560 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_seq.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    20827 2023-05-04 19:03:37.000000 lmql-0.0.6.2/src/lmql/runtime/dclib/decoders.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4144 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/runtime/dclib/trie_cache.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3176 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/runtime/hf_integration.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    34822 2023-05-04 19:03:37.000000 lmql-0.0.6.2/src/lmql/runtime/interpreter.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      250 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/runtime/interrupt.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1084 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/runtime/langchain.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6367 2023-05-02 15:32:22.000000 lmql-0.0.6.2/src/lmql/runtime/lmql_runtime.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1186 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/runtime/maiohttp.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1726 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/runtime/masks.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      732 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/runtime/model_registry.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5835 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/runtime/multi_head_interpretation.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    42592 2023-05-03 11:12:24.000000 lmql-0.0.6.2/src/lmql/runtime/openai_integration.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1971 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/runtime/openai_secret.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4042 2023-05-02 15:32:22.000000 lmql-0.0.6.2/src/lmql/runtime/output_writer.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.320651 lmql-0.0.6.2/src/lmql/runtime/postprocessing/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/runtime/postprocessing/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3530 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/runtime/postprocessing/conditional_prob.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      152 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/runtime/postprocessing/group_by.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1980 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/runtime/program_state.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1317 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/runtime/stats.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9778 2023-05-10 08:24:41.000000 lmql-0.0.6.2/src/lmql/runtime/tokenizer.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.320651 lmql-0.0.6.2/src/lmql/tests/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      319 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/tests/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5667 2023-05-04 19:03:37.000000 lmql-0.0.6.2/src/lmql/tests/expr_test_utils.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1314 2023-05-04 19:03:37.000000 lmql-0.0.6.2/src/lmql/tests/fin_and.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.320651 lmql-0.0.6.2/src/lmql/tests/outdated/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1611 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/outdated/mask_product_test.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2789 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/outdated/monotonicity.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      546 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/outdated/one_of_tests.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      758 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/outdated/sentences_op.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      984 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/outdated/starts_with_op_test.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1236 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/outdated/stops_at.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      537 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/outdated/str_in_str_tests.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4738 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/outdated/test_multi_head.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3036 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/outdated/token_set_test.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.320651 lmql-0.0.6.2/src/lmql/tests/system/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3402 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/tests/system/basic_use_cases.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      971 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/tail_token_set.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      788 2023-05-02 15:32:22.000000 lmql-0.0.6.2/src/lmql/tests/test_back2back_caching.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2382 2023-05-09 13:19:22.000000 lmql-0.0.6.2/src/lmql/tests/test_eq.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      457 2023-05-04 19:03:37.000000 lmql-0.0.6.2/src/lmql/tests/test_orop.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2481 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/test_sample_queries.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1720 2023-05-09 13:19:22.000000 lmql-0.0.6.2/src/lmql/tests/test_scoping.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3572 2023-05-09 13:19:22.000000 lmql-0.0.6.2/src/lmql/tests/test_stopping.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.320651 lmql-0.0.6.2/src/lmql/ui/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       27 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/__init__.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.320651 lmql-0.0.6.2/src/lmql/ui/live/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/live/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6747 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/live/live.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3334 2023-05-04 19:03:37.000000 lmql-0.0.6.2/src/lmql/ui/live/live.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3885 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/live/livelib.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      349 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/live/package.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    33701 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/live/yarn.lock
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.324651 lmql-0.0.6.2/src/lmql/ui/playground/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       31 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/.dockerignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)       34 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/.env
+-rw-rw-r--   0 luca      (1000) luca      (1000)      310 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)      354 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/Dockerfile
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3359 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1327 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/package.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.324651 lmql-0.0.6.2/src/lmql/ui/playground/public/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       90 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/_headers
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3870 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/favicon.ico
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1678 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/index.html
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2817 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/lmql.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)      306 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/manifest.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.328651 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/
+-rw-rw-r--   0 luca      (1000) luca      (1000)  1227728 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/calc.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   295285 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/chat.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   160153 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/cot.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    81768 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/distribution.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5221 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/hello.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    89531 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/joke.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)  1710847 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/kv.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    52748 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/list.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   628184 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/meta.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   264768 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/translation.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   215050 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/wiki.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       67 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/robots.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.328651 lmql-0.0.6.2/src/lmql/ui/playground/public/snippets/
+-rw-rw-r--   0 luca      (1000) luca      (1000)   381736 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   184008 2023-05-02 15:32:22.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/snippets/json-parsing.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       62 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/ref.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/run-in-docker.sh
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.332651 lmql-0.0.6.2/src/lmql/ui/playground/src/
+-rw-rw-r--   0 luca      (1000) luca      (1000)    69135 2023-05-03 14:14:45.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/App.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      246 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/App.test.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)    29983 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/CodeScreenshot.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      807 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/Configuration.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1174 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/DataListView.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)    21319 2023-05-03 11:12:24.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/DecoderGraph.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)      329 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/DecodingTree.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)       89 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/Embed.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9601 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/Explore.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      675 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/SharedState.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4819 2023-05-04 19:03:37.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/State.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5871 2023-05-04 19:03:37.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/ValidationGraph.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9360 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/browser_process.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1163 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/build_info.js
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.332651 lmql-0.0.6.2/src/lmql/ui/playground/src/editor/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8696 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4758 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/editor/theme.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      889 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/explore.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1345 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/graph-layout.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1698 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/index.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)      489 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/index.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2632 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/logo.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8104 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/queries.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5990 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/remote_process.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)      362 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/reportWebVitals.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9520 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/screenshot.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)      241 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/setupTests.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3466 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/spinner.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2949 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/tagged-model-result.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)   449905 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/yarn.lock
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.332651 lmql-0.0.6.2/src/lmql/ui/vscode/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       76 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/vscode/.gitattributes
+-rw-rw-r--   0 luca      (1000) luca      (1000)       19 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/vscode/.gitignore
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.332651 lmql-0.0.6.2/src/lmql/ui/vscode/.vscode/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      540 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/vscode/.vscode/launch.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       66 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/vscode/.vscodeignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/ui/vscode/LICENSE
+-rw-rw-r--   0 luca      (1000) luca      (1000)      357 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/ui/vscode/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      959 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/vscode/language-configuration.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    11532 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/ui/vscode/lmql-vscode.png
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1214 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/ui/vscode/package.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.332651 lmql-0.0.6.2/src/lmql/ui/vscode/syntaxes/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      518 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      642 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      853 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/vscode/syntaxes/pylmql.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.332651 lmql-0.0.6.2/src/lmql/utils/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/utils/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2402 2023-05-02 15:32:22.000000 lmql-0.0.6.2/src/lmql/utils/docstring_parser.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4933 2023-05-10 09:22:32.000000 lmql-0.0.6.2/src/lmql/utils/graph.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2402 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/utils/nputil.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      115 2023-05-11 15:00:35.000000 lmql-0.0.6.2/src/lmql/version.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.316651 lmql-0.0.6.2/src/lmql.egg-info/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4988 2023-05-11 15:00:40.000000 lmql-0.0.6.2/src/lmql.egg-info/PKG-INFO
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7176 2023-05-11 15:00:40.000000 lmql-0.0.6.2/src/lmql.egg-info/SOURCES.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)        1 2023-05-11 15:00:40.000000 lmql-0.0.6.2/src/lmql.egg-info/dependency_links.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)       39 2023-05-11 15:00:40.000000 lmql-0.0.6.2/src/lmql.egg-info/entry_points.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)       94 2023-05-11 15:00:40.000000 lmql-0.0.6.2/src/lmql.egg-info/requires.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)        5 2023-05-11 15:00:40.000000 lmql-0.0.6.2/src/lmql.egg-info/top_level.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)   115785 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql.svg
```

### Comparing `lmql-0.0.6.1/.github/workflows/lmql-web.yml` & `lmql-0.0.6.2/.github/workflows/lmql-web.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-# This workflow will do a clean installation of node dependencies, cache/restore them, build the source code and run tests across different versions of node
-# For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-nodejs
-
 name: Browser Build & Web Deploy
 
 on:
   push:
-    branches: [ "main", "updated-web"]
+    branches: [ "main", "next"]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
 
     steps:
@@ -34,14 +31,55 @@
         node-version: 19.x
     - uses: actions/download-artifact@v3
       name: Restore docs/build/html
       with:
         name: DocumentationHTML
         path: docs/build/html/
     - name: Build web/ and In-Browser LMQL Distribution
-      run: cd web && bash deploy.sh
-    
+      run: cd web && bash deploy.sh    
+    - uses: actions/upload-artifact@master
+      with:
+        name: lmql-web-payload
+        path: web-deploy
+
+  deploy-main:
+    name: Deploy Main Playground 
+    runs-on: ubuntu-latest
+    needs: [build]
+    if:
+      contains('
+        refs/heads/main
+      ', github.ref)
+    steps:
+    - uses: actions/checkout@master
+    - uses: actions/download-artifact@master
+      with:
+        name: lmql-web-payload
+        path: web-deploy
     - name: Deploy to web branch
       uses: JamesIves/github-pages-deploy-action@v4
       with:
         folder: web-deploy
         branch: web
+
+  deploy-next:
+    name: Deploy Next Playground
+    runs-on: ubuntu-latest
+    needs: [build]
+    if:
+      contains('
+        refs/heads/next
+      ', github.ref)
+    steps:
+    - uses: actions/checkout@master
+    - uses: actions/download-artifact@master
+      with:
+        name: lmql-web-payload
+        path: web-deploy
+    - run: cp web-deploy/index-next.html web-deploy/index.html
+    - name: Deploy to web branch
+      uses: JamesIves/github-pages-deploy-action@v4
+      with:
+        folder: web-deploy
+        branch: web-next
+
+
```

### Comparing `lmql-0.0.6.1/.gitignore` & `lmql-0.0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/LICENSE` & `lmql-0.0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/PKG-INFO` & `lmql-0.0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.0.6.1
+Version: 0.0.6.2
 Summary: A query language for language models.
 Home-page: https://lmql.ai
 Author: Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 Author-email: hello@lmql.ai
 Project-URL: Docs, https://docs.lmql.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: hf
 License-File: LICENSE
 
 <div align="center">
   <a href="https://lmql.ai">
     <img src="https://raw.githubusercontent.com/eth-sri/lmql/web/lmql.svg" alt="Logo" width="80" height="80">
   </a>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: lmql Version: 0.0.6.1 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.0.6.2 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
-Type: text/markdown License-File: LICENSE
+Type: text/markdown Provides-Extra: hf License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
           A query language for programming (large) language models.
                                Documentation_Â»
 
                Explore_Examples Â· Playground_IDE Â· Report_Bug
```

### Comparing `lmql-0.0.6.1/README.md` & `lmql-0.0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/Makefile` & `lmql-0.0.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/make.bat` & `lmql-0.0.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/_ext/lmql_snippets.py` & `lmql-0.0.6.2/docs/source/_ext/lmql_snippets.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/_static/css/lmql-docs.css` & `lmql-0.0.6.2/docs/source/_static/css/lmql-docs.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/_static/images/lmql.svg` & `lmql-0.0.6.2/docs/source/_static/images/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/_static/js/lmql-playground.js` & `lmql-0.0.6.2/docs/source/_static/js/lmql-playground.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/blog/release-0.0.5.md` & `lmql-0.0.6.2/docs/source/blog/release-0.0.5.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/blog/release-0.0.6.md` & `lmql-0.0.6.2/docs/source/blog/release-0.0.6.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/conf.py` & `lmql-0.0.6.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/dev-setup.md` & `lmql-0.0.6.2/docs/source/dev-setup.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/index.rst` & `lmql-0.0.6.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/installation.md` & `lmql-0.0.6.2/docs/source/installation.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/language/constraints.md` & `lmql-0.0.6.2/docs/source/language/constraints.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/language/decoders.md` & `lmql-0.0.6.2/docs/source/language/decoders.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/language/functions.md` & `lmql-0.0.6.2/docs/source/language/functions.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/language/models.md` & `lmql-0.0.6.2/docs/source/language/models.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/language/overview.md` & `lmql-0.0.6.2/docs/source/language/overview.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/language/scripted_prompts.md` & `lmql-0.0.6.2/docs/source/language/scripted_prompts.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/lmql.svg` & `lmql-0.0.6.2/docs/source/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/logo.png` & `lmql-0.0.6.2/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/python/langchain.ipynb` & `lmql-0.0.6.2/docs/source/python/langchain.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/python/llama_index.ipynb` & `lmql-0.0.6.2/docs/source/python/llama_index.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/python/lmql.txt` & `lmql-0.0.6.2/docs/source/python/lmql.txt`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/python/output.ipynb` & `lmql-0.0.6.2/docs/source/python/output.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/python/pandas.ipynb` & `lmql-0.0.6.2/docs/source/python/pandas.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/python/python.ipynb` & `lmql-0.0.6.2/docs/source/python/python.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/quickstart.md` & `lmql-0.0.6.2/docs/source/quickstart.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/docs/source/releases/misc-snippets.md` & `lmql-0.0.6.2/docs/source/releases/misc-snippets.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/scripts/wheel.sh` & `lmql-0.0.6.2/scripts/wheel.sh`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/setup.cfg` & `lmql-0.0.6.2/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lmql
-version = 0.0.6.1
+version = 0.0.6.2
 author = Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 author_email = hello@lmql.ai
 description = A query language for language models.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://lmql.ai
 project_urls = 
@@ -19,18 +19,19 @@
 	= src
 include_package_data = True
 python_requires = >=3.10
 install_requires = 
 	astunparse ==1.6.3
 	openai
 	termcolor
-	pydot
-	transformers ==4.25.1
-	pandas
-	accelerate
+	numpy
+	gpt3_tokenizer
+
+[options.extras_require]
+hf = transformers >=4.28.1; accelerate
 
 [options.packages.find]
 where = src
 exclude = 
 	**/node_modules/*
 	**/web/**/*
 	**/vscode/**/*
```

### Comparing `lmql-0.0.6.1/src/lmql/__init__.py` & `lmql-0.0.6.2/src/lmql/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,42 +72,54 @@
     if output_writer is not None:
         output_writer.add_compiler_output(module.code())
 
     module = module.load()
     module.query.force_model(force_model)
     return module
 
-async def run_file(filepath, output_writer=None, force_model=None, *args):
+async def run_file(filepath, *args, output_writer=None, force_model=None, **kwargs):
+    import inspect
     module = load(filepath, autoconnect=True, output_writer=output_writer, force_model=force_model)
     
     if module is None: 
         print("Failed to compile query.")
         return
 
     if output_writer is not None:
         module.query.output_writer = output_writer
-    
-    if len(args) == 1 and args[0] == "":
-        kwargs = {}
+
+    compiled_fct_args = module.query.args
+    query_args = []
+
+    calling_frame = inspect.stack()[1]
+    scope = LMQLInputVariableScope(module.query.fct, calling_frame)
+    for arg in compiled_fct_args:
+        if scope.resolve(arg) == None:
+            query_args.append(arg)
+
+    output_variables = module.query.output_variables
+    query_args = list(set(query_args) - set(output_variables))
+
+    if len(args) > 0:
+        assert False, "Positional arguments for queries are not supported yet"
     else:
-        kwargs = {}
-        for line in args:
-            line = line.strip()
-            key, value = line.split(":", 1)
-            kwargs[key.strip()] = value.strip()
+        assert len(kwargs) == len(query_args), f"Expected {len(query_args)} keyword arguments for query, got {len(kwargs)}: Expected: {query_args}, got: {kwargs}"
 
+        for query_kw in kwargs.keys():
+            assert query_kw in query_args, f"Unknown query argument '{query_kw}'"
+            
     return await module.query(**kwargs)
 
-async def run(code, output_writer=None):
+async def run(code, *args, output_writer=None, **kwargs):
     temp_lmql_file = tempfile.mktemp(suffix=".lmql")
     with open(temp_lmql_file, "w") as f:
         f.write(code)
     
     os.chdir(os.path.join(os.path.dirname(__file__), "../../")) 
-    return await run_file(temp_lmql_file, output_writer=output_writer)
+    return await run_file(temp_lmql_file, *args, output_writer=output_writer, **kwargs)
         
 def _query_from_string(s):
     temp_lmql_file = tempfile.mktemp(suffix=".lmql")
     with open(temp_lmql_file, "w") as f:
         f.write(s)
     module = load(temp_lmql_file, autoconnect=True, output_writer=silent)
     return module.query
```

### Comparing `lmql-0.0.6.1/src/lmql/cli.py` & `lmql-0.0.6.2/src/lmql/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -180,16 +180,22 @@
     if backend is None or backend == "openai":
         print("[Greeting OpenAI]")
         code_openai = """
     argmax "Hello[WHO]" from "openai/text-ada-001" where len(WHO) < 10    
     """
         asyncio.run(lmql.run(code_openai, output_writer=lmql.printing))
 
+def basic_samples():
+    from lmql.tests.test_sample_queries import main
+    import asyncio
+    asyncio.run(main())
+
 hidden_commands = {
-    "hello": hello
+    "hello": hello,
+    "test": basic_samples
 }
 
 def main():
     if len(sys.argv) < 2:
         cmd_usage()
         sys.exit(1)
     # get all functions defined in this file
```

### Comparing `lmql-0.0.6.1/src/lmql/demo.py` & `lmql-0.0.6.2/src/lmql/demo.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/http.py` & `lmql-0.0.6.2/src/lmql/http.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/language/compiler.py` & `lmql-0.0.6.2/src/lmql/language/compiler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from _ast import AsyncFunctionDef, ClassDef, FunctionDef, Import, ImportFrom
 import ast
 import sys
+from typing import Any
 import astunparse
 import os
 import importlib
 import re
 
 from io import StringIO
 from lmql.ops.ops import lmql_operation_registry
@@ -14,44 +16,100 @@
 from lmql.runtime.model_registry import model_name_aliases
 import lmql.runtime.lmql_runtime as lmql_runtime
 from lmql.runtime.dclib import get_all_decoders
 
 OPS_NAMESPACE = "lmql.ops"
 
 class FreeVarCollector(ast.NodeVisitor):
-    def __init__(self, free_vars, exclude=None):
+    def __init__(self, free_vars, exclude_criteria=None):
         self.free_vars = free_vars
-        self.exclude = exclude or set()
+        
+        self.exclude = exclude_criteria or []
+
+    def is_excluded(self, name):
+        for criterion in self.exclude:
+            if type(criterion) is list:
+                return name in criterion
+            elif callable(criterion):
+                return criterion(name)
+            else:
+                assert False, f"compiler error: invalid type for exclusion criterion in identifier collection: {type(criterion)}"
+        return False
 
     def visit_Name(self, node):
         if type(node.ctx) is ast.Load:
-            if node.id in self.exclude:
+            if self.is_excluded(node.id):
                 return
             self.free_vars.add(node.id)
 
+class DefinedVarsCollector(ast.NodeVisitor):
+    def __init__(self, defined_vars):
+        self.defined_vars = defined_vars
+
+    def visit_Name(self, node):
+        if type(node.ctx) is ast.Store:
+            self.defined_vars.add(node.id)
+
+    def visit_FunctionDef(self, node: FunctionDef) -> Any:
+        self.defined_vars.add(node.name)
+    
+    def visit_ClassDef(self, node: ClassDef) -> Any:
+        self.defined_vars.add(node.name)
+
+    def visit_Import(self, node: Import) -> Any:
+        for alias in node.names:
+            self.defined_vars.add(alias.asname or alias.name)
+
+    def visit_ImportFrom(self, node: ImportFrom) -> Any:
+        for alias in node.names:
+            self.defined_vars.add(alias.asname or alias.name)
+
+    def visit_AsyncFunctionDef(self, node: AsyncFunctionDef) -> Any:
+        self.defined_vars.add(node.name)
+
 class PromptScope(ast.NodeVisitor):
+    def __init__(self):
+        self.distribution_vars = set()
+        self.defined_vars = set()
+        self.prologue_vars = set()
+        self.free_vars = set()
+        self.written_vars = set()
+
+    def scope_prologue(self, query: LMQLQuery):
+        if query.prologue is None: return
+        
+        DefinedVarsCollector(self.prologue_vars).visit(ast.parse(query.prologue))
+
     def scope(self, query: LMQLQuery):
         self.distribution_vars = set([query.distribution.variable_name]) if query.distribution is not None else set()    
         self.defined_vars = set()
+        self.prologue_vars = set()
 
         # collect set of global query template variables
         self.free_vars = set()
         self.written_vars = set()
 
+        # collect defined vars in prologue
+        self.scope_prologue(query)
+
+        # collect defined vars in prompt
         for p in query.prompt: self.visit(p)
-        
+
         # also collect variable reads from where clause
         if query.where is not None:
-            FreeVarCollector(self.free_vars).visit(query.where)
+            FreeVarCollector(self.free_vars, exclude_criteria=[self.exclude_identifier]).visit(query.where)
         if query.from_ast is not None:
-            FreeVarCollector(self.free_vars).visit(query.from_ast)
+            FreeVarCollector(self.free_vars, exclude_criteria=[self.exclude_identifier]).visit(query.from_ast)
         if query.decode is not None:
-            FreeVarCollector(self.free_vars, exclude=get_all_decoders()).visit(query.decode)
+            FreeVarCollector(self.free_vars, exclude_criteria=[self.exclude_identifier]).visit(query.decode)
         if query.distribution is not None:
-            FreeVarCollector(self.free_vars).visit(query.distribution.values)
+            FreeVarCollector(self.free_vars, exclude_criteria=[self.exclude_identifier]).visit(query.distribution.values)
+
+        # remove all defined and prologue vars from free vars
+        self.free_vars = self.free_vars - self.defined_vars - self.prologue_vars
 
         query.scope = self
 
     def visit_Constant(self, node):
         if type(node.value) is not str: return super().visit_Constant(node)
         qstring = node.value
 
@@ -71,40 +129,55 @@
                 continue
             try:
                 parsed = ast.parse(v).body[0].value
                 self.visit(parsed)
             except:
                 raise RuntimeError("Failed to parse fstring expression: ", v)
 
-            
-            # if v not in self.defined_vars and v not in self.free_vars and v not in self.written_vars:
-            #     self.free_vars.add(v)
-
         # put double curly braces back in
         qstring = qstring.replace("__curly_open__", "{{").replace("__curly_close__", "}}")
                 
         template_tags = [v[1:-1] for v in re.findall("\{:[A-z0-9]+\}", qstring)]
         for tt in template_tags:
             qstring = qstring.replace(f"{{{tt}}}", f"{{lmql.tag('{tt[1:]}')}}")
         
         node.value = qstring
 
         return super().visit_Constant(node)
 
+    def exclude_identifier(self, name):
+        # make sure "input" can be intercepted
+        if name in ["input"]:
+            return False
+        if name in self.free_vars:
+            return True
+        if name in self.written_vars:
+            return True
+        # exclude LMQL built-ins
+        if get_builtin_name(name) is not None:
+            return True
+        # exclude Python built-ins
+        if __builtins__.get(name) is not None:
+            return True
+        if name in get_all_decoders():
+            return True
+        return False
+
     def visit_Name(self, node: ast.Name):
         name = str(node.id)
         
         if type(node.ctx) is ast.Store:
             self.written_vars.add(name)
             if name in self.free_vars:
                 self.free_vars.remove(name)
             
         if type(node.ctx) is ast.Load:
-            if name not in self.free_vars and name not in self.written_vars:
-                self.free_vars.add(name)
+            if self.exclude_identifier(name):
+                return
+            self.free_vars.add(name)
         
         return True
 
 class QueryStringTransformation(ast.NodeTransformer):
     """
     Transformes string expressions on statement level to model queries.
     """
@@ -348,17 +421,20 @@
 def is_allowed_builtin_python_call(node):
     if type(node) is not ast.Name:
         return False
     allowed_builtin_functions = set(["set", "all"])
     return node.id in allowed_builtin_functions
 
 def get_builtin_name(node, plain_python=False):
-    if type(node) is not ast.Name:
-        return None
-    n = node.id
+    if type(node) is str:
+        n = node
+    else:
+        if type(node) is not ast.Name:
+            return None
+        n = node.id
     
     if n in lmql_operation_registry.keys():
         return OPS_NAMESPACE + "." + lmql_operation_registry[n]
     
     return None
 
 def is_type_constraint(expr: ast.Expr):
```

### Comparing `lmql-0.0.6.1/src/lmql/language/fragment_parser.py` & `lmql-0.0.6.2/src/lmql/language/fragment_parser.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/language/qstrings.py` & `lmql-0.0.6.2/src/lmql/language/qstrings.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/language/validator.py` & `lmql-0.0.6.2/src/lmql/language/validator.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/model/async_generation_utils.py` & `lmql-0.0.6.2/src/lmql/model/async_generation_utils.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/model/local_client.py` & `lmql-0.0.6.2/src/lmql/model/local_client.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/model/serve.py` & `lmql-0.0.6.2/src/lmql/model/serve.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/model/served_model.py` & `lmql-0.0.6.2/src/lmql/model/served_model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ops/follow_map.py` & `lmql-0.0.6.2/src/lmql/ops/follow_map.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ops/ops.py` & `lmql-0.0.6.2/src/lmql/ops/ops.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,46 +61,74 @@
         Orders application of postprocessing operations. Returns "before", "after" or 0 if order is not defined.
         
         Only invoked for `other` operations, that return true for the same `postprocess_var`.
         """
         return 0 # by default, no order is defined (only one postprocessing operation per variable can be applied)
 
 def DynamicTypeDispatch(name, type_map):
-    def get_handler(args):
-        for signature, op in type_map:
-            # fallback implementation
-            if signature == "*": return op
-            
-            # check for matching signature
-            is_match = True
-            if type(signature) is tuple:
-                for arg, t in zip(args, signature):
-                    is_match = is_match and isinstance(arg, t)
-            else:
-                is_match = isinstance(args, signature)
-            if is_match: return op
-        raise NotImplementedError("error: no matching implemntation of {} for arguments of type {}".format(name, [type(arg) for arg in args]))
-    
     class TypeDispatchingNode(Node):
+        def __init__(self, *args, **kwargs):
+            super().__init__(*args, **kwargs)
+            
+            self.delegate_args = args
+            self.delegate_kwargs = kwargs
+            self.delegate = None
+
+        def get_handler(self, args):
+            if self.delegate is not None:
+                return self.delegate
+
+            assert all(a is not None for a in args), "Cannot dispatch to handler with None arguments: {}".format(args)
+
+            for signature, op in type_map:
+                # fallback implementation
+                if signature == "*": 
+                    self.delegate = op(*self.delegate_args, **self.delegate_kwargs)
+                    return self.delegate
+                
+                # check for matching signature
+                is_match = True
+                if type(signature) is tuple:
+                    for arg, t in zip(args, signature):
+                        is_match = is_match and isinstance(arg, t)
+                else:
+                    is_match = isinstance(args, signature)
+                if is_match: 
+                    self.delegate = op(*self.delegate_args, **self.delegate_kwargs)
+                    return self.delegate
+            raise NotImplementedError("error: no matching implemntation of {} for arguments of type {}".format(name, [type(arg) for arg in args]))
+
         def forward(self, *args, **kwargs):
-            return get_handler(args).forward(self, *args, **kwargs)
+            if any(a is None for a in args):
+                return None
+            return self.get_handler(args).forward(*args, **kwargs)
         
         def follow(self, *args, **kwargs):
-            return get_handler(args).follow(self, *args, **kwargs)
+            if any(a is None for a in args):
+                return None
+            return self.get_handler(args).follow(*args, **kwargs)
         
         def final(self, *args, **kwargs):
-            return get_handler(args).final(self, *args, **kwargs)
+            if any(a is None for a in kwargs.get("operands")):
+                return None
+            return self.get_handler(kwargs.get("operands")).final(*args, **kwargs)
         
         def __str__(self):
+            if self.delegate is not None:
+                return str(self.delegate)
             return f"<{name}>"
         
         def __repr__(self):
+            if self.delegate is not None:
+                return repr(self.delegate)
             return f"<{name}>"
         
         def __nodelabel__(self):
+            if self.delegate is not None:
+                return self.delegate.__nodelabel__()
             return name
 
     return TypeDispatchingNode
 
 NextToken = "<lmql.next>"
 
 def is_next_token(t): 
@@ -261,36 +289,32 @@
 class TokensOp(Node):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         
         self.depends_on_context = True
 
     def forward(self, x, context, **kwargs):
-        import asyncio
         if x is None: return None
         if x == "": return []
 
-        assert False, "TOKENS() operation is currently not supported"
-
-        tokens = context.runtime.model.sync_tokenize(x)
-        return tokens
+        return tuple(context.runtime.model.sync_tokenize(x))
 
     def follow(self, v, context=None, **kwargs):
         if v is None: return None
         contains_next_token = v != strip_next_token(v)
-        words = self.forward(strip_next_token(v), context)
 
-        # if len(words) > 0 and contains_next_token:
-        #     # allow continuation sub-tokens
-        #     continuation_tokens = tset("[^\u0120].*", regex=True)
-        #     valid_continuations = union(tset("eos"), continuation_tokens)
-        #     components = [((valid_continuations, (words[:-1] + [words[-1] + NextToken])))] + components
-        
+        if not contains_next_token:
+            tokens = tuple(context.runtime.model.sync_tokenize(v))
+            return tokens
+        v = strip_next_token(v)
+        tokens = tuple(context.runtime.model.sync_tokenize(v))
+
         return fmap(
-            ("*", (words + [NextToken]) if contains_next_token else words)
+            ("eos", tokens),
+            ("*", (*tokens, NextToken))
         )
 
     def final(self, x, context, operands=None, result=None, **kwargs):
         return x[0]
 
 @LMQLOp("WORDS")
 class WordsOp(Node):
@@ -328,14 +352,16 @@
     def final(self, x, operands=None, result=None, **kwargs):
         return x[0]
 
 @LMQLOp("len")
 class LenOp(Node):
     def forward(self, x, **kwargs):
         if x is None: return None
+        if type(x) is list or type(x) is tuple:
+            return len(x)
         if type(x) is not str: 
             x = str(x)
         return len(x)
     
     def follow(self, v, **kwargs):
         if v is None: return None
         if type(v) is list or type(v) is tuple:
@@ -346,15 +372,15 @@
             if NextToken not in v:
                 return len(v)
             v = strip_next_token(v)
             
             len_masks = []
             for l,tmask in charlen_tsets().items():
                 len_masks.append((tmask, len(v) + l))
-            
+
             return fmap(*len_masks)
 
     def final(self, x, operands=None, result=None, **kwargs):
         return x[0]
 
 class NotOp(Node):
     def forward(self, op, **kwargs):
@@ -391,48 +417,43 @@
         else: 
             r = transition_table[op1][op2]
         
         return r
 
 def Gt(preds): return Lt(list(reversed(preds)))
 
-class EqOp(Node):
+class EqOpGeneric(Node):
     def __init__(self, predecessors):
         super().__init__(predecessors)
 
     def forward(self, *args, **kwargs):
         return all([a == args[0] for a in args])
 
     def follow(self, *args, **kwargs):
         op1 = args[0]
         op2 = args[1]
         
         if op1 is None or op2 is None:
             return None
         
+        
         if is_next_token(op1):
             if is_next_token(op2): 
                 return fmap(
                     ("*", True)
                 )
             else:
-                return fmap(
-                    (op2, True),
-                    ("*", False)
-                )
+                return InOpStrInSet([]).follow(op1, [op2])
         if is_next_token(op2):
             if is_next_token(op1): 
                 return fmap(
                     ("*", True)
                 )
             else:
-                return fmap(
-                    (op1, True),
-                    ("*", False)
-                )
+                return InOpStrInSet([]).follow(op2, [op1])
 
         if type(op1) is str or type(op1) is str:
             op_shorter = op1 if len(strip_next_token(op1)) < len(strip_next_token(op2)) else op2
             op_longer = op1 if len(strip_next_token(op1)) > len(strip_next_token(op2)) else op2
 
             if strip_next_token(op_longer) == op_longer and strip_next_token(op_shorter) != op_shorter:
                 return InOpStrInSet([]).follow(op_shorter, [op_longer])
@@ -476,14 +497,52 @@
             elif of == "inc":
                 if not fixed_value.startswith(o): return "fin"
             else: # of == "var":
                 continue
         
         return super().final(operand_final, operands=operands, result=result, **kwargs)
 
+class EqOpInt(Node):
+    def __init__(self, predecessors):
+        super().__init__(predecessors)
+
+    def forward(self, *args, **kwargs):
+        return all([a == args[0] for a in args])
+
+    def follow(self, *args, **kwargs):
+        op1 = args[0]
+        op2 = args[1]
+        
+        if op1 is None or op2 is None:
+            return None
+        
+        return op1 == op2
+
+    def final(self, operand_final, operands=None, result=None, **kwargs):
+        op1f = operand_final[0]
+        op1 = operands[0]
+        op2f = operand_final[1]
+        op2 = operands[1]
+
+        if op1f == "fin" and op1 <= op2 and (op2f in ["fin", "inc"]):
+            return "fin"
+        if op2f == "fin" and op2 <= op1 and (op1f in ["fin", "inc"]):
+            return "fin"
+
+        # default behavior
+        if all([a == "fin" for a in operand_final]):
+            return "fin"
+        
+        return "var"
+
+EqOp = DynamicTypeDispatch("EqOp", (
+    ((int, int), EqOpInt),
+    ("*", EqOpGeneric),
+))
+
 class SelectOp(Node):
     def forward(self, *args, **kwargs):
         if len(args[0]) <= args[1]:
             return None
         return args[0][args[1]]
 
     def follow(self, *args, **kwargs):
@@ -618,15 +677,15 @@
         allowed_subtokens = tset(f".*{suffix}.*", regex=True)
 
         return fmap(
             (allowed_subtokens, True),
             (setminus("*", allowed_subtokens), False)
         )
 
-    def final(self, op_final, result=None, **kwargs):
+    def final(self, op_final, operands=None, result=None, **kwargs):
         if not result:
             return super().final(op_final, result=result, **kwargs)
         if op_final[1] == "inc" and op_final[0] == "fin":
             return "fin"
         return super().final(op_final, result=result, **kwargs)
 
 class InOpStrInSet(Node):
@@ -794,39 +853,14 @@
         if op1 == "inc" and op2 == "fin":
             if len(operands[0]) == 0 and not result:
                 return "var"
             return "fin"
         
         return super().final(ops_final, **kwargs)
 
-    # def final(self, args, operands=None, result=None, pattern: TokenSet=None, **kwargs):
-    #     x_final = args[0]
-
-    #     if result is None:
-    #         return "var"
-    #     elif result == False:
-    #         x = operands[0]
-    #         allowed_phrases = operands[1]
-
-    #         if x_final == "inc":
-    #             # check whether there are suffixes which could be matched
-    #             suffixes = list(matching_phrases_suffixes(x, allowed_phrases))
-    #             suffixes = [s for s in suffixes if pattern is None or pattern.starts_with(s)]
-    #             # print("final() with x_final inc", x, allowed_phrases)
-    #             if len(suffixes) > 0: return "var"
-    #             else: return "fin"
-    #         elif x_final == "fin":
-    #             return "fin"
-    #         else:
-    #             return "var"
-    #     else: # result == True
-    #         if x_final == "inc" or x_final == "fin":
-    #             return "fin"
-    #         return "var"
-
 @LMQLOp(["STOPS_AT", "stops_at"])
 class StopAtOp(Node):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._tokenized_stopping_phrase_cache = {}
 
     def execute_predecessors(self, trace, context):
@@ -836,94 +870,73 @@
         var_op.diff_aware_read = True
         return super().execute_predecessors(trace, context)
     
     @property
     def variable(self):
         return self.predecessors[0]
 
-    async def stopping_phrase_tokenized(self, tokenizer):
-        if tokenizer in self._tokenized_stopping_phrase_cache:
-            return self._tokenized_stopping_phrase_cache[tokenizer]
-        else:
-            result = (await tokenizer(self.stopping_phrase))
-            self._tokenized_stopping_phrase_cache[tokenizer] = result
-            return result
-
     def forward(self, *args, final, **kwargs):
-        if any([a is None for a in args]): return None
+        return True
 
-        if all([a == "fin" for a in final]):
-            return True
-
-        op1, op1_diff = args[0]
-        op2 = args[1]
+    def follow(self, *args, previous_result=None, **kwargs):
+        return fmap(("*", True))
 
-        if op1 is None: return
-        if op1_diff is None: op1_diff = ""
+    def final(self, ops_final, operands, result, **kwargs):
+        return "var"
 
-        matched_phrase_index = op1.rfind(op2)
-        op2_in_op1 = matched_phrase_index != -1 and matched_phrase_index + len(op2) > len(op1) - len(op1_diff)
+    def stop(self, *args, final, **kwargs):
+        if any([a is None for a in args]): return None
 
-        return not op2_in_op1 or op1.endswith(op2)
-
-    def follow(self, *args, previous_result=None, **kwargs):
-        if any([a is None for a in args]): 
-            return None
+        if all([a == "fin" for a in final]): return False
 
         op1, op1_diff = args[0]
-        if op1 is None: return None
-        if op1_diff is None: op1_diff = ""
-
-        op1 = strip_next_token(op1)
         op2 = args[1]
 
-        matched_phrase_index = op1.rfind(op2)
-        op2_in_op1 = matched_phrase_index != -1 and matched_phrase_index + len(op2) > len(op1) - len(op1_diff)
+        if op1 is None: return False
+        if op1_diff is None: op1_diff = ""
 
-        if not op2_in_op1: return fmap(("*", True))
 
-        ends_with_stopping_phrase = op1.endswith(op2)
+        matched_phrase_index = op1.rfind(op2)
+        match_only_with_diff = op2 in op1 and matched_phrase_index >= len(op1) - len(op1_diff)
 
-        if op1 != args[0][0] and ends_with_stopping_phrase:
-            # print("StopAtOp.follow()", [op1], [op2], valid)
-            ends_with_stopping_phrase = False
-        if len(op1) == 0:
-            ends_with_stopping_phrase = True
-        
-        return fmap(("*", ends_with_stopping_phrase))
+        return match_only_with_diff or op1.endswith(op2)
 
-    def final(self, ops_final, operands, result, **kwargs):
-        if result: 
-            if ops_final[0] == "var":
-                return "var"
-            return "fin"
-        else: # not result
-            if ops_final[0] == "var": 
-                r = "var"
-            elif ops_final[0] == "dec": 
-                r = "var"
-            else: 
-                r = "fin"
-            return r
+    def stopping_phrase(self, trace):
+        if type(self.predecessors[1]) is Node:
+            return trace[self.predecessors[1]]
+        return self.predecessors[1]
 
     def postprocess_var(self, var_name):
         return var_name == self.predecessors[0].name
 
     def postprocess(self, operands, value):
-        op2 = operands[1]
-        matched_phrase_index = value.rfind(op2)
+        if value != operands[0][0]:
+            return value
+        value_diff: str = operands[0][1]
+        stopping_phrase = operands[1]
+
+        # find earliest match of stopping phrase in value_diff
+        matched_phrase_index = value.rfind(stopping_phrase)
+        next_matched_phrase_index = value.rfind(stopping_phrase, 0, matched_phrase_index)
+        while next_matched_phrase_index != -1 and next_matched_phrase_index >= len(value) - len(value_diff):
+            matched_phrase_index = next_matched_phrase_index
+            next_matched_phrase_index = value.rfind(stopping_phrase, 0, matched_phrase_index)
+
+        if matched_phrase_index + len(stopping_phrase) <= len(value) - len(value_diff):
+            return None
+
         if matched_phrase_index != -1:
-            value = value[:matched_phrase_index + len(op2)]
+            value = value[:matched_phrase_index + len(stopping_phrase)]
 
         return postprocessed_rewrite(value), postprocessed_value(value)
     
     def postprocess_order(self, other, operands, other_inputs, **kwargs):
         if type(other) is IntOp:
             return "before"
-        if type(other) is StopAtOp:
+        if isinstance(other, StopAtOp):
             value, value_diff = operands[0]
             op2 = operands[1]
             assert value == other_inputs[0][0], "internal error: comparing postprocess_order with two StopAtOps with different values (do they refer to different variables) {}".format((value, other_inputs[0]))
             matched_phrase_index = value.rfind(op2)
             other_matched_phrase_index = other_inputs[0][0].rfind(other_inputs[1])
             if matched_phrase_index == -1:
                 return "before" # this operator does not match, so order does not matter
@@ -935,24 +948,32 @@
                 return "after"
         
         return 0 # other constraints cannot be compared
 
 @LMQLOp(["STOPS_BEFORE", "stops_before"])
 class StopBeforeOp(StopAtOp):
     def postprocess(self, operands, value):
-        op2 = operands[1]
-        matched_phrase_index = value.find(op2)
+        value: str = operands[0][0]
+        value_diff: str = operands[0][1]
+        stopping_phrase = operands[1]
+
+        # find earliest match of stopping phrase in value_diff
+        matched_phrase_index = value.rfind(stopping_phrase)
+        next_matched_phrase_index = value.rfind(stopping_phrase, 0, matched_phrase_index)
+        while next_matched_phrase_index != -1 and next_matched_phrase_index >= len(value) - len(value_diff):
+            matched_phrase_index = next_matched_phrase_index
+            next_matched_phrase_index = value.rfind(stopping_phrase, 0, matched_phrase_index)
+
+        if matched_phrase_index + len(stopping_phrase) <= len(value) - len(value_diff):
+            return None
+
         if matched_phrase_index != -1:
             value = value[:matched_phrase_index]
 
         return postprocessed_rewrite(value), postprocessed_value(value)
-    
-    @property
-    def stopping_phrase(self):
-        return self.predecessors[1]
 
 class OpaqueLambdaOp(Node):
     def forward(self, *args, **kwargs):
         if any([a is None for a in args]): return None
         fct, *args = args
         return fct(*args)
     
@@ -1028,52 +1049,65 @@
 
     context_arg = ()
     if op.depends_on_context: 
         context_arg += (context,)
     
     return op.final(predecessor_final, *context_arg, operands=predecessor_values, result=result)
 
-def execute_op_stops_at_only(op: Node, result=None):
+def execute_op_stops_at_only(variable: str, op: Node, trace, result=None, sidecondition=None):
     """
     Evaluates a Node and returns the list of defined StopAtOps for the query.
     """
-    if result is None: result = []
-
-    if type(op) is StopBeforeOp:
-        result.append(op)
+    is_root_call = result is None and sidecondition is None
+    
+    if result is None: 
+        result = []
+    if sidecondition is None: 
+        sidecondition = []
+
+    if isinstance(op, StopAtOp):
+        if op.predecessors[0].name == variable:
+            result.append((op, sidecondition.copy()))
     elif type(op) is AndOp:
+        non_stop_ops = [o for o in op.predecessors if not isinstance(o, StopAtOp)]
         for p in op.predecessors:
-            execute_op_stops_at_only(p, result=result)
+            execute_op_stops_at_only(variable, p, trace=trace, result=result, sidecondition=sidecondition + non_stop_ops)
     elif type(op) is OrOp:
-        subresults = []
         for p in op.predecessors:
-            subresult = []
-            execute_op_stops_at_only(p, result=subresult)
-            subresults.append(subresult)
-        # intersect subresults
-        result += list(set.intersection(*[set(r) for r in subresults]))
-
+            execute_op_stops_at_only(variable, p, trace=trace, result=result, sidecondition=sidecondition)
+    elif type(op) is NotOp:
+        negated_stop_ops = []
+        execute_op_stops_at_only(variable, op.predecessors[0], trace=trace, result=negated_stop_ops)
+        assert len(negated_stop_ops) == 0, "error: nesting stopping operators with 'not' expressions is not supported"
     else:
         # other ops are no-ops from a STOPS_AT perspective (cannot contain additional STOPS_AT ops)
         # TODO: what about not
         return []
+    
+    if is_root_call:
+        # only return stop ops whose sidecondition are all satisfied
+        result = [sp for sp, sc in result if all(trace[p][0] is None or trace[p][0] for p in sc)]
+    
     return result
 
-def execute_postprocess(op: Node, var_name: str, value: str, trace=None, context=None):
+def execute_postprocess(op: Node, var_name: str, value: str, context=None):
     """
     Applies any postprocess() operations of the provided constraints
     to the specified variable and value.
 
     Returns a tuple of (postprocessed_value, rewritten_prompt)
     """
     if op is None: return value, value
 
+    root_op = op
     nodes = [op]
 
     trace = {}
+    expr_value = execute_op(op, trace=trace, context=context, return_final=False)
+    
     postprocessors = []
 
     # collect and sort set of postprocessing operations
     while len(nodes) > 0:
         op = nodes.pop()
         nodes += [p for p in op.predecessors if isinstance(p, Node)]
 
@@ -1088,25 +1122,28 @@
                 if relative_order == "before":
                     break
                 elif relative_order == "after":
                     i += 1
                 else:
                     assert len(postprocessors) == 0, "The specified set of constraints contains multiple incompatible postprocessing operations for the same variable. The conflicting operations are: {} and {}. Please make sure the used constraints implement postprocess_order for each other, to use them together.".format(current_op, op)
             postprocessors.insert(i, (op, inputs))
-    
+
+    # filter out stopping conditions as postprocessors that were not actually triggered (due to unfulfilled sideconditions)
+    stopping_conditions: List[StopAtOp] = execute_op_stops_at_only(var_name, root_op, trace)
+    postprocessors = [p for p in postprocessors if not isinstance(p[0], StopAtOp) or p[0] in stopping_conditions]
+
     rewritten_value = None
     rewritten_prompt = value
 
     # apply postprocessing operations
     for pop in postprocessors:
         pop, inputs = pop # unpack to get op and inputs
         result = pop.postprocess(inputs, rewritten_prompt)
 
         if result is not None:
-            
             if type(result) is tuple:
                 for v in result:
                     if type(v) is postprocessed_value:
                         rewritten_value = v.value
                     elif type(v) is postprocessed_rewrite:
                         rewritten_prompt = v.rewrite
                     else:
@@ -1117,15 +1154,15 @@
     if rewritten_prompt is None:
         rewritten_prompt = str(value)
     if rewritten_value is None:
         rewritten_value = value
     
     return rewritten_value, rewritten_prompt
 
-def execute_op(op: Node, trace=None, context=None, return_final=False):
+def execute_op(op: Node, trace=None, context=None, return_final=False, semantics="forward"):
     # for constant dependencies, just return their value
     if not is_node(op): 
         return op
     
     # only evaluate each operation once
     if op in trace.keys(): 
         return trace[op][0]
@@ -1133,15 +1170,16 @@
     # compute predecessor values
     inputs = op.execute_predecessors(trace, context)
     
     if op.depends_on_context: 
         inputs += (context,)
 
     inputs_final = derive_predecessor_final(op, trace)
-    result = op.forward(*inputs, final=inputs_final)
+    semantics_fct = op.__getattribute__(semantics)
+    result = semantics_fct(*inputs, final=inputs_final)
     is_final = derive_final(op, trace, context, result)
     
     if trace is not None: 
         trace[op] = (result, is_final)
 
     if return_final:
         return result, is_final
```

### Comparing `lmql-0.0.6.1/src/lmql/ops/token_set.py` & `lmql-0.0.6.2/src/lmql/ops/token_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from tokenize import Token
 from typing import Iterable, Tuple
 from itertools import product
 
 from lmql.utils import nputil
 import numpy as np
 from lmql.runtime.stats import Stats
-
+from lmql.runtime.caching import cachefile, cache_file_exists
 from lmql.runtime.tokenizer import get_vocab
 
 class VocabularyMatcher:
     """
     Generates sub-token level logit masks from provided tokens.
     """
     def __init__(self, tokenizer, model_identifier):
@@ -36,69 +36,62 @@
     @staticmethod
     def init(tokenizer):
         if VocabularyMatcher._instance is not None:
             return
 
         # first try to load pickled matcher from cache (faster)
         import pickle
-        import pathlib
 
-        cache_dir = pathlib.Path.home() / ".cache" / "lmql"
-        cache_dir.mkdir(parents=True, exist_ok=True)
         cache_identifier = tokenizer.model_identifier.replace("/", "-")
-        cache_path = cache_dir / f"token-mask-cache-{cache_identifier}.pkl"
-        matcher_path = cache_dir / f"matcher-{cache_identifier}.pkl"
+        cache_path = f"token-mask-cache-{cache_identifier}.pkl"
+        matcher_path = f"matcher-{cache_identifier}.pkl"
 
         try:
-            with open(matcher_path, "rb") as f:
+            assert False
+            with cachefile(matcher_path, "rb") as f:
                 VocabularyMatcher._instance = pickle.load(f)
                 VocabularyMatcher._instance.stats = Stats("VocabularyMatcher")
         except:
             VocabularyMatcher._instance = VocabularyMatcher(tokenizer, tokenizer.model_identifier)
 
-        if cache_path.exists():
-            with open(cache_path, "rb") as f:
+        if cache_file_exists(cache_path) and False:
+            with cachefile(cache_path, "rb") as f:
                 try:
                     import time
                     s = time.time()
                     VocabularyMatcher.cache = pickle.load(f)
                     VocabularyMatcher._instance.disk_cached = len(VocabularyMatcher.cache)
                     # print("Matcher cache loaded in {}s".format(time.time() - s))
                 except:
                     print("Failed to load token mask cache from {}. If the cache is corrupted, please delete it.".format(cache_path))
 
         atexit.register(lambda: VocabularyMatcher._instance.save())
 
     def save(self):
         # save cache to disk
         import pickle
-        import pathlib
-
-        # assert False
 
-        cache_dir = pathlib.Path.home() / ".cache" / "lmql"
-        cache_dir.mkdir(parents=True, exist_ok=True)
         cache_identifier = self.model_identifier.replace("/", "-")
-        cache_path = cache_dir / f"token-mask-cache-{cache_identifier}.pkl"
-        matcher_path = cache_dir / f"matcher-{cache_identifier}.pkl"
+        cache_path = f"token-mask-cache-{cache_identifier}.pkl"
+        matcher_path = f"matcher-{cache_identifier}.pkl"
 
-        with open(matcher_path, "wb") as f:
+        with cachefile(matcher_path, "wb") as f:
             stats = self.stats
             self.stats = None
             pickle.dump(self, f)
             self.stats = stats
 
         def is_cached(k):
             if k.startswith("named:"):
                 return True
             if k.startswith("charlen:"):
                 return True
             return False
 
-        with open(cache_path, "wb") as f:
+        with cachefile(cache_path, "wb") as f:
             pickle.dump({k: v for k, v in VocabularyMatcher.cache.items() if is_cached(k)}, f)
 
     @staticmethod
     def instance():
         if VocabularyMatcher._instance is None:
             raise Exception("VocabularyMatcher not initialized.")
         return VocabularyMatcher._instance
@@ -545,15 +538,15 @@
 
 def charlen_tsets():
     l1 = tset(charlen=1)
     token_lengths = VocabularyMatcher.instance().token_lengths
     assert token_lengths is not None, "VocabularyMatcher.instance().token_lengths is None even though it should be fully initialized."
     # get unique values in token_lengths (numpy)
     length_values = np.unique(token_lengths)
-    return {l: tset(charlen=l) for l in length_values}
+    return {int(l): tset(charlen=l) for l in length_values}
 
 def ntset(*tokens):
     if len(tokens) == 1 and type(tokens[0]) is set:
         return TokenSet(set(list(tokens[0])), minus=True)
     return TokenSet(set(tokens), minus=True)
 
 class ArgTuple(tuple):
```

### Comparing `lmql-0.0.6.1/src/lmql/output/http.py` & `lmql-0.0.6.2/src/lmql/output/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,11 +54,11 @@
         # get post data
         if request.method == "POST":
             payload = await request.json()
         # get query parameters
         elif request.method == "GET":
             payload = request.query
 
-        kwargs = {**payload, **kwargs}
+        query_kwargs = {**payload, **(kwargs.copy())}
 
-        return await serve(request, q, *args, output_writer_cls=output_writer_cls, **kwargs)
+        return await serve(request, q, *args, output_writer_cls=output_writer_cls, **query_kwargs)
     return handler
```

### Comparing `lmql-0.0.6.1/src/lmql/output/sse.py` & `lmql-0.0.6.2/src/lmql/output/sse.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/output/ws.py` & `lmql-0.0.6.2/src/lmql/output/ws.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/bopenai/__init__.py` & `lmql-0.0.6.2/src/lmql/runtime/bopenai/__init__.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/bopenai/batched_openai.py` & `lmql-0.0.6.2/src/lmql/runtime/bopenai/batched_openai.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/bopenai/openai_api.py` & `lmql-0.0.6.2/src/lmql/runtime/bopenai/openai_api.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_array.py` & `lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_array.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_cache.py` & `lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,52 @@
 from .dclib_array import DataArray
 from .dclib_seq import DecoderSequence, Continuation, DeterministicDecoderSequence, deepcopy, deepmerge, detseq
 from .dclib_model import DcModel, CacheDelegate
 from .dclib_rewrite import DcModelRewriteMixin
 import lmql.runtime.masks as masks
 from lmql.utils.nputil import ensure_iterable
 
+class CacheFile:
+    def __init__(self, filename, initial_ids, model):
+        self.filename = filename
+        self.initial_ids = initial_ids
+        self.model = model
+    
+    def load(self):
+        if self.filename is not None and os.path.exists(self.filename):
+            with open(self.filename, "rb") as f:
+                cache = pickle.load(f)
+                if cache.get("model") != self.model:
+                    print("warning: cache file is from a different model. Its contents will be overwritten. {} != {}".format(cache["model"], self.model))
+                else:
+                    if not str(self.initial_ids) in cache.keys():
+                        print(str(self.initial_ids))
+                        print("cache miss for", self.filename, cache.keys())
+                    return cache.get(str(self.initial_ids), {})
+        return {}
+    
+    def save(self, cache):
+        if os.path.exists(self.filename):
+            with open(self.filename, "rb") as f:
+                existing_cache = pickle.load(f)
+                if existing_cache.get("model") != self.model:
+                    print("warning: cache file is from a different model. Its contents will be overwritten. {} != {}".format(cache.get("model"), self.model))
+                    existing_cache = {}
+        else:
+            existing_cache = {}
+        if "model" in existing_cache.keys() and existing_cache["model"] != self.model:
+            print("warning: cache file is from a different model. Its contents will be overwritten. {} != {}".format(existing_cache.get("model"), self.model))
+            existing_cache = {}
+        existing_cache["model"] = self.model
+        existing_cache[str(self.initial_ids)] = cache
+        
+        with open(self.filename, "wb") as f:
+            pickle.dump(existing_cache, f)
+
+
 class CachedDcModel(DcModelRewriteMixin, CacheDelegate):
     delegate: DcModel
     
     def __new__(cls, delegate: DcModel, initial_prompt_ids=None, cache_file=None, show_speculative=False):
         mc = super().__new__(cls)
         
         mc.delegate: DcModel = delegate
@@ -29,56 +67,47 @@
         
         mc.cache = {}
         mc.user_data_cache = {}
         mc.cache_lock = asyncio.Lock()
 
         mc.mask_cache = {}
         mc.show_speculative = show_speculative
+        mc.initial_ids = initial_prompt_ids
         
         mc.input_id_key_offset = len(initial_prompt_ids) if initial_prompt_ids else 0
         mc.initial_prompt_ids = initial_prompt_ids
-        mc.cache["initial_prompt_ids"] = str(initial_prompt_ids) if initial_prompt_ids is not None else None
         mc.cache["model"] = delegate.model_identifier
     
         mc.calls = 0
         mc.hits = 0
 
         mc.cache_file = cache_file
 
         try:
-            if cache_file is not None and os.path.exists(cache_file):
-                with open(cache_file, "rb") as f:
-                    cache = pickle.load(f)
-                    if cache.get("model") != delegate.model_identifier:
-                        print("warning: cache file is from a different model. Its contents will be overwritten.")
-                    else:
-                        mc.cache = cache.get(str(initial_prompt_ids), {})
+            mc.cache = CacheFile(cache_file, initial_prompt_ids, delegate.model_identifier).load()
         except Exception as e:
             print("error: failed to load token cache from file", e)
             pass
 
         return mc
     
     def close(self):
         self.model.cache_delegate = None
         for ts in self.token_streams:
             ts.cancel()
         self.token_streams = []
 
     def save(self):
         if self.cache_file is not None:
-            if os.path.exists(self.cache_file):
-                with open(self.cache_file, "rb") as f:
-                    cache = pickle.load(f)
-            else:
-                cache = {}
-            cache[str(self.initial_prompt_ids)] = self.cache
-            cache["model"] = self.cache["model"]
-            with open(self.cache_file, "wb") as f:
-                pickle.dump(cache, f)
+            cf = CacheFile(self.cache_file, self.initial_ids, self.delegate.model_identifier)
+            try:
+                cf.save(self.cache)
+            except Exception as e:
+                print("error: failed to save token cache to file", e, flush=True)
+                pass
     
     def base_key(self, ids, *args):
         if isinstance(ids, DecoderSequence):
             return self.base_key(ids.input_ids)
         return str(ids[self.input_id_key_offset:])
 
     async def get_mask(self, s: DecoderSequence, **kwargs):
```

### Comparing `lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_global.py` & `lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_global.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_model.py` & `lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_rewrite.py` & `lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_rewrite.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_seq.py` & `lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_seq.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/dclib/decoders.py` & `lmql-0.0.6.2/src/lmql/runtime/dclib/decoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     T = 0
 
     base_scorer = dc.alpha_length_normalized()
     while T < budget and len(h) > 0 or len(done) == 0:
         scorer = BestKScorer(base_scorer, t, kappa, beta)
         H, h = dc.seperate_topk(h, k, scorer=scorer)
         g = len(H)
-        H = H.extend(await model.topk_continuations(H, k=top_k_continuations))
+        H = H.extend(await model.topk_continuations(H, k=top_k_continuations, **kwargs))
         H = await model.rewrite(H)
         not_done = dc.logical_and(dc.logical_not(dc.eos), dc.lt(max_len))
         H, H_done = H.separate_by(not_done)
         # print(len(H), len(H_done))
         done = (done + H_done)
         H = H.filter(lambda s: np.exp(s.logprobs[-1]) >= gamma)
         H.data('time', t)
@@ -210,15 +210,15 @@
 
             h = non_det
             h, done_new = (h + done).separate_by(not_done)
             num_completed += len(done_new) - len(done)
             done = done_new
 
         h_before_extension = h
-        h_extended = h.extend(await model.topk_continuations(h, k=n))
+        h_extended = h.extend(await model.topk_continuations(h, k=n, **kwargs))
 
         if inject_stop:
             h_injected = await h_before_extension.aelement_wise(stop_phrase_injection, model, **kwargs)
             h_extended = (h_injected + h_extended)
             h_extended_shape = h_extended.shape
             h_extended = dc.token_unique(h_extended, lambda s, t: dc.is_deterministic(s), flatten=True)
             h_extended = h_extended.reshape(h_extended_shape)
@@ -428,15 +428,15 @@
         i = 0
 
         while not is_seq_beams_search_done(active, variable_done, num_beams=b):
             # inner variable decoding (beam_sample with 2*n beams and branching factor n)
             if sample:
                 active = active.extend(await model.sample(active, temperature=temperature, num_samples=b))
             else:
-                active = active.extend(await model.topk_continuations(active, k=b))
+                active = active.extend(await model.topk_continuations(active, k=b, **kwargs))
             
             active = await model.rewrite(active)
 
             active, variable_done = (active + variable_done).separate_by(is_active_variable)
             active = dc.topk(active, b)
 
             active.name(str(active_variable.get()) + "[" + str(i) + "]_")
@@ -451,15 +451,15 @@
         top_variable_done = dc.seqs()
 
         while not (len(active) == 0 or (len(top_variable_done) == b and dc.max_score(active, scorer=nw_score) < dc.min_score(top_variable_done, scorer=nw_score))):
             # inner variable decoding (beam_sample with 2*n beams and branching factor n)
             if sample:
                 active = active.extend(await model.sample(active, temperature=temperature, num_samples=b))
             else:
-                active = active.extend(await model.topk_continuations(active, k=b))
+                active = active.extend(await model.topk_continuations(active, k=b, **kwargs))
             
             for s in active.flatten().items():
                 # s.data("eos_score", s.score
                 s.data("eos_score", regular_scorer(s.logprobs))
 
             active = await model.rewrite(active)
 
@@ -495,22 +495,23 @@
 @dc.decoder
 async def bsseq(prompt_ids: np.ndarray, b=2, max_len=384, **kwargs):
     kwargs.pop("n", None)
     async for s in var(prompt_ids, b=b, n=1, max_len=max_len, subdecoder="beam_seq", **kwargs):
         yield s
 
 @dc.decoder
-async def var(prompt_ids: np.ndarray, b=2, n=None, max_len=384, subdecoder="sample", **kwargs):
+async def var(prompt_ids: np.ndarray, b=2, n=None, max_len=384, subdecoder="sample", temperature=1.0, **kwargs):
     """
     sample: 
         if True, uses beam_sample variable-local-decoding, otherwise uses beam_search-like decoding
     var_temperature: 
         sampling temperature to use to obtain multiple variable values
     """
     model = dc.model(**kwargs)
+    kwargs.update({"temperature": temperature})
 
     # keep track of active beams and finished sequences
     variable_done = dc.seqs([dc.seq(prompt_ids)])
     active_variable = shared(None)
     done = dc.seqs()
     is_not_done = dc.logical_and(dc.logical_not(dc.eos), dc.lt(max_len))
```

### Comparing `lmql-0.0.6.1/src/lmql/runtime/dclib/trie_cache.py` & `lmql-0.0.6.2/src/lmql/runtime/dclib/trie_cache.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/hf_integration.py` & `lmql-0.0.6.2/src/lmql/runtime/hf_integration.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/interpreter.py` & `lmql-0.0.6.2/src/lmql/runtime/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 import asyncio
 from collections import namedtuple
 
 from dataclasses import dataclass
-from typing import Any, Dict, Optional, List, Union, NamedTuple
+from typing import Any, Dict, Optional, List, Union, NamedTuple, Tuple
 import numpy as np
 from lmql.runtime.multi_head_interpretation import InterpretationHead, InterpreterCall, InterpretationHeadDone
 from lmql.runtime.program_state import ProgramState
 import lmql.runtime.dclib as dc
 from lmql.runtime.stats import Stats
 from lmql.runtime.tokenizer import LMQLTokenizer
 from lmql.runtime.interrupt import interrupt
@@ -139,14 +139,15 @@
         self.model = force_model
         self.model_identifier = force_model
         self.tokenizer: LMQLTokenizer = None
 
         # decoder configuration
         self.decoder = None
         self.decoder_kwargs = {}
+        self.decoder_step = 0
         
         # extra interpreter flags passed via @lmql.query/@lmql.compiled_query
         self.extra_kwargs = {}
 
         # query program
         self.fct = None
         self.root_state = None
@@ -385,29 +386,40 @@
 
             # digest token with where expr
             valid, is_final, trace, follow_trace = ops.digest(self.where,
                 context=program_state,
                 follow_context=follow_program_state
             )
 
-            stopping_conditions: List[ops.StopAtOp] = ops.execute_op_stops_at_only(self.where)
-            stopping_phrases = {
-                "tokenized": [await self.tokenize(sc.stopping_phrase) for sc in stopping_conditions if sc.variable.name == variable],
-                "text": [sc.stopping_phrase for sc in stopping_conditions if sc.variable.name == variable],
-            }
-
             # obtain where follow map
             follow_map = follow_trace[self.where] if self.where is not None else None
             # print(id(self), self.variable, [text], "mask", follow_map)
             mask = ops.create_mask(follow_map, valid, is_final)
 
             if mask == "*": 
                 logit_mask = None
             else:
                 logit_mask = mask.mask
+            
+            # check stopping conditions
+            stopping_conditions: List[ops.StopAtOp] = ops.execute_op_stops_at_only(state.variable, self.where, trace)
+            for sc in stopping_conditions:
+                stop_trace = trace.copy()
+                del stop_trace[sc]
+                # check if stopping phrase applies in this step
+                if ops.execute_op(sc, stop_trace, context=program_state, semantics="stop"):
+                    # print("apply stop", sc, [text], [diff_text])
+                    mask = tset("eos")
+                    logit_mask = mask.mask
+                    trace[sc] = (sc.stopping_phrase(trace), "stopped")
+            stopping_phrases = {
+                "text": [sc.stopping_phrase(trace) for sc in stopping_conditions if type(sc) is ops.StopBeforeOp],
+                "tokenized": [self.tokenizer(sc.stopping_phrase(trace))["input_ids"] for sc in stopping_conditions if type(sc) is ops.StopBeforeOp]
+            }
+
         else:
             assert False, f"error: where() is called but current variable and current prompt are None and query head has result {state.query_head.result}"
 
         await self.debugger_output(state, s, valid, is_final, mask, stopping_phrases, program_state, trace, text)
 
         state = state.updated(
                         variable=variable,
@@ -474,19 +486,21 @@
         assert state is not None, "prompt interpreter state must be set in predecessor node"
 
         if seq.is_done() and state.variable is not None:
             program_state = state.program_state.copy()
             variable = state.variable
             
             text = (await seq.text(offset=state.variable_offset, limit=-1, pretty=False))
+            text_diff = text[len(await seq.text(state.variable_offset, limit=-2, pretty=False)):]
+            
             assert seq.input_ids[-1] == self.tokenizer.eos_token_id, "last token must be eos token"
             variable_value = text
-            raw = variable_value
             # set raw variable value
-            program_state.set(variable, variable_value, scores=(), diff="", montonicity="fin")
+            program_state.set(variable, variable_value, scores=(), diff=text_diff, montonicity="fin")
+            
             # apply postprocessing, if constraints specify it
             # - variable_value is the postprocessed, converted value (does not have to be a string)
             # - postprocessed_prompt is the string in the prompt that corresponds to the variable value
             variable_value, postprocessed_prompt = ops.execute_postprocess(self.where, variable, variable_value, context=program_state)
             
             # set postprocessed variable value and program value
             program_state.set(variable, postprocessed_prompt, program_value=variable_value, scores=(), diff="", montonicity="fin")
@@ -633,14 +647,17 @@
 
         # pass processor as decoder argument
         decoder_args["modern_logits_processor"] = self.where_processor
         
         # pass rewriter as decoder argument
         decoder_args["modern_rewriter"] = self.rewrite_processor
 
+        if "__get_where__" in decoder_args:
+            return self.where
+
         if "output_writer" in decoder_args:
             set_dclib_debug_printer(decoder_args["output_writer"])
         elif self.output_writer is not None:
             set_dclib_debug_printer(self.output_writer)
 
         if _DCLibDebugPrinter.printer is not None:
             if hasattr(_DCLibDebugPrinter.printer, "records_graph"):
```

### Comparing `lmql-0.0.6.1/src/lmql/runtime/langchain.py` & `lmql-0.0.6.2/src/lmql/runtime/langchain.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/lmql_runtime.py` & `lmql-0.0.6.2/src/lmql/runtime/lmql_runtime.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/maiohttp.py` & `lmql-0.0.6.2/src/lmql/runtime/maiohttp.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/masks.py` & `lmql-0.0.6.2/src/lmql/runtime/masks.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/model_registry.py` & `lmql-0.0.6.2/src/lmql/runtime/model_registry.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/multi_head_interpretation.py` & `lmql-0.0.6.2/src/lmql/runtime/multi_head_interpretation.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/openai_integration.py` & `lmql-0.0.6.2/src/lmql/runtime/openai_integration.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/openai_secret.py` & `lmql-0.0.6.2/src/lmql/runtime/openai_secret.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/output_writer.py` & `lmql-0.0.6.2/src/lmql/runtime/output_writer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/postprocessing/conditional_prob.py` & `lmql-0.0.6.2/src/lmql/runtime/postprocessing/conditional_prob.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/program_state.py` & `lmql-0.0.6.2/src/lmql/runtime/program_state.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/stats.py` & `lmql-0.0.6.2/src/lmql/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/runtime/tokenizer.py` & `lmql-0.0.6.2/src/lmql/runtime/tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,71 +1,82 @@
 import asyncio
+from lmql.runtime.caching import cache_file_exists, cachefile
 
-def get_js_tokenizer(model_identifier):
-    import js
-    from pyodide.ffi import to_js
-
-    assert "gpt" in model_identifier, "JS tokenizer only supports GPT models."
-
-    class JSBridgedTokenizer:
-        """ Custom tokenizer to be used only in a browser environment. This tokenizer only supports GPT tokenization. """
-        def __init__(self):
-            self.bos_token_id = 50256
-            self.eos_token_id = 50256
-            self._vocab = None
-
-        @property
-        def vocab_size(self):
-            return len(self.vocab)
-
-        @property
-        def vocab(self):
-            if self._vocab is None:
-                self._vocab = js.get_vocab().to_py()
-            return self._vocab
-
-        def convert_tokens_to_string(self, tokens):
-            return js.convert_tokens_to_string_gpt(to_js(tokens))
-
-        def tokenize(self, s):
-            unpack = False
-            if type(s) is not list:
-                s = [s]
-                unpack = True
-            tokens = [js.tokenize_gpt_toks(se).to_py() for se in s]
-            
-            if unpack:
-                return tokens[0]
-            else:
-                return tokens
-         
-        def decode(self, input_ids, clean_up_tokenization_spaces=None):
-            # set typed array type of input_ids to int
-            return str(js.detokenize_gpt(to_js([int(i) for i in input_ids])))
-
-        def __call__(self, s: str, add_special_tokens=False):
-            unpack = False
-            if type(s) is not list:
-                s = [s]
-                unpack = True
-            input_ids = [[int(v) for v in js.tokenize_gpt(se)] for se in s]
-            
-            if unpack:
-                return {"input_ids": input_ids[0]}
-            else:
-                return {"input_ids": input_ids}
-    
-    return JSBridgedTokenizer()
+class PythonBackedTokenizer:
+    """ Custom tokenizer to be used only in a browser environment. This tokenizer only supports GPT tokenization. """
+    def __init__(self, model_identifier):
+        import gpt3_tokenizer
+        assert "gpt" in model_identifier, "PythonBackedTokenizer only supports GPT family models"
+
+        self.bos_token_id = 50256
+        self.eos_token_id = 50256
+        self._vocab = None
+
+    @property
+    def vocab_size(self):
+        return len(self.vocab)
+
+    @property
+    def vocab(self):
+        if self._vocab is None:
+            import gpt3_tokenizer
+            self._vocab = gpt3_tokenizer._entry._encoder
+        return self._vocab
+
+    def convert_tokens_to_string(self, tokens):
+        import gpt3_tokenizer
+        text_with_bytes = "".join(tokens)
+        textarr = [int(gpt3_tokenizer._entry._byte_decoder[x]) for x in list(text_with_bytes)]
+        text = bytearray(textarr).decode("utf-8")
+        return text
+
+    def tokenize(self, s):
+        if ("<|endoftext|>" in s):
+            return [50256];
+        import gpt3_tokenizer
+        unpack = False
+        if type(s) is not list:
+            s = [s]
+            unpack = True
+
+        tokens = [[gpt3_tokenizer._entry._decoder[i] for i in gpt3_tokenizer.encode(se)] for se in s]
+
+        if unpack:
+            return tokens[0]
+        else:
+            return tokens
+        
+    def decode(self, input_ids, clean_up_tokenization_spaces=None):
+        import gpt3_tokenizer
+        return gpt3_tokenizer.decode(input_ids)
+
+    def __call__(self, s: str, add_special_tokens=False):
+        import gpt3_tokenizer
+        
+
+        unpack = False
+        if type(s) is not list:
+            s = [s]
+            unpack = True
+        
+        input_ids = [gpt3_tokenizer.encode(se) if se != "<|endoftext|>" else [self.eos_token_id] for se in s]
+        
+        if unpack:
+            return {"input_ids": input_ids[0]}
+        else:
+            return {"input_ids": input_ids}
 
 global special_token_mappings
 special_token_mappings = {}
 global reverse_special_token_mappings
 reverse_special_token_mappings = {}
 
 class LMQLTokenizer:
+    INVALID_CHARACTER = "\uFFFD"
+
     def __init__(self, tokenizer_impl, model_identifier):
         self.tokenizer_impl = tokenizer_impl
         self.model_identifier = model_identifier
         self.detokenizer_cache = {}
 
         self._vocab = get_vocab(self.tokenizer_impl)
         self.vocab_range = max(self._vocab.values()) + 1
@@ -112,14 +123,16 @@
             if key in self.detokenizer_cache[n-1].keys():
                 global reverse_special_token_mappings
                 # print("secondary cache hit")
                 if input_ids[-1] >= self.vocab_size:
                     extended = self.detokenizer_cache[n-1][key] + "<" + reverse_special_token_mappings[input_ids[-1]] + "/>"
                 else:
                     extended = self.detokenizer_cache[n-1][key] + self.tokenizer_impl.decode([input_ids[-1]], clean_up_tokenization_spaces=False)
+                    if self.INVALID_CHARACTER in extended:
+                        return self.detokenizer_cache[n-1][key]
                 if not n in self.detokenizer_cache.keys():
                     self.detokenizer_cache[n] = {}
                 self.detokenizer_cache[n][str(input_ids)] = extended
                 return extended
 
         s = ""
         for chunk in self.chunk_out_by_special_ids(input_ids):
@@ -196,42 +209,45 @@
                 segments.append(self.special_token_id("lmql:" + m.group(1)))
             else:
                 segments.append("lmql:" + m.group(1))
             offset = m.end()
         segments.append(s[offset:])
         return segments
 
+def load_tokenizer_notransformers(model_identifier):
+    return PythonBackedTokenizer(model_identifier)
+
 def load_tokenizer(model_identifier):
     import os
 
-    # check environment of USE_JS_TOKENIZER
-    if "LMQL_BROWSER" in os.environ:
-        return LMQLTokenizer(get_js_tokenizer(model_identifier), model_identifier)
-
-    from transformers import AutoTokenizer
-    import torch
-
     # first try to load pickled tokenizer from cache (faster)
     import pickle
     import pathlib
 
-    cache_dir = pathlib.Path.home() / ".cache" / "lmql"
-    cache_dir.mkdir(parents=True, exist_ok=True)
     cache_identifier = model_identifier.replace("/", "-")
-    cache_path = cache_dir / f"tokenizer-{cache_identifier}.pkl"
+    cache_path = f"tokenizer-{cache_identifier}.pkl"
 
-    if cache_path.exists():
-        with open(cache_path, "rb") as f:
-            return LMQLTokenizer(pickle.load(f), model_identifier)
-    else:
+    try:
+        import torch
         from transformers import AutoTokenizer
-        t = AutoTokenizer.from_pretrained(model_identifier)
-        with open(cache_path, "wb") as f:
-            pickle.dump(t, f)
-        return LMQLTokenizer(t, model_identifier)
+
+        if cache_file_exists(cache_path):
+            with cachefile(cache_path, "rb") as f:
+                return LMQLTokenizer(pickle.load(f), model_identifier)
+        else:
+            t = AutoTokenizer.from_pretrained(model_identifier)
+
+            with cachefile(cache_path, "wb") as f:
+                pickle.dump(t, f)
+    except Exception as e:
+        # print("info: trying to use python-based tokenizer as 'transformers' is not available")
+        # fallback to non-transformers tokenizer
+        t = load_tokenizer_notransformers(model_identifier)
+
+    return LMQLTokenizer(t, model_identifier)
 
 def get_vocab(tokenizer):
     if hasattr(tokenizer, "vocab"):
         return tokenizer.vocab
     elif hasattr(tokenizer, "get_vocab"):
         return tokenizer.get_vocab()
     elif hasattr(tokenizer, "tokenizer_impl"):
```

### Comparing `lmql-0.0.6.1/src/lmql/tests/expr_test_utils.py` & `lmql-0.0.6.2/src/lmql/tests/expr_test_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import sys
 import ast
+import asyncio
 import types
 import astunparse
 import inspect
 import termcolor
 from lmql.language.fragment_parser import LMQLQuery
 from lmql.language.compiler import PromptScope, SNFList, WhereClauseTransformation
 from lmql.ops.ops import NextToken, digest
 from lmql.runtime.program_state import ProgramState
+from lmql.runtime.lmql_runtime import LMQLQueryFunction
 
 
 global show_transformed
 show_transformed = False
 
 SEQ = "<SEQ placeholder>"
 
@@ -44,15 +46,15 @@
             program_variables.set(variable_name, text, "inc")
 
             # follow context
             follow_program_variables = program_variables.copy()
             follow_program_variables.set(variable_name, text + NextToken, "inc")
 
             # digest token with where expr
-            result, is_final, trace = digest(self.node,
+            result, is_final, trace, follow_trace = digest(self.node,
                 context=program_variables,
                 follow_context=follow_program_variables
             )
 
             if type(result) is list: 
                 result = tuple(result)
             
@@ -91,15 +93,15 @@
                 call = self.visit(node.value)
                 snf = SNFList()
                 
                 direct_result = self.expr_compiler.transform_node(call.args[0], snf)
                 value = ast.Name(snf.last_var()) if snf.var_counter > 0 else ast.parse(direct_result.strip())
 
                 return ast.copy_location(ast.Expr([
-                    ast.parse("import lmql.runtime.lmql_runtime as lmql"),
+                    # ast.parse("import lmql.runtime.lmql_runtime as lmql"),
                     snf.ast(),
                     ast.Assign(
                         node.targets, 
                         ast.Call(ast.Name("LMQLExpr"), [value], [])
                     )
                 ]), node)
         
@@ -139,25 +141,39 @@
 
 def dec(v):
     return (v, "dec")
 
 def run_all_tests(g):
     g = g.copy()
     num_errors = 0
+    loop = asyncio.get_event_loop()
+
     for k in list(g.keys()):
         try:
             if k.startswith("test"): 
                 print("Running", k, "." * (40 - len(k)), end=" ")
-                g[k]()
+                
+                if type(g[k]) is LMQLQueryFunction:
+                    loop.run_until_complete(g[k]())
+                elif inspect.iscoroutinefunction(g[k]):
+                    loop.run_until_complete(g[k]())
+                else:
+                    g[k]()
                 termcolor.cprint("OK", "green")
         except AssertionError as e:
             print(e)
             num_errors += 1
             termcolor.cprint("FAILED", "red")
-    
+
+    # wait for all tasks to finish
+    try:
+        loop.close()
+    except RuntimeError:
+        pass
+
     if num_errors != 0: 
         print(num_errors, "test(s) failed.")
         sys.exit(1)
     else: 
         print("All tests passed.")
         sys.exit(0)
```

### Comparing `lmql-0.0.6.1/src/lmql/tests/outdated/mask_product_test.py` & `lmql-0.0.6.2/src/lmql/tests/outdated/mask_product_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/tests/outdated/monotonicity.py` & `lmql-0.0.6.2/src/lmql/tests/outdated/monotonicity.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/tests/outdated/one_of_tests.py` & `lmql-0.0.6.2/src/lmql/tests/outdated/one_of_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/tests/outdated/sentences_op.py` & `lmql-0.0.6.2/src/lmql/tests/outdated/sentences_op.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/tests/outdated/starts_with_op_test.py` & `lmql-0.0.6.2/src/lmql/tests/outdated/starts_with_op_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/tests/outdated/stops_at.py` & `lmql-0.0.6.2/src/lmql/tests/outdated/stops_at.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/tests/outdated/str_in_str_tests.py` & `lmql-0.0.6.2/src/lmql/tests/outdated/str_in_str_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/tests/outdated/test_multi_head.py` & `lmql-0.0.6.2/src/lmql/tests/outdated/test_multi_head.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/tests/outdated/token_set_test.py` & `lmql-0.0.6.2/src/lmql/tests/outdated/token_set_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/tests/system/basic_use_cases.py` & `lmql-0.0.6.2/src/lmql/tests/system/basic_use_cases.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/tests/tail_token_set.py` & `lmql-0.0.6.2/src/lmql/tests/tail_token_set.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/tests/test_back2back_caching.py` & `lmql-0.0.6.2/src/lmql/tests/test_back2back_caching.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/tests/test_sample_queries.py` & `lmql-0.0.6.2/src/lmql/tests/test_sample_queries.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/live/live.js` & `lmql-0.0.6.2/src/lmql/ui/live/live.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/live/live.py` & `lmql-0.0.6.2/src/lmql/ui/live/live.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         
         def node_data(op):
             follow_map = "<follow_map output not supported>"
 
             result = "-"
             if trace is not None and op in trace:
                 result = trace[op]
-            
+
             return {
                 "result": result,
                 "follow_map": follow_map,
                 "repr": repr(op)
             }
 
         writer = CytoscapeGraphWriter(extra_data_provider=node_data)
```

### Comparing `lmql-0.0.6.1/src/lmql/ui/live/livelib.py` & `lmql-0.0.6.2/src/lmql/ui/live/livelib.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/live/yarn.lock` & `lmql-0.0.6.2/src/lmql/ui/live/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/README.md` & `lmql-0.0.6.2/src/lmql/ui/playground/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/package.json` & `lmql-0.0.6.2/src/lmql/ui/playground/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/public/favicon.ico` & `lmql-0.0.6.2/src/lmql/ui/playground/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/public/index.html` & `lmql-0.0.6.2/src/lmql/ui/playground/public/index.html`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/public/lmql.svg` & `lmql-0.0.6.2/src/lmql/ui/playground/public/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/calc.json` & `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/calc.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/chat.json` & `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/chat.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/cot.json` & `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/cot.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/distribution.json` & `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/distribution.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/hello.json` & `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/hello.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/joke.json` & `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/joke.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/kv.json` & `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/kv.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/list.json` & `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/list.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/meta.json` & `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/meta.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/translation.json` & `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/translation.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/wiki.json` & `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/wiki.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/public/snippets/dynamic-cfg.json` & `lmql-0.0.6.2/src/lmql/ui/playground/public/snippets/dynamic-cfg.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/public/snippets/json-parsing.json` & `lmql-0.0.6.2/src/lmql/ui/playground/public/snippets/json-parsing.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/App.jsx` & `lmql-0.0.6.2/src/lmql/ui/playground/src/App.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/CodeScreenshot.jsx` & `lmql-0.0.6.2/src/lmql/ui/playground/src/CodeScreenshot.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/Configuration.js` & `lmql-0.0.6.2/src/lmql/ui/playground/src/Configuration.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/DataListView.js` & `lmql-0.0.6.2/src/lmql/ui/playground/src/DataListView.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/DecoderGraph.js` & `lmql-0.0.6.2/src/lmql/ui/playground/src/DecoderGraph.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/Explore.jsx` & `lmql-0.0.6.2/src/lmql/ui/playground/src/Explore.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/SharedState.js` & `lmql-0.0.6.2/src/lmql/ui/playground/src/SharedState.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/ValidationGraph.jsx` & `lmql-0.0.6.2/src/lmql/ui/playground/src/ValidationGraph.jsx`

 * *Files 2% similar despite different names*

```diff
@@ -187,14 +187,16 @@
                       n.data.color = "rgb(113, 42, 42)"
                   } else if (value == false) {
                       n.data.color = "rgb(119, 90, 79)"
                   } else if (final == "fin" && value == true) {
                       n.data.color = "rgb(38, 87, 38)"
                   } else if (value == true) {
                       n.data.color = "rgb(58, 88, 58)"
+                  } else if (final == "stopped") {
+                      n.data.color = "rgb(134, 79, 142)"
                   } else {
                       n.data.color = "rgb(64, 61, 61)"
                   }
                   cy.add({group: "nodes", ...n})
               })
               props.graph.edges.forEach(e => {
                   cy.add({group: "edges", ...e})
```

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/browser_process.js` & `lmql-0.0.6.2/src/lmql/ui/playground/src/browser_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/build_info.js` & `lmql-0.0.6.2/src/lmql/ui/playground/src/build_info.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/editor/lmql-monaco-language.js` & `lmql-0.0.6.2/src/lmql/ui/playground/src/editor/lmql-monaco-language.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/editor/theme.json` & `lmql-0.0.6.2/src/lmql/ui/playground/src/editor/theme.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/explore.svg` & `lmql-0.0.6.2/src/lmql/ui/playground/src/explore.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/graph-layout.css` & `lmql-0.0.6.2/src/lmql/ui/playground/src/graph-layout.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/index.css` & `lmql-0.0.6.2/src/lmql/ui/playground/src/index.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/logo.svg` & `lmql-0.0.6.2/src/lmql/ui/playground/src/logo.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/queries.js` & `lmql-0.0.6.2/src/lmql/ui/playground/src/queries.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/remote_process.js` & `lmql-0.0.6.2/src/lmql/ui/playground/src/remote_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/screenshot.css` & `lmql-0.0.6.2/src/lmql/ui/playground/src/screenshot.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/spinner.svg` & `lmql-0.0.6.2/src/lmql/ui/playground/src/spinner.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/src/tagged-model-result.js` & `lmql-0.0.6.2/src/lmql/ui/playground/src/tagged-model-result.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/playground/yarn.lock` & `lmql-0.0.6.2/src/lmql/ui/playground/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/vscode/.vscode/launch.json` & `lmql-0.0.6.2/src/lmql/ui/vscode/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/vscode/LICENSE` & `lmql-0.0.6.2/src/lmql/ui/vscode/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/vscode/language-configuration.json` & `lmql-0.0.6.2/src/lmql/ui/vscode/language-configuration.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/vscode/lmql-vscode.png` & `lmql-0.0.6.2/src/lmql/ui/vscode/lmql-vscode.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/vscode/package.json` & `lmql-0.0.6.2/src/lmql/ui/vscode/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/vscode/syntaxes/lmql.qstring.json` & `lmql-0.0.6.2/src/lmql/ui/vscode/syntaxes/lmql.qstring.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json` & `lmql-0.0.6.2/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/ui/vscode/syntaxes/pylmql.json` & `lmql-0.0.6.2/src/lmql/ui/vscode/syntaxes/pylmql.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/utils/docstring_parser.py` & `lmql-0.0.6.2/src/lmql/utils/docstring_parser.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql/utils/graph.py` & `lmql-0.0.6.2/src/lmql/utils/graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,15 @@
 import io
-
-import pydot
 import os
+from dataclasses import dataclass
 
 from lmql.ops.ops import Node
 
-def show(pydot_graph):
-    # png_str = pydot_graph.create_png(prog=['dot','-Gsize=70,70!'])
-
-    # # treat the DOT output as an image file
-    # sio = io.BytesIO()
-    # sio.write(png_str)
-    # sio.seek(0)
-    # img = mpimg.imread(sio)
-
-    # # plot the image
-    # imgplot = plt.imshow(img, aspect='equal')
-    # plt.show()
-
-    pydot_graph.write_png("out.png", prog=['dot','-Gsize=70,70!'])
-    pydot_graph.write_dot('test.dot')
-    # os.system("open out.png")
-
 class GraphWriter:
     def __init__(self, name=None, type=None, extra_data_provider=None):
-        self.graph = pydot.Dot(name if name is not None else "graphwriter_graph", graph_type='graph')
-        
         if type is not None: self.graph.set_type(type)
         
         self.node_names = {}
         self.name_counter = 0 
 
         self.extra_data_provider = extra_data_provider
 
@@ -96,27 +76,32 @@
                 n[0].set_label(label)
             return n[0]
         else:
             name = f"n{self.name_counter}"
             self.name_counter += 1
             self.node_names[obj] = name
 
-        n = pydot.Node(name, label=label, shape="box", **kwargs, cyto_data=cyto_data)
+        n = {
+            "name": name, 
+            "label": label, 
+            **kwargs, 
+            "cyto_data": cyto_data
+        }
         self.graph.add_node(n)
 
         return name
 
     def edge(self, src, dst):
         n1 = self.node(src)
         n2 = self.node(dst)
 
-        self.graph.add_edge(pydot.Edge(n1, n2))
-
-    def show(self):
-        show(self.graph)
+        self.graph.add_edge({
+            "src": n1,
+            "dst": n2
+        })
 
 class CytoscapeNode:
     def __init__(self, node, graph):
         self.node = node
         self.graph = graph
 
     def set_label(self, l):
@@ -136,36 +121,43 @@
             "edges": self.edges
         }
 
         if return_dict: return d
         else: return json.dumps(d)
 
     def add_node(self, node_data, label=None):
-        node = node_data.obj_dict["name"]
-        if label is None and "label" in node_data.obj_dict["attributes"]:
-            label = node_data.obj_dict["attributes"]["label"]
+        # {
+        #     "name": name, 
+        #     "label": label, 
+        #     **kwargs, 
+        #     "cyto_data": cyto_data
+        # }
+
+        node = node_data["name"]
+        if label is None and "label" in node_data.keys():
+            label = node_data["label"]
         if label is None and node in self.nodes.keys():
             label = self.nodes[node]["data"]["label"]
 
         self.nodes[node] = {
             "data": { 
                 "id": node,
                 "label": label,
                 "is_token": 1 if "SequenceOp" in label else 0
             }
         }
 
-        if "cyto_data" in node_data.obj_dict["attributes"]:
-            self.nodes[node]["data"].update(node_data.obj_dict["attributes"]["cyto_data"])
+        if "cyto_data" in node_data.keys():
+            self.nodes[node]["data"].update(node_data["cyto_data"])
 
     def get_node(self, node):
         return [CytoscapeNode(node, self)] if node in self.nodes else []
 
     def add_edge(self, edge):
-        src, dst = edge.obj_dict["points"]
+        src, dst = edge["src"], edge["dst"]
         if type(src) is CytoscapeNode: src = src.node
         if type(dst) is CytoscapeNode: dst = dst.node
 
         self.edges.append({ "data": { "source": src, "target": dst } })
 
 
 class CytoscapeGraphWriter(GraphWriter):
```

### Comparing `lmql-0.0.6.1/src/lmql/utils/nputil.py` & `lmql-0.0.6.2/src/lmql/utils/nputil.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.1/src/lmql.egg-info/PKG-INFO` & `lmql-0.0.6.2/src/lmql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.0.6.1
+Version: 0.0.6.2
 Summary: A query language for language models.
 Home-page: https://lmql.ai
 Author: Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 Author-email: hello@lmql.ai
 Project-URL: Docs, https://docs.lmql.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: hf
 License-File: LICENSE
 
 <div align="center">
   <a href="https://lmql.ai">
     <img src="https://raw.githubusercontent.com/eth-sri/lmql/web/lmql.svg" alt="Logo" width="80" height="80">
   </a>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: lmql Version: 0.0.6.1 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.0.6.2 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
-Type: text/markdown License-File: LICENSE
+Type: text/markdown Provides-Extra: hf License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
           A query language for programming (large) language models.
                                Documentation_Â»
 
                Explore_Examples Â· Playground_IDE Â· Report_Bug
```

### Comparing `lmql-0.0.6.1/src/lmql.egg-info/SOURCES.txt` & `lmql-0.0.6.2/src/lmql.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 docs/source/quickstart.md
 docs/source/_ext/lmql_snippets.py
 docs/source/_static/css/lmql-docs.css
 docs/source/_static/images/lmql.svg
 docs/source/_static/js/lmql-playground.js
 docs/source/_templates/layout.html
 docs/source/blog/release-0.0.5.md
+docs/source/blog/release-0.0.6.1.md
 docs/source/blog/release-0.0.6.md
 docs/source/language/constraints.md
 docs/source/language/decoders.md
 docs/source/language/functions.md
 docs/source/language/models.md
 docs/source/language/overview.md
 docs/source/language/scripted_prompts.md
@@ -74,14 +75,15 @@
 src/lmql/ops/ops.py
 src/lmql/ops/token_set.py
 src/lmql/output/__init__.py
 src/lmql/output/http.py
 src/lmql/output/sse.py
 src/lmql/output/ws.py
 src/lmql/runtime/__init__.py
+src/lmql/runtime/caching.py
 src/lmql/runtime/hf_integration.py
 src/lmql/runtime/interpreter.py
 src/lmql/runtime/interrupt.py
 src/lmql/runtime/langchain.py
 src/lmql/runtime/lmql_runtime.py
 src/lmql/runtime/maiohttp.py
 src/lmql/runtime/masks.py
@@ -106,17 +108,22 @@
 src/lmql/runtime/dclib/decoders.py
 src/lmql/runtime/dclib/trie_cache.py
 src/lmql/runtime/postprocessing/__init__.py
 src/lmql/runtime/postprocessing/conditional_prob.py
 src/lmql/runtime/postprocessing/group_by.py
 src/lmql/tests/README.md
 src/lmql/tests/expr_test_utils.py
+src/lmql/tests/fin_and.py
 src/lmql/tests/tail_token_set.py
 src/lmql/tests/test_back2back_caching.py
+src/lmql/tests/test_eq.py
+src/lmql/tests/test_orop.py
 src/lmql/tests/test_sample_queries.py
+src/lmql/tests/test_scoping.py
+src/lmql/tests/test_stopping.py
 src/lmql/tests/outdated/mask_product_test.py
 src/lmql/tests/outdated/monotonicity.py
 src/lmql/tests/outdated/one_of_tests.py
 src/lmql/tests/outdated/sentences_op.py
 src/lmql/tests/outdated/starts_with_op_test.py
 src/lmql/tests/outdated/stops_at.py
 src/lmql/tests/outdated/str_in_str_tests.py
```

### Comparing `lmql-0.0.6.1/src/lmql.svg` & `lmql-0.0.6.2/src/lmql.svg`

 * *Files identical despite different names*

