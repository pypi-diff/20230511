# Comparing `tmp/lmql-0.0.6.2.tar.gz` & `tmp/lmql-0.0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmql-0.0.6.2.tar", last modified: Thu May 11 15:00:40 2023, max compression
+gzip compressed data, was "lmql-0.0.6.3.tar", last modified: Thu May 11 15:59:16 2023, max compression
```

## Comparing `lmql-0.0.6.2.tar` & `lmql-0.0.6.3.tar`

### file list

```diff
@@ -1,256 +1,257 @@
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.332651 lmql-0.0.6.2/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.308651 lmql-0.0.6.2/.github/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/.github/workflows/
--rw-rw-r--   0 luca      (1000) luca      (1000)     2285 2023-05-09 13:19:22.000000 lmql-0.0.6.2/.github/workflows/lmql-web.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)     2743 2023-05-01 11:40:25.000000 lmql-0.0.6.2/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.6.2/LICENSE
--rw-rw-r--   0 luca      (1000) luca      (1000)      140 2023-04-17 14:44:31.000000 lmql-0.0.6.2/MANIFEST.in
--rw-rw-r--   0 luca      (1000) luca      (1000)     4988 2023-05-11 15:00:40.332651 lmql-0.0.6.2/PKG-INFO
--rw-rw-r--   0 luca      (1000) luca      (1000)     4538 2023-05-03 11:12:24.000000 lmql-0.0.6.2/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)       75 2023-04-17 14:44:31.000000 lmql-0.0.6.2/TODO.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/
--rw-rw-r--   0 luca      (1000) luca      (1000)      638 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/Makefile
--rw-rw-r--   0 luca      (1000) luca      (1000)      444 2023-03-14 15:27:49.000000 lmql-0.0.6.2/docs/RELEASE.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      799 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/make.bat
--rw-rw-r--   0 luca      (1000) luca      (1000)       81 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/requirements.txt
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/source/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/source/_ext/
--rw-rw-r--   0 luca      (1000) luca      (1000)     5526 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/_ext/lmql_snippets.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.308651 lmql-0.0.6.2/docs/source/_static/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/source/_static/css/
--rw-rw-r--   0 luca      (1000) luca      (1000)     5883 2023-04-20 08:07:08.000000 lmql-0.0.6.2/docs/source/_static/css/lmql-docs.css
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/source/_static/images/
--rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/_static/images/lmql.svg
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/source/_static/js/
--rw-rw-r--   0 luca      (1000) luca      (1000)     2191 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/_static/js/lmql-playground.js
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/source/_templates/
--rw-rw-r--   0 luca      (1000) luca      (1000)      292 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/_templates/layout.html
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/source/blog/
--rw-rw-r--   0 luca      (1000) luca      (1000)     4591 2023-05-01 11:40:25.000000 lmql-0.0.6.2/docs/source/blog/release-0.0.5.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     1444 2023-05-04 19:03:37.000000 lmql-0.0.6.2/docs/source/blog/release-0.0.6.1.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     8976 2023-05-01 11:40:25.000000 lmql-0.0.6.2/docs/source/blog/release-0.0.6.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     1167 2023-04-17 14:48:56.000000 lmql-0.0.6.2/docs/source/conf.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1293 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/dev-setup.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     2780 2023-05-02 15:32:22.000000 lmql-0.0.6.2/docs/source/index.rst
--rw-rw-r--   0 luca      (1000) luca      (1000)     2484 2023-04-18 06:55:18.000000 lmql-0.0.6.2/docs/source/installation.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/source/language/
--rw-rw-r--   0 luca      (1000) luca      (1000)     7435 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/language/constraints.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     4067 2023-04-17 14:48:56.000000 lmql-0.0.6.2/docs/source/language/decoders.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     7850 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/language/functions.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     8252 2023-05-02 15:32:22.000000 lmql-0.0.6.2/docs/source/language/models.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     8507 2023-04-18 06:55:18.000000 lmql-0.0.6.2/docs/source/language/overview.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     3676 2023-04-18 06:55:18.000000 lmql-0.0.6.2/docs/source/language/scripted_prompts.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/lmql.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)    28444 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/logo.png
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/source/python/
--rw-rw-r--   0 luca      (1000) luca      (1000)       11 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/python/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    10831 2023-04-18 06:55:18.000000 lmql-0.0.6.2/docs/source/python/langchain.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     6681 2023-04-30 16:34:02.000000 lmql-0.0.6.2/docs/source/python/llama_index.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)    75148 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/python/lmql.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)     7458 2023-05-02 15:32:22.000000 lmql-0.0.6.2/docs/source/python/output.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     9592 2023-04-20 08:07:08.000000 lmql-0.0.6.2/docs/source/python/pandas.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     8847 2023-04-19 15:28:18.000000 lmql-0.0.6.2/docs/source/python/python.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     3135 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/source/quickstart.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/docs/source/releases/
--rw-rw-r--   0 luca      (1000) luca      (1000)     2263 2023-05-02 15:32:22.000000 lmql-0.0.6.2/docs/source/releases/misc-snippets.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      321 2023-04-17 14:48:56.000000 lmql-0.0.6.2/docs/source/releases/release-0.0.5.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      257 2023-04-17 14:44:31.000000 lmql-0.0.6.2/docs/todo.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      137 2023-03-14 15:27:49.000000 lmql-0.0.6.2/pyproject.toml
--rw-rw-r--   0 luca      (1000) luca      (1000)       74 2023-05-10 09:23:13.000000 lmql-0.0.6.2/requirements.txt
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.312651 lmql-0.0.6.2/scripts/
--rw-rw-r--   0 luca      (1000) luca      (1000)      295 2023-04-17 14:44:31.000000 lmql-0.0.6.2/scripts/activate-dev.sh
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.316651 lmql-0.0.6.2/scripts/conda/
--rw-rw-r--   0 luca      (1000) luca      (1000)      198 2023-05-10 09:22:47.000000 lmql-0.0.6.2/scripts/conda/requirements-no-gpu.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)      332 2023-05-10 09:22:44.000000 lmql-0.0.6.2/scripts/conda/requirements.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)      486 2023-03-14 15:27:49.000000 lmql-0.0.6.2/scripts/pypi-release.sh
--rw-rw-r--   0 luca      (1000) luca      (1000)      817 2023-03-14 15:27:49.000000 lmql-0.0.6.2/scripts/wheel.sh
--rw-rw-r--   0 luca      (1000) luca      (1000)      866 2023-05-11 15:00:40.332651 lmql-0.0.6.2/setup.cfg
--rw-rw-r--   0 luca      (1000) luca      (1000)       37 2023-05-10 14:35:25.000000 lmql-0.0.6.2/setup.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.316651 lmql-0.0.6.2/src/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.316651 lmql-0.0.6.2/src/lmql/
--rw-rw-r--   0 luca      (1000) luca      (1000)     6208 2023-05-09 13:19:22.000000 lmql-0.0.6.2/src/lmql/__init__.py
--rwxrwxr-x   0 luca      (1000) luca      (1000)     8142 2023-05-04 19:03:37.000000 lmql-0.0.6.2/src/lmql/cli.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1577 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/demo.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1531 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/http.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.316651 lmql-0.0.6.2/src/lmql/language/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/language/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    24147 2023-05-09 13:19:22.000000 lmql-0.0.6.2/src/lmql/language/compiler.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    10194 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/language/fragment_parser.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      979 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/language/qstrings.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1804 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/language/validator.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.316651 lmql-0.0.6.2/src/lmql/model/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/model/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    24468 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/model/async_generation_utils.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1299 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/model/local_client.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    18118 2023-05-10 08:09:52.000000 lmql-0.0.6.2/src/lmql/model/serve.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     8052 2023-05-02 15:48:30.000000 lmql-0.0.6.2/src/lmql/model/served_model.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.316651 lmql-0.0.6.2/src/lmql/ops/
--rw-rw-r--   0 luca      (1000) luca      (1000)       93 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ops/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     7542 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/ops/follow_map.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    41664 2023-05-09 13:19:22.000000 lmql-0.0.6.2/src/lmql/ops/ops.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    20831 2023-05-10 08:09:02.000000 lmql-0.0.6.2/src/lmql/ops/token_set.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.316651 lmql-0.0.6.2/src/lmql/output/
--rw-rw-r--   0 luca      (1000) luca      (1000)       57 2023-05-02 15:32:22.000000 lmql-0.0.6.2/src/lmql/output/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2334 2023-05-10 08:08:53.000000 lmql-0.0.6.2/src/lmql/output/http.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1889 2023-05-02 15:32:22.000000 lmql-0.0.6.2/src/lmql/output/sse.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2282 2023-05-02 15:32:22.000000 lmql-0.0.6.2/src/lmql/output/ws.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.316651 lmql-0.0.6.2/src/lmql/runtime/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/runtime/__init__.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.320651 lmql-0.0.6.2/src/lmql/runtime/bopenai/
--rw-rw-r--   0 luca      (1000) luca      (1000)     2236 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/runtime/bopenai/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    28384 2023-05-03 14:14:45.000000 lmql-0.0.6.2/src/lmql/runtime/bopenai/batched_openai.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    17221 2023-05-03 11:12:24.000000 lmql-0.0.6.2/src/lmql/runtime/bopenai/openai_api.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1906 2023-05-10 08:09:02.000000 lmql-0.0.6.2/src/lmql/runtime/caching.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.320651 lmql-0.0.6.2/src/lmql/runtime/dclib/
--rw-rw-r--   0 luca      (1000) luca      (1000)      494 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/runtime/dclib/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    18631 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_array.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    27728 2023-05-10 08:08:53.000000 lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_cache.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      538 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_global.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    21721 2023-05-02 16:00:00.000000 lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_model.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     8589 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_rewrite.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    30560 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_seq.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    20827 2023-05-04 19:03:37.000000 lmql-0.0.6.2/src/lmql/runtime/dclib/decoders.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4144 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/runtime/dclib/trie_cache.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3176 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/runtime/hf_integration.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    34822 2023-05-04 19:03:37.000000 lmql-0.0.6.2/src/lmql/runtime/interpreter.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      250 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/runtime/interrupt.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1084 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/runtime/langchain.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     6367 2023-05-02 15:32:22.000000 lmql-0.0.6.2/src/lmql/runtime/lmql_runtime.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1186 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/runtime/maiohttp.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1726 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/runtime/masks.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      732 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/runtime/model_registry.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     5835 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/runtime/multi_head_interpretation.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    42592 2023-05-03 11:12:24.000000 lmql-0.0.6.2/src/lmql/runtime/openai_integration.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1971 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/runtime/openai_secret.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4042 2023-05-02 15:32:22.000000 lmql-0.0.6.2/src/lmql/runtime/output_writer.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.320651 lmql-0.0.6.2/src/lmql/runtime/postprocessing/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/runtime/postprocessing/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3530 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/runtime/postprocessing/conditional_prob.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      152 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/runtime/postprocessing/group_by.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1980 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/runtime/program_state.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1317 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/runtime/stats.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     9778 2023-05-10 08:24:41.000000 lmql-0.0.6.2/src/lmql/runtime/tokenizer.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.320651 lmql-0.0.6.2/src/lmql/tests/
--rw-rw-r--   0 luca      (1000) luca      (1000)      319 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/tests/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     5667 2023-05-04 19:03:37.000000 lmql-0.0.6.2/src/lmql/tests/expr_test_utils.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1314 2023-05-04 19:03:37.000000 lmql-0.0.6.2/src/lmql/tests/fin_and.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.320651 lmql-0.0.6.2/src/lmql/tests/outdated/
--rw-rw-r--   0 luca      (1000) luca      (1000)     1611 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/outdated/mask_product_test.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2789 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/outdated/monotonicity.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      546 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/outdated/one_of_tests.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      758 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/outdated/sentences_op.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      984 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/outdated/starts_with_op_test.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1236 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/outdated/stops_at.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      537 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/outdated/str_in_str_tests.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4738 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/outdated/test_multi_head.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3036 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/outdated/token_set_test.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.320651 lmql-0.0.6.2/src/lmql/tests/system/
--rw-rw-r--   0 luca      (1000) luca      (1000)     3402 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/tests/system/basic_use_cases.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      971 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/tail_token_set.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      788 2023-05-02 15:32:22.000000 lmql-0.0.6.2/src/lmql/tests/test_back2back_caching.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2382 2023-05-09 13:19:22.000000 lmql-0.0.6.2/src/lmql/tests/test_eq.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      457 2023-05-04 19:03:37.000000 lmql-0.0.6.2/src/lmql/tests/test_orop.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2481 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/tests/test_sample_queries.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1720 2023-05-09 13:19:22.000000 lmql-0.0.6.2/src/lmql/tests/test_scoping.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3572 2023-05-09 13:19:22.000000 lmql-0.0.6.2/src/lmql/tests/test_stopping.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.320651 lmql-0.0.6.2/src/lmql/ui/
--rw-rw-r--   0 luca      (1000) luca      (1000)       27 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/__init__.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.320651 lmql-0.0.6.2/src/lmql/ui/live/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/live/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     6747 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/live/live.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     3334 2023-05-04 19:03:37.000000 lmql-0.0.6.2/src/lmql/ui/live/live.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3885 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/live/livelib.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      349 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/live/package.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    33701 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/live/yarn.lock
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.324651 lmql-0.0.6.2/src/lmql/ui/playground/
--rw-rw-r--   0 luca      (1000) luca      (1000)       31 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/.dockerignore
--rw-rw-r--   0 luca      (1000) luca      (1000)       34 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/.env
--rw-rw-r--   0 luca      (1000) luca      (1000)      310 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)      354 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/Dockerfile
--rw-rw-r--   0 luca      (1000) luca      (1000)     3359 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     1327 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/package.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.324651 lmql-0.0.6.2/src/lmql/ui/playground/public/
--rw-rw-r--   0 luca      (1000) luca      (1000)       90 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/_headers
--rw-rw-r--   0 luca      (1000) luca      (1000)     3870 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/favicon.ico
--rw-rw-r--   0 luca      (1000) luca      (1000)     1678 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/index.html
--rw-rw-r--   0 luca      (1000) luca      (1000)     2817 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/lmql.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)      306 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/manifest.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.328651 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/
--rw-rw-r--   0 luca      (1000) luca      (1000)  1227728 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/calc.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   295285 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/chat.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   160153 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/cot.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    81768 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/distribution.json
--rw-rw-r--   0 luca      (1000) luca      (1000)     5221 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/hello.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    89531 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/joke.json
--rw-rw-r--   0 luca      (1000) luca      (1000)  1710847 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/kv.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    52748 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/list.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   628184 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/meta.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   264768 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/translation.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   215050 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/wiki.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       67 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/robots.txt
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.328651 lmql-0.0.6.2/src/lmql/ui/playground/public/snippets/
--rw-rw-r--   0 luca      (1000) luca      (1000)   381736 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   184008 2023-05-02 15:32:22.000000 lmql-0.0.6.2/src/lmql/ui/playground/public/snippets/json-parsing.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       62 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/ref.py
--rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/run-in-docker.sh
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.332651 lmql-0.0.6.2/src/lmql/ui/playground/src/
--rw-rw-r--   0 luca      (1000) luca      (1000)    69135 2023-05-03 14:14:45.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/App.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      246 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/App.test.js
--rw-rw-r--   0 luca      (1000) luca      (1000)    29983 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/CodeScreenshot.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      807 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/Configuration.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     1174 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/DataListView.js
--rw-rw-r--   0 luca      (1000) luca      (1000)    21319 2023-05-03 11:12:24.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/DecoderGraph.js
--rw-rw-r--   0 luca      (1000) luca      (1000)      329 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/DecodingTree.js
--rw-rw-r--   0 luca      (1000) luca      (1000)       89 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/Embed.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)     9601 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/Explore.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      675 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/SharedState.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     4819 2023-05-04 19:03:37.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/State.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     5871 2023-05-04 19:03:37.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/ValidationGraph.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)     9360 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/browser_process.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     1163 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/build_info.js
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.332651 lmql-0.0.6.2/src/lmql/ui/playground/src/editor/
--rw-rw-r--   0 luca      (1000) luca      (1000)     8696 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     4758 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/editor/theme.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      889 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/explore.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     1345 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/graph-layout.css
--rw-rw-r--   0 luca      (1000) luca      (1000)     1698 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/index.css
--rw-rw-r--   0 luca      (1000) luca      (1000)      489 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/index.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     2632 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/logo.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     8104 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/queries.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     5990 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/remote_process.js
--rw-rw-r--   0 luca      (1000) luca      (1000)      362 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/reportWebVitals.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     9520 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/screenshot.css
--rw-rw-r--   0 luca      (1000) luca      (1000)      241 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/setupTests.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     3466 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/spinner.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     2949 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/src/tagged-model-result.js
--rw-rw-r--   0 luca      (1000) luca      (1000)   449905 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/playground/yarn.lock
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.332651 lmql-0.0.6.2/src/lmql/ui/vscode/
--rw-rw-r--   0 luca      (1000) luca      (1000)       76 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/vscode/.gitattributes
--rw-rw-r--   0 luca      (1000) luca      (1000)       19 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/vscode/.gitignore
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.332651 lmql-0.0.6.2/src/lmql/ui/vscode/.vscode/
--rw-rw-r--   0 luca      (1000) luca      (1000)      540 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/vscode/.vscode/launch.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       66 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/vscode/.vscodeignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/ui/vscode/LICENSE
--rw-rw-r--   0 luca      (1000) luca      (1000)      357 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/ui/vscode/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      959 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/vscode/language-configuration.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    11532 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/ui/vscode/lmql-vscode.png
--rw-rw-r--   0 luca      (1000) luca      (1000)     1214 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql/ui/vscode/package.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.332651 lmql-0.0.6.2/src/lmql/ui/vscode/syntaxes/
--rw-rw-r--   0 luca      (1000) luca      (1000)      518 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      642 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      853 2023-04-17 14:44:31.000000 lmql-0.0.6.2/src/lmql/ui/vscode/syntaxes/pylmql.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.332651 lmql-0.0.6.2/src/lmql/utils/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.2/src/lmql/utils/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2402 2023-05-02 15:32:22.000000 lmql-0.0.6.2/src/lmql/utils/docstring_parser.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4933 2023-05-10 09:22:32.000000 lmql-0.0.6.2/src/lmql/utils/graph.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2402 2023-05-01 11:40:25.000000 lmql-0.0.6.2/src/lmql/utils/nputil.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      115 2023-05-11 15:00:35.000000 lmql-0.0.6.2/src/lmql/version.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:00:40.316651 lmql-0.0.6.2/src/lmql.egg-info/
--rw-rw-r--   0 luca      (1000) luca      (1000)     4988 2023-05-11 15:00:40.000000 lmql-0.0.6.2/src/lmql.egg-info/PKG-INFO
--rw-rw-r--   0 luca      (1000) luca      (1000)     7176 2023-05-11 15:00:40.000000 lmql-0.0.6.2/src/lmql.egg-info/SOURCES.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)        1 2023-05-11 15:00:40.000000 lmql-0.0.6.2/src/lmql.egg-info/dependency_links.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)       39 2023-05-11 15:00:40.000000 lmql-0.0.6.2/src/lmql.egg-info/entry_points.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)       94 2023-05-11 15:00:40.000000 lmql-0.0.6.2/src/lmql.egg-info/requires.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)        5 2023-05-11 15:00:40.000000 lmql-0.0.6.2/src/lmql.egg-info/top_level.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)   115785 2023-04-17 14:48:56.000000 lmql-0.0.6.2/src/lmql.svg
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.165824 lmql-0.0.6.3/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.141824 lmql-0.0.6.3/.github/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/.github/workflows/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2285 2023-05-11 15:18:25.000000 lmql-0.0.6.3/.github/workflows/lmql-web.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2743 2023-05-11 15:13:38.000000 lmql-0.0.6.3/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.6.3/LICENSE
+-rw-rw-r--   0 luca      (1000) luca      (1000)      140 2023-04-17 14:44:31.000000 lmql-0.0.6.3/MANIFEST.in
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4988 2023-05-11 15:59:16.165824 lmql-0.0.6.3/PKG-INFO
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4538 2023-05-11 15:13:38.000000 lmql-0.0.6.3/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)       75 2023-04-17 14:44:31.000000 lmql-0.0.6.3/TODO.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      638 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/Makefile
+-rw-rw-r--   0 luca      (1000) luca      (1000)      444 2023-03-14 15:27:49.000000 lmql-0.0.6.3/docs/RELEASE.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      799 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/make.bat
+-rw-rw-r--   0 luca      (1000) luca      (1000)       81 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/requirements.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/source/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/source/_ext/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5526 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/_ext/lmql_snippets.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.141824 lmql-0.0.6.3/docs/source/_static/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/source/_static/css/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5883 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/_static/css/lmql-docs.css
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/source/_static/images/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/_static/images/lmql.svg
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/source/_static/js/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2191 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/_static/js/lmql-playground.js
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/source/_templates/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      292 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/_templates/layout.html
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/source/blog/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4591 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/blog/release-0.0.5.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1444 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/blog/release-0.0.6.1.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1887 2023-05-11 15:59:04.000000 lmql-0.0.6.3/docs/source/blog/release-0.0.6.3.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8976 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/blog/release-0.0.6.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1167 2023-04-17 14:48:56.000000 lmql-0.0.6.3/docs/source/conf.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1293 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/dev-setup.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2780 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/index.rst
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2484 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/installation.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/source/language/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7435 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/language/constraints.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4067 2023-04-17 14:48:56.000000 lmql-0.0.6.3/docs/source/language/decoders.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7850 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/language/functions.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8310 2023-05-11 15:34:04.000000 lmql-0.0.6.3/docs/source/language/models.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8507 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/language/overview.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3676 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/language/scripted_prompts.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/lmql.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)    28444 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/logo.png
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/source/python/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       11 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/python/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    10831 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/python/langchain.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6681 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/python/llama_index.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)    75148 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/python/lmql.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7458 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/python/output.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9592 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/python/pandas.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8847 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/python/python.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3135 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/source/quickstart.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/docs/source/releases/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2263 2023-05-11 15:13:38.000000 lmql-0.0.6.3/docs/source/releases/misc-snippets.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      321 2023-04-17 14:48:56.000000 lmql-0.0.6.3/docs/source/releases/release-0.0.5.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      257 2023-04-17 14:44:31.000000 lmql-0.0.6.3/docs/todo.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      137 2023-03-14 15:27:49.000000 lmql-0.0.6.3/pyproject.toml
+-rw-rw-r--   0 luca      (1000) luca      (1000)       74 2023-05-11 15:26:02.000000 lmql-0.0.6.3/requirements.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/scripts/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      295 2023-04-17 14:44:31.000000 lmql-0.0.6.3/scripts/activate-dev.sh
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/scripts/conda/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      198 2023-05-11 15:26:02.000000 lmql-0.0.6.3/scripts/conda/requirements-no-gpu.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)      332 2023-05-11 15:26:02.000000 lmql-0.0.6.3/scripts/conda/requirements.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)      486 2023-03-14 15:27:49.000000 lmql-0.0.6.3/scripts/pypi-release.sh
+-rw-rw-r--   0 luca      (1000) luca      (1000)      817 2023-03-14 15:27:49.000000 lmql-0.0.6.3/scripts/wheel.sh
+-rw-rw-r--   0 luca      (1000) luca      (1000)      866 2023-05-11 15:59:16.165824 lmql-0.0.6.3/setup.cfg
+-rw-rw-r--   0 luca      (1000) luca      (1000)       37 2023-05-10 14:35:25.000000 lmql-0.0.6.3/setup.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.145824 lmql-0.0.6.3/src/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.149824 lmql-0.0.6.3/src/lmql/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6208 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/__init__.py
+-rwxrwxr-x   0 luca      (1000) luca      (1000)     8142 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/cli.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1577 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/demo.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1531 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/http.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.149824 lmql-0.0.6.3/src/lmql/language/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/language/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    24147 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/language/compiler.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    10194 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/language/fragment_parser.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      979 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/language/qstrings.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1804 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/language/validator.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.149824 lmql-0.0.6.3/src/lmql/model/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/model/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    24468 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/model/async_generation_utils.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1299 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/model/local_client.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    18118 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/model/serve.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8052 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/model/served_model.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.149824 lmql-0.0.6.3/src/lmql/ops/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       93 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ops/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7542 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/ops/follow_map.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    41664 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/ops/ops.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    20806 2023-05-11 15:34:49.000000 lmql-0.0.6.3/src/lmql/ops/token_set.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.149824 lmql-0.0.6.3/src/lmql/output/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       57 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/output/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2334 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/output/http.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1889 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/output/sse.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2282 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/output/ws.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.149824 lmql-0.0.6.3/src/lmql/runtime/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/runtime/__init__.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.153824 lmql-0.0.6.3/src/lmql/runtime/bopenai/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2236 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/runtime/bopenai/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    28384 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/runtime/bopenai/batched_openai.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    17221 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/runtime/bopenai/openai_api.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1906 2023-05-11 15:26:02.000000 lmql-0.0.6.3/src/lmql/runtime/caching.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.153824 lmql-0.0.6.3/src/lmql/runtime/dclib/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      494 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/runtime/dclib/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    18631 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_array.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    27728 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_cache.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      538 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_global.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    21721 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_model.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8589 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_rewrite.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    30560 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_seq.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    20827 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/runtime/dclib/decoders.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4144 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/runtime/dclib/trie_cache.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3176 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/runtime/hf_integration.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    34822 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/runtime/interpreter.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      250 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/runtime/interrupt.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1084 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/runtime/langchain.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6367 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/runtime/lmql_runtime.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1186 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/runtime/maiohttp.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1726 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/runtime/masks.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      732 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/runtime/model_registry.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5835 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/runtime/multi_head_interpretation.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    42592 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/runtime/openai_integration.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1971 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/runtime/openai_secret.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4042 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/runtime/output_writer.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.153824 lmql-0.0.6.3/src/lmql/runtime/postprocessing/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/runtime/postprocessing/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3530 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/runtime/postprocessing/conditional_prob.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      152 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/runtime/postprocessing/group_by.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1980 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/runtime/program_state.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1317 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/runtime/stats.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9778 2023-05-11 15:26:02.000000 lmql-0.0.6.3/src/lmql/runtime/tokenizer.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.153824 lmql-0.0.6.3/src/lmql/tests/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      319 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/tests/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5667 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/tests/expr_test_utils.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1314 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/fin_and.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.153824 lmql-0.0.6.3/src/lmql/tests/outdated/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1611 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/outdated/mask_product_test.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2789 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/outdated/monotonicity.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      546 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/outdated/one_of_tests.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      758 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/outdated/sentences_op.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      984 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/outdated/starts_with_op_test.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1236 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/outdated/stops_at.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      537 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/outdated/str_in_str_tests.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4738 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/outdated/test_multi_head.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3036 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/outdated/token_set_test.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.153824 lmql-0.0.6.3/src/lmql/tests/system/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3402 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/tests/system/basic_use_cases.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      971 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/tail_token_set.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      788 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/test_back2back_caching.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2382 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/test_eq.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      457 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/test_orop.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2481 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/test_sample_queries.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1720 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/test_scoping.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3572 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/tests/test_stopping.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.153824 lmql-0.0.6.3/src/lmql/ui/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       27 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/__init__.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.153824 lmql-0.0.6.3/src/lmql/ui/live/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/live/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6747 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/live/live.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3334 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/ui/live/live.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3885 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/live/livelib.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      349 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/live/package.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    33701 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/live/yarn.lock
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.157824 lmql-0.0.6.3/src/lmql/ui/playground/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       31 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/.dockerignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)       34 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/.env
+-rw-rw-r--   0 luca      (1000) luca      (1000)      310 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)      354 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/Dockerfile
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3359 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1327 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/package.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.157824 lmql-0.0.6.3/src/lmql/ui/playground/public/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       90 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/_headers
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3870 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/favicon.ico
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1678 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/index.html
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2817 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/lmql.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)      306 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/manifest.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.161824 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/
+-rw-rw-r--   0 luca      (1000) luca      (1000)  1227728 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/calc.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   295285 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/chat.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   160153 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/cot.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    81768 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/distribution.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5221 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/hello.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    89531 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/joke.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)  1710847 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/kv.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    52748 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/list.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   628184 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/meta.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   264768 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/translation.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   215050 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/wiki.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       67 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/robots.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.161824 lmql-0.0.6.3/src/lmql/ui/playground/public/snippets/
+-rw-rw-r--   0 luca      (1000) luca      (1000)   381736 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   184008 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/ui/playground/public/snippets/json-parsing.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       62 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/ref.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/run-in-docker.sh
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.165824 lmql-0.0.6.3/src/lmql/ui/playground/src/
+-rw-rw-r--   0 luca      (1000) luca      (1000)    69135 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/App.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      246 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/App.test.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)    29983 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/CodeScreenshot.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      807 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/Configuration.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1174 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/DataListView.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)    21319 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/DecoderGraph.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)      329 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/DecodingTree.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)       89 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/Embed.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9601 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/Explore.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      675 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/SharedState.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4819 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/State.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5871 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/ValidationGraph.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9360 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/browser_process.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1163 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/build_info.js
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.165824 lmql-0.0.6.3/src/lmql/ui/playground/src/editor/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8696 2023-05-11 15:18:25.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4758 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/editor/theme.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      889 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/explore.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1345 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/graph-layout.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1698 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/index.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)      489 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/index.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2632 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/logo.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8104 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/queries.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5990 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/remote_process.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)      362 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/reportWebVitals.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9520 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/screenshot.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)      241 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/setupTests.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3466 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/spinner.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2949 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/src/tagged-model-result.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)   449905 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/playground/yarn.lock
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.165824 lmql-0.0.6.3/src/lmql/ui/vscode/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       76 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/vscode/.gitattributes
+-rw-rw-r--   0 luca      (1000) luca      (1000)       19 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/vscode/.gitignore
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.165824 lmql-0.0.6.3/src/lmql/ui/vscode/.vscode/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      540 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/vscode/.vscode/launch.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       66 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/vscode/.vscodeignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/ui/vscode/LICENSE
+-rw-rw-r--   0 luca      (1000) luca      (1000)      357 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/ui/vscode/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      959 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/vscode/language-configuration.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    11532 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/ui/vscode/lmql-vscode.png
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1214 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql/ui/vscode/package.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.165824 lmql-0.0.6.3/src/lmql/ui/vscode/syntaxes/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      518 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      642 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      853 2023-04-17 14:44:31.000000 lmql-0.0.6.3/src/lmql/ui/vscode/syntaxes/pylmql.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.165824 lmql-0.0.6.3/src/lmql/utils/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.3/src/lmql/utils/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2402 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/utils/docstring_parser.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4933 2023-05-11 15:26:02.000000 lmql-0.0.6.3/src/lmql/utils/graph.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2402 2023-05-11 15:13:38.000000 lmql-0.0.6.3/src/lmql/utils/nputil.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      115 2023-05-11 15:59:11.000000 lmql-0.0.6.3/src/lmql/version.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-11 15:59:16.149824 lmql-0.0.6.3/src/lmql.egg-info/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4988 2023-05-11 15:59:15.000000 lmql-0.0.6.3/src/lmql.egg-info/PKG-INFO
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7212 2023-05-11 15:59:16.000000 lmql-0.0.6.3/src/lmql.egg-info/SOURCES.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)        1 2023-05-11 15:59:15.000000 lmql-0.0.6.3/src/lmql.egg-info/dependency_links.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)       39 2023-05-11 15:59:15.000000 lmql-0.0.6.3/src/lmql.egg-info/entry_points.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)       94 2023-05-11 15:59:15.000000 lmql-0.0.6.3/src/lmql.egg-info/requires.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)        5 2023-05-11 15:59:15.000000 lmql-0.0.6.3/src/lmql.egg-info/top_level.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)   115785 2023-04-17 14:48:56.000000 lmql-0.0.6.3/src/lmql.svg
```

### Comparing `lmql-0.0.6.2/.github/workflows/lmql-web.yml` & `lmql-0.0.6.3/.github/workflows/lmql-web.yml`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/.gitignore` & `lmql-0.0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/LICENSE` & `lmql-0.0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/PKG-INFO` & `lmql-0.0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.0.6.2
+Version: 0.0.6.3
 Summary: A query language for language models.
 Home-page: https://lmql.ai
 Author: Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 Author-email: hello@lmql.ai
 Project-URL: Docs, https://docs.lmql.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lmql Version: 0.0.6.2 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.0.6.3 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
 Type: text/markdown Provides-Extra: hf License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
```

