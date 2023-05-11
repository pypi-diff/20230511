# Comparing `tmp/jupyterlab_pachyderm-2.6.0rc1.tar.gz` & `tmp/jupyterlab_pachyderm-2.6.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_pachyderm-2.6.0rc1.tar", last modified: Thu Apr 27 17:59:20 2023, max compression
+gzip compressed data, was "jupyterlab_pachyderm-2.6.0rc2.tar", last modified: Fri May  5 14:43:53 2023, max compression
```

## Comparing `jupyterlab_pachyderm-2.6.0rc1.tar` & `jupyterlab_pachyderm-2.6.0rc2.tar`

### file list

```diff
@@ -1,163 +1,164 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.596783 jupyterlab_pachyderm-2.6.0rc1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      749 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11108 2023-04-27 17:59:20.596783 jupyterlab_pachyderm-2.6.0rc1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10130 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/babel.config.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/install.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/jest.config.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.564783 jupyterlab_pachyderm-2.6.0rc1/jupyter-config/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.568783 jupyterlab_pachyderm-2.6.0rc1/jupyter-config/nb-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/jupyter-config/nb-config/jupyterlab_pachyderm.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.568783 jupyterlab_pachyderm-2.6.0rc1/jupyter-config/server-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/jupyter-config/server-config/jupyterlab_pachyderm.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.572783 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/dev_server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      554 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/env.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/filemanager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12522 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/handlers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.572783 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4409 2023-04-27 17:59:18.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.564783 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/schemas/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.580783 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-04-27 17:59:09.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-04-27 17:59:09.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-04-27 17:59:09.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4267 2023-04-27 17:59:09.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-04-27 17:59:09.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.584783 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-04-27 17:59:18.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2023-04-27 17:59:18.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    70514 2023-04-27 17:59:18.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2023-04-27 17:59:18.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)   401782 2023-04-27 17:59:18.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   102166 2023-04-27 17:59:18.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16896 2023-04-27 17:59:18.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   160105 2023-04-27 17:59:18.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/static/829.58d0c33e721471840271.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8301 2023-04-27 17:59:18.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/static/remoteEntry.c5d05e90c93a9acec52d.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-04-27 17:59:09.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/static/style.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8183 2023-04-27 17:59:18.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/static/third-party-licenses.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/log.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9051 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/mount_server_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      640 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/pachyderm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9410 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/pps_client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.584783 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      100 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.584783 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      811 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19088 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/tests/test_handlers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14356 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/tests/test_integrations.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.572783 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11108 2023-04-27 17:59:20.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4641 2023-04-27 17:59:20.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-27 17:59:20.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-27 17:58:54.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-04-27 17:59:20.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-04-27 17:59:20.000000 jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4267 2023-04-27 17:56:41.000000 jupyterlab_pachyderm-2.6.0rc1/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/pyproject.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.588783 jupyterlab_pachyderm-2.6.0rc1/schema/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/schema/examples.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/schema/help.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/schema/mount.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/schema/telemetry.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2023-04-27 17:59:20.596783 jupyterlab_pachyderm-2.6.0rc1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2260 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.588783 jupyterlab_pachyderm-2.6.0rc1/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/global.d.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/handler.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.568783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.588783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/examples/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.588783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/examples/__test__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/examples/__test__/examples.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/examples/examples.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/examples/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.588783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/help/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.588783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/help/__tests__/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.588783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/help/__tests__/__snapshots__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1937 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/help/__tests__/help.test.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/help/help.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/help/help.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/help/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.588783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.588783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5675 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/__tests__/mount.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.564783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.588783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8530 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Config/Config.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.588783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Config/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12024 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Config/__tests__/Config.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.588783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Config/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Config/hooks/useConfig.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.588783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Datum/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4675 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Datum/Datum.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.592783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Datum/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7511 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.592783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Datum/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6182 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Datum/hooks/useDatum.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.592783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/FullPageError/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1012 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/FullPageError/FullPageError.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.592783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/FullPageError/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.592783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Pipeline/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5779 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Pipeline/Pipeline.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Pipeline/Splash.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.592783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Pipeline/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3800 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.592783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Pipeline/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4746 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.592783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/SortableList/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3730 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/SortableList/ListMount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5159 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/SortableList/ListUnmount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3415 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/SortableList/SortableList.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.592783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/SortableList/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14680 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2984 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/customFileBrowser.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1488 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8702 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/mount.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21546 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/mount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2993 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/mountDrive.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3658 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/pollMounts.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2606 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/types.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.592783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/telemetry/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.592783 jupyterlab_pachyderm-2.6.0rc1/src/plugins/telemetry/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/telemetry/__tests__/telemetry.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/telemetry/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/plugins/telemetry/telemetry.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/setupTests.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.592783 jupyterlab_pachyderm-2.6.0rc1/src/utils/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.568783 jupyterlab_pachyderm-2.6.0rc1/src/utils/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.592783 jupyterlab_pachyderm-2.6.0rc1/src/utils/components/Circle/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/utils/components/Circle/Circle.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/utils/components/Circle/circle.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.592783 jupyterlab_pachyderm-2.6.0rc1/src/utils/components/LoadingDots/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/utils/components/LoadingDots/LoadingDots.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/utils/components/LoadingDots/loadingDots.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.592783 jupyterlab_pachyderm-2.6.0rc1/src/utils/components/Svgs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26381 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/utils/components/Svgs/GenericError.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    74288 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/utils/components/Svgs/KubernetesElephant.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16523 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/utils/components/Svgs/PachydermLogo.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/utils/components/Svgs/StatusWarning.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/utils/components/Svgs/index.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.592783 jupyterlab_pachyderm-2.6.0rc1/src/utils/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/utils/hooks/usePreviousValue.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/utils/hooks/useSort.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      675 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/utils/icons.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/src/utils/testUtils.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.596783 jupyterlab_pachyderm-2.6.0rc1/style/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/style/base.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.596783 jupyterlab_pachyderm-2.6.0rc1/style/components/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1524 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/style/components/button.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/style/components/input.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 17:59:20.596783 jupyterlab_pachyderm-2.6.0rc1/style/icons/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/style/icons/file.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/style/icons/info.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/style/icons/mount-logo.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/style/icons/repo.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/style/index.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/style/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-04-27 17:56:40.000000 jupyterlab_pachyderm-2.6.0rc1/tsconfig.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.383269 jupyterlab_pachyderm-2.6.0rc2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11108 2023-05-05 14:43:53.383269 jupyterlab_pachyderm-2.6.0rc2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10130 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/babel.config.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/install.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jest.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.359269 jupyterlab_pachyderm-2.6.0rc2/jupyter-config/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.363269 jupyterlab_pachyderm-2.6.0rc2/jupyter-config/nb-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyter-config/nb-config/jupyterlab_pachyderm.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.363269 jupyterlab_pachyderm-2.6.0rc2/jupyter-config/server-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyter-config/server-config/jupyterlab_pachyderm.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.367269 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/dev_server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      554 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/env.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/filemanager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12522 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/handlers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.367269 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4409 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.359269 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/schemas/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.367269 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-05-05 14:43:40.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-05-05 14:43:40.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-05-05 14:43:40.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4267 2023-05-05 14:43:40.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-05-05 14:43:40.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.371269 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    70514 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   401782 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   102166 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16896 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   160105 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/829.58d0c33e721471840271.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8301 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/remoteEntry.020bdee857c5f964fd3e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-05-05 14:43:40.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/style.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8183 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/third-party-licenses.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/log.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9051 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/mount_server_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      640 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/pachyderm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9524 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/pps_client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.371269 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.371269 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/tests/data/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19088 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/tests/test_handlers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16841 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/tests/test_integrations.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.367269 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11108 2023-05-05 14:43:53.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4690 2023-05-05 14:43:53.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-05 14:43:53.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-05 14:43:24.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-05-05 14:43:53.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-05-05 14:43:53.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4267 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/pyproject.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.371269 jupyterlab_pachyderm-2.6.0rc2/schema/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/schema/examples.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/schema/help.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/schema/mount.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/schema/telemetry.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2023-05-05 14:43:53.383269 jupyterlab_pachyderm-2.6.0rc2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2260 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.371269 jupyterlab_pachyderm-2.6.0rc2/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/global.d.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/handler.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.363269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/examples/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/examples/__test__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/examples/__test__/examples.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/examples/examples.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/examples/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/__tests__/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/__tests__/__snapshots__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1937 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/__tests__/help.test.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/help.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/help.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5675 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/__tests__/mount.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.363269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8530 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Config/Config.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Config/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12024 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Config/__tests__/Config.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Config/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Config/hooks/useConfig.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Datum/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4675 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Datum/Datum.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Datum/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7511 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Datum/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6182 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Datum/hooks/useDatum.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/FullPageError/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1012 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/FullPageError/FullPageError.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/FullPageError/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5779 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/Pipeline.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/Splash.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3800 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4746 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/SortableList/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3730 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/SortableList/ListMount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5159 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/SortableList/ListUnmount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3415 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/SortableList/SortableList.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/SortableList/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14680 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2984 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/customFileBrowser.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1488 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8702 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/mount.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21546 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/mount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2993 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/mountDrive.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3658 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/pollMounts.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2606 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/types.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/telemetry/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/telemetry/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/telemetry/__tests__/telemetry.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/telemetry/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/telemetry/telemetry.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/setupTests.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/src/utils/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.363269 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Circle/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Circle/Circle.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Circle/circle.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/LoadingDots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/LoadingDots/LoadingDots.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/LoadingDots/loadingDots.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Svgs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26381 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Svgs/GenericError.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74288 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Svgs/KubernetesElephant.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16523 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Svgs/PachydermLogo.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Svgs/StatusWarning.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Svgs/index.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/src/utils/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/hooks/usePreviousValue.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/hooks/useSort.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      675 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/icons.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/testUtils.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/style/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/style/base.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/style/components/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1524 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/style/components/button.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/style/components/input.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.383269 jupyterlab_pachyderm-2.6.0rc2/style/icons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/style/icons/file.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/style/icons/info.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/style/icons/mount-logo.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/style/icons/repo.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/style/index.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/style/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/tsconfig.json
```

### Comparing `jupyterlab_pachyderm-2.6.0rc1/LICENSE` & `jupyterlab_pachyderm-2.6.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/MANIFEST.in` & `jupyterlab_pachyderm-2.6.0rc2/MANIFEST.in`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 include LICENSE
 include *.md
 include pyproject.toml
 recursive-include jupyter-config *.json
-recursive-include jupyterlab_pachyderm *.ipynb
+include jupyterlab_pachyderm/tests/data/*
 
 exclude ci-requirements.txt
 exclude .circleci/*
 exclude cypress/*
 exclude cypress.json
 exclude Dockerfile
 exclude scripts/*
```