### Comparing `lmql-0.0.6.2/README.md` & `lmql-0.0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/Makefile` & `lmql-0.0.6.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/make.bat` & `lmql-0.0.6.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/_ext/lmql_snippets.py` & `lmql-0.0.6.3/docs/source/_ext/lmql_snippets.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/_static/css/lmql-docs.css` & `lmql-0.0.6.3/docs/source/_static/css/lmql-docs.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/_static/images/lmql.svg` & `lmql-0.0.6.3/docs/source/_static/images/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/_static/js/lmql-playground.js` & `lmql-0.0.6.3/docs/source/_static/js/lmql-playground.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/blog/release-0.0.5.md` & `lmql-0.0.6.3/docs/source/blog/release-0.0.5.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/blog/release-0.0.6.1.md` & `lmql-0.0.6.3/docs/source/blog/release-0.0.6.1.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/blog/release-0.0.6.md` & `lmql-0.0.6.3/docs/source/blog/release-0.0.6.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/conf.py` & `lmql-0.0.6.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/dev-setup.md` & `lmql-0.0.6.3/docs/source/dev-setup.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/index.rst` & `lmql-0.0.6.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/installation.md` & `lmql-0.0.6.3/docs/source/installation.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/language/constraints.md` & `lmql-0.0.6.3/docs/source/language/constraints.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/language/decoders.md` & `lmql-0.0.6.3/docs/source/language/decoders.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/language/functions.md` & `lmql-0.0.6.3/docs/source/language/functions.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/language/models.md` & `lmql-0.0.6.3/docs/source/language/models.md`

 * *Files 3% similar despite different names*