### Comparing `jupyterlab_pachyderm-2.6.0rc1/PKG-INFO` & `jupyterlab_pachyderm-2.6.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_pachyderm
-Version: 2.6.0rc1
+Version: 2.6.0rc2
 Summary: A JupyterLab extension.
 Home-page: https://github.com/pachyderm/jupyterlab-pachyderm
 Author: 
 Author-email: 
 License: BSD-3-Clause
 Keywords: jupyter,jupyterlab,jupyterlab-extension
 Platform: Linux
```

### Comparing `jupyterlab_pachyderm-2.6.0rc1/README.md` & `jupyterlab_pachyderm-2.6.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/__init__.py` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/_version.py` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/_version.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/env.py` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/env.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/handlers.py` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/package.json` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9758597883597885%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.020bdee857c5f964fd3e.js'}}",*

 * * "'version'": "'2.6.0-rc.2'"}*

```diff
@@ -68,15 +68,15 @@
                 "npm"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.c5d05e90c93a9acec52d.js",
+            "load": "static/remoteEntry.020bdee857c5f964fd3e.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "jupyterlab-pachyderm:examples"
         ],
         "discovery": {
             "server": {
@@ -133,9 +133,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.6.0-rc.1"
+    "version": "2.6.0-rc.2"
 }
```

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'2.6.0-rc.2'"}*

```diff
@@ -128,9 +128,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.6.0-rc.1"
+    "version": "2.6.0-rc.2"
 }
```

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/static/829.58d0c33e721471840271.js` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/829.58d0c33e721471840271.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/static/remoteEntry.c5d05e90c93a9acec52d.js` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/remoteEntry.020bdee857c5f964fd3e.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -116,15 +116,15 @@
                         (!u || !u.loaded && (!a != !u.eager ? a : l > u.from)) && (n[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     i = [];
-                return "default" === t && (u("jupyterlab-pachyderm", "2.6.0-rc.1", (() => Promise.all([j.e(371), j.e(829)]).then((() => () => j(7363))))), u("lodash", "4.17.21", (() => j.e(486).then((() => () => j(6486))))), u("rudder-sdk-js", "1.2.5", (() => j.e(67).then((() => () => j(3067))))), u("yaml", "0", (() => j.e(676).then((() => () => j(5676)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("jupyterlab-pachyderm", "2.6.0-rc.2", (() => Promise.all([j.e(371), j.e(829)]).then((() => () => j(7363))))), u("lodash", "4.17.21", (() => j.e(486).then((() => () => j(6486))))), u("rudder-sdk-js", "1.2.5", (() => j.e(67).then((() => () => j(3067))))), u("yaml", "0", (() => j.e(676).then((() => () => j(5676)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/labextension/static/third-party-licenses.json` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/mount_server_client.py` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/mount_server_client.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/pachyderm.py` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/pachyderm.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/pps_client.py` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/pps_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,14 @@
         check = body.get('last_modified_time')
         if not check:
             raise HTTPError(status_code=400,
                 reason="Bad Request: last_modified_time not specified")
         check = datetime.fromisoformat(check.rstrip('Z'))
 
         last_modified = datetime.utcfromtimestamp(os.path.getmtime(path))
-        get_logger().error(f"{check}, {last_modified}")
         if check != last_modified:
             raise HTTPError(
                 status_code=400,
                 reason=f"stale notebook: client time ({check}) != on-disk time ({last_modified})"
             )
         try:
             config = PpsConfig.from_notebook(path)
@@ -91,15 +90,19 @@
         except Exception as e:
             raise HTTPError(
                 status_code=500,
                 reason=f"could not verify connection to Pachyderm cluster: {repr(e)}"
             )
 
         companion_repo = f"{config.pipeline.name}__context"
-        if companion_repo not in (item.repo.name for item in client.list_repo()):
+        for item in client.list_repo():
+            same_project = config.pipeline.project.name == item.repo.project.name
+            if (companion_repo == item.repo.name) and same_project:
+                break
+        else:
             client.create_repo(
                 repo_name=companion_repo,
                 project_name=config.pipeline.project.name,
                 description=f"files for running the {config.pipeline.name} pipeline"
             )
 
         companion_branch = upload_environment(client, companion_repo, config, script.encode('utf-8'))
@@ -233,15 +236,15 @@
     def entrypoint():
         """Entrypoint used by the PPS extension."""
         print("Greetings from the Pachyderm PPS Extension")
 
         from pathlib import Path
         from subprocess import run
 
-        reqs = Path("requirements.txt")
+        reqs = Path(__file__).parent.joinpath("requirements.txt")
         if reqs.exists():
             run(["pip", "--disable-pip-version-check", "install", "-r", reqs.as_posix()])
 
         import user_code  # This runs the user's code.
 
     entrypoint_script = (
         f'{dedent(getsource(entrypoint))}\n\n'
```

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9868489583333333%*

 * *Differences: {"'cells'": "{0: {'source': ['import pip_install_test']}}",*

 * * "'metadata'": "{'pachyderm_pps': {'config': {'requirements': './requirements.txt'}}}"}*