```diff
@@ -94,15 +94,21 @@
 * The **OpenAI Completions API only provides the top-5 logprobs per predicted token**. This means that decoding algorithms that explore e.g. the top-n probabilities to make decisions like beam search, are limited to a branching factor of 5.
 
 * The **OpenAI Chat API does not provide any way to mask tokens or obtain the token distribution (ChatGPT, GPT-4)**. Simple constraints can still be enforced, as the LMQL runtime optimizes them to fit the OpenAI API. However, more complex constraints may not be enforceable. In these cases, LMQL will print a error message to the console. As a workaround users may then adjust their constraints to fit these API limitations or resort to post-processing and backtracking. Scripted prompting, intermediate instructions and simple constraints are still supported with Chat API models, nonetheless.
 ## 🤗 Transformers Models
 
 LMQL also support locally-hosted models via [🤗 Transformers](https://huggingface.co/transformers). This includes all models that are available via the [🤗 Transformers Model Hub](https://huggingface.co/models) and conform to the AutoModelForCausalLM API. Examples include `gpt2` or `facebook/opt-30B`.
 
-The API limitations mentioned above do not apply to locally-hosted models, as the LMQL runtime can leverage the full power of the 🤗 Transformers API and access the full token distribution, enforcing token masks of arbitrary size.
+Before you start using LMQL with 🤗 Transformers models, make sure you have installed the `lmql` package with the optional `hf` flag:
+
+```bash
+pip install lmql[hf]
+```
+
+This will install the `transformers` package and its dependencies, which is required to load 🤗  Transformers models.
 
 ### Running LMQL with 🤗 Transformers
 
 To speed-up turnaround time during query development, LMQL supports a two process architecture. One process (long-running) loads the model and provides a simple inference API, and the other process (short-lived) executes the LMQL query. This architecture is particularly useful for locally-hosted models, as the model loading time can be quite long.
 
 To start a model serving process, e.g. for the `gpt2-medium` model, run the following command:
```