```diff
@@ -3,15 +3,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": true
             },
             "outputs": [],
-            "source": []
+            "source": [
+                "import pip_install_test"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
@@ -31,15 +33,15 @@
         "pachyderm_pps": {
             "config": {
                 "image": "python:3.10",
                 "input_spec": "pfs:\n  repo: images\n  glob: \"/*\"",
                 "pipeline": {
                     "name": "my_pipeline"
                 },
-                "requirements": ""
+                "requirements": "./requirements.txt"
             },
             "version": "v1.0.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 0
 }
```

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/tests/test_handlers.py` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm/tests/test_integrations.py` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/tests/test_integrations.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 
 import pytest
 import requests
 
 from jupyterlab_pachyderm.handlers import NAMESPACE, VERSION
 from jupyterlab_pachyderm.env import PFS_MOUNT_DIR
 from jupyterlab_pachyderm.pps_client import METADATA_KEY, PpsConfig
+from python_pachyderm.proto.v2.pps.pps_pb2 import JobState
 
-from . import TEST_NOTEBOOK
+from . import TEST_NOTEBOOK, TEST_REQUIREMENTS
 
 ADDRESS = "http://localhost:8888"
 BASE_URL = f"{ADDRESS}/{NAMESPACE}/{VERSION}"
 CONFIG_PATH = "~/.pachyderm/config.json"
 ROOT_TOKEN = "iamroot"
 DEFAULT_PROJECT = "default"
 
@@ -408,47 +409,91 @@
         client.create_repo(repo_name)
         yield client, "default", repo_name, pipeline_name
         client.delete_pipeline(pipeline_name, force=True)
         client.delete_repo(f"{pipeline_name}__context", force=True)
         client.delete_repo(repo_name, force=True)
 
 
+def _update_metadata(notebook: Path, project_name: str, repo_name: str, pipeline_name: str) -> str:
+    """Updates the metadata of the specified notebook file with the specified
+    project/repo/pipeline information.
+
+    Returns a serialized JSON object that can be written to a file.
+    """
+    notebook_data = json.loads(notebook.read_bytes())
+    config = PpsConfig.from_notebook(notebook)
+    config.pipeline = dict(name=pipeline_name, project=dict(name=project_name))
+    # sub in repo_name
+    config.input_spec = f"pfs:\n  repo: {repo_name}\n  glob: \"/*\""
+    config.requirements = str(notebook.with_name(config.requirements).relative_to(os.getcwd()))
+    notebook_data['metadata'][METADATA_KEY]['config'] = config.to_dict()
+    return json.dumps(notebook_data)
+
+
 @pytest.fixture
 def notebook_path(simple_pachyderm_env) -> Path:
     """Yields a path to a notebook file suitable for testing.
 
     This writes a temporary notebook file with its metadata populated
       with the expected pipeline and repo names provided by the
       simple_pachyderm_env fixture.
     """
     _client, project_name, repo_name, pipeline_name = simple_pachyderm_env
 
     # Do a considerable amount of data munging.
-    notebook_data = json.loads(TEST_NOTEBOOK.read_bytes())
-    config = PpsConfig.from_notebook(TEST_NOTEBOOK)
-    config.pipeline = dict(name=pipeline_name, project=dict(name=project_name))
-    # sub in repo_name
-    config.input_spec = f"pfs:\n  repo: {repo_name}\n  glob: \"/*\""
-    notebook_data['metadata'][METADATA_KEY]['config'] = config.to_dict()
-
+    notebook_data = _update_metadata(TEST_NOTEBOOK, project_name, repo_name, pipeline_name)
     notebook_path = TEST_NOTEBOOK.with_stem(f"{TEST_NOTEBOOK.stem}_generated")
-    notebook_path.write_text(json.dumps(notebook_data))
+    notebook_path.write_text(notebook_data)
+
     yield notebook_path.relative_to(os.getcwd())
     if notebook_path.exists():
         notebook_path.unlink()
 
 
 def test_pps(dev_server, simple_pachyderm_env, notebook_path):
     client, project_name, repo_name, pipeline_name = simple_pachyderm_env