### Comparing `lmql-0.0.6.2/docs/source/language/overview.md` & `lmql-0.0.6.3/docs/source/language/overview.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/language/scripted_prompts.md` & `lmql-0.0.6.3/docs/source/language/scripted_prompts.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/lmql.svg` & `lmql-0.0.6.3/docs/source/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/logo.png` & `lmql-0.0.6.3/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/python/langchain.ipynb` & `lmql-0.0.6.3/docs/source/python/langchain.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/python/llama_index.ipynb` & `lmql-0.0.6.3/docs/source/python/llama_index.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/python/lmql.txt` & `lmql-0.0.6.3/docs/source/python/lmql.txt`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/python/output.ipynb` & `lmql-0.0.6.3/docs/source/python/output.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/python/pandas.ipynb` & `lmql-0.0.6.3/docs/source/python/pandas.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/python/python.ipynb` & `lmql-0.0.6.3/docs/source/python/python.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/quickstart.md` & `lmql-0.0.6.3/docs/source/quickstart.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/docs/source/releases/misc-snippets.md` & `lmql-0.0.6.3/docs/source/releases/misc-snippets.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/scripts/wheel.sh` & `lmql-0.0.6.3/scripts/wheel.sh`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/setup.cfg` & `lmql-0.0.6.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lmql
-version = 0.0.6.2
+version = 0.0.6.3
 author = Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 author_email = hello@lmql.ai
 description = A query language for language models.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://lmql.ai
 project_urls =