+    with client.commit(repo_name, "master", project_name=project_name) as commit:
+        client.put_file_bytes(commit, "/data", b"data")
     last_modified = datetime.utcfromtimestamp(os.path.getmtime(notebook_path))
     data = dict(last_modified_time=f"{datetime.isoformat(last_modified)}Z")
     r = requests.put(f"{BASE_URL}/pps/_create/{notebook_path}", data=json.dumps(data))
     assert r.status_code == 200
-    assert next(client.inspect_pipeline(pipeline_name, project_name=project_name))
+
+    job_info = next(client.list_job(pipeline_name=pipeline_name, project_name=project_name))
+    job_info = next(client.inspect_job(job_info.job.id, pipeline_name=pipeline_name, project_name=project_name, wait=True))
+    assert job_info.state == JobState.JOB_SUCCESS
+
     assert r.json()["message"] == ("Create pipeline request sent. You may monitor its "
     "status by running \"pachctl list pipelines\" in a terminal.")
 
 
 def test_pps_validation_errors(dev_server, notebook_path):
     r = requests.put(f"{BASE_URL}/pps/_create/{notebook_path}", data=json.dumps({}))
     assert r.status_code == 400
     assert r.json()['reason'] == f"Bad Request: last_modified_time not specified"
+
+
+@pytest.mark.parametrize("simple_pachyderm_env", [True], indirect=True)
+def test_pps_reuse_pipeline_name_different_project(dev_server, simple_pachyderm_env, notebook_path):
+    """This tests creating a pipeline from a notebook within a project, and then creating a new
+    pipeline with the same name inside the default project. A bug existed where reusing the pipeline
+    name caused an error. """
+    client, project_name, repo_name, pipeline_name = simple_pachyderm_env
+    test_pps(dev_server, simple_pachyderm_env, notebook_path)
+
+    new_notebook_data = _update_metadata(TEST_NOTEBOOK, "default", repo_name, pipeline_name)
+    new_notebook = TEST_NOTEBOOK.with_stem(f"{TEST_NOTEBOOK.stem}_generated_2")
+    try:
+        client.create_repo(repo_name, project_name="default")
+        new_notebook.write_text(new_notebook_data)
+        new_notebook = new_notebook.relative_to(os.getcwd())
+        last_modified = datetime.utcfromtimestamp(os.path.getmtime(new_notebook))
+        data = dict(last_modified_time=f"{datetime.isoformat(last_modified)}Z")
+        r = requests.put(f"{BASE_URL}/pps/_create/{new_notebook}", data=json.dumps(data))
+        assert r.status_code == 200
+        assert next(client.inspect_pipeline(pipeline_name, project_name="default"))
+    finally:
+        client.delete_pipeline(pipeline_name, project_name="default", force=True)
+        client.delete_repo(f"{pipeline_name}__context", project_name="default", force=True)
+        client.delete_repo(repo_name, project_name="default")
+        if new_notebook.exists():
+            new_notebook.unlink()
```

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm.egg-info/PKG-INFO` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-pachyderm
-Version: 2.6.0rc1
+Version: 2.6.0rc2
 Summary: A JupyterLab extension.
 Home-page: https://github.com/pachyderm/jupyterlab-pachyderm
 Author: 
 Author-email: 
 License: BSD-3-Clause
 Keywords: jupyter,jupyterlab,jupyterlab-extension
 Platform: Linux
```

### Comparing `jupyterlab_pachyderm-2.6.0rc1/jupyterlab_pachyderm.egg-info/SOURCES.txt` & `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,21 +37,22 @@
 jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
 jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
 jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
 jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
 jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
 jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
 jupyterlab_pachyderm/labextension/static/829.58d0c33e721471840271.js
-jupyterlab_pachyderm/labextension/static/remoteEntry.c5d05e90c93a9acec52d.js
+jupyterlab_pachyderm/labextension/static/remoteEntry.020bdee857c5f964fd3e.js
 jupyterlab_pachyderm/labextension/static/style.js
 jupyterlab_pachyderm/labextension/static/third-party-licenses.json
 jupyterlab_pachyderm/tests/__init__.py
 jupyterlab_pachyderm/tests/test_handlers.py
 jupyterlab_pachyderm/tests/test_integrations.py
 jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
+jupyterlab_pachyderm/tests/data/requirements.txt
 schema/examples.json
 schema/help.json
 schema/mount.json
 schema/telemetry.json
 src/global.d.ts
 src/handler.ts
 src/index.ts
```

### Comparing `jupyterlab_pachyderm-2.6.0rc1/package.json` & `jupyterlab_pachyderm-2.6.0rc2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'2.6.0-rc.2'"}*

```diff
@@ -128,9 +128,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.6.0-rc.1"
+    "version": "2.6.0-rc.2"
 }
```

### Comparing `jupyterlab_pachyderm-2.6.0rc1/pyproject.toml` & `jupyterlab_pachyderm-2.6.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/setup.cfg` & `jupyterlab_pachyderm-2.6.0rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/setup.py` & `jupyterlab_pachyderm-2.6.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/handler.ts` & `jupyterlab_pachyderm-2.6.0rc2/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/examples/__test__/examples.test.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/examples/__test__/examples.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/examples/examples.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/examples/examples.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/help/__tests__/help.test.ts` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/__tests__/help.test.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/help/help.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/help.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/__tests__/mount.test.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/__tests__/mount.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Config/Config.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Config/Config.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Config/__tests__/Config.test.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Config/__tests__/Config.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Config/hooks/useConfig.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Config/hooks/useConfig.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Datum/Datum.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Datum/Datum.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Datum/hooks/useDatum.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Datum/hooks/useDatum.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/FullPageError/FullPageError.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/FullPageError/FullPageError.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Pipeline/Pipeline.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/Pipeline.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Pipeline/Splash.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/Splash.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/SortableList/ListMount.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/SortableList/ListMount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/SortableList/ListUnmount.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/SortableList/ListUnmount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/SortableList/SortableList.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/SortableList/SortableList.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/customFileBrowser.ts` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/customFileBrowser.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/index.ts` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/mount.css` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/mount.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/mount.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/mount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/mountDrive.ts` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/mountDrive.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/pollMounts.ts` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/pollMounts.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/mount/types.ts` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/types.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/telemetry/__tests__/telemetry.test.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/telemetry/__tests__/telemetry.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/plugins/telemetry/telemetry.ts` & `jupyterlab_pachyderm-2.6.0rc2/src/plugins/telemetry/telemetry.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/utils/components/Circle/Circle.tsx` & `jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Circle/Circle.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/utils/components/LoadingDots/loadingDots.css` & `jupyterlab_pachyderm-2.6.0rc2/src/utils/components/LoadingDots/loadingDots.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/utils/components/Svgs/GenericError.js` & `jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Svgs/GenericError.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/utils/components/Svgs/KubernetesElephant.js` & `jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Svgs/KubernetesElephant.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/utils/components/Svgs/PachydermLogo.js` & `jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Svgs/PachydermLogo.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/utils/components/Svgs/StatusWarning.js` & `jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Svgs/StatusWarning.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/utils/hooks/useSort.ts` & `jupyterlab_pachyderm-2.6.0rc2/src/utils/hooks/useSort.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/src/utils/icons.ts` & `jupyterlab_pachyderm-2.6.0rc2/src/utils/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/style/base.css` & `jupyterlab_pachyderm-2.6.0rc2/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/style/components/button.css` & `jupyterlab_pachyderm-2.6.0rc2/style/components/button.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/style/icons/file.svg` & `jupyterlab_pachyderm-2.6.0rc2/style/icons/file.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/style/icons/info.svg` & `jupyterlab_pachyderm-2.6.0rc2/style/icons/info.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/style/icons/mount-logo.svg` & `jupyterlab_pachyderm-2.6.0rc2/style/icons/mount-logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc1/style/icons/repo.svg` & `jupyterlab_pachyderm-2.6.0rc2/style/icons/repo.svg`

 * *Files identical despite different names*