```

### Comparing `lmql-0.0.6.2/src/lmql/__init__.py` & `lmql-0.0.6.3/src/lmql/__init__.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/cli.py` & `lmql-0.0.6.3/src/lmql/cli.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/demo.py` & `lmql-0.0.6.3/src/lmql/demo.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/http.py` & `lmql-0.0.6.3/src/lmql/http.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/language/compiler.py` & `lmql-0.0.6.3/src/lmql/language/compiler.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/language/fragment_parser.py` & `lmql-0.0.6.3/src/lmql/language/fragment_parser.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/language/qstrings.py` & `lmql-0.0.6.3/src/lmql/language/qstrings.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/language/validator.py` & `lmql-0.0.6.3/src/lmql/language/validator.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/model/async_generation_utils.py` & `lmql-0.0.6.3/src/lmql/model/async_generation_utils.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/model/local_client.py` & `lmql-0.0.6.3/src/lmql/model/local_client.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/model/serve.py` & `lmql-0.0.6.3/src/lmql/model/serve.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/model/served_model.py` & `lmql-0.0.6.3/src/lmql/model/served_model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ops/follow_map.py` & `lmql-0.0.6.3/src/lmql/ops/follow_map.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ops/ops.py` & `lmql-0.0.6.3/src/lmql/ops/ops.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ops/token_set.py` & `lmql-0.0.6.3/src/lmql/ops/token_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         import pickle
 
         cache_identifier = tokenizer.model_identifier.replace("/", "-")
         cache_path = f"token-mask-cache-{cache_identifier}.pkl"
         matcher_path = f"matcher-{cache_identifier}.pkl"
 
         try:
-            assert False
             with cachefile(matcher_path, "rb") as f:
                 VocabularyMatcher._instance = pickle.load(f)
                 VocabularyMatcher._instance.stats = Stats("VocabularyMatcher")
         except:
             VocabularyMatcher._instance = VocabularyMatcher(tokenizer, tokenizer.model_identifier)
 
         if cache_file_exists(cache_path) and False:
```

### Comparing `lmql-0.0.6.2/src/lmql/output/http.py` & `lmql-0.0.6.3/src/lmql/output/http.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/output/sse.py` & `lmql-0.0.6.3/src/lmql/output/sse.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/output/ws.py` & `lmql-0.0.6.3/src/lmql/output/ws.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/bopenai/__init__.py` & `lmql-0.0.6.3/src/lmql/runtime/bopenai/__init__.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/bopenai/batched_openai.py` & `lmql-0.0.6.3/src/lmql/runtime/bopenai/batched_openai.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/bopenai/openai_api.py` & `lmql-0.0.6.3/src/lmql/runtime/bopenai/openai_api.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/caching.py` & `lmql-0.0.6.3/src/lmql/runtime/caching.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_array.py` & `lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_array.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_cache.py` & `lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_cache.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_global.py` & `lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_global.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_model.py` & `lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_model.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_rewrite.py` & `lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_rewrite.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/dclib/dclib_seq.py` & `lmql-0.0.6.3/src/lmql/runtime/dclib/dclib_seq.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/dclib/decoders.py` & `lmql-0.0.6.3/src/lmql/runtime/dclib/decoders.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/dclib/trie_cache.py` & `lmql-0.0.6.3/src/lmql/runtime/dclib/trie_cache.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/hf_integration.py` & `lmql-0.0.6.3/src/lmql/runtime/hf_integration.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/interpreter.py` & `lmql-0.0.6.3/src/lmql/runtime/interpreter.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/langchain.py` & `lmql-0.0.6.3/src/lmql/runtime/langchain.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/lmql_runtime.py` & `lmql-0.0.6.3/src/lmql/runtime/lmql_runtime.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/maiohttp.py` & `lmql-0.0.6.3/src/lmql/runtime/maiohttp.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/masks.py` & `lmql-0.0.6.3/src/lmql/runtime/masks.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/model_registry.py` & `lmql-0.0.6.3/src/lmql/runtime/model_registry.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/multi_head_interpretation.py` & `lmql-0.0.6.3/src/lmql/runtime/multi_head_interpretation.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/openai_integration.py` & `lmql-0.0.6.3/src/lmql/runtime/openai_integration.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/openai_secret.py` & `lmql-0.0.6.3/src/lmql/runtime/openai_secret.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/output_writer.py` & `lmql-0.0.6.3/src/lmql/runtime/output_writer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/postprocessing/conditional_prob.py` & `lmql-0.0.6.3/src/lmql/runtime/postprocessing/conditional_prob.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/program_state.py` & `lmql-0.0.6.3/src/lmql/runtime/program_state.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/stats.py` & `lmql-0.0.6.3/src/lmql/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/runtime/tokenizer.py` & `lmql-0.0.6.3/src/lmql/runtime/tokenizer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/tests/expr_test_utils.py` & `lmql-0.0.6.3/src/lmql/tests/expr_test_utils.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/tests/fin_and.py` & `lmql-0.0.6.3/src/lmql/tests/fin_and.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/tests/outdated/mask_product_test.py` & `lmql-0.0.6.3/src/lmql/tests/outdated/mask_product_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/tests/outdated/monotonicity.py` & `lmql-0.0.6.3/src/lmql/tests/outdated/monotonicity.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/tests/outdated/one_of_tests.py` & `lmql-0.0.6.3/src/lmql/tests/outdated/one_of_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/tests/outdated/sentences_op.py` & `lmql-0.0.6.3/src/lmql/tests/outdated/sentences_op.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/tests/outdated/starts_with_op_test.py` & `lmql-0.0.6.3/src/lmql/tests/outdated/starts_with_op_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/tests/outdated/stops_at.py` & `lmql-0.0.6.3/src/lmql/tests/outdated/stops_at.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/tests/outdated/str_in_str_tests.py` & `lmql-0.0.6.3/src/lmql/tests/outdated/str_in_str_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/tests/outdated/test_multi_head.py` & `lmql-0.0.6.3/src/lmql/tests/outdated/test_multi_head.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/tests/outdated/token_set_test.py` & `lmql-0.0.6.3/src/lmql/tests/outdated/token_set_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/tests/system/basic_use_cases.py` & `lmql-0.0.6.3/src/lmql/tests/system/basic_use_cases.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/tests/tail_token_set.py` & `lmql-0.0.6.3/src/lmql/tests/tail_token_set.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/tests/test_back2back_caching.py` & `lmql-0.0.6.3/src/lmql/tests/test_back2back_caching.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/tests/test_eq.py` & `lmql-0.0.6.3/src/lmql/tests/test_eq.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/tests/test_sample_queries.py` & `lmql-0.0.6.3/src/lmql/tests/test_sample_queries.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/tests/test_scoping.py` & `lmql-0.0.6.3/src/lmql/tests/test_scoping.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/tests/test_stopping.py` & `lmql-0.0.6.3/src/lmql/tests/test_stopping.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/live/live.js` & `lmql-0.0.6.3/src/lmql/ui/live/live.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/live/live.py` & `lmql-0.0.6.3/src/lmql/ui/live/live.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/live/livelib.py` & `lmql-0.0.6.3/src/lmql/ui/live/livelib.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/live/yarn.lock` & `lmql-0.0.6.3/src/lmql/ui/live/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/README.md` & `lmql-0.0.6.3/src/lmql/ui/playground/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/package.json` & `lmql-0.0.6.3/src/lmql/ui/playground/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/public/favicon.ico` & `lmql-0.0.6.3/src/lmql/ui/playground/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/public/index.html` & `lmql-0.0.6.3/src/lmql/ui/playground/public/index.html`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/public/lmql.svg` & `lmql-0.0.6.3/src/lmql/ui/playground/public/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/calc.json` & `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/calc.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/chat.json` & `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/chat.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/cot.json` & `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/cot.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/distribution.json` & `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/distribution.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/hello.json` & `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/hello.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/joke.json` & `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/joke.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/kv.json` & `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/kv.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/list.json` & `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/list.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/meta.json` & `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/meta.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/translation.json` & `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/translation.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/public/precomputed/wiki.json` & `lmql-0.0.6.3/src/lmql/ui/playground/public/precomputed/wiki.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/public/snippets/dynamic-cfg.json` & `lmql-0.0.6.3/src/lmql/ui/playground/public/snippets/dynamic-cfg.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/public/snippets/json-parsing.json` & `lmql-0.0.6.3/src/lmql/ui/playground/public/snippets/json-parsing.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/App.jsx` & `lmql-0.0.6.3/src/lmql/ui/playground/src/App.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/CodeScreenshot.jsx` & `lmql-0.0.6.3/src/lmql/ui/playground/src/CodeScreenshot.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/Configuration.js` & `lmql-0.0.6.3/src/lmql/ui/playground/src/Configuration.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/DataListView.js` & `lmql-0.0.6.3/src/lmql/ui/playground/src/DataListView.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/DecoderGraph.js` & `lmql-0.0.6.3/src/lmql/ui/playground/src/DecoderGraph.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/Explore.jsx` & `lmql-0.0.6.3/src/lmql/ui/playground/src/Explore.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/SharedState.js` & `lmql-0.0.6.3/src/lmql/ui/playground/src/SharedState.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/State.js` & `lmql-0.0.6.3/src/lmql/ui/playground/src/State.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/ValidationGraph.jsx` & `lmql-0.0.6.3/src/lmql/ui/playground/src/ValidationGraph.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/browser_process.js` & `lmql-0.0.6.3/src/lmql/ui/playground/src/browser_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/build_info.js` & `lmql-0.0.6.3/src/lmql/ui/playground/src/build_info.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/editor/lmql-monaco-language.js` & `lmql-0.0.6.3/src/lmql/ui/playground/src/editor/lmql-monaco-language.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/editor/theme.json` & `lmql-0.0.6.3/src/lmql/ui/playground/src/editor/theme.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/explore.svg` & `lmql-0.0.6.3/src/lmql/ui/playground/src/explore.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/graph-layout.css` & `lmql-0.0.6.3/src/lmql/ui/playground/src/graph-layout.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/index.css` & `lmql-0.0.6.3/src/lmql/ui/playground/src/index.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/logo.svg` & `lmql-0.0.6.3/src/lmql/ui/playground/src/logo.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/queries.js` & `lmql-0.0.6.3/src/lmql/ui/playground/src/queries.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/remote_process.js` & `lmql-0.0.6.3/src/lmql/ui/playground/src/remote_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/screenshot.css` & `lmql-0.0.6.3/src/lmql/ui/playground/src/screenshot.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/spinner.svg` & `lmql-0.0.6.3/src/lmql/ui/playground/src/spinner.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/src/tagged-model-result.js` & `lmql-0.0.6.3/src/lmql/ui/playground/src/tagged-model-result.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/playground/yarn.lock` & `lmql-0.0.6.3/src/lmql/ui/playground/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/vscode/.vscode/launch.json` & `lmql-0.0.6.3/src/lmql/ui/vscode/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/vscode/LICENSE` & `lmql-0.0.6.3/src/lmql/ui/vscode/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/vscode/language-configuration.json` & `lmql-0.0.6.3/src/lmql/ui/vscode/language-configuration.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/vscode/lmql-vscode.png` & `lmql-0.0.6.3/src/lmql/ui/vscode/lmql-vscode.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/vscode/package.json` & `lmql-0.0.6.3/src/lmql/ui/vscode/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/vscode/syntaxes/lmql.qstring.json` & `lmql-0.0.6.3/src/lmql/ui/vscode/syntaxes/lmql.qstring.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json` & `lmql-0.0.6.3/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/ui/vscode/syntaxes/pylmql.json` & `lmql-0.0.6.3/src/lmql/ui/vscode/syntaxes/pylmql.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/utils/docstring_parser.py` & `lmql-0.0.6.3/src/lmql/utils/docstring_parser.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/utils/graph.py` & `lmql-0.0.6.3/src/lmql/utils/graph.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql/utils/nputil.py` & `lmql-0.0.6.3/src/lmql/utils/nputil.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.2/src/lmql.egg-info/PKG-INFO` & `lmql-0.0.6.3/src/lmql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.0.6.2
+Version: 0.0.6.3
 Summary: A query language for language models.
 Home-page: https://lmql.ai
 Author: Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 Author-email: hello@lmql.ai
 Project-URL: Docs, https://docs.lmql.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lmql Version: 0.0.6.2 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.0.6.3 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
 Type: text/markdown Provides-Extra: hf License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
```

### Comparing `lmql-0.0.6.2/src/lmql.egg-info/SOURCES.txt` & `lmql-0.0.6.3/src/lmql.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 docs/source/_ext/lmql_snippets.py
 docs/source/_static/css/lmql-docs.css
 docs/source/_static/images/lmql.svg
 docs/source/_static/js/lmql-playground.js
 docs/source/_templates/layout.html
 docs/source/blog/release-0.0.5.md
 docs/source/blog/release-0.0.6.1.md
+docs/source/blog/release-0.0.6.3.md
 docs/source/blog/release-0.0.6.md
 docs/source/language/constraints.md
 docs/source/language/decoders.md
 docs/source/language/functions.md
 docs/source/language/models.md
 docs/source/language/overview.md
 docs/source/language/scripted_prompts.md
```

### Comparing `lmql-0.0.6.2/src/lmql.svg` & `lmql-0.0.6.3/src/lmql.svg`

 * *Files identical despite different names*

