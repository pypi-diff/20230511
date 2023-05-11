# Comparing `tmp/ellar-0.3.6.tar.gz` & `tmp/ellar-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellar-0.3.6.tar", last modified: Mon Apr 10 20:01:35 2023, max compression
+gzip compressed data, was "ellar-0.3.8.tar", last modified: Thu May 11 21:02:51 2023, max compression
```

## Comparing `ellar-0.3.6.tar` & `ellar-0.3.8.tar`

### file list

```diff
@@ -1,455 +1,520 @@
--rw-r--r--   0        0        0      270 2023-04-10 20:01:01.562943 ellar-0.3.6/.coveragerc
--rw-r--r--   0        0        0       65 2023-04-10 20:01:01.562943 ellar-0.3.6/.dockerignore
--rw-r--r--   0        0        0      146 2023-04-10 20:01:01.562943 ellar-0.3.6/.flake8
--rw-r--r--   0        0        0      205 2023-04-10 20:01:01.562943 ellar-0.3.6/.github/dependabot.yml
--rw-r--r--   0        0        0      635 2023-04-10 20:01:01.562943 ellar-0.3.6/.github/workflows/publish.yml
--rw-r--r--   0        0        0      545 2023-04-10 20:01:01.562943 ellar-0.3.6/.github/workflows/test.yml
--rw-r--r--   0        0        0     1122 2023-04-10 20:01:01.562943 ellar-0.3.6/.github/workflows/test_full.yml
--rw-r--r--   0        0        0     1891 2023-04-10 20:01:01.562943 ellar-0.3.6/.gitignore
--rw-r--r--   0        0        0       53 2023-04-10 20:01:01.562943 ellar-0.3.6/.isort.cfg
--rw-r--r--   0        0        0     1073 2023-04-10 20:01:01.562943 ellar-0.3.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1083 2023-04-10 20:01:01.562943 ellar-0.3.6/LICENSE
--rw-r--r--   0        0        0     1166 2023-04-10 20:01:01.562943 ellar-0.3.6/Makefile
--rw-r--r--   0        0        0    10995 2023-04-10 20:01:01.562943 ellar-0.3.6/README.md
--rw-r--r--   0        0        0       15 2023-04-10 20:01:01.562943 ellar-0.3.6/docs/background-task.md
--rw-r--r--   0        0        0       15 2023-04-10 20:01:01.562943 ellar-0.3.6/docs/basics/api-docs.md
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.562943 ellar-0.3.6/docs/basics/custom-providers.md
--rw-r--r--   0        0        0       15 2023-04-10 20:01:01.562943 ellar-0.3.6/docs/basics/events.md
--rw-r--r--   0        0        0    10761 2023-04-10 20:01:01.562943 ellar-0.3.6/docs/basics/execution-context.md
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.562943 ellar-0.3.6/docs/basics/file-streaming.md
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.562943 ellar-0.3.6/docs/basics/injection-scope.md
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.562943 ellar-0.3.6/docs/basics/model-view-controller.md
--rw-r--r--   0        0        0    14945 2023-04-10 20:01:01.562943 ellar-0.3.6/docs/basics/testing.md
--rw-r--r--   0        0        0     7829 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/basics/versioning.md
--rw-r--r--   0        0        0    20977 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/caching.md
--rw-r--r--   0        0        0     1177 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/commands/command-grouping.md
--rw-r--r--   0        0        0     6586 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/commands/create-module-command.md
--rw-r--r--   0        0        0      388 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/commands/create-project-command.md
--rw-r--r--   0        0        0     2755 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/commands/custom-commands.md
--rw-r--r--   0        0        0     1340 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/commands/index.md
--rw-r--r--   0        0        0     1206 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/commands/new-command.md
--rw-r--r--   0        0        0      803 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/commands/runserver-command.md
--rw-r--r--   0        0        0     9064 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/configurations.md
--rw-r--r--   0        0        0     1765 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/custom-setup.md
--rw-r--r--   0        0        0     6728 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/handling-response/response-model.md
--rw-r--r--   0        0        0     6813 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/handling-response/response.md
--rwxr-xr-x   0        0        0    25915 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/img/EllarLogoB.png
--rwxr-xr-x   0        0        0    36744 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/img/EllarLogoIconOnly.png
--rwxr-xr-x   0        0        0    26456 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/img/EllarLogoW.png
--rwxr-xr-x   0        0        0     3888 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/img/Icon.svg
--rwxr-xr-x   0        0        0     4781 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/img/Logo.svg
--rw-r--r--   0        0        0    92094 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/img/ModuleDescription.png
--rw-r--r--   0        0        0    71483 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/img/body-schema-doc.png
--rw-r--r--   0        0        0   233058 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/img/body-schema-doc2.png
--rw-r--r--   0        0        0   196608 2023-04-10 20:01:01.570943 ellar-0.3.6/docs/img/body-schema-doc3.png
--rwxr-xr-x   0        0        0    54689 2023-04-10 20:01:01.570943 ellar-0.3.6/docs/img/car_api.png
--rw-r--r--   0        0        0  1632661 2023-04-10 20:01:01.582943 ellar-0.3.6/docs/img/car_controller.gif
--rw-r--r--   0        0        0    50364 2023-04-10 20:01:01.582943 ellar-0.3.6/docs/img/controller_description.png
--rw-r--r--   0        0        0    45273 2023-04-10 20:01:01.582943 ellar-0.3.6/docs/img/create-car-schema.png
--rw-r--r--   0        0        0    19519 2023-04-10 20:01:01.582943 ellar-0.3.6/docs/img/create-dog-schema.png
--rwxr-xr-x   0        0        0  1326350 2023-04-10 20:01:01.594943 ellar-0.3.6/docs/img/ellar_demo.gif
--rwxr-xr-x   0        0        0    69977 2023-04-10 20:01:01.594943 ellar-0.3.6/docs/img/ellar_framework.png
--rw-r--r--   0        0        0   244178 2023-04-10 20:01:01.594943 ellar-0.3.6/docs/img/enum_docs_swagger.png
--rw-r--r--   0        0        0   168505 2023-04-10 20:01:01.598943 ellar-0.3.6/docs/img/event_docs_swagger.png
--rw-r--r--   0        0        0   253271 2023-04-10 20:01:01.598943 ellar-0.3.6/docs/img/form-schema-doc.png
--rw-r--r--   0        0        0   170683 2023-04-10 20:01:01.598943 ellar-0.3.6/docs/img/json_api_response_model.png
--rw-r--r--   0        0        0   216500 2023-04-10 20:01:01.602943 ellar-0.3.6/docs/img/math_router.png
--rw-r--r--   0        0        0   280669 2023-04-10 20:01:01.602943 ellar-0.3.6/docs/img/math_router_with_request_object.png
--rw-r--r--   0        0        0    52280 2023-04-10 20:01:01.602943 ellar-0.3.6/docs/img/middleware.png
--rw-r--r--   0        0        0   267982 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/img/query_filter_swagger.png
--rw-r--r--   0        0        0   208787 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/img/response_description.png
--rw-r--r--   0        0        0     4427 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/index.md
--rw-r--r--   0        0        0       15 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/mount.md
--rw-r--r--   0        0        0    12584 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/overview/controllers.md
--rw-r--r--   0        0        0    22543 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/overview/custom_decorators.md
--rw-r--r--   0        0        0     8099 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/overview/exception_handling.md
--rw-r--r--   0        0        0     8830 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/overview/guards.md
--rw-r--r--   0        0        0     7667 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/overview/index.md
--rw-r--r--   0        0        0     9240 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/overview/middleware.md
--rw-r--r--   0        0        0     4493 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/overview/module-router.md
--rw-r--r--   0        0        0    16329 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/overview/modules.md
--rw-r--r--   0        0        0     9435 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/overview/providers.md
--rw-r--r--   0        0        0     9184 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/parsing-inputs/body.md
--rw-r--r--   0        0        0     1443 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/parsing-inputs/cookie-params.md
--rw-r--r--   0        0        0     6826 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/parsing-inputs/file-params.md
--rw-r--r--   0        0        0     4268 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/parsing-inputs/form-params.md
--rw-r--r--   0        0        0     3911 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/parsing-inputs/header-params.md
--rw-r--r--   0        0        0     1621 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/parsing-inputs/index.md
--rw-r--r--   0        0        0     6931 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/parsing-inputs/path-params.md
--rw-r--r--   0        0        0     5080 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/parsing-inputs/query-params.md
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/release-notes.md
--rw-r--r--   0        0        0       57 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     4115 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/templating/staticfiles.md
--rw-r--r--   0        0        0    13624 2023-04-10 20:01:01.610942 ellar-0.3.6/docs/templating/templating.md
--rw-r--r--   0        0        0     7321 2023-04-10 20:01:01.610942 ellar-0.3.6/docs/throttling.md
--rw-r--r--   0        0        0       15 2023-04-10 20:01:01.610942 ellar-0.3.6/docs/websockets.md
--rw-r--r--   0        0        0      143 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/__init__.py
--rw-r--r--   0        0        0      396 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/asgi_args.py
--rw-r--r--   0        0        0      257 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/__init__.py
--rw-r--r--   0        0        0      109 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/backends/__init__.py
--rw-r--r--   0        0        0     4841 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/backends/_aio_cache.py.ellar
--rw-r--r--   0        0        0     4361 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/backends/base.py
--rw-r--r--   0        0        0     5138 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/backends/local_cache.py
--rw-r--r--   0        0        0      944 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/backends/pylib_cache.py
--rw-r--r--   0        0        0     2215 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/backends/pymem_cache.py
--rw-r--r--   0        0        0       72 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/backends/redis/__init__.py
--rw-r--r--   0        0        0     6541 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/backends/redis/backend.py
--rw-r--r--   0        0        0     1397 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/backends/serializer.py
--rw-r--r--   0        0        0     5144 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/decorator.py
--rw-r--r--   0        0        0    10943 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/interface.py
--rw-r--r--   0        0        0     2020 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/make_key_decorator.py
--rw-r--r--   0        0        0     2501 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/model.py
--rw-r--r--   0        0        0     1859 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/module.py
--rw-r--r--   0        0        0      852 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/schema.py
--rw-r--r--   0        0        0     4505 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/service.py
--rw-r--r--   0        0        0       62 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/commands/__init__.py
--rw-r--r--   0        0        0     2234 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/commands/base.py
--rw-r--r--   0        0        0     1496 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/__init__.py
--rw-r--r--   0        0        0      839 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/__init__.py
--rw-r--r--   0        0        0      494 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/base.py
--rw-r--r--   0        0        0     1510 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/command.py
--rw-r--r--   0        0        0     6821 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/controller.py
--rw-r--r--   0        0        0     1029 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/exception.py
--rw-r--r--   0        0        0      554 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/extra_args.py
--rw-r--r--   0        0        0     2503 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/file.py
--rw-r--r--   0        0        0      531 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/guards.py
--rw-r--r--   0        0        0     4712 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/html.py
--rw-r--r--   0        0        0      800 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/middleware.py
--rw-r--r--   0        0        0     3421 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/modules.py
--rw-r--r--   0        0        0      918 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/openapi.py
--rw-r--r--   0        0        0     1285 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/serializer.py
--rw-r--r--   0        0        0      395 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/versioning.py
--rw-r--r--   0        0        0     1238 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/routing/__init__.py
--rw-r--r--   0        0        0    10415 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/routing/params.py
--rw-r--r--   0        0        0      345 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/compatible/__init__.py
--rw-r--r--   0        0        0     1174 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/compatible/cache_properties.py
--rw-r--r--   0        0        0      238 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/compatible/contextmanager.py
--rw-r--r--   0        0        0     1515 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/compatible/dict.py
--rw-r--r--   0        0        0      641 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/compatible/emails.py
--rw-r--r--   0        0        0     5387 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/constants.py
--rw-r--r--   0        0        0     1423 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/__init__.py
--rw-r--r--   0        0        0      120 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/conf/__init__.py
--rw-r--r--   0        0        0     4877 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/conf/app_settings_models.py
--rw-r--r--   0        0        0     2149 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/conf/config.py
--rw-r--r--   0        0        0     5129 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/conf/mixins.py
--rw-r--r--   0        0        0      129 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/connection/__init__.py
--rw-r--r--   0        0        0      681 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/connection/http.py
--rw-r--r--   0        0        0      245 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/connection/websocket.py
--rw-r--r--   0        0        0      786 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/context/__init__.py
--rw-r--r--   0        0        0      103 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/context/exceptions.py
--rw-r--r--   0        0        0     1468 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/context/execution.py
--rw-r--r--   0        0        0     2474 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/context/factory.py
--rw-r--r--   0        0        0     2038 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/context/host.py
--rw-r--r--   0        0        0     2077 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/context/http.py
--rw-r--r--   0        0        0     3767 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/context/interface.py
--rw-r--r--   0        0        0      791 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/context/websocket.py
--rw-r--r--   0        0        0       98 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/controller/__init__.py
--rw-r--r--   0        0        0      927 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/controller/model.py
--rw-r--r--   0        0        0     1670 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/converters.py
--rw-r--r--   0        0        0     1511 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/core_service_registration.py
--rw-r--r--   0        0        0      809 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/datastructures.py
--rw-r--r--   0        0        0      867 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/exceptions/__init__.py
--rw-r--r--   0        0        0     1447 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/exceptions/base.py
--rw-r--r--   0        0        0     2510 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/exceptions/callable_exceptions.py
--rw-r--r--   0        0        0     1239 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/exceptions/exceptions_types.py
--rw-r--r--   0        0        0     2529 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/exceptions/handlers.py
--rw-r--r--   0        0        0     1366 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/exceptions/interfaces.py
--rw-r--r--   0        0        0     2239 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/exceptions/service.py
--rw-r--r--   0        0        0      598 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/exceptions/validation.py
--rw-r--r--   0        0        0     7619 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/factory.py
--rw-r--r--   0        0        0      422 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/guard/__init__.py
--rw-r--r--   0        0        0      731 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/guard/apikey.py
--rw-r--r--   0        0        0     4266 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/guard/base.py
--rw-r--r--   0        0        0     3249 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/guard/http.py
--rw-r--r--   0        0        0     9179 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/main.py
--rw-r--r--   0        0        0     1159 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/middleware/__init__.py
--rw-r--r--   0        0        0     2663 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/middleware/di.py
--rw-r--r--   0        0        0     2680 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/middleware/exceptions.py
--rw-r--r--   0        0        0     2244 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/middleware/function.py
--rw-r--r--   0        0        0      447 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/middleware/schema.py
--rw-r--r--   0        0        0      121 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/middleware/sessions.py
--rw-r--r--   0        0        0     1076 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/middleware/versioning.py
--rw-r--r--   0        0        0      317 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/modules/__init__.py
--rw-r--r--   0        0        0     1292 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/modules/base.py
--rw-r--r--   0        0        0     2935 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/modules/builder.py
--rw-r--r--   0        0        0     7450 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/modules/config.py
--rw-r--r--   0        0        0      787 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/modules/helper.py
--rw-r--r--   0        0        0    10173 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/modules/ref.py
--rw-r--r--   0        0        0      681 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/__init__.py
--rw-r--r--   0        0        0      315 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/args/__init__.py
--rw-r--r--   0        0        0    14136 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/args/base.py
--rw-r--r--   0        0        0     1608 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/args/extra_args.py
--rw-r--r--   0        0        0     2002 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/args/factory.py
--rw-r--r--   0        0        0     4158 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/args/request_model.py
--rw-r--r--   0        0        0     5830 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/args/resolver_generators.py
--rw-r--r--   0        0        0     2425 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/args/websocket_model.py
--rw-r--r--   0        0        0     1203 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/helpers.py
--rw-r--r--   0        0        0     9194 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/params.py
--rw-r--r--   0        0        0     1083 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/__init__.py
--rw-r--r--   0        0        0     1651 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/base.py
--rw-r--r--   0        0        0     4455 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/bulk_parameter.py
--rw-r--r--   0        0        0      687 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/non_parameter/__init__.py
--rw-r--r--   0        0        0     2942 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/non_parameter/base.py
--rw-r--r--   0        0        0      386 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/non_parameter/connection.py
--rw-r--r--   0        0        0      323 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/non_parameter/context.py
--rw-r--r--   0        0        0     1648 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/non_parameter/inject.py
--rw-r--r--   0        0        0      382 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/non_parameter/request.py
--rw-r--r--   0        0        0      389 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/non_parameter/response.py
--rw-r--r--   0        0        0      519 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/non_parameter/session.py
--rw-r--r--   0        0        0      381 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/non_parameter/websocket.py
--rw-r--r--   0        0        0     9511 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/parameter.py
--rw-r--r--   0        0        0      623 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/response/__init__.py
--rw-r--r--   0        0        0      961 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/response/model/__init__.py
--rw-r--r--   0        0        0     8397 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/response/model/base.py
--rw-r--r--   0        0        0      715 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/response/model/factory.py
--rw-r--r--   0        0        0     3117 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/response/model/file.py
--rw-r--r--   0        0        0     2036 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/response/model/html.py
--rw-r--r--   0        0        0      802 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/response/model/interface.py
--rw-r--r--   0        0        0     2310 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/response/model/json.py
--rw-r--r--   0        0        0     4244 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/response/model/route.py
--rw-r--r--   0        0        0      995 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/response/response_types.py
--rw-r--r--   0        0        0      465 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/__init__.py
--rw-r--r--   0        0        0     4609 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/base.py
--rw-r--r--   0        0        0      272 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/controller/__init__.py
--rw-r--r--   0        0        0     1180 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/controller/base.py
--rw-r--r--   0        0        0     1233 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/controller/route.py
--rw-r--r--   0        0        0      190 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/controller/websocket/__init__.py
--rw-r--r--   0        0        0     1421 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/controller/websocket/handler.py
--rw-r--r--   0        0        0     2004 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/controller/websocket/route.py
--rw-r--r--   0        0        0    10981 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/operation_definitions.py
--rw-r--r--   0        0        0     4616 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/route.py
--rw-r--r--   0        0        0      230 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/router/__init__.py
--rw-r--r--   0        0        0     3838 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/router/app.py
--rw-r--r--   0        0        0     7819 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/router/module.py
--rw-r--r--   0        0        0     3567 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/routing/router/route_collections.py
--rw-r--r--   0        0        0      161 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/routing/websocket/__init__.py
--rw-r--r--   0        0        0     5643 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/routing/websocket/handler.py
--rw-r--r--   0        0        0     4917 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/routing/websocket/route.py
--rw-r--r--   0        0        0     3402 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/schema.py
--rw-r--r--   0        0        0     1718 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/staticfiles.py
--rw-r--r--   0        0        0      600 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/templating/__init__.py
--rw-r--r--   0        0        0      472 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/templating/environment.py
--rw-r--r--   0        0        0     7419 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/templating/interface.py
--rw-r--r--   0        0        0     1634 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/templating/loader.py
--rw-r--r--   0        0        0     2421 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/templating/renderer.py
--rw-r--r--   0        0        0      563 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/versioning/__init__.py
--rw-r--r--   0        0        0     2519 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/versioning/base.py
--rw-r--r--   0        0        0     6182 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/versioning/resolver.py
--rw-r--r--   0        0        0      620 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/di/__init__.py
--rw-r--r--   0        0        0      400 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/di/exceptions.py
--rw-r--r--   0        0        0      117 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/di/injector/__init__.py
--rw-r--r--   0        0        0     7411 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/di/injector/container.py
--rw-r--r--   0        0        0     5270 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/di/injector/ellar_injector.py
--rw-r--r--   0        0        0      845 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/di/providers.py
--rw-r--r--   0        0        0     2253 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/di/scopes.py
--rw-r--r--   0        0        0     4545 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/di/service_config.py
--rw-r--r--   0        0        0     2045 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/events.py
--rw-r--r--   0        0        0     1485 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/helper/__init__.py
--rw-r--r--   0        0        0      658 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/helper/enums.py
--rw-r--r--   0        0        0      389 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/helper/event_loop.py
--rw-r--r--   0        0        0     2137 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/helper/importer.py
--rw-r--r--   0        0        0     1272 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/helper/modelfield.py
--rw-r--r--   0        0        0      703 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/helper/module_loading.py
--rw-r--r--   0        0        0       52 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/logger.py
--rw-r--r--   0        0        0      573 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/__init__.py
--rw-r--r--   0        0        0     8077 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/builder.py
--rw-r--r--   0        0        0      239 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/docs_generators/__init__.py
--rw-r--r--   0        0        0      530 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/docs_generators/base.py
--rw-r--r--   0        0        0      959 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/docs_generators/redocs.py
--rw-r--r--   0        0        0     1025 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/docs_generators/swagger.py
--rw-r--r--   0        0        0     2934 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/module.py
--rw-r--r--   0        0        0    10597 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/openapi_v3.py
--rw-r--r--   0        0        0    15790 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/route_doc_models.py
--rw-r--r--   0        0        0      702 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/templates/redocs.html
--rw-r--r--   0        0        0      758 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/templates/swagger.html
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/py.typed
--rw-r--r--   0        0        0     5274 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/reflect.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/samples/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/samples/controllers/__init__.py
--rw-r--r--   0        0        0      403 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/samples/controllers/home.py
--rw-r--r--   0        0        0      211 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/samples/modules.py
--rw-r--r--   0        0        0   155845 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/samples/static/css/bootstrap.min.css
--rwxr-xr-x   0        0        0    25915 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/samples/static/img/EllarLogoB.png
--rwxr-xr-x   0        0        0    36744 2023-04-10 20:01:01.622942 ellar-0.3.6/ellar/samples/static/img/EllarLogoIconOnly.png
--rwxr-xr-x   0        0        0     3888 2023-04-10 20:01:01.622942 ellar-0.3.6/ellar/samples/static/img/Icon.svg
--rw-r--r--   0        0        0     1312 2023-04-10 20:01:01.622942 ellar-0.3.6/ellar/samples/templates/home/index.html
--rw-r--r--   0        0        0     4959 2023-04-10 20:01:01.622942 ellar-0.3.6/ellar/serializer.py
--rw-r--r--   0        0        0       58 2023-04-10 20:01:01.622942 ellar-0.3.6/ellar/services/__init__.py
--rw-r--r--   0        0        0     1949 2023-04-10 20:01:01.622942 ellar-0.3.6/ellar/services/reflector.py
--rw-r--r--   0        0        0      458 2023-04-10 20:01:01.622942 ellar-0.3.6/ellar/shortcuts.py
--rw-r--r--   0        0        0      129 2023-04-10 20:01:01.622942 ellar-0.3.6/ellar/testing/__init__.py
--rw-r--r--   0        0        0     4034 2023-04-10 20:01:01.622942 ellar-0.3.6/ellar/testing/module.py
--rw-r--r--   0        0        0      585 2023-04-10 20:01:01.622942 ellar-0.3.6/ellar/types.py
--rw-r--r--   0        0        0      509 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/README.md
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/__init__.py
--rw-r--r--   0        0        0     1681 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/controllers.py
--rw-r--r--   0        0        0     1077 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/module.py
--rw-r--r--   0        0        0     1237 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/routers.py
--rw-r--r--   0        0        0      622 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/schemas.py
--rw-r--r--   0        0        0      666 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/services.py
--rw-r--r--   0        0        0     1708 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/statics/blog/blog.css
--rw-r--r--   0        0        0     1586 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/statics/blog/blog.rtl.css
--rw-r--r--   0        0        0     1008 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo-white.svg
--rw-r--r--   0        0        0     2047 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo.svg
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/tests/__init__.py
--rw-r--r--   0        0        0     2900 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/tests/test_controllers.py
--rw-r--r--   0        0        0     1604 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/tests/test_routers.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/tests/test_services.py
--rw-r--r--   0        0        0      202 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/views/car/list.html
--rw-r--r--   0        0        0      202 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/views/cat/list.html
--rw-r--r--   0        0        0    15257 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/views/index.html
--rw-r--r--   0        0        0      242 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/commands.py
--rw-r--r--   0        0        0      187 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/config.py
--rw-r--r--   0        0        0      635 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/root_module.py
--rw-r--r--   0        0        0      947 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/server.py
--rw-r--r--   0        0        0      134 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/tests/conftest.py
--rw-r--r--   0        0        0      241 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/pyproject.toml
--rw-r--r--   0        0        0     3755 2023-04-10 20:01:01.622942 ellar-0.3.6/mkdocs.yml
--rw-r--r--   0        0        0      639 2023-04-10 20:01:01.622942 ellar-0.3.6/mypy.ini
--rw-r--r--   0        0        0     2920 2023-04-10 20:01:01.622942 ellar-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      207 2023-04-10 20:01:01.622942 ellar-0.3.6/pytest.ini
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/__init__.py
--rw-r--r--   0        0        0     1022 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/conftest.py
--rw-r--r--   0        0        0      616 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/injector_module.py
--rw-r--r--   0        0        0     5270 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/main.py
--rw-r--r--   0        0        0       23 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/private/test.css
--rw-r--r--   0        0        0      741 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/schema.py
--rw-r--r--   0        0        0        4 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/statics/example.txt
--rw-r--r--   0        0        0      160 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/templates/ellar/index.html
--rw-r--r--   0        0        0      102 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/templates/ellar/list.html
--rw-r--r--   0        0        0      129 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/templates/index.html
--rw-r--r--   0        0        0      128 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/templates/list.html
--rw-r--r--   0        0        0       65 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/templates/render_string.html
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_application/__init__.py
--rw-r--r--   0        0        0       84 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_application/config.py
--rw-r--r--   0        0        0     2869 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_application/sample.py
--rw-r--r--   0        0        0     3385 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_application/test_application_factory.py
--rw-r--r--   0        0        0    15889 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_application/test_application_functions.py
--rw-r--r--   0        0        0    18052 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_application/test_cors.py
--rw-r--r--   0        0        0     4254 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_application/test_replacing_app_services.py
--rw-r--r--   0        0        0     2329 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_application/test_trusted_host.py
--rw-r--r--   0        0        0      860 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_attribute_dict.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_cache/__init__.py
--rw-r--r--   0        0        0     3625 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_cache/_test_aio_memcache.py.ellar
--rw-r--r--   0        0        0     1893 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_cache/pylib_mock.py
--rw-r--r--   0        0        0     2592 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_cache/redis_mock.py
--rw-r--r--   0        0        0     2795 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_cache/test_cache_decorator.py
--rw-r--r--   0        0        0     1775 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_cache/test_cache_many_config.py
--rw-r--r--   0        0        0     4772 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_cache/test_cache_service.py
--rw-r--r--   0        0        0     4995 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_cache/test_local_cache.py
--rw-r--r--   0        0        0      596 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_cache/test_module_setup.py
--rw-r--r--   0        0        0     9973 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_cache/test_pylibmc_cache.py
--rw-r--r--   0        0        0     6093 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_cache/test_redis_cache.py
--rw-r--r--   0        0        0      577 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_cache/test_schema.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/__init__.py
--rw-r--r--   0        0        0     3352 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/test_decorators/test_controller.py
--rw-r--r--   0        0        0      782 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/test_decorators/test_exception.py
--rw-r--r--   0        0        0     3495 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/test_decorators/test_file.py
--rw-r--r--   0        0        0     1104 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/test_decorators/test_guards.py
--rw-r--r--   0        0        0     4078 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/test_decorators/test_html.py
--rw-r--r--   0        0        0      646 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/test_decorators/test_middleware.py
--rw-r--r--   0        0        0     2064 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/test_decorators/test_modules.py
--rw-r--r--   0        0        0      901 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/test_decorators/test_openapi.py
--rw-r--r--   0        0        0     1297 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/test_decorators/test_serializer.py
--rw-r--r--   0        0        0      468 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/test_decorators/test_versioning.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_conf/__init__.py
--rw-r--r--   0        0        0     5216 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_conf/test_default_conf.py
--rw-r--r--   0        0        0     1151 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_conf/test_mixins.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_controller/__init__.py
--rw-r--r--   0        0        0      439 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_controller/sample.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_controller/test_application_router.py
--rw-r--r--   0        0        0     4442 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_controller/test_controller_decorator.py
--rw-r--r--   0        0        0     2445 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_controller/test_controller_inheritance.py
--rw-r--r--   0        0        0     2626 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_controller/test_module_router.py
--rw-r--r--   0        0        0     7156 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_controller/test_route_collection.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_di/__init__.py
--rw-r--r--   0        0        0     1332 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_di/examples.py
--rw-r--r--   0        0        0     2078 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_di/test_injectable_resolving.py
--rw-r--r--   0        0        0     5831 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_di/test_injector.py
--rw-r--r--   0        0        0     3508 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_di/test_provider_scopes.py
--rw-r--r--   0        0        0     3993 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_di/test_providers.py
--rw-r--r--   0        0        0     1810 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_events.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_exceptions/__init__.py
--rw-r--r--   0        0        0      206 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_exceptions/exception_runner.py
--rw-r--r--   0        0        0     2560 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_exceptions/test_api_exception.py
--rw-r--r--   0        0        0     8679 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_exceptions/test_custom_exceptions.py
--rw-r--r--   0        0        0     1195 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_exceptions/test_error_details.py
--rw-r--r--   0        0        0     3720 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_exceptions/test_validation_exception.py
--rw-r--r--   0        0        0     7249 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_guard.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_helper/__init__.py
--rw-r--r--   0        0        0      564 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_helper/test_enum.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_helper/test_importer.py
--rw-r--r--   0        0        0      784 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_helper/test_model_field.py
--rw-r--r--   0        0        0      291 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_helper/test_module_loading.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_middleware/__init__.py
--rw-r--r--   0        0        0     2286 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_middleware/test_functional_middleware.py
--rw-r--r--   0        0        0     4207 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_middleware/test_service_provider_middleware.py
--rw-r--r--   0        0        0     2161 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_middleware/test_versioning_middleware.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_modules/__init__.py
--rw-r--r--   0        0        0     1847 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_modules/sample.py
--rw-r--r--   0        0        0     6752 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_modules/test_module_config.py
--rw-r--r--   0        0        0     9889 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_modules/test_module_ref.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_openapi/__init__.py
--rw-r--r--   0        0        0     8369 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_openapi/test_builder.py
--rw-r--r--   0        0        0     6656 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_openapi/test_module.py
--rw-r--r--   0        0        0    16438 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_openapi/test_open_api_route_documentation.py
--rw-r--r--   0        0        0     5598 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_reflect.py
--rw-r--r--   0        0        0     2159 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_reflector.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_response/__init__.py
--rw-r--r--   0        0        0     2483 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_response/test_defined_response_model.py
--rw-r--r--   0        0        0     4592 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_response/test_pydantic_response_model.py
--rw-r--r--   0        0        0     3447 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_response/test_response_file.py
--rw-r--r--   0        0        0     5078 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_response/test_response_html.py
--rw-r--r--   0        0        0     3282 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_response/test_response_streaming.py
--rw-r--r--   0        0        0     3882 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_response/test_response_type_definition_converter.py
--rw-r--r--   0        0        0     3509 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_response/test_route_response_model.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/__init__.py
--rw-r--r--   0        0        0     1088 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/sample.py
--rw-r--r--   0        0        0     3598 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_body_schema.py
--rw-r--r--   0        0        0     3659 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_body_schema_extra_properties.py
--rw-r--r--   0        0        0     4135 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_body_union_schema.py
--rw-r--r--   0        0        0     3958 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_cookie_schema.py
--rw-r--r--   0        0        0     6875 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_extra_args.py
--rw-r--r--   0        0        0     2402 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_form_schema.py
--rw-r--r--   0        0        0    10085 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_formparsers.py
--rw-r--r--   0        0        0     1312 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_forms.py
--rw-r--r--   0        0        0     1326 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_forms_from_non_typing_sequences.py
--rw-r--r--   0        0        0     3578 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_header_schema.py
--rw-r--r--   0        0        0     1569 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_invalid_path_param.py
--rw-r--r--   0        0        0     1788 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_routing/test_invalid_sequence_param.py
--rw-r--r--   0        0        0     5233 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_routing/test_multi_body_errors.py
--rw-r--r--   0        0        0     3811 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_routing/test_multi_query_errors.py
--rw-r--r--   0        0        0     9423 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_routing/test_path.py
--rw-r--r--   0        0        0     2825 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_routing/test_path_with_schema.py
--rw-r--r--   0        0        0     3361 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_routing/test_put_with_no_body_schema.py
--rw-r--r--   0        0        0     2242 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_routing/test_query.py
--rw-r--r--   0        0        0     3644 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_routing/test_query_schema.py
--rw-r--r--   0        0        0     2017 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_routing/test_request.py
--rw-r--r--   0        0        0     3430 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_routing/test_route_endpoint_params.py
--rw-r--r--   0        0        0      451 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_sample_project.py
--rw-r--r--   0        0        0     2689 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_schema.py
--rw-r--r--   0        0        0     6372 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_serializer.py
--rw-r--r--   0        0        0      768 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_shortcuts.py
--rw-r--r--   0        0        0    14104 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_staticfiles.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_templating/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_templating/module_statics/watever.txt
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_templating/static/watever.txt
--rw-r--r--   0        0        0      167 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_templating/templates/watever.html
--rw-r--r--   0        0        0     2892 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_templating/test_module_templating.py
--rw-r--r--   0        0        0     2757 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_templating/test_renderer.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_templating/views/watever.html
--rw-r--r--   0        0        0     2418 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_testing.py
--rw-r--r--   0        0        0        0 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_versioning/__init__.py
--rw-r--r--   0        0        0     1968 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_versioning/operations.py
--rw-r--r--   0        0        0     2138 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_versioning/test_default_versioning.py
--rw-r--r--   0        0        0     4449 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_versioning/test_default_versioning_for_controllers.py
--rw-r--r--   0        0        0     4468 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_versioning/test_header_versioning.py
--rw-r--r--   0        0        0     7813 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_versioning/test_header_versioning_controller.py
--rw-r--r--   0        0        0     3816 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_versioning/test_host_versioning.py
--rw-r--r--   0        0        0     3220 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_versioning/test_query_versioning.py
--rw-r--r--   0        0        0     2858 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_versioning/test_url_versioning.py
--rw-r--r--   0        0        0    17496 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_websocket.py
--rw-r--r--   0        0        0    11066 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_websocket_handler.py
--rw-r--r--   0        0        0    14875 1970-01-01 00:00:00.000000 ellar-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0      270 2023-05-11 21:02:05.040800 ellar-0.3.8/.coveragerc
+-rw-r--r--   0        0        0       65 2023-05-11 21:02:05.040800 ellar-0.3.8/.dockerignore
+-rw-r--r--   0        0        0      146 2023-05-11 21:02:05.040800 ellar-0.3.8/.flake8
+-rw-r--r--   0        0        0      205 2023-05-11 21:02:05.040800 ellar-0.3.8/.github/dependabot.yml
+-rw-r--r--   0        0        0      635 2023-05-11 21:02:05.040800 ellar-0.3.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      545 2023-05-11 21:02:05.040800 ellar-0.3.8/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1122 2023-05-11 21:02:05.044801 ellar-0.3.8/.github/workflows/test_full.yml
+-rw-r--r--   0        0        0     1891 2023-05-11 21:02:05.044801 ellar-0.3.8/.gitignore
+-rw-r--r--   0        0        0       53 2023-05-11 21:02:05.044801 ellar-0.3.8/.isort.cfg
+-rw-r--r--   0        0        0     1073 2023-05-11 21:02:05.044801 ellar-0.3.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1083 2023-05-11 21:02:05.044801 ellar-0.3.8/LICENSE
+-rw-r--r--   0        0        0     1166 2023-05-11 21:02:05.044801 ellar-0.3.8/Makefile
+-rw-r--r--   0        0        0    10720 2023-05-11 21:02:05.044801 ellar-0.3.8/README.md
+-rw-r--r--   0        0        0       15 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/background-task.md
+-rw-r--r--   0        0        0       15 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/basics/api-docs.md
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/basics/custom-providers.md
+-rw-r--r--   0        0        0       15 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/basics/events.md
+-rw-r--r--   0        0        0    10656 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/basics/execution-context.md
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/basics/file-streaming.md
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/basics/injection-scope.md
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/basics/model-view-controller.md
+-rw-r--r--   0        0        0    14828 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/basics/testing.md
+-rw-r--r--   0        0        0     7857 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/basics/versioning.md
+-rw-r--r--   0        0        0    20991 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/caching.md
+-rw-r--r--   0        0        0     1177 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/commands/command-grouping.md
+-rw-r--r--   0        0        0     6586 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/commands/create-module-command.md
+-rw-r--r--   0        0        0      388 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/commands/create-project-command.md
+-rw-r--r--   0        0        0     2755 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/commands/custom-commands.md
+-rw-r--r--   0        0        0     1340 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/commands/index.md
+-rw-r--r--   0        0        0     1206 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/commands/new-command.md
+-rw-r--r--   0        0        0      803 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/commands/runserver-command.md
+-rw-r--r--   0        0        0     9048 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/configurations.md
+-rw-r--r--   0        0        0     1765 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/custom-setup.md
+-rw-r--r--   0        0        0     6502 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/handling-response/response-model.md
+-rw-r--r--   0        0        0     6571 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/handling-response/response.md
+-rwxr-xr-x   0        0        0    25915 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/img/EllarLogoB.png
+-rwxr-xr-x   0        0        0    36744 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/img/EllarLogoIconOnly.png
+-rwxr-xr-x   0        0        0    26456 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/img/EllarLogoW.png
+-rwxr-xr-x   0        0        0     3888 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/img/Icon.svg
+-rwxr-xr-x   0        0        0     4781 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/img/Logo.svg
+-rw-r--r--   0        0        0    92094 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/img/ModuleDescription.png
+-rw-r--r--   0        0        0    71483 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/img/body-schema-doc.png
+-rw-r--r--   0        0        0   233058 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/img/body-schema-doc2.png
+-rw-r--r--   0        0        0   196608 2023-05-11 21:02:05.048801 ellar-0.3.8/docs/img/body-schema-doc3.png
+-rwxr-xr-x   0        0        0    54689 2023-05-11 21:02:05.048801 ellar-0.3.8/docs/img/car_api.png
+-rw-r--r--   0        0        0  1632661 2023-05-11 21:02:05.056801 ellar-0.3.8/docs/img/car_controller.gif
+-rw-r--r--   0        0        0    50364 2023-05-11 21:02:05.056801 ellar-0.3.8/docs/img/controller_description.png
+-rw-r--r--   0        0        0    45273 2023-05-11 21:02:05.056801 ellar-0.3.8/docs/img/create-car-schema.png
+-rw-r--r--   0        0        0    19519 2023-05-11 21:02:05.056801 ellar-0.3.8/docs/img/create-dog-schema.png
+-rwxr-xr-x   0        0        0  1326350 2023-05-11 21:02:05.064801 ellar-0.3.8/docs/img/ellar_demo.gif
+-rwxr-xr-x   0        0        0    69977 2023-05-11 21:02:05.064801 ellar-0.3.8/docs/img/ellar_framework.png
+-rw-r--r--   0        0        0   244178 2023-05-11 21:02:05.064801 ellar-0.3.8/docs/img/enum_docs_swagger.png
+-rw-r--r--   0        0        0   168505 2023-05-11 21:02:05.068801 ellar-0.3.8/docs/img/event_docs_swagger.png
+-rw-r--r--   0        0        0   253271 2023-05-11 21:02:05.068801 ellar-0.3.8/docs/img/form-schema-doc.png
+-rw-r--r--   0        0        0   170683 2023-05-11 21:02:05.068801 ellar-0.3.8/docs/img/json_api_response_model.png
+-rw-r--r--   0        0        0    71548 2023-05-11 21:02:05.068801 ellar-0.3.8/docs/img/live_support_websocket.gif
+-rw-r--r--   0        0        0   121361 2023-05-11 21:02:05.068801 ellar-0.3.8/docs/img/live_support_websocket_3.gif
+-rw-r--r--   0        0        0   216500 2023-05-11 21:02:05.072801 ellar-0.3.8/docs/img/math_router.png
+-rw-r--r--   0        0        0   280669 2023-05-11 21:02:05.072801 ellar-0.3.8/docs/img/math_router_with_request_object.png
+-rw-r--r--   0        0        0    52280 2023-05-11 21:02:05.072801 ellar-0.3.8/docs/img/middleware.png
+-rw-r--r--   0        0        0   267982 2023-05-11 21:02:05.072801 ellar-0.3.8/docs/img/query_filter_swagger.png
+-rw-r--r--   0        0        0   208787 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/img/response_description.png
+-rw-r--r--   0        0        0     4486 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/index.md
+-rw-r--r--   0        0        0       15 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/mount.md
+-rw-r--r--   0        0        0    12542 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/overview/controllers.md
+-rw-r--r--   0        0        0    22629 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/overview/custom_decorators.md
+-rw-r--r--   0        0        0     7960 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/overview/exception_handling.md
+-rw-r--r--   0        0        0     8926 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/overview/guards.md
+-rw-r--r--   0        0        0     7665 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/overview/index.md
+-rw-r--r--   0        0        0     9240 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/overview/middleware.md
+-rw-r--r--   0        0        0     4493 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/overview/module-router.md
+-rw-r--r--   0        0        0    15322 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/overview/modules.md
+-rw-r--r--   0        0        0     9375 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/overview/providers.md
+-rw-r--r--   0        0        0     8879 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/parsing-inputs/body.md
+-rw-r--r--   0        0        0     1371 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/parsing-inputs/cookie-params.md
+-rw-r--r--   0        0        0     6588 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/parsing-inputs/file-params.md
+-rw-r--r--   0        0        0     4096 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/parsing-inputs/form-params.md
+-rw-r--r--   0        0        0     3795 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/parsing-inputs/header-params.md
+-rw-r--r--   0        0        0     1560 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/parsing-inputs/index.md
+-rw-r--r--   0        0        0     6749 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/parsing-inputs/path-params.md
+-rw-r--r--   0        0        0     4920 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/parsing-inputs/query-params.md
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/release-notes.md
+-rw-r--r--   0        0        0       69 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     4111 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/templating/staticfiles.md
+-rw-r--r--   0        0        0    13593 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/templating/templating.md
+-rw-r--r--   0        0        0     7327 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/throttling.md
+-rw-r--r--   0        0        0    12688 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/websockets/index.md
+-rw-r--r--   0        0        0    12825 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/websockets/socketio.md
+-rw-r--r--   0        0        0      143 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/__init__.py
+-rw-r--r--   0        0        0      257 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/__init__.py
+-rw-r--r--   0        0        0      109 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/backends/__init__.py
+-rw-r--r--   0        0        0     4841 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/backends/_aio_cache.py.ellar
+-rw-r--r--   0        0        0     4361 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/backends/base.py
+-rw-r--r--   0        0        0     5145 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/backends/local_cache.py
+-rw-r--r--   0        0        0      944 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/backends/pylib_cache.py
+-rw-r--r--   0        0        0     2215 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/backends/pymem_cache.py
+-rw-r--r--   0        0        0       72 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/backends/redis/__init__.py
+-rw-r--r--   0        0        0     6548 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/backends/redis/backend.py
+-rw-r--r--   0        0        0     1397 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/backends/serializer.py
+-rw-r--r--   0        0        0     5132 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/decorator.py
+-rw-r--r--   0        0        0    10943 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/interface.py
+-rw-r--r--   0        0        0     2027 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/make_key_decorator.py
+-rw-r--r--   0        0        0     2501 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/model.py
+-rw-r--r--   0        0        0     1859 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/module.py
+-rw-r--r--   0        0        0      852 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/schema.py
+-rw-r--r--   0        0        0     4505 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/service.py
+-rw-r--r--   0        0        0     3727 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/__init__.py
+-rw-r--r--   0        0        0      108 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/commands/__init__.py
+-rw-r--r--   0        0        0     2234 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/commands/base.py
+-rw-r--r--   0        0        0     1517 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/commands/decorator.py
+-rw-r--r--   0        0        0      270 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/compatible/__init__.py
+-rw-r--r--   0        0        0     1166 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/compatible/cache_properties.py
+-rw-r--r--   0        0        0     1511 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/compatible/dict.py
+-rw-r--r--   0        0        0      637 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/compatible/emails.py
+-rw-r--r--   0        0        0     4620 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/constants.py
+-rw-r--r--   0        0        0     1670 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/converters.py
+-rw-r--r--   0        0        0      809 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/datastructures.py
+-rw-r--r--   0        0        0      795 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/decorators/__init__.py
+-rw-r--r--   0        0        0      501 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/decorators/base.py
+-rw-r--r--   0        0        0     6652 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/decorators/controller.py
+-rw-r--r--   0        0        0     1036 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/decorators/exception.py
+-rw-r--r--   0        0        0      610 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/decorators/extra_args.py
+-rw-r--r--   0        0        0     2528 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/decorators/file.py
+-rw-r--r--   0        0        0      541 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/decorators/guards.py
+-rw-r--r--   0        0        0     4748 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/decorators/html.py
+-rw-r--r--   0        0        0      626 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/decorators/middleware.py
+-rw-r--r--   0        0        0     3105 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/decorators/modules.py
+-rw-r--r--   0        0        0      932 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/decorators/openapi.py
+-rw-r--r--   0        0        0     1295 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/decorators/serializer.py
+-rw-r--r--   0        0        0      402 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/decorators/versioning.py
+-rw-r--r--   0        0        0      840 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/exceptions/__init__.py
+-rw-r--r--   0        0        0      472 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/exceptions/api/__init__.py
+-rw-r--r--   0        0        0     1447 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/exceptions/api/base.py
+-rw-r--r--   0        0        0     1239 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/exceptions/api/exceptions_types.py
+-rw-r--r--   0        0        0     2498 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/exceptions/callable_exceptions.py
+-rw-r--r--   0        0        0      103 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/exceptions/context.py
+-rw-r--r--   0        0        0     2517 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/exceptions/handlers.py
+-rw-r--r--   0        0        0      598 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/exceptions/validation.py
+-rw-r--r--   0        0        0     1485 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/helper/__init__.py
+-rw-r--r--   0        0        0      658 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/helper/enums.py
+-rw-r--r--   0        0        0      389 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/helper/event_loop.py
+-rw-r--r--   0        0        0     2137 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/helper/importer.py
+-rw-r--r--   0        0        0     1272 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/helper/modelfield.py
+-rw-r--r--   0        0        0      703 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/helper/module_loading.py
+-rw-r--r--   0        0        0      800 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/interfaces/__init__.py
+-rw-r--r--   0        0        0     3560 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/interfaces/context.py
+-rw-r--r--   0        0        0      278 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/interfaces/controller_factory.py
+-rw-r--r--   0        0        0     1356 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/interfaces/exceptions.py
+-rw-r--r--   0        0        0     1771 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/interfaces/module.py
+-rw-r--r--   0        0        0      749 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/interfaces/response_model.py
+-rw-r--r--   0        0        0      908 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/interfaces/templating.py
+-rw-r--r--   0        0        0       52 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/logger.py
+-rw-r--r--   0        0        0      274 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/models/__init__.py
+-rw-r--r--   0        0        0      923 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/models/controller.py
+-rw-r--r--   0        0        0     4258 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/models/guard.py
+-rw-r--r--   0        0        0      476 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/__init__.py
+-rw-r--r--   0        0        0      365 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/args/__init__.py
+-rw-r--r--   0        0        0    14101 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/args/base.py
+-rw-r--r--   0        0        0     1615 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/args/extra_args.py
+-rw-r--r--   0        0        0     2045 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/args/factory.py
+-rw-r--r--   0        0        0     4252 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/args/request_model.py
+-rw-r--r--   0        0        0     5893 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/args/resolver_generators.py
+-rw-r--r--   0        0        0     2457 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/args/websocket_model.py
+-rw-r--r--   0        0        0     1235 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/helpers.py
+-rw-r--r--   0        0        0     9342 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/params.py
+-rw-r--r--   0        0        0     1083 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/__init__.py
+-rw-r--r--   0        0        0     1678 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/base.py
+-rw-r--r--   0        0        0     4460 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/bulk_parameter.py
+-rw-r--r--   0        0        0      687 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/non_parameter/__init__.py
+-rw-r--r--   0        0        0     2961 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/non_parameter/base.py
+-rw-r--r--   0        0        0      391 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/non_parameter/connection.py
+-rw-r--r--   0        0        0      328 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/non_parameter/context.py
+-rw-r--r--   0        0        0     1660 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/non_parameter/inject.py
+-rw-r--r--   0        0        0      387 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/non_parameter/request.py
+-rw-r--r--   0        0        0      394 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/non_parameter/response.py
+-rw-r--r--   0        0        0      524 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/non_parameter/session.py
+-rw-r--r--   0        0        0      386 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/non_parameter/websocket.py
+-rw-r--r--   0        0        0     9544 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/parameter.py
+-rw-r--r--   0        0        0      415 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/__init__.py
+-rw-r--r--   0        0        0      925 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/models/__init__.py
+-rw-r--r--   0        0        0     6157 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/models/base.py
+-rw-r--r--   0        0        0       50 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/models/exceptions.py
+-rw-r--r--   0        0        0     3129 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/models/file.py
+-rw-r--r--   0        0        0      691 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/models/helper.py
+-rw-r--r--   0        0        0     1952 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/models/html.py
+-rw-r--r--   0        0        0     2336 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/models/json.py
+-rw-r--r--   0        0        0     4256 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/models/route.py
+-rw-r--r--   0        0        0     2167 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/models/type_converter.py
+-rw-r--r--   0        0        0      995 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/response_types.py
+-rw-r--r--   0        0        0     1668 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/__init__.py
+-rw-r--r--   0        0        0     4546 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/base.py
+-rw-r--r--   0        0        0     1314 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/builder.py
+-rw-r--r--   0        0        0      272 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/controller/__init__.py
+-rw-r--r--   0        0        0     1175 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/controller/base.py
+-rw-r--r--   0        0        0     1881 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/controller/factory.py
+-rw-r--r--   0        0        0     1242 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/controller/route.py
+-rw-r--r--   0        0        0      190 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/controller/websocket/__init__.py
+-rw-r--r--   0        0        0     1424 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/controller/websocket/handler.py
+-rw-r--r--   0        0        0     2011 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/controller/websocket/route.py
+-rw-r--r--   0        0        0     6698 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/mount.py
+-rw-r--r--   0        0        0    10992 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/operation_definitions.py
+-rw-r--r--   0        0        0    10559 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/params.py
+-rw-r--r--   0        0        0     4569 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/route.py
+-rw-r--r--   0        0        0     3576 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/route_collections.py
+-rw-r--r--   0        0        0     3201 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/schema.py
+-rw-r--r--   0        0        0      161 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/websocket/__init__.py
+-rw-r--r--   0        0        0     5680 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/websocket/handler.py
+-rw-r--r--   0        0        0     4879 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/websocket/route.py
+-rw-r--r--   0        0        0      499 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/serializer/__init__.py
+-rw-r--r--   0        0        0     4959 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/serializer/base.py
+-rw-r--r--   0        0        0      194 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/serializer/guard.py
+-rw-r--r--   0        0        0      453 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/shortcuts.py
+-rw-r--r--   0        0        0      613 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/templating/__init__.py
+-rw-r--r--   0        0        0      472 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/templating/environment.py
+-rw-r--r--   0        0        0     1634 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/templating/loader.py
+-rw-r--r--   0        0        0     2895 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/templating/model.py
+-rw-r--r--   0        0        0     2482 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/templating/renderer.py
+-rw-r--r--   0        0        0      110 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/templating/schema.py
+-rw-r--r--   0        0        0      585 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/types.py
+-rw-r--r--   0        0        0      925 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/core/__init__.py
+-rw-r--r--   0        0        0      120 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/core/conf/__init__.py
+-rw-r--r--   0        0        0     4914 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/core/conf/app_settings_models.py
+-rw-r--r--   0        0        0     2177 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/core/conf/config.py
+-rw-r--r--   0        0        0     5122 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/core/conf/mixins.py
+-rw-r--r--   0        0        0      470 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/core/connection/__init__.py
+-rw-r--r--   0        0        0      688 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/core/connection/http.py
+-rw-r--r--   0        0        0      245 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/core/connection/websocket.py
+-rw-r--r--   0        0        0      458 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/core/context/__init__.py
+-rw-r--r--   0        0        0     1453 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/core/context/execution.py
+-rw-r--r--   0        0        0     2539 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/context/factory.py
+-rw-r--r--   0        0        0     2091 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/context/host.py
+-rw-r--r--   0        0        0     2122 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/context/http.py
+-rw-r--r--   0        0        0      817 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/context/websocket.py
+-rw-r--r--   0        0        0     1492 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/core_service_registration.py
+-rw-r--r--   0        0        0       97 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/exceptions/__init__.py
+-rw-r--r--   0        0        0     2273 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/exceptions/service.py
+-rw-r--r--   0        0        0     7616 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/factory.py
+-rw-r--r--   0        0        0      263 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/guard/__init__.py
+-rw-r--r--   0        0        0      744 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/guard/apikey.py
+-rw-r--r--   0        0        0     3318 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/guard/http.py
+-rw-r--r--   0        0        0     9463 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/main.py
+-rw-r--r--   0        0        0     1159 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/middleware/__init__.py
+-rw-r--r--   0        0        0     2576 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/middleware/di.py
+-rw-r--r--   0        0        0     2704 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/middleware/exceptions.py
+-rw-r--r--   0        0        0     2256 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/middleware/function.py
+-rw-r--r--   0        0        0      121 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/middleware/sessions.py
+-rw-r--r--   0        0        0     1095 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/middleware/versioning.py
+-rw-r--r--   0        0        0      321 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/modules/__init__.py
+-rw-r--r--   0        0        0     1287 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/modules/base.py
+-rw-r--r--   0        0        0     3139 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/modules/builder.py
+-rw-r--r--   0        0        0     5827 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/modules/config.py
+-rw-r--r--   0        0        0      787 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/modules/helper.py
+-rw-r--r--   0        0        0    10210 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/modules/ref.py
+-rw-r--r--   0        0        0       75 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/routing/__init__.py
+-rw-r--r--   0        0        0     3853 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/routing/app.py
+-rw-r--r--   0        0        0       58 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/services/__init__.py
+-rw-r--r--   0        0        0     1949 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/services/reflector.py
+-rw-r--r--   0        0        0     1718 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/staticfiles.py
+-rw-r--r--   0        0        0       67 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/templating/__init__.py
+-rw-r--r--   0        0        0     3978 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/templating/app.py
+-rw-r--r--   0        0        0      563 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/versioning/__init__.py
+-rw-r--r--   0        0        0     2526 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/versioning/base.py
+-rw-r--r--   0        0        0     6198 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/versioning/resolver.py
+-rw-r--r--   0        0        0      915 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/__init__.py
+-rw-r--r--   0        0        0      344 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/asgi_args.py
+-rw-r--r--   0        0        0     1073 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/constants.py
+-rw-r--r--   0        0        0      400 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/exceptions.py
+-rw-r--r--   0        0        0      117 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/injector/__init__.py
+-rw-r--r--   0        0        0     7647 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/injector/container.py
+-rw-r--r--   0        0        0     5268 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/injector/ellar_injector.py
+-rw-r--r--   0        0        0      845 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/providers.py
+-rw-r--r--   0        0        0     2247 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/scopes.py
+-rw-r--r--   0        0        0     4525 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/service_config.py
+-rw-r--r--   0        0        0       39 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/types.py
+-rw-r--r--   0        0        0      244 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/utils.py
+-rw-r--r--   0        0        0     2052 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/events.py
+-rw-r--r--   0        0        0      573 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/__init__.py
+-rw-r--r--   0        0        0     8069 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/builder.py
+-rw-r--r--   0        0        0      239 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/docs_generators/__init__.py
+-rw-r--r--   0        0        0      530 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/docs_generators/base.py
+-rw-r--r--   0        0        0      959 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/docs_generators/redocs.py
+-rw-r--r--   0        0        0     1025 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/docs_generators/swagger.py
+-rw-r--r--   0        0        0     2937 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/module.py
+-rw-r--r--   0        0        0    10611 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/openapi_v3.py
+-rw-r--r--   0        0        0    15879 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/route_doc_models.py
+-rw-r--r--   0        0        0      115 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/schemas/__init__.py
+-rw-r--r--   0        0        0      342 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/schemas/validation.py
+-rw-r--r--   0        0        0      702 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/templates/redocs.html
+-rw-r--r--   0        0        0      758 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/templates/swagger.html
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/py.typed
+-rw-r--r--   0        0        0      180 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/reflect/__init__.py
+-rw-r--r--   0        0        0     5356 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/reflect/_reflect.py
+-rw-r--r--   0        0        0       34 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/reflect/constants.py
+-rw-r--r--   0        0        0      238 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/reflect/contextmanager_fix.py
+-rw-r--r--   0        0        0       58 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/samples/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/samples/controllers/__init__.py
+-rw-r--r--   0        0        0      381 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/samples/controllers/home.py
+-rw-r--r--   0        0        0      211 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/samples/modules.py
+-rw-r--r--   0        0        0   155845 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/samples/static/css/bootstrap.min.css
+-rwxr-xr-x   0        0        0    25915 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/samples/static/img/EllarLogoB.png
+-rwxr-xr-x   0        0        0    36744 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/samples/static/img/EllarLogoIconOnly.png
+-rwxr-xr-x   0        0        0     3888 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/samples/static/img/Icon.svg
+-rw-r--r--   0        0        0     1312 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/samples/templates/home/index.html
+-rw-r--r--   0        0        0      596 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/socket_io/__init__.py
+-rw-r--r--   0        0        0      423 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/socket_io/adapter.py
+-rw-r--r--   0        0        0      524 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/socket_io/constants.py
+-rw-r--r--   0        0        0     1659 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/socket_io/context.py
+-rw-r--r--   0        0        0      225 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/socket_io/decorators/__init__.py
+-rw-r--r--   0        0        0      667 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/socket_io/decorators/events.py
+-rw-r--r--   0        0        0     3846 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/socket_io/decorators/gateway.py
+-rw-r--r--   0        0        0      578 2023-05-11 21:02:05.088801 ellar-0.3.8/ellar/socket_io/decorators/subscribe_message.py
+-rw-r--r--   0        0        0     2521 2023-05-11 21:02:05.088801 ellar-0.3.8/ellar/socket_io/factory.py
+-rw-r--r--   0        0        0     9918 2023-05-11 21:02:05.088801 ellar-0.3.8/ellar/socket_io/gateway.py
+-rw-r--r--   0        0        0      144 2023-05-11 21:02:05.088801 ellar-0.3.8/ellar/socket_io/model.py
+-rw-r--r--   0        0        0      465 2023-05-11 21:02:05.088801 ellar-0.3.8/ellar/socket_io/responses.py
+-rw-r--r--   0        0        0      107 2023-05-11 21:02:05.088801 ellar-0.3.8/ellar/socket_io/testing/__init__.py
+-rw-r--r--   0        0        0     1704 2023-05-11 21:02:05.088801 ellar-0.3.8/ellar/socket_io/testing/module.py
+-rw-r--r--   0        0        0      129 2023-05-11 21:02:05.088801 ellar-0.3.8/ellar/testing/__init__.py
+-rw-r--r--   0        0        0     4074 2023-05-11 21:02:05.088801 ellar-0.3.8/ellar/testing/module.py
+-rw-r--r--   0        0        0     1215 2023-05-11 21:02:05.088801 ellar-0.3.8/ellar/testing/uvicorn_server.py
+-rw-r--r--   0        0        0      509 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/__init__.py
+-rw-r--r--   0        0        0     1659 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/controllers.py
+-rw-r--r--   0        0        0     1077 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/module.py
+-rw-r--r--   0        0        0     1146 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/routers.py
+-rw-r--r--   0        0        0      629 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/schemas.py
+-rw-r--r--   0        0        0      666 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/services.py
+-rw-r--r--   0        0        0     1708 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/statics/blog/blog.css
+-rw-r--r--   0        0        0     1586 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/statics/blog/blog.rtl.css
+-rw-r--r--   0        0        0     1008 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo-white.svg
+-rw-r--r--   0        0        0     2047 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo.svg
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/tests/__init__.py
+-rw-r--r--   0        0        0     2900 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/tests/test_controllers.py
+-rw-r--r--   0        0        0     1604 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/tests/test_routers.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/tests/test_services.py
+-rw-r--r--   0        0        0      202 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/views/car/list.html
+-rw-r--r--   0        0        0      202 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/views/cat/list.html
+-rw-r--r--   0        0        0    15257 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/views/index.html
+-rw-r--r--   0        0        0      216 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/commands.py
+-rw-r--r--   0        0        0      187 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/config.py
+-rw-r--r--   0        0        0      598 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/root_module.py
+-rw-r--r--   0        0        0      954 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/server.py
+-rw-r--r--   0        0        0      134 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/tests/conftest.py
+-rw-r--r--   0        0        0      241 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/pyproject.toml
+-rw-r--r--   0        0        0      264 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/README.md
+-rw-r--r--   0        0        0      283 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/__init__.py
+-rw-r--r--   0        0        0      455 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/controllers.py
+-rw-r--r--   0        0        0     2182 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/gateways.py
+-rw-r--r--   0        0        0     1005 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/module.py
+-rw-r--r--   0        0        0      295 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/routers.py
+-rw-r--r--   0        0        0      542 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/schemas.py
+-rw-r--r--   0        0        0      179 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/services.py
+-rw-r--r--   0        0        0     3829 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/templates/events/index.html
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/tests/test_controllers.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/tests/test_routers.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/tests/test_services.py
+-rw-r--r--   0        0        0     2602 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/config.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/domain/__init__.py
+-rw-r--r--   0        0        0      480 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/root_module.py
+-rw-r--r--   0        0        0     1045 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/server.py
+-rw-r--r--   0        0        0       43 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/tests/conftest.py
+-rw-r--r--   0        0        0     3824 2023-05-11 21:02:05.088801 ellar-0.3.8/mkdocs.yml
+-rw-r--r--   0        0        0      597 2023-05-11 21:02:05.088801 ellar-0.3.8/mypy.ini
+-rw-r--r--   0        0        0     3037 2023-05-11 21:02:05.088801 ellar-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0      207 2023-05-11 21:02:05.088801 ellar-0.3.8/pytest.ini
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/__init__.py
+-rw-r--r--   0        0        0     1022 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/conftest.py
+-rw-r--r--   0        0        0      616 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/injector_module.py
+-rw-r--r--   0        0        0     5249 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/main.py
+-rw-r--r--   0        0        0       23 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/private/test.css
+-rw-r--r--   0        0        0      748 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/schema.py
+-rw-r--r--   0        0        0        4 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/statics/example.txt
+-rw-r--r--   0        0        0      160 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/templates/ellar/index.html
+-rw-r--r--   0        0        0      102 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/templates/ellar/list.html
+-rw-r--r--   0        0        0      129 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/templates/index.html
+-rw-r--r--   0        0        0      128 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/templates/list.html
+-rw-r--r--   0        0        0       65 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/templates/render_string.html
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_application/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_application/config.py
+-rw-r--r--   0        0        0     2854 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_application/sample.py
+-rw-r--r--   0        0        0     3548 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_application/test_application_factory.py
+-rw-r--r--   0        0        0    15855 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_application/test_application_functions.py
+-rw-r--r--   0        0        0    18052 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_application/test_cors.py
+-rw-r--r--   0        0        0     4284 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_application/test_replacing_app_services.py
+-rw-r--r--   0        0        0     2329 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_application/test_trusted_host.py
+-rw-r--r--   0        0        0      862 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_attribute_dict.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/__init__.py
+-rw-r--r--   0        0        0     3625 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/_test_aio_memcache.py.ellar
+-rw-r--r--   0        0        0     1893 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/pylib_mock.py
+-rw-r--r--   0        0        0     2592 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/redis_mock.py
+-rw-r--r--   0        0        0     2764 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/test_cache_decorator.py
+-rw-r--r--   0        0        0     1744 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/test_cache_many_config.py
+-rw-r--r--   0        0        0     4772 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/test_cache_service.py
+-rw-r--r--   0        0        0     4995 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/test_local_cache.py
+-rw-r--r--   0        0        0      596 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/test_module_setup.py
+-rw-r--r--   0        0        0     9973 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/test_pylibmc_cache.py
+-rw-r--r--   0        0        0     6093 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/test_redis_cache.py
+-rw-r--r--   0        0        0      577 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/test_schema.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_conf/__init__.py
+-rw-r--r--   0        0        0     5223 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_conf/test_default_conf.py
+-rw-r--r--   0        0        0     1151 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_conf/test_mixins.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_controller/__init__.py
+-rw-r--r--   0        0        0      387 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_controller/sample.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_controller/test_application_router.py
+-rw-r--r--   0        0        0     4450 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_controller/test_controller_decorator.py
+-rw-r--r--   0        0        0     2442 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_controller/test_controller_inheritance.py
+-rw-r--r--   0        0        0     2628 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_controller/test_module_router.py
+-rw-r--r--   0        0        0     7165 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_controller/test_route_collection.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/__init__.py
+-rw-r--r--   0        0        0     3360 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/test_controller.py
+-rw-r--r--   0        0        0      789 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/test_exception.py
+-rw-r--r--   0        0        0     3508 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/test_file.py
+-rw-r--r--   0        0        0     1050 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/test_guards.py
+-rw-r--r--   0        0        0     4082 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/test_html.py
+-rw-r--r--   0        0        0      554 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/test_middleware.py
+-rw-r--r--   0        0        0     2061 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/test_modules.py
+-rw-r--r--   0        0        0      915 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/test_openapi.py
+-rw-r--r--   0        0        0     1311 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/test_serializer.py
+-rw-r--r--   0        0        0      475 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/test_versioning.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_di/__init__.py
+-rw-r--r--   0        0        0     1332 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_di/examples.py
+-rw-r--r--   0        0        0     2078 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_di/test_injectable_resolving.py
+-rw-r--r--   0        0        0     6275 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_di/test_injector.py
+-rw-r--r--   0        0        0     3508 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_di/test_provider_scopes.py
+-rw-r--r--   0        0        0     3993 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_di/test_providers.py
+-rw-r--r--   0        0        0     1817 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_events.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_exceptions/__init__.py
+-rw-r--r--   0        0        0      206 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_exceptions/exception_runner.py
+-rw-r--r--   0        0        0     2562 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_exceptions/test_api_exception.py
+-rw-r--r--   0        0        0     8609 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_exceptions/test_custom_exceptions.py
+-rw-r--r--   0        0        0     1195 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_exceptions/test_error_details.py
+-rw-r--r--   0        0        0     3722 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_exceptions/test_validation_exception.py
+-rw-r--r--   0        0        0     7162 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_guard.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_helper/__init__.py
+-rw-r--r--   0        0        0      571 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_helper/test_enum.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_helper/test_importer.py
+-rw-r--r--   0        0        0      795 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_helper/test_model_field.py
+-rw-r--r--   0        0        0      298 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_helper/test_module_loading.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_middleware/__init__.py
+-rw-r--r--   0        0        0     2302 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_middleware/test_functional_middleware.py
+-rw-r--r--   0        0        0     4243 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_middleware/test_service_provider_middleware.py
+-rw-r--r--   0        0        0     2168 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_middleware/test_versioning_middleware.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_modules/__init__.py
+-rw-r--r--   0        0        0     1847 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_modules/sample.py
+-rw-r--r--   0        0        0     6760 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_modules/test_module_config.py
+-rw-r--r--   0        0        0    10084 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_modules/test_module_ref.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_openapi/__init__.py
+-rw-r--r--   0        0        0     8341 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_openapi/test_builder.py
+-rw-r--r--   0        0        0     6680 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_openapi/test_module.py
+-rw-r--r--   0        0        0    16449 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_openapi/test_open_api_route_documentation.py
+-rw-r--r--   0        0        0     5571 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_reflect.py
+-rw-r--r--   0        0        0     2154 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_reflector.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_response/__init__.py
+-rw-r--r--   0        0        0     2481 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_response/test_defined_response_model.py
+-rw-r--r--   0        0        0     4562 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_response/test_pydantic_response_model.py
+-rw-r--r--   0        0        0     3393 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_response/test_response_file.py
+-rw-r--r--   0        0        0     5063 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_response/test_response_html.py
+-rw-r--r--   0        0        0     3228 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_response/test_response_streaming.py
+-rw-r--r--   0        0        0     3902 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_response/test_response_type_definition_converter.py
+-rw-r--r--   0        0        0     3524 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_response/test_route_response_model.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/__init__.py
+-rw-r--r--   0        0        0     1126 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/sample.py
+-rw-r--r--   0        0        0     3605 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_body_schema.py
+-rw-r--r--   0        0        0     3666 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_body_schema_extra_properties.py
+-rw-r--r--   0        0        0     4142 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_body_union_schema.py
+-rw-r--r--   0        0        0     3902 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_cookie_schema.py
+-rw-r--r--   0        0        0     6854 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_extra_args.py
+-rw-r--r--   0        0        0     2346 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_form_schema.py
+-rw-r--r--   0        0        0    10018 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_formparsers.py
+-rw-r--r--   0        0        0     1282 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_forms.py
+-rw-r--r--   0        0        0     1296 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_forms_from_non_typing_sequences.py
+-rw-r--r--   0        0        0     3522 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_header_schema.py
+-rw-r--r--   0        0        0     1563 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_invalid_path_param.py
+-rw-r--r--   0        0        0     1760 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_invalid_sequence_param.py
+-rw-r--r--   0        0        0     5205 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_multi_body_errors.py
+-rw-r--r--   0        0        0     3783 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_multi_query_errors.py
+-rw-r--r--   0        0        0     9423 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_path.py
+-rw-r--r--   0        0        0     2769 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_path_with_schema.py
+-rw-r--r--   0        0        0     3333 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_put_with_no_body_schema.py
+-rw-r--r--   0        0        0     2242 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_query.py
+-rw-r--r--   0        0        0     3588 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_query_schema.py
+-rw-r--r--   0        0        0     1987 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_request.py
+-rw-r--r--   0        0        0     3415 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_route_endpoint_params.py
+-rw-r--r--   0        0        0      451 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_sample_project.py
+-rw-r--r--   0        0        0     2712 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_schema.py
+-rw-r--r--   0        0        0     6379 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_serializer.py
+-rw-r--r--   0        0        0      775 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_shortcuts.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_socket_io/__init__.py
+-rw-r--r--   0        0        0     4110 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_socket_io/sample.py
+-rw-r--r--   0        0        0      718 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_socket_io/test_decorators/test_events.py
+-rw-r--r--   0        0        0     3592 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_socket_io/test_decorators/test_gateway.py
+-rw-r--r--   0        0        0      719 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_socket_io/test_decorators/test_subcribe_message.py
+-rw-r--r--   0        0        0     8889 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_socket_io/test_operation.py
+-rw-r--r--   0        0        0    14104 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_staticfiles.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_templating/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_templating/module_statics/watever.txt
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_templating/static/watever.txt
+-rw-r--r--   0        0        0      167 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_templating/templates/watever.html
+-rw-r--r--   0        0        0     2904 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_templating/test_module_templating.py
+-rw-r--r--   0        0        0     2718 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_templating/test_renderer.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_templating/views/watever.html
+-rw-r--r--   0        0        0     2425 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_testing.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_versioning/__init__.py
+-rw-r--r--   0        0        0     1968 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_versioning/operations.py
+-rw-r--r--   0        0        0     2138 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_versioning/test_default_versioning.py
+-rw-r--r--   0        0        0     4449 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_versioning/test_default_versioning_for_controllers.py
+-rw-r--r--   0        0        0     4475 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_versioning/test_header_versioning.py
+-rw-r--r--   0        0        0     7820 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_versioning/test_header_versioning_controller.py
+-rw-r--r--   0        0        0     3823 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_versioning/test_host_versioning.py
+-rw-r--r--   0        0        0     3227 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_versioning/test_query_versioning.py
+-rw-r--r--   0        0        0     2865 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_versioning/test_url_versioning.py
+-rw-r--r--   0        0        0    17496 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_websocket.py
+-rw-r--r--   0        0        0    11075 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_websocket_handler.py
+-rw-r--r--   0        0        0    14822 1970-01-01 00:00:00.000000 ellar-0.3.8/PKG-INFO
```

### Comparing `ellar-0.3.6/.github/workflows/publish.yml` & `ellar-0.3.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/.github/workflows/test.yml` & `ellar-0.3.8/.github/workflows/test.yml`

 * *Files 0% similar despite different names*

```diff
@@ -18,8 +18,8 @@
       - name: Install Flit
         run: pip install flit
       - name: Install Dependencies
         run: flit install --symlink
       - name: Test
         run: make test-cov
       - name: Coverage
-        uses: codecov/codecov-action@v3.1.1
+        uses: codecov/codecov-action@v3.1.3
```

### Comparing `ellar-0.3.6/.github/workflows/test_full.yml` & `ellar-0.3.8/.github/workflows/test_full.yml`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/.gitignore` & `ellar-0.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/.pre-commit-config.yaml` & `ellar-0.3.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/LICENSE` & `ellar-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/Makefile` & `ellar-0.3.8/Makefile`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/README.md` & `ellar-0.3.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,110 +1,107 @@
 <p align="center">
-  <a href="#" target="blank"><img src="docs/img/EllarLogoIconOnly.png" width="200" alt="Ellar Logo" /></a>
+  <a href="#" target="blank"><img src="docs/img/EllarLogoB.png" width="200" alt="Ellar Logo" /></a>
 </p>
 
 <p align="center"> Ellar - Python ASGI web framework for building fast, efficient and scalable RESTAPIs and server-side application. </p>
 
 ![Test](https://github.com/eadwinCode/ellar/actions/workflows/test_full.yml/badge.svg)
 ![Coverage](https://img.shields.io/codecov/c/github/eadwinCode/ellar)
 [![PyPI version](https://badge.fury.io/py/ellar.svg)](https://badge.fury.io/py/ellar)
 [![PyPI version](https://img.shields.io/pypi/v/ellar.svg)](https://pypi.python.org/pypi/ellar)
 [![PyPI version](https://img.shields.io/pypi/pyversions/ellar.svg)](https://pypi.python.org/pypi/ellar)
 
-## Introduction
+## **Introduction**
 
 Ellar is a lightweight ASGI framework for building efficient and scalable server-side python applications.
 It supports both OOP (Object-Oriented Programming) and FP (Functional Programming)
 
 Ellar is based on [Starlette (ASGI toolkit)](https://www.starlette.io/), a lightweight ASGI framework/toolkit well-suited for developing asynchronous web services with Python. 
-While Ellar provides a high level of abstraction on top of Starlette, it still incorporates some of its features, as well as those of FastAPI. 
-If you are familiar with these frameworks, you will find it easy to understand and use Ellar.
 
-## Features Summary
+## **Features Summary**
 
 - **Easy to Use**: Ellar has a simple and intuitive API that makes it easy to get started with building a fast and scalable web applications or web APIs in Python.
 - **Dependency Injection (DI)**: It comes with DI system makes it easy to manage dependencies and reduce coupling between components.
 - **Pydantic Integration**: It is properly integrated with Pydantic, a popular Python library for data validation, to ensure that input data is valid.
 - **Templating with Jinja2**: Ellar provides built-in support for Jinja2 templates, making it easy to create dynamic web pages.
 - **OpenAPI Documentation**: It comes with built-in support for OpenAPI documentation, making it easy to generate `Swagger` or `ReDoc` documentation for your API. And more can be added with ease if necessary.
 - **Controller (MVC) Architecture**: Ellar's controller architecture follows the Model-View-Controller (MVC) pattern, making it easy to organize your code.
 - **Guards for Authentication and Authorization**: It provides built-in support for guards, allowing you to easily implement authentication and authorization in your application.
 - **Modularity**: Ellar follows a modular architecture inspired by NestJS, making it easy to organize your code into reusable modules.
 - **Asynchronous programming**: It allows you to takes advantage of Python's `async/await` feature to write efficient and fast code that can handle large numbers of concurrent requests
 
-## Dependencies
+## **Dependencies**
 - Python >= 3.7
 - Starlette
 - Injector
 - Pydantic
 
-## Installation
+## **Installation**
 ### Poetry Installation
 For [Poetry](https://python-poetry.org/) usages
 
 ```shell
 poetry add ellar-cli
 ```
 
 ### Pip Installation
 For normal pip installation
 ```shell
 pip install ellar-cli
 ```
 
-## Create a project
+## Creating a project
 To create an ellar project, you need to have a `pyproject.toml` available on your root directory.
 This is necessary for ellar to store some `metadata` about your project. 
 
-### Create a project
 For Pip Users, you need to create `pyproject.toml` file
 ```shell
 ellar new carsite
 ```
 If you are using `Poetry`, at your project root directory with `pyproject.toml`,
 run the ellar create project cli command,
 ```shell
 ellar create-project carsite
 ```
 
-## Run your project
+## **Run your project**
 Ellar runs [UVICORN - ASGI Server](https://www.uvicorn.org/) under the hood.
 ```shell
 ellar runserver --reload
 ```
 `--reload` is to watch for file changes
 
 Now go to [http://127.0.0.1:8000](http://127.0.0.1:8000)
 ![Swagger UI](docs/img/ellar_framework.png)
 
 For more info on Ellar CLI, click [here](https://github.com/eadwinCode/ellar-cli)
 
-## Create a project module
+## **Adding a project module**
 A project module is a project app defining a group of controllers or services including templates and static files.
 So, now we have a project created, lets add an app to the project.
 ```shell
 ellar create-module car
 ```
 
-## Add Schema
+## **Add Schema**
 In `car/schema.py`, lets add some serializer for car input and output data
 ```python
-from ellar.serializer import Serializer
+from ellar.common import Serializer
 
 class CarSerializer(Serializer):
     name: str
     model: str
     brand: str
 
 
 class RetrieveCarSerializer(CarSerializer):
     pk: str
 ```
 
-## Add Services
+## **Add Services**
 In `car/services.py`, lets create a dummy repository `CarDummyDB` to manage our car data.
 ```python
 import typing as t
 import uuid
 from ellar.di import injectable, singleton_scope
 
 
@@ -149,22 +146,21 @@
             return self._data[idx]
 
     def remove(self, car_id: str) -> t.Optional["CarDummyDB.CarDummyDBItem"]:
         idx = self._data.index(car_id)
         if idx >= 0:
             return self._data.pop(idx)
 ```
-## Add Controller
+## **Add Controller**
 In `car/controllers.py`, lets create `CarController`
 
 ```python
 import typing as t
-from ellar.common import Controller, delete, get, put, post
-from ellar.core import ControllerBase
-from ellar.core.exceptions import NotFound
+from ellar.common import Controller, delete, get, put, post, ControllerBase
+from ellar.common.exceptions import NotFound
 from .schemas import CarSerializer, RetrieveCarSerializer
 from .services import CarDummyDB
 
 
 @Controller
 class CarController(ControllerBase):
     def __init__(self, db: CarDummyDB) -> None:
@@ -197,15 +193,15 @@
         return 204, {}
 
     @get("/", response={200: t.List[RetrieveCarSerializer]})
     async def list(self):
         return self.car_db.list()
 
 ```
-## Register Service and Controller
+## **Register Service and Controller**
 In `car/module.py`, lets register `CarController` and `CarDummyDB`
 
 ```python
 from ellar.common import Module
 from ellar.core import ModuleBase
 from ellar.di import Container
 
@@ -221,40 +217,39 @@
 class CarModule(ModuleBase):
     def register_providers(self, container: Container) -> None:
         # for more complicated provider registrations
         # container.register_instance(...)
         pass
 ```
 
-## Registering Module
+## **Registering Module**
 Ellar is not aware of `CarModule` yet, so we need to add it to the `modules` list of `ApplicationModule` at the `carsite/root_module.py`.
 ```python
-from ellar.common import Module, exception_handler
-from ellar.core import IHostContext, ModuleBase
-from ellar.core.response import JSONResponse, Response
+from ellar.common import Module, exception_handler, JSONResponse, Response, IHostContext
+from ellar.core import ModuleBase
 
 from ellar.samples.modules import HomeModule
 from .apps.car.module import CarModule
 
 
 @Module(modules=[HomeModule, CarModule])
 class ApplicationModule(ModuleBase):
     @exception_handler(404)
     def exception_404_handler(cls, context: IHostContext, exc: Exception) -> Response:
         return JSONResponse(dict(detail="Resource not found."))
 
 ```
-## Enabling OpenAPI Docs
+## **Enabling OpenAPI Docs**
 To start up openapi, we need to go back to project folder in the `server.py`
 then add the following below.
 ```python
 import os
 
 from ellar.constants import ELLAR_CONFIG_MODULE
-from ellar.core.factory import AppFactory
+from ellar.core import AppFactory
 from ellar.openapi import OpenAPIDocumentModule, OpenAPIDocumentBuilder, SwaggerDocumentGenerator
 from .root_module import ApplicationModule
 
 application = AppFactory.create_from_app_module(
     ApplicationModule,
     config_module=os.environ.get(
         ELLAR_CONFIG_MODULE, "carsite.config:DevelopmentConfig"
@@ -276,15 +271,15 @@
 application.install_module(module)
 ```
 
 Now we can test our API at [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs#/)
 Please ensure your server is running
 ![Swagger UI](docs/img/car_api.png)
 
-## HTML Templating
+## **HTML Templating**
 Ellar has built-in support for Jinja2, which is a popular template engine for HTML. This feature allows for easy and efficient HTML templating similar to that of Flask. Jinja2 can be used to create reusable templates, and to insert dynamic data into HTML pages. It also has support for template inheritance, control structures, and other useful features that can help to simplify and streamline the process of creating HTML templates.
 
 ```html
 <html>
   <body>
     <ul>
       {% for item in items %}
```

### Comparing `ellar-0.3.6/docs/basics/execution-context.md` & `ellar-0.3.8/docs/basics/execution-context.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 The `HostContext` class provides a wrapper around `ASGI` app parameters (`scope`, `receive` and `send`) and provides some methods that allows you choosing the appropriate context(e.g., HTTP or WebSockets).
 
 For example, the `catch()` method of an **exception handlers** is called with an IHostContext.
 
 ```python
 # project_name/apps/custom_exceptions.py
 import typing as t
-from ellar.core.exceptions import IExceptionHandler
-from ellar.core.context import IHostContext
-from starlette.responses import Response
+from ellar.common import IExceptionHandler, IHostContext, Response
 
 class MyCustomException(Exception):
     pass
 
 
 class MyCustomExceptionHandler(IExceptionHandler):
     exception_type_or_code = MyCustomException
@@ -143,15 +141,16 @@
 
 ## **ExecutionContext Class**
 `ExecutionContext` extends `HostContext` and provides extra information like `Controller` class and controller `function` 
 that will handler the current request.
 
 ```python
 import typing
-from ellar.core import HostContext, ControllerBase
+from ellar.common import ControllerBase
+from ellar.core import HostContext
 
 
 class ExecutionContext(HostContext):
     # Returns the type of the controller class which the current handler belongs to.
     def get_class(self) -> typing.Type[ControllerBase]:
         pass
     
@@ -192,16 +191,15 @@
 ## **Reflector and Metadata**
 Ellar provides the ability to attach **custom metadata** to route handlers through the `@set_metadata()` decorator. 
 We can then access this metadata from within our class to make certain decisions.
 
 ```python
 # project_name/apps/cars/controllers.py
 
-from ellar.common import Body, Controller, post, set_metadata
-from ellar.core import ControllerBase
+from ellar.common import Body, Controller, post, set_metadata, ControllerBase
 from .schemas import CreateCarSerializer
 
 
 @Controller('/car')
 class CarController(ControllerBase):
     @post()
     @set_metadata('role', ['admin'])
@@ -214,16 +212,15 @@
 With the construction above, we attached the `roles` metadata (roles is a metadata key and ['admin'] is the associated value) 
 to the `create()` method. While this works, it's not good practice to use `@set_metadata()` directly in your routes. 
 Instead, create your own decorators, as shown below:
 
 ```python
 # project_name/apps/cars/controllers.py
 import typing
-from ellar.common import Body, Controller, post, set_metadata
-from ellar.core import ControllerBase
+from ellar.common import Body, Controller, post, set_metadata, ControllerBase
 from .schemas import CreateCarSerializer
 
 
 def roles(*_roles: str) -> typing.Callable:
     return set_metadata('roles', list(_roles))
 
 
@@ -242,16 +239,16 @@
 
 To access the route's role(s) (custom metadata), we'll use the `Reflector` helper class, which is provided out of the box by the framework. 
 `Reflector` can be injected into a class in the normal way:
 
 ```python
 # project_name/apps/cars/guards.py
 from ellar.di import injectable
-from ellar.core import GuardCanActivate, IExecutionContext
-from ellar.services import Reflector
+from ellar.common import GuardCanActivate, IExecutionContext
+from ellar.core.services import Reflector
 
 
 @injectable()
 class RoleGuard(GuardCanActivate):
     def __init__(self, reflector: Reflector):
         self.reflector = reflector
 
@@ -265,16 +262,15 @@
 ```
 
 Next, we apply the `RoleGuard` to `CarController`
 
 ```python
 # project_name/apps/cars/controllers.py
 import typing
-from ellar.common import Body, Controller, post, set_metadata, Guards
-from ellar.core import ControllerBase
+from ellar.common import Body, Controller, post, set_metadata, Guards, ControllerBase
 from .schemas import CreateCarSerializer
 from .guards import RoleGuard
 
 def roles(*_roles: str) -> typing.Callable:
     return set_metadata('roles', list(_roles))
```

### Comparing `ellar-0.3.6/docs/basics/testing.md` & `ellar-0.3.8/docs/basics/testing.md`

 * *Files 2% similar despite different names*

```diff
@@ -151,17 +151,16 @@
 ```
 We this, anywhere `CarRepository` is needed, a `MockCarRepository()` instance will be applied.
 
 In same way, we can override `Guards` used in controllers during testing. For example, lets assume `CarController` has a guard `JWTGuard`
 
 ```python
 import typing
-from ellar.compatible.dict import AttributeDict
-from ellar.common import Guards, Controller
-from ellar.core import ControllerBase
+from ellar.common.compatible import AttributeDict
+from ellar.common import Guards, Controller, ControllerBase
 from ellar.core.guard import HttpBearerAuth
 from ellar.di import injectable
 
 
 @injectable()
 class JWTGuard(HttpBearerAuth):
     async def authenticate(self, connection, credentials) -> typing.Any:
@@ -310,27 +309,30 @@
 In example above, `TestClient` needs an `ASGI` Callable. It exposes the same interface as any other `httpx` session. 
 In particular, note that the calls to make a request are just standard function calls, not awaitable.
 
 Let's see how we can use `TestClient` in writing e2e testing for `CarController` and `CarRepository`.
 
 ```python
 # project_name/car/tests/test_controllers.py
-from unittest.mock import patch
 from ellar.di import ProviderConfig
 from ellar.testing import Test, TestClient
 from project_name.apps.car.controllers import CarController
-from project_name.apps.car.schemas import CreateCarSerializer, CarListFilter
 from project_name.apps.car.services import CarRepository
 
 
+class MockCarRepository(CarRepository):
+    def get_all(self):
+        return [dict(id=2, model='CLS',name='Mercedes', year=2023)]
+
+
 class TestCarControllerE2E:
     def setup(self):
         test_module = Test.create_test_module(
             controllers=[CarController,],
-            providers=[ProviderConfig(CarRepository, use_class=CarRepository)],
+            providers=[ProviderConfig(CarRepository, use_class=MockCarRepository)],
             config_module=dict(
                 REDIRECT_SLASHES=True
             )
         )
         self.client: TestClient = test_module.get_test_client()
 
     def test_create_action(self):
@@ -342,16 +344,15 @@
             "id": "1",
             "message": "This action adds a new car",
             "model": "CLS",
             "name": "Mercedes",
             "year": 2022,
         }
 
-    @patch.object(CarRepository, 'get_all', return_value=[dict(id=2, model='CLS',name='Mercedes', year=2023)])
-    def test_get_all_action(self, mock_get_all):
+    def test_get_all_action(self):
         res = self.client.get('/car?offset=0&limit=10')
         assert res.status_code == 200
         assert res.json() == {
             'cars': [
                 {
                     'id': 2,
                     'model': 'CLS',
```

### Comparing `ellar-0.3.6/docs/basics/versioning.md` & `ellar-0.3.8/docs/basics/versioning.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 Accept: application/json
 ```
 
 To enable **URL Versioning** for your application, do the following:
 ```python
 # project_name/server.py
 import os
-from ellar.constants import ELLAR_CONFIG_MODULE
+from ellar.common.constants import ELLAR_CONFIG_MODULE
 from ellar.core.factory import AppFactory
 from ellar.core.versioning import VersioningSchemes
 from .root_module import ApplicationModule
 
 application = AppFactory.create_from_app_module(
     ApplicationModule,
     config_module=os.environ.get(
@@ -51,15 +51,15 @@
 Accept: application/json; version=1
 ```
 
 To enable **Header Versioning** for your application, do the following:
 ```python
 # project_name/server.py
 import os
-from ellar.constants import ELLAR_CONFIG_MODULE
+from ellar.common.constants import ELLAR_CONFIG_MODULE
 from ellar.core.factory import AppFactory
 from ellar.core.versioning import VersioningSchemes
 from .root_module import ApplicationModule
 
 application = AppFactory.create_from_app_module(
     ApplicationModule,
     config_module=os.environ.get(
@@ -106,15 +106,15 @@
 Accept: application/json
 ```
 
 To enable **Query Versioning** for your application, do the following:
 ```python
 # project_name/server.py
 import os
-from ellar.constants import ELLAR_CONFIG_MODULE
+from ellar.common.constants import ELLAR_CONFIG_MODULE
 from ellar.core.factory import AppFactory
 from ellar.core.versioning import VersioningSchemes
 from .root_module import ApplicationModule
 
 application = AppFactory.create_from_app_module(
     ApplicationModule,
     config_module=os.environ.get(
@@ -139,15 +139,15 @@
 Accept: application/json
 ```
 
 To enable **Host Versioning** for your application, do the following:
 ```python
 # project_name/server.py
 import os
-from ellar.constants import ELLAR_CONFIG_MODULE
+from ellar.common.constants import ELLAR_CONFIG_MODULE
 from ellar.core.factory import AppFactory
 from ellar.core.versioning import VersioningSchemes
 from .root_module import ApplicationModule
 
 application = AppFactory.create_from_app_module(
     ApplicationModule,
     config_module=os.environ.get(
```

### Comparing `ellar-0.3.6/docs/caching.md` & `ellar-0.3.8/docs/caching.md`

 * *Files 0% similar despite different names*

```diff
@@ -453,15 +453,15 @@
 The `make_key_callback` function takes an `ExecutionContext` instance (which contains information about the request context) and the `key_prefix` value as input, and should return the custom cache key to use.
 
 Here's an example of how to use a custom `make_key_callback` function with the cache decorator:
 === "Synchronous Route Function"
     ```python
     from ellar.common import get, cache
     from ellar.core import ExecutionContext
-    from ellar.helper import get_name
+    from ellar.common.helper import get_name
     
     def make_key_function(ctx: ExecutionContext, key_prefix: str) -> str:
         function_name = get_name(ctx.get_handler())
         return "%s:%s:%s" % (function_name, key_prefix, ctx.switch_to_http_connection().get_client().url)
     
     ...
     @get("/my_endpoint")
@@ -473,15 +473,15 @@
     ...
     ```
 === "Asynchronous Route Function"
     
     ```python
     from ellar.common import get, cache
     from ellar.core import ExecutionContext
-    from ellar.helper import get_name
+    from ellar.common.helper import get_name
     
     def make_key_function(ctx: ExecutionContext, key_prefix: str) -> str:
         function_name = get_name(ctx.get_handler())
         return "%s:%s:%s" % (function_name, key_prefix, ctx.switch_to_http_connection().get_client().url)
     
     ...
     @get("/my_endpoint")
```

### Comparing `ellar-0.3.6/docs/commands/command-grouping.md` & `ellar-0.3.8/docs/commands/command-grouping.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/commands/create-module-command.md` & `ellar-0.3.8/docs/commands/create-module-command.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/commands/custom-commands.md` & `ellar-0.3.8/docs/commands/custom-commands.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/commands/index.md` & `ellar-0.3.8/docs/commands/index.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/commands/new-command.md` & `ellar-0.3.8/docs/commands/new-command.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/commands/runserver-command.md` & `ellar-0.3.8/docs/commands/runserver-command.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/configurations.md` & `ellar-0.3.8/docs/configurations.md`

 * *Files 5% similar despite different names*

```diff
@@ -28,22 +28,22 @@
 
 A boolean that turns on/off injector `auto_bind` property.
 
 When turned on, `injector` can automatically bind to missing types as `singleton` at the point of resolving object dependencies.
 And when turned off, missing types will raise an `UnsatisfiedRequirement` exception.
 
 ### **DEFAULT_JSON_CLASS**
-Default: `JSONResponse` - (`starlette.response.JSONResponse`)
+Default: `JSONResponse` - (`starlette.common.JSONResponse`)
 
 **DEFAULT_JSON_CLASS** is used when sending JSON response to the client.
 
 There are other options for JSON available in Ellar:
 
-- **UJSONResponse**(`ellar.core.response.UJSONResponse`):  renders JSON response using [ujson](https://pypi.python.org/pypi/ujson). 
-- **ORJSONResponse**(`ellar.core.response.ORJSONResponse`):  renders JSON response using [orjson](https://pypi.org/project/orjson/). 
+- **UJSONResponse**(`ellar.common.UJSONResponse`):  renders JSON response using [ujson](https://pypi.python.org/pypi/ujson). 
+- **ORJSONResponse**(`ellar.common.ORJSONResponse`):  renders JSON response using [orjson](https://pypi.org/project/orjson/). 
 
 ### **JINJA_TEMPLATES_OPTIONS**
 Default: `{}`
 
 Default is an empty dictionary object. It defines options used when creating `Jinja2` Environment for templating.
 
 Different keys available:
@@ -148,18 +148,18 @@
 
 ### **DEFAULT_NOT_FOUND_HANDLER**
 Default: `not_found` (`not_found(scope: TScope, receive: TReceive, send: TSend)`)
 
 Default is an ASGI function. **DEFAULT_NOT_FOUND_HANDLER** is used by the application router as a callback function to a resource not found.
 
 ```python
-from ellar.types import TScope, TReceive, TSend
+from ellar.common.types import TScope, TReceive, TSend
 from starlette.exceptions import HTTPException as StarletteHTTPException
 from starlette.websockets import WebSocketClose
-from ellar.core.response import PlainTextResponse
+from ellar.common import PlainTextResponse
 
 
 async def _not_found(scope: TScope, receive: TReceive, send: TSend) -> None:
     if scope["type"] == "websocket":
         websocket_close = WebSocketClose()
         await websocket_close(scope, receive, send)
         return
```

### Comparing `ellar-0.3.6/docs/custom-setup.md` & `ellar-0.3.8/docs/custom-setup.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/handling-response/response-model.md` & `ellar-0.3.8/docs/handling-response/response-model.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 
 Each route handler has key-value pair of status codes and a response model. 
 This response model holds information on the type of response to be returned.
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.serializer import Serializer
-from ellar.common import Controller, get
-from ellar.core import ControllerBase
+from ellar.common import Controller, get, Serializer, ControllerBase
 
 class UserSchema(Serializer):
     username: str
     email: str = None
     first_name: str = None
     last_name: str = None
 
@@ -26,16 +24,16 @@
 
 During route response computation, the `me` route handler response will evaluate to a
 `JSONResponseModel` with `UserSchema` as content validation schema.
 
 The resulting route responses will be:
 
 ```python
-from ellar.serializer import Serializer
-from ellar.core.response.model import JSONResponseModel
+from ellar.common import Serializer
+from ellar.common.responses.models import JSONResponseModel
 
 
 class UserSchema(Serializer):
     username: str
     email: str = None
     first_name: str = None
     last_name: str = None
@@ -69,18 +67,15 @@
 When you use a `Response` class as response, a `ResponseModel` is used and the `response_type` is replaced with applied response class.
 
 For example:
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.common import Controller, get
-from ellar.core import ControllerBase
-from starlette.responses import PlainTextResponse
-from ellar.serializer import Serializer
+from ellar.common import Controller, get, ControllerBase,PlainTextResponse, Serializer
 
 
 class UserSchema(Serializer):
     username: str
     email: str = None
     first_name: str = None
     last_name: str = None
@@ -91,30 +86,29 @@
     @get("/me", response={200: PlainTextResponse, 201: UserSchema})
     def me(self):
         return "some text response."
 ```
 This will be translated to:
 
 ```python
-from ellar.core.response.model import ResponseModel, JSONResponseModel
-from starlette.responses import PlainTextResponse
+from ellar.common.responses.models import ResponseModel, JSONResponseModel
+from ellar.common import PlainTextResponse
 
 response = {200: ResponseModel(response_type=PlainTextResponse), 201: JSONResponseModel(model_field_or_schema=UserSchema)}
 ```
 
 ## Response Model Properties
 
 All response model follows `IResponseModel` contract.
 
 ```python
 import typing as t
 
 from pydantic.fields import ModelField
-from ellar.core.context import IExecutionContext
-from ellar.core.response import Response
+from ellar.common import IExecutionContext, Response
 
 
 class IResponseModel:
     media_type: str
     description: str
     get_model_field: t.Callable[..., t.Optional[t.Union[ModelField, t.Any]]]
     create_response: t.Callable[[IExecutionContext, t.Any], Response]
@@ -193,18 +187,16 @@
 
 Lets create a new JSON response model.
 
 ```python
 # project_name/apps/items/controllers.py
 
 import typing as t
-from ellar.common import Controller, get
-from ellar.core import ControllerBase
-from ellar.core.response.model.base import ResponseModel
-from ellar.core.response import JSONResponse
+from ellar.common import Controller, get, ControllerBase, JSONResponse
+from ellar.common.responses.models import ResponseModel
 from dataclasses import dataclass
 
 
 @dataclass
 class NoteSchema:
     id: t.Union[int, None]
     text: str
```

### Comparing `ellar-0.3.6/docs/handling-response/response.md` & `ellar-0.3.8/docs/handling-response/response.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ## Introduction
 The `Serializer` class in the Ellar, is a custom class based on `pydantic` models, which provides additional functionality specific to Ellar's requirements.
 
 To use `Serializer` in Ellar, you simply need to create a class that inherits from `Serializer` and define your data model using pydantic fields. 
 Here's an example of how you could define a serializer class for a user model:
 
 ```python
-from ellar.serializer import Serializer
+from ellar.common import Serializer
 
 class UserSerializer(Serializer):
     name: str
     email: str
     age: int
 
 ```
@@ -23,17 +23,15 @@
 
 The response schema is defined on the HTTP method decorator.
 
 For example:
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.serializer import Serializer
-from ellar.common import Controller, get
-from ellar.core import ControllerBase
+from ellar.common import Controller, get, Serializer, ControllerBase
 
 # Define a User class with username, email, first_name, and last_name attributes
 class User:
     def __init__(self, username: str, email:str=None, first_name:str=None, last_name:str=None) -> None:
         self.username = username
         self.email = email
         self.first_name = first_name
@@ -76,15 +74,15 @@
 ## Using Dataclass as Response Schema
 We can utilize the `dataclasses` feature as a response schema by utilizing the `DataclassSerializer` a base class. 
 
 For instance, we can convert the `UserSchema` to a dataclass by defining `UserDataclass` as follows:
 
 ```python
 from dataclasses import dataclass
-from ellar.serializer import DataclassSerializer
+from ellar.common import DataclassSerializer
 
 
 @dataclass
 class UserDataclass(DataclassSerializer):
     username: str
     email: str = None
     first_name: str = None
@@ -97,17 +95,15 @@
 ### Multiple Response Types
 
 The `response` parameter takes different shape. Let's see how to return a different response if the user is not authenticated.
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.serializer import Serializer
-from ellar.common import Controller, get
-from ellar.core import ControllerBase
+from ellar.common import Controller, get, ControllerBase, Serializer
 
 class User:
     def __init__(self, username: str, email:str=None, first_name:str=None, last_name:str=None) -> None:
         self.username = username
         self.email = email
         self.first_name = first_name
         self.last_name = last_name
@@ -163,17 +159,15 @@
 ## Using Response Type/Object As Response
 
 You can use `Response` type to change the format of data returned from endpoint functions.
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.common import Controller, get
-from ellar.core import ControllerBase
-from starlette.responses import PlainTextResponse
+from ellar.common import Controller, get, ControllerBase, PlainTextResponse
 
 
 @Controller
 class ItemsController(ControllerBase):
     @get("/me", response=PlainTextResponse)
     def me(self):
         return "some text response."
@@ -181,18 +175,15 @@
 ```
 
 Also, we can return response object from endpoint functions, and it will override initial `response` declared before.
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.serializer import Serializer
-from ellar.common import Controller, get
-from ellar.core import ControllerBase
-from starlette.responses import PlainTextResponse
+from ellar.common import Controller, get, Serializer, ControllerBase, PlainTextResponse
 
 class UserSchema(Serializer):
     username: str
     email: str = None
     first_name: str = None
     last_name: str = None
```

### Comparing `ellar-0.3.6/docs/img/EllarLogoB.png` & `ellar-0.3.8/docs/img/EllarLogoB.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/EllarLogoIconOnly.png` & `ellar-0.3.8/docs/img/EllarLogoIconOnly.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/EllarLogoW.png` & `ellar-0.3.8/docs/img/EllarLogoW.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/Icon.svg` & `ellar-0.3.8/docs/img/Icon.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/Logo.svg` & `ellar-0.3.8/docs/img/Logo.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/ModuleDescription.png` & `ellar-0.3.8/docs/img/ModuleDescription.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/body-schema-doc.png` & `ellar-0.3.8/docs/img/body-schema-doc.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/body-schema-doc2.png` & `ellar-0.3.8/docs/img/body-schema-doc2.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/body-schema-doc3.png` & `ellar-0.3.8/docs/img/body-schema-doc3.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/car_api.png` & `ellar-0.3.8/docs/img/car_api.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/car_controller.gif` & `ellar-0.3.8/docs/img/car_controller.gif`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/controller_description.png` & `ellar-0.3.8/docs/img/controller_description.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/create-car-schema.png` & `ellar-0.3.8/docs/img/create-car-schema.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/create-dog-schema.png` & `ellar-0.3.8/docs/img/create-dog-schema.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/ellar_demo.gif` & `ellar-0.3.8/docs/img/ellar_demo.gif`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/ellar_framework.png` & `ellar-0.3.8/docs/img/ellar_framework.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/enum_docs_swagger.png` & `ellar-0.3.8/docs/img/enum_docs_swagger.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/event_docs_swagger.png` & `ellar-0.3.8/docs/img/event_docs_swagger.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/form-schema-doc.png` & `ellar-0.3.8/docs/img/form-schema-doc.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/json_api_response_model.png` & `ellar-0.3.8/docs/img/json_api_response_model.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/math_router.png` & `ellar-0.3.8/docs/img/math_router.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/math_router_with_request_object.png` & `ellar-0.3.8/docs/img/math_router_with_request_object.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/middleware.png` & `ellar-0.3.8/docs/img/middleware.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/query_filter_swagger.png` & `ellar-0.3.8/docs/img/query_filter_swagger.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/img/response_description.png` & `ellar-0.3.8/docs/img/response_description.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/index.md` & `ellar-0.3.8/docs/index.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,51 @@
+# **[ellar](#introduction)**
 <p align="center">
-  <a href="#" target="blank"><img src="img/EllarLogoIconOnly.png" width="200" alt="Ellar Logo" /></a>
+  <a href="#" target="blank"><img src="img/EllarLogoB.png" width="200" alt="Ellar Logo" /></a>
 </p>
 
 <p align="center"> Ellar - Python ASGI web framework for building fast, efficient and scalable RESTAPIs and server-side application. </p>
 
 ![Test](https://github.com/eadwinCode/ellar/actions/workflows/test_full.yml/badge.svg)
 ![Coverage](https://img.shields.io/codecov/c/github/eadwinCode/ellar)
 [![PyPI version](https://badge.fury.io/py/ellar.svg)](https://badge.fury.io/py/ellar)
 [![PyPI version](https://img.shields.io/pypi/v/ellar.svg)](https://pypi.python.org/pypi/ellar)
 [![PyPI version](https://img.shields.io/pypi/pyversions/ellar.svg)](https://pypi.python.org/pypi/ellar)
 
 ---
-## Introduction
+## **Introduction**
 Ellar is a lightweight ASGI framework for building efficient and scalable server-side python applications.
 It supports both OOP (Object-Oriented Programming) and FP (Functional Programming)
 
-Ellar is based on [Starlette (ASGI toolkit)](https://www.starlette.io/), a lightweight ASGI framework/toolkit well-suited for developing asynchronous web services in Python. 
-And while Ellar provides a high level of abstraction on top of Starlette, it still incorporates some of its features, as well as those of FastAPI. 
-If you are familiar with these frameworks, you will find it easy to understand and use Ellar.
+Ellar is also a higher level of abstraction of [Starlette (ASGI toolkit)](https://www.starlette.io/), a lightweight ASGI framework/toolkit well-suited for developing asynchronous web services in Python.
 
-## Inspiration
-Ellar was deeply influenced by [NestJS](https://docs.nestjs.com/) for its ease of use and ability to handle complex project structures and applications. 
-Additionally, it took some concepts from [FastAPI](https://fastapi.tiangolo.com/) in terms of request parameter handling and data serialization with Pydantic. 
+## **Inspiration**
+Ellar was deeply influenced by [NestJS](https://docs.nestjs.com/) for its ease of use, project structures and patterns that aids in building small or complex project applications.
+Also, Ellar took some concepts from [FastAPI](https://fastapi.tiangolo.com/) in terms of request parameter handling and data serialization with Pydantic. 
 
-With that said, the objective of Ellar is to offer a high level of abstraction in its framework APIs, along with a well-structured project setup, an object-oriented approach to web application design, 
-the ability to adapt to any desired software architecture, and ultimately, speedy request handling.
+The objective of Ellar is to provide a high level of abstracted interface to the web, along with a well-structured project setup, give room for object-oriented approach to web application design, 
+allow you chose your desired application architecture, and ultimately, deliver speedy handling to requests.
 
+As developers, we never know how big a project can become or evolve over time but following some design patterns and architecture makes it easier to build a more testable and maintainable application.
 
-## Features Summary
+
+
+## **Features Summary**
 
 - **Easy to Use**: Ellar has a simple and intuitive API that makes it easy to get started with building a fast and scalable web applications or web APIs with Python.
 - **Dependency Injection (DI)**: It comes with DI system makes it easy to manage dependencies and reduce coupling between components.
 - **Pydantic Integration**: It is properly integrated with Pydantic, a popular Python library for data validation, to ensure that input data is valid.
 - **Templating with Jinja2**: Ellar provides built-in support for Jinja2 templates, making it easy to create dynamic web pages.
 - **OpenAPI Documentation**: It comes with built-in support for OpenAPI documentation, making it easy to generate `Swagger` or `ReDoc` documentation for your API. And more can be added with ease if necessary.
 - **Controller (MVC) Architecture**: Ellar's controller architecture follows the Model-View-Controller (MVC) pattern, making it easy to organize your code.
 - **Guards for Authentication and Authorization**: It provides built-in support for guards, allowing you to easily implement authentication and authorization in your application.
 - **Modularity**: Ellar follows a modular architecture inspired by NestJS, making it easy to organize your code into reusable modules.
 - **Asynchronous programming**: It allows you to takes advantage of Python's `async/await` feature to write efficient and fast code that can handle large numbers of concurrent requests
 
-## Installation
+## **Installation**
 To get started, you need to scaffold a project using [Ellar-CLI](https://eadwincode.github.io/ellar-cli/) toolkit. This is recommended for a first-time user.
 The scaffolded project is more like a guide to project setup.
 
 ```shell
 $(venv) pip install ellar
 ```
 
@@ -57,20 +59,20 @@
 ```shell
 $(venv) ellar runserver --reload
 ```
 
 Open your browser and navigate to [`http://localhost:8000/`](http://localhost:8000/).
 ![Swagger UI](img/ellar_framework.png)
 
-## Dependency Summary
+## **Dependency Summary**
 - `Python >= 3.7`
 - `Starlette`
 - `Pydantic`
 - `Injector`
 
-## Status
+## **Status**
 
 Project is still in development
 
 - Documentation - in progress
 - Interceptors  -  [Aspect Oriented Programming](https://en.wikipedia.org/wiki/Aspect-oriented_programming) (AOP) technique
 - Database Plugin with [Encode/ORM](https://github.com/encode/orm)
```

#### html2text {}

```diff
@@ -1,58 +1,59 @@
+# **[ellar](#introduction)**
                                  [Ellar_Logo]
   Ellar - Python ASGI web framework for building fast, efficient and scalable
                      RESTAPIs and server-side application.
 ![Test](https://github.com/eadwinCode/ellar/actions/workflows/test_full.yml/
 badge.svg) ![Coverage](https://img.shields.io/codecov/c/github/eadwinCode/
 ellar) [![PyPI version](https://badge.fury.io/py/ellar.svg)](https://
 badge.fury.io/py/ellar) [![PyPI version](https://img.shields.io/pypi/v/
 ellar.svg)](https://pypi.python.org/pypi/ellar) [![PyPI version](https://
 img.shields.io/pypi/pyversions/ellar.svg)](https://pypi.python.org/pypi/ellar)
---- ## Introduction Ellar is a lightweight ASGI framework for building
+--- ## **Introduction** Ellar is a lightweight ASGI framework for building
 efficient and scalable server-side python applications. It supports both OOP
-(Object-Oriented Programming) and FP (Functional Programming) Ellar is based on
-[Starlette (ASGI toolkit)](https://www.starlette.io/), a lightweight ASGI
-framework/toolkit well-suited for developing asynchronous web services in
-Python. And while Ellar provides a high level of abstraction on top of
-Starlette, it still incorporates some of its features, as well as those of
-FastAPI. If you are familiar with these frameworks, you will find it easy to
-understand and use Ellar. ## Inspiration Ellar was deeply influenced by
-[NestJS](https://docs.nestjs.com/) for its ease of use and ability to handle
-complex project structures and applications. Additionally, it took some
-concepts from [FastAPI](https://fastapi.tiangolo.com/) in terms of request
-parameter handling and data serialization with Pydantic. With that said, the
-objective of Ellar is to offer a high level of abstraction in its framework
-APIs, along with a well-structured project setup, an object-oriented approach
-to web application design, the ability to adapt to any desired software
-architecture, and ultimately, speedy request handling. ## Features Summary -
-**Easy to Use**: Ellar has a simple and intuitive API that makes it easy to get
-started with building a fast and scalable web applications or web APIs with
-Python. - **Dependency Injection (DI)**: It comes with DI system makes it easy
-to manage dependencies and reduce coupling between components. - **Pydantic
-Integration**: It is properly integrated with Pydantic, a popular Python
-library for data validation, to ensure that input data is valid. - **Templating
-with Jinja2**: Ellar provides built-in support for Jinja2 templates, making it
-easy to create dynamic web pages. - **OpenAPI Documentation**: It comes with
-built-in support for OpenAPI documentation, making it easy to generate
-`Swagger` or `ReDoc` documentation for your API. And more can be added with
-ease if necessary. - **Controller (MVC) Architecture**: Ellar's controller
-architecture follows the Model-View-Controller (MVC) pattern, making it easy to
-organize your code. - **Guards for Authentication and Authorization**: It
-provides built-in support for guards, allowing you to easily implement
-authentication and authorization in your application. - **Modularity**: Ellar
-follows a modular architecture inspired by NestJS, making it easy to organize
-your code into reusable modules. - **Asynchronous programming**: It allows you
-to takes advantage of Python's `async/await` feature to write efficient and
-fast code that can handle large numbers of concurrent requests ## Installation
-To get started, you need to scaffold a project using [Ellar-CLI](https://
-eadwincode.github.io/ellar-cli/) toolkit. This is recommended for a first-time
-user. The scaffolded project is more like a guide to project setup. ```shell $
-(venv) pip install ellar ``` After that, lets create a new project. Run the
-command below and change the `project-name` with whatever name you decide.
-```shell $(venv) ellar new project-name ``` then, start the app with: ```shell
-$(venv) ellar runserver --reload ``` Open your browser and navigate to [`http:/
-/localhost:8000/`](http://localhost:8000/). ![Swagger UI](img/
-ellar_framework.png) ## Dependency Summary - `Python >= 3.7` - `Starlette` -
-`Pydantic` - `Injector` ## Status Project is still in development -
-Documentation - in progress - Interceptors - [Aspect Oriented Programming]
-(https://en.wikipedia.org/wiki/Aspect-oriented_programming) (AOP) technique -
-Database Plugin with [Encode/ORM](https://github.com/encode/orm)
+(Object-Oriented Programming) and FP (Functional Programming) Ellar is also a
+higher level of abstraction of [Starlette (ASGI toolkit)](https://
+www.starlette.io/), a lightweight ASGI framework/toolkit well-suited for
+developing asynchronous web services in Python. ## **Inspiration** Ellar was
+deeply influenced by [NestJS](https://docs.nestjs.com/) for its ease of use,
+project structures and patterns that aids in building small or complex project
+applications. Also, Ellar took some concepts from [FastAPI](https://
+fastapi.tiangolo.com/) in terms of request parameter handling and data
+serialization with Pydantic. The objective of Ellar is to provide a high level
+of abstracted interface to the web, along with a well-structured project setup,
+give room for object-oriented approach to web application design, allow you
+chose your desired application architecture, and ultimately, deliver speedy
+handling to requests. As developers, we never know how big a project can become
+or evolve over time but following some design patterns and architecture makes
+it easier to build a more testable and maintainable application. ## **Features
+Summary** - **Easy to Use**: Ellar has a simple and intuitive API that makes it
+easy to get started with building a fast and scalable web applications or web
+APIs with Python. - **Dependency Injection (DI)**: It comes with DI system
+makes it easy to manage dependencies and reduce coupling between components. -
+**Pydantic Integration**: It is properly integrated with Pydantic, a popular
+Python library for data validation, to ensure that input data is valid. -
+**Templating with Jinja2**: Ellar provides built-in support for Jinja2
+templates, making it easy to create dynamic web pages. - **OpenAPI
+Documentation**: It comes with built-in support for OpenAPI documentation,
+making it easy to generate `Swagger` or `ReDoc` documentation for your API. And
+more can be added with ease if necessary. - **Controller (MVC) Architecture**:
+Ellar's controller architecture follows the Model-View-Controller (MVC)
+pattern, making it easy to organize your code. - **Guards for Authentication
+and Authorization**: It provides built-in support for guards, allowing you to
+easily implement authentication and authorization in your application. -
+**Modularity**: Ellar follows a modular architecture inspired by NestJS, making
+it easy to organize your code into reusable modules. - **Asynchronous
+programming**: It allows you to takes advantage of Python's `async/await`
+feature to write efficient and fast code that can handle large numbers of
+concurrent requests ## **Installation** To get started, you need to scaffold a
+project using [Ellar-CLI](https://eadwincode.github.io/ellar-cli/) toolkit.
+This is recommended for a first-time user. The scaffolded project is more like
+a guide to project setup. ```shell $(venv) pip install ellar ``` After that,
+lets create a new project. Run the command below and change the `project-name`
+with whatever name you decide. ```shell $(venv) ellar new project-name ```
+then, start the app with: ```shell $(venv) ellar runserver --reload ``` Open
+your browser and navigate to [`http://localhost:8000/`](http://localhost:8000/
+). ![Swagger UI](img/ellar_framework.png) ## **Dependency Summary** - `Python
+>= 3.7` - `Starlette` - `Pydantic` - `Injector` ## **Status** Project is still
+in development - Documentation - in progress - Interceptors - [Aspect Oriented
+Programming](https://en.wikipedia.org/wiki/Aspect-oriented_programming) (AOP)
+technique - Database Plugin with [Encode/ORM](https://github.com/encode/orm)
```

### Comparing `ellar-0.3.6/docs/overview/controllers.md` & `ellar-0.3.8/docs/overview/controllers.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 Controllers can be said to be a router with many routes registered in them.
 
 ### **Creating a Controller**
 To create a controller, we use classes and decorators. The `Controller` decorator associates classes with a required
 `metadata` needed for Ellar to create a routing table
 
 ```python
-from ellar.common import Controller
-from ellar.core import ControllerBase
+from ellar.common import Controller, ControllerBase
 
 @Controller()
 class UserController(ControllerBase):
     """We have created a controller that will manage our Users"""
 ```
 
 ## **Routing**
@@ -26,16 +25,15 @@
 
 For example, we may choose to group a set of routes that manage interactions with a customer entity under the route `/user`. 
 In that case, we could specify the path prefix `/user` in the `@Controller()` decorator so we don't have to repeat that portion of the path for each route in the controller.
 
 ```python
 # project_name/apps/car/controllers.py
 
-from ellar.common import Controller, get
-from ellar.core import ControllerBase
+from ellar.common import Controller, get, ControllerBase
 
 @Controller('/car')
 class CarController(ControllerBase):
     @get()
     def get_all(self):
         return 'This action returns all car'
     
@@ -76,16 +74,16 @@
 
 ### **Annotation (`parameter_name:Request`)**
 
 Ellar will resolve any parameter annotated as `Request` in the request handler signature as a `Request` object.
 ```python
 # project_name/apps/car/controllers.py
 
-from ellar.common import Controller, get
-from ellar.core import ControllerBase, Request
+from ellar.common import Controller, get, ControllerBase
+from ellar.core import Request
 
 @Controller('/car')
 class CarController(ControllerBase):
     @get()
     def get_all(self, request: Request):
         assert isinstance(request, Request) # True
         return 'This action returns all cars'
@@ -95,16 +93,16 @@
 
 ### **injection (`parameter_name=Req()`)**
 
 We can also inject request object to any handler by using `@Req` decorator in handler signature.
 ```python
 # project_name/apps/car/controllers.py
 
-from ellar.common import Controller, get, Req
-from ellar.core import ControllerBase, Request
+from ellar.common import Controller, ControllerBase, get, Req
+from ellar.core import Request
 
 @Controller('/car')
 class CarController(ControllerBase):
     @get()
     def get_all(self, req_data: Request, req_data_2=Req()):
         assert isinstance(req_data, Request) # True
         assert isinstance(req_data_2, Request)
@@ -115,16 +113,16 @@
 
 ### **Controllers Context**
 
 During request handler execution, `Execution Context` is available on the Controller instance and the `request` object can be gotten from the context.
 ```python
 # project_name/apps/car/controllers.py
 
-from ellar.common import Controller, get
-from ellar.core import ControllerBase, Request
+from ellar.common import Controller, ControllerBase, get
+from ellar.core import Request
 
 @Controller('/car')
 class CarController(ControllerBase):
     @get()
     def get_all(self):
         assert isinstance(self.context.switch_to_http_connection().get_request(), Request) # True
         return 'This action returns all cars'
@@ -151,16 +149,16 @@
 
 ## **Resource**
 
 Let add create endpoint to our `CarController` resource.
 ```python
 # project_name/apps/car/controllers.py
 
-from ellar.common import Controller, get, post
-from ellar.core import ControllerBase, Request
+from ellar.common import Controller, ControllerBase, get, post
+from ellar.core import Request
 
 @Controller('/car')
 class CarController(ControllerBase):
     @post()
     def create(self):
         return 'This action adds a new car'
     
@@ -188,16 +186,16 @@
 ## **Asynchronicity**
 
 Ellar supports modern asynchronous programming in python using `async` and `await` syntax.
 
 ```python
 # project_name/apps/car/controllers.py
 
-from ellar.common import Controller, get, post
-from ellar.core import ControllerBase, Request
+from ellar.common import Controller, ControllerBase, get, post
+from ellar.core import Request
 
 @Controller('/car')
 class CarController(ControllerBase):
     @post()
     async def create(self):
         return 'This action adds a new car'
     
@@ -211,15 +209,15 @@
 ## **Request Payload**
 
 Let's use `@Body()` to define the required data to create a car in our previous `create`(POST) endpoint.
 Before that, we need to define our data input/output serializers
 
 ```python
 # project_name/apps/car/schema.py
-from ellar.serializer import Serializer
+from ellar.common import Serializer
 from pydantic import Field
 
 
 class CreateCarSerializer(Serializer):
     name: str
     year: int = Field(..., gt=0)
     model: str
@@ -237,15 +235,15 @@
     model: str
 ```
 
 Let's add the `CreateCarSerializer` to `create` endpoint,
 ```python
 # project_name/apps/car/controllers.py
 ...
-from ellar.common import Body
+from ellar.common import Body, post
 from .schemas import CreateCarSerializer
 
 
 @post()
 async def create(self, payload: CreateCarSerializer = Body()):
     return 'This action adds a new car'
 ```
@@ -254,23 +252,23 @@
 
 It's important to note the way we used `CreateCarSerializer` as a type annotation of the `payload` parameter in the `create` route handler method. 
 Ellar will compute values for all the route handler parameters and validates them based on the annotated types before executing the handler. 
 
 !!! info
     if a parameter is not annotated, it will be assumed as a `string` type
 
-![CreateDogSchema](../img/create-car-schema.png)
+![CreateCarSchema](../img/create-car-schema.png)
 
 Let's add other endpoints
 
 ```python
 # project_name/apps/car/controllers.py
 
-from ellar.common import Body, Controller, delete, get, post, put, Query
-from ellar.core import ControllerBase, Request
+from ellar.common import Body, Controller, ControllerBase, delete, get, post, put, Query
+from ellar.core import Request
 from .schemas import CreateCarSerializer, CarListFilter
 
 
 @Controller('/car')
 class CarController(ControllerBase):
     @post()
     async def create(self, payload: CreateCarSerializer = Body()):
```

### Comparing `ellar-0.3.6/docs/overview/custom_decorators.md` & `ellar-0.3.8/docs/overview/custom_decorators.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,20 +42,22 @@
 from ellar.common import WsBody, ws_route
 from ellar.core import WebSocket
 ...
 @ws_route('/websocket', use_extra_handler=True)
 def sample_endpoint_ws(self, websocket: WebSocket, data_schema: str = WsBody()):
     pass
 
-@sample_endpoint_ws.connect
+@ws_route.connect(sample_endpoint_ws)
 async def on_connect(self, websocket: WebSocket):
+    # Called when there is a connection to `sample_endpoint_ws`
     await websocket.accept()
 
-@sample_endpoint_ws.disconnect
-async def on_connect(self, websocket: WebSocket, code: int):
+@ws_route.disconnect(sample_endpoint_ws)
+async def on_disconnect(self, websocket: WebSocket, code: int):
+    # Called when there is a disconnect from `sample_endpoint_ws`
     await websocket.close(code)
 ```
 
 ## **Non Route Function Parameters Decorators**
 We discussed decorators that are used to define route function parameter dependencies in Ellar. 
 These decorators, such as `Query`, `Form`, and `Body`, etc. are pydantic models used to specify the expected parameters for a route function. 
 
@@ -184,16 +186,16 @@
 They are gotten from the application of the NonParameterResolver, like so - `def s(parameter_name:type_annotation = NonParameterResolver())`.
 
 `NonParameterResolver` receives current `IExecutionContext` must return a tuple of dict object of the resulting resolve data with `parameter_name` and list of errors if any. As shown in the return statements in the example below.
 
 For example:
 ```python
 import typing as t
-from ellar.core.params import NonParameterResolver
-from ellar.core import IExecutionContext
+from ellar.common.params import NonParameterResolver
+from ellar.common import IExecutionContext
 from pydantic.error_wrappers import ErrorWrapper
 
 
 class UserParam(NonParameterResolver):
     async def resolve(self, ctx: IExecutionContext, **kwargs: t.Any) -> t.Any:
         request = ctx.switch_to_http_connection().get_request()
         user = request.get('user', None)
@@ -249,15 +251,15 @@
 #### FileResponseModel as file(streaming=False)
 When `streaming` parameter in `@file(streaming=False)` decorator is set to `False`, a `FileResponseModel` is created as the response model for the decorated route function. 
 And the route function is required to return a dictionary object that follows a `FileResponseModelSchema` format:
 
 ```python
 import typing as t
 from enum import Enum
-from ellar.serializer import Serializer
+from ellar.common import Serializer
 
 
 class ContentDispositionType(str, Enum):
     inline = "inline"
     attachment = "attachment"
 
     
@@ -356,16 +358,15 @@
 - `exclude_unset`: whether fields which were not explicitly set when creating the model should be excluded from the returned dictionary; default `False`.
 - `exclude_defaults`: whether fields which are equal to their default values (whether set or otherwise) should be excluded from the returned dictionary; default `False`
 - `exclude_none`: whether fields which are equal to None should be excluded from the returned dictionary; default `False`
 
 For example:
 ```python
 import typing as t
-from ellar.common import serializer_filter, get
-from ellar.serializer import Serializer
+from ellar.common import serializer_filter, get, Serializer
 
 class UserSchema(Serializer):
     username: str
     password: str
     first_name: t.Optional[str]
     last_name: t.Optional[str]
 
@@ -409,16 +410,15 @@
 
 More information on how to use this decorator can be found in the [Guard Documentation]()
 
 A quick example on how to use `Guards` decorator:
 ```python
 import typing as t
 from ellar.common import get, Guards
-from ellar.core.guard import APIKeyQuery
-from ellar.core.connection import HTTPConnection
+from ellar.core import APIKeyQuery, HTTPConnection
 
 
 class MyAPIKeyQuery(APIKeyQuery):
     async def authenticate(self, connection: HTTPConnection, key: t.Optional[t.Any]) -> t.Optional[t.Any]:
         if key == 'supersecret':
             return True
         return False
```

### Comparing `ellar-0.3.6/docs/overview/exception_handling.md` & `ellar-0.3.8/docs/overview/exception_handling.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 ## **APIException**
 It is a type of exception for REST API based applications. It gives more concept to error and provides a simple interface for creating other custom exception needs in your application without having to create an extra exception handler.
 
 For example,
 
 ```python
-from ellar.core.exceptions import APIException
+from ellar.common.exceptions import APIException
 from starlette import status
 
 class ServiceUnavailableException(APIException):
     status_code = status.HTTP_503_SERVICE_UNAVAILABLE
     code = 'service_unavailable'
 
 ```
@@ -86,16 +86,15 @@
 To create an exception handler for your custom exception, you have to make a class that follows the `IExceptionHandler` contract.
 
 At the root project folder, create a file `custom_exceptions.py`,
 
 ```python
 # project_name/custom_exceptions.py
 import typing as t
-from ellar.core.exceptions import IExceptionHandler
-from ellar.core.context import IHostContext
+from ellar.common import IExceptionHandler, IHostContext
 from starlette.responses import Response
 
 
 class MyCustomException(Exception):
     pass
 
 
@@ -118,17 +117,15 @@
 - `catch()`: defines the handling code and response to be returned to the client.
 
 ### **Creating Exception Handler for status code**
 Let's create a handler for `MethodNotAllowedException` which, according to the HTTP code is `405`.
 ```python
 # project_name/apps/custom_exceptions.py
 import typing as t
-from ellar.core.exceptions import IExceptionHandler
-from ellar.core.context import IHostContext
-from ellar.core import render_template
+from ellar.common import IExceptionHandler, IHostContext, render_template
 from starlette.responses import Response
 from starlette.exceptions import HTTPException
 
 class MyCustomException(Exception):
     pass
 
 
@@ -166,15 +163,15 @@
 
 - `config.py`: The config file holds manage application settings. The `EXCEPTION_HANDLERS` variable defines all custom exception handlers registered to `ExceptionMiddlewareService` when bootstrapping the application.
 
 ```python
 # project_name/config.py
 import typing as t
 from ellar.core import ConfigDefaultTypesMixin
-from ellar.core.exceptions import IExceptionHandler
+from ellar.common import IExceptionHandler
 from .apps.custom_exceptions import MyCustomExceptionHandler, ExceptionHandlerAction405
 
 class BaseConfig(ConfigDefaultTypesMixin):
     EXCEPTION_HANDLERS: t.List[IExceptionHandler] = [
         MyCustomExceptionHandler(),
         ExceptionHandlerAction405()
     ]
@@ -182,15 +179,15 @@
 - `application instance`: You can also add exception through `app` instance.
 
 ```python
 # project_name/server.py
 
 import os
 
-from ellar.constants import ELLAR_CONFIG_MODULE
+from ellar.common.constants import ELLAR_CONFIG_MODULE
 from ellar.core.factory import AppFactory
 from .root_module import ApplicationModule
 from .apps.custom_exceptions import MyCustomExceptionHandler, ExceptionHandlerAction405
 
 application = AppFactory.create_from_app_module(
     ApplicationModule,
     config_module=os.environ.get(
@@ -209,16 +206,15 @@
 To override any exception handler, it follows the same pattern and then defines the target to exception type
 
 For example:
 
 ```python
 # project_name/apps/custom_exceptions.py
 import typing as t
-from ellar.core.exceptions import IExceptionHandler, APIException
-from ellar.core.context import IHostContext
+from ellar.common import IHostContext, IExceptionHandler, APIException
 from starlette.responses import Response
 
 
 class OverrideAPIExceptionHandler(IExceptionHandler):
     exception_type_or_code = APIException
     
     async def catch(
```

### Comparing `ellar-0.3.6/docs/overview/guards.md` & `ellar-0.3.8/docs/overview/guards.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,20 @@
     Guards are executed **after** all middleware
 
 ## **Authorization guard**
 Authorization is a great example of a guard because some routes should be available only to specific authenticated user and or users that sufficient permissions. 
 Let's assume we have a `AuthGard` which checks if a making a request is authenticated.
 
 ```python
-from ellar.core import GuardCanActivate, ExecutionContext
+from ellar.common import GuardCanActivate, IExecutionContext
 from ellar.di import injectable
 
 @injectable()
 class AuthGuard(GuardCanActivate):
-  async def can_activate(self,context: ExecutionContext) -> bool: 
+  async def can_activate(self,context: IExecutionContext) -> bool: 
     request = context.switch_to_http_connection().get_request()
     return self.validate_request(request)
 
   def validate_request(self, request) -> bool:
     ...
 
 ```
@@ -40,20 +40,20 @@
 Let's build a more functional guard that permits access only to users with a specific role. 
 We'll start with a basic guard template, and build on it in the coming sections. 
 For now, it allows all requests to proceed:
 
 ```python
 # project_name/cars/guards.py
 
-from ellar.core import GuardCanActivate, ExecutionContext
+from ellar.common import GuardCanActivate, IExecutionContext
 from ellar.di import injectable
 
 @injectable()
 class RoleGuard(GuardCanActivate):
-  async def can_activate(self,context: ExecutionContext) -> bool: 
+  async def can_activate(self,context: IExecutionContext) -> bool: 
     return True
 ```
 
 ## **Applying guards**
 Guards can be **`controller-scoped`**, **`method-scoped`**, or **`global-scoped`**. We apply guards to controllers or route function by using `@Guards`.
 The `@Guards` takes a single argument, or a comma-separated list of arguments of `GuardCanActivate` types or instances.
 
@@ -105,15 +105,15 @@
 Global guards are used across the whole application, for every controller and every route function but individual controller or route function `@Guards` definition can override `global` scoped guards.
 
 Global guards are applied at the `global_guards` parameter of the `AppFactory` creation level as shown below:
 ```python
 # project_name/server.py
 import os
 
-from ellar.constants import ELLAR_CONFIG_MODULE
+from ellar.common.constants import ELLAR_CONFIG_MODULE
 from ellar.core.factory import AppFactory
 from .apps.cars.guards import RoleGuard
 from .root_module import ApplicationModule
 
 application = AppFactory.create_from_app_module(
     ApplicationModule,
     config_module=os.environ.get(
@@ -169,16 +169,16 @@
 
 In order to access the route's function `role(s)` **(custom metadata)**, we'll use the `Reflector` helper class, which is provided out of the box by the framework.
 
 ```python
 # project_name/apps/cars/guards.py
 import typing as t
 from ellar.di import injectable
-from ellar.core import GuardCanActivate, IExecutionContext
-from ellar.services import Reflector
+from ellar.common import GuardCanActivate, IExecutionContext
+from ellar.core.services import Reflector
 
 
 @injectable()
 class RoleGuard(GuardCanActivate):
     def __init__(self, reflector: Reflector):
         self.reflector = reflector
     
@@ -210,15 +210,17 @@
   "status_code": 403
 }
 ```
 
 Note that behind the scenes, when a guard returns `false`, the framework throws a `HTTPException` with status code **403** . 
 If you want to return a different error response, you should throw your own specific exception by override `raise_exception` function as shown below:
 ```python
-from ellar.core.exceptions import APIException
+from ellar.common import APIException, GuardCanActivate
+from ellar.di import injectable
+from ellar.core import Reflector
 
 @injectable()
 class RoleGuard(GuardCanActivate):
     def __init__(self, reflector: Reflector):
         self.reflector = reflector
         
     def raise_exception(self) -> None:
```

### Comparing `ellar-0.3.6/docs/overview/index.md` & `ellar-0.3.8/docs/overview/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -142,19 +142,19 @@
 ```
 Brief overview of the generated files:
 
 |                   |                                                   |
 |-------------------|---------------------------------------------------|
 | `car.controllers` | A basic controller with an `index` route.         |
 | `car.module.py`   | car module/app `Module` metadata definition.      |
-| `car.services.py` | For Dogs module service declarations.             |
+| `car.services.py` | For Car module service declarations.              |
 | `car.schemas.py`  | Data-transfer-object or Serializers declarations. |
-| `car.tests/`      | testing directory for the dogs module.            |
+| `car.tests/`      | testing directory for the car module.             |
 
-To finish up with the created `dogs` module, we need to register it to the 
+To finish up with the created `car` module, we need to register it to the 
 `project_name.root_module.py`
 
 ```python
 # project_name/root_module.py
 ...
 from .apps.cars.module import CarModule
 
@@ -163,15 +163,15 @@
 class ApplicationModule(ModuleBase):
     @exception_handler(404)
     def exception_404_handler(cls, request: Request, exc: Exception) -> Response:
         return JSONResponse(dict(detail="Resource not found."))
 ```
 That's it.
 
-Goto your browser and visit: [http://localhost:8000/dogs/](http://localhost:8000/car/)
+Goto your browser and visit: [http://localhost:8000/car/](http://localhost:8000/car/)
 ```json
 {
   "detail": "Welcome Car Resource"
 }
 ```
 
 ## Enabling OpenAPI Docs
```

### Comparing `ellar-0.3.6/docs/overview/middleware.md` & `ellar-0.3.8/docs/overview/middleware.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/docs/overview/module-router.md` & `ellar-0.3.8/docs/overview/module-router.md`

 * *Files 2% similar despite different names*

```diff
@@ -75,16 +75,16 @@
 ## **Accessing Other Request Object**
 In functional route handle, we can access request object and response object through custom decorators or type annotation as shown below.
 
 ### By Type Annotation
 Let's inject request and response object in `addition` route handler function from our previous example
 
 ```python
-from ellar.core import Request, Response
-from ellar.common import ModuleRouter
+from ellar.core import Request
+from ellar.common import ModuleRouter, Response
 
 
 math_router = ModuleRouter('/math', tag='Math')
 
 @math_router.get('/add')
 def addition(request: Request, res: Response, a:int, b:int):
     res.headers['x-operation'] = 'Addition'
@@ -92,16 +92,16 @@
 
 ```
 
 ### **By Custom decorators**
 You can also achieve the same result by using custom decorator.
 
 ```python
-from ellar.core import Request, Response
-from ellar.common import ModuleRouter, Req, Res
+from ellar.core import Request
+from ellar.common import ModuleRouter, Req, Res, Response
 
 
 math_router = ModuleRouter('/math', tag='Math')
 
 @math_router.get('/add')
 def addition(*, request=Req(), res=Res(), a:int, b:int):
     res.headers['x-operation'] = 'Addition'
@@ -111,16 +111,16 @@
 
 ![math_router_with_request_object.png](../img/math_router_with_request_object.png)
 
 ## **Inject Services**
 We can also inject service providers just like controller routes using the `Provide` function.
 
 ```python
-from ellar.core import Response, Config
-from ellar.common import ModuleRouter, Provide
+from ellar.core import Config
+from ellar.common import ModuleRouter, Provide, Response
 
 
 math_router = ModuleRouter('/math', tag='Math')
 
 @math_router.get('/subtract')
 def subtraction(a:int, b:int, res:Response, config=Provide(Config)):
     res.headers['x-operation'] = 'Subtraction'
```

### Comparing `ellar-0.3.6/docs/overview/modules.md` & `ellar-0.3.8/docs/overview/modules.md`

 * *Files 4% similar despite different names*

```diff
@@ -88,52 +88,20 @@
     
     def application_ready(self, app: App) -> None:
         """Called when application is ready - this is similar to @on_startup event"""
 
 ```
 `before_init` receives current app `Config` as a parameter and `application_ready` function receives `App` instance as parameter.
 
-####  **Starlette Application Events**
-We can register multiple event handlers for dealing with `tasks` that need to run before
-the application starts `up`, or when the application is shutting `down`.
-This is the way we support `Starlette` start-up events in `Ellar`
-
-```python
-
-from ellar.common import Module, on_shutdown, on_startup
-from ellar.core import ModuleBase
-
-@Module()
-class ModuleRequestEventsSample(ModuleBase):
-    @on_startup
-    def on_startup_func(cls):
-        pass
-    
-    @on_startup()
-    async def on_startup_func_2(cls):
-        pass
-    
-    @on_shutdown
-    def on_shutdown_func(cls):
-        pass
-    
-    @on_shutdown()
-    async def on_shutdown_func_2(cls):
-        pass
-```
-These will be registered to the application router during the `ModuleRequestEventsSample` computation at runtime.
-Also, the events can be `async` as in the case of `on_shutdown_func_2` and `on_startup_func_2`
-
 ### **Module Exceptions**
 Custom exception handlers can be registered through modules.
 
 ```python
-from ellar.common import Module, exception_handler
-from ellar.core import  ModuleBase, JSONResponse, Response
-from ellar.core.context import IHostContext
+from ellar.common import Module, exception_handler, JSONResponse, Response, IHostContext
+from ellar.core import ModuleBase
 
 @Module()
 class ModuleExceptionSample(ModuleBase):
     @exception_handler(404)
     def exception_404_handler(cls, context: IHostContext, exc: Exception) -> Response:
         return JSONResponse(dict(detail="Resource not found."))
 ```
@@ -196,18 +164,16 @@
 ## **Module Middleware**
 
 Middlewares functions can be defined at Module level with `@middleware()` function decorator.
 
 For example:
 
 ```python
-from ellar.common import Module, middleware
+from ellar.common import Module, middleware, IHostContext, PlainTextResponse
 from ellar.core import ModuleBase
-from ellar.core.context import IHostContext
-from starlette.responses import PlainTextResponse
 
 
 @Module()
 class ModuleMiddlewareSample(ModuleBase):
     @middleware()
     async def my_middleware_function_1(cls, context: IHostContext, call_next):
         request = context.switch_to_http_connection().get_request() # for http response only
@@ -349,17 +315,17 @@
 - **`factory`:** a factory function used to configure the module and take `Module` type as first argument and other services as listed in `inject` attribute.
 
 Let's look this `ModuleSetup` example code below with our focus on how we eventually configured `DynamicService` type, 
 how we used `my_module_configuration_factory` to dynamically build `MyModule` module.
 
 ```python
 import typing as t
-from ellar.common import Module
+from ellar.common import Module, IModuleSetup
 from ellar.di import ProviderConfig
-from ellar.core import DynamicModule, ModuleBase, IModuleSetup, Config, ModuleSetup, AppFactory
+from ellar.core import DynamicModule, ModuleBase, Config, ModuleSetup, AppFactory
 
 
 class Foo:
     def __init__(self):
         self.foo = 'foo'
```

### Comparing `ellar-0.3.6/docs/overview/providers.md` & `ellar-0.3.8/docs/overview/providers.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 
 We have created a `UserRepository` provider that will help manage the loading and saving of user data to the database.
 
 Let's add this service to a controller.
 
 ```python
 from ellar.di import injectable, singleton_scope
-from ellar.core import ControllerBase
-from ellar.common import Controller
+from ellar.common import Controller, ControllerBase
 
 
 @injectable(scope=singleton_scope)
 class UserRepository:
     pass
 
 
@@ -61,16 +60,15 @@
 We have successfully created a `CarRepository` with a `singleton` scope.
 
 Let's wire it up to `CarController`. And rewrite some route handles.
 
 ```python
 # project_name/apps/car/controllers.py
 
-from ellar.common import Body, Controller, get, post, Query
-from ellar.core import ControllerBase
+from ellar.common import Body, Controller, get, post, Query, ControllerBase
 from .schemas import CreateCarSerializer, CarListFilter
 from .services import CarRepository
 
 
 @Controller('/car')
 class CarController(ControllerBase):
     def __init__(self, repo: CarRepository):
@@ -292,15 +290,15 @@
 
 For example:
 ```python
 # main.py
 
 from ellar.common import Module
 from ellar.core import ModuleBase, Config
-from ellar.di import Container, EllarInjector, injectable, ProviderConfig
+from ellar.di import Container, EllarInjector, injectable
 from ellar.core.modules.ref import create_module_ref_factor
 
 injector = EllarInjector(auto_bind=False)
 
 
 class IFoo:
     pass
```

### Comparing `ellar-0.3.6/docs/parsing-inputs/body.md` & `ellar-0.3.8/docs/parsing-inputs/body.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ## Import Serializer
 
 First, you need to import `Serializer` from `ella.serializer`:
 
 ```python
 # project_name/apps/items/controllers.py
-from ellar.serializer import Serializer
+from ellar.common import Serializer
 
 # class Item(Serializer):
 #     name: str
 #     description: str = None
 #     price: float
 #     quantity: int
 
@@ -29,18 +29,15 @@
 Then you declare your data model as a class that inherits from `Serializer`.
 
 Use standard Python types for all the attributes:
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.serializer import Serializer
-from ellar.common import Controller, post
-from ellar.core import ControllerBase
-
+from ellar.common import Serializer, ControllerBase, Controller, post
 
 class Item(Serializer):
     name: str
     description: str = None
     price: float
     quantity: int
 
@@ -77,17 +74,15 @@
 ## Declare it as a parameter
 
 To add it to your *path operation*, declare it the same way you declared the path and query parameters:
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.serializer import Serializer
-from ellar.common import Controller, post
-from ellar.core import ControllerBase
+from ellar.common import Serializer, Controller, post, ControllerBase
 
 
 class Item(Serializer):
     name: str
     description: str = None
     price: float
     quantity: int
@@ -133,17 +128,15 @@
 You can declare path parameters **and** body requests at the same time.
 
 **Ellar** will recognize that the function parameters that match path parameters should be **taken from the path**, and that function parameters that are declared with `Serializer` should be **taken from the request body**.
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.serializer import Serializer
-from ellar.common import Controller, post, put
-from ellar.core import ControllerBase
+from ellar.common import Serializer, Controller, post, put, ControllerBase
 
 
 class Item(Serializer):
     name: str
     description: str = None
     price: float
     quantity: int
@@ -164,17 +157,15 @@
 You can also declare **body**, **path** and **query** parameters, all at the same time.
 
 **Ellar** will recognize each of them and take the data from the correct place.
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.serializer import Serializer
-from ellar.common import Controller, post, put
-from ellar.core import ControllerBase
+from ellar.common import Serializer, Controller, post, put, ControllerBase
 
 
 class Item(Serializer):
     name: str
     description: str = None
     price: float
     quantity: int
@@ -209,17 +200,15 @@
 If you declare it as is, because it is a singular value, **Ellar** will assume that it is a query parameter.
 
 But you can instruct **Ellar** to treat it as another body key using Body:
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.serializer import Serializer
-from ellar.common import Controller, Body, post, put
-from ellar.core import ControllerBase
+from ellar.common import Serializer, Controller, Body, post, put, ControllerBase
 from pydantic import BaseModel
 
 
 class Item(Serializer):
     name: str
     description: str = None
     price: float
@@ -270,17 +259,15 @@
 As, by default, singular values are interpreted as query parameters, you don't have to explicitly add a `Query`, you can just do:
 
 For example:
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.serializer import Serializer
-from ellar.common import Controller, Body, post, put
-from ellar.core import ControllerBase
+from ellar.common import Serializer, Controller, Body, post, put, ControllerBase
 from pydantic import BaseModel
 
 
 class Item(Serializer):
     name: str
     description: str = None
     price: float
```

### Comparing `ellar-0.3.6/docs/parsing-inputs/cookie-params.md` & `ellar-0.3.8/docs/parsing-inputs/cookie-params.md`

 * *Files 23% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 
 The first value is the default value, you can pass all the extra validation or annotation parameters:
 
 ```python
 # project_name/apps/items/controllers.py
 
 from typing import Optional
-from ellar.common import get, Controller, Cookie
-from ellar.core import ControllerBase
+from ellar.common import get, Controller, Cookie, ControllerBase
 
 
 @Controller
 class ItemsController(ControllerBase):
     @get("/")
     async def read_items(self, ads_id: Optional[str] = Cookie(default=None)):
         return {"ads_id": ads_id}
@@ -33,17 +32,15 @@
 ### Using Schema
 
 You can also use Schema to encapsulate `Cookies` parameters:
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.serializer import Serializer
-from ellar.common import get, Controller, Cookie
-from ellar.core import ControllerBase
+from ellar.common import Serializer, get, Controller, Cookie, ControllerBase
 
 
 
 class CookieSchema(Serializer):
     cookieItem1: int = 100
     cookieItem2: str = None
```

### Comparing `ellar-0.3.6/docs/parsing-inputs/file-params.md` & `ellar-0.3.8/docs/parsing-inputs/file-params.md`

 * *Files 8% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 
 ## Define `File` parameters
 
 Create file parameters the same way you would for `Body` or `Form`:
 
 ```python
 # project_name/apps/items/controllers.py
-from ellar.common import File
-from ellar.common import Controller, post
-from ellar.core import ControllerBase
+from ellar.common import File, Controller, post, ControllerBase
 
 
 @Controller
 class ItemsController(ControllerBase):
     @post("/files/")
     async def create_file(self, file: bytes = File()):
         return {"file_size": len(file)}
@@ -42,17 +40,15 @@
 
 ## `File` parameters with `UploadFile`
 
 Define a `File` parameter with a type of `UploadFile`:
 
 ```python
 # project_name/apps/items/controllers.py
-from ellar.common import File, UploadFile
-from ellar.common import Controller, post
-from ellar.core import ControllerBase
+from ellar.common import File, UploadFile, Controller, post, ControllerBase
 
 
 @Controller
 class ItemsController(ControllerBase):
     @post("/files/")
     async def create_file(self, file: bytes = File()):
         return {"file_size": len(file)}
@@ -114,17 +110,15 @@
 
 To **upload several files** at the same time, just declare a `List` of `UploadFile`:
 
 
 ```python
 # project_name/apps/items/controllers.py
 from typing import List
-from ellar.common import File, UploadFile
-from ellar.common import Controller, post
-from ellar.core import ControllerBase
+from ellar.common import File, UploadFile, Controller, post, ControllerBase
 
 
 @Controller
 class ItemsController(ControllerBase):
     @post("/upload-many")
     def upload_many(self, files: List[UploadFile] = File()):
         return [f.filename for f in files]
@@ -135,17 +129,15 @@
 Note: HTTP protocol does not allow you to send files in application/json format by default (unless you encode it somehow to JSON on client side)
 
 To send files along with some extra attributes you need to send bodies in multipart/form-data encoding. You can do it by simply marking fields with `Form`:
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.serializer import Serializer
-from ellar.common import Controller, Form, File, UploadFile, post
-from ellar.core import ControllerBase
+from ellar.common import Serializer, Controller, Form, File, UploadFile, post, ControllerBase
 from datetime import date
 
 
 class UserDetails(Serializer):
     first_name: str
     last_name: str
     birthdate: date
@@ -162,17 +154,15 @@
 Note: in this case all fields should be sent as form fields
 
 You can as well send payload in single field as JSON - just remove the Form mark from:
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.serializer import Serializer
-from ellar.common import Controller, File, UploadFile, post
-from ellar.core import ControllerBase
+from ellar.common import Serializer, Controller, File, UploadFile, post, ControllerBase
 from datetime import date
 
 
 class UserDetails(Serializer):
     first_name: str
     last_name: str
     birthdate: date
```

### Comparing `ellar-0.3.6/docs/parsing-inputs/form-params.md` & `ellar-0.3.8/docs/parsing-inputs/form-params.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
 
 ## Form Data as params 
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.common import Controller, Form, post
-from ellar.core import ControllerBase
+from ellar.common import Controller, Form, post, ControllerBase
 
 
 @Controller
 class ItemsController(ControllerBase):
     @post("/login")
     def login(self, username: str = Form(), password: str = Form()):
         return {'username': username, 'password': '*****'}
@@ -44,17 +43,15 @@
 
 In a similar manner to [Body](../body/#declare-it-as-a-parameter), you can use
 a Schema to organize your parameters.
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.serializer import Serializer
-from ellar.common import Controller, post, Form
-from ellar.core import ControllerBase
+from ellar.common import Serializer, Controller, post, Form, ControllerBase
 
 
 class Item(Serializer):
     name: str
     description: str = None
     price: float
     quantity: int
@@ -79,17 +76,15 @@
 **Ellar** will recognize that the function parameters that match path
 parameters should be **taken from the path**, and that function parameters that
 are declared with `Form(...)` should be **taken from the request form fields**, etc.
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.serializer import Serializer
-from ellar.common import Controller, Form, post, put
-from ellar.core import ControllerBase
+from ellar.common import Serializer, Controller, Form, post, put, ControllerBase
 
 
 class Item(Serializer):
     name: str
     description: str = None
     price: float
     quantity: int
@@ -113,17 +108,15 @@
 
 This can be fixed, as described in the Pydantic docs, by using
 [Generic Classes as Types](https://pydantic-docs.helpmanual.io/usage/types/#generic-classes-as-types).
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.serializer import Serializer
-from ellar.common import Controller, Form, post, put
-from ellar.core import ControllerBase
+from ellar.common import Serializer, Controller, Form, post, put, ControllerBase
 from pydantic.fields import ModelField
 from typing import Generic, TypeVar
 
 PydanticField = TypeVar("PydanticField")
 
 
 class EmptyStrToDefault(Generic[PydanticField]):
```

### Comparing `ellar-0.3.6/docs/parsing-inputs/header-params.md` & `ellar-0.3.8/docs/parsing-inputs/header-params.md`

 * *Files 11% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 Then declare the header parameters using the same structure as with `Path`, `Query` and `Cookie`.
 
 The first value is the default value, you can pass all the extra validation or annotation parameters:
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.common import Controller, get, Header
-from ellar.core import ControllerBase
+from ellar.common import Controller, get, Header, ControllerBase
 from typing import Optional
 
 
 @Controller
 class ItemsController(ControllerBase):
     @get("/")
     async def read_items(self, user_agent: Optional[str] = Header(default=None)):
@@ -47,16 +46,15 @@
 So, you can use `user_agent` as you normally would in Python code, instead of needing to capitalize the first letters as `User_Agent` or something similar.
 
 If for some reason you need to disable automatic conversion of underscores to hyphens, set the parameter `convert_underscores` of `Header` to `False`:
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.common import Controller, get, Header
-from ellar.core import ControllerBase
+from ellar.common import Controller, get, Header, ControllerBase
 from typing import Optional
 
 
 @Controller
 class ItemsController(ControllerBase):
     @get("/")
     async def read_items(
@@ -78,16 +76,15 @@
 You will receive all the values from the duplicate header as a Python `list`.
 
 For example, to declare a header of `X-Token` that can appear more than once, you can write:
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.common import Controller, get, Header
-from ellar.core import ControllerBase
+from ellar.common import Controller, get, Header, ControllerBase
 from typing import Optional, List
 
 
 @Controller
 class ItemsController(ControllerBase):
     @get("/")
     async def read_items(self, x_token: Optional[List[str]] = Header(default=None)):
@@ -116,17 +113,15 @@
 
 You can also use Schema to encapsulate `Header` parameters:
 
 ```python
 # project_name/apps/items/controllers.py
 
 from typing import List
-from ellar.serializer import Serializer
-from ellar.common import get, Controller, Header
-from ellar.core import ControllerBase
+from ellar.common import Serializer, get, Controller, Header, ControllerBase
 
 
 
 class HeaderSchema(Serializer):
     version: int = 1
     x_token: List[str] = None # similar to x_token: Optional[List[str]]
```

### Comparing `ellar-0.3.6/docs/parsing-inputs/index.md` & `ellar-0.3.8/docs/parsing-inputs/index.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,18 +9,16 @@
 ```shell
 $(venv) ellar create-module items
 ```
 
 Next, goto `project_name/root_module.py` and add `ItemsModule` to list of modules.
 
 ```python
-from ellar.common import Module, exception_handler
+from ellar.common import Module, exception_handler, IExecutionContext, JSONResponse, Response
 from ellar.core import ModuleBase
-from ellar.core.context import IExecutionContext
-from ellar.core.response import JSONResponse, Response
 from ellar.samples.modules import HomeModule
 from .apps.car.module import CarModule
 from .apps.items.module import ItemsModule
 
 
 @Module(modules=[HomeModule, CarModule, ItemsModule])
 class ApplicationModule(ModuleBase):
```

### Comparing `ellar-0.3.6/docs/parsing-inputs/path-params.md` & `ellar-0.3.8/docs/parsing-inputs/path-params.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 You can declare path "parameters" with the same syntax used by Python format-strings 
 which is similar to [OpenAPI path parameters](https://swagger.io/docs/specification/describing-parameters/#path-parameters)
 
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.common import get, Controller
-from ellar.core import ControllerBase
+from ellar.common import get, Controller, ControllerBase
 
 
 @Controller
 class ItemsController(ControllerBase):
     @get("/{item_id}")
     def read_item(self, item_id):
         return {"item_id": item_id}
@@ -29,16 +28,15 @@
 
 ### Path parameters with types
 You can declare the type of path parameter in the function using standard Python type annotations:
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.common import get, Controller
-from ellar.core import ControllerBase
+from ellar.common import get, Controller, ControllerBase
 
 
 @Controller
 class ItemsController(ControllerBase):
     @get("/items/{item_id}")
     def read_item(self, item_id: int):
         return {"item_id": item_id}
@@ -83,16 +81,15 @@
 ### Path Converters
 
 You can use [Starlette Path Converters](https://www.starlette.io/routing/#path-parameters) to help parse the path:
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.common import get, Controller
-from ellar.core import ControllerBase
+from ellar.common import get, Controller, ControllerBase
 
 
 @Controller
 class ItemsController(ControllerBase):
     @get("/{item_id:int}")
     def read_item(self, item_id):
         return {"item_id": item_id}
@@ -119,16 +116,15 @@
 
 For example, lets another route handler `some_view` and give it a path `/dir/{value:path}`.
 What this means is that the parameter is `value`, and the last part, `:path`, tells it that the parameter should match any path.
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.common import get, Controller
-from ellar.core import ControllerBase
+from ellar.common import get, Controller, ControllerBase
 
 
 @Controller
 class ItemsController(ControllerBase):
     @get('/dir/{value:path}')
     def some_view(self, value: str):
         return value
@@ -139,16 +135,15 @@
 ### Multiple parameters
 
 You can pass as many variables as you want into `path`, just remember to have unique names and don't forget to use the same names in the function arguments.
 
 ```Python
 # project_name/apps/items/controllers.py
 
-from ellar.common import get, Controller
-from ellar.core import ControllerBase
+from ellar.common import get, Controller, ControllerBase
 
 
 @Controller
 class ItemsController(ControllerBase):
     @get("/events/{year}/{month}/{day}")
     def events(self, year: int, month: int, day: int):
         return {"date": [year, month, day]}
@@ -159,17 +154,15 @@
 
 You can also use Schema to encapsulate path parameters that depend on each other (and validate them as a group):
 
 ```python
 # project_name/apps/items/controllers.py
 
 import datetime
-from ellar.serializer import Serializer
-from ellar.common import get, Controller, Path
-from ellar.core import ControllerBase
+from ellar.common import Serializer, get, Controller, Path, ControllerBase
 
 
 class PathDate(Serializer):
     year: int
     month: int
     day: int
 
@@ -197,16 +190,15 @@
 but you want the possible valid path parameter values to be predefined, you can use a standard Python `Enum`.
 
 For an example:
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.common import get, Controller
-from ellar.core import ControllerBase
+from ellar.common import get, Controller, ControllerBase
 from enum import Enum
 
 class ModelName(str, Enum):
     alexnet = "alexnet"
     resnet = "resnet"
     lenet = "lenet"
```

### Comparing `ellar-0.3.6/docs/parsing-inputs/query-params.md` & `ellar-0.3.8/docs/parsing-inputs/query-params.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # Query parameters
 
 When you declare other function parameters that are not part of the path parameters, they are automatically interpreted as "query" parameters.
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.common import get, Controller
-from ellar.core import ControllerBase
+from ellar.common import get, Controller, ControllerBase
 
 fake_items_db = [{"item_name": "Foo"}, {"item_name": "Bar"}, {"item_name": "Baz"}]
 
 
 @Controller
 class ItemsController(ControllerBase):
     @get('/weapons')
@@ -34,16 +33,15 @@
 
 
 Note: if you do not annotate your arguments, they will be treated as `str` types:
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.common import get, Controller
-from ellar.core import ControllerBase
+from ellar.common import get, Controller, ControllerBase
 
 fake_items_db = [{"item_name": "Foo"}, {"item_name": "Bar"}, {"item_name": "Baz"}]
 
 
 @Controller
 class ItemsController(ControllerBase):
     @get('/weapons')
@@ -56,16 +54,15 @@
 ### Defaults
 
 As query parameters are not a fixed part of a path, they are optional and can have default values:
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.common import get, Controller
-from ellar.core import ControllerBase
+from ellar.common import get, Controller, ControllerBase
 
 fake_items_db = [{"item_name": "Foo"}, {"item_name": "Bar"}, {"item_name": "Baz"}]
 
 
 @Controller
 class ItemsController(ControllerBase):
     @get('/weapons')
@@ -97,16 +94,15 @@
 ### Required and optional parameters
 
 You can declare required or optional GET parameters in the same way as declaring Python function arguments:
 
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.common import get, Controller
-from ellar.core import ControllerBase
+from ellar.common import get, Controller, ControllerBase
 
 weapons = ["Ninjato", "Shuriken", "Katana", "Kama", "Kunai", "Naginata", "Yari"]
 
 
 @Controller
 class ItemsController(ControllerBase):
     @get("/weapons/search")
@@ -120,16 +116,15 @@
 
 ### GET parameters type conversion
 
 Let's declare multiple type arguments:
 ```python
 # project_name/apps/items/controllers.py
 
-from ellar.common import get, Controller
-from ellar.core import ControllerBase
+from ellar.common import get, Controller, ControllerBase
 from datetime import date
 
 
 @Controller
 class ItemsController(ControllerBase):
     @get("/example")
     def example(self, s: str = None, b: bool = None, d: date = None, i: int = None):
@@ -161,17 +156,15 @@
 You can also use Schema to encapsulate GET parameters:
 
 ```python
 # project_name/apps/items/controllers.py
 
 from typing import List
 from pydantic import Field
-from ellar.serializer import Serializer
-from ellar.common import get, Controller, Query
-from ellar.core import ControllerBase
+from ellar.common import Serializer, get, Controller, Query, ControllerBase
 
 
 
 class Filters(Serializer):
     limit: int = 100
     offset: int = None
     query: str = None
```

### Comparing `ellar-0.3.6/docs/templating/staticfiles.md` & `ellar-0.3.8/docs/templating/staticfiles.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 In addition, Ellar creates a route that mounts the static server at the `/static` path. 
 The path can be modified by providing a new value for the `STATIC_MOUNT_PATH` configuration variable.
 
 ## **Configuring static files**
 
 1. In your config file, define `STATIC_MOUNT_PATH`, for example:
     ```python
-    
-   class Config:
+    class Config:
         STATIC_MOUNT_PATH = '/static'
     ```
 
 2. Store your static files in a folder called **static** in your module. For example **my_module/static/my_module/example.jpg**.
 3. In your templates, use the `url_for` with `static` and `path` parameter to build the URL for the given relative path using the configured in `STATIC_DIRECTORIES`, `STATIC_FOLDER_PACKAGES` or Module.
    ```html
     <img src="{{url_for('static', path='my_module/example.jpg')}}" alt="My image">
@@ -27,57 +26,57 @@
 
 Managing multiple sets of static files in larger projects can be challenging, 
 but by organizing each set of static files within a specific module, 
 it becomes easier to manage and maintain. 
 This approach allows for clear organization and separation of static assets, 
 making it more manageable in a large project.
 
-In our previous project, within the `dogs` module folder, we can create a following directories, `my_static/dogs`. 
-Inside this folder `my_static/dogs`, we can create a file named `example.txt`. 
-This allows us to keep all of the static files related to the dogs module organized in one location `my_static`.
+In our previous project, within the `car` module folder, we can create a following directories, `my_static/car`. 
+Inside this folder `my_static/car`, we can create a file named `example.txt`. 
+This allows us to keep all of the static files related to the car module organized in one location `my_static`.
 
-Next, we tell `DogModule` about our static folder.
+Next, we tell `CarModule` about our static folder.
 
 ```python
-# project_name/apps/dogs/module.py
+# project_name/apps/car/module.py
 
 from ellar.common import Module
 from ellar.core import ModuleBase
 from ellar.di import Container
 
-from .controllers import DogsController
+from .controllers import CarController
 
 
 @Module(
-    controllers=[DogsController], static_folder='my_static'
+    controllers=[CarController], static_folder='my_static'
 )
-class DogsModule(ModuleBase):
+class CarModule(ModuleBase):
     def register_providers(self, container: Container) -> None:
         # for more complicated provider registrations
         # container.register_instance(...)
         pass
 ```
 
 ## **Other Static Configurations**
 In addition to setting static directories within modules, 
 it is also possible to manually specify additional static directories that are not located within a module by using the 
 `STATIC_FOLDER_PACKAGES` and `STATIC_DIRECTORIES` variables in the application's configuration. 
 These variables allow for even more flexibility in organizing and managing static files in a project. 
 These directories will be served by the StaticFiles ASGI class along with the module-scoped static files.
 
-### `STATIC_DIRECTORIES`
+### **`STATIC_DIRECTORIES`**
 `STATIC_DIRECTORIES` variable is a list of directories within the project that contain static files. 
 These directories are not necessarily scoped to a specific module and can be used to serve static files from any location within the project. 
 These directories can be added to the `STATIC_DIRECTORIES` list in the application's configuration.
 
 ```python
 STATIC_DIRECTORIES =  ['project_name/static-files', 'project_name/path/to/static/files']
 ```
 
-### `STATIC_FOLDER_PACKAGES`
+### **`STATIC_FOLDER_PACKAGES`**
 `STATIC_FOLDER_PACKAGES` variable is a list of tuples that contain python packages that hold some static files. 
 These packages should have a `static` folder and the **package name** should be passed as tuple `(package_name, package_path)`, 
 **package_path** is the relative path of static folder.
 
 ```python
 
 STATIC_FOLDER_PACKAGES =  [('bootstrap', 'statics'), ('package-name', 'path/to/static/directory')]
```

### Comparing `ellar-0.3.6/docs/templating/templating.md` & `ellar-0.3.8/docs/templating/templating.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,16 @@
 To render the template, you'll need to use the Jinja2 API in your view function. Here's an example of how you might do this:
 
 ```python
 # main.py
 
 import uvicorn
 from jinja2 import Environment, FileSystemLoader
-from ellar.core.response import HTMLResponse
 from ellar.core import Request, AppFactory
-from ellar.common import ModuleRouter
+from ellar.common import ModuleRouter, HTMLResponse
 from pathlib import Path
 
 BASE_DIR = Path(__file__).parent
 router = ModuleRouter('/template-testing')
 
 # Also create a templates folder at the main.py root dir. And add template.html into it
```

### Comparing `ellar-0.3.6/docs/throttling.md` & `ellar-0.3.8/docs/throttling.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 To get started, you'll need to install the `ellar-throttler` package.
 
 ```shell
 $(venv) pip install ellar-throttler
 ```
 
-## ThrottlerModule
+## **ThrottlerModule**
 
 The `ThrottlerModule` is the main entry point for this package, and can be used in a synchronous or asynchronous manner. 
 All the needs to be passed is the `ttl`, the time to live in seconds for the request tracker, and the `limit`, 
 or how many times an endpoint can be hit before returning a 429 status code.
 
 ```python
 from ellar.common import Module
@@ -198,15 +198,15 @@
 ```
 
 ### **Working with WebSockets**
 To work with Websockets you can extend the `ThrottlerGuard` and override the `handle_request` method with the code below:
 ```python
 from ellar_throttler import ThrottlerGuard
 from ellar.di import injectable
-from ellar.core import IExecutionContext
+from ellar.common import IExecutionContext
 from ellar_throttler import ThrottledException
 
 @injectable()
 class WsThrottleGuard(ThrottlerGuard):
     async def handle_request(self, context: IExecutionContext, limit: int, ttl: int) -> bool:
         websocket_client = context.switch_to_websocket().get_client()
```

### Comparing `ellar-0.3.6/ellar/cache/backends/_aio_cache.py.ellar` & `ellar-0.3.8/ellar/cache/backends/_aio_cache.py.ellar`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/cache/backends/base.py` & `ellar-0.3.8/ellar/cache/backends/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/cache/backends/local_cache.py` & `ellar-0.3.8/ellar/cache/backends/local_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 import typing as t
 from abc import ABC
 from collections import OrderedDict
 
 from anyio import Lock
 
-from ellar.helper.event_loop import get_or_create_eventloop
+from ellar.common.helper.event_loop import get_or_create_eventloop
 
 from ..interface import IBaseCacheBackendAsync
 from ..make_key_decorator import make_key_decorator, make_key_decorator_and_validate
 from ..model import BaseCacheBackend
 
 
 class _LocalMemCacheBackendSync(IBaseCacheBackendAsync, ABC):
```

### Comparing `ellar-0.3.6/ellar/cache/backends/pylib_cache.py` & `ellar-0.3.8/ellar/cache/backends/pylib_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/cache/backends/pymem_cache.py` & `ellar-0.3.8/ellar/cache/backends/pymem_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/cache/backends/redis/backend.py` & `ellar-0.3.8/ellar/cache/backends/redis/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import random
 import typing as t
 from abc import ABC
 
-from ellar.helper.event_loop import get_or_create_eventloop
+from ellar.common.helper.event_loop import get_or_create_eventloop
 
 try:
     from redis.asyncio import Redis  # type: ignore
     from redis.asyncio.connection import ConnectionPool  # type: ignore
 except ImportError as e:  # pragma: no cover
     raise RuntimeError(
         "To use `RedisCacheBackend`, you have to install 'redis' package e.g. `pip install redis`"
```

### Comparing `ellar-0.3.6/ellar/cache/backends/serializer.py` & `ellar-0.3.8/ellar/cache/backends/serializer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/cache/decorator.py` & `ellar-0.3.8/ellar/cache/decorator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import typing as t
 import uuid
 from functools import wraps
 
 from ellar.cache.interface import ICacheService
-from ellar.common import Context, Provide, extra_args
-from ellar.core import ExecutionContext, IExecutionContext
-from ellar.core.params import ExtraEndpointArg
-from ellar.helper import is_async_callable
+from ellar.common import Context, IExecutionContext, Provide, extra_args
+from ellar.common.helper import is_async_callable
+from ellar.common.params import ExtraEndpointArg
 
 
 class _CacheDecorator:
     __slots__ = (
         "_is_async",
         "_key_prefix",
         "_version",
@@ -37,18 +36,22 @@
         self._version = version
         self._backend = backend
         self._func = func
         self._ttl = ttl
 
         # create extra args
         self._cache_service_arg = ExtraEndpointArg(
-            name=f"cache_service_{uuid.uuid4().hex[:4]}", annotation=ICacheService, default_value=Provide()  # type: ignore
+            name=f"cache_service_{uuid.uuid4().hex[:4]}",
+            annotation=ICacheService,  # type:ignore[misc]
+            default_value=Provide(),
         )
         self._context_arg = ExtraEndpointArg(
-            name=f"route_context_{uuid.uuid4().hex[:4]}", annotation=IExecutionContext, default_value=Context()  # type: ignore
+            name=f"route_context_{uuid.uuid4().hex[:4]}",
+            annotation=IExecutionContext,  # type:ignore[misc]
+            default_value=Context(),
         )
         # apply extra_args to endpoint
         extra_args(self._cache_service_arg, self._context_arg)(func)
         self._make_key_callback: t.Callable[[IExecutionContext, str], str] = (
             make_key_callback or self.route_cache_make_key
         )
 
@@ -125,17 +128,15 @@
 
 def cache(
     ttl: t.Union[float, int],
     *,
     key_prefix: str = "",
     version: str = None,
     backend: str = "default",
-    make_key_callback: t.Callable[
-        [t.Union[ExecutionContext, IExecutionContext], str], str
-    ] = None,
+    make_key_callback: t.Callable[[IExecutionContext, str], str] = None,
 ) -> t.Callable:
     """
 
     :param ttl: the time to live
     :param key_prefix: cache key prefix
     :param version: will be used in constructing the key
     :param backend: Cache Backend to use. Default is `default`
```

### Comparing `ellar-0.3.6/ellar/cache/interface.py` & `ellar-0.3.8/ellar/cache/interface.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/cache/make_key_decorator.py` & `ellar-0.3.8/ellar/cache/make_key_decorator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import functools
 import typing as t
 
-from ellar.helper import is_async_callable
+from ellar.common.helper import is_async_callable
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from .model import BaseCacheBackend
 
 
 class MakeKeyDecorator:
     __slots__ = ("_func", "_validate", "_is_async")
```

### Comparing `ellar-0.3.6/ellar/cache/model.py` & `ellar-0.3.8/ellar/cache/model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/cache/module.py` & `ellar-0.3.8/ellar/cache/module.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing as t
 
-from ellar.common import Module
-from ellar.core import Config, DynamicModule, IModuleSetup, ModuleBase, ModuleSetup
+from ellar.common import IModuleSetup, Module
+from ellar.core import Config, DynamicModule, ModuleBase, ModuleSetup
 from ellar.di import ProviderConfig
 
 from .interface import ICacheService
 from .model import BaseCacheBackend
 from .schema import CacheModuleSchemaSetup
 from .service import CacheService
```

### Comparing `ellar-0.3.6/ellar/cache/schema.py` & `ellar-0.3.8/ellar/cache/schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/cache/service.py` & `ellar-0.3.8/ellar/cache/service.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/commands/base.py` & `ellar-0.3.8/ellar/common/commands/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/common/decorators/__init__.py` & `ellar-0.3.8/ellar/common/decorators/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import typing as t
 
 from .base import set_metadata
-from .command import command
 from .controller import Controller
 from .exception import exception_handler
 from .extra_args import extra_args
 from .file import file
 from .guards import Guards
 from .html import render, template_filter, template_global
 from .middleware import middleware
@@ -20,15 +19,14 @@
     "Version",
     "Guards",
     "template_filter",
     "template_global",
     "file",
     "render",
     "exception_handler",
-    "command",
     "set_metadata",
     "middleware",
     "openapi_info",
     "Module",
     "extra_args",
 ]
```

### Comparing `ellar-0.3.6/ellar/common/decorators/command.py` & `ellar-0.3.8/ellar/common/commands/decorator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing as t
 
 import click
 from typer.core import TyperCommand
 from typer.models import CommandFunctionType, CommandInfo
 
-from ellar.constants import CALLABLE_COMMAND_INFO
+from ellar.common.constants import CALLABLE_COMMAND_INFO
 
 
 @t.no_type_check
 def command(
     name: t.Optional[str] = None,
     cls: t.Optional[t.Type[click.Command]] = None,
     context_settings: t.Optional[t.Dict[t.Any, t.Any]] = None,
```

### Comparing `ellar-0.3.6/ellar/common/decorators/controller.py` & `ellar-0.3.8/ellar/common/decorators/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import inspect
 import typing as t
 from abc import ABC
 from types import FunctionType
 
-from ellar.compatible import AttributeDict
-from ellar.constants import (
+from ellar.common.compatible import AttributeDict
+from ellar.common.constants import (
     CONTROLLER_CLASS_KEY,
     CONTROLLER_METADATA,
     CONTROLLER_OPERATION_HANDLER_KEY,
     CONTROLLER_WATERMARK,
     NOT_SET,
     OPERATION_ENDPOINT_KEY,
-    REFLECT_TYPE,
 )
-from ellar.core import ControllerBase
-from ellar.core.controller import ControllerType
-from ellar.core.exceptions import ImproperConfiguration
-from ellar.core.routing.controller import ControllerRouteOperationBase
+from ellar.common.exceptions import ImproperConfiguration
+from ellar.common.models import ControllerBase, ControllerType
+from ellar.common.routing.controller import ControllerRouteOperationBase
 from ellar.di import RequestScope, injectable
-from ellar.reflect import reflect
+from ellar.reflect import REFLECT_TYPE, reflect
 
 
 def get_route_functions(
     cls: t.Type,
 ) -> t.Iterable[t.Union[t.Callable, ControllerRouteOperationBase]]:
     for method in cls.__dict__.values():
         if hasattr(method, OPERATION_ENDPOINT_KEY) or isinstance(
@@ -82,16 +80,14 @@
     Controller Class Decorator
     :param prefix: Route Prefix default=[ControllerName]
     :param tag: OPENAPI tag
     :param description: OPENAPI description
     :param external_doc_description: OPENAPI External Doc Description
     :param external_doc_url: OPENAPI External Document URL
     :param name: route name prefix for url reversing, eg name:route_name default=''
-    :param version: default URL versioning for all defined route in a controller
-    :param guards: default guard for all routes defined under this controller
     :param include_in_schema: include controller in OPENAPI schema
     :return: t.Type[ControllerBase]
     """
     ...
 
 
 def Controller(
```

### Comparing `ellar-0.3.6/ellar/common/decorators/exception.py` & `ellar-0.3.8/ellar/common/decorators/exception.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing as t
 
 from pydantic import BaseModel
 
-from ellar.constants import EXCEPTION_HANDLERS_KEY
+from ellar.common.constants import EXCEPTION_HANDLERS_KEY
 
 
 class ValidateExceptionHandler(BaseModel):
     key: t.Union[int, t.Type[Exception]]
     value: t.Union[t.Callable, t.Type]
```

### Comparing `ellar-0.3.6/ellar/common/decorators/file.py` & `ellar-0.3.8/ellar/common/decorators/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import inspect
 import typing as t
 import warnings
 
-from ellar.constants import NOT_SET, RESPONSE_OVERRIDE_KEY
-from ellar.core.response.model import (
-    FileResponseModel,
-    IResponseModel,
-    StreamingResponseModel,
-)
-from ellar.shortcuts import fail_silently
+from ellar.common.constants import NOT_SET, RESPONSE_OVERRIDE_KEY
+from ellar.common.interfaces import IResponseModel
+from ellar.common.shortcuts import fail_silently
 
+from ..responses.models import FileResponseModel, StreamingResponseModel
 from .base import set_metadata as set_meta
 
 
 def file(media_type: t.Optional[str] = NOT_SET, streaming: bool = False) -> t.Callable:
     """
     ========= ROUTE FUNCTION DECORATOR ==============
```

### Comparing `ellar-0.3.6/ellar/common/decorators/guards.py` & `ellar-0.3.8/ellar/common/decorators/guards.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as t
 
-from ellar.constants import GUARDS_KEY
+from ellar.common.constants import GUARDS_KEY
 
 from .base import set_metadata as set_meta
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.core.guard import GuardCanActivate
+    from ellar.common.models import GuardCanActivate
 
 
 def Guards(
     *_guards: t.Union[t.Type["GuardCanActivate"], "GuardCanActivate"]
 ) -> t.Callable:
     """
     =========CONTROLLER AND ROUTE FUNCTION DECORATOR ==============
```

### Comparing `ellar-0.3.6/ellar/common/decorators/html.py` & `ellar-0.3.8/ellar/common/decorators/html.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import asyncio
 import inspect
 import typing as t
 import warnings
 
-from ellar.constants import (
+from ellar.common.constants import (
     NOT_SET,
     RESPONSE_OVERRIDE_KEY,
     TEMPLATE_FILTER_KEY,
     TEMPLATE_GLOBAL_KEY,
 )
-from ellar.core.exceptions import ImproperConfiguration
-from ellar.core.response.model import HTMLResponseModel
-from ellar.core.templating import TemplateFunctionData
-from ellar.helper import class_base_function_regex, get_name
-from ellar.shortcuts import fail_silently
-from ellar.types import TemplateFilterCallable, TemplateGlobalCallable
+from ellar.common.exceptions import ImproperConfiguration
+from ellar.common.helper import class_base_function_regex, get_name
+from ellar.common.responses.models import HTMLResponseModel
+from ellar.common.shortcuts import fail_silently
+from ellar.common.templating import TemplateFunctionData
+from ellar.common.types import TemplateFilterCallable, TemplateGlobalCallable
 
 from .base import set_metadata as set_meta
 
 
 class RenderDecoratorException(Exception):
     pass
```

### Comparing `ellar-0.3.6/ellar/common/decorators/modules.py` & `ellar-0.3.8/ellar/common/decorators/modules.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import inspect
 import typing as t
 from functools import partial
 from pathlib import Path
 
 from starlette.routing import Host, Mount
 
-from ellar.compatible import AttributeDict
-from ellar.constants import MODULE_METADATA, MODULE_WATERMARK
-from ellar.core import ControllerBase
-from ellar.core.exceptions import ImproperConfiguration
-from ellar.core.modules.base import ModuleBase, ModuleBaseMeta
-from ellar.core.routing import ModuleMount, ModuleRouter
+from ellar.common.compatible import AttributeDict
+from ellar.common.constants import MODULE_METADATA, MODULE_WATERMARK
+from ellar.common.exceptions import ImproperConfiguration
+from ellar.common.models import ControllerBase
+from ellar.common.routing import ModuleMount, ModuleRouter
 from ellar.di import ProviderConfig, SingletonScope, injectable
 from ellar.reflect import reflect
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.commands import EllarTyper
+    from ellar.common.commands import EllarTyper
 
 
 def _wrapper(
     target: t.Type,
     watermark_key: str,
     metadata_keys: t.List[str],
     name: str,
@@ -30,37 +29,27 @@
 
     if not isinstance(target, type):
         raise ImproperConfiguration(f"{name} is a class decorator - {target}")
 
     if not kwargs.base_directory:
         kwargs.update(base_directory=Path(inspect.getfile(target)).resolve().parent)
 
-    if type(target) != ModuleBaseMeta:
-        attr: t.Dict = {
-            item: getattr(target, item) for item in dir(target) if "__" not in item
-        }
-        target = type(
-            target.__name__,
-            (target, ModuleBase),
-            attr,
-        )
-
     reflect.define_metadata(watermark_key, True, target)
     for key in metadata_keys:
         reflect.define_metadata(key, kwargs[key], target)
     injectable(SingletonScope)(target)
-    return t.cast(t.Type, target)
+    return target
 
 
 def Module(
     *,
     name: t.Optional[str] = None,
     controllers: t.Sequence[t.Union[t.Type[ControllerBase], t.Type]] = tuple(),
     routers: t.Sequence[t.Union[ModuleRouter, ModuleMount, Mount, Host]] = tuple(),
-    providers: t.Sequence[t.Union[t.Type, ProviderConfig]] = tuple(),
+    providers: t.Sequence[t.Union[t.Type, "ProviderConfig"]] = tuple(),
     template_folder: t.Optional[str] = "templates",
     base_directory: t.Optional[t.Union[Path, str]] = None,
     static_folder: str = "static",
     modules: t.Sequence[t.Union[t.Type, t.Any]] = tuple(),
     commands: t.Sequence[t.Union[t.Callable, "EllarTyper"]] = tuple(),
 ) -> t.Callable:
     """
```

### Comparing `ellar-0.3.6/ellar/common/decorators/openapi.py` & `ellar-0.3.8/ellar/common/decorators/openapi.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing as t
 
-from ellar.compatible import AttributeDict
-from ellar.constants import OPENAPI_KEY
+from ellar.common.compatible import AttributeDict
+from ellar.common.constants import OPENAPI_KEY
 
 from .base import set_metadata as set_meta
 
 
 def openapi_info(
     operation_id: t.Optional[str] = None,
     summary: t.Optional[str] = None,
```

### Comparing `ellar-0.3.6/ellar/common/decorators/serializer.py` & `ellar-0.3.8/ellar/common/decorators/serializer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import typing as t
 
-from ellar.constants import SERIALIZER_FILTER_KEY
+from ellar.common.constants import SERIALIZER_FILTER_KEY
+from ellar.common.serializer import SerializerFilter
 
 from .base import set_metadata as set_meta
 
 
 def serializer_filter(
     include: t.Optional[
         t.Union[t.Set[t.Union[int, str]], t.Mapping[t.Union[int, str], t.Any]]
@@ -27,15 +28,14 @@
     :param by_alias:
     :param skip_defaults:
     :param exclude_unset:
     :param exclude_defaults:
     :param exclude_none:
     :return:
     """
-    from ellar.serializer import SerializerFilter
 
     return set_meta(
         SERIALIZER_FILTER_KEY,
         SerializerFilter(
             include=include,
             exclude=exclude,
             by_alias=by_alias,
```

### Comparing `ellar-0.3.6/ellar/common/routing/params.py` & `ellar-0.3.8/ellar/common/routing/params.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import typing as t
 
 from pydantic.fields import Undefined
 from starlette.responses import Response
 
-from ellar.core.connection import HTTPConnection, Request, WebSocket
-from ellar.core.context import IExecutionContext
-from ellar.core.params import params
-from ellar.core.params.resolvers.non_parameter import (
+from ellar.common.interfaces import IExecutionContext
+from ellar.common.params.resolvers.non_parameter import (
     ConnectionParam,
     ExecutionContextParameter,
     HostRequestParam,
     ProviderParameterInjector,
     RequestParameter,
     ResponseRequestParam,
     SessionRequestParam,
     WebSocketParameter,
 )
-from ellar.types import T
+
+from ..params import params
+from ..types import T
+
+if t.TYPE_CHECKING:  # pragma: no cover
+    from ellar.core import HTTPConnection, Request, WebSocket
 
 
 def Path(
     default: t.Any = ...,
     *,
     alias: t.Optional[str] = None,
     title: t.Optional[str] = None,
@@ -36,15 +39,15 @@
     examples: t.Optional[t.Dict[str, t.Any]] = None,
     deprecated: t.Optional[bool] = None,
     **extra: t.Any,
 ) -> t.Any:
     """
     Defines expected path in Route Function Parameter
     """
-    return params.Path(
+    return params.PathFieldInfo(
         default=default,
         alias=alias,
         title=title,
         description=description,
         gt=gt,
         ge=ge,
         lt=lt,
@@ -76,15 +79,15 @@
     examples: t.Optional[t.Dict[str, t.Any]] = None,
     deprecated: t.Optional[bool] = None,
     **extra: t.Any,
 ) -> t.Any:
     """
     Defines expected query in Route Function Parameter
     """
-    return params.Query(
+    return params.QueryFieldInfo(
         default,
         alias=alias,
         title=title,
         description=description,
         gt=gt,
         ge=ge,
         lt=lt,
@@ -117,15 +120,15 @@
     examples: t.Optional[t.Dict[str, t.Any]] = None,
     deprecated: t.Optional[bool] = None,
     **extra: t.Any,
 ) -> t.Any:
     """
     Defines expected header in Route Function Parameter
     """
-    return params.Header(
+    return params.HeaderFieldInfo(
         default,
         alias=alias,
         convert_underscores=convert_underscores,
         title=title,
         description=description,
         gt=gt,
         ge=ge,
@@ -158,15 +161,15 @@
     examples: t.Optional[t.Dict[str, t.Any]] = None,
     deprecated: t.Optional[bool] = None,
     **extra: t.Any,
 ) -> t.Any:
     """
     Defines expected cookie in Route Function Parameter
     """
-    return params.Cookie(
+    return params.CookieFieldInfo(
         default,
         alias=alias,
         title=title,
         description=description,
         gt=gt,
         ge=ge,
         lt=lt,
@@ -199,15 +202,15 @@
     example: t.Any = Undefined,
     examples: t.Optional[t.Dict[str, t.Any]] = None,
     **extra: t.Any,
 ) -> t.Any:
     """
     Defines expected body object in Route Function Parameter
     """
-    return params.Body(
+    return params.BodyFieldInfo(
         default,
         embed=embed,
         media_type=media_type,
         alias=alias,
         title=title,
         description=description,
         gt=gt,
@@ -240,15 +243,15 @@
     example: t.Any = Undefined,
     examples: t.Optional[t.Dict[str, t.Any]] = None,
     **extra: t.Any,
 ) -> t.Any:
     """
     Defines expected form parameter in Route Function Parameter
     """
-    return params.Form(
+    return params.FormFieldInfo(
         default,
         media_type=media_type,
         alias=alias,
         title=title,
         description=description,
         gt=gt,
         ge=ge,
@@ -280,15 +283,15 @@
     example: t.Any = Undefined,
     examples: t.Optional[t.Dict[str, t.Any]] = None,
     **extra: t.Any,
 ) -> t.Any:
     """
     Defines expected file data in Route Function Parameter
     """
-    return params.File(
+    return params.FileFieldInfo(
         default,
         media_type=media_type,
         alias=alias,
         title=title,
         description=description,
         gt=gt,
         ge=ge,
@@ -321,15 +324,15 @@
     example: t.Any = Undefined,
     examples: t.Optional[t.Dict[str, t.Any]] = None,
     **extra: t.Any,
 ) -> t.Any:
     """
     Defines expected body object in websocket Route Function Parameter
     """
-    return params.WsBody(
+    return params.WsBodyFieldInfo(
         default,
         embed=embed,
         media_type=media_type,
         alias=alias,
         title=title,
         description=description,
         gt=gt,
@@ -341,36 +344,36 @@
         regex=regex,
         example=example,
         examples=examples,
         **extra,
     )
 
 
-def Http() -> HTTPConnection:
+def Http() -> "HTTPConnection":
     """
     Route Function Parameter for retrieving Current Request Instance
     :return: Request
     """
-    return t.cast(Request, ConnectionParam())
+    return ConnectionParam()  # type: ignore[return-value]
 
 
-def Req() -> Request:
+def Req() -> "Request":
     """
     Route Function Parameter for retrieving Current Request Instance
     :return: Request
     """
-    return t.cast(Request, RequestParameter())
+    return RequestParameter()  # type: ignore[return-value]
 
 
-def Ws() -> WebSocket:
+def Ws() -> "WebSocket":
     """
     Route Function Parameter for retrieving Current WebSocket Instance
     :return: WebSocket
     """
-    return t.cast(WebSocket, WebSocketParameter())
+    return WebSocketParameter()  # type: ignore[return-value]
 
 
 def Context() -> IExecutionContext:
     """
     Route Function Parameter for retrieving Current IExecutionContext Instance
     :return: IExecutionContext
     """
```

### Comparing `ellar-0.3.6/ellar/compatible/cache_properties.py` & `ellar-0.3.8/ellar/common/compatible/cache_properties.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing as t
 
-from ellar.constants import NOT_SET
-from ellar.types import T
+from ..constants import NOT_SET
+from ..types import T
 
 try:
     from functools import cached_property
 except (Exception,):  # pragma: no cover
 
     class _CachedProperty(property, t.Generic[T]):
         def __init__(
```

### Comparing `ellar-0.3.6/ellar/compatible/dict.py` & `ellar-0.3.8/ellar/common/compatible/dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing as t
 
-from ellar.types import KT, VT
+from ..types import KT, VT
 
 
 class AttributeDictAccessMixin:
     def __getattr__(self, name) -> VT:
         if name in self:
             value = self.get(name)
             return value
```

### Comparing `ellar-0.3.6/ellar/compatible/emails.py` & `ellar-0.3.8/ellar/common/compatible/emails.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing as t
 
-from ellar.logger import logger
+from ..logger import logger
 
 try:
     import email_validator
 
     assert email_validator
     from pydantic import EmailStr
 except ImportError:  # pragma: no cover
```

### Comparing `ellar-0.3.6/ellar/core/__init__.py` & `ellar-0.3.8/ellar/core/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,43 @@
 import typing as t
 
 from .conf import Config, ConfigDefaultTypesMixin
-from .connection import Request, WebSocket
-from .context import ExecutionContext, HostContext, IExecutionContext, IHostContext
-from .controller import ControllerBase
+from .connection import HTTPConnection, Request, WebSocket
+from .context import ExecutionContext, HostContext
 from .factory import AppFactory
-from .guard import BaseAPIKey, BaseAuthGuard, BaseHttpAuth, GuardCanActivate
-from .main import App
-from .modules import DynamicModule, IModuleSetup, ModuleBase, ModuleSetup
-from .response import (
-    FileResponse,
-    HTMLResponse,
-    JSONResponse,
-    ORJSONResponse,
-    PlainTextResponse,
-    RedirectResponse,
-    Response,
-    StreamingResponse,
-    UJSONResponse,
+from .guard import (
+    APIKeyCookie,
+    APIKeyHeader,
+    APIKeyQuery,
+    HttpBasicAuth,
+    HttpBearerAuth,
+    HttpDigestAuth,
 )
-from .templating import render_template, render_template_string
+from .main import App
+from .modules import DynamicModule, ModuleBase, ModuleSetup
+from .services import Reflector
 
 __all__ = [
     "App",
     "AppFactory",
-    "render_template",
-    "render_template_string",
+    "HTTPConnection",
     "ExecutionContext",
-    "IExecutionContext",
-    "IHostContext",
     "HostContext",
-    "ControllerBase",
     "ConfigDefaultTypesMixin",
     "ModuleBase",
-    "BaseAPIKey",
-    "BaseAuthGuard",
-    "IModuleSetup",
-    "BaseHttpAuth",
-    "GuardCanActivate",
     "Config",
-    "JSONResponse",
-    "UJSONResponse",
-    "ORJSONResponse",
-    "StreamingResponse",
-    "HTMLResponse",
-    "FileResponse",
-    "PlainTextResponse",
-    "RedirectResponse",
-    "Response",
     "Request",
     "WebSocket",
     "ModuleSetup",
     "DynamicModule",
+    "Reflector",
+    "APIKeyCookie",
+    "APIKeyHeader",
+    "APIKeyQuery",
+    "HttpBasicAuth",
+    "HttpBearerAuth",
+    "HttpDigestAuth",
 ]
 
 
 def __dir__() -> t.List[str]:
     return sorted(__all__)  # pragma: no cover
```

### Comparing `ellar-0.3.6/ellar/core/conf/app_settings_models.py` & `ellar-0.3.8/ellar/core/conf/app_settings_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import typing as t
 
 from pydantic import Field, validator
 from pydantic.json import ENCODERS_BY_TYPE as encoders_by_type
 from starlette.exceptions import HTTPException as StarletteHTTPException
 from starlette.websockets import WebSocketClose
 
-from ellar.constants import DEFAULT_LOGGING as default_logging, LOG_LEVELS as log_levels
-from ellar.core.response import JSONResponse, PlainTextResponse
+from ellar.common.constants import (
+    DEFAULT_LOGGING as default_logging,
+    LOG_LEVELS as log_levels,
+)
+from ellar.common.responses import JSONResponse, PlainTextResponse
+from ellar.common.serializer import Serializer, SerializerFilter
+from ellar.common.types import ASGIApp, TReceive, TScope, TSend
 from ellar.core.versioning import DefaultAPIVersioning
-from ellar.serializer import Serializer, SerializerFilter
-from ellar.types import ASGIApp, TReceive, TScope, TSend
 
 from .mixins import ConfigDefaultTypesMixin, TExceptionHandler, TMiddleware, TVersioning
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.core.main import App
```

### Comparing `ellar-0.3.6/ellar/core/conf/config.py` & `ellar-0.3.8/ellar/core/conf/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as t
 
 from starlette.config import environ
 
-from ellar.compatible.dict import AttributeDictAccessMixin, DataMutableMapper
-from ellar.constants import ELLAR_CONFIG_MODULE
-from ellar.helper.importer import import_from_string
-from ellar.types import VT
+from ellar.common.compatible.dict import AttributeDictAccessMixin, DataMutableMapper
+from ellar.common.constants import ELLAR_CONFIG_MODULE
+from ellar.common.helper.importer import import_from_string
+from ellar.common.types import VT
 
 from .app_settings_models import ConfigValidationSchema
 from .mixins import ConfigDefaultTypesMixin
 
 
 class ConfigRuntimeError(RuntimeError):
     pass
```

### Comparing `ellar-0.3.6/ellar/core/conf/mixins.py` & `ellar-0.3.8/ellar/core/conf/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import inspect
 import typing as t
 
 from starlette.responses import JSONResponse
 from starlette.types import ASGIApp
 
-from ellar.constants import LOG_LEVELS as log_levels
-from ellar.core.exceptions.interfaces import IExceptionHandler
+from ellar.common.constants import LOG_LEVELS as log_levels
+from ellar.common.interfaces import IExceptionHandler
 from ellar.core.middleware import Middleware
 from ellar.core.versioning import BaseAPIVersioning
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.core import App
 
 __all__ = [
@@ -139,15 +139,15 @@
 
     # logging configuration
     LOGGING_CONFIG: t.Optional[t.Dict[str, t.Any]]
 
     # logging Level
     LOG_LEVEL: t.Optional[log_levels]
 
-    # CORS Middleware setup (ellar.core.middleware.CORSMiddleware)
+    # CORS Middleware setup (ellar.middleware.CORSMiddleware)
     CORS_ALLOW_ORIGINS: t.List[str]
     CORS_ALLOW_METHODS: t.List[str]
     CORS_ALLOW_HEADERS: t.List[str]
     CORS_ALLOW_CREDENTIALS: bool
 
     CORS_ALLOW_ORIGIN_REGEX: t.Optional[str]
     CORS_EXPOSE_HEADERS: t.Sequence[str]
```

### Comparing `ellar-0.3.6/ellar/core/connection/http.py` & `ellar-0.3.8/ellar/core/connection/http.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as t
 
 from starlette.requests import (
     HTTPConnection as StarletteHTTPConnection,
     Request as StarletteRequest,
 )
 
-from ellar.constants import SCOPE_SERVICE_PROVIDER
+from ellar.common.constants import SCOPE_SERVICE_PROVIDER
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.di import EllarInjector
 
 
 class HTTPConnection(StarletteHTTPConnection):
     @property
```

### Comparing `ellar-0.3.6/ellar/core/context/execution.py` & `ellar-0.3.8/ellar/core/context/execution.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import typing as t
 
-from ellar.constants import CONTROLLER_CLASS_KEY
-from ellar.services.reflector import Reflector
-from ellar.types import TReceive, TScope, TSend
+from ellar.common.constants import CONTROLLER_CLASS_KEY
+from ellar.common.interfaces import IExecutionContext
+from ellar.common.models import ControllerBase
+from ellar.common.types import TReceive, TScope, TSend
+from ellar.core.services.reflector import Reflector
 
 from .host import HostContext
-from .interface import IExecutionContext
-
-if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.core.controller import ControllerBase
 
 
 class ExecutionContext(HostContext, IExecutionContext):
     """
     Context for route functions and controllers
     """
```

### Comparing `ellar-0.3.6/ellar/core/context/factory.py` & `ellar-0.3.8/ellar/core/context/factory.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import typing as t
 
-from ellar.di import injectable, request_scope
-from ellar.services import Reflector
-from ellar.types import TReceive, TScope, TSend
-
-from .exceptions import HostContextException
-from .execution import ExecutionContext
-from .host import HostContext
-from .http import HTTPHostContext
-from .interface import (
+from ellar.common.constants import empty_receive, empty_send
+from ellar.common.exceptions import HostContextException
+from ellar.common.interfaces import (
     IExecutionContext,
     IExecutionContextFactory,
     IHostContext,
     IHostContextFactory,
     IHTTPConnectionContextFactory,
     IWebSocketContextFactory,
-    empty_receive,
-    empty_send,
 )
+from ellar.common.types import TReceive, TScope, TSend
+from ellar.core.services import Reflector
+from ellar.di import injectable, request_scope
+
+from .execution import ExecutionContext
+from .host import HostContext
+from .http import HTTPHostContext
 from .websocket import WebSocketHostContext
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.core.routing import RouteOperationBase
+    from ellar.common.routing import RouteOperationBase
 
 
 class HTTPConnectionContextFactory(IHTTPConnectionContextFactory):
     context_type = HTTPHostContext
 
     def validate(self, context: IHostContext) -> None:
         """
```

### Comparing `ellar-0.3.6/ellar/core/context/host.py` & `ellar-0.3.8/ellar/core/context/host.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import typing as t
 
-from ellar.compatible import cached_property
-from ellar.constants import SCOPE_SERVICE_PROVIDER
-from ellar.types import TReceive, TScope, TSend
-
-from .interface import (
-    IHostContext,
+from ellar.common import (
     IHTTPConnectionContextFactory,
     IHTTPHostContext,
     IWebSocketContextFactory,
     IWebSocketHostContext,
 )
+from ellar.common.compatible import cached_property
+from ellar.common.constants import SCOPE_SERVICE_PROVIDER
+from ellar.common.interfaces import IHostContext
+from ellar.common.types import TReceive, TScope, TSend
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.core.main import App
     from ellar.di import EllarInjector
 
 
 class HostContext(IHostContext):
```

### Comparing `ellar-0.3.6/ellar/core/context/http.py` & `ellar-0.3.8/ellar/core/context/http.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import typing as t
 
 from starlette.background import BackgroundTasks
 from starlette.responses import Response
 
-from ellar.compatible import cached_property
-from ellar.constants import SCOPED_RESPONSE
+from ellar.common.compatible import cached_property
+from ellar.common.constants import SCOPED_RESPONSE
+from ellar.common.exceptions import HostContextException
+from ellar.common.interfaces import IHTTPHostContext
+from ellar.common.types import TReceive, TScope, TSend
 from ellar.core.connection import HTTPConnection, Request
-from ellar.types import TReceive, TScope, TSend
-
-from .exceptions import HostContextException
-from .interface import IHTTPHostContext
 
 
 class HTTPHostContext(IHTTPHostContext):
     """
     Provides a context around HTTP Connection
     """
```

### Comparing `ellar-0.3.6/ellar/core/context/interface.py` & `ellar-0.3.8/ellar/common/interfaces/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,45 @@
 import typing as t
 from abc import ABC, ABCMeta, abstractmethod
 
-from ellar.core.connection import HTTPConnection, Request, WebSocket
-from ellar.core.response import Response
-from ellar.types import T, TMessage, TReceive, TScope, TSend
+from starlette.requests import empty_send
+from starlette.responses import Response
+
+from ellar.common.constants import empty_receive
+from ellar.common.types import T, TReceive, TScope, TSend
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.core import ControllerBase
-    from ellar.core.main import App
-    from ellar.core.routing import RouteOperationBase
+    from ellar.common.models import ControllerBase
+    from ellar.common.routing import RouteOperationBase
+    from ellar.core import App, HTTPConnection, Request, WebSocket
     from ellar.di.injector import EllarInjector
 
 
-async def empty_receive() -> t.NoReturn:  # pragma: no cover
-    raise RuntimeError("Receive channel has not been made available")
-
-
-async def empty_send(message: TMessage) -> t.NoReturn:  # pragma: no cover
-    raise RuntimeError("Send channel has not been made available")
-
-
 class IHTTPHostContext(ABC):
     @property
     @abstractmethod
     def has_response(self) -> bool:
         """checks if response was requested before send"""
 
     @abstractmethod
-    def get_response(self) -> Response:
+    def get_response(self) -> "Response":
         """Gets response"""
 
     @abstractmethod
-    def get_request(self) -> Request:
+    def get_request(self) -> "Request":
         """Returns Request instance"""
 
     @abstractmethod
-    def get_client(self) -> HTTPConnection:
+    def get_client(self) -> "HTTPConnection":
         """Returns HTTPConnection instance"""
 
 
 class IWebSocketHostContext(ABC):
     @abstractmethod
-    def get_client(self) -> WebSocket:
+    def get_client(self) -> "WebSocket":
         """Returns WebSocket instance"""
 
 
 class IHostContext(ABC, metaclass=ABCMeta):
     @abstractmethod
     def get_service_provider(self) -> "EllarInjector":
         """Gets  RequestServiceProvider instance"""
```

### Comparing `ellar-0.3.6/ellar/core/context/websocket.py` & `ellar-0.3.8/ellar/core/context/websocket.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from ellar.compatible import cached_property
+from ellar.common.compatible import cached_property
+from ellar.common.interfaces import IWebSocketHostContext
+from ellar.common.types import TReceive, TScope, TSend
 from ellar.core.connection import WebSocket
-from ellar.types import TReceive, TScope, TSend
-
-from .interface import IWebSocketHostContext
 
 
 class WebSocketHostContext(IWebSocketHostContext):
     """
     Provides a context around websocket session
     """
```

### Comparing `ellar-0.3.6/ellar/core/controller/model.py` & `ellar-0.3.8/ellar/common/models/controller.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing as t
 
-from ellar.core.context import ExecutionContext
+from ..interfaces import IExecutionContext
 
 
 class ControllerType(type):
     _controller_name: t.Optional[str]
 
     @t.no_type_check
     def __new__(mcls, name, bases, namespace):
@@ -22,8 +22,8 @@
         """ """
         return f"{cls.controller_class_name()}/{name}"
 
 
 class ControllerBase(metaclass=ControllerType):
     # `context` variable will change based on the route function called on the APIController
     # that way we can get some specific items things that belong the route function during execution
-    context: t.Optional[ExecutionContext] = None
+    context: t.Optional[IExecutionContext] = None
```

### Comparing `ellar-0.3.6/ellar/core/converters.py` & `ellar-0.3.8/ellar/common/converters.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/core/core_service_registration.py` & `ellar-0.3.8/ellar/core/core_service_registration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import typing as t
 
-from ellar.di import EllarInjector
-from ellar.services.reflector import Reflector
-
-from .context import (
-    ExecutionContextFactory,
-    HostContextFactory,
+from ellar.common import (
+    IExceptionMiddlewareService,
     IExecutionContextFactory,
     IHostContextFactory,
     IHTTPConnectionContextFactory,
     IWebSocketContextFactory,
 )
+from ellar.core.services import Reflector
+from ellar.di import EllarInjector
+
+from .context import ExecutionContextFactory, HostContextFactory
 from .context.factory import HTTPConnectionContextFactory, WebSocketContextFactory
-from .exceptions.interfaces import IExceptionMiddlewareService
 from .exceptions.service import ExceptionMiddlewareService
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.core.conf import Config
 
 
 class CoreServiceRegistration:
```

### Comparing `ellar-0.3.6/ellar/core/datastructures.py` & `ellar-0.3.8/ellar/common/datastructures.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/core/exceptions/__init__.py` & `ellar-0.3.8/ellar/common/exceptions/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from starlette.exceptions import HTTPException, WebSocketException
 
-from .base import APIException
-from .exceptions_types import (
+from .api import (
+    APIException,
     AuthenticationFailed,
     ImproperConfiguration,
     MethodNotAllowed,
     NotAcceptable,
     NotAuthenticated,
     NotFound,
     PermissionDenied,
     UnsupportedMediaType,
 )
-from .interfaces import IExceptionHandler, IExceptionMiddlewareService
+from .context import ExecutionContextException, HostContextException
 from .validation import RequestValidationError, WebSocketRequestValidationError
 
 __all__ = [
-    "IExceptionHandler",
-    "IExceptionMiddlewareService",
+    "HostContextException",
+    "ExecutionContextException",
     "HTTPException",
+    "WebSocketException",
     "ImproperConfiguration",
     "APIException",
     "WebSocketRequestValidationError",
     "RequestValidationError",
     "AuthenticationFailed",
     "NotAuthenticated",
     "PermissionDenied",
     "NotFound",
     "MethodNotAllowed",
     "NotAcceptable",
     "UnsupportedMediaType",
-    "WebSocketException",
 ]
```

### Comparing `ellar-0.3.6/ellar/core/exceptions/base.py` & `ellar-0.3.8/ellar/common/exceptions/api/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/core/exceptions/callable_exceptions.py` & `ellar-0.3.8/ellar/common/exceptions/callable_exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import typing as t
 
 from starlette.concurrency import run_in_threadpool
 from starlette.responses import Response
 
-from ellar.core.context import IHostContext
-from ellar.helper import is_async_callable
-
-from .interfaces import IExceptionHandler
+from ellar.common.helper import is_async_callable
+from ellar.common.interfaces import IExceptionHandler, IHostContext
 
 
 class CallableExceptionHandler(IExceptionHandler):
     """
     Default Exception Handler Setup for functions
 
     usage:
```

### Comparing `ellar-0.3.6/ellar/core/exceptions/exceptions_types.py` & `ellar-0.3.8/ellar/common/exceptions/api/exceptions_types.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/core/exceptions/handlers.py` & `ellar-0.3.8/ellar/common/exceptions/handlers.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 from starlette import status
 from starlette.exceptions import (
     HTTPException as StarletteHTTPException,
     WebSocketException as StarletteWebSocketException,
 )
 from starlette.responses import Response
 
-from ellar.core.context import IHostContext
-from ellar.serializer import serialize_object
+from ellar.common.interfaces import IExceptionHandler, IHostContext
+from ellar.common.serializer import serialize_object
 
-from .base import APIException
-from .interfaces import IExceptionHandler
+from .api import APIException
 from .validation import RequestValidationError
 
 
 class HTTPExceptionHandler(IExceptionHandler):
     exception_type_or_code = StarletteHTTPException
 
     async def catch(
```

### Comparing `ellar-0.3.6/ellar/core/exceptions/interfaces.py` & `ellar-0.3.8/ellar/common/interfaces/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing as t
 from abc import ABC, abstractmethod
 
 from starlette.responses import Response
 
-from ellar.core.context import IHostContext
+from .context import IHostContext
 
 
 class IExceptionHandler(ABC, t.Iterable):
     def __eq__(self, other: t.Any) -> bool:
         if isinstance(other, IExceptionHandler):
             return other.exception_type_or_code == self.exception_type_or_code
         return False
```

### Comparing `ellar-0.3.6/ellar/core/exceptions/service.py` & `ellar-0.3.8/ellar/core/exceptions/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import typing as t
 
-from ellar.di import injectable
-
-from .handlers import (
+from ellar.common.exceptions.handlers import (
     APIExceptionHandler,
     HTTPExceptionHandler,
     RequestValidationErrorHandler,
     WebSocketExceptionHandler,
 )
-from .interfaces import IExceptionHandler, IExceptionMiddlewareService
+from ellar.common.interfaces import IExceptionHandler, IExceptionMiddlewareService
+from ellar.di import injectable
 
 
 @injectable()
 class ExceptionMiddlewareService(IExceptionMiddlewareService):
     DEFAULTS: t.List[IExceptionHandler] = [
         HTTPExceptionHandler(),
         APIExceptionHandler(),
```

### Comparing `ellar-0.3.6/ellar/core/exceptions/validation.py` & `ellar-0.3.8/ellar/common/exceptions/validation.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/core/factory.py` & `ellar-0.3.8/ellar/core/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import typing as t
 from collections import OrderedDict
 from pathlib import Path
 from uuid import uuid4
 
 from starlette.routing import Host, Mount
 
-from ellar.constants import MODULE_METADATA, MODULE_WATERMARK
+from ellar.common import EllarTyper
+from ellar.common.constants import MODULE_METADATA, MODULE_WATERMARK
+from ellar.common.models import GuardCanActivate
 from ellar.core.main import App
 from ellar.core.modules import DynamicModule, ModuleBase, ModuleSetup
 from ellar.di import EllarInjector, ProviderConfig
 from ellar.reflect import reflect
 
 from .conf import Config
 from .core_service_registration import CoreServiceRegistration
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.commands import EllarTyper
-    from ellar.core import GuardCanActivate
-    from ellar.core.routing import ModuleMount, ModuleRouter
+    from ellar.common.routing import ModuleMount, ModuleRouter
 
 
 class AppFactory:
     """
     Factory for creating Ellar Application
     """
 
@@ -193,15 +193,15 @@
             providers=providers,
             template_folder=template_folder,
             base_directory=base_directory,
             static_folder=static_folder,
             modules=modules,
             commands=commands,
         )
-        app_factory_module = type(f"Module{uuid4().hex[:6]}", (ModuleBase,), {})
+        app_factory_module = type(f"Module{uuid4().hex[:6]}", (), {})
         module(app_factory_module)
         return cls._create_app(
             module=app_factory_module,
             config_module=config_module,
             global_guards=global_guards,
         )
```

### Comparing `ellar-0.3.6/ellar/core/guard/apikey.py` & `ellar-0.3.8/ellar/core/guard/apikey.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import typing as t
 from abc import ABC
 
+from ellar.common.models import BaseAPIKey
 from ellar.core.connection import HTTPConnection
 
-from .base import BaseAPIKey
-
 
 class APIKeyQuery(BaseAPIKey, ABC):
     openapi_in: str = "query"
 
     def _get_key(self, connection: HTTPConnection) -> t.Optional[t.Any]:
         return connection.query_params.get(self.parameter_name)
```

### Comparing `ellar-0.3.6/ellar/core/guard/base.py` & `ellar-0.3.8/ellar/common/models/guard.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import typing as t
 from abc import ABC, ABCMeta, abstractmethod
 
-from pydantic import BaseModel
 from starlette.exceptions import HTTPException
 from starlette.status import HTTP_401_UNAUTHORIZED, HTTP_403_FORBIDDEN
 
-from ellar.core.connection import HTTPConnection
-from ellar.core.context import IExecutionContext
-from ellar.core.exceptions import APIException
+from ellar.common.exceptions import APIException
+from ellar.common.interfaces import IExecutionContext
+from ellar.common.serializer.guard import (
+    HTTPAuthorizationCredentials,
+    HTTPBasicCredentials,
+)
+
+if t.TYPE_CHECKING:  # pragma: no cover
+    from ellar.core.connection import HTTPConnection
 
 
 class GuardCanActivate(ABC, metaclass=ABCMeta):
     exception_class: t.Union[
         t.Type[HTTPException], t.Type[APIException]
     ] = HTTPException
     status_code: int = HTTP_403_FORBIDDEN
@@ -29,15 +34,17 @@
     status_code = HTTP_401_UNAUTHORIZED
     openapi_scope: t.List = []
     openapi_in: t.Optional[str] = None
     openapi_description: t.Optional[str] = None
     openapi_name: t.Optional[str] = None
 
     @abstractmethod
-    async def handle_request(self, *, connection: HTTPConnection) -> t.Optional[t.Any]:
+    async def handle_request(
+        self, *, connection: "HTTPConnection"
+    ) -> t.Optional[t.Any]:
         pass
 
     @classmethod
     @abstractmethod
     def get_guard_scheme(cls) -> t.Dict:
         pass
 
@@ -47,45 +54,35 @@
         if result:
             # auth parameter on request
             connection.scope["user"] = result
             return True
         return False
 
 
-class HTTPBasicCredentials(BaseModel):
-    username: str
-    password: str
-
-
-class HTTPAuthorizationCredentials(BaseModel):
-    scheme: str
-    credentials: str
-
-
 class BaseAPIKey(BaseAuthGuard, ABC, metaclass=ABCMeta):
     exception_class = APIException
     parameter_name: str = "key"
 
     def __init__(self) -> None:
         self.name = self.parameter_name
         super().__init__()
 
-    async def handle_request(self, connection: HTTPConnection) -> t.Optional[t.Any]:
+    async def handle_request(self, connection: "HTTPConnection") -> t.Optional[t.Any]:
         key = self._get_key(connection)
         if not key:
             self.raise_exception()
         return await self.authenticate(connection, key)
 
     @abstractmethod
-    def _get_key(self, connection: HTTPConnection) -> t.Optional[t.Any]:
+    def _get_key(self, connection: "HTTPConnection") -> t.Optional[t.Any]:
         pass  # pragma: no cover
 
     @abstractmethod
     async def authenticate(
-        self, connection: HTTPConnection, key: t.Optional[t.Any]
+        self, connection: "HTTPConnection", key: t.Optional[t.Any]
     ) -> t.Optional[t.Any]:
         pass  # pragma: no cover
 
     @classmethod
     def get_guard_scheme(cls) -> t.Dict:
         assert cls.openapi_in, "openapi_in is required"
         return {
@@ -107,26 +104,26 @@
         if authorization:
             return authorization.partition(" ")
         return None, None, None
 
     @abstractmethod
     async def authenticate(
         self,
-        connection: HTTPConnection,
+        connection: "HTTPConnection",
         credentials: t.Union[HTTPBasicCredentials, HTTPAuthorizationCredentials],
     ) -> t.Optional[t.Any]:
         pass  # pragma: no cover
 
-    async def handle_request(self, connection: HTTPConnection) -> t.Optional[t.Any]:
+    async def handle_request(self, connection: "HTTPConnection") -> t.Optional[t.Any]:
         credentials = self._get_credentials(connection)
         return await self.authenticate(connection, credentials)
 
     @abstractmethod
     def _get_credentials(
-        self, connection: HTTPConnection
+        self, connection: "HTTPConnection"
     ) -> t.Union[HTTPBasicCredentials, HTTPAuthorizationCredentials]:
         pass  # pragma: no cover
 
     @classmethod
     def get_guard_scheme(cls) -> t.Dict:
         assert cls.openapi_scheme, "openapi_scheme is required"
         return {
```

### Comparing `ellar-0.3.6/ellar/core/guard/http.py` & `ellar-0.3.8/ellar/core/guard/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import binascii
 import typing as t
 from abc import ABC
 from base64 import b64decode
 
+from ellar.common.exceptions import APIException, AuthenticationFailed
+from ellar.common.models import BaseHttpAuth
+from ellar.common.serializer.guard import (
+    HTTPAuthorizationCredentials,
+    HTTPBasicCredentials,
+)
 from ellar.core.connection import HTTPConnection
-from ellar.core.exceptions import APIException, AuthenticationFailed
-
-from .base import BaseHttpAuth, HTTPAuthorizationCredentials, HTTPBasicCredentials
 
 
 class HttpBearerAuth(BaseHttpAuth, ABC):
     exception_class = APIException
     openapi_scheme: str = "bearer"
     openapi_bearer_format: t.Optional[str] = None
     header: str = "Authorization"
```

### Comparing `ellar-0.3.6/ellar/core/main.py` & `ellar-0.3.8/ellar/core/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import logging
 import typing as t
 
 from starlette.routing import BaseRoute, Mount
 
-from ellar.constants import LOG_LEVELS
-from ellar.core.datastructures import State, URLPath
-from ellar.core.exceptions.interfaces import (
-    IExceptionHandler,
-    IExceptionMiddlewareService,
-)
-from ellar.core.guard import GuardCanActivate
+from ellar.common.compatible import cached_property
+from ellar.common.constants import LOG_LEVELS
+from ellar.common.datastructures import State, URLPath
+from ellar.common.interfaces import IExceptionHandler, IExceptionMiddlewareService
+from ellar.common.logger import logger
+from ellar.common.models import GuardCanActivate
+from ellar.common.templating import Environment
+from ellar.common.types import ASGIApp, T, TReceive, TScope, TSend
 from ellar.core.middleware import (
     CORSMiddleware,
     ExceptionMiddleware,
     Middleware,
     RequestServiceProviderMiddleware,
     RequestVersioningMiddleware,
     TrustedHostMiddleware,
 )
 from ellar.core.modules import (
     DynamicModule,
-    ModuleBase,
     ModuleRefBase,
     ModuleSetup,
     ModuleTemplateRef,
 )
 from ellar.core.routing import ApplicationRouter
-from ellar.core.templating import AppTemplating, Environment
+from ellar.core.services import Reflector
+from ellar.core.templating import AppTemplating
 from ellar.core.versioning import BaseAPIVersioning, VersioningSchemes
 from ellar.di.injector import EllarInjector
-from ellar.logger import logger
-from ellar.types import ASGIApp, T, TReceive, TScope, TSend
 
 from .conf import Config
+from .modules import ModuleBase
 
 
 class App(AppTemplating):
     def __init__(
         self,
         config: "Config",
         injector: EllarInjector,
@@ -256,7 +256,11 @@
                 self._exception_handlers.append(exception_handler)
                 _added_any = True
         if _added_any:
             self.rebuild_middleware_stack()
 
     def rebuild_middleware_stack(self) -> None:
         self.middleware_stack = self.build_middleware_stack()
+
+    @cached_property
+    def reflector(self) -> Reflector:
+        return self.injector.get(Reflector)  # type: ignore[no-any-return]
```

### Comparing `ellar-0.3.6/ellar/core/middleware/__init__.py` & `ellar-0.3.8/ellar/core/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/core/middleware/di.py` & `ellar-0.3.8/ellar/core/middleware/di.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-import typing as t
-
 from starlette.middleware.errors import ServerErrorMiddleware
 from starlette.requests import Request as StarletteRequest
 from starlette.responses import JSONResponse
 
-from ellar.constants import SCOPE_RESPONSE_STARTED, SCOPE_SERVICE_PROVIDER
+from ellar.common.constants import SCOPE_RESPONSE_STARTED, SCOPE_SERVICE_PROVIDER
+from ellar.common.interfaces import IExceptionHandler, IHostContextFactory
+from ellar.common.responses import Response
+from ellar.common.types import ASGIApp, TMessage, TReceive, TScope, TSend
 from ellar.core.connection.http import Request
-from ellar.core.context import IHostContextFactory
-from ellar.core.response import Response
 from ellar.di import EllarInjector
-from ellar.types import ASGIApp, TMessage, TReceive, TScope, TSend
-
-if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.core.exceptions.interfaces import IExceptionHandler
 
 
 class RequestServiceProviderMiddleware(ServerErrorMiddleware):
     def __init__(
         self,
         app: ASGIApp,
         *,
```

### Comparing `ellar-0.3.6/ellar/core/middleware/exceptions.py` & `ellar-0.3.8/ellar/core/middleware/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import typing as t
 
 from starlette.exceptions import HTTPException
 
-from ellar.constants import SCOPE_SERVICE_PROVIDER
-from ellar.core.context import IHostContextFactory
-from ellar.types import ASGIApp, TMessage, TReceive, TScope, TSend
+from ellar.common.constants import SCOPE_SERVICE_PROVIDER
+from ellar.common.interfaces import IHostContextFactory
+from ellar.common.types import ASGIApp, TMessage, TReceive, TScope, TSend
 
 if t.TYPE_CHECKING:  # pragma: no cover
+    from ellar.core.exceptions.service import ExceptionMiddlewareService
     from ellar.di import EllarInjector
-    from ellar.exceptions.service import ExceptionMiddlewareService
 
 
 class ExceptionMiddleware:
     def __init__(
         self,
         app: ASGIApp,
         exception_middleware_service: "ExceptionMiddlewareService",
```

### Comparing `ellar-0.3.6/ellar/core/middleware/function.py` & `ellar-0.3.8/ellar/core/middleware/function.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing as t
 
 from starlette.responses import Response
 
+from ellar.common.interfaces import IHostContext, IHostContextFactory
+from ellar.common.types import ASGIApp, TReceive, TScope, TSend
 from ellar.core.connection import HTTPConnection
-from ellar.core.context import IHostContext, IHostContextFactory
-from ellar.types import ASGIApp, TReceive, TScope, TSend
 
 AwaitableCallable = t.Callable[..., t.Awaitable]
 DispatchFunction = t.Callable[
     [IHostContext, AwaitableCallable], t.Awaitable[t.Optional[Response]]
 ]
 T = t.TypeVar("T")
```

### Comparing `ellar-0.3.6/ellar/core/middleware/versioning.py` & `ellar-0.3.8/ellar/core/middleware/versioning.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import typing as t
 
 from starlette.types import ASGIApp
 
-from ellar.constants import SCOPE_API_VERSIONING_RESOLVER
+from ellar.common.constants import SCOPE_API_VERSIONING_RESOLVER
+from ellar.common.types import TReceive, TScope, TSend
 from ellar.core.versioning import BaseAPIVersioning
-from ellar.types import TReceive, TScope, TSend
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.conf import Config
+    from ellar.core.conf import Config
 
 
 class RequestVersioningMiddleware:
     def __init__(self, app: ASGIApp, *, debug: bool, config: "Config") -> None:
         self.app = app
         self.debug = debug
         self.config = config
```

### Comparing `ellar-0.3.6/ellar/core/modules/base.py` & `ellar-0.3.8/ellar/core/modules/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import typing as t
 
 from injector import Binder, Module as _InjectorModule
 
-from ellar.constants import MODULE_FIELDS
-from ellar.core.modules.builder import ModuleBaseBuilder
+from ellar.common.constants import MODULE_FIELDS
 from ellar.di.injector import Container
 
+from .builder import ModuleBaseBuilder
+
 if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.conf import Config
+    from ellar.core.conf import Config
 
 
 class ModuleBaseMeta(type):
     __MODULE_FIELDS__: t.Dict = {}
 
     @t.no_type_check
     def __init__(cls, name, bases, namespace) -> None:
```

### Comparing `ellar-0.3.6/ellar/core/modules/builder.py` & `ellar-0.3.8/ellar/core/modules/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import typing as t
 
-from ellar.constants import (
+from starlette.middleware import Middleware
+
+from ellar.common.compatible import AttributeDict
+from ellar.common.constants import (
     EXCEPTION_HANDLERS_KEY,
     MIDDLEWARE_HANDLERS_KEY,
     MODULE_FIELDS,
     TEMPLATE_FILTER_KEY,
     TEMPLATE_GLOBAL_KEY,
 )
+from ellar.common.exceptions.callable_exceptions import CallableExceptionHandler
+from ellar.core.middleware import FunctionBasedMiddleware
 from ellar.reflect import reflect
 
-from ..exceptions.callable_exceptions import CallableExceptionHandler
 from .helper import module_callable_factory
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.core.middleware.schema import MiddlewareSchema
-    from ellar.core.modules.base import ModuleBase, ModuleBaseMeta
-    from ellar.core.templating import TemplateFunctionData
+    from ellar.common.templating import TemplateFunctionData
+    from ellar.core.modules import ModuleBase, ModuleBaseMeta
 
 
 class ModuleBaseBuilder:
     __slots__ = ("_cls", "_actions")
 
     def __init__(self, cls: t.Union[t.Type["ModuleBase"], "ModuleBaseMeta"]) -> None:
         self._cls = cls
@@ -40,19 +43,23 @@
         for k, v in exception_dict.items():
             func = CallableExceptionHandler(
                 self._cls, callable_exception_handler=v, exc_class_or_status_code=k
             )
             reflect.define_metadata(EXCEPTION_HANDLERS_KEY, [func], self._cls)
 
     @t.no_type_check
-    def middleware_config(self, middleware: "MiddlewareSchema") -> None:
-        middleware.dispatch = module_callable_factory(middleware.dispatch, self._cls)
+    def middleware_config(self, middleware: AttributeDict) -> None:
+        dispatch = module_callable_factory(middleware.dispatch, self._cls)
         reflect.define_metadata(
             MIDDLEWARE_HANDLERS_KEY,
-            [middleware.create_middleware()],
+            [
+                Middleware(
+                    FunctionBasedMiddleware, dispatch=dispatch, **middleware.options
+                )
+            ],
             self._cls,
         )
 
     def template_filter_config(self, template_filter: "TemplateFunctionData") -> None:
         reflect.define_metadata(
             TEMPLATE_FILTER_KEY,
             {
```

### Comparing `ellar-0.3.6/ellar/core/modules/config.py` & `ellar-0.3.8/ellar/core/modules/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import dataclasses
 import typing as t
 
 from starlette.routing import BaseRoute
 
 import ellar.core.main as main
-import ellar.di as di
-from ellar.constants import MODULE_METADATA, MODULE_REF_TYPES
+from ellar.common.constants import MODULE_METADATA, MODULE_WATERMARK
+from ellar.common.models import ControllerBase
 from ellar.core.conf import Config
+from ellar.di import MODULE_REF_TYPES, Container, EllarInjector
 from ellar.reflect import reflect
 
-from .base import ModuleBase
 from .ref import ModuleRefBase, create_module_ref_factor
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.commands import EllarTyper
-    from ellar.core import ControllerBase
+    from ellar.common import EllarTyper, IModuleSetup
+
+    from .base import ModuleBase
 
 
 @dataclasses.dataclass
 class DynamicModule:
     # Module type to be configured
     module: t.Type[t.Union["ModuleBase", t.Any]]
 
@@ -36,15 +37,15 @@
 
     commands: t.Sequence[t.Union[t.Callable, "EllarTyper"]] = dataclasses.field(
         default_factory=lambda: tuple()
     )
     _is_configured: bool = False
 
     def __post_init__(self) -> None:
-        if not isinstance(self.module, type) or not issubclass(self.module, ModuleBase):
+        if not reflect.get_metadata(MODULE_WATERMARK, self.module):
             raise Exception(f"{self.module.__name__} is not a valid Module")
 
     def apply_configuration(self) -> None:
         if self._is_configured:
             return
 
         kwargs = dict(
@@ -87,30 +88,30 @@
 
     @Module(modules=[ModuleSetup(MyModule, inject=[Config, Foo], factory=module_a_configuration_factory), ])
     Class ApplicationModule(ModuleBase):
         pass
     """
 
     # Module type to be configured
-    module: t.Type[t.Union[ModuleBase, "IModuleSetup", t.Any]]
+    module: t.Type[t.Union["ModuleBase", "IModuleSetup", t.Any]]
 
     # `inject` property holds collection types to be injected to `use_factory` method.
     # the order at which the types are defined becomes the order at which they are injected.
 
     ref_type: str = MODULE_REF_TYPES.DYNAMIC
 
     inject: t.Sequence[t.Union[t.Type, t.Any]] = dataclasses.field(
         default_factory=lambda: []
     )
 
     init_kwargs: t.Dict[t.Any, t.Any] = dataclasses.field(default_factory=lambda: {})
     factory: t.Callable[..., DynamicModule] = None  # type: ignore[assignment]
 
     def __post_init__(self) -> None:
-        if not isinstance(self.module, type) or not issubclass(self.module, ModuleBase):
+        if not reflect.get_metadata(MODULE_WATERMARK, self.module):
             raise Exception(f"{self.module.__name__} is not a valid Module")
 
         if main.App in self.inject:
             self.ref_type = MODULE_REF_TYPES.APP_DEPENDENT
 
     @property
     def has_factory_function(self) -> bool:
@@ -123,99 +124,48 @@
                 return False
 
             if inject_size == 1 and self.inject[0] == Config:
                 return False
             return True
 
     def get_module_ref(
-        self, config: "Config", container: di.Container
+        self, config: "Config", container: Container
     ) -> t.Union[ModuleRefBase, "ModuleSetup"]:
         if self.has_factory_function or self.ref_type == MODULE_REF_TYPES.APP_DEPENDENT:
             return self
 
         if self.factory:
             return self.configure_with_factory(config, container)
 
         return create_module_ref_factor(
             self.module, config, container, **self.init_kwargs
         )
 
     def configure_with_factory(
-        self, config: "Config", container: di.Container
+        self, config: "Config", container: Container
     ) -> ModuleRefBase:
         services = self._get_services(container.injector)
 
         res = self.factory(self.module, *services)
         if not isinstance(res, DynamicModule):
             raise Exception(
                 f"Factory function for {self.module.__name__} module "
                 f"configuration must return `DynamicModule` instance"
             )
         res.apply_configuration()
 
         init_kwargs = dict(self.init_kwargs)
         return create_module_ref_factor(self.module, config, container, **init_kwargs)
 
-    def _get_services(self, injector: di.EllarInjector) -> t.List:
+    def _get_services(self, injector: EllarInjector) -> t.List:
         """
         Get list of services to be injected to the factory function.
         :param injector:
         :return:
         """
         res = []
         for service in self.inject:
             res.append(injector.get(service))
         return res
 
     def __hash__(self) -> int:  # pragma: no cover
         return hash(self.module)
-
-
-class IModuleSetup:
-    """Modules that must have a custom setup should inherit from IModuleSetup"""
-
-    @classmethod
-    @t.no_type_check
-    def setup(cls, *args: t.Any, **kwargs: t.Any) -> DynamicModule:
-        """
-        Provides Dynamic set up for a module.
-
-        Usage:
-
-        class MyModule(ModuleBase, IModuleSetup):
-            @classmethod
-            def setup(cls, param1: Any, param2: Any) -> DynamicModule:
-                :return DynamicModule(module, provider=[], controllers=[], routers=[])
-
-
-        @Module(modules=[MyModule.setup(param1='xyz', param2='abc')])
-        class ApplicationModule(ModuleBase):
-            pass
-        """
-
-    @classmethod
-    @t.no_type_check
-    def register_setup(cls, *args: t.Any, **kwargs: t.Any) -> ModuleSetup:
-        """
-        The module defines all the dependencies its needs for its setup.
-        Allowing parameters needed for setting up the module to come from app Config.
-
-        Usage:
-
-        class MyModule(ModuleBase, IModuleSetup):
-            @classmethod
-            def register_setup(cls) -> ModuleSetup:
-                :return ModuleSetup(cls, inject=[Config, OtherServices], factory=cls.setup_module_factory)
-
-            @staticmethod
-            def setup_module_factory(module: t.Type['MyModule'], config: Config, others: OtherServices) -> DynamicModule:
-                param1 = config.param1
-                param2 = config.param2
-
-                :return DynamicModule(module, provider=[], controllers=[], routers=[])
-
-
-        @Module(modules=[MyModule.register_setup()])
-        class ApplicationModule(ModuleBase):
-            pass
-
-        """
```

### Comparing `ellar-0.3.6/ellar/core/modules/helper.py` & `ellar-0.3.8/ellar/core/modules/helper.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/core/modules/ref.py` & `ellar-0.3.8/ellar/core/modules/ref.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 import inspect
 import typing as t
 from abc import ABC, abstractmethod
 from pathlib import Path
 
 from starlette.routing import BaseRoute, Mount
 
-from ellar.constants import (
-    CONTROLLER_WATERMARK,
+from ellar.common.constants import (
     EXCEPTION_HANDLERS_KEY,
     MIDDLEWARE_HANDLERS_KEY,
     MODULE_METADATA,
-    MODULE_REF_TYPES,
     MODULE_WATERMARK,
     TEMPLATE_FILTER_KEY,
     TEMPLATE_GLOBAL_KEY,
 )
-from ellar.core.controller import ControllerType
-from ellar.core.routing import ModuleMount
-from ellar.core.routing.router.module import controller_router_factory
-from ellar.core.templating import ModuleTemplating
-from ellar.di import Container, ProviderConfig, injectable, is_decorated_with_injectable
+from ellar.common.models import ControllerBase
+from ellar.common.routing import ModuleMount
+from ellar.common.routing.builder import get_controller_builder_factory
+from ellar.common.templating import ModuleTemplating
+from ellar.di import (
+    MODULE_REF_TYPES,
+    Container,
+    ProviderConfig,
+    injectable,
+    is_decorated_with_injectable,
+)
 from ellar.di.providers import ModuleProvider
 from ellar.reflect import reflect
 
 from .base import ModuleBase, ModuleBaseMeta
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.core import Config, ControllerBase
+    from ellar.core import Config
 
 
 class InvalidModuleTypeException(Exception):
     pass
 
 
 def create_module_ref_factor(
@@ -80,15 +84,16 @@
         """gets module ref container"""
 
     @property
     def routes(self) -> t.List[BaseRoute]:
         return []
 
     def run_module_register_services(self) -> None:
-        self.module.before_init(config=self.config)
+        if hasattr(self.module, "before_init"):
+            self.module.before_init(config=self.config)
         _module_type_instance = self.get_module_instance()
         self.container.install(_module_type_instance)  # support for injector module
         # _module_type_instance.register_services(self.container)
 
     def _build_init_kwargs(self, kwargs: t.Dict) -> t.Dict:
         _result = dict()
         if hasattr(self.module, "__init__"):
@@ -139,37 +144,32 @@
         return self._container
 
     @property
     def config(self) -> "Config":
         return self._config
 
     def _register_module(self) -> None:
-        _module = self.module
         if not is_decorated_with_injectable(self.module):
-            _module = injectable()(self.module)
+            self._module_type = injectable()(self.module)
         self.container.register(
-            _module, ModuleProvider(self.module, **self._init_kwargs)
+            self._module_type, ModuleProvider(self.module, **self._init_kwargs)
         )
 
 
 class ModuleTemplateRef(ModuleRefBase, ModuleTemplating):
     ref_type: str = MODULE_REF_TYPES.TEMPLATE
 
     def __init__(
         self,
         module_type: t.Union[t.Type[ModuleBase], t.Type],
         *,
         container: Container,
         config: "Config",
         **kwargs: t.Any,
     ) -> None:
-        assert (
-            type(module_type) == ModuleBaseMeta
-        ), f"Module Type must be a subclass of ModuleBase;\n Invalid Type[{module_type}]"
-
         self._module_type: t.Type[ModuleBase] = module_type
         self._container = container
         self._config = config
         self._init_kwargs = self._build_init_kwargs(kwargs)
         self._register_module()
 
         self._template_folder: t.Optional[str] = reflect.get_metadata(
@@ -186,17 +186,19 @@
         )
 
         self._routers: t.Sequence[
             t.Union[BaseRoute, ModuleMount, Mount]
         ] = self._get_all_routers()
         self._flatten_routes: t.List[BaseRoute] = []
 
-        self.scan_templating_filters()
-        self.scan_exceptions_handlers()
-        self.scan_middleware()
+        if isinstance(self.module, type) and issubclass(self.module, ModuleBase):
+            self.scan_templating_filters()
+            self.scan_exceptions_handlers()
+            self.scan_middleware()
+
         self.register_providers()
         self.register_controllers()
         self._build_flatten_routes()
 
     @property
     def module(self) -> t.Type[ModuleBase]:
         return self._module_type
@@ -226,14 +228,16 @@
             #     continue
             # if isinstance(router, BaseRoute):
             #     self._flatten_routes.append(router)
             if isinstance(router, BaseRoute):
                 self._flatten_routes.append(router)
 
     def _register_module(self) -> None:
+        if not is_decorated_with_injectable(self.module):
+            self._module_type = injectable()(self.module)
         self.container.register(
             self.module, ModuleProvider(self.module, **self._init_kwargs)
         )
 
     def scan_templating_filters(self) -> None:
         templating_filter = (
             reflect.get_metadata(TEMPLATE_FILTER_KEY, self._module_type) or {}
@@ -288,12 +292,11 @@
     #     _module_type_instance.application_ready(app)
 
     def _get_all_routers(self) -> t.Sequence[t.Union[ModuleMount, Mount, BaseRoute]]:
         _routers = list(
             reflect.get_metadata(MODULE_METADATA.ROUTERS, self._module_type) or []
         )
         for controller in self._controllers:
-            assert reflect.get_metadata(
-                CONTROLLER_WATERMARK, controller
-            ) and isinstance(controller, ControllerType), "Invalid Controller Type."
-            _routers.append(controller_router_factory(controller))
+            factory_builder = get_controller_builder_factory(type(controller))
+            factory_builder.check_type(controller)
+            _routers.append(factory_builder.build(controller))
         return _routers
```

### Comparing `ellar-0.3.6/ellar/core/params/__init__.py` & `ellar-0.3.8/ellar/common/params/resolvers/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,40 @@
-from .args import (
-    EndpointArgsModel,
-    ExtraEndpointArg,
-    RequestEndpointArgsModel,
-    WebsocketEndpointArgsModel,
-)
-from .params import Body, Cookie, File, Form, Header, Param, ParamTypes, Path, Query
-from .resolvers import (
-    BaseConnectionParameterResolver,
+from .base import (
+    BaseRouteParameterResolver,
     IRouteParameterResolver,
-    NonParameterResolver,
+    RouteParameterModelField,
+)
+from .bulk_parameter import (
+    BulkBodyParameterResolver,
+    BulkFormParameterResolver,
+    BulkParameterResolver,
+)
+from .non_parameter.base import BaseConnectionParameterResolver, NonParameterResolver
+from .parameter import (
+    BodyParameterResolver,
+    CookieParameterResolver,
+    FileParameterResolver,
+    FormParameterResolver,
+    HeaderParameterResolver,
+    PathParameterResolver,
+    QueryParameterResolver,
+    WsBodyParameterResolver,
 )
 
 __all__ = [
-    "WebsocketEndpointArgsModel",
-    "RequestEndpointArgsModel",
-    "ExtraEndpointArg",
-    "EndpointArgsModel",
+    "IRouteParameterResolver",
+    "RouteParameterModelField",
+    "BaseRouteParameterResolver",
+    "BodyParameterResolver",
+    "WsBodyParameterResolver",
+    "FormParameterResolver",
+    "PathParameterResolver",
+    "CookieParameterResolver",
+    "HeaderParameterResolver",
+    "BulkParameterResolver",
+    "BulkBodyParameterResolver",
+    "BulkFormParameterResolver",
+    "QueryParameterResolver",
+    "FileParameterResolver",
     "NonParameterResolver",
     "BaseConnectionParameterResolver",
-    "IRouteParameterResolver",
-    "Body",
-    "Cookie",
-    "File",
-    "Form",
-    "Header",
-    "Path",
-    "Query",
-    "Param",
-    "ParamTypes",
 ]
```

### Comparing `ellar-0.3.6/ellar/core/params/args/base.py` & `ellar-0.3.8/ellar/common/params/args/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 from starlette.requests import (
     HTTPConnection as StarletteHTTPConnection,
     Request as StarletteRequest,
 )
 from starlette.responses import Response
 from starlette.websockets import WebSocket as StarletteWebSocket
 
-from ellar.constants import ROUTE_OPENAPI_PARAMETERS, primitive_types, sequence_types
-from ellar.core.connection.http import HTTPConnection, Request
-from ellar.core.connection.websocket import WebSocket
-from ellar.core.context import ExecutionContext, IExecutionContext
-from ellar.core.exceptions import ImproperConfiguration
+from ellar.common.constants import (
+    ROUTE_OPENAPI_PARAMETERS,
+    primitive_types,
+    sequence_types,
+)
+from ellar.common.exceptions import ImproperConfiguration
+from ellar.common.interfaces import IExecutionContext
 
 from .. import params
 from ..helpers import is_scalar_field, is_scalar_sequence_field
 from ..resolvers import (
     BaseRouteParameterResolver,
     IRouteParameterResolver,
     NonParameterResolver,
@@ -42,38 +44,34 @@
     BulkArgsResolverGenerator,
     FormArgsResolverGenerator,
     PathArgsResolverGenerator,
     QueryHeaderResolverGenerator,
 )
 
 DEFAULT_RESOLVERS: t.Dict[t.Type, t.Type[NonParameterResolver]] = {
-    Request: RequestParameter,
     StarletteRequest: RequestParameter,
-    WebSocket: WebSocketParameter,
     StarletteWebSocket: WebSocketParameter,
     Response: ResponseRequestParam,
-    HTTPConnection: ConnectionParam,
     StarletteHTTPConnection: ConnectionParam,
     IExecutionContext: ExecutionContextParameter,
-    ExecutionContext: ExecutionContextParameter,
 }
 
 
 def add_default_resolver(
     type_identifier: t.Type, resolver_type: t.Type[NonParameterResolver]
 ) -> None:  # pragma: no cover
     DEFAULT_RESOLVERS.update({type_identifier: resolver_type})
 
 
 class EndpointArgsModel:
     _bulk_resolvers_generators = {
-        str(params.Form): FormArgsResolverGenerator,
-        str(params.Path): PathArgsResolverGenerator,
-        str(params.Query): QueryHeaderResolverGenerator,
-        str(params.Header): QueryHeaderResolverGenerator,
+        str(params.FormFieldInfo): FormArgsResolverGenerator,
+        str(params.PathFieldInfo): PathArgsResolverGenerator,
+        str(params.QueryFieldInfo): QueryHeaderResolverGenerator,
+        str(params.HeaderFieldInfo): QueryHeaderResolverGenerator,
     }
 
     _provider_skip = primitive_types + sequence_types + (Representation,)
 
     __slots__ = (
         "path",
         "_computation_models",
@@ -105,15 +103,15 @@
         ] = None
         self._route_models: t.List[IRouteParameterResolver] = []
         self._extra_endpoint_args: t.List[ExtraEndpointArg] = (
             list(extra_endpoint_args) if extra_endpoint_args else []
         )
 
     def get_resolver_generator(
-        self, param: params.Param
+        self, param: params.ParamFieldInfo
     ) -> t.Type[BulkArgsResolverGenerator]:
         return self._bulk_resolvers_generators.get(
             str(type(param)), BulkArgsResolverGenerator
         )
 
     def get_route_models(self) -> t.List[IRouteParameterResolver]:
         """
@@ -137,17 +135,17 @@
     ) -> ModelField:
         _converter_signature = inspect.signature(convertor.convert)
         assert (
             _converter_signature.return_annotation is not inspect.Parameter.empty
         ), f"{convertor.__class__.__name__} Convertor must have return type"
         _type = _converter_signature.return_annotation
         return get_parameter_field(
-            param_default=params.Path(),
+            param_default=params.PathFieldInfo(),
             param_annotation=_type,
-            default_field_info=params.Path,
+            default_field_info=params.PathFieldInfo,
             param_name=param_name,
         )
 
     def get_omitted_prefix(self) -> t.List[ModelField]:
         """
         Tracks for omitted path parameters for OPENAPI purpose
         :return: None
@@ -168,23 +166,23 @@
         :return:
         """
         self._computation_models = defaultdict(list)
         self.compute_route_parameter_list()
         self.compute_extra_route_args()
         self.build_body_field()
         self._route_models = (
-            self._computation_models[params.Header.in_.value]
-            + self._computation_models[params.Path.in_.value]
-            + self._computation_models[params.Query.in_.value]
-            + self._computation_models[params.Cookie.in_.value]
+            self._computation_models[params.HeaderFieldInfo.in_.value]
+            + self._computation_models[params.PathFieldInfo.in_.value]
+            + self._computation_models[params.QueryFieldInfo.in_.value]
+            + self._computation_models[params.CookieFieldInfo.in_.value]
             + self._computation_models[NonParameterResolver.in_]
         )
 
     def compute_route_parameter_list(
-        self, body_field_class: t.Type[FieldInfo] = params.Body
+        self, body_field_class: t.Type[FieldInfo] = params.BodyFieldInfo
     ) -> None:
         for param_name, param in self.endpoint_signature.parameters.items():
             if (
                 param.kind == param.VAR_KEYWORD
                 or param.kind == param.VAR_POSITIONAL
                 or (
                     param.name == "self" and param.annotation == inspect.Parameter.empty
@@ -204,45 +202,45 @@
                 param_name=param.name,
                 param_default=param.default,
                 param_annotation=param.annotation,
             ):
                 continue
 
             if param_name in self.path_param_names:
-                if isinstance(param.default, params.Path):
+                if isinstance(param.default, params.PathFieldInfo):
                     ignore_default = False
                 else:
                     ignore_default = True
                 param_field = get_parameter_field(
                     param_default=param.default,
                     param_annotation=param.annotation,
                     param_name=param_name,
-                    default_field_info=params.Path,
+                    default_field_info=params.PathFieldInfo,
                     ignore_default=ignore_default,
                 )
                 assert is_scalar_field(
                     field=param_field
                 ), "Path params must be of one of the supported types"
                 self._add_to_model(field=param_field)
             else:
                 default_field_info = t.cast(
-                    t.Type[params.Param],
+                    t.Type[params.ParamFieldInfo],
                     param.default
                     if isinstance(param.default, FieldInfo)
-                    else params.Query,
+                    else params.QueryFieldInfo,
                 )
                 param_field = get_parameter_field(
                     param_default=param.default,
                     param_annotation=param.annotation,
                     default_field_info=default_field_info,
                     param_name=param_name,
                     body_field_class=body_field_class,
                 )
                 if not isinstance(
-                    param_field.field_info, (params.Body, params.File)
+                    param_field.field_info, (params.BodyFieldInfo, params.FileFieldInfo)
                 ) and not is_scalar_field(field=param_field):
                     if not is_scalar_sequence_field(param_field):
                         if not lenient_issubclass(param_field.outer_type_, BaseModel):
                             raise ImproperConfiguration(
                                 f"{param_field.outer_type_} type can't be processed as a field"
                             )
 
@@ -295,15 +293,15 @@
         annotation = param.annotation
         if isinstance(annotation, str):
             annotation = ForwardRef(annotation)
             annotation = evaluate_forwardref(annotation, globalns, globalns)
         return annotation
 
     def _add_to_model(self, *, field: ModelField, key: str = None) -> None:
-        field_info = t.cast(params.Param, field.field_info)
+        field_info = t.cast(params.ParamFieldInfo, field.field_info)
         self._computation_models[str(key or field_info.in_.value)].append(
             field_info.create_resolver(model_field=field)
         )
 
     async def resolve_dependencies(
         self, *, ctx: IExecutionContext
     ) -> t.Tuple[t.Dict[str, t.Any], t.List[ErrorWrapper]]:
@@ -339,16 +337,18 @@
                 param_default=param.default,
                 param_annotation=param.annotation,
                 key=key,
             ):
                 continue
 
             default_field_info = t.cast(
-                t.Type[params.Param],
-                param.default if isinstance(param.default, FieldInfo) else params.Query,
+                t.Type[params.ParamFieldInfo],
+                param.default
+                if isinstance(param.default, FieldInfo)
+                else params.QueryFieldInfo,
             )
             param_field = get_parameter_field(
                 param_default=param.default,
                 param_annotation=param.annotation,
                 default_field_info=default_field_info,
                 param_name=param.name,
             )
```

### Comparing `ellar-0.3.6/ellar/core/params/args/extra_args.py` & `ellar-0.3.8/ellar/common/params/args/extra_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 import typing as t
 
-from ellar.types import T
+from ellar.common.types import T
 
 
 class ExtraEndpointArg(t.Generic[T]):
     """
     Add more route function parameters programmatically.
     For example:
     lets add `limit` and `offset` to a route function.
```

### Comparing `ellar-0.3.6/ellar/core/params/args/factory.py` & `ellar-0.3.8/ellar/common/params/args/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import inspect
 import typing as t
 
 from pydantic.fields import FieldInfo, ModelField, Required
 from pydantic.schema import get_annotation_from_field_info
 
-from ellar.helper.modelfield import create_model_field
+from ellar.common.helper.modelfield import create_model_field
 
 from .. import params
 from ..helpers import is_scalar_field
 
 
 def get_parameter_field(
     *,
     param_default: t.Any,
     param_annotation: t.Type,
     param_name: str,
-    default_field_info: t.Type[params.Param] = params.Param,
+    default_field_info: t.Type[params.ParamFieldInfo] = params.ParamFieldInfo,
     ignore_default: bool = False,
-    body_field_class: t.Type[FieldInfo] = params.Body,
+    body_field_class: t.Type[FieldInfo] = params.BodyFieldInfo,
 ) -> ModelField:
 
     default_value = Required
     had_schema = False
     if param_default is not inspect.Parameter.empty and ignore_default is False:
         default_value = param_default
 
     if isinstance(default_value, FieldInfo):
         had_schema = True
         field_info = default_value
         default_value = field_info.default
         if (
-            isinstance(field_info, params.Param)
+            isinstance(field_info, params.ParamFieldInfo)
             and getattr(field_info, "in_", None) is None
         ):
             field_info.in_ = default_field_info.in_
     else:
         field_info = default_field_info(default_value)
 
     required = default_value == Required
```

### Comparing `ellar-0.3.6/ellar/core/params/args/request_model.py` & `ellar-0.3.8/ellar/common/params/args/request_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as t
 
 from pydantic import BaseModel, create_model
 from starlette.convertors import Convertor
 
-from ellar.constants import MULTI_RESOLVER_KEY
-from ellar.core.context import IExecutionContext
-from ellar.helper.modelfield import create_model_field
+from ellar.common.constants import MULTI_RESOLVER_KEY
+from ellar.common.helper.modelfield import create_model_field
+from ellar.common.interfaces import IExecutionContext
 
 from .. import params
 from ..resolvers import BaseRouteParameterResolver
 from .base import EndpointArgsModel
 from .extra_args import ExtraEndpointArg
 
 
@@ -46,15 +46,15 @@
     def build_body_field(self) -> None:
         """
         Group common body / form fields to one field
         :return:
         """
         self.body_resolver = None
 
-        body_resolvers = self._computation_models[params.Body.in_.value]
+        body_resolvers = self._computation_models[params.BodyFieldInfo.in_.value]
         if body_resolvers and len(body_resolvers) == 1:
             self.body_resolver = body_resolvers[0]
         elif body_resolvers:
             # if body_resolvers is more than one, we create a bulk_body_resolver instead
             _body_resolvers_model_fields = (
                 t.cast(BaseRouteParameterResolver, item).model_field
                 for item in body_resolvers
@@ -68,16 +68,16 @@
                 _fields_required.append(f.required)
                 _body_param_class[
                     getattr(f.field_info, "media_type", "application/json")
                 ] = (f.field_info.__class__, f.field_info)
 
             required = any(_fields_required)
             body_field_info: t.Union[
-                t.Type[params.Body], t.Type[params.Param]
-            ] = params.Body
+                t.Type[params.BodyFieldInfo], t.Type[params.ParamFieldInfo]
+            ] = params.BodyFieldInfo
             media_type = "application/json"
             if len(_body_param_class) == 1:
                 _, (klass, field_info) = _body_param_class.popitem()
                 body_field_info = klass
                 media_type = getattr(field_info, "media_type", media_type)
             elif len(_body_param_class) > 1:
                 key = list(reversed(sorted(_body_param_class.keys())))[0]
@@ -92,15 +92,17 @@
                 alias="body",
                 field_info=body_field_info(
                     media_type=media_type,
                     default=None,
                     **{MULTI_RESOLVER_KEY: body_resolvers},  # type:ignore
                 ),
             )
-            final_field.field_info = t.cast(params.Param, final_field.field_info)
+            final_field.field_info = t.cast(
+                params.ParamFieldInfo, final_field.field_info
+            )
             self.body_resolver = final_field.field_info.create_resolver(final_field)
 
     async def resolve_body(
         self, ctx: IExecutionContext, values: t.Dict, errors: t.List
     ) -> None:
         if not self.body_resolver:
             return
```

### Comparing `ellar-0.3.6/ellar/core/params/args/resolver_generators.py` & `ellar-0.3.8/ellar/common/params/args/resolver_generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import typing as t
 
 from pydantic import BaseModel
 from pydantic.fields import FieldInfo, ModelField
 
-from ellar.constants import (
+from ellar.common.constants import (
     MULTI_RESOLVER_FORM_GROUPED_KEY,
     MULTI_RESOLVER_KEY,
     sequence_types,
 )
-from ellar.core.exceptions import ImproperConfiguration
+from ellar.common.exceptions import ImproperConfiguration
 
 from .. import params
 from ..helpers import is_scalar_field, is_scalar_sequence_field
 from .factory import get_parameter_field
 
 
 class BulkArgsResolverGenerator:
@@ -56,17 +56,17 @@
 
     def get_parameter_field(
         self,
         field_name: str,
         field: ModelField,
         field_info_attrs: t.Dict,
         body_field_class: t.Type[FieldInfo],
-    ) -> t.Tuple[ModelField, params.Param]:
-        field_info_type: t.Type[params.Param] = t.cast(
-            t.Type[params.Param], type(self.param_field.field_info)
+    ) -> t.Tuple[ModelField, params.ParamFieldInfo]:
+        field_info_type: t.Type[params.ParamFieldInfo] = t.cast(
+            t.Type[params.ParamFieldInfo], type(self.param_field.field_info)
         )
         field_info = field_info_type(**field_info_attrs)
         model_field = get_parameter_field(
             param_default=field_info,
             param_annotation=field.outer_type_,
             default_field_info=field_info_type,
             param_name=field_info.alias or field_name,
@@ -138,17 +138,17 @@
 
     def get_parameter_field(
         self,
         field_name: str,
         field: ModelField,
         field_info_attrs: t.Dict,
         body_field_class: t.Type[FieldInfo],
-    ) -> t.Tuple[ModelField, params.Param]:
-        field_info = params.Path(**field_info_attrs)
+    ) -> t.Tuple[ModelField, params.ParamFieldInfo]:
+        field_info = params.PathFieldInfo(**field_info_attrs)
         model_field = get_parameter_field(
             param_default=field_info,
             param_annotation=field.outer_type_,
-            default_field_info=params.Path,
+            default_field_info=params.PathFieldInfo,
             param_name=field_info.alias or field_name,
             ignore_default=False,
         )
         return model_field, field_info
```

### Comparing `ellar-0.3.6/ellar/core/params/args/websocket_model.py` & `ellar-0.3.8/ellar/common/params/args/websocket_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing as t
 
 from pydantic.error_wrappers import ErrorWrapper
 from pydantic.fields import FieldInfo
 from starlette.convertors import Convertor
 
-from ellar.core.context import IExecutionContext
+from ellar.common.interfaces import IExecutionContext
 
 from .. import params
 from ..resolvers import BaseRouteParameterResolver, WsBodyParameterResolver
 from .base import EndpointArgsModel
 from .extra_args import ExtraEndpointArg
 
 
@@ -28,29 +28,29 @@
             endpoint=endpoint,
             param_converters=param_converters,
             extra_endpoint_args=extra_endpoint_args,
         )
         self.body_resolver = []
 
     def build_body_field(self) -> None:
-        for resolver in list(self._computation_models[params.Body.in_.value]):
+        for resolver in list(self._computation_models[params.BodyFieldInfo.in_.value]):
             if isinstance(resolver, WsBodyParameterResolver):
                 self.body_resolver.append(resolver)
                 self._computation_models[
                     resolver.model_field.field_info.in_.value
                 ].remove(resolver)
 
         if self.body_resolver and len(self.body_resolver) > 1:
             for resolver in self.body_resolver:
                 setattr(resolver.model_field.field_info, "embed", True)
 
     def compute_route_parameter_list(
-        self, body_field_class: t.Type[FieldInfo] = params.Body
+        self, body_field_class: t.Type[FieldInfo] = params.BodyFieldInfo
     ) -> None:
-        super().compute_route_parameter_list(body_field_class=params.WsBody)
+        super().compute_route_parameter_list(body_field_class=params.WsBodyFieldInfo)
 
     async def resolve_ws_body_dependencies(
         self, *, ctx: IExecutionContext, body_data: t.Any
     ) -> t.Tuple[t.Dict[str, t.Any], t.List[ErrorWrapper]]:
         values: t.Dict[str, t.Any] = {}
         errors: t.List[ErrorWrapper] = []
         for parameter_resolver in self.body_resolver or []:
```

### Comparing `ellar-0.3.6/ellar/core/params/helpers.py` & `ellar-0.3.8/ellar/common/params/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pydantic import BaseModel
 from pydantic.fields import SHAPE_SINGLETON, ModelField
 from pydantic.utils import lenient_issubclass
 
-from ellar.constants import sequence_shapes, sequence_types
+from ..constants import sequence_shapes, sequence_types
 
 
 def is_scalar_sequence_field(field: ModelField) -> bool:
     if (field.shape in sequence_shapes) and not lenient_issubclass(
         field.type_, BaseModel
     ):
         if field.sub_fields is not None:
@@ -16,22 +16,22 @@
         return True
     if lenient_issubclass(field.type_, sequence_types):
         return True
     return False
 
 
 def is_scalar_field(field: ModelField) -> bool:
-    from .params import Body, WsBody
+    from .params import BodyFieldInfo, WsBodyFieldInfo
 
     field_info = field.field_info
     if not (
         field.shape == SHAPE_SINGLETON
         and not lenient_issubclass(field.type_, BaseModel)
         and not lenient_issubclass(field.type_, sequence_types + (dict,))
-        and not isinstance(field_info, Body)
-        and not isinstance(field_info, WsBody)
+        and not isinstance(field_info, BodyFieldInfo)
+        and not isinstance(field_info, WsBodyFieldInfo)
     ):
         return False
     if field.sub_fields:
         if not all(is_scalar_field(f) for f in field.sub_fields):
             return False
     return True
```

### Comparing `ellar-0.3.6/ellar/core/params/params.py` & `ellar-0.3.8/ellar/common/params/params.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 import re
 import sys
 import typing as t
 from enum import Enum
 
 from pydantic.fields import FieldInfo, ModelField, Undefined
 
-from ellar.constants import MULTI_RESOLVER_FORM_GROUPED_KEY, MULTI_RESOLVER_KEY
-
+from ..constants import MULTI_RESOLVER_FORM_GROUPED_KEY, MULTI_RESOLVER_KEY
 from .resolvers import (
     BaseRouteParameterResolver,
     BodyParameterResolver,
     BulkBodyParameterResolver,
     BulkFormParameterResolver,
     BulkParameterResolver,
     CookieParameterResolver,
@@ -35,15 +34,15 @@
     query = "query"
     header = "header"
     path = "path"
     cookie = "cookie"
     body = "body"
 
 
-class Param(FieldInfo):
+class ParamFieldInfo(FieldInfo):
     in_: ParamTypes = ParamTypes.query
     resolver: t.Type[BaseRouteParameterResolver] = QueryParameterResolver
     bulk_resolver: t.Type[BulkParameterResolver] = BulkParameterResolver
 
     def __init__(
         self,
         default: t.Any = ...,
@@ -90,15 +89,15 @@
             )
         return self.resolver(model_field)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.default})"
 
 
-class Path(Param):
+class PathFieldInfo(ParamFieldInfo):
     in_ = ParamTypes.path
     resolver: t.Type[BaseRouteParameterResolver] = PathParameterResolver
 
     def __init__(
         self,
         default: t.Any = ...,
         *,
@@ -132,20 +131,20 @@
             deprecated=deprecated,
             example=example,
             examples=examples,
             **extra,
         )
 
 
-class Query(Param):
+class QueryFieldInfo(ParamFieldInfo):
     in_ = ParamTypes.query
     resolver: t.Type[BaseRouteParameterResolver] = QueryParameterResolver
 
 
-class Header(Param):
+class HeaderFieldInfo(ParamFieldInfo):
     in_ = ParamTypes.header
     resolver: t.Type[BaseRouteParameterResolver] = HeaderParameterResolver
 
     def __init__(
         self,
         default: t.Any,
         *,
@@ -181,20 +180,20 @@
             deprecated=deprecated,
             example=example,
             examples=examples,
             **extra,
         )
 
 
-class Cookie(Param):
+class CookieFieldInfo(ParamFieldInfo):
     in_ = ParamTypes.cookie
     resolver: t.Type[BaseRouteParameterResolver] = CookieParameterResolver
 
 
-class Body(Param):
+class BodyFieldInfo(ParamFieldInfo):
     in_ = ParamTypes.body
     MEDIA_TYPE: str = "application/json"
     resolver: t.Type[BaseRouteParameterResolver] = BodyParameterResolver
     bulk_resolver: t.Type[BulkParameterResolver] = BulkBodyParameterResolver
 
     def __init__(
         self,
@@ -236,19 +235,19 @@
             **extra,
         )
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.default})"
 
 
-class WsBody(Body):
+class WsBodyFieldInfo(BodyFieldInfo):
     resolver: t.Type[BaseRouteParameterResolver] = WsBodyParameterResolver
 
 
-class Form(Param):
+class FormFieldInfo(ParamFieldInfo):
     in_ = ParamTypes.body
     resolver: t.Type[BaseRouteParameterResolver] = FormParameterResolver
     MEDIA_TYPE: str = "application/form-data"
     bulk_resolver: t.Type[BulkParameterResolver] = BulkFormParameterResolver
 
     def __init__(
         self,
@@ -300,10 +299,10 @@
                 model_field=model_field,
                 resolvers=multiple_resolvers,
                 is_grouped=is_grouped,
             )
         return self.resolver(model_field)
 
 
-class File(Form):
+class FileFieldInfo(FormFieldInfo):
     resolver: t.Type[BaseRouteParameterResolver] = FileParameterResolver
     MEDIA_TYPE: str = "multipart/form-data"
```

### Comparing `ellar-0.3.6/ellar/core/params/resolvers/base.py` & `ellar-0.3.8/ellar/common/params/resolvers/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from abc import ABC, ABCMeta, abstractmethod
 
 from pydantic.error_wrappers import ErrorWrapper
 from pydantic.errors import MissingError
 from pydantic.fields import ModelField
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from ..params import Param
+    from ..params import ParamFieldInfo
 
 
 class RouteParameterModelField(ModelField):
-    field_info: "Param"
+    field_info: "ParamFieldInfo"
 
 
 class IRouteParameterResolver(ABC, metaclass=ABCMeta):
     @abstractmethod
     @t.no_type_check
     async def resolve(self, *args: t.Any, **kwargs: t.Any) -> t.Tuple:
         """Resolve handle"""
@@ -26,15 +26,15 @@
             RouteParameterModelField, model_field
         )
 
     def assert_field_info(self) -> None:
         from .. import params
 
         assert isinstance(
-            self.model_field.field_info, params.Param
+            self.model_field.field_info, params.ParamFieldInfo
         ), "Params must be subclasses of Param"
 
     @classmethod
     def create_error(cls, loc: t.Any) -> ErrorWrapper:
         return ErrorWrapper(MissingError(), loc=loc)
 
     @classmethod
```

### Comparing `ellar-0.3.6/ellar/core/params/resolvers/bulk_parameter.py` & `ellar-0.3.8/ellar/common/params/resolvers/bulk_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing as t
 
 from pydantic.error_wrappers import ErrorWrapper
 from pydantic.fields import ModelField
 
-from ellar.core.context import IExecutionContext
+from ellar.common.interfaces import IExecutionContext
 
 from .base import BaseRouteParameterResolver
 from .parameter import BodyParameterResolver, FormParameterResolver
 
 
 class BulkParameterResolver(BaseRouteParameterResolver):
     def __init__(
```

### Comparing `ellar-0.3.6/ellar/core/params/resolvers/non_parameter/__init__.py` & `ellar-0.3.8/ellar/common/params/resolvers/non_parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/core/params/resolvers/non_parameter/base.py` & `ellar-0.3.8/ellar/common/params/resolvers/non_parameter/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as t
 from abc import ABC, abstractmethod
 
 from pydantic.error_wrappers import ErrorWrapper
 
-from ellar.core.context import IExecutionContext
-from ellar.logger import logger
-from ellar.types import T
+from ellar.common.interfaces import IExecutionContext
+from ellar.common.logger import logger
+from ellar.common.types import T
 
 from ..base import IRouteParameterResolver
 
 
 class NonParameterResolver(IRouteParameterResolver, ABC):
     """
     Define extra route function parameter dependencies that does not depend on user inputs
```

### Comparing `ellar-0.3.6/ellar/core/params/resolvers/non_parameter/inject.py` & `ellar-0.3.8/ellar/common/params/resolvers/non_parameter/inject.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 import typing as t
 
-from ellar.core.context import IExecutionContext
-from ellar.types import T
+from ellar.common.interfaces import IExecutionContext
+from ellar.common.types import T
 
 from .base import NonParameterResolver
 
 
 class ProviderParameterInjector(NonParameterResolver):
     """
     Defines `Provider` resolver for route parameter based on the provided `service`
```

### Comparing `ellar-0.3.6/ellar/core/params/resolvers/non_parameter/session.py` & `ellar-0.3.8/ellar/common/params/resolvers/non_parameter/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing as t
 
-from ellar.core.context import IExecutionContext
+from ellar.common.interfaces import IExecutionContext
 
 from .base import BaseConnectionParameterResolver
 
 
 class HostRequestParam(BaseConnectionParameterResolver):
     lookup_connection_field = None
```

### Comparing `ellar-0.3.6/ellar/core/params/resolvers/parameter.py` & `ellar-0.3.8/ellar/common/params/resolvers/parameter.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,18 +6,22 @@
 import anyio
 from pydantic.error_wrappers import ErrorWrapper
 from pydantic.fields import Undefined
 from pydantic.utils import lenient_issubclass
 from starlette.datastructures import FormData, Headers, QueryParams
 from starlette.exceptions import HTTPException
 
-from ellar.constants import sequence_shape_to_type, sequence_shapes, sequence_types
-from ellar.core.context import IExecutionContext
-from ellar.core.datastructures import UploadFile
-from ellar.core.exceptions import RequestValidationError
+from ellar.common.constants import (
+    sequence_shape_to_type,
+    sequence_shapes,
+    sequence_types,
+)
+from ellar.common.datastructures import UploadFile
+from ellar.common.exceptions import RequestValidationError
+from ellar.common.interfaces import IExecutionContext
 
 from .base import BaseRouteParameterResolver
 
 
 class HeaderParameterResolver(BaseRouteParameterResolver):
     @classmethod
     def get_received_parameter(
```

### Comparing `ellar-0.3.6/ellar/core/response/model/__init__.py` & `ellar-0.3.8/ellar/common/responses/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,29 @@
-from .base import (
-    BaseResponseModel,
-    ResponseModel,
-    ResponseModelField,
-    ResponseTypeDefinitionConverter,
-    RouteResponseExecution,
-)
-from .factory import create_response_model
+from .base import BaseResponseModel, ResponseModel, ResponseModelField
+from .exceptions import RouteResponseExecution
 from .file import (
     FileResponseModel,
     StreamingResponseModel,
     StreamingResponseModelInvalidContent,
 )
+from .helper import create_response_model
 from .html import HTMLResponseModel, HTMLResponseModelRuntimeError
-from .interface import IResponseModel
 from .json import EmptyAPIResponseModel, JSONResponseModel
 from .route import RouteResponseModel
+from .type_converter import ResponseTypeDefinitionConverter
 
 __all__ = [
     "ResponseModel",
     "BaseResponseModel",
-    "RouteResponseExecution",
     "ResponseModelField",
     "JSONResponseModel",
     "EmptyAPIResponseModel",
     "FileResponseModel",
     "StreamingResponseModel",
     "RouteResponseModel",
-    "ResponseTypeDefinitionConverter",
-    "IResponseModel",
     "HTMLResponseModel",
     "create_response_model",
     "HTMLResponseModelRuntimeError",
     "StreamingResponseModelInvalidContent",
+    "RouteResponseExecution",
+    "ResponseTypeDefinitionConverter",
 ]
```

### Comparing `ellar-0.3.6/ellar/core/response/model/base.py` & `ellar-0.3.8/ellar/common/responses/models/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,34 @@
 import typing as t
 from abc import ABC, abstractmethod
-from dataclasses import is_dataclass
 
 from pydantic import BaseModel
 from pydantic.fields import ModelField
+from starlette.responses import Response
 
-from ellar.constants import SERIALIZER_FILTER_KEY, primitive_types
-from ellar.core.context import IExecutionContext
-from ellar.core.converters import TypeDefinitionConverter
-from ellar.core.exceptions import RequestValidationError
-from ellar.helper.modelfield import create_model_field
+from ellar.common.constants import SERIALIZER_FILTER_KEY
+from ellar.common.exceptions import RequestValidationError
+from ellar.common.helper.modelfield import create_model_field
+from ellar.common.interfaces import IExecutionContext, IResponseModel
+from ellar.common.serializer import SerializerFilter, serialize_object
 from ellar.reflect import reflect
-from ellar.serializer import (
-    BaseSerializer,
-    DataclassSerializer,
-    Serializer,
-    SerializerBase,
-    SerializerFilter,
-    convert_dataclass_to_pydantic_model,
-    serialize_object,
-)
 
-from ..response_types import Response
-from .interface import IResponseModel
+from .type_converter import ResponseTypeDefinitionConverter
 
 
 def serialize_if_pydantic_object(obj: t.Any) -> t.Any:
     if isinstance(obj, BaseModel):
         return obj.dict(by_alias=True)
     elif isinstance(obj, list):
         return [serialize_if_pydantic_object(item) for item in obj]
     elif isinstance(obj, dict):
         return {k: serialize_if_pydantic_object(v) for k, v in obj.items()}
     return obj
 
 
-class ResponseResolver(t.NamedTuple):
-    status_code: int
-    response_model: IResponseModel
-    response_object: t.Any
-
-
 class ResponseModelField(ModelField):
     def validate_object(self, obj: t.Any) -> t.Any:
         values, error = self.validate(obj, {}, loc=(self.alias,))
         if error:
             _errors = list(error) if isinstance(error, list) else [error]
             raise RequestValidationError(errors=_errors)
         return values
@@ -165,68 +149,21 @@
             endpoint_response = http_connection.get_response()
             response_args = dict(background=endpoint_response.background)
             if endpoint_response.status_code > 0:
                 response_args["status_code"] = endpoint_response.status_code
             return response_args, dict(endpoint_response.headers)
         return response_args, {}
 
-    def __deepcopy__(self, memodict: t.Dict = {}) -> "BaseResponseModel":
-        return self.__copy__(memodict)
-
-    def __copy__(self, memodict: t.Dict = {}) -> "BaseResponseModel":
-        return self
-
 
 class ResponseModel(BaseResponseModel):
     def serialize(
         self,
         response_obj: t.Any,
         serializer_filter: t.Optional[SerializerFilter] = None,
     ) -> t.Union[t.List[t.Dict], t.Dict, t.Any]:
         return response_obj
 
 
-class RouteResponseExecution(Exception):
-    pass
-
-
-class ResponseTypeDefinitionConverter(TypeDefinitionConverter):
-    _registry: t.Dict[t.Any, t.Type[BaseSerializer]] = {}
-
-    def _get_modified_type(
-        self, outer_type_: t.Type
-    ) -> t.Union[t.Type[BaseSerializer], t.Any]:
-        if not isinstance(outer_type_, type):
-            raise Exception(f"{outer_type_} is not a type")
-
-        if issubclass(outer_type_, DataclassSerializer):
-            schema_model = outer_type_.get_pydantic_model()
-            cls = type(outer_type_.__name__, (schema_model, SerializerBase), {})
-            return t.cast(t.Type[BaseSerializer], cls)
-
-        if isinstance(outer_type_, type) and issubclass(outer_type_, (BaseSerializer,)):
-            return outer_type_
-
-        if issubclass(outer_type_, BaseModel):
-            cls = type(outer_type_.__name__, (outer_type_, Serializer), dict())
-            return t.cast(t.Type[BaseSerializer], cls)
-
-        if is_dataclass(outer_type_):
-            if hasattr(outer_type_, "__pydantic_model__"):
-                schema_model = outer_type_.__pydantic_model__
-                return self._get_modified_type(t.cast(type, schema_model))
-            return self._get_modified_type(
-                t.cast(type, convert_dataclass_to_pydantic_model(outer_type_))
-            )
-
-        if outer_type_ in primitive_types:
-            return outer_type_
-
-        attrs = {"__annotations__": getattr(outer_type_, "__annotations__", ())}
-        cls = type(outer_type_.__name__, (outer_type_, Serializer), attrs)
-
-        return t.cast(t.Type[BaseSerializer], cls)
-
-    def get_modified_type(self, outer_type_: t.Type) -> t.Type[BaseSerializer]:
-        if outer_type_ not in self._registry:
-            self._registry[outer_type_] = self._get_modified_type(outer_type_)
-        return self._registry[outer_type_]
+class ResponseResolver(t.NamedTuple):
+    status_code: int
+    response_model: IResponseModel
+    response_object: t.Any
```

### Comparing `ellar-0.3.6/ellar/core/response/model/factory.py` & `ellar-0.3.8/ellar/common/responses/models/helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import typing as t
 
 from starlette.responses import Response
 
-if t.TYPE_CHECKING:
-    from .base import ResponseModel, ResponseModelField
+from .base import ResponseModel, ResponseModelField
 
 T = t.TypeVar("T")
 
 
 def create_response_model(
     response_model: t.Union[t.Type["ResponseModel"], t.Type[T]],
     *,
```

### Comparing `ellar-0.3.6/ellar/core/response/model/file.py` & `ellar-0.3.8/ellar/common/responses/models/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing as t
 from enum import Enum
 
-from ellar.core.context import IExecutionContext
-from ellar.serializer import Serializer, SerializerFilter, serialize_object
+from ellar.common.interfaces import IExecutionContext
+from ellar.common.serializer import Serializer, SerializerFilter, serialize_object
 
 from ..response_types import FileResponse, Response, StreamingResponse
 from .base import ResponseModel, ResponseModelField
 
 
 class StreamingResponseModelInvalidContent(RuntimeError):
     pass
```

### Comparing `ellar-0.3.6/ellar/core/response/model/html.py` & `ellar-0.3.8/ellar/common/responses/models/html.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import typing as t
 
-from ellar.core.context import ExecutionContext, IExecutionContext
-from ellar.core.templating import Environment, TemplateResponse
-from ellar.core.templating.renderer import get_template_name, process_view_model
+from ellar.common.interfaces import IExecutionContext
+from ellar.common.templating import (
+    Environment,
+    TemplateResponse,
+    get_template_name,
+    process_view_model,
+)
 
 from ..response_types import Response
 from .base import ResponseModel
 
 
 class HTMLResponseModelRuntimeError(RuntimeError):
     pass
@@ -39,16 +43,15 @@
         response_args, headers = self.get_context_response(context=context)
         response_args.update(template=template, context=template_context)
         response = self._response_type(**response_args, headers=headers)
         return response
 
     def _get_template_name(self, ctx: IExecutionContext) -> str:
         template_name = self.template_name
-        exe_ctx = t.cast(ExecutionContext, ctx)
         if self.use_mvc:
-            controller_class = exe_ctx.get_class()
+            controller_class = ctx.get_class()
             if not controller_class or not hasattr(controller_class, "full_view_name"):
                 raise HTMLResponseModelRuntimeError(
                     "cannot find Controller in request context"
                 )
             template_name = controller_class.full_view_name(self.template_name)
         return get_template_name(template_name)
```

### Comparing `ellar-0.3.6/ellar/core/response/model/interface.py` & `ellar-0.3.8/ellar/common/interfaces/response_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import typing as t
 from abc import ABC, abstractmethod
 
 from pydantic.fields import ModelField
+from starlette.responses import Response
 
-from ellar.core.context import IExecutionContext
-
-from ..response_types import Response
+from .context import IExecutionContext
 
 
 class IResponseModel(ABC):
-    # TODO: abstract to a interface package
-
     @property
     def media_type(self) -> str:  # pragma: no cover
         return "text/plain"
 
     @property
     def description(self) -> str:  # pragma: no cover
         return ""
```

### Comparing `ellar-0.3.6/ellar/core/response/model/json.py` & `ellar-0.3.8/ellar/common/responses/models/json.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing as t
 
-from ellar.constants import SERIALIZER_FILTER_KEY
-from ellar.core.context import IExecutionContext
-from ellar.helper.modelfield import create_model_field
+from ellar.common.constants import SERIALIZER_FILTER_KEY
+from ellar.common.helper.modelfield import create_model_field
+from ellar.common.interfaces import IExecutionContext
+from ellar.common.serializer import SerializerFilter, serialize_object
 from ellar.reflect import reflect
-from ellar.serializer import SerializerFilter, serialize_object
 
 from ..response_types import JSONResponse, Response
 from .base import ResponseModel, ResponseModelField
 
 DictModelField: ResponseModelField = t.cast(
     ResponseModelField,
     create_model_field(
```

### Comparing `ellar-0.3.6/ellar/core/response/model/route.py` & `ellar-0.3.8/ellar/common/responses/models/route.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import typing as t
 
 from pydantic import BaseModel
 
-from ellar.constants import SCOPE_RESPONSE_STARTED
-from ellar.core.context import IExecutionContext
+from ellar.common.constants import SCOPE_RESPONSE_STARTED
+from ellar.common.interfaces import IExecutionContext, IResponseModel
 
 from ..response_types import Response
-from .base import ResponseModel, ResponseResolver, RouteResponseExecution
-from .factory import create_response_model
-from .interface import IResponseModel
+from .base import ResponseModel, ResponseResolver
+from .exceptions import RouteResponseExecution
+from .helper import create_response_model
 from .json import JSONResponseModel
 
 
 class RouteResponseModel:
     __slots__ = ("models",)
 
     def __init__(
```

### Comparing `ellar-0.3.6/ellar/core/response/response_types.py` & `ellar-0.3.8/ellar/common/responses/response_types.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/core/routing/base.py` & `ellar-0.3.8/ellar/common/routing/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import typing as t
 from abc import ABC, abstractmethod
 
 from starlette.routing import Match
 
-from ellar.constants import (
+from ellar.common.constants import (
     CONTROLLER_CLASS_KEY,
     GUARDS_KEY,
     SCOPE_API_VERSIONING_RESOLVER,
     SCOPE_SERVICE_PROVIDER,
     VERSIONING_KEY,
 )
-from ellar.core.context import IExecutionContext, IExecutionContextFactory
-from ellar.di import EllarInjector
+from ellar.common.interfaces import IExecutionContext, IExecutionContextFactory
+from ellar.common.models import GuardCanActivate
+from ellar.common.types import TReceive, TScope, TSend
 from ellar.reflect import reflect
-from ellar.services.reflector import Reflector
-from ellar.types import TReceive, TScope, TSend
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.core.guard import GuardCanActivate
     from ellar.core.versioning.resolver import BaseAPIVersioningResolver
+    from ellar.di import EllarInjector
 
 __all__ = [
     "RouteOperationBase",
     "WebsocketRouteOperationBase",
 ]
 
 
@@ -39,16 +38,16 @@
 
     @abstractmethod
     def _load_model(self) -> None:
         """compute route models"""
 
     @t.no_type_check
     async def run_route_guards(self, context: IExecutionContext) -> None:
-        reflector = context.get_service_provider().get(Reflector)
         app = context.get_app()
+        reflector = app.reflector
 
         targets = [self.endpoint, self.get_control_type()]
 
         _guards: t.Optional[
             t.List[t.Union[t.Type["GuardCanActivate"], "GuardCanActivate"]]
         ] = reflector.get_all_and_override(GUARDS_KEY, *targets)
 
@@ -61,15 +60,15 @@
                     guard = context.get_service_provider().get(guard)
 
                 result = await guard.can_activate(context)
                 if not result:
                     guard.raise_exception()
 
     async def app(self, scope: TScope, receive: TReceive, send: TSend) -> None:
-        service_provider = t.cast(EllarInjector, scope[SCOPE_SERVICE_PROVIDER])
+        service_provider: "EllarInjector" = scope[SCOPE_SERVICE_PROVIDER]
 
         execution_context_factory = service_provider.get(IExecutionContextFactory)
         context = execution_context_factory.create_context(
             operation=self, scope=scope, receive=receive, send=send
         )
 
         await self.run_route_guards(context=context)
```

### Comparing `ellar-0.3.6/ellar/core/routing/controller/base.py` & `ellar-0.3.8/ellar/common/routing/controller/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing as t
 
-from ellar.constants import CONTROLLER_CLASS_KEY
-from ellar.core.context import IExecutionContext
-from ellar.core.controller import ControllerBase
+from ellar.common.constants import CONTROLLER_CLASS_KEY
+from ellar.common.interfaces import IExecutionContext
+from ellar.common.models import ControllerBase
 from ellar.reflect import reflect
 
 
 class ControllerRouteOperationBase:
     endpoint: t.Callable
 
     def _get_controller_instance(self, ctx: IExecutionContext) -> ControllerBase:
@@ -17,15 +17,15 @@
             controller_type and not issubclass(controller_type, ControllerBase)
         ):
             raise RuntimeError("Controller Type was not found")
 
         service_provider = ctx.get_service_provider()
 
         controller_instance: ControllerBase = service_provider.get(controller_type)
-        controller_instance.context = ctx  # type:ignore
+        controller_instance.context = ctx
         return controller_instance
 
     @t.no_type_check
     def __call__(
         self, context: IExecutionContext, *args: t.Any, **kwargs: t.Any
     ) -> t.Any:
         controller_instance = self._get_controller_instance(ctx=context)
```

### Comparing `ellar-0.3.6/ellar/core/routing/controller/route.py` & `ellar-0.3.8/ellar/common/routing/controller/route.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as t
 
 from starlette.concurrency import run_in_threadpool
 from starlette.responses import Response
 
-from ellar.core.context import IExecutionContext
-from ellar.core.exceptions import RequestValidationError
-from ellar.core.routing.route import RouteOperation
+from ellar.common.exceptions import RequestValidationError
+from ellar.common.interfaces import IExecutionContext
+from ellar.common.routing.route import RouteOperation
 
 from .base import ControllerRouteOperationBase
 
 
 class ControllerRouteOperation(ControllerRouteOperationBase, RouteOperation):
     methods: t.Set[str]
```

### Comparing `ellar-0.3.6/ellar/core/routing/controller/websocket/route.py` & `ellar-0.3.8/ellar/common/routing/controller/websocket/route.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing as t
 
 from starlette.status import WS_1008_POLICY_VIOLATION
 from starlette.websockets import WebSocketState
 
-from ellar.core.context import IExecutionContext
-from ellar.core.exceptions import WebSocketRequestValidationError
+from ellar.common.exceptions import WebSocketRequestValidationError
+from ellar.common.interfaces import IExecutionContext
 
 from ...websocket import WebsocketRouteOperation
 from ..base import ControllerRouteOperationBase
 from .handler import ControllerWebSocketExtraHandler
 
 
 class ControllerWebsocketRouteOperation(
```

### Comparing `ellar-0.3.6/ellar/core/routing/operation_definitions.py` & `ellar-0.3.8/ellar/common/routing/operation_definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import functools
 import typing as t
 from functools import partial
 from types import FunctionType
 
-from ellar.constants import (
+from ellar.common.constants import (
     CONTROLLER_OPERATION_HANDLER_KEY,
     DELETE,
     GET,
     HEAD,
     OPERATION_ENDPOINT_KEY,
     OPTIONS,
     PATCH,
     POST,
     PUT,
     TRACE,
 )
-from ellar.core.schema import RouteParameters, WsRouteParameters
-from ellar.helper import class_base_function_regex
+from ellar.common.helper import class_base_function_regex
+from ellar.common.types import TCallable
 from ellar.reflect import reflect
-from ellar.types import TCallable
 
 from .controller.route import ControllerRouteOperation
 from .controller.websocket.route import ControllerWebsocketRouteOperation
 from .route import RouteOperation
+from .schema import RouteParameters, WsRouteParameters
 from .websocket import WebsocketRouteOperation
 
 TOperation = t.Union[RouteOperation, ControllerRouteOperation]
 TWebsocketOperation = t.Union[
     WebsocketRouteOperation, ControllerWebsocketRouteOperation
 ]
```

### Comparing `ellar-0.3.6/ellar/core/routing/route.py` & `ellar-0.3.8/ellar/common/routing/route.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 import inspect
 import typing as t
 
 from starlette.concurrency import run_in_threadpool
 from starlette.responses import Response
 from starlette.routing import Route as StarletteRoute, compile_path
 
-from ellar.constants import (
+from ellar.common.constants import (
     CONTROLLER_OPERATION_HANDLER_KEY,
     EXTRA_ROUTE_ARGS_KEY,
     NOT_SET,
     RESPONSE_OVERRIDE_KEY,
 )
-from ellar.core.context import IExecutionContext
-from ellar.core.exceptions import ImproperConfiguration, RequestValidationError
-from ellar.core.params import RequestEndpointArgsModel
-from ellar.core.response.model import RouteResponseModel
-from ellar.helper import generate_operation_unique_id, get_name
+from ellar.common.exceptions import ImproperConfiguration, RequestValidationError
+from ellar.common.helper import generate_operation_unique_id, get_name
+from ellar.common.interfaces import IExecutionContext
+from ellar.common.params import ExtraEndpointArg, RequestEndpointArgsModel
+from ellar.common.responses.models import RouteResponseModel
 from ellar.reflect import reflect
 
 from .base import RouteOperationBase
 
-if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.core.params import ExtraEndpointArg
-
 
 class RouteOperation(RouteOperationBase, StarletteRoute):
     methods: t.Set[str]
     request_endpoint_args_model: t.Type[
         RequestEndpointArgsModel
     ] = RequestEndpointArgsModel
```

### Comparing `ellar-0.3.6/ellar/core/routing/router/app.py` & `ellar-0.3.8/ellar/core/routing/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import typing as t
 from functools import wraps
 from types import FunctionType
 
 from starlette.routing import BaseRoute, Router as StarletteRouter
 
-from ellar.constants import (
+from ellar.common.constants import (
     CONTROLLER_OPERATION_HANDLER_KEY,
     SCOPE_API_VERSIONING_RESOLVER,
 )
+from ellar.common.routing import RouteCollection
+from ellar.common.types import ASGIApp, TReceive, TScope, TSend
 from ellar.reflect import reflect
-from ellar.types import ASGIApp, TReceive, TScope, TSend
-
-from .route_collections import RouteCollection
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.core.versioning.resolver import BaseAPIVersioningResolver
 
 __all__ = ["ApplicationRouter"]
```

### Comparing `ellar-0.3.6/ellar/core/routing/router/module.py` & `ellar-0.3.8/ellar/common/routing/mount.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,32 @@
 import typing as t
 import uuid
 
 from starlette.routing import BaseRoute, Match, Mount as StarletteMount, Route, Router
 from starlette.types import ASGIApp
 
-from ellar.compatible import AttributeDict
-from ellar.constants import (
+from ellar.common.compatible import AttributeDict
+from ellar.common.constants import (
     CONTROLLER_CLASS_KEY,
-    CONTROLLER_METADATA,
-    CONTROLLER_OPERATION_HANDLER_KEY,
     GUARDS_KEY,
     NOT_SET,
     OPERATION_ENDPOINT_KEY,
     VERSIONING_KEY,
 )
-from ellar.core.controller import ControllerBase
-from ellar.core.routing.route import RouteOperation
-from ellar.core.schema import RouteParameters, WsRouteParameters
-from ellar.helper import get_unique_control_type
+from ellar.common.helper import get_unique_control_type
+from ellar.common.models import GuardCanActivate
+from ellar.common.types import TReceive, TScope, TSend
 from ellar.reflect import reflect
-from ellar.types import TReceive, TScope, TSend
 
-from ..operation_definitions import (
-    OperationDefinitions,
-    TOperation,
-    TWebsocketOperation,
-)
+from .operation_definitions import OperationDefinitions, TOperation, TWebsocketOperation
+from .route import RouteOperation
 from .route_collections import RouteCollection
+from .schema import RouteParameters, WsRouteParameters
 
-if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.core.guard import GuardCanActivate
-
-__all__ = ["ModuleMount", "ModuleRouter", "controller_router_factory"]
-
-
-def controller_router_factory(
-    controller: t.Union[t.Type[ControllerBase], t.Any]
-) -> "ModuleMount":
-    openapi = reflect.get_metadata(CONTROLLER_METADATA.OPENAPI, controller) or dict()
-    routes = reflect.get_metadata(CONTROLLER_OPERATION_HANDLER_KEY, controller) or []
-    app = Router()
-    app.routes = RouteCollection(routes)  # type:ignore
-
-    include_in_schema = reflect.get_metadata_or_raise_exception(
-        CONTROLLER_METADATA.INCLUDE_IN_SCHEMA, controller
-    )
-    router = ModuleMount(
-        app=app,
-        path=reflect.get_metadata_or_raise_exception(
-            CONTROLLER_METADATA.PATH, controller
-        ),
-        name=reflect.get_metadata_or_raise_exception(
-            CONTROLLER_METADATA.NAME, controller
-        ),
-        include_in_schema=include_in_schema if include_in_schema is not None else True,
-        control_type=controller,
-        **openapi,
-    )
-    return router
+__all__ = ["ModuleMount", "ModuleRouter"]
 
 
 class ModuleMount(StarletteMount):
     def __init__(
         self,
         path: str,
         control_type: t.Type,
```

### Comparing `ellar-0.3.6/ellar/core/routing/router/route_collections.py` & `ellar-0.3.8/ellar/common/routing/route_collections.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import typing as t
 import uuid
 from collections import OrderedDict
 
 from starlette.routing import BaseRoute, Host, Mount
 
-from ellar.constants import CONTROLLER_CLASS_KEY
-from ellar.core.routing import RouteOperation, RouteOperationBase
-from ellar.core.routing.websocket.route import WebsocketRouteOperation
-from ellar.helper import (
+from ellar.common.constants import CONTROLLER_CLASS_KEY
+from ellar.common.helper import (
     generate_controller_operation_unique_id,
     get_unique_control_type,
 )
-from ellar.logger import logger
+from ellar.common.logger import logger
 from ellar.reflect import reflect
 
+from .base import RouteOperationBase
+from .route import RouteOperation
+from .websocket.route import WebsocketRouteOperation
+
 
 class RouteCollection(t.Sequence[BaseRoute]):
     __slots__ = ("_routes", "_served_routes")
 
     def __init__(self, routes: t.Optional[t.Sequence[BaseRoute]] = None) -> None:
         self._routes: t.Dict[int, BaseRoute] = OrderedDict()
         self._served_routes: t.List[BaseRoute] = []
```

### Comparing `ellar-0.3.6/ellar/core/routing/websocket/handler.py` & `ellar-0.3.8/ellar/common/routing/websocket/handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import json
 import typing as t
 
 from starlette import status
+from starlette.exceptions import WebSocketException
 from starlette.status import WS_1008_POLICY_VIOLATION
 from starlette.types import Message
 
-from ellar.core.exceptions import WebSocketException, WebSocketRequestValidationError
-from ellar.core.params import WebsocketEndpointArgsModel
+from ellar.common.exceptions import WebSocketRequestValidationError
+from ellar.common.interfaces import IExecutionContext
+from ellar.common.params import WebsocketEndpointArgsModel
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.core.connection import WebSocket
-    from ellar.core.context import IExecutionContext
 
 
 class WebSocketExtraHandler:
     def __init__(
         self,
         on_receive: t.Callable,
         *,
```

### Comparing `ellar-0.3.6/ellar/core/routing/websocket/route.py` & `ellar-0.3.8/ellar/common/routing/websocket/route.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import typing as t
 
 from starlette.routing import WebSocketRoute as StarletteWebSocketRoute, compile_path
 from starlette.status import WS_1008_POLICY_VIOLATION
 from starlette.websockets import WebSocketState
 
-from ellar.constants import (
+from ellar.common.constants import (
     CONTROLLER_OPERATION_HANDLER_KEY,
     EXTRA_ROUTE_ARGS_KEY,
     NOT_SET,
 )
-from ellar.core.context import IExecutionContext
-from ellar.core.exceptions import ImproperConfiguration, WebSocketRequestValidationError
-from ellar.core.params import WebsocketEndpointArgsModel
-from ellar.helper import get_name
+from ellar.common.exceptions import (
+    ImproperConfiguration,
+    WebSocketRequestValidationError,
+)
+from ellar.common.helper import get_name
+from ellar.common.interfaces import IExecutionContext
+from ellar.common.params import ExtraEndpointArg, WebsocketEndpointArgsModel
 from ellar.reflect import reflect
 
 from ..base import WebsocketRouteOperationBase
 from .handler import WebSocketExtraHandler
 
-if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.core.params import ExtraEndpointArg
-
 
 class WebsocketRouteOperation(WebsocketRouteOperationBase, StarletteWebSocketRoute):
     websocket_endpoint_args_model: t.Type[
         WebsocketEndpointArgsModel
     ] = WebsocketEndpointArgsModel
 
     __slots__ = (
```

### Comparing `ellar-0.3.6/ellar/core/schema.py` & `ellar-0.3.8/ellar/common/routing/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 import typing as t
 
 from pydantic import BaseModel, Field, root_validator, validator
 
-from ellar.constants import ROUTE_METHODS
-from ellar.core.response.model import (
-    EmptyAPIResponseModel,
-    IResponseModel,
-    create_response_model,
-)
-from ellar.serializer import BaseSerializer, Serializer
+from ellar.common.constants import ROUTE_METHODS
+from ellar.common.interfaces import IResponseModel
+from ellar.common.responses.models import EmptyAPIResponseModel, create_response_model
+from ellar.common.serializer import BaseSerializer
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.core.routing.websocket import WebSocketExtraHandler
+    from ellar.common.routing.websocket import WebSocketExtraHandler
 
 
 class TResponseModel:
     @classmethod
     def __get_validators__(
         cls: t.Type["TResponseModel"],
-    ) -> t.Iterable[t.Callable[..., t.Any]]:
-        yield cls.validate
+    ) -> t.Any:
+        yield cls.validate  # type:ignore[misc]
 
     @classmethod
-    def validate(cls: t.Type["IResponseModel"], v: t.Any) -> t.Any:
+    def validate(cls: t.Type["IResponseModel"], v: t.Any) -> t.Any:  # type:ignore[misc]
         if not isinstance(v, IResponseModel):
             raise ValueError(f"Expected ResponseModel, received: {type(v)}")
         return v
 
 
 class RouteParameters(BaseModel):
     class Config:
@@ -45,30 +42,30 @@
             t.Type[BaseModel],
             t.Type[BaseSerializer],
             t.Any,
         ]
     ]
 
     @validator("methods")
-    def validate_methods(cls, value: t.Any):
-        methods = list(map(lambda m: m.upper(), value))
+    def validate_methods(cls, value: t.Any) -> t.List[str]:
+        methods = list(map(lambda m: m.upper(), value))  # type:ignore[no-any-return]
         not_valid_methods = list(set(methods) - set(ROUTE_METHODS))
 
         if not_valid_methods:
             raise ValueError(f"Method {','.join(not_valid_methods)} not allowed")
         return methods
 
     @validator("endpoint")
-    def validate_endpoint(cls, value: t.Any):
+    def validate_endpoint(cls, value: t.Any) -> t.Any:
         if not callable(value):
             raise ValueError("An endpoint must be a callable")
         return value
 
     @root_validator
-    def validate_root(cls, values: t.Any):
+    def validate_root(cls, values: t.Any) -> t.Any:
         if "response" not in values:
             raise ValueError(
                 "Expected "
                 "IResponseModel | Dict[int, Any | Type[BaseModel] | "
                 "Type[BaseSerializer] | IResponseModel]  | Type[BaseModel] | Type[BaseSerializer]"
             )
 
@@ -85,31 +82,17 @@
     name: t.Optional[str] = None
     endpoint: t.Callable
     encoding: t.Optional[str] = Field("json")
     use_extra_handler: bool = Field(False)
     extra_handler_type: t.Optional[t.Type["WebSocketExtraHandler"]] = None
 
     @validator("endpoint")
-    def validate_endpoint(cls, value: t.Any):
+    def validate_endpoint(cls, value: t.Any) -> t.Any:
         return value
 
     @validator("encoding")
-    def validate_encoding(cls, value: t.Any):
+    def validate_encoding(cls, value: t.Any) -> t.Any:
         if value not in ["json", "text", "bytes", None]:
             raise ValueError(
                 f"Encoding type not supported. Once [json | text | bytes]. Received: {value}"
             )
         return value
-
-
-class ValidationError(BaseModel):
-    loc: t.List[str] = Field(..., title="Location")
-    msg: str = Field(..., title="Message")
-    type: str = Field(..., title="Error Type")
-
-
-class HTTPValidationError(BaseModel):
-    detail: t.List[ValidationError] = Field(..., title="Details")
-
-
-class Schema(Serializer):
-    pass
```

### Comparing `ellar-0.3.6/ellar/core/staticfiles.py` & `ellar-0.3.8/ellar/core/staticfiles.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/core/templating/loader.py` & `ellar-0.3.8/ellar/common/templating/loader.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/core/templating/renderer.py` & `ellar-0.3.8/ellar/common/templating/renderer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import typing as t
 from functools import lru_cache
 
 import jinja2
 from starlette.background import BackgroundTask
 from starlette.templating import _TemplateResponse as TemplateResponse
 
-from ellar.core.connection import Request
+from ellar.common.templating import Environment
 
-from .environment import Environment
+if t.TYPE_CHECKING:  # pragma: no cover
+    from ellar.core.connection import Request
 
 
 @lru_cache(1200)
 def get_template_name(template_name: str) -> str:
     if not template_name.endswith(".html"):
         return template_name + ".html"
     return template_name
@@ -20,25 +21,25 @@
 def process_view_model(view_response: t.Any) -> t.Dict:
     if isinstance(view_response, dict):
         return view_response
     return dict(model=view_response)
 
 
 def _get_jinja_and_template_context(
-    template_name: str, request: Request, **context: t.Any
+    template_name: str, request: "Request", **context: t.Any
 ) -> t.Tuple["jinja2.Template", t.Dict]:
     jinja_environment = request.service_provider.get(Environment)
     jinja_template = jinja_environment.get_template(get_template_name(template_name))
     template_context = dict(context)
     template_context.update(request=request)
     return jinja_template, template_context
 
 
 def render_template_string(
-    template_name: str, request: Request, **template_kwargs: t.Any
+    template_name: str, request: "Request", **template_kwargs: t.Any
 ) -> str:
     """Renders a template to string.
     :param request: Request instance
     :param template_name: the name of the template to be rendered
     :param template_kwargs: variables that should be available in the context of the template.
     """
     jinja_template, template_context = _get_jinja_and_template_context(
@@ -46,15 +47,15 @@
     )
 
     return jinja_template.render(template_context)
 
 
 def render_template(
     template_name: str,
-    request: Request,
+    request: "Request",
     background: BackgroundTask = None,
     **template_kwargs: t.Any
 ) -> TemplateResponse:
     """Renders a template from the template folder with the given context.
     :param request: Request instance
     :param template_name: the name of the template to be rendered
     :param template_kwargs: variables that should be available in the context of the template.
```

### Comparing `ellar-0.3.6/ellar/core/versioning/__init__.py` & `ellar-0.3.8/ellar/core/versioning/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/core/versioning/base.py` & `ellar-0.3.8/ellar/core/versioning/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing as t
 from abc import ABC
 
-from ellar.types import TScope
+from ellar.common.types import TScope
 
 from .resolver import (
     BaseAPIVersioningResolver,
     DefaultAPIVersionResolver,
     HeaderVersionResolver,
     HostNameAPIVersionResolver,
     QueryParameterAPIVersionResolver,
```

### Comparing `ellar-0.3.6/ellar/core/versioning/resolver.py` & `ellar-0.3.8/ellar/core/versioning/resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import email
 import re
 import typing as t
 from abc import abstractmethod
 
 from starlette.routing import compile_path
 
-from ellar.constants import NOT_SET
+from ellar.common.constants import NOT_SET
+from ellar.common.exceptions import NotAcceptable, NotFound
+from ellar.common.types import TScope
 from ellar.core.connection import HTTPConnection
-from ellar.core.exceptions import NotAcceptable, NotFound
-from ellar.types import TScope
 
 
 class BaseAPIVersioningResolver:
     def __init__(
         self, *, scope: TScope, version_parameter: str, default_version: t.Optional[str]
     ) -> None:
         self.version_parameter = version_parameter
```

### Comparing `ellar-0.3.6/ellar/di/injector/container.py` & `ellar-0.3.8/ellar/di/injector/container.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,33 +7,32 @@
     Binding,
     Module as InjectorModule,
     Scope as InjectorScope,
     UnsatisfiedRequirement,
     _is_specialization,
 )
 
-from ellar.constants import NOT_SET
-from ellar.helper import get_name
-from ellar.types import T
-
 from ..providers import Provider
 from ..scopes import (
     DIScope,
     RequestScope,
     ScopeDecorator,
     SingletonScope,
     TransientScope,
 )
 from ..service_config import get_scope, is_decorated_with_injectable
+from ..types import T
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.core.modules import ModuleBase
 
     from .ellar_injector import EllarInjector
 
+NOT_SET = object()
+
 
 class Container(InjectorBinder):
     __slots__ = (
         "injector",
         "_auto_bind",
         "_bindings",
         "parent",
@@ -90,16 +89,16 @@
         base_type: t.Type,
         concrete_type: t.Union[t.Type[T], t.Type, T] = None,
         scope: t.Union[t.Type[DIScope], ScopeDecorator] = None,
     ) -> None:
         try:
             if concrete_type and isinstance(concrete_type, type):
                 assert issubclass(concrete_type, base_type), (
-                    f"Cannot register {get_name(base_type)} for abstract class "
-                    f"{get_name(concrete_type)}"
+                    f"Cannot register {base_type.__name__} for abstract class "
+                    f"{concrete_type.__name__}"
                 )
         except TypeError:  # pragma: no cover
             # ignore generic types issues
             pass
 
         provider = self.provider_for(base_type, concrete_type)
 
@@ -236,10 +235,16 @@
 
         instance = t.cast(t.Union[t.Type["ModuleBase"], "ModuleBase"], module)
 
         if isinstance(instance, type) and issubclass(
             t.cast(type, instance), InjectorModule
         ):
             instance = t.cast(type, instance)(**init_kwargs)
+        elif isinstance(instance, type) and not isinstance(instance, InjectorModule):
+            return self.injector.get(t.cast(type, instance))
+        elif not isinstance(instance, type) and not isinstance(
+            type(instance), InjectorModule
+        ):
+            return instance
 
         instance(self)
         return instance
```

### Comparing `ellar-0.3.6/ellar/di/injector/ellar_injector.py` & `ellar-0.3.8/ellar/di/injector/ellar_injector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
+import logging
 import typing as t
 from collections import OrderedDict, defaultdict
 
 from injector import Injector
 
-from ellar.asgi_args import RequestScopeContext
-from ellar.compatible import asynccontextmanager
-from ellar.constants import MODULE_REF_TYPES, SCOPED_CONTEXT_VAR
-from ellar.logger import logger as log
-from ellar.types import T
+from ellar.reflect import asynccontextmanager
 
+from ..asgi_args import RequestScopeContext
+from ..constants import MODULE_REF_TYPES, SCOPED_CONTEXT_VAR
 from ..providers import InstanceProvider, Provider
 from ..scopes import DIScope, ScopeDecorator
+from ..types import T
 from .container import Container
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.core.modules import (
         ModuleBase,
         ModuleRefBase,
         ModuleSetup,
         ModuleTemplateRef,
     )
 
+log = logging.getLogger("ellar.di")
+
 
 class EllarInjector(Injector):
     __slots__ = (
         "_stack",
         "parent",
         "container",
         "_modules",
```

### Comparing `ellar-0.3.6/ellar/di/providers.py` & `ellar-0.3.8/ellar/di/providers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/di/scopes.py` & `ellar-0.3.8/ellar/di/scopes.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 from injector import (
     NoScope as InjectorNoScope,
     Scope as InjectorScope,
     ScopeDecorator as ScopeDecorator,
     SingletonScope as InjectorSingletonScope,
 )
 
-from ellar.types import T
-
 from .providers import InstanceProvider, Provider
+from .types import T
 
 
 class DIScope(InjectorScope):
     @abstractmethod
     def get(
         self,
         key: t.Type[T],
```

### Comparing `ellar-0.3.6/ellar/di/service_config.py` & `ellar-0.3.8/ellar/di/service_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 
 from injector import (
     ConstructorOrClassT,
     inject,
     is_decorated_with_inject as injector_is_decorated_with_inject,
 )
 
-from ellar.constants import INJECTABLE_ATTRIBUTE
-from ellar.shortcuts import fail_silently
-from ellar.types import T
-
+from .constants import INJECTABLE_ATTRIBUTE
 from .exceptions import DIImproperConfiguration
 from .scopes import DIScope, ScopeDecorator, SingletonScope
+from .types import T
+from .utils import fail_silently
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from .injector import Container
 
 __all__ = (
     "ProviderConfig",
     "injectable",
```

### Comparing `ellar-0.3.6/ellar/events.py` & `ellar-0.3.8/ellar/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import typing as t
 from abc import abstractmethod
 
-from ellar.types import T
+from ellar.common.types import T
 
 
 class EventHandler:
     __slots__ = ("is_coroutine", "handler")
 
     def __init__(self, func: t.Callable) -> None:
         self.is_coroutine = asyncio.iscoroutinefunction(func)
```

### Comparing `ellar-0.3.6/ellar/helper/__init__.py` & `ellar-0.3.8/ellar/common/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/helper/enums.py` & `ellar-0.3.8/ellar/common/helper/enums.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/helper/importer.py` & `ellar-0.3.8/ellar/common/helper/importer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/helper/modelfield.py` & `ellar-0.3.8/ellar/common/helper/modelfield.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/helper/module_loading.py` & `ellar-0.3.8/ellar/common/helper/module_loading.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/openapi/__init__.py` & `ellar-0.3.8/ellar/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/openapi/builder.py` & `ellar-0.3.8/ellar/openapi/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,29 @@
     TypeModelOrEnum,
     get_flat_models_from_fields,
     get_model_name_map,
     model_process_schema,
 )
 from starlette.routing import BaseRoute, Mount
 
-from ellar.compatible import cached_property
-from ellar.constants import GUARDS_KEY, OPENAPI_KEY
+from ellar.common.compatible import cached_property
+from ellar.common.constants import GUARDS_KEY, OPENAPI_KEY, REF_PREFIX
+from ellar.common.helper.modelfield import create_model_field
+from ellar.common.routing import ModuleMount, RouteOperation
+from ellar.common.routing.controller import ControllerRouteOperation
 from ellar.core.main import App
-from ellar.core.routing import ModuleMount, RouteOperation
-from ellar.core.routing.controller.route import ControllerRouteOperation
-from ellar.core.schema import HTTPValidationError, ValidationError
-from ellar.helper.modelfield import create_model_field
-from ellar.services.reflector import Reflector
+from ellar.core.services.reflector import Reflector
 
-from ..constants import REF_PREFIX
 from .openapi_v3 import OpenAPI
 from .route_doc_models import (
     OpenAPIMountDocumentation,
     OpenAPIRoute,
     OpenAPIRouteDocumentation,
 )
+from .schemas import HTTPValidationError, ValidationError
 
 default_openapi_version = "3.0.2"
 
 
 class OpenAPIDocumentBuilder:
     def __init__(self) -> None:
         self._build: t.Dict = dict()
```

### Comparing `ellar-0.3.6/ellar/openapi/docs_generators/base.py` & `ellar-0.3.8/ellar/openapi/docs_generators/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/openapi/docs_generators/redocs.py` & `ellar-0.3.8/ellar/openapi/docs_generators/redocs.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/openapi/docs_generators/swagger.py` & `ellar-0.3.8/ellar/openapi/docs_generators/swagger.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/openapi/module.py` & `ellar-0.3.8/ellar/openapi/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing as t
 
-from ellar.common import Module, ModuleRouter, render
-from ellar.core import DynamicModule, IModuleSetup, ModuleBase
-from ellar.core.guard import GuardCanActivate
+from ellar.common import IModuleSetup, Module, ModuleRouter, render
+from ellar.common.models import GuardCanActivate
+from ellar.core import DynamicModule, ModuleBase
 from ellar.openapi.docs_generators import IDocumentationGenerator
 from ellar.openapi.openapi_v3 import OpenAPI
 
 __all__ = ["OpenAPIDocumentModule"]
 
 
 @Module(template_folder="templates")
```

### Comparing `ellar-0.3.6/ellar/openapi/openapi_v3.py` & `ellar-0.3.8/ellar/openapi/openapi_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing as t
 from enum import Enum
 
 from pydantic import AnyUrl, BaseModel, Field
 
-from ellar.compatible import EmailStr
-from ellar.serializer import Serializer, SerializerFilter
+from ellar.common.compatible import EmailStr
+from ellar.common.serializer import Serializer, SerializerFilter
 
 
 class Contact(BaseModel):
     name: t.Optional[str] = None
     url: t.Optional[AnyUrl] = None
     email: t.Optional[EmailStr] = None
```

### Comparing `ellar-0.3.6/ellar/openapi/route_doc_models.py` & `ellar-0.3.8/ellar/openapi/route_doc_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,31 +4,36 @@
 
 from pydantic import BaseModel
 from pydantic.fields import ModelField, Undefined
 from pydantic.schema import field_schema
 from starlette.routing import Mount, compile_path
 from starlette.status import HTTP_422_UNPROCESSABLE_ENTITY
 
-from ellar.compatible import AttributeDict, cached_property
-from ellar.constants import GUARDS_KEY, METHODS_WITH_BODY, OPENAPI_KEY, REF_PREFIX
-from ellar.core.guard import BaseAuthGuard
-from ellar.core.params.args import EndpointArgsModel
-from ellar.core.params.params import Body, Param
-from ellar.core.params.resolvers import (
+from ellar.common.compatible import AttributeDict, cached_property
+from ellar.common.constants import (
+    GUARDS_KEY,
+    METHODS_WITH_BODY,
+    OPENAPI_KEY,
+    REF_PREFIX,
+)
+from ellar.common.models import BaseAuthGuard
+from ellar.common.params.args import EndpointArgsModel
+from ellar.common.params.params import BodyFieldInfo as Body, ParamFieldInfo as Param
+from ellar.common.params.resolvers import (
     BaseRouteParameterResolver,
     BodyParameterResolver,
     BulkParameterResolver,
     RouteParameterModelField,
 )
-from ellar.core.routing import ModuleMount, RouteOperation
-from ellar.services.reflector import Reflector
-from ellar.shortcuts import normalize_path
+from ellar.common.routing import ModuleMount, RouteOperation
+from ellar.common.shortcuts import normalize_path
+from ellar.core.services.reflector import Reflector
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.core.guard import GuardCanActivate
+    from ellar.common import GuardCanActivate
 
 
 class OpenAPIRoute(ABC):
     @abstractmethod
     def get_route_models(self) -> t.List[t.Union[ModelField, RouteParameterModelField]]:
         pass
```

### Comparing `ellar-0.3.6/ellar/openapi/templates/redocs.html` & `ellar-0.3.8/ellar/openapi/templates/redocs.html`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/openapi/templates/swagger.html` & `ellar-0.3.8/ellar/openapi/templates/swagger.html`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/reflect.py` & `ellar-0.3.8/ellar/reflect/_reflect.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,40 @@
+import logging
 import typing as t
 from contextlib import contextmanager
 from inspect import ismethod
 from weakref import WeakKeyDictionary
 
-from ellar.compatible import AttributeDict, asynccontextmanager
-from ellar.constants import REFLECT_TYPE
-from ellar.shortcuts import fail_silently
+from .constants import REFLECT_TYPE
+from .contextmanager_fix import asynccontextmanager
+
+logger = logging.getLogger(__name__)
 
 
 def _get_actual_target(
     target: t.Union[t.Type, t.Callable]
 ) -> t.Union[t.Type, t.Callable]:
     try:
         reflect_type = target.__dict__[REFLECT_TYPE]
     except KeyError:
-        fail_silently(setattr, target, REFLECT_TYPE, target)
+        try:
+            setattr(target, REFLECT_TYPE, target)
+        except Exception as ex:  # pragma: no cover
+            logger.debug(f"Setting REFLECT_TYPE failed. \nError Message: {ex}")
         return target
     else:
         return t.cast(t.Union[t.Type, t.Callable], reflect_type)
 
 
 class _Reflect:
     __slots__ = ("_meta_data",)
 
     def __init__(self) -> None:
         self._meta_data: t.MutableMapping[
-            t.Union[t.Type, t.Callable], AttributeDict
+            t.Union[t.Type, t.Callable], t.Dict
         ] = WeakKeyDictionary()
 
     def define_metadata(
         self,
         metadata_key: str,
         metadata_value: t.Any,
         target: t.Union[t.Type, t.Callable],
@@ -100,32 +105,32 @@
     ) -> None:
         target_metadata = self._get_or_create_metadata(target)
         if target_metadata and metadata_key in target_metadata:
             target_metadata.pop(metadata_key)
 
     def _get_or_create_metadata(
         self, target: t.Union[t.Type, t.Callable], create: bool = False
-    ) -> t.Optional[AttributeDict]:
+    ) -> t.Optional[t.Dict]:
         _target = _get_actual_target(target)
         if _target in self._meta_data:
             return self._meta_data[_target]
 
         if create:
-            self._meta_data[_target] = AttributeDict()
+            self._meta_data[_target] = dict()
             return self._meta_data[_target]
         return None
 
     def _clone_meta_data(
         self,
-    ) -> t.MutableMapping[t.Union[t.Type, t.Callable], AttributeDict]:
+    ) -> t.MutableMapping[t.Union[t.Type, t.Callable], t.Dict]:
         _meta_data: t.MutableMapping[
-            t.Union[t.Type, t.Callable], AttributeDict
+            t.Union[t.Type, t.Callable], t.Dict
         ] = WeakKeyDictionary()
         for k, v in self._meta_data.items():
-            _meta_data[k] = AttributeDict(v)
+            _meta_data[k] = dict(v)
         return _meta_data
 
     @asynccontextmanager
     async def async_context(self) -> t.AsyncGenerator[None, None]:
         cached_meta_data = self._meta_data
         try:
             self._meta_data = self._clone_meta_data()
```

### Comparing `ellar-0.3.6/ellar/samples/static/css/bootstrap.min.css` & `ellar-0.3.8/ellar/samples/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/samples/static/img/EllarLogoB.png` & `ellar-0.3.8/ellar/samples/static/img/EllarLogoB.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/samples/static/img/EllarLogoIconOnly.png` & `ellar-0.3.8/ellar/samples/static/img/EllarLogoIconOnly.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/samples/static/img/Icon.svg` & `ellar-0.3.8/ellar/samples/static/img/Icon.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/samples/templates/home/index.html` & `ellar-0.3.8/ellar/samples/templates/home/index.html`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/serializer.py` & `ellar-0.3.8/ellar/common/serializer/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/services/reflector.py` & `ellar-0.3.8/ellar/core/services/reflector.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/ellar/testing/module.py` & `ellar-0.3.8/ellar/testing/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import typing as t
 from pathlib import Path
 from uuid import uuid4
 
 from starlette.testclient import TestClient as TestClient
 
 from ellar.common import Module
+from ellar.common.routing import ModuleRouter
+from ellar.common.types import T
 from ellar.core import ModuleBase
 from ellar.core.factory import AppFactory
 from ellar.core.main import App
-from ellar.core.routing import ModuleRouter
 from ellar.di import ProviderConfig
-from ellar.types import T
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.core import GuardCanActivate
+    from ellar.common import GuardCanActivate
 
 
 class TestingModule:
     def __init__(
         self,
         testing_module: t.Type[t.Union[ModuleBase, t.Any]],
         global_guards: t.List[
@@ -89,15 +89,15 @@
         template_folder: t.Optional[str] = None,
         base_directory: t.Optional[t.Union[str, Path]] = None,
         static_folder: str = "static",
         global_guards: t.List[
             t.Union[t.Type["GuardCanActivate"], "GuardCanActivate"]
         ] = None,
         config_module: t.Union[str, t.Dict] = None,
-    ) -> TestingModule:
+    ) -> TESTING_MODULE:  # type: ignore[valid-type]
         """
         Create a TestingModule to test controllers and services in isolation
         :param modules:
         :param controllers:
         :param routers:
         :param providers:
         :param template_folder:
```

### Comparing `ellar-0.3.6/ellar/types.py` & `ellar-0.3.8/ellar/common/types.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/examples/01-carapp/carapp/apps/car/controllers.py` & `ellar-0.3.8/examples/01-carapp/carapp/apps/car/controllers.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 @Controller("/dogs", tag="Dogs", description="Dogs Resources")
 class MyController(ControllerBase):
     @get('/')
     def index(self):
         return {'detail': "Welcome Dog's Resources"}
 """
 import typing_extensions as types
-from ellar.common import Body, Controller, Query, get, post, render, Version
-from ellar.core import ControllerBase
+from ellar.common import Body, Controller, Query, get, post, render, Version, ControllerBase
 
 from .schemas import CarListFilter, CreateCarSerializer
 from .services import CarRepository
 
 
 @Controller("/car", description='Example of Car Resource with <strong>Controller</strong>', tag='Controller')
 class CarController(ControllerBase):
```

### Comparing `ellar-0.3.6/examples/01-carapp/carapp/apps/car/module.py` & `ellar-0.3.8/examples/01-carapp/carapp/apps/car/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/examples/01-carapp/carapp/apps/car/routers.py` & `ellar-0.3.8/examples/01-carapp/carapp/apps/car/routers.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,18 +8,15 @@
 def index(request: Request):
     return {'detail': 'Welcome to Cats Resource'}
 """
 
 from dataclasses import dataclass
 from typing import List
 
-from ellar.common import Provide, render, Req
-from ellar.core.routing import ModuleRouter
-from ellar.core.templating import render_template
-from ellar.serializer import DataclassSerializer
+from ellar.common import Provide, render, Req, ModuleRouter, render_template, DataclassSerializer
 
 from .services import CarRepository
 
 router = ModuleRouter("/car-as-router", tag='Router', description='Example of car Resource from a <strong>ModuleRouter</strong>')
 
 
 @dataclass
```

### Comparing `ellar-0.3.6/examples/01-carapp/carapp/apps/car/schemas.py` & `ellar-0.3.8/examples/01-carapp/carapp/apps/car/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 for dataclasses, Inherit from DataclassSerializer
 
 @dataclass
 class ASampleDTO(DataclassSerializer):
     name: str
     age: t.Optional[int] = None
 """
-from ellar.serializer import DataclassSerializer, Serializer
+from ellar.common.serializer import DataclassSerializer, Serializer
 from pydantic import Field
 
 
 class CreateCarSerializer(Serializer):
     name: str
     year: int = Field(..., gt=0)
     model: str
```

### Comparing `ellar-0.3.6/examples/01-carapp/carapp/apps/car/services.py` & `ellar-0.3.8/examples/01-carapp/carapp/apps/car/services.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/examples/01-carapp/carapp/apps/car/statics/blog/blog.css` & `ellar-0.3.8/examples/01-carapp/carapp/apps/car/statics/blog/blog.css`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/examples/01-carapp/carapp/apps/car/statics/blog/blog.rtl.css` & `ellar-0.3.8/examples/01-carapp/carapp/apps/car/statics/blog/blog.rtl.css`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo-white.svg` & `ellar-0.3.8/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo-white.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo.svg` & `ellar-0.3.8/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/examples/01-carapp/carapp/apps/car/tests/test_controllers.py` & `ellar-0.3.8/examples/01-carapp/carapp/apps/car/tests/test_controllers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/examples/01-carapp/carapp/apps/car/tests/test_routers.py` & `ellar-0.3.8/examples/01-carapp/carapp/apps/car/tests/test_routers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/examples/01-carapp/carapp/apps/car/views/index.html` & `ellar-0.3.8/examples/01-carapp/carapp/apps/car/views/index.html`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/examples/01-carapp/carapp/root_module.py` & `ellar-0.3.8/examples/01-carapp/carapp/root_module.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from ellar.common import exception_handler
 from ellar.core import ModuleBase
-from ellar.core.context import IExecutionContext
-from ellar.core.response import JSONResponse, Response
+from ellar.common import IExecutionContext, JSONResponse, Response
 from ellar.samples.modules import HomeModule
 from ellar.common import Module
 from .commands import db, whatever_you_want
 from .apps.car.module import CarModule
 
 
 @Module(modules=[HomeModule, CarModule], commands=[db, whatever_you_want])
```

### Comparing `ellar-0.3.6/examples/01-carapp/carapp/server.py` & `ellar-0.3.8/examples/01-carapp/carapp/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from ellar.core.factory import AppFactory
 from ellar.openapi import OpenAPIDocumentModule, SwaggerDocumentGenerator, OpenAPIDocumentBuilder, ReDocDocumentGenerator
-from ellar.constants import ELLAR_CONFIG_MODULE
+from ellar.common.constants import ELLAR_CONFIG_MODULE
 from .root_module import ApplicationModule
 
 application = AppFactory.create_from_app_module(ApplicationModule, config_module=os.environ.get(
         ELLAR_CONFIG_MODULE, "carapp.config:DevelopmentConfig"
 ))
 
 document_builder = OpenAPIDocumentBuilder()
```

### Comparing `ellar-0.3.6/mkdocs.yml` & `ellar-0.3.8/mkdocs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -36,16 +36,16 @@
       scheme: slate
       primary: pink
       accent: pink
       toggle:
         icon: material/lightbulb-outline
         name: Switch to light mode
   font:
-    text: Roboto
-    code: Roboto Mono
+    text: Source Sans Pro
+    code: Fira Code
   language: en
   logo: img/Icon.svg
   favicon: img/Icon.svg
   icon:
     repo: fontawesome/brands/git-alt
 
 plugins:
@@ -97,15 +97,17 @@
         - create project: commands/create-project-command.md
         - create module: commands/create-module-command.md
         - runserver: commands/runserver-command.md
     - Custom Commands: commands/custom-commands.md
     - Command Grouping: commands/command-grouping.md
   - Versioning: basics/versioning.md
   - Testing: basics/testing.md
-  - WebSockets: websockets.md
+  - WebSockets:
+      - index: websockets/index.md
+      - socketio: websockets/socketio.md
   - Mount: mount.md
   - Background Tasks: background-task.md
   - Release Notes: release-notes.md
 
 markdown_extensions:
   - attr_list
   - toc:
```

#### html2text {}

```diff
@@ -6,38 +6,39 @@
 site theme: name: material features: - announce.dismiss - content.action.edit -
 content.action.view - content.code.annotate - content.code.copy -
 content.tooltips - search.highlight - search.share - search.suggest -
 toc.follow palette: - media: "(prefers-color-scheme: light)" scheme: default
 primary: pink accent: pink toggle: icon: material/lightbulb name: Switch to
 dark mode - media: "(prefers-color-scheme: dark)" scheme: slate primary: pink
 accent: pink toggle: icon: material/lightbulb-outline name: Switch to light
-mode font: text: Roboto code: Roboto Mono language: en logo: img/Icon.svg
-favicon: img/Icon.svg icon: repo: fontawesome/brands/git-alt plugins: - search:
-separator: '[\s\-,:!=\[\]()"`/]+|\.(?!\d)|&[lg]t;|(?!\b)(?=[A-Z][a-z])' -
-minify: minify_html: true - git-revision-date-localized: enable_creation_date:
-false nav: - Introduction: index.md - Overview: - Step One: overview/index.md -
-Controllers: overview/controllers.md - Providers: overview/providers.md -
-Modules: overview/modules.md - Middlewares: overview/middleware.md - Exception
-Handling: overview/exception_handling.md - Guards: overview/guards.md - Custom
-Decorators: overview/custom_decorators.md - Module Router: overview/module-
-router.md - Execution Context: basics/execution-context.md - Configuration:
-configurations.md - How-to Guides: - Input Parsing: parsing-inputs/index.md -
-Path: parsing-inputs/path-params.md - Query: parsing-inputs/query-params.md -
-Header: parsing-inputs/header-params.md - Cookie: parsing-inputs/cookie-
-params.md - Body: parsing-inputs/body.md - Form: parsing-inputs/form-params.md
-- File: parsing-inputs/file-params.md - Handling Response: - Response Schema:
-handling-response/response.md - Response Model: handling-response/response-
-model.md - Templating: - html: templating/templating.md - Static Files:
-templating/staticfiles.md - Caching: caching.md - Rate Limiting: throttling.md
-# - Injection Scopes: basics/injection-scope.md # - Events: basics/events.md -
-Commands: - Introduction: commands/index.md - CLI Commands: - new: commands/
-new-command.md - create project: commands/create-project-command.md - create
-module: commands/create-module-command.md - runserver: commands/runserver-
-command.md - Custom Commands: commands/custom-commands.md - Command Grouping:
-commands/command-grouping.md - Versioning: basics/versioning.md - Testing:
-basics/testing.md - WebSockets: websockets.md - Mount: mount.md - Background
-Tasks: background-task.md - Release Notes: release-notes.md
+mode font: text: Source Sans Pro code: Fira Code language: en logo: img/
+Icon.svg favicon: img/Icon.svg icon: repo: fontawesome/brands/git-alt plugins:
+- search: separator: '[\s\-,:!=\[\]()"`/]+|\.(?!\d)|&[lg]t;|(?!\b)(?=[A-Z][a-
+z])' - minify: minify_html: true - git-revision-date-localized:
+enable_creation_date: false nav: - Introduction: index.md - Overview: - Step
+One: overview/index.md - Controllers: overview/controllers.md - Providers:
+overview/providers.md - Modules: overview/modules.md - Middlewares: overview/
+middleware.md - Exception Handling: overview/exception_handling.md - Guards:
+overview/guards.md - Custom Decorators: overview/custom_decorators.md - Module
+Router: overview/module-router.md - Execution Context: basics/execution-
+context.md - Configuration: configurations.md - How-to Guides: - Input Parsing:
+parsing-inputs/index.md - Path: parsing-inputs/path-params.md - Query: parsing-
+inputs/query-params.md - Header: parsing-inputs/header-params.md - Cookie:
+parsing-inputs/cookie-params.md - Body: parsing-inputs/body.md - Form: parsing-
+inputs/form-params.md - File: parsing-inputs/file-params.md - Handling
+Response: - Response Schema: handling-response/response.md - Response Model:
+handling-response/response-model.md - Templating: - html: templating/
+templating.md - Static Files: templating/staticfiles.md - Caching: caching.md -
+Rate Limiting: throttling.md # - Injection Scopes: basics/injection-scope.md #
+- Events: basics/events.md - Commands: - Introduction: commands/index.md - CLI
+Commands: - new: commands/new-command.md - create project: commands/create-
+project-command.md - create module: commands/create-module-command.md -
+runserver: commands/runserver-command.md - Custom Commands: commands/custom-
+commands.md - Command Grouping: commands/command-grouping.md - Versioning:
+basics/versioning.md - Testing: basics/testing.md - WebSockets: - index:
+websockets/index.md - socketio: websockets/socketio.md - Mount: mount.md -
+Background Tasks: background-task.md - Release Notes: release-notes.md
 markdown_extensions: - attr_list - toc: permalink: true - admonition - def_list
 - tables - abbr - footnotes - md_in_html - codehilite - pymdownx.superfences:
 custom_fences: - name: mermaid class: mermaid - pymdownx.details -
 pymdownx.tabbed: alternate_style: true - pymdownx.saneheaders extra_css: -
 stylesheets/extra.css
```

### Comparing `ellar-0.3.6/mypy.ini` & `ellar-0.3.8/mypy.ini`

 * *Files 9% similar despite different names*

```diff
@@ -14,24 +14,21 @@
 warn_redundant_casts = True
 warn_unused_ignores = True
 
 disallow_untyped_defs = True
 check_untyped_defs = True
 implicit_reexport = False
 
-[mypy-ellar.compatible.*]
+[mypy-ellar.common.compatible.*]
 ignore_errors = True
 
 [mypy-ellar.core.services.*]
 ignore_errors = True
 
 [mypy-ellar.cli.*]
 ignore_errors = True
 
-[mypy-ellar.core.schema.*]
-ignore_errors = True
-
 [mypy-ellar.__main__.*]
 ignore_errors = True
 
 [mypy-ellar.samples.*]
 ignore_errors = True
```

### Comparing `ellar-0.3.6/pyproject.toml` & `ellar-0.3.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -72,35 +72,38 @@
     "anyio[trio] >= 3.2.1",
     "autoflake",
     "email_validator >=1.1.1",
     "pylibmc",
     "pymemcache",
     "aiomcache",
     "redis",
-
+    "itsdangerous >=1.1.0,<3.0.0",
     # types
-    "types-ujson ==5.7.0.1",
+    "types-ujson ==5.7.0.5",
     "types-orjson ==3.6.2",
     "types-dataclasses ==0.6.6",
+    "python-socketio",
+    "uvicorn[standard] == 0.20.0",
+    "aiohttp == 3.8.4",
 ]
 dev = [
     "pre-commit"
 ]
 
 all = [
     "python-multipart >=0.0.5,<0.0.7",
     "itsdangerous >=1.1.0,<3.0.0",
     "pyyaml >=5.3.1,<7.0.0",
     "ujson >=4.0.1,!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0",
     "orjson >=3.2.1,<4.0.0",
-    "email_validator >=1.1.1,<2.0.0",
+    "email_validator >=1.1.1,<3.0.0",
 ]
 doc = [
     "mkdocs >=1.1.2,<2.0.0",
-    "mkdocs-material >=7.1.9,<9.0.0",
+    "mkdocs-material >=7.1.9,<10.0.0",
     "mdx-include >=1.4.1,<2.0.0",
     "mkdocs-markdownextradata-plugin >=0.1.7,<0.3.0",
     "markdown-include",
     "mkdocstrings",
     "mkdocs-minify-plugin",
     "mkdocs-git-revision-date-localized-plugin"
 ]
```

### Comparing `ellar-0.3.6/tests/conftest.py` & `ellar-0.3.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/injector_module.py` & `ellar-0.3.8/tests/injector_module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/main.py` & `ellar-0.3.8/tests/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import Optional
 from uuid import UUID
 
 from pydantic import Field
 
-from ellar.common import ModuleRouter, Path, Query
+from ellar.common import ModuleRouter, Path, Query, Serializer
 from ellar.core.connection import Request
 from ellar.core.factory import AppFactory
-from ellar.core.schema import Schema
 
 router = ModuleRouter("")
 
 
 @router.get("/root")
 def non_operation():
     return {"message": "Hello World"}
@@ -201,15 +200,15 @@
 
 @router.get("/query/param-required/int")
 def get_query_param_required_type(query: int = Query(...)):
     assert isinstance(query, int)
     return f"foo bar {query}"
 
 
-class AliasedSchema(Schema):
+class AliasedSchema(Serializer):
     query: str = Field(..., alias="aliased.-_~name")
 
 
 @router.get("/query/aliased-name")
 def get_query_aliased_name(query: AliasedSchema = Query(..., alias="aliased.-_~name")):
     return f"foo bar {query.query}"
```

### Comparing `ellar-0.3.6/tests/test_application/sample.py` & `ellar-0.3.8/tests/test_application/sample.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 
 from starlette.exceptions import HTTPException
 from starlette.responses import JSONResponse, PlainTextResponse
 from starlette.routing import Host, Mount, Route, Router
 
 from ellar.common import Controller, Module, ModuleRouter, exception_handler, get
-from ellar.core.connection import Request, WebSocket
-from ellar.core.guard import APIKeyQuery
+from ellar.core import APIKeyQuery, ModuleBase, Request, WebSocket
 
 
 def create_tmp_template_and_static_dir(tmpdir):
     template_folder = os.path.join(tmpdir, "templates")
     os.mkdir(template_folder)
     static_folder = os.path.join(tmpdir, "statics")
     os.mkdir(static_folder)
@@ -92,15 +91,15 @@
     routers=[
         Host("{subdomain}.example.org", app=sub_domain),
         Mount("/users", app=users),
         router,
     ],
     controllers=[ClassBaseController],
 )
-class ApplicationModule:
+class ApplicationModule(ModuleBase):
     @exception_handler(405)
     async def method_not_allow_exception(self, ctx, exec):
         return JSONResponse({"detail": "Custom message"}, status_code=405)
 
     @exception_handler(500)
     async def error_500(self, ctx, exec):
         return JSONResponse({"detail": "Server Error"}, status_code=500)
```

### Comparing `ellar-0.3.6/tests/test_application/test_application_factory.py` & `ellar-0.3.8/tests/test_application/test_application_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import pytest
 from starlette.routing import Host, Mount
 
 from ellar.common import Module
+from ellar.common.constants import MODULE_WATERMARK
 from ellar.core import AppFactory, Config, ModuleBase, ModuleSetup
 from ellar.di import EllarInjector
+from ellar.reflect import reflect
 from ellar.testing import TestClient
 
 from .sample import (
     AppAPIKey,
     ApplicationModule,
     ClassBaseController,
     create_tmp_template_and_static_dir,
@@ -69,15 +71,16 @@
     )
 
 
 def test_factory_create_app_dynamically_creates_module():
     app = AppFactory.create_app()
     first_module_ref = next(app.get_module_loaders())
     module_instance = first_module_ref.get_module_instance()
-    assert isinstance(module_instance, ModuleBase)
+    assert not isinstance(module_instance, ModuleBase)
+    assert reflect.get_metadata(MODULE_WATERMARK, type(module_instance))
     assert "ellar.core.factory.Module" in str(module_instance.__class__)
 
 
 def test_factory_create_app_works(tmpdir):
     create_tmp_template_and_static_dir(tmpdir)
 
     @Module()
```

### Comparing `ellar-0.3.6/tests/test_application/test_application_functions.py` & `ellar-0.3.8/tests/test_application/test_application_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 import os
 import typing as t
 
 from starlette.responses import JSONResponse, PlainTextResponse, Response
 
-from ellar.common import Module, get, template_filter, template_global
-from ellar.compatible import asynccontextmanager
+from ellar.common import (
+    IExceptionHandler,
+    IExecutionContext,
+    Module,
+    get,
+    template_filter,
+    template_global,
+)
+from ellar.common.helper.importer import get_class_import
+from ellar.common.templating import Environment
 from ellar.core import App, AppFactory, Config, ModuleBase
 from ellar.core.connection import Request
-from ellar.core.context import IExecutionContext
 from ellar.core.core_service_registration import CoreServiceRegistration
-from ellar.core.exceptions.interfaces import IExceptionHandler
 from ellar.core.modules import ModuleTemplateRef
+from ellar.core.services.reflector import Reflector
 from ellar.core.staticfiles import StaticFiles
-from ellar.core.templating import Environment
 from ellar.core.versioning import (
     DefaultAPIVersioning,
     UrlPathAPIVersioning,
     VersioningSchemes as VERSIONING,
 )
 from ellar.di import EllarInjector
-from ellar.helper.importer import get_class_import
 from ellar.openapi import OpenAPIDocumentModule
-from ellar.services.reflector import Reflector
+from ellar.reflect import asynccontextmanager
 from ellar.testing import Test, TestClient
 
 from .config import ConfigTrustHostConfigure
 from .sample import AppAPIKey, ApplicationModule
 
 test_module = Test.create_test_module(
     modules=(ApplicationModule,),
```

### Comparing `ellar-0.3.6/tests/test_application/test_cors.py` & `ellar-0.3.8/tests/test_application/test_cors.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_application/test_replacing_app_services.py` & `ellar-0.3.8/tests/test_application/test_replacing_app_services.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from starlette.exceptions import HTTPException
 from starlette.responses import PlainTextResponse
 
-from ellar.common import Controller, Module, exception_handler, get
-from ellar.core.context import (
-    ExecutionContext,
-    HostContext,
+from ellar.common import (
+    Controller,
+    IExceptionMiddlewareService,
     IExecutionContext,
     IExecutionContextFactory,
     IHostContext,
     IHostContextFactory,
+    Module,
+    exception_handler,
+    get,
 )
-from ellar.core.exceptions import IExceptionMiddlewareService
+from ellar.core import ModuleBase
+from ellar.core.context import ExecutionContext, HostContext
 from ellar.core.exceptions.service import ExceptionMiddlewareService
+from ellar.core.services import Reflector
 from ellar.di import ProviderConfig, injectable
-from ellar.services import Reflector
 from ellar.testing import Test
 
 
 @Controller
 class ExampleController:
     @get()
     def index(self):
@@ -97,15 +100,15 @@
         controllers=[ExampleController],
         providers=[
             ProviderConfig(
                 IExceptionMiddlewareService, use_class=NewExceptionMiddlewareService
             )
         ],
     )
-    class ExampleModule:
+    class ExampleModule(ModuleBase):
         @exception_handler(400)
         def exception_400(self, context: IHostContext, exc: Exception):
             return PlainTextResponse(
                 "Exception 400 handled by ExampleModule.exception_400"
             )
 
     tm = Test.create_test_module(modules=[ExampleModule])
```

### Comparing `ellar-0.3.6/tests/test_application/test_trusted_host.py` & `ellar-0.3.8/tests/test_application/test_trusted_host.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_attribute_dict.py` & `ellar-0.3.8/tests/test_attribute_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ellar.compatible.dict import AttributeDict
+from ellar.common.compatible import AttributeDict
 
 
 class MyDict(AttributeDict):
     pass
 
 
 def test_set_value_for_attribute_dict_type():
```

### Comparing `ellar-0.3.6/tests/test_cache/_test_aio_memcache.py.ellar` & `ellar-0.3.8/tests/test_cache/_test_aio_memcache.py.ellar`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_cache/pylib_mock.py` & `ellar-0.3.8/tests/test_cache/pylib_mock.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_cache/redis_mock.py` & `ellar-0.3.8/tests/test_cache/redis_mock.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_cache/test_cache_decorator.py` & `ellar-0.3.8/tests/test_cache/test_cache_decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from time import sleep
 
 from ellar.cache import CacheModule, cache
-from ellar.common import ModuleRouter
-from ellar.core.response import PlainTextResponse
+from ellar.common import ModuleRouter, PlainTextResponse
 from ellar.testing import Test
 
 
 def test_cache_route_function_return_data():
     called_count = 0
 
     mr = ModuleRouter()
```

### Comparing `ellar-0.3.6/tests/test_cache/test_cache_many_config.py` & `ellar-0.3.8/tests/test_cache/test_cache_many_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from ellar.cache import CacheModule, ICacheService, cache
 from ellar.cache.backends.local_cache import LocalMemCacheBackend
-from ellar.common import Controller, get
-from ellar.core.response import PlainTextResponse
+from ellar.common import Controller, PlainTextResponse, get
 from ellar.testing import Test
 
 
 @Controller("")
 class ExampleController:
     @get("/index-1")
     @cache(ttl=1, backend="another")
```

### Comparing `ellar-0.3.6/tests/test_cache/test_cache_service.py` & `ellar-0.3.8/tests/test_cache/test_cache_service.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_cache/test_local_cache.py` & `ellar-0.3.8/tests/test_cache/test_local_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_cache/test_module_setup.py` & `ellar-0.3.8/tests/test_cache/test_module_setup.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_cache/test_pylibmc_cache.py` & `ellar-0.3.8/tests/test_cache/test_pylibmc_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_cache/test_redis_cache.py` & `ellar-0.3.8/tests/test_cache/test_redis_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_cache/test_schema.py` & `ellar-0.3.8/tests/test_cache/test_schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_common/test_decorators/test_controller.py` & `ellar-0.3.8/tests/test_decorators/test_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import pytest
 
-from ellar.common import Controller, Guards, Version, set_metadata
-from ellar.constants import CONTROLLER_METADATA, GUARDS_KEY, NOT_SET, VERSIONING_KEY
-from ellar.core import ControllerBase
-from ellar.core.exceptions import ImproperConfiguration
+from ellar.common import Controller, ControllerBase, Guards, Version, set_metadata
+from ellar.common.constants import (
+    CONTROLLER_METADATA,
+    GUARDS_KEY,
+    NOT_SET,
+    VERSIONING_KEY,
+)
+from ellar.common.exceptions import ImproperConfiguration
 from ellar.reflect import reflect
 
 
 @set_metadata("OtherAttributes", "Something")
 @Controller(
     prefix="/decorator",
     description="Some description",
```

### Comparing `ellar-0.3.6/tests/test_common/test_decorators/test_exception.py` & `ellar-0.3.8/tests/test_decorators/test_exception.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ellar.common import exception_handler
-from ellar.constants import EXCEPTION_HANDLERS_KEY
+from ellar.common.constants import EXCEPTION_HANDLERS_KEY
 
 
 class CustomException(Exception):
     pass
 
 
 @exception_handler(CustomException)
```

### Comparing `ellar-0.3.6/tests/test_common/test_decorators/test_file.py` & `ellar-0.3.8/tests/test_decorators/test_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import pytest
 
 from ellar.common import Controller, file, get
-from ellar.constants import CONTROLLER_OPERATION_HANDLER_KEY, RESPONSE_OVERRIDE_KEY
-from ellar.core.connection import Request
-from ellar.core.response.model import (
+from ellar.common.constants import (
+    CONTROLLER_OPERATION_HANDLER_KEY,
+    RESPONSE_OVERRIDE_KEY,
+)
+from ellar.common.responses.models import (
     FileResponseModel,
     ResponseModelField,
     StreamingResponseModel,
 )
+from ellar.core import Request
 from ellar.reflect import reflect
 
 
 def test_file_decorator_works():
     @file(media_type="text/javascript")
     def endpoint_file(request: Request):
         """ignore"""
```

### Comparing `ellar-0.3.6/tests/test_common/test_decorators/test_guards.py` & `ellar-0.3.8/tests/test_decorators/test_guards.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-from ellar.common import Guards
-from ellar.constants import GUARDS_KEY
-from ellar.core import ExecutionContext
-from ellar.core.connection import Request
-from ellar.core.guard import GuardCanActivate
+from ellar.common import GuardCanActivate, Guards
+from ellar.common.constants import GUARDS_KEY
+from ellar.core import ExecutionContext, Request
 from ellar.reflect import reflect
 
 
 class SomeGuard(GuardCanActivate):
     async def can_activate(self, context: ExecutionContext) -> bool:
         return True  # pragma: no cover
```

### Comparing `ellar-0.3.6/tests/test_common/test_decorators/test_html.py` & `ellar-0.3.8/tests/test_decorators/test_html.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pytest
 
 from ellar.common import Controller, get, render, template_filter, template_global
-from ellar.common.decorators.html import RenderDecoratorException
-from ellar.constants import (
+from ellar.common.constants import (
     CONTROLLER_OPERATION_HANDLER_KEY,
     RESPONSE_OVERRIDE_KEY,
     TEMPLATE_FILTER_KEY,
     TEMPLATE_GLOBAL_KEY,
 )
-from ellar.core.connection import Request
-from ellar.core.exceptions import ImproperConfiguration
-from ellar.core.response.model import HTMLResponseModel
-from ellar.core.templating import TemplateFunctionData
+from ellar.common.decorators.html import RenderDecoratorException
+from ellar.common.exceptions import ImproperConfiguration
+from ellar.common.responses.models import HTMLResponseModel
+from ellar.common.templating import TemplateFunctionData
+from ellar.core import Request
 from ellar.reflect import reflect
 
 
 def test_render_decorator_works():
     @render("index")
     def endpoint_render(request: Request):
         pass  # pragma: no cover
```

### Comparing `ellar-0.3.6/tests/test_common/test_decorators/test_middleware.py` & `ellar-0.3.8/tests/test_decorators/test_middleware.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from ellar.common import middleware
-from ellar.constants import MIDDLEWARE_HANDLERS_KEY
-from ellar.core.middleware import FunctionBasedMiddleware
-from ellar.core.middleware.schema import MiddlewareSchema
+from ellar.common.compatible import AttributeDict
+from ellar.common.constants import MIDDLEWARE_HANDLERS_KEY
 
 
 @middleware()
 def middleware_function_test():
     pass  # pragma: no cover
 
 
 def test_middleware_decorator_works():
     assert hasattr(middleware_function_test, MIDDLEWARE_HANDLERS_KEY)
-    middleware_detail: MiddlewareSchema = getattr(
+    middleware_detail: AttributeDict = getattr(
         middleware_function_test, MIDDLEWARE_HANDLERS_KEY
     )
-    assert middleware_detail.middleware_class is FunctionBasedMiddleware
     assert middleware_detail.dispatch is middleware_function_test
+    assert middleware_detail.options == {}
```

### Comparing `ellar-0.3.6/tests/test_common/test_decorators/test_modules.py` & `ellar-0.3.8/tests/test_decorators/test_modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
 from ellar.common import Module
-from ellar.constants import MODULE_METADATA, MODULE_WATERMARK
-from ellar.core.exceptions import ImproperConfiguration
+from ellar.common.constants import MODULE_METADATA, MODULE_WATERMARK
+from ellar.common.exceptions import ImproperConfiguration
 from ellar.di import has_binding, is_decorated_with_injectable
 from ellar.reflect import reflect
 
 
 @Module(
     name="test",
     static_folder="test",
@@ -43,15 +43,15 @@
     assert reflect.get_metadata(MODULE_WATERMARK, ModuleDecoratorTest)
 
 
 def test_base_directory_is_dynamically_set_when_none():
     base_path = reflect.get_metadata(
         MODULE_METADATA.BASE_DIRECTORY, ModuleDecoratorTest
     )
-    assert "/test_common/test_decorators" in str(base_path)
+    assert "/test_decorators" in str(base_path)
 
 
 def test_cannot_decorate_module_class_twice():
     with pytest.raises(
         ImproperConfiguration, match="is already identified as a Module"
     ):
         Module()(ModuleDecoratorTest)
```

### Comparing `ellar-0.3.6/tests/test_common/test_decorators/test_openapi.py` & `ellar-0.3.8/tests/test_decorators/test_openapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ellar.common import openapi_info
-from ellar.compatible import AttributeDict
-from ellar.constants import OPENAPI_KEY
+from ellar.common.compatible import AttributeDict
+from ellar.common.constants import OPENAPI_KEY
 from ellar.core.connection import Request
 from ellar.reflect import reflect
 
 
 @openapi_info(
     summary="Endpoint Summary",
     description="Endpoint Description",
```

### Comparing `ellar-0.3.6/tests/test_common/test_decorators/test_serializer.py` & `ellar-0.3.8/tests/test_decorators/test_serializer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ellar.common import serializer_filter
-from ellar.constants import SERIALIZER_FILTER_KEY
+from ellar.common.constants import SERIALIZER_FILTER_KEY
+from ellar.common.serializer import SerializerFilter
 from ellar.reflect import reflect
-from ellar.serializer import SerializerFilter
 
 
 @serializer_filter(
     include={"test1", "test2"},
     exclude_none=True,
     by_alias=False,
     exclude={"exclude1", "exclude2"},
```

### Comparing `ellar-0.3.6/tests/test_conf/test_default_conf.py` & `ellar-0.3.8/tests/test_conf/test_default_conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 import pytest
 from pydantic.json import ENCODERS_BY_TYPE
 from starlette.responses import JSONResponse
 
-from ellar.constants import ELLAR_CONFIG_MODULE
+from ellar.common.constants import ELLAR_CONFIG_MODULE
 from ellar.core.conf import Config, ConfigDefaultTypesMixin
 from ellar.core.conf.config import ConfigRuntimeError
 from ellar.core.versioning import DefaultAPIVersioning, UrlPathAPIVersioning
 
 
 class ConfigTesting(ConfigDefaultTypesMixin):
     DEBUG: bool = True
```

### Comparing `ellar-0.3.6/tests/test_conf/test_mixins.py` & `ellar-0.3.8/tests/test_conf/test_mixins.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_controller/test_controller_decorator.py` & `ellar-0.3.8/tests/test_controller/test_controller_decorator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import pytest
 
-from ellar.common import Controller, get, http_route, ws_route
-from ellar.constants import CONTROLLER_CLASS_KEY, CONTROLLER_OPERATION_HANDLER_KEY
-from ellar.core import ControllerBase
-from ellar.core.routing.router.module import controller_router_factory
+from ellar.common import Controller, ControllerBase, get, http_route, ws_route
+from ellar.common.constants import (
+    CONTROLLER_CLASS_KEY,
+    CONTROLLER_OPERATION_HANDLER_KEY,
+)
+from ellar.common.routing import ControllerRouterFactory
 from ellar.di import has_binding, is_decorated_with_injectable
 from ellar.reflect import reflect
 
 from .sample import SampleController
 
 
 @Controller(prefix="/items/{orgID:int}", name="override_name", tag="new_tag")
@@ -54,15 +56,15 @@
         assert controller_type == SampleController
 
 
 def test_controller_computed_properties():
     assert isinstance(SampleController, type) and issubclass(
         SampleController, ControllerBase
     )
-    router = controller_router_factory(SampleController)
+    router = ControllerRouterFactory.build(SampleController)
 
     assert is_decorated_with_injectable(SampleController)
     assert not has_binding(SampleController)
 
     assert router.get_meta() == {
         "tag": "sample",
         "external_doc_description": None,
@@ -77,45 +79,45 @@
         external_doc_url="https://test.com",
         external_doc_description="Find out more here",
     )
     class SomeControllerB(ControllerBase):
         def __init__(self, a: str):
             self.a = a
 
-    router = controller_router_factory(SomeControllerB)
+    router = ControllerRouterFactory.build(SomeControllerB)
     assert router.get_meta() == {
         "tag": "Item",
         "description": "Some Controller",
         "external_doc_description": "Find out more here",
         "external_doc_url": "https://test.com",
     }
     assert is_decorated_with_injectable(SomeControllerB)
     assert has_binding(SomeControllerB)
 
 
 def test_tag_configuration_controller_decorator():
     new_controller = Controller(
         prefix="/items/{orgID:int}", name="override_name", tag="new_tag"
     )(type("SomeControllerX", (ControllerBase,), {}))
-    router = controller_router_factory(new_controller)
+    router = ControllerRouterFactory.build(new_controller)
     assert router.get_meta()["tag"] == "new_tag"
     assert router.name == "override_name"
 
     # defaults to controller name
     new_controller = Controller(
         prefix="/items/{orgID:int}",
     )(type("SomeControllerY", (ControllerBase,), {}))
-    router = controller_router_factory(new_controller)
+    router = ControllerRouterFactory.build(new_controller)
     assert router.get_meta()["tag"] == "somey"
     assert router.name == "somey"
 
     new_controller = Controller(prefix="/items/{orgID:int}", tag="new_tag")(
         type("SomeControllerZ", (ControllerBase,), {})
     )
-    router = controller_router_factory(new_controller)
+    router = ControllerRouterFactory.build(new_controller)
     assert router.get_meta()["tag"] == "new_tag"
     assert router.name == "somez"
 
 
 @pytest.mark.parametrize(
     "controller_type, tag, prefix, name",
     [
@@ -125,11 +127,11 @@
             "new_tag",
             "/items/{orgID:int}",
             "override_name",
         ),
     ],
 )
 def test_controller_url_reverse(controller_type, tag, prefix, name):
-    router = controller_router_factory(controller_type)
+    router = ControllerRouterFactory.build(controller_type)
     for route in router.routes:
         reversed_path = router.url_path_for(f"{name}:{route.name}")
         assert reversed_path == router.path_format.replace("/{path}", route.path)
```

### Comparing `ellar-0.3.6/tests/test_controller/test_controller_inheritance.py` & `ellar-0.3.8/tests/test_controller/test_controller_inheritance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 
 from ellar.common import Controller, get, ws_route
-from ellar.constants import CONTROLLER_CLASS_KEY
+from ellar.common.constants import CONTROLLER_CLASS_KEY
+from ellar.common.routing import ControllerRouterFactory
 from ellar.core import AppFactory
-from ellar.core.routing.router.module import controller_router_factory
 from ellar.reflect import reflect
 
 
 class ControllerImplementationBase:
     @get("/sample")
     def some_example(self):
         pass
@@ -45,15 +45,15 @@
     reflect.define_metadata(
         CONTROLLER_CLASS_KEY,
         None,
         AnotherSampleController.endpoint_once,
     )
 
     with pytest.raises(Exception, match=r"Operation must have a single control type."):
-        controller_router_factory(AnotherSampleController)
+        ControllerRouterFactory.build(AnotherSampleController)
 
 
 def test_controller_raise_exception_for_controller_operation_without_controller_class(
     test_client_factory,
 ):
     @Controller("/abcd")
     class Another2SampleController:
```

### Comparing `ellar-0.3.6/tests/test_controller/test_module_router.py` & `ellar-0.3.8/tests/test_controller/test_module_router.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from ellar.core.routing import ModuleRouter
+from ellar.common.routing import ModuleRouter
 
 from .sample import router
 
 another_router = ModuleRouter("/prefix/another", tag="another_router", name="arouter")
 
 
 @another_router.get("/sample")
```

### Comparing `ellar-0.3.6/tests/test_controller/test_route_collection.py` & `ellar-0.3.8/tests/test_controller/test_route_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from typing import List
 
 import pytest
 from starlette.responses import JSONResponse
 from starlette.routing import Host, Mount
 
 from ellar.common import Version as version_decorator, get, http_route, ws_route
-from ellar.constants import CONTROLLER_CLASS_KEY, CONTROLLER_OPERATION_HANDLER_KEY
-from ellar.core.routing import RouteOperation, WebsocketRouteOperation
-from ellar.core.routing.router import RouteCollection
+from ellar.common.constants import (
+    CONTROLLER_CLASS_KEY,
+    CONTROLLER_OPERATION_HANDLER_KEY,
+)
+from ellar.common.helper import generate_controller_operation_unique_id
+from ellar.common.routing import (
+    RouteCollection,
+    RouteOperation,
+    WebsocketRouteOperation,
+)
 from ellar.core.versioning import UrlPathAPIVersioning
-from ellar.helper import generate_controller_operation_unique_id
 from ellar.reflect import reflect
 from ellar.testing import Test
 
 
 class Configuration:
     VERSIONING_SCHEME = UrlPathAPIVersioning()
```

### Comparing `ellar-0.3.6/tests/test_di/examples.py` & `ellar-0.3.8/tests/test_di/examples.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_di/test_injectable_resolving.py` & `ellar-0.3.8/tests/test_di/test_injectable_resolving.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_di/test_injector.py` & `ellar-0.3.8/tests/test_di/test_injector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,68 @@
 from collections import OrderedDict
 
 import pytest
 from injector import Binder, Injector, UnsatisfiedRequirement
 
 from ellar.common import Module
-from ellar.constants import MODULE_REF_TYPES, SCOPED_CONTEXT_VAR
 from ellar.core import Config, ModuleBase
 from ellar.core.modules.ref import create_module_ref_factor
-from ellar.di import Container, EllarInjector
+from ellar.di import MODULE_REF_TYPES, SCOPED_CONTEXT_VAR, Container, EllarInjector
 from ellar.di.providers import ClassProvider, InstanceProvider
 
 from .examples import Foo, Foo1, Foo2
 
 
 class EllarTestPlainModule(ModuleBase):
     pass
 
 
 @Module(template_folder="some_template")
 class EllarTestTemplateModule(ModuleBase):
     pass
 
 
-def test_container_install_module():
+def test_container_install_module_case_1():
     called = False
     app_container = EllarInjector().container
 
     class FakeModule(ModuleBase):
         def register_services(self, container: Container) -> None:
             nonlocal called
             called = True
 
     @Module()
-    class DecoratedModule:
+    class DecoratedModuleWithBase(ModuleBase):
         def register_services(self, container: Container) -> None:
             nonlocal called
             called = True
 
     fake_module = app_container.install(FakeModule)
     assert called
     assert isinstance(fake_module, FakeModule)
 
     called = False
 
-    decorated_module = app_container.install(DecoratedModule)
+    decorated_module = app_container.install(DecoratedModuleWithBase)
     assert called
+    assert isinstance(decorated_module, DecoratedModuleWithBase)
+
+
+def test_container_install_module_return_case_2():
+    called = False
+    app_container = EllarInjector().container
+
+    @Module()
+    class DecoratedModule:
+        def register_services(self, container: Container) -> None:
+            nonlocal called
+            called = True
+
+    decorated_module = app_container.install(DecoratedModule)
+    assert called is False
     assert isinstance(decorated_module, DecoratedModule)
 
 
 def test_default_container_registration():
     injector = EllarInjector(auto_bind=False)
     assert isinstance(injector.get(Container), Container)
     assert isinstance(injector.get(EllarInjector), EllarInjector)
```

### Comparing `ellar-0.3.6/tests/test_di/test_provider_scopes.py` & `ellar-0.3.8/tests/test_di/test_provider_scopes.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_di/test_providers.py` & `ellar-0.3.8/tests/test_di/test_providers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_events.py` & `ellar-0.3.8/tests/test_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from ellar.constants import NOT_SET
+from ellar.common.constants import NOT_SET
 from ellar.core import Config
 from ellar.events import EventHandler, RouterEventManager
 
 
 @pytest.mark.anyio
 async def test_router_event_manager():
     called = 0
```

### Comparing `ellar-0.3.6/tests/test_exceptions/test_api_exception.py` & `ellar-0.3.8/tests/test_exceptions/test_api_exception.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import http
 
 import pytest
 
 from ellar.common import get
-from ellar.core.exceptions import (
+from ellar.common.exceptions import (
     APIException,
     AuthenticationFailed,
     MethodNotAllowed,
     NotAcceptable,
     NotAuthenticated,
     NotFound,
     PermissionDenied,
```

### Comparing `ellar-0.3.6/tests/test_exceptions/test_custom_exceptions.py` & `ellar-0.3.8/tests/test_exceptions/test_custom_exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 from unittest.mock import patch
 
 import pytest
 from pydantic.error_wrappers import ValidationError
 from starlette.exceptions import HTTPException
 from starlette.responses import JSONResponse, Response
 
-from ellar.common import get
+from ellar.common import IExceptionHandler, IHostContext, get
+from ellar.common.exceptions.callable_exceptions import CallableExceptionHandler
+from ellar.common.exceptions.handlers import APIException, APIExceptionHandler
 from ellar.core import Config
-from ellar.core.context import IHostContext
-from ellar.core.exceptions.callable_exceptions import CallableExceptionHandler
-from ellar.core.exceptions.handlers import APIException, APIExceptionHandler
-from ellar.core.exceptions.interfaces import IExceptionHandler
 from ellar.core.exceptions.service import ExceptionMiddlewareService
 from ellar.core.middleware import ExceptionMiddleware
 from ellar.testing import Test
 
 
 class InvalidExceptionHandler:
     pass
```

### Comparing `ellar-0.3.6/tests/test_exceptions/test_error_details.py` & `ellar-0.3.8/tests/test_exceptions/test_error_details.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_exceptions/test_validation_exception.py` & `ellar-0.3.8/tests/test_exceptions/test_validation_exception.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 from pydantic.error_wrappers import ErrorWrapper
 
 from ellar.common import Ws, WsBody, get, ws_route
-from ellar.core.exceptions.validation import (
+from ellar.common.exceptions.validation import (
     RequestValidationError,
     WebSocketRequestValidationError,
 )
 from ellar.testing import Test
 
 from .exception_runner import ExceptionRunner
```

### Comparing `ellar-0.3.6/tests/test_guard.py` & `ellar-0.3.8/tests/test_guard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import pytest
 from starlette.status import HTTP_401_UNAUTHORIZED
 
-from ellar.common import Guards, Req, get
-from ellar.core import AppFactory
-from ellar.core.exceptions import APIException
+from ellar.common import APIException, Guards, Req, get, serialize_object
+from ellar.core import AppFactory, Reflector
 from ellar.core.guard import (
     APIKeyCookie,
     APIKeyHeader,
     APIKeyQuery,
     HttpBasicAuth,
     HttpBearerAuth,
     HttpDigestAuth,
 )
 from ellar.di import injectable
 from ellar.openapi import OpenAPIDocumentBuilder
-from ellar.serializer import serialize_object
-from ellar.services import Reflector
 from ellar.testing import TestClient
 
 
 class CustomException(APIException):
     pass
```

### Comparing `ellar-0.3.6/tests/test_helper/test_enum.py` & `ellar-0.3.8/tests/test_helper/test_enum.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ellar.helper.enums import create_enums_from_dict, create_enums_from_list
+from ellar.common.helper.enums import create_enums_from_dict, create_enums_from_list
 
 
 def test_create_enums_from_list():
     new_enum = create_enums_from_list("new_enum", "key1", "key2")
     assert new_enum.__name__ == "new_enum"
     assert new_enum.key1.value == "key1"
     assert new_enum.key2.value == "key2"
```

### Comparing `ellar-0.3.6/tests/test_helper/test_model_field.py` & `ellar-0.3.8/tests/test_helper/test_model_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 from pydantic.fields import ModelField
 
-from ellar.core.response.model import ResponseModelField
-from ellar.helper.modelfield import create_model_field
+from ellar.common.helper.modelfield import create_model_field
+from ellar.common.responses.models import ResponseModelField
 
 
 def test_create_model_field_works():
     response_model = create_model_field(
         name="response_model",
         type_=dict,
         model_field_class=ResponseModelField,
```

### Comparing `ellar-0.3.6/tests/test_middleware/test_functional_middleware.py` & `ellar-0.3.8/tests/test_middleware/test_functional_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from starlette.requests import Request
 from starlette.responses import PlainTextResponse
 
-from ellar.common import Module, ModuleRouter, middleware
-from ellar.core.context import IHostContext
+from ellar.common import IHostContext, Module, ModuleRouter, middleware
+from ellar.core import ModuleBase
 from ellar.testing import Test
 
 mr = ModuleRouter()
 
 
 @mr.get()
 def homepage(request: Request):
@@ -15,15 +15,15 @@
 
     if request.state.user:
         return request.state.user
     return "homepage"
 
 
 @Module(routers=[mr])
-class ModuleMiddleware:
+class ModuleMiddleware(ModuleBase):
     @middleware()
     async def middleware_modify_response(cls, context: IHostContext, call_next):
         response = context.switch_to_http_connection().get_response()
         response.headers.setdefault("modified-header", "Ellar")
         await call_next()
 
     @middleware()
```

### Comparing `ellar-0.3.6/tests/test_middleware/test_service_provider_middleware.py` & `ellar-0.3.8/tests/test_middleware/test_service_provider_middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 
 import pytest
 
-from ellar.constants import SCOPE_SERVICE_PROVIDER
+from ellar.common import IHostContextFactory
+from ellar.common.constants import SCOPE_SERVICE_PROVIDER
+from ellar.common.exceptions import HostContextException
 from ellar.core import Config
-from ellar.core.context import HostContextException, IHostContextFactory
 from ellar.core.core_service_registration import CoreServiceRegistration
 from ellar.core.middleware import RequestServiceProviderMiddleware
 from ellar.di import EllarInjector
 
 from ..injector_module import Configuration, DummyModule
```

### Comparing `ellar-0.3.6/tests/test_middleware/test_versioning_middleware.py` & `ellar-0.3.8/tests/test_middleware/test_versioning_middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import pytest
 
-from ellar.constants import SCOPE_API_VERSIONING_RESOLVER
+from ellar.common.constants import SCOPE_API_VERSIONING_RESOLVER
 from ellar.core import Config
 from ellar.core.middleware import RequestVersioningMiddleware
 from ellar.core.versioning import (
     DefaultAPIVersioning,
     HeaderAPIVersioning,
     HostNameAPIVersioning,
     QueryParameterAPIVersioning,
```

### Comparing `ellar-0.3.6/tests/test_modules/sample.py` & `ellar-0.3.8/tests/test_modules/sample.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_modules/test_module_config.py` & `ellar-0.3.8/tests/test_modules/test_module_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from abc import ABC
 from unittest.mock import patch
 
 import pytest
 
-from ellar.common import Controller, Module, ModuleRouter, get
-from ellar.constants import MODULE_METADATA
-from ellar.core import (
-    App,
-    Config,
+from ellar.common import (
+    Controller,
     ControllerBase,
-    DynamicModule,
     IModuleSetup,
-    ModuleBase,
-    ModuleSetup,
+    Module,
+    ModuleRouter,
+    get,
 )
+from ellar.common.constants import MODULE_METADATA
+from ellar.core import App, Config, DynamicModule, ModuleBase, ModuleSetup
+from ellar.core.services import Reflector
 from ellar.di import EllarInjector, ProviderConfig
 from ellar.reflect import reflect
-from ellar.services import Reflector
 from ellar.testing import Test
 
 from ..main import router
 
 
 class IDynamic(ABC):
     a: int
```

### Comparing `ellar-0.3.6/tests/test_modules/test_module_ref.py` & `ellar-0.3.8/tests/test_modules/test_module_ref.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 from ellar.common import (
     Module,
     exception_handler,
     middleware,
     template_filter,
     template_global,
 )
-from ellar.constants import (
+from ellar.common.constants import (
     EXCEPTION_HANDLERS_KEY,
     MIDDLEWARE_HANDLERS_KEY,
     MODULE_METADATA,
     TEMPLATE_FILTER_KEY,
     TEMPLATE_GLOBAL_KEY,
 )
+from ellar.common.helper import get_name
 from ellar.core import AppFactory, Config, ModuleBase
 from ellar.core.modules.ref import (
     InvalidModuleTypeException,
     ModulePlainRef,
     ModuleProvider,
     ModuleTemplateRef,
     create_module_ref_factor,
 )
 from ellar.di import EllarInjector, TransientScope, injectable
-from ellar.helper import get_name
 from ellar.reflect import reflect
 
 from .sample import AnotherUserService, ModuleBaseExample, SampleController, UserService
 
 
 @injectable(scope=TransientScope)
 @Module()
@@ -201,18 +201,22 @@
     with reflect.context():
         reflect.define_metadata(
             MODULE_METADATA.CONTROLLERS, [some_invalid_controller], ModuleBaseExample
         )
         config = Config()
         container = EllarInjector(auto_bind=False).container
 
-        with pytest.raises(AssertionError, match="Invalid Controller Type."):
+        with pytest.raises(Exception) as ex:
             create_module_ref_factor(
                 ModuleBaseExample, config=config, container=container
             )
+        assert (
+            str(ex.value)
+            == "Router Factory Builder was not found.\nUse `ControllerRouterBuilderFactory` as an example create a FactoryBuilder for this type: <class 'type'>"
+        )
 
 
 def test_invalid_module_template_ref():
     config = Config()
     container = EllarInjector(auto_bind=False).container
 
     invalid_module = type("InvalidModule", (), {})
```

### Comparing `ellar-0.3.6/tests/test_openapi/test_builder.py` & `ellar-0.3.8/tests/test_openapi/test_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from ellar.common import Controller, get, put
+from ellar.common import Controller, get, put, serialize_object
 from ellar.core import AppFactory
 from ellar.openapi.builder import OpenAPIDocumentBuilder
-from ellar.serializer import serialize_object
 
 
 @Controller
 class CatController:
     @get("/create")
     async def create_cat(self):
         return dict(message="created")
```

### Comparing `ellar-0.3.6/tests/test_openapi/test_module.py` & `ellar-0.3.8/tests/test_openapi/test_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 
 import pytest
 
-from ellar.core import AppFactory, Config, ExecutionContext, GuardCanActivate
+from ellar.common import GuardCanActivate
+from ellar.core import AppFactory, Config, ExecutionContext
 from ellar.core.modules.ref import create_module_ref_factor
 from ellar.di import EllarInjector
 from ellar.openapi import (
     OpenAPIDocumentBuilder,
     OpenAPIDocumentModule,
     ReDocDocumentGenerator,
     SwaggerDocumentGenerator,
```

### Comparing `ellar-0.3.6/tests/test_openapi/test_open_api_route_documentation.py` & `ellar-0.3.8/tests/test_openapi/test_open_api_route_documentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import typing as t
 
 from pydantic.schema import get_flat_models_from_fields, get_model_name_map
 
 from ellar.common import Body, ModuleRouter, Query, openapi_info
-from ellar.constants import CONTROLLER_OPERATION_HANDLER_KEY, OPENAPI_KEY
+from ellar.common.constants import CONTROLLER_OPERATION_HANDLER_KEY, OPENAPI_KEY
+from ellar.common.responses.models import ResponseModel, ResponseModelField
 from ellar.core.connection import HTTPConnection
 from ellar.core.guard import APIKeyCookie
-from ellar.core.response.model import ResponseModel, ResponseModelField
 from ellar.openapi import OpenAPIRouteDocumentation
 from ellar.reflect import reflect
 
 from ..schema import BlogObjectDTO, CreateCarSchema, Filter, NoteSchemaDC
 
 
 class CustomCookieAPIKey(APIKeyCookie):
```

### Comparing `ellar-0.3.6/tests/test_reflect.py` & `ellar-0.3.8/tests/test_reflect.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pytest
 
-from ellar.constants import REFLECT_TYPE
-from ellar.reflect import reflect
+from ellar.reflect import REFLECT_TYPE, reflect
 
 
 def test_define_metadata_creates_attribute_dict(random_type):
     key = "FrameworkName"
     reflect.define_metadata(key, "Ellar", random_type)
     assert hasattr(random_type, REFLECT_TYPE)
     assert reflect.get_metadata(key, random_type) == "Ellar"
```

### Comparing `ellar-0.3.6/tests/test_reflector.py` & `ellar-0.3.8/tests/test_reflector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from ellar.core.services import Reflector
 from ellar.reflect import reflect
-from ellar.services.reflector import Reflector
 
 reflector = Reflector()
 
 
 class SampleTarget:
     pass
```

### Comparing `ellar-0.3.6/tests/test_response/test_defined_response_model.py` & `ellar-0.3.8/tests/test_response/test_defined_response_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional
 
 import pytest
 from pydantic import BaseModel
 
+from ellar.common import ModuleRouter
+from ellar.common.responses.models import RouteResponseExecution
 from ellar.core import AppFactory
-from ellar.core.response.model import RouteResponseExecution
-from ellar.core.routing import ModuleRouter
 
 mr = ModuleRouter("")
 
 
 class Item(BaseModel):
     name: str
     price: Optional[float] = None
```

### Comparing `ellar-0.3.6/tests/test_response/test_pydantic_response_model.py` & `ellar-0.3.8/tests/test_response/test_pydantic_response_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Dict, List, Optional
 
 from pydantic import BaseModel, Field
 
-from ellar.common import serializer_filter
+from ellar.common import ModuleRouter, serializer_filter
 from ellar.core import AppFactory
-from ellar.core.routing import ModuleRouter
 
 mr = ModuleRouter("")
 
 
 class Item(BaseModel):
     name: str = Field(..., alias="aliased_name")
     price: Optional[float] = None
```

### Comparing `ellar-0.3.6/tests/test_response/test_response_file.py` & `ellar-0.3.8/tests/test_response/test_response_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from pathlib import Path
 
 import pytest
 
-from ellar.common import Controller, file, get
-from ellar.core.response.model import FileResponseModel
-from ellar.core.routing import ModuleRouter
+from ellar.common import Controller, ModuleRouter, file, get, serialize_object
+from ellar.common.responses.models import FileResponseModel
 from ellar.openapi import OpenAPIDocumentBuilder
-from ellar.serializer import serialize_object
 from ellar.testing import Test
 
 BASEDIR = Path(__file__).resolve().parent.parent
 FILE_RESPONSE_SCHEMA = {
     "200": {
         "description": "Successful Response",
         "content": {"text/css": {"schema": {"type": "string"}}},
```

### Comparing `ellar-0.3.6/tests/test_response/test_response_html.py` & `ellar-0.3.8/tests/test_response/test_response_html.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import re
 from pathlib import Path
 
 import pytest
 from jinja2 import TemplateNotFound
 
-from ellar.common import Controller, get, render
-from ellar.constants import CONTROLLER_OPERATION_HANDLER_KEY
-from ellar.core.response.model import HTMLResponseModel
-from ellar.core.response.model.html import HTMLResponseModelRuntimeError
-from ellar.core.routing import ModuleRouter
+from ellar.common import Controller, ModuleRouter, get, render
+from ellar.common.constants import CONTROLLER_OPERATION_HANDLER_KEY
+from ellar.common.responses.models import HTMLResponseModel
+from ellar.common.responses.models.html import HTMLResponseModelRuntimeError
 from ellar.reflect import reflect
 from ellar.testing import Test
 
 BASEDIR = Path(__file__).resolve().parent.parent
 
 
 @Controller
```

### Comparing `ellar-0.3.6/tests/test_response/test_response_streaming.py` & `ellar-0.3.8/tests/test_response/test_response_streaming.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import asyncio
 from pathlib import Path
 
 import pytest
 
-from ellar.common import Controller, file, get
-from ellar.core.response.model import (
+from ellar.common import Controller, ModuleRouter, file, get, serialize_object
+from ellar.common.responses.models import (
     StreamingResponseModel,
     StreamingResponseModelInvalidContent,
 )
-from ellar.core.routing import ModuleRouter
 from ellar.openapi import OpenAPIDocumentBuilder
-from ellar.serializer import serialize_object
 from ellar.testing import Test
 
 BASEDIR = Path(__file__).resolve().parent.parent
 FILE_RESPONSE_SCHEMA = {
     "200": {
         "description": "Successful Response",
         "content": {"text/html": {"schema": {"type": "string"}}},
```

### Comparing `ellar-0.3.6/tests/test_response/test_response_type_definition_converter.py` & `ellar-0.3.8/tests/test_response/test_response_type_definition_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Dict, List, Union, cast
 
 import pytest
 from pydantic.typing import get_args
 
-from ellar.core.exceptions import RequestValidationError
-from ellar.core.response.model import (
+from ellar.common.exceptions import RequestValidationError
+from ellar.common.helper.modelfield import create_model_field
+from ellar.common.responses.models import (
     ResponseModelField,
     ResponseTypeDefinitionConverter,
 )
-from ellar.helper.modelfield import create_model_field
-from ellar.serializer import BaseSerializer
+from ellar.common.serializer import BaseSerializer
 
 from ..schema import BlogObjectDTO, NoteSchemaDC
 
 
 def test_response_type_definition_converter():
     defined_type = List[Union[NoteSchemaDC, BlogObjectDTO]]
     converter = ResponseTypeDefinitionConverter(defined_type)
```

### Comparing `ellar-0.3.6/tests/test_response/test_route_response_model.py` & `ellar-0.3.8/tests/test_response/test_route_response_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import List, Union
 
 import pytest
 from starlette.responses import JSONResponse
 
-from ellar.constants import RESPONSE_OVERRIDE_KEY
-from ellar.core.exceptions import ImproperConfiguration
-from ellar.core.response.model import (
+from ellar.common.constants import RESPONSE_OVERRIDE_KEY
+from ellar.common.exceptions import ImproperConfiguration
+from ellar.common.responses.models import (
     EmptyAPIResponseModel,
     JSONResponseModel,
     ResponseModel,
     RouteResponseExecution,
     RouteResponseModel,
 )
-from ellar.core.routing import RouteOperation
+from ellar.common.routing import RouteOperation
 from ellar.reflect import reflect
 
 from ..schema import BlogObjectDTO, NoteSchemaDC
 
 
 def endpoint_sample():
     pass  # pragma: no cover
```

### Comparing `ellar-0.3.6/tests/test_routing/test_body_schema.py` & `ellar-0.3.8/tests/test_routing/test_body_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ellar.common import post
+from ellar.common.serializer import serialize_object
 from ellar.core.factory import AppFactory
 from ellar.openapi import OpenAPIDocumentBuilder
-from ellar.serializer import serialize_object
 
 from .sample import Product
 
 app = AppFactory.create_app()
 
 
 @post("/product")
```

### Comparing `ellar-0.3.6/tests/test_routing/test_body_schema_extra_properties.py` & `ellar-0.3.8/tests/test_routing/test_body_schema_extra_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict
 
 from pydantic import BaseModel
 
 from ellar.common import post
+from ellar.common.serializer import serialize_object
 from ellar.openapi import OpenAPIDocumentBuilder
-from ellar.serializer import serialize_object
 from ellar.testing import Test
 
 tm = Test.create_test_module()
 
 
 class Items_(BaseModel):
     items: Dict[str, int]
```

### Comparing `ellar-0.3.6/tests/test_routing/test_body_union_schema.py` & `ellar-0.3.8/tests/test_routing/test_body_union_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Union
 
 from ellar.common import post
+from ellar.common.serializer import serialize_object
 from ellar.openapi import OpenAPIDocumentBuilder
-from ellar.serializer import serialize_object
 from ellar.testing import Test
 
 from .sample import Item, OtherItem
 
 tm = Test.create_test_module()
```

### Comparing `ellar-0.3.6/tests/test_routing/test_cookie_schema.py` & `ellar-0.3.8/tests/test_routing/test_cookie_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import pytest
 
-from ellar.common import Cookie, get
+from ellar.common import Cookie, ModuleRouter, get, serialize_object
+from ellar.common.exceptions import ImproperConfiguration
 from ellar.core.connection import Request
-from ellar.core.exceptions import ImproperConfiguration
-from ellar.core.routing import ModuleRouter
 from ellar.openapi import OpenAPIDocumentBuilder
-from ellar.serializer import serialize_object
 from ellar.testing import Test
 
 from .sample import Data, Filter, ListOfPrimitiveSchema, NonPrimitiveSchema
 
 router = ModuleRouter("")
```

### Comparing `ellar-0.3.6/tests/test_routing/test_extra_args.py` & `ellar-0.3.8/tests/test_routing/test_extra_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from functools import wraps
 
 from starlette.responses import Response
 
-from ellar.common import Context, Query, Res, extra_args, get
+from ellar.common import Context, IExecutionContext, Query, Res, extra_args, get
+from ellar.common.params import ExtraEndpointArg
+from ellar.common.serializer import serialize_object
 from ellar.core.connection import Request
-from ellar.core.context import IExecutionContext
-from ellar.core.params import ExtraEndpointArg
 from ellar.openapi import OpenAPIDocumentBuilder
-from ellar.serializer import serialize_object
 from ellar.testing import Test
 
 from .sample import Filter
 
 tm = Test.create_test_module()
 app = tm.create_application()
```

### Comparing `ellar-0.3.6/tests/test_routing/test_form_schema.py` & `ellar-0.3.8/tests/test_routing/test_form_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import pytest
 
-from ellar.common import Form, post
+from ellar.common import Form, ModuleRouter, post, serialize_object
+from ellar.common.exceptions import ImproperConfiguration
 from ellar.core.connection import Request
-from ellar.core.exceptions import ImproperConfiguration
-from ellar.core.routing import ModuleRouter
 from ellar.openapi import OpenAPIDocumentBuilder
-from ellar.serializer import serialize_object
 from ellar.testing import Test
 
 from .sample import Filter, NonPrimitiveSchema
 
 mr = ModuleRouter("")
```

### Comparing `ellar-0.3.6/tests/test_routing/test_formparsers.py` & `ellar-0.3.8/tests/test_routing/test_formparsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import os
 import sys
 from typing import List, Union
 
 import pytest
 from starlette.formparsers import UploadFile as StarletteUploadFile
 
-from ellar.common import File, Form
-from ellar.core.datastructures import UploadFile
-from ellar.core.routing import ModuleRouter
+from ellar.common import File, Form, ModuleRouter, UploadFile
 from ellar.testing import Test
 
 router = ModuleRouter("")
 
 
 class ForceMultipartDict(dict):
     def __bool__(self):
```

### Comparing `ellar-0.3.6/tests/test_routing/test_forms.py` & `ellar-0.3.8/tests/test_routing/test_forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from ellar.common import Form
-from ellar.core.routing import ModuleRouter
+from ellar.common import Form, ModuleRouter
 from ellar.testing import Test
 
 router = ModuleRouter("")
 
 
 @router.post("/form/python-list")
 def post_form_param_list(items: list = Form(...)):
```

### Comparing `ellar-0.3.6/tests/test_routing/test_forms_from_non_typing_sequences.py` & `ellar-0.3.8/tests/test_routing/test_forms_from_non_typing_sequences.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from ellar.common import Form
+from ellar.common import Form, ModuleRouter
 from ellar.core import AppFactory
-from ellar.core.routing import ModuleRouter
 from ellar.testing import TestClient
 
 mr = ModuleRouter("")
 
 
 @mr.post("/form/python-list")
 def post_form_param_list(items: list = Form(...)):
```

### Comparing `ellar-0.3.6/tests/test_routing/test_header_schema.py` & `ellar-0.3.8/tests/test_routing/test_header_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import pytest
 
-from ellar.common import Header, get
+from ellar.common import Header, ModuleRouter, get, serialize_object
+from ellar.common.exceptions import ImproperConfiguration
 from ellar.core.connection import Request
-from ellar.core.exceptions import ImproperConfiguration
-from ellar.core.routing import ModuleRouter
 from ellar.openapi import OpenAPIDocumentBuilder
-from ellar.serializer import serialize_object
 from ellar.testing import Test
 
 from .sample import Data, Filter, NonPrimitiveSchema
 
 mr = ModuleRouter("")
```

### Comparing `ellar-0.3.6/tests/test_routing/test_invalid_path_param.py` & `ellar-0.3.8/tests/test_routing/test_invalid_path_param.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, List, Tuple
 
 import pytest
 from pydantic import BaseModel
 
-from ellar.core.routing import ModuleRouter
+from ellar.common import ModuleRouter
 
 mr = ModuleRouter("")
 
 
 def test_invalid_sequence():
     with pytest.raises(AssertionError):
```

### Comparing `ellar-0.3.6/tests/test_routing/test_invalid_sequence_param.py` & `ellar-0.3.8/tests/test_routing/test_invalid_sequence_param.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Dict, List, Optional, Tuple
 
 import pytest
 from pydantic import BaseModel
 
-from ellar.common import Header, Query
-from ellar.core.exceptions import ImproperConfiguration
-from ellar.core.routing import ModuleRouter
+from ellar.common import Header, ModuleRouter, Query
+from ellar.common.exceptions import ImproperConfiguration
 
 mr = ModuleRouter("")
 
 
 class Item(BaseModel):
     title: str
```

### Comparing `ellar-0.3.6/tests/test_routing/test_multi_body_errors.py` & `ellar-0.3.8/tests/test_routing/test_multi_body_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from decimal import Decimal
 from typing import List
 
 from pydantic import BaseModel, condecimal
 
-from ellar.common import post
+from ellar.common import post, serialize_object
 from ellar.openapi import OpenAPIDocumentBuilder
-from ellar.serializer import serialize_object
 from ellar.testing import Test
 
 tm = Test.create_test_module()
 app = tm.create_application()
 
 
 class Item2(BaseModel):
```

### Comparing `ellar-0.3.6/tests/test_routing/test_multi_query_errors.py` & `ellar-0.3.8/tests/test_routing/test_multi_query_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import List
 
-from ellar.common import Query, get
+from ellar.common import Query, get, serialize_object
 from ellar.openapi import OpenAPIDocumentBuilder
-from ellar.serializer import serialize_object
 from ellar.testing import Test
 
 tm = Test.create_test_module()
 app = tm.create_application()
 
 
 @get("/items/")
```

### Comparing `ellar-0.3.6/tests/test_routing/test_path.py` & `ellar-0.3.8/tests/test_routing/test_path.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_routing/test_path_with_schema.py` & `ellar-0.3.8/tests/test_routing/test_path_with_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import pytest
 
-from ellar.common import Path, get
+from ellar.common import ModuleRouter, Path, get, serialize_object
+from ellar.common.exceptions import ImproperConfiguration
 from ellar.core.connection import Request
-from ellar.core.exceptions import ImproperConfiguration
-from ellar.core.routing import ModuleRouter
 from ellar.openapi import OpenAPIDocumentBuilder
-from ellar.serializer import serialize_object
 from ellar.testing import Test
 
 from .sample import Filter, ListOfPrimitiveSchema, NonPrimitiveSchema
 
 mr = ModuleRouter("")
```

### Comparing `ellar-0.3.6/tests/test_routing/test_put_with_no_body_schema.py` & `ellar-0.3.8/tests/test_routing/test_put_with_no_body_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from ellar.common import put
+from ellar.common import put, serialize_object
 from ellar.openapi import OpenAPIDocumentBuilder
-from ellar.serializer import serialize_object
 from ellar.testing import Test
 
 tm = Test.create_test_module()
 app = tm.create_application()
 
 
 @put("/items/{item_id}")
```

### Comparing `ellar-0.3.6/tests/test_routing/test_query.py` & `ellar-0.3.8/tests/test_routing/test_query.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_routing/test_query_schema.py` & `ellar-0.3.8/tests/test_routing/test_query_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import pytest
 
-from ellar.common import Query, get
+from ellar.common import ModuleRouter, Query, get, serialize_object
+from ellar.common.exceptions import ImproperConfiguration
 from ellar.core.connection import Request
-from ellar.core.exceptions import ImproperConfiguration
-from ellar.core.routing import ModuleRouter
 from ellar.openapi import OpenAPIDocumentBuilder
-from ellar.serializer import serialize_object
 from ellar.testing import Test
 
 from .sample import Data, Filter, NonPrimitiveSchema
 
 mr = ModuleRouter("")
```

### Comparing `ellar-0.3.6/tests/test_routing/test_request.py` & `ellar-0.3.8/tests/test_routing/test_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pytest
 
-from ellar.common import Cookie, Header
+from ellar.common import Cookie, Header, ModuleRouter
 from ellar.core.connection import Request
-from ellar.core.routing import ModuleRouter
 from ellar.testing import Test
 
 mr = ModuleRouter("")
 
 
 @mr.get("/headers1")
 def headers1(request: Request, user_agent: str = Header(...)):
```

### Comparing `ellar-0.3.6/tests/test_routing/test_route_endpoint_params.py` & `ellar-0.3.8/tests/test_routing/test_route_endpoint_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 from starlette.requests import (
     HTTPConnection as StarletteHTTPConnection,
     Request as StarletteRequest,
 )
 from starlette.responses import Response as StarletteResponse
 from starlette.websockets import WebSocket as StarletteWebSocket
 
-from ellar.common import Context, Host, Http, Provide, Req, Res, Session, Ws
+from ellar.common import (
+    Context,
+    Host,
+    Http,
+    IExecutionContext,
+    ModuleRouter,
+    Provide,
+    Req,
+    Res,
+    Session,
+    Ws,
+)
 from ellar.core import Config, ExecutionContext
 from ellar.core.connection import (
     HTTPConnection as EllarHTTPConnection,
     Request as EllarRequest,
     WebSocket as EllarWebSocket,
 )
-from ellar.core.context import IExecutionContext
 from ellar.core.middleware import Middleware
 from ellar.core.middleware.sessions import SessionMiddleware
-from ellar.core.routing import ModuleRouter
 from ellar.testing import Test
 
 router = ModuleRouter()
 
 
 @router.get("/starlette-request")
 def get_requests(request: StarletteRequest, req=Req()):
```

### Comparing `ellar-0.3.6/tests/test_schema.py` & `ellar-0.3.8/tests/test_schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 from pydantic import BaseModel
 
-from ellar.compatible import AttributeDict
-from ellar.core.response.model import EmptyAPIResponseModel
-from ellar.core.routing.websocket import WebSocketExtraHandler
-from ellar.core.schema import RouteParameters, WsRouteParameters
+from ellar.common.compatible import AttributeDict
+from ellar.common.responses.models import EmptyAPIResponseModel
+from ellar.common.routing.schema import RouteParameters, WsRouteParameters
+from ellar.common.routing.websocket import WebSocketExtraHandler
 
 
 class Item(BaseModel):
     name: str
 
 
 class SampleResponseModel(EmptyAPIResponseModel):
```

### Comparing `ellar-0.3.6/tests/test_serializer.py` & `ellar-0.3.8/tests/test_serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datetime import datetime, timezone
 from enum import Enum
 from pathlib import PureWindowsPath
 
 import pytest
 from pydantic import BaseModel, Field, dataclasses as pydantic_dataclasses
 
-from ellar.serializer import (
+from ellar.common.serializer import (
     DataclassSerializer,
     Serializer,
     SerializerFilter,
     convert_dataclass_to_pydantic_model,
     get_dataclass_pydantic_model,
     serialize_object,
 )
```

### Comparing `ellar-0.3.6/tests/test_shortcuts.py` & `ellar-0.3.8/tests/test_shortcuts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ellar.shortcuts import fail_silently, normalize_path
+from ellar.common.shortcuts import fail_silently, normalize_path
 
 
 def test_fail_silently():
     def call_with_args_kwargs(*args, **kwargs):
         return args, kwargs
 
     def raise_exception():
```

### Comparing `ellar-0.3.6/tests/test_staticfiles.py` & `ellar-0.3.8/tests/test_staticfiles.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_templating/test_module_templating.py` & `ellar-0.3.8/tests/test_templating/test_module_templating.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def double_global_dec_2(cls, n):
         return n * 2
 
 
 @Module(
     static_folder="module_statics",
 )
-class SomeModule2:
+class SomeModule2(ModuleBase):
     @template_filter()
     def double_filter(cls, n):
         return n * 2
 
     @template_global()
     def double_global(cls, n):
         return n * 2
```

### Comparing `ellar-0.3.6/tests/test_templating/test_renderer.py` & `ellar-0.3.8/tests/test_templating/test_renderer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import re
 from pathlib import Path
 
-from ellar.common import Controller, get, render
-from ellar.core import ControllerBase
-from ellar.core.templating import (
+from ellar.common import (
+    Controller,
+    ControllerBase,
     TemplateResponse,
+    get,
+    render,
     render_template,
     render_template_string,
 )
 from ellar.testing import Test
 
 BASEDIR = Path(__file__).resolve().parent.parent
```

### Comparing `ellar-0.3.6/tests/test_testing.py` & `ellar-0.3.8/tests/test_testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import abstractmethod
 
 from starlette.routing import Host, Mount
 
-from ellar.constants import MODULE_METADATA
+from ellar.common.constants import MODULE_METADATA
 from ellar.di import ProviderConfig
 from ellar.reflect import reflect
 from ellar.testing import Test
 
 from .test_application.sample import (
     ApplicationModule,
     ClassBaseController,
```

### Comparing `ellar-0.3.6/tests/test_versioning/operations.py` & `ellar-0.3.8/tests/test_versioning/operations.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_versioning/test_default_versioning.py` & `ellar-0.3.8/tests/test_versioning/test_default_versioning.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_versioning/test_default_versioning_for_controllers.py` & `ellar-0.3.8/tests/test_versioning/test_default_versioning_for_controllers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_versioning/test_header_versioning.py` & `ellar-0.3.8/tests/test_versioning/test_header_versioning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from ellar.constants import NOT_SET
+from ellar.common.constants import NOT_SET
 from ellar.core.versioning import VersioningSchemes as VERSIONING
 from ellar.testing import Test
 
 from .operations import mr
 
 tm = Test.create_test_module(routers=(mr,))
 app = tm.create_application()
```

### Comparing `ellar-0.3.6/tests/test_versioning/test_header_versioning_controller.py` & `ellar-0.3.8/tests/test_versioning/test_header_versioning_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from ellar.constants import NOT_SET
+from ellar.common.constants import NOT_SET
 from ellar.core.versioning import VersioningSchemes as VERSIONING
 from ellar.testing import Test
 
 from .operations import (
     ControllerIndividualVersioning,
     ControllerListVersioning,
     ControllerVersioning,
```

### Comparing `ellar-0.3.6/tests/test_versioning/test_host_versioning.py` & `ellar-0.3.8/tests/test_versioning/test_host_versioning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from ellar.constants import NOT_SET
+from ellar.common.constants import NOT_SET
 from ellar.core.versioning import VersioningSchemes as VERSIONING
 from ellar.testing import Test
 
 from .operations import mr
 
 tm = Test.create_test_module(routers=(mr,))
 app = tm.create_application()
```

### Comparing `ellar-0.3.6/tests/test_versioning/test_query_versioning.py` & `ellar-0.3.8/tests/test_versioning/test_query_versioning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from ellar.constants import NOT_SET
+from ellar.common.constants import NOT_SET
 from ellar.core.versioning import VersioningSchemes as VERSIONING
 from ellar.testing import Test
 
 from .operations import mr
 
 tm = Test.create_test_module(routers=(mr,))
 app = tm.create_application()
```

### Comparing `ellar-0.3.6/tests/test_versioning/test_url_versioning.py` & `ellar-0.3.8/tests/test_versioning/test_url_versioning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from ellar.constants import NOT_SET
+from ellar.common.constants import NOT_SET
 from ellar.core.versioning import UrlPathAPIVersioning, VersioningSchemes as VERSIONING
 from ellar.testing import Test
 
 from .operations import mr
 
 tm = Test.create_test_module(routers=(mr,))
 app = tm.create_application()
```

### Comparing `ellar-0.3.6/tests/test_websocket.py` & `ellar-0.3.8/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.6/tests/test_websocket_handler.py` & `ellar-0.3.8/tests/test_websocket_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 from starlette.websockets import WebSocket, WebSocketState
 
 from ellar.common import Controller, ModuleRouter, WsBody, ws_route
-from ellar.constants import CONTROLLER_OPERATION_HANDLER_KEY
-from ellar.core.exceptions import ImproperConfiguration
+from ellar.common.constants import CONTROLLER_OPERATION_HANDLER_KEY
+from ellar.common.exceptions import ImproperConfiguration
 from ellar.reflect import reflect
 from ellar.testing import Test
 
 from .schema import Item
 
 router = ModuleRouter("/router")
```

### Comparing `ellar-0.3.6/PKG-INFO` & `ellar-0.3.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 656c 6c61  : 2.1.Name: ella
-00000020: 720a 5665 7273 696f 6e3a 2030 2e33 2e36  r.Version: 0.3.6
+00000020: 720a 5665 7273 696f 6e3a 2030 2e33 2e38  r.Version: 0.3.8
 00000030: 0a53 756d 6d61 7279 3a20 456c 6c61 7220  .Summary: Ellar 
 00000040: 2d20 5079 7468 6f6e 2041 5347 4920 7765  - Python ASGI we
 00000050: 6220 6672 616d 6577 6f72 6b20 666f 7220  b framework for 
 00000060: 6275 696c 6469 6e67 2066 6173 742c 2065  building fast, e
 00000070: 6666 6963 6965 6e74 2061 6e64 2073 6361  fficient and sca
 00000080: 6c61 626c 6520 5245 5354 4150 4973 2061  lable RESTAPIs a
 00000090: 6e64 2073 6572 7665 722d 7369 6465 2061  nd server-side a
@@ -119,812 +119,809 @@
 00000760: 302e 3020 3b20 6578 7472 6120 3d3d 2022  0.0 ; extra == "
 00000770: 616c 6c22 0a52 6571 7569 7265 732d 4469  all".Requires-Di
 00000780: 7374 3a20 6f72 6a73 6f6e 203e 3d33 2e32  st: orjson >=3.2
 00000790: 2e31 2c3c 342e 302e 3020 3b20 6578 7472  .1,<4.0.0 ; extr
 000007a0: 6120 3d3d 2022 616c 6c22 0a52 6571 7569  a == "all".Requi
 000007b0: 7265 732d 4469 7374 3a20 656d 6169 6c5f  res-Dist: email_
 000007c0: 7661 6c69 6461 746f 7220 3e3d 312e 312e  validator >=1.1.
-000007d0: 312c 3c32 2e30 2e30 203b 2065 7874 7261  1,<2.0.0 ; extra
+000007d0: 312c 3c33 2e30 2e30 203b 2065 7874 7261  1,<3.0.0 ; extra
 000007e0: 203d 3d20 2261 6c6c 220a 5265 7175 6972   == "all".Requir
 000007f0: 6573 2d44 6973 743a 2070 7265 2d63 6f6d  es-Dist: pre-com
 00000800: 6d69 7420 3b20 6578 7472 6120 3d3d 2022  mit ; extra == "
 00000810: 6465 7622 0a52 6571 7569 7265 732d 4469  dev".Requires-Di
 00000820: 7374 3a20 6d6b 646f 6373 203e 3d31 2e31  st: mkdocs >=1.1
 00000830: 2e32 2c3c 322e 302e 3020 3b20 6578 7472  .2,<2.0.0 ; extr
 00000840: 6120 3d3d 2022 646f 6322 0a52 6571 7569  a == "doc".Requi
 00000850: 7265 732d 4469 7374 3a20 6d6b 646f 6373  res-Dist: mkdocs
 00000860: 2d6d 6174 6572 6961 6c20 3e3d 372e 312e  -material >=7.1.
-00000870: 392c 3c39 2e30 2e30 203b 2065 7874 7261  9,<9.0.0 ; extra
-00000880: 203d 3d20 2264 6f63 220a 5265 7175 6972   == "doc".Requir
-00000890: 6573 2d44 6973 743a 206d 6478 2d69 6e63  es-Dist: mdx-inc
-000008a0: 6c75 6465 203e 3d31 2e34 2e31 2c3c 322e  lude >=1.4.1,<2.
-000008b0: 302e 3020 3b20 6578 7472 6120 3d3d 2022  0.0 ; extra == "
-000008c0: 646f 6322 0a52 6571 7569 7265 732d 4469  doc".Requires-Di
-000008d0: 7374 3a20 6d6b 646f 6373 2d6d 6172 6b64  st: mkdocs-markd
-000008e0: 6f77 6e65 7874 7261 6461 7461 2d70 6c75  ownextradata-plu
-000008f0: 6769 6e20 3e3d 302e 312e 372c 3c30 2e33  gin >=0.1.7,<0.3
-00000900: 2e30 203b 2065 7874 7261 203d 3d20 2264  .0 ; extra == "d
-00000910: 6f63 220a 5265 7175 6972 6573 2d44 6973  oc".Requires-Dis
-00000920: 743a 206d 6172 6b64 6f77 6e2d 696e 636c  t: markdown-incl
-00000930: 7564 6520 3b20 6578 7472 6120 3d3d 2022  ude ; extra == "
-00000940: 646f 6322 0a52 6571 7569 7265 732d 4469  doc".Requires-Di
-00000950: 7374 3a20 6d6b 646f 6373 7472 696e 6773  st: mkdocstrings
-00000960: 203b 2065 7874 7261 203d 3d20 2264 6f63   ; extra == "doc
-00000970: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000980: 206d 6b64 6f63 732d 6d69 6e69 6679 2d70   mkdocs-minify-p
-00000990: 6c75 6769 6e20 3b20 6578 7472 6120 3d3d  lugin ; extra ==
-000009a0: 2022 646f 6322 0a52 6571 7569 7265 732d   "doc".Requires-
-000009b0: 4469 7374 3a20 6d6b 646f 6373 2d67 6974  Dist: mkdocs-git
-000009c0: 2d72 6576 6973 696f 6e2d 6461 7465 2d6c  -revision-date-l
-000009d0: 6f63 616c 697a 6564 2d70 6c75 6769 6e20  ocalized-plugin 
-000009e0: 3b20 6578 7472 6120 3d3d 2022 646f 6322  ; extra == "doc"
-000009f0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000a00: 7079 7465 7374 203e 3d36 2e32 2e34 2c3c  pytest >=6.2.4,<
-00000a10: 382e 302e 3020 3b20 6578 7472 6120 3d3d  8.0.0 ; extra ==
-00000a20: 2022 7465 7374 220a 5265 7175 6972 6573   "test".Requires
-00000a30: 2d44 6973 743a 2070 7974 6573 742d 636f  -Dist: pytest-co
-00000a40: 7620 3e3d 322e 3132 2e30 2c3c 352e 302e  v >=2.12.0,<5.0.
-00000a50: 3020 3b20 6578 7472 6120 3d3d 2022 7465  0 ; extra == "te
-00000a60: 7374 220a 5265 7175 6972 6573 2d44 6973  st".Requires-Dis
-00000a70: 743a 206d 7970 7920 3d3d 302e 3937 3120  t: mypy ==0.971 
-00000a80: 3b20 6578 7472 6120 3d3d 2022 7465 7374  ; extra == "test
-00000a90: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000aa0: 2066 6c61 6b65 3820 3e3d 332e 382e 332c   flake8 >=3.8.3,
-00000ab0: 3c37 2e30 2e30 203b 2065 7874 7261 203d  <7.0.0 ; extra =
-00000ac0: 3d20 2274 6573 7422 0a52 6571 7569 7265  = "test".Require
-00000ad0: 732d 4469 7374 3a20 626c 6163 6b20 3d3d  s-Dist: black ==
-00000ae0: 3232 2e31 322e 3020 3b20 6578 7472 6120  22.12.0 ; extra 
-00000af0: 3d3d 2022 7465 7374 220a 5265 7175 6972  == "test".Requir
-00000b00: 6573 2d44 6973 743a 2069 736f 7274 203e  es-Dist: isort >
-00000b10: 3d35 2e30 2e36 2c3c 362e 302e 3020 3b20  =5.0.6,<6.0.0 ; 
-00000b20: 6578 7472 6120 3d3d 2022 7465 7374 220a  extra == "test".
-00000b30: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
-00000b40: 7974 6573 742d 6173 796e 6369 6f20 3b20  ytest-asyncio ; 
-00000b50: 6578 7472 6120 3d3d 2022 7465 7374 220a  extra == "test".
-00000b60: 5265 7175 6972 6573 2d44 6973 743a 2064  Requires-Dist: d
-00000b70: 6174 6162 6173 6573 5b73 716c 6974 655d  atabases[sqlite]
-00000b80: 203e 3d20 302e 332e 3220 3b20 6578 7472   >= 0.3.2 ; extr
-00000b90: 6120 3d3d 2022 7465 7374 220a 5265 7175  a == "test".Requ
-00000ba0: 6972 6573 2d44 6973 743a 206f 726a 736f  ires-Dist: orjso
-00000bb0: 6e20 3e3d 2033 2e32 2e31 203b 2065 7874  n >= 3.2.1 ; ext
-00000bc0: 7261 203d 3d20 2274 6573 7422 0a52 6571  ra == "test".Req
-00000bd0: 7569 7265 732d 4469 7374 3a20 756a 736f  uires-Dist: ujso
-00000be0: 6e20 3e3d 2034 2e30 2e31 203b 2065 7874  n >= 4.0.1 ; ext
-00000bf0: 7261 203d 3d20 2274 6573 7422 0a52 6571  ra == "test".Req
-00000c00: 7569 7265 732d 4469 7374 3a20 7079 7468  uires-Dist: pyth
-00000c10: 6f6e 2d6d 756c 7469 7061 7274 203e 3d20  on-multipart >= 
-00000c20: 302e 302e 3520 3b20 6578 7472 6120 3d3d  0.0.5 ; extra ==
-00000c30: 2022 7465 7374 220a 5265 7175 6972 6573   "test".Requires
-00000c40: 2d44 6973 743a 2061 6e79 696f 5b74 7269  -Dist: anyio[tri
-00000c50: 6f5d 203e 3d20 332e 322e 3120 3b20 6578  o] >= 3.2.1 ; ex
-00000c60: 7472 6120 3d3d 2022 7465 7374 220a 5265  tra == "test".Re
-00000c70: 7175 6972 6573 2d44 6973 743a 2061 7574  quires-Dist: aut
-00000c80: 6f66 6c61 6b65 203b 2065 7874 7261 203d  oflake ; extra =
-00000c90: 3d20 2274 6573 7422 0a52 6571 7569 7265  = "test".Require
-00000ca0: 732d 4469 7374 3a20 656d 6169 6c5f 7661  s-Dist: email_va
-00000cb0: 6c69 6461 746f 7220 3e3d 312e 312e 3120  lidator >=1.1.1 
-00000cc0: 3b20 6578 7472 6120 3d3d 2022 7465 7374  ; extra == "test
-00000cd0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000ce0: 2070 796c 6962 6d63 203b 2065 7874 7261   pylibmc ; extra
-00000cf0: 203d 3d20 2274 6573 7422 0a52 6571 7569   == "test".Requi
-00000d00: 7265 732d 4469 7374 3a20 7079 6d65 6d63  res-Dist: pymemc
-00000d10: 6163 6865 203b 2065 7874 7261 203d 3d20  ache ; extra == 
-00000d20: 2274 6573 7422 0a52 6571 7569 7265 732d  "test".Requires-
-00000d30: 4469 7374 3a20 6169 6f6d 6361 6368 6520  Dist: aiomcache 
-00000d40: 3b20 6578 7472 6120 3d3d 2022 7465 7374  ; extra == "test
-00000d50: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000d60: 2072 6564 6973 203b 2065 7874 7261 203d   redis ; extra =
-00000d70: 3d20 2274 6573 7422 0a52 6571 7569 7265  = "test".Require
-00000d80: 732d 4469 7374 3a20 7479 7065 732d 756a  s-Dist: types-uj
-00000d90: 736f 6e20 3d3d 352e 372e 302e 3120 3b20  son ==5.7.0.1 ; 
-00000da0: 6578 7472 6120 3d3d 2022 7465 7374 220a  extra == "test".
-00000db0: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
-00000dc0: 7970 6573 2d6f 726a 736f 6e20 3d3d 332e  ypes-orjson ==3.
-00000dd0: 362e 3220 3b20 6578 7472 6120 3d3d 2022  6.2 ; extra == "
-00000de0: 7465 7374 220a 5265 7175 6972 6573 2d44  test".Requires-D
-00000df0: 6973 743a 2074 7970 6573 2d64 6174 6163  ist: types-datac
-00000e00: 6c61 7373 6573 203d 3d30 2e36 2e36 203b  lasses ==0.6.6 ;
-00000e10: 2065 7874 7261 203d 3d20 2274 6573 7422   extra == "test"
-00000e20: 0a50 726f 6a65 6374 2d55 524c 3a20 446f  .Project-URL: Do
-00000e30: 6375 6d65 6e74 6174 696f 6e2c 2068 7474  cumentation, htt
-00000e40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000e50: 6561 6477 696e 436f 6465 2f65 6c6c 6172  eadwinCode/ellar
-00000e60: 0a50 726f 6a65 6374 2d55 524c 3a20 486f  .Project-URL: Ho
-00000e70: 6d65 7061 6765 2c20 6874 7470 733a 2f2f  mepage, https://
-00000e80: 6561 6477 696e 636f 6465 2e67 6974 6875  eadwincode.githu
-00000e90: 622e 696f 2f65 6c6c 6172 2f0a 5072 6f6a  b.io/ellar/.Proj
-00000ea0: 6563 742d 5552 4c3a 2053 6f75 7263 652c  ect-URL: Source,
-00000eb0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000ec0: 636f 6d2f 6561 6477 696e 436f 6465 2f65  com/eadwinCode/e
-00000ed0: 6c6c 6172 0a50 726f 7669 6465 732d 4578  llar.Provides-Ex
-00000ee0: 7472 613a 2061 6c6c 0a50 726f 7669 6465  tra: all.Provide
-00000ef0: 732d 4578 7472 613a 2064 6576 0a50 726f  s-Extra: dev.Pro
-00000f00: 7669 6465 732d 4578 7472 613a 2064 6f63  vides-Extra: doc
-00000f10: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000f20: 2074 6573 740a 0a3c 7020 616c 6967 6e3d   test..<p align=
-00000f30: 2263 656e 7465 7222 3e0a 2020 3c61 2068  "center">.  <a h
-00000f40: 7265 663d 2223 2220 7461 7267 6574 3d22  ref="#" target="
-00000f50: 626c 616e 6b22 3e3c 696d 6720 7372 633d  blank"><img src=
-00000f60: 2264 6f63 732f 696d 672f 456c 6c61 724c  "docs/img/EllarL
-00000f70: 6f67 6f49 636f 6e4f 6e6c 792e 706e 6722  ogoIconOnly.png"
-00000f80: 2077 6964 7468 3d22 3230 3022 2061 6c74   width="200" alt
-00000f90: 3d22 456c 6c61 7220 4c6f 676f 2220 2f3e  ="Ellar Logo" />
-00000fa0: 3c2f 613e 0a3c 2f70 3e0a 0a3c 7020 616c  </a>.</p>..<p al
-00000fb0: 6967 6e3d 2263 656e 7465 7222 3e20 456c  ign="center"> El
-00000fc0: 6c61 7220 2d20 5079 7468 6f6e 2041 5347  lar - Python ASG
-00000fd0: 4920 7765 6220 6672 616d 6577 6f72 6b20  I web framework 
-00000fe0: 666f 7220 6275 696c 6469 6e67 2066 6173  for building fas
-00000ff0: 742c 2065 6666 6963 6965 6e74 2061 6e64  t, efficient and
-00001000: 2073 6361 6c61 626c 6520 5245 5354 4150   scalable RESTAP
-00001010: 4973 2061 6e64 2073 6572 7665 722d 7369  Is and server-si
-00001020: 6465 2061 7070 6c69 6361 7469 6f6e 2e20  de application. 
-00001030: 3c2f 703e 0a0a 215b 5465 7374 5d28 6874  </p>..![Test](ht
-00001040: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001050: 2f65 6164 7769 6e43 6f64 652f 656c 6c61  /eadwinCode/ella
-00001060: 722f 6163 7469 6f6e 732f 776f 726b 666c  r/actions/workfl
-00001070: 6f77 732f 7465 7374 5f66 756c 6c2e 796d  ows/test_full.ym
-00001080: 6c2f 6261 6467 652e 7376 6729 0a21 5b43  l/badge.svg).![C
-00001090: 6f76 6572 6167 655d 2868 7474 7073 3a2f  overage](https:/
-000010a0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000010b0: 636f 6465 636f 762f 632f 6769 7468 7562  codecov/c/github
-000010c0: 2f65 6164 7769 6e43 6f64 652f 656c 6c61  /eadwinCode/ella
-000010d0: 7229 0a5b 215b 5079 5049 2076 6572 7369  r).[![PyPI versi
-000010e0: 6f6e 5d28 6874 7470 733a 2f2f 6261 6467  on](https://badg
-000010f0: 652e 6675 7279 2e69 6f2f 7079 2f65 6c6c  e.fury.io/py/ell
-00001100: 6172 2e73 7667 295d 2868 7474 7073 3a2f  ar.svg)](https:/
-00001110: 2f62 6164 6765 2e66 7572 792e 696f 2f70  /badge.fury.io/p
-00001120: 792f 656c 6c61 7229 0a5b 215b 5079 5049  y/ellar).[![PyPI
-00001130: 2076 6572 7369 6f6e 5d28 6874 7470 733a   version](https:
-00001140: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00001150: 2f70 7970 692f 762f 656c 6c61 722e 7376  /pypi/v/ellar.sv
-00001160: 6729 5d28 6874 7470 733a 2f2f 7079 7069  g)](https://pypi
-00001170: 2e70 7974 686f 6e2e 6f72 672f 7079 7069  .python.org/pypi
-00001180: 2f65 6c6c 6172 290a 5b21 5b50 7950 4920  /ellar).[![PyPI 
-00001190: 7665 7273 696f 6e5d 2868 7474 7073 3a2f  version](https:/
-000011a0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000011b0: 7079 7069 2f70 7976 6572 7369 6f6e 732f  pypi/pyversions/
-000011c0: 656c 6c61 722e 7376 6729 5d28 6874 7470  ellar.svg)](http
-000011d0: 733a 2f2f 7079 7069 2e70 7974 686f 6e2e  s://pypi.python.
-000011e0: 6f72 672f 7079 7069 2f65 6c6c 6172 290a  org/pypi/ellar).
-000011f0: 0a23 2320 496e 7472 6f64 7563 7469 6f6e  .## Introduction
-00001200: 0a0a 456c 6c61 7220 6973 2061 206c 6967  ..Ellar is a lig
-00001210: 6874 7765 6967 6874 2041 5347 4920 6672  htweight ASGI fr
-00001220: 616d 6577 6f72 6b20 666f 7220 6275 696c  amework for buil
-00001230: 6469 6e67 2065 6666 6963 6965 6e74 2061  ding efficient a
-00001240: 6e64 2073 6361 6c61 626c 6520 7365 7276  nd scalable serv
-00001250: 6572 2d73 6964 6520 7079 7468 6f6e 2061  er-side python a
-00001260: 7070 6c69 6361 7469 6f6e 732e 0a49 7420  pplications..It 
-00001270: 7375 7070 6f72 7473 2062 6f74 6820 4f4f  supports both OO
-00001280: 5020 284f 626a 6563 742d 4f72 6965 6e74  P (Object-Orient
-00001290: 6564 2050 726f 6772 616d 6d69 6e67 2920  ed Programming) 
-000012a0: 616e 6420 4650 2028 4675 6e63 7469 6f6e  and FP (Function
-000012b0: 616c 2050 726f 6772 616d 6d69 6e67 290a  al Programming).
-000012c0: 0a45 6c6c 6172 2069 7320 6261 7365 6420  .Ellar is based 
-000012d0: 6f6e 205b 5374 6172 6c65 7474 6520 2841  on [Starlette (A
-000012e0: 5347 4920 746f 6f6c 6b69 7429 5d28 6874  SGI toolkit)](ht
-000012f0: 7470 733a 2f2f 7777 772e 7374 6172 6c65  tps://www.starle
-00001300: 7474 652e 696f 2f29 2c20 6120 6c69 6768  tte.io/), a ligh
-00001310: 7477 6569 6768 7420 4153 4749 2066 7261  tweight ASGI fra
-00001320: 6d65 776f 726b 2f74 6f6f 6c6b 6974 2077  mework/toolkit w
-00001330: 656c 6c2d 7375 6974 6564 2066 6f72 2064  ell-suited for d
-00001340: 6576 656c 6f70 696e 6720 6173 796e 6368  eveloping asynch
-00001350: 726f 6e6f 7573 2077 6562 2073 6572 7669  ronous web servi
-00001360: 6365 7320 7769 7468 2050 7974 686f 6e2e  ces with Python.
-00001370: 200a 5768 696c 6520 456c 6c61 7220 7072   .While Ellar pr
-00001380: 6f76 6964 6573 2061 2068 6967 6820 6c65  ovides a high le
-00001390: 7665 6c20 6f66 2061 6273 7472 6163 7469  vel of abstracti
-000013a0: 6f6e 206f 6e20 746f 7020 6f66 2053 7461  on on top of Sta
-000013b0: 726c 6574 7465 2c20 6974 2073 7469 6c6c  rlette, it still
-000013c0: 2069 6e63 6f72 706f 7261 7465 7320 736f   incorporates so
-000013d0: 6d65 206f 6620 6974 7320 6665 6174 7572  me of its featur
-000013e0: 6573 2c20 6173 2077 656c 6c20 6173 2074  es, as well as t
-000013f0: 686f 7365 206f 6620 4661 7374 4150 492e  hose of FastAPI.
-00001400: 200a 4966 2079 6f75 2061 7265 2066 616d   .If you are fam
-00001410: 696c 6961 7220 7769 7468 2074 6865 7365  iliar with these
-00001420: 2066 7261 6d65 776f 726b 732c 2079 6f75   frameworks, you
-00001430: 2077 696c 6c20 6669 6e64 2069 7420 6561   will find it ea
-00001440: 7379 2074 6f20 756e 6465 7273 7461 6e64  sy to understand
-00001450: 2061 6e64 2075 7365 2045 6c6c 6172 2e0a   and use Ellar..
-00001460: 0a23 2320 4665 6174 7572 6573 2053 756d  .## Features Sum
-00001470: 6d61 7279 0a0a 2d20 2a2a 4561 7379 2074  mary..- **Easy t
-00001480: 6f20 5573 652a 2a3a 2045 6c6c 6172 2068  o Use**: Ellar h
-00001490: 6173 2061 2073 696d 706c 6520 616e 6420  as a simple and 
-000014a0: 696e 7475 6974 6976 6520 4150 4920 7468  intuitive API th
-000014b0: 6174 206d 616b 6573 2069 7420 6561 7379  at makes it easy
-000014c0: 2074 6f20 6765 7420 7374 6172 7465 6420   to get started 
-000014d0: 7769 7468 2062 7569 6c64 696e 6720 6120  with building a 
-000014e0: 6661 7374 2061 6e64 2073 6361 6c61 626c  fast and scalabl
-000014f0: 6520 7765 6220 6170 706c 6963 6174 696f  e web applicatio
-00001500: 6e73 206f 7220 7765 6220 4150 4973 2069  ns or web APIs i
-00001510: 6e20 5079 7468 6f6e 2e0a 2d20 2a2a 4465  n Python..- **De
-00001520: 7065 6e64 656e 6379 2049 6e6a 6563 7469  pendency Injecti
-00001530: 6f6e 2028 4449 292a 2a3a 2049 7420 636f  on (DI)**: It co
-00001540: 6d65 7320 7769 7468 2044 4920 7379 7374  mes with DI syst
-00001550: 656d 206d 616b 6573 2069 7420 6561 7379  em makes it easy
-00001560: 2074 6f20 6d61 6e61 6765 2064 6570 656e   to manage depen
-00001570: 6465 6e63 6965 7320 616e 6420 7265 6475  dencies and redu
-00001580: 6365 2063 6f75 706c 696e 6720 6265 7477  ce coupling betw
-00001590: 6565 6e20 636f 6d70 6f6e 656e 7473 2e0a  een components..
-000015a0: 2d20 2a2a 5079 6461 6e74 6963 2049 6e74  - **Pydantic Int
-000015b0: 6567 7261 7469 6f6e 2a2a 3a20 4974 2069  egration**: It i
-000015c0: 7320 7072 6f70 6572 6c79 2069 6e74 6567  s properly integ
-000015d0: 7261 7465 6420 7769 7468 2050 7964 616e  rated with Pydan
-000015e0: 7469 632c 2061 2070 6f70 756c 6172 2050  tic, a popular P
-000015f0: 7974 686f 6e20 6c69 6272 6172 7920 666f  ython library fo
-00001600: 7220 6461 7461 2076 616c 6964 6174 696f  r data validatio
-00001610: 6e2c 2074 6f20 656e 7375 7265 2074 6861  n, to ensure tha
-00001620: 7420 696e 7075 7420 6461 7461 2069 7320  t input data is 
-00001630: 7661 6c69 642e 0a2d 202a 2a54 656d 706c  valid..- **Templ
-00001640: 6174 696e 6720 7769 7468 204a 696e 6a61  ating with Jinja
-00001650: 322a 2a3a 2045 6c6c 6172 2070 726f 7669  2**: Ellar provi
-00001660: 6465 7320 6275 696c 742d 696e 2073 7570  des built-in sup
-00001670: 706f 7274 2066 6f72 204a 696e 6a61 3220  port for Jinja2 
-00001680: 7465 6d70 6c61 7465 732c 206d 616b 696e  templates, makin
-00001690: 6720 6974 2065 6173 7920 746f 2063 7265  g it easy to cre
-000016a0: 6174 6520 6479 6e61 6d69 6320 7765 6220  ate dynamic web 
-000016b0: 7061 6765 732e 0a2d 202a 2a4f 7065 6e41  pages..- **OpenA
-000016c0: 5049 2044 6f63 756d 656e 7461 7469 6f6e  PI Documentation
-000016d0: 2a2a 3a20 4974 2063 6f6d 6573 2077 6974  **: It comes wit
-000016e0: 6820 6275 696c 742d 696e 2073 7570 706f  h built-in suppo
-000016f0: 7274 2066 6f72 204f 7065 6e41 5049 2064  rt for OpenAPI d
-00001700: 6f63 756d 656e 7461 7469 6f6e 2c20 6d61  ocumentation, ma
-00001710: 6b69 6e67 2069 7420 6561 7379 2074 6f20  king it easy to 
-00001720: 6765 6e65 7261 7465 2060 5377 6167 6765  generate `Swagge
-00001730: 7260 206f 7220 6052 6544 6f63 6020 646f  r` or `ReDoc` do
-00001740: 6375 6d65 6e74 6174 696f 6e20 666f 7220  cumentation for 
-00001750: 796f 7572 2041 5049 2e20 416e 6420 6d6f  your API. And mo
-00001760: 7265 2063 616e 2062 6520 6164 6465 6420  re can be added 
-00001770: 7769 7468 2065 6173 6520 6966 206e 6563  with ease if nec
-00001780: 6573 7361 7279 2e0a 2d20 2a2a 436f 6e74  essary..- **Cont
-00001790: 726f 6c6c 6572 2028 4d56 4329 2041 7263  roller (MVC) Arc
-000017a0: 6869 7465 6374 7572 652a 2a3a 2045 6c6c  hitecture**: Ell
-000017b0: 6172 2773 2063 6f6e 7472 6f6c 6c65 7220  ar's controller 
-000017c0: 6172 6368 6974 6563 7475 7265 2066 6f6c  architecture fol
-000017d0: 6c6f 7773 2074 6865 204d 6f64 656c 2d56  lows the Model-V
-000017e0: 6965 772d 436f 6e74 726f 6c6c 6572 2028  iew-Controller (
-000017f0: 4d56 4329 2070 6174 7465 726e 2c20 6d61  MVC) pattern, ma
-00001800: 6b69 6e67 2069 7420 6561 7379 2074 6f20  king it easy to 
-00001810: 6f72 6761 6e69 7a65 2079 6f75 7220 636f  organize your co
-00001820: 6465 2e0a 2d20 2a2a 4775 6172 6473 2066  de..- **Guards f
-00001830: 6f72 2041 7574 6865 6e74 6963 6174 696f  or Authenticatio
-00001840: 6e20 616e 6420 4175 7468 6f72 697a 6174  n and Authorizat
-00001850: 696f 6e2a 2a3a 2049 7420 7072 6f76 6964  ion**: It provid
-00001860: 6573 2062 7569 6c74 2d69 6e20 7375 7070  es built-in supp
-00001870: 6f72 7420 666f 7220 6775 6172 6473 2c20  ort for guards, 
-00001880: 616c 6c6f 7769 6e67 2079 6f75 2074 6f20  allowing you to 
-00001890: 6561 7369 6c79 2069 6d70 6c65 6d65 6e74  easily implement
-000018a0: 2061 7574 6865 6e74 6963 6174 696f 6e20   authentication 
-000018b0: 616e 6420 6175 7468 6f72 697a 6174 696f  and authorizatio
-000018c0: 6e20 696e 2079 6f75 7220 6170 706c 6963  n in your applic
-000018d0: 6174 696f 6e2e 0a2d 202a 2a4d 6f64 756c  ation..- **Modul
-000018e0: 6172 6974 792a 2a3a 2045 6c6c 6172 2066  arity**: Ellar f
-000018f0: 6f6c 6c6f 7773 2061 206d 6f64 756c 6172  ollows a modular
-00001900: 2061 7263 6869 7465 6374 7572 6520 696e   architecture in
-00001910: 7370 6972 6564 2062 7920 4e65 7374 4a53  spired by NestJS
-00001920: 2c20 6d61 6b69 6e67 2069 7420 6561 7379  , making it easy
-00001930: 2074 6f20 6f72 6761 6e69 7a65 2079 6f75   to organize you
-00001940: 7220 636f 6465 2069 6e74 6f20 7265 7573  r code into reus
-00001950: 6162 6c65 206d 6f64 756c 6573 2e0a 2d20  able modules..- 
-00001960: 2a2a 4173 796e 6368 726f 6e6f 7573 2070  **Asynchronous p
-00001970: 726f 6772 616d 6d69 6e67 2a2a 3a20 4974  rogramming**: It
-00001980: 2061 6c6c 6f77 7320 796f 7520 746f 2074   allows you to t
-00001990: 616b 6573 2061 6476 616e 7461 6765 206f  akes advantage o
-000019a0: 6620 5079 7468 6f6e 2773 2060 6173 796e  f Python's `asyn
-000019b0: 632f 6177 6169 7460 2066 6561 7475 7265  c/await` feature
-000019c0: 2074 6f20 7772 6974 6520 6566 6669 6369   to write effici
-000019d0: 656e 7420 616e 6420 6661 7374 2063 6f64  ent and fast cod
-000019e0: 6520 7468 6174 2063 616e 2068 616e 646c  e that can handl
-000019f0: 6520 6c61 7267 6520 6e75 6d62 6572 7320  e large numbers 
-00001a00: 6f66 2063 6f6e 6375 7272 656e 7420 7265  of concurrent re
-00001a10: 7175 6573 7473 0a0a 2323 2044 6570 656e  quests..## Depen
-00001a20: 6465 6e63 6965 730a 2d20 5079 7468 6f6e  dencies.- Python
-00001a30: 203e 3d20 332e 370a 2d20 5374 6172 6c65   >= 3.7.- Starle
-00001a40: 7474 650a 2d20 496e 6a65 6374 6f72 0a2d  tte.- Injector.-
-00001a50: 2050 7964 616e 7469 630a 0a23 2320 496e   Pydantic..## In
-00001a60: 7374 616c 6c61 7469 6f6e 0a23 2323 2050  stallation.### P
-00001a70: 6f65 7472 7920 496e 7374 616c 6c61 7469  oetry Installati
-00001a80: 6f6e 0a46 6f72 205b 506f 6574 7279 5d28  on.For [Poetry](
-00001a90: 6874 7470 733a 2f2f 7079 7468 6f6e 2d70  https://python-p
-00001aa0: 6f65 7472 792e 6f72 672f 2920 7573 6167  oetry.org/) usag
-00001ab0: 6573 0a0a 6060 6073 6865 6c6c 0a70 6f65  es..```shell.poe
-00001ac0: 7472 7920 6164 6420 656c 6c61 722d 636c  try add ellar-cl
-00001ad0: 690a 6060 600a 0a23 2323 2050 6970 2049  i.```..### Pip I
-00001ae0: 6e73 7461 6c6c 6174 696f 6e0a 466f 7220  nstallation.For 
-00001af0: 6e6f 726d 616c 2070 6970 2069 6e73 7461  normal pip insta
-00001b00: 6c6c 6174 696f 6e0a 6060 6073 6865 6c6c  llation.```shell
-00001b10: 0a70 6970 2069 6e73 7461 6c6c 2065 6c6c  .pip install ell
-00001b20: 6172 2d63 6c69 0a60 6060 0a0a 2323 2043  ar-cli.```..## C
-00001b30: 7265 6174 6520 6120 7072 6f6a 6563 740a  reate a project.
-00001b40: 546f 2063 7265 6174 6520 616e 2065 6c6c  To create an ell
-00001b50: 6172 2070 726f 6a65 6374 2c20 796f 7520  ar project, you 
-00001b60: 6e65 6564 2074 6f20 6861 7665 2061 2060  need to have a `
-00001b70: 7079 7072 6f6a 6563 742e 746f 6d6c 6020  pyproject.toml` 
-00001b80: 6176 6169 6c61 626c 6520 6f6e 2079 6f75  available on you
-00001b90: 7220 726f 6f74 2064 6972 6563 746f 7279  r root directory
-00001ba0: 2e0a 5468 6973 2069 7320 6e65 6365 7373  ..This is necess
-00001bb0: 6172 7920 666f 7220 656c 6c61 7220 746f  ary for ellar to
-00001bc0: 2073 746f 7265 2073 6f6d 6520 606d 6574   store some `met
-00001bd0: 6164 6174 6160 2061 626f 7574 2079 6f75  adata` about you
-00001be0: 7220 7072 6f6a 6563 742e 200a 0a23 2323  r project. ..###
-00001bf0: 2043 7265 6174 6520 6120 7072 6f6a 6563   Create a projec
-00001c00: 740a 466f 7220 5069 7020 5573 6572 732c  t.For Pip Users,
-00001c10: 2079 6f75 206e 6565 6420 746f 2063 7265   you need to cre
-00001c20: 6174 6520 6070 7970 726f 6a65 6374 2e74  ate `pyproject.t
-00001c30: 6f6d 6c60 2066 696c 650a 6060 6073 6865  oml` file.```she
-00001c40: 6c6c 0a65 6c6c 6172 206e 6577 2063 6172  ll.ellar new car
-00001c50: 7369 7465 0a60 6060 0a49 6620 796f 7520  site.```.If you 
-00001c60: 6172 6520 7573 696e 6720 6050 6f65 7472  are using `Poetr
-00001c70: 7960 2c20 6174 2079 6f75 7220 7072 6f6a  y`, at your proj
-00001c80: 6563 7420 726f 6f74 2064 6972 6563 746f  ect root directo
-00001c90: 7279 2077 6974 6820 6070 7970 726f 6a65  ry with `pyproje
-00001ca0: 6374 2e74 6f6d 6c60 2c0a 7275 6e20 7468  ct.toml`,.run th
-00001cb0: 6520 656c 6c61 7220 6372 6561 7465 2070  e ellar create p
-00001cc0: 726f 6a65 6374 2063 6c69 2063 6f6d 6d61  roject cli comma
-00001cd0: 6e64 2c0a 6060 6073 6865 6c6c 0a65 6c6c  nd,.```shell.ell
-00001ce0: 6172 2063 7265 6174 652d 7072 6f6a 6563  ar create-projec
-00001cf0: 7420 6361 7273 6974 650a 6060 600a 0a23  t carsite.```..#
-00001d00: 2320 5275 6e20 796f 7572 2070 726f 6a65  # Run your proje
-00001d10: 6374 0a45 6c6c 6172 2072 756e 7320 5b55  ct.Ellar runs [U
-00001d20: 5649 434f 524e 202d 2041 5347 4920 5365  VICORN - ASGI Se
-00001d30: 7276 6572 5d28 6874 7470 733a 2f2f 7777  rver](https://ww
-00001d40: 772e 7576 6963 6f72 6e2e 6f72 672f 2920  w.uvicorn.org/) 
-00001d50: 756e 6465 7220 7468 6520 686f 6f64 2e0a  under the hood..
-00001d60: 6060 6073 6865 6c6c 0a65 6c6c 6172 2072  ```shell.ellar r
-00001d70: 756e 7365 7276 6572 202d 2d72 656c 6f61  unserver --reloa
-00001d80: 640a 6060 600a 602d 2d72 656c 6f61 6460  d.```.`--reload`
-00001d90: 2069 7320 746f 2077 6174 6368 2066 6f72   is to watch for
-00001da0: 2066 696c 6520 6368 616e 6765 730a 0a4e   file changes..N
-00001db0: 6f77 2067 6f20 746f 205b 6874 7470 3a2f  ow go to [http:/
-00001dc0: 2f31 3237 2e30 2e30 2e31 3a38 3030 305d  /127.0.0.1:8000]
-00001dd0: 2868 7474 703a 2f2f 3132 372e 302e 302e  (http://127.0.0.
-00001de0: 313a 3830 3030 290a 215b 5377 6167 6765  1:8000).![Swagge
-00001df0: 7220 5549 5d28 646f 6373 2f69 6d67 2f65  r UI](docs/img/e
-00001e00: 6c6c 6172 5f66 7261 6d65 776f 726b 2e70  llar_framework.p
-00001e10: 6e67 290a 0a46 6f72 206d 6f72 6520 696e  ng)..For more in
-00001e20: 666f 206f 6e20 456c 6c61 7220 434c 492c  fo on Ellar CLI,
-00001e30: 2063 6c69 636b 205b 6865 7265 5d28 6874   click [here](ht
-00001e40: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001e50: 2f65 6164 7769 6e43 6f64 652f 656c 6c61  /eadwinCode/ella
-00001e60: 722d 636c 6929 0a0a 2323 2043 7265 6174  r-cli)..## Creat
-00001e70: 6520 6120 7072 6f6a 6563 7420 6d6f 6475  e a project modu
-00001e80: 6c65 0a41 2070 726f 6a65 6374 206d 6f64  le.A project mod
-00001e90: 756c 6520 6973 2061 2070 726f 6a65 6374  ule is a project
-00001ea0: 2061 7070 2064 6566 696e 696e 6720 6120   app defining a 
-00001eb0: 6772 6f75 7020 6f66 2063 6f6e 7472 6f6c  group of control
-00001ec0: 6c65 7273 206f 7220 7365 7276 6963 6573  lers or services
-00001ed0: 2069 6e63 6c75 6469 6e67 2074 656d 706c   including templ
-00001ee0: 6174 6573 2061 6e64 2073 7461 7469 6320  ates and static 
-00001ef0: 6669 6c65 732e 0a53 6f2c 206e 6f77 2077  files..So, now w
-00001f00: 6520 6861 7665 2061 2070 726f 6a65 6374  e have a project
-00001f10: 2063 7265 6174 6564 2c20 6c65 7473 2061   created, lets a
-00001f20: 6464 2061 6e20 6170 7020 746f 2074 6865  dd an app to the
-00001f30: 2070 726f 6a65 6374 2e0a 6060 6073 6865   project..```she
-00001f40: 6c6c 0a65 6c6c 6172 2063 7265 6174 652d  ll.ellar create-
-00001f50: 6d6f 6475 6c65 2063 6172 0a60 6060 0a0a  module car.```..
-00001f60: 2323 2041 6464 2053 6368 656d 610a 496e  ## Add Schema.In
-00001f70: 2060 6361 722f 7363 6865 6d61 2e70 7960   `car/schema.py`
-00001f80: 2c20 6c65 7473 2061 6464 2073 6f6d 6520  , lets add some 
-00001f90: 7365 7269 616c 697a 6572 2066 6f72 2063  serializer for c
-00001fa0: 6172 2069 6e70 7574 2061 6e64 206f 7574  ar input and out
-00001fb0: 7075 7420 6461 7461 0a60 6060 7079 7468  put data.```pyth
-00001fc0: 6f6e 0a66 726f 6d20 656c 6c61 722e 7365  on.from ellar.se
-00001fd0: 7269 616c 697a 6572 2069 6d70 6f72 7420  rializer import 
-00001fe0: 5365 7269 616c 697a 6572 0a0a 636c 6173  Serializer..clas
-00001ff0: 7320 4361 7253 6572 6961 6c69 7a65 7228  s CarSerializer(
-00002000: 5365 7269 616c 697a 6572 293a 0a20 2020  Serializer):.   
-00002010: 206e 616d 653a 2073 7472 0a20 2020 206d   name: str.    m
-00002020: 6f64 656c 3a20 7374 720a 2020 2020 6272  odel: str.    br
-00002030: 616e 643a 2073 7472 0a0a 0a63 6c61 7373  and: str...class
-00002040: 2052 6574 7269 6576 6543 6172 5365 7269   RetrieveCarSeri
-00002050: 616c 697a 6572 2843 6172 5365 7269 616c  alizer(CarSerial
-00002060: 697a 6572 293a 0a20 2020 2070 6b3a 2073  izer):.    pk: s
-00002070: 7472 0a60 6060 0a0a 2323 2041 6464 2053  tr.```..## Add S
-00002080: 6572 7669 6365 730a 496e 2060 6361 722f  ervices.In `car/
-00002090: 7365 7276 6963 6573 2e70 7960 2c20 6c65  services.py`, le
-000020a0: 7473 2063 7265 6174 6520 6120 6475 6d6d  ts create a dumm
-000020b0: 7920 7265 706f 7369 746f 7279 2060 4361  y repository `Ca
-000020c0: 7244 756d 6d79 4442 6020 746f 206d 616e  rDummyDB` to man
-000020d0: 6167 6520 6f75 7220 6361 7220 6461 7461  age our car data
-000020e0: 2e0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
-000020f0: 7274 2074 7970 696e 6720 6173 2074 0a69  rt typing as t.i
-00002100: 6d70 6f72 7420 7575 6964 0a66 726f 6d20  mport uuid.from 
-00002110: 656c 6c61 722e 6469 2069 6d70 6f72 7420  ellar.di import 
-00002120: 696e 6a65 6374 6162 6c65 2c20 7369 6e67  injectable, sing
-00002130: 6c65 746f 6e5f 7363 6f70 650a 0a0a 4069  leton_scope...@i
-00002140: 6e6a 6563 7461 626c 6528 7363 6f70 653d  njectable(scope=
-00002150: 7369 6e67 6c65 746f 6e5f 7363 6f70 6529  singleton_scope)
-00002160: 0a63 6c61 7373 2043 6172 4475 6d6d 7944  .class CarDummyD
-00002170: 423a 0a20 2020 2063 6c61 7373 2043 6172  B:.    class Car
-00002180: 4475 6d6d 7944 4249 7465 6d3a 0a20 2020  DummyDBItem:.   
-00002190: 2020 2020 2070 6b3a 2073 7472 0a0a 2020       pk: str..  
-000021a0: 2020 2020 2020 6465 6620 5f5f 696e 6974        def __init
-000021b0: 5f5f 2873 656c 662c 202a 2a64 6174 613a  __(self, **data:
-000021c0: 2074 2e44 6963 7429 202d 3e20 4e6f 6e65   t.Dict) -> None
-000021d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000021e0: 6c66 2e5f 5f64 6963 745f 5f20 3d20 6461  lf.__dict__ = da
-000021f0: 7461 0a0a 2020 2020 2020 2020 6465 6620  ta..        def 
-00002200: 5f5f 6571 5f5f 2873 656c 662c 206f 7468  __eq__(self, oth
-00002210: 6572 293a 0a20 2020 2020 2020 2020 2020  er):.           
-00002220: 2069 6620 6973 696e 7374 616e 6365 286f   if isinstance(o
-00002230: 7468 6572 2c20 4361 7244 756d 6d79 4442  ther, CarDummyDB
-00002240: 2e43 6172 4475 6d6d 7944 4249 7465 6d29  .CarDummyDBItem)
-00002250: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002260: 2020 7265 7475 726e 2073 656c 662e 706b    return self.pk
-00002270: 203d 3d20 6f74 6865 722e 706b 0a20 2020   == other.pk.   
-00002280: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00002290: 7365 6c66 2e70 6b20 3d3d 2073 7472 286f  self.pk == str(o
-000022a0: 7468 6572 290a 0a20 2020 2064 6566 205f  ther)..    def _
-000022b0: 5f69 6e69 745f 5f28 7365 6c66 2920 2d3e  _init__(self) ->
-000022c0: 204e 6f6e 653a 0a20 2020 2020 2020 2073   None:.        s
-000022d0: 656c 662e 5f64 6174 613a 2074 2e4c 6973  elf._data: t.Lis
-000022e0: 745b 4361 7244 756d 6d79 4442 2e43 6172  t[CarDummyDB.Car
-000022f0: 4475 6d6d 7944 4249 7465 6d5d 203d 205b  DummyDBItem] = [
-00002300: 5d0a 0a20 2020 2064 6566 2061 6464 5f63  ]..    def add_c
-00002310: 6172 2873 656c 662c 2064 6174 613a 2074  ar(self, data: t
-00002320: 2e44 6963 7429 202d 3e20 7374 723a 0a20  .Dict) -> str:. 
-00002330: 2020 2020 2020 2070 6b20 3d20 7575 6964         pk = uuid
-00002340: 2e75 7569 6434 2829 0a20 2020 2020 2020  .uuid4().       
-00002350: 205f 6461 7461 203d 2064 6963 7428 6461   _data = dict(da
-00002360: 7461 290a 2020 2020 2020 2020 5f64 6174  ta).        _dat
-00002370: 612e 7570 6461 7465 2870 6b3d 7374 7228  a.update(pk=str(
-00002380: 706b 2929 0a20 2020 2020 2020 2069 7465  pk)).        ite
-00002390: 6d20 3d20 7365 6c66 2e43 6172 4475 6d6d  m = self.CarDumm
-000023a0: 7944 4249 7465 6d28 2a2a 5f64 6174 6129  yDBItem(**_data)
-000023b0: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
-000023c0: 6174 612e 6170 7065 6e64 2869 7465 6d29  ata.append(item)
-000023d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000023e0: 6974 656d 2e70 6b0a 0a20 2020 2064 6566  item.pk..    def
-000023f0: 206c 6973 7428 7365 6c66 2920 2d3e 2074   list(self) -> t
-00002400: 2e4c 6973 745b 2243 6172 4475 6d6d 7944  .List["CarDummyD
-00002410: 422e 4361 7244 756d 6d79 4442 4974 656d  B.CarDummyDBItem
-00002420: 225d 3a0a 2020 2020 2020 2020 7265 7475  "]:.        retu
-00002430: 726e 2073 656c 662e 5f64 6174 610a 0a20  rn self._data.. 
-00002440: 2020 2064 6566 2075 7064 6174 6528 7365     def update(se
-00002450: 6c66 2c20 6361 725f 6964 3a20 7374 722c  lf, car_id: str,
-00002460: 2064 6174 613a 2074 2e44 6963 7429 202d   data: t.Dict) -
-00002470: 3e20 742e 4f70 7469 6f6e 616c 5b22 4361  > t.Optional["Ca
-00002480: 7244 756d 6d79 4442 2e43 6172 4475 6d6d  rDummyDB.CarDumm
-00002490: 7944 4249 7465 6d22 5d3a 0a20 2020 2020  yDBItem"]:.     
-000024a0: 2020 2069 6478 203d 2073 656c 662e 5f64     idx = self._d
-000024b0: 6174 612e 696e 6465 7828 6361 725f 6964  ata.index(car_id
-000024c0: 290a 2020 2020 2020 2020 6966 2069 6478  ).        if idx
-000024d0: 203e 3d20 303a 0a20 2020 2020 2020 2020   >= 0:.         
-000024e0: 2020 205f 6461 7461 203d 2064 6963 7428     _data = dict(
-000024f0: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
-00002500: 2020 5f64 6174 612e 7570 6461 7465 2870    _data.update(p
-00002510: 6b3d 7374 7228 6361 725f 6964 2929 0a20  k=str(car_id)). 
-00002520: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002530: 5f64 6174 615b 6964 785d 203d 2073 656c  _data[idx] = sel
-00002540: 662e 4361 7244 756d 6d79 4442 4974 656d  f.CarDummyDBItem
-00002550: 282a 2a5f 6461 7461 290a 2020 2020 2020  (**_data).      
-00002560: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00002570: 662e 5f64 6174 615b 6964 785d 0a0a 2020  f._data[idx]..  
-00002580: 2020 6465 6620 6765 7428 7365 6c66 2c20    def get(self, 
-00002590: 6361 725f 6964 3a20 7374 7229 202d 3e20  car_id: str) -> 
-000025a0: 742e 4f70 7469 6f6e 616c 5b22 4361 7244  t.Optional["CarD
-000025b0: 756d 6d79 4442 2e43 6172 4475 6d6d 7944  ummyDB.CarDummyD
-000025c0: 4249 7465 6d22 5d3a 0a20 2020 2020 2020  BItem"]:.       
-000025d0: 2069 6478 203d 2073 656c 662e 5f64 6174   idx = self._dat
-000025e0: 612e 696e 6465 7828 6361 725f 6964 290a  a.index(car_id).
-000025f0: 2020 2020 2020 2020 6966 2069 6478 203e          if idx >
-00002600: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00002610: 2072 6574 7572 6e20 7365 6c66 2e5f 6461   return self._da
-00002620: 7461 5b69 6478 5d0a 0a20 2020 2064 6566  ta[idx]..    def
-00002630: 2072 656d 6f76 6528 7365 6c66 2c20 6361   remove(self, ca
-00002640: 725f 6964 3a20 7374 7229 202d 3e20 742e  r_id: str) -> t.
-00002650: 4f70 7469 6f6e 616c 5b22 4361 7244 756d  Optional["CarDum
-00002660: 6d79 4442 2e43 6172 4475 6d6d 7944 4249  myDB.CarDummyDBI
-00002670: 7465 6d22 5d3a 0a20 2020 2020 2020 2069  tem"]:.        i
-00002680: 6478 203d 2073 656c 662e 5f64 6174 612e  dx = self._data.
-00002690: 696e 6465 7828 6361 725f 6964 290a 2020  index(car_id).  
-000026a0: 2020 2020 2020 6966 2069 6478 203e 3d20        if idx >= 
-000026b0: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
-000026c0: 6574 7572 6e20 7365 6c66 2e5f 6461 7461  eturn self._data
-000026d0: 2e70 6f70 2869 6478 290a 6060 600a 2323  .pop(idx).```.##
-000026e0: 2041 6464 2043 6f6e 7472 6f6c 6c65 720a   Add Controller.
-000026f0: 496e 2060 6361 722f 636f 6e74 726f 6c6c  In `car/controll
-00002700: 6572 732e 7079 602c 206c 6574 7320 6372  ers.py`, lets cr
-00002710: 6561 7465 2060 4361 7243 6f6e 7472 6f6c  eate `CarControl
-00002720: 6c65 7260 0a0a 6060 6070 7974 686f 6e0a  ler`..```python.
-00002730: 696d 706f 7274 2074 7970 696e 6720 6173  import typing as
-00002740: 2074 0a66 726f 6d20 656c 6c61 722e 636f   t.from ellar.co
-00002750: 6d6d 6f6e 2069 6d70 6f72 7420 436f 6e74  mmon import Cont
-00002760: 726f 6c6c 6572 2c20 6465 6c65 7465 2c20  roller, delete, 
-00002770: 6765 742c 2070 7574 2c20 706f 7374 0a66  get, put, post.f
-00002780: 726f 6d20 656c 6c61 722e 636f 7265 2069  rom ellar.core i
-00002790: 6d70 6f72 7420 436f 6e74 726f 6c6c 6572  mport Controller
-000027a0: 4261 7365 0a66 726f 6d20 656c 6c61 722e  Base.from ellar.
-000027b0: 636f 7265 2e65 7863 6570 7469 6f6e 7320  core.exceptions 
-000027c0: 696d 706f 7274 204e 6f74 466f 756e 640a  import NotFound.
-000027d0: 6672 6f6d 202e 7363 6865 6d61 7320 696d  from .schemas im
-000027e0: 706f 7274 2043 6172 5365 7269 616c 697a  port CarSerializ
-000027f0: 6572 2c20 5265 7472 6965 7665 4361 7253  er, RetrieveCarS
-00002800: 6572 6961 6c69 7a65 720a 6672 6f6d 202e  erializer.from .
-00002810: 7365 7276 6963 6573 2069 6d70 6f72 7420  services import 
-00002820: 4361 7244 756d 6d79 4442 0a0a 0a40 436f  CarDummyDB...@Co
-00002830: 6e74 726f 6c6c 6572 0a63 6c61 7373 2043  ntroller.class C
-00002840: 6172 436f 6e74 726f 6c6c 6572 2843 6f6e  arController(Con
-00002850: 7472 6f6c 6c65 7242 6173 6529 3a0a 2020  trollerBase):.  
-00002860: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00002870: 656c 662c 2064 623a 2043 6172 4475 6d6d  elf, db: CarDumm
-00002880: 7944 4229 202d 3e20 4e6f 6e65 3a0a 2020  yDB) -> None:.  
-00002890: 2020 2020 2020 7365 6c66 2e63 6172 5f64        self.car_d
-000028a0: 6220 3d20 6462 0a0a 2020 2020 4070 6f73  b = db..    @pos
-000028b0: 7428 222f 6372 6561 7465 222c 2072 6573  t("/create", res
-000028c0: 706f 6e73 653d 7b32 3030 3a20 7374 727d  ponse={200: str}
-000028d0: 290a 2020 2020 6173 796e 6320 6465 6620  ).    async def 
-000028e0: 6372 6561 7465 5f63 6174 2873 656c 662c  create_cat(self,
-000028f0: 2070 6179 6c6f 6164 3a20 4361 7253 6572   payload: CarSer
-00002900: 6961 6c69 7a65 7229 3a0a 2020 2020 2020  ializer):.      
-00002910: 2020 706b 203d 2073 656c 662e 6361 725f    pk = self.car_
-00002920: 6462 2e61 6464 5f63 6172 2870 6179 6c6f  db.add_car(paylo
-00002930: 6164 2e64 6963 7428 2929 0a20 2020 2020  ad.dict()).     
-00002940: 2020 2072 6574 7572 6e20 706b 0a0a 2020     return pk..  
-00002950: 2020 4070 7574 2822 2f7b 6361 725f 6964    @put("/{car_id
-00002960: 3a73 7472 7d22 2c20 7265 7370 6f6e 7365  :str}", response
-00002970: 3d7b 3230 303a 2052 6574 7269 6576 6543  ={200: RetrieveC
-00002980: 6172 5365 7269 616c 697a 6572 7d29 0a20  arSerializer}). 
-00002990: 2020 2061 7379 6e63 2064 6566 2075 7064     async def upd
-000029a0: 6174 655f 6361 7428 7365 6c66 2c20 6361  ate_cat(self, ca
-000029b0: 725f 6964 3a20 7374 722c 2070 6179 6c6f  r_id: str, paylo
-000029c0: 6164 3a20 4361 7253 6572 6961 6c69 7a65  ad: CarSerialize
-000029d0: 7229 3a0a 2020 2020 2020 2020 6361 7220  r):.        car 
-000029e0: 3d20 7365 6c66 2e63 6172 5f64 622e 7570  = self.car_db.up
-000029f0: 6461 7465 2863 6172 5f69 642c 2070 6179  date(car_id, pay
-00002a00: 6c6f 6164 2e64 6963 7428 2929 0a20 2020  load.dict()).   
-00002a10: 2020 2020 2069 6620 6e6f 7420 6361 723a       if not car:
-00002a20: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00002a30: 7365 204e 6f74 466f 756e 6428 2249 7465  se NotFound("Ite
-00002a40: 6d20 6e6f 7420 666f 756e 6422 290a 2020  m not found").  
-00002a50: 2020 2020 2020 7265 7475 726e 2063 6172        return car
-00002a60: 0a0a 2020 2020 4067 6574 2822 2f7b 6361  ..    @get("/{ca
-00002a70: 725f 6964 3a73 7472 7d22 2c20 7265 7370  r_id:str}", resp
-00002a80: 6f6e 7365 3d7b 3230 303a 2052 6574 7269  onse={200: Retri
-00002a90: 6576 6543 6172 5365 7269 616c 697a 6572  eveCarSerializer
-00002aa0: 7d29 0a20 2020 2061 7379 6e63 2064 6566  }).    async def
-00002ab0: 2067 6574 5f63 6172 5f62 795f 6964 2873   get_car_by_id(s
-00002ac0: 656c 662c 2063 6172 5f69 643a 2073 7472  elf, car_id: str
-00002ad0: 293a 0a20 2020 2020 2020 2063 6172 203d  ):.        car =
-00002ae0: 2073 656c 662e 6361 725f 6462 2e67 6574   self.car_db.get
-00002af0: 2863 6172 5f69 6429 0a20 2020 2020 2020  (car_id).       
-00002b00: 2069 6620 6e6f 7420 6361 723a 0a20 2020   if not car:.   
-00002b10: 2020 2020 2020 2020 2072 6169 7365 204e           raise N
-00002b20: 6f74 466f 756e 6428 2749 7465 6d20 6e6f  otFound('Item no
-00002b30: 7420 666f 756e 642e 2729 0a20 2020 2020  t found.').     
-00002b40: 2020 2072 6574 7572 6e20 6361 720a 0a20     return car.. 
-00002b50: 2020 2040 6465 6c65 7465 2822 2f7b 6361     @delete("/{ca
-00002b60: 725f 6964 3a73 7472 7d22 2c20 7265 7370  r_id:str}", resp
-00002b70: 6f6e 7365 3d7b 3230 343a 2064 6963 747d  onse={204: dict}
-00002b80: 290a 2020 2020 6173 796e 6320 6465 6620  ).    async def 
-00002b90: 6465 6c65 7465 645f 6361 7428 7365 6c66  deleted_cat(self
-00002ba0: 2c20 6361 725f 6964 3a20 7374 7229 3a0a  , car_id: str):.
-00002bb0: 2020 2020 2020 2020 6361 7220 3d20 7365          car = se
-00002bc0: 6c66 2e63 6172 5f64 622e 7265 6d6f 7665  lf.car_db.remove
-00002bd0: 2863 6172 5f69 6429 0a20 2020 2020 2020  (car_id).       
-00002be0: 2069 6620 6e6f 7420 6361 723a 0a20 2020   if not car:.   
-00002bf0: 2020 2020 2020 2020 2072 6169 7365 204e           raise N
-00002c00: 6f74 466f 756e 6428 2749 7465 6d20 6e6f  otFound('Item no
-00002c10: 7420 666f 756e 642e 2729 0a20 2020 2020  t found.').     
-00002c20: 2020 2072 6574 7572 6e20 3230 342c 207b     return 204, {
-00002c30: 7d0a 0a20 2020 2040 6765 7428 222f 222c  }..    @get("/",
-00002c40: 2072 6573 706f 6e73 653d 7b32 3030 3a20   response={200: 
-00002c50: 742e 4c69 7374 5b52 6574 7269 6576 6543  t.List[RetrieveC
-00002c60: 6172 5365 7269 616c 697a 6572 5d7d 290a  arSerializer]}).
-00002c70: 2020 2020 6173 796e 6320 6465 6620 6c69      async def li
-00002c80: 7374 2873 656c 6629 3a0a 2020 2020 2020  st(self):.      
-00002c90: 2020 7265 7475 726e 2073 656c 662e 6361    return self.ca
-00002ca0: 725f 6462 2e6c 6973 7428 290a 0a60 6060  r_db.list()..```
-00002cb0: 0a23 2320 5265 6769 7374 6572 2053 6572  .## Register Ser
-00002cc0: 7669 6365 2061 6e64 2043 6f6e 7472 6f6c  vice and Control
-00002cd0: 6c65 720a 496e 2060 6361 722f 6d6f 6475  ler.In `car/modu
-00002ce0: 6c65 2e70 7960 2c20 6c65 7473 2072 6567  le.py`, lets reg
-00002cf0: 6973 7465 7220 6043 6172 436f 6e74 726f  ister `CarContro
-00002d00: 6c6c 6572 6020 616e 6420 6043 6172 4475  ller` and `CarDu
-00002d10: 6d6d 7944 4260 0a0a 6060 6070 7974 686f  mmyDB`..```pytho
-00002d20: 6e0a 6672 6f6d 2065 6c6c 6172 2e63 6f6d  n.from ellar.com
-00002d30: 6d6f 6e20 696d 706f 7274 204d 6f64 756c  mon import Modul
-00002d40: 650a 6672 6f6d 2065 6c6c 6172 2e63 6f72  e.from ellar.cor
-00002d50: 6520 696d 706f 7274 204d 6f64 756c 6542  e import ModuleB
-00002d60: 6173 650a 6672 6f6d 2065 6c6c 6172 2e64  ase.from ellar.d
-00002d70: 6920 696d 706f 7274 2043 6f6e 7461 696e  i import Contain
-00002d80: 6572 0a0a 6672 6f6d 202e 636f 6e74 726f  er..from .contro
-00002d90: 6c6c 6572 7320 696d 706f 7274 2043 6172  llers import Car
-00002da0: 436f 6e74 726f 6c6c 6572 0a66 726f 6d20  Controller.from 
-00002db0: 2e73 6572 7669 6365 7320 696d 706f 7274  .services import
-00002dc0: 2043 6172 4475 6d6d 7944 420a 0a0a 404d   CarDummyDB...@M
-00002dd0: 6f64 756c 6528 0a20 2020 2063 6f6e 7472  odule(.    contr
-00002de0: 6f6c 6c65 7273 3d5b 4361 7243 6f6e 7472  ollers=[CarContr
-00002df0: 6f6c 6c65 725d 2c0a 2020 2020 7072 6f76  oller],.    prov
-00002e00: 6964 6572 733d 5b43 6172 4475 6d6d 7944  iders=[CarDummyD
-00002e10: 425d 2c0a 2020 2020 726f 7574 6572 733d  B],.    routers=
-00002e20: 5b5d 2c0a 290a 636c 6173 7320 4361 724d  [],.).class CarM
-00002e30: 6f64 756c 6528 4d6f 6475 6c65 4261 7365  odule(ModuleBase
-00002e40: 293a 0a20 2020 2064 6566 2072 6567 6973  ):.    def regis
-00002e50: 7465 725f 7072 6f76 6964 6572 7328 7365  ter_providers(se
-00002e60: 6c66 2c20 636f 6e74 6169 6e65 723a 2043  lf, container: C
-00002e70: 6f6e 7461 696e 6572 2920 2d3e 204e 6f6e  ontainer) -> Non
-00002e80: 653a 0a20 2020 2020 2020 2023 2066 6f72  e:.        # for
-00002e90: 206d 6f72 6520 636f 6d70 6c69 6361 7465   more complicate
-00002ea0: 6420 7072 6f76 6964 6572 2072 6567 6973  d provider regis
-00002eb0: 7472 6174 696f 6e73 0a20 2020 2020 2020  trations.       
-00002ec0: 2023 2063 6f6e 7461 696e 6572 2e72 6567   # container.reg
-00002ed0: 6973 7465 725f 696e 7374 616e 6365 282e  ister_instance(.
-00002ee0: 2e2e 290a 2020 2020 2020 2020 7061 7373  ..).        pass
-00002ef0: 0a60 6060 0a0a 2323 2052 6567 6973 7465  .```..## Registe
-00002f00: 7269 6e67 204d 6f64 756c 650a 456c 6c61  ring Module.Ella
-00002f10: 7220 6973 206e 6f74 2061 7761 7265 206f  r is not aware o
-00002f20: 6620 6043 6172 4d6f 6475 6c65 6020 7965  f `CarModule` ye
-00002f30: 742c 2073 6f20 7765 206e 6565 6420 746f  t, so we need to
-00002f40: 2061 6464 2069 7420 746f 2074 6865 2060   add it to the `
-00002f50: 6d6f 6475 6c65 7360 206c 6973 7420 6f66  modules` list of
-00002f60: 2060 4170 706c 6963 6174 696f 6e4d 6f64   `ApplicationMod
-00002f70: 756c 6560 2061 7420 7468 6520 6063 6172  ule` at the `car
-00002f80: 7369 7465 2f72 6f6f 745f 6d6f 6475 6c65  site/root_module
-00002f90: 2e70 7960 2e0a 6060 6070 7974 686f 6e0a  .py`..```python.
-00002fa0: 6672 6f6d 2065 6c6c 6172 2e63 6f6d 6d6f  from ellar.commo
-00002fb0: 6e20 696d 706f 7274 204d 6f64 756c 652c  n import Module,
-00002fc0: 2065 7863 6570 7469 6f6e 5f68 616e 646c   exception_handl
-00002fd0: 6572 0a66 726f 6d20 656c 6c61 722e 636f  er.from ellar.co
-00002fe0: 7265 2069 6d70 6f72 7420 4948 6f73 7443  re import IHostC
-00002ff0: 6f6e 7465 7874 2c20 4d6f 6475 6c65 4261  ontext, ModuleBa
-00003000: 7365 0a66 726f 6d20 656c 6c61 722e 636f  se.from ellar.co
-00003010: 7265 2e72 6573 706f 6e73 6520 696d 706f  re.response impo
-00003020: 7274 204a 534f 4e52 6573 706f 6e73 652c  rt JSONResponse,
-00003030: 2052 6573 706f 6e73 650a 0a66 726f 6d20   Response..from 
-00003040: 656c 6c61 722e 7361 6d70 6c65 732e 6d6f  ellar.samples.mo
-00003050: 6475 6c65 7320 696d 706f 7274 2048 6f6d  dules import Hom
-00003060: 654d 6f64 756c 650a 6672 6f6d 202e 6170  eModule.from .ap
-00003070: 7073 2e63 6172 2e6d 6f64 756c 6520 696d  ps.car.module im
-00003080: 706f 7274 2043 6172 4d6f 6475 6c65 0a0a  port CarModule..
-00003090: 0a40 4d6f 6475 6c65 286d 6f64 756c 6573  .@Module(modules
-000030a0: 3d5b 486f 6d65 4d6f 6475 6c65 2c20 4361  =[HomeModule, Ca
-000030b0: 724d 6f64 756c 655d 290a 636c 6173 7320  rModule]).class 
-000030c0: 4170 706c 6963 6174 696f 6e4d 6f64 756c  ApplicationModul
-000030d0: 6528 4d6f 6475 6c65 4261 7365 293a 0a20  e(ModuleBase):. 
-000030e0: 2020 2040 6578 6365 7074 696f 6e5f 6861     @exception_ha
-000030f0: 6e64 6c65 7228 3430 3429 0a20 2020 2064  ndler(404).    d
-00003100: 6566 2065 7863 6570 7469 6f6e 5f34 3034  ef exception_404
-00003110: 5f68 616e 646c 6572 2863 6c73 2c20 636f  _handler(cls, co
-00003120: 6e74 6578 743a 2049 486f 7374 436f 6e74  ntext: IHostCont
-00003130: 6578 742c 2065 7863 3a20 4578 6365 7074  ext, exc: Except
-00003140: 696f 6e29 202d 3e20 5265 7370 6f6e 7365  ion) -> Response
-00003150: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00003160: 204a 534f 4e52 6573 706f 6e73 6528 6469   JSONResponse(di
-00003170: 6374 2864 6574 6169 6c3d 2252 6573 6f75  ct(detail="Resou
-00003180: 7263 6520 6e6f 7420 666f 756e 642e 2229  rce not found.")
-00003190: 290a 0a60 6060 0a23 2320 456e 6162 6c69  )..```.## Enabli
-000031a0: 6e67 204f 7065 6e41 5049 2044 6f63 730a  ng OpenAPI Docs.
-000031b0: 546f 2073 7461 7274 2075 7020 6f70 656e  To start up open
-000031c0: 6170 692c 2077 6520 6e65 6564 2074 6f20  api, we need to 
-000031d0: 676f 2062 6163 6b20 746f 2070 726f 6a65  go back to proje
-000031e0: 6374 2066 6f6c 6465 7220 696e 2074 6865  ct folder in the
-000031f0: 2060 7365 7276 6572 2e70 7960 0a74 6865   `server.py`.the
-00003200: 6e20 6164 6420 7468 6520 666f 6c6c 6f77  n add the follow
-00003210: 696e 6720 6265 6c6f 772e 0a60 6060 7079  ing below..```py
-00003220: 7468 6f6e 0a69 6d70 6f72 7420 6f73 0a0a  thon.import os..
-00003230: 6672 6f6d 2065 6c6c 6172 2e63 6f6e 7374  from ellar.const
-00003240: 616e 7473 2069 6d70 6f72 7420 454c 4c41  ants import ELLA
-00003250: 525f 434f 4e46 4947 5f4d 4f44 554c 450a  R_CONFIG_MODULE.
-00003260: 6672 6f6d 2065 6c6c 6172 2e63 6f72 652e  from ellar.core.
-00003270: 6661 6374 6f72 7920 696d 706f 7274 2041  factory import A
-00003280: 7070 4661 6374 6f72 790a 6672 6f6d 2065  ppFactory.from e
-00003290: 6c6c 6172 2e6f 7065 6e61 7069 2069 6d70  llar.openapi imp
-000032a0: 6f72 7420 4f70 656e 4150 4944 6f63 756d  ort OpenAPIDocum
-000032b0: 656e 744d 6f64 756c 652c 204f 7065 6e41  entModule, OpenA
-000032c0: 5049 446f 6375 6d65 6e74 4275 696c 6465  PIDocumentBuilde
-000032d0: 722c 2053 7761 6767 6572 446f 6375 6d65  r, SwaggerDocume
-000032e0: 6e74 4765 6e65 7261 746f 720a 6672 6f6d  ntGenerator.from
-000032f0: 202e 726f 6f74 5f6d 6f64 756c 6520 696d   .root_module im
-00003300: 706f 7274 2041 7070 6c69 6361 7469 6f6e  port Application
-00003310: 4d6f 6475 6c65 0a0a 6170 706c 6963 6174  Module..applicat
-00003320: 696f 6e20 3d20 4170 7046 6163 746f 7279  ion = AppFactory
-00003330: 2e63 7265 6174 655f 6672 6f6d 5f61 7070  .create_from_app
-00003340: 5f6d 6f64 756c 6528 0a20 2020 2041 7070  _module(.    App
-00003350: 6c69 6361 7469 6f6e 4d6f 6475 6c65 2c0a  licationModule,.
-00003360: 2020 2020 636f 6e66 6967 5f6d 6f64 756c      config_modul
-00003370: 653d 6f73 2e65 6e76 6972 6f6e 2e67 6574  e=os.environ.get
-00003380: 280a 2020 2020 2020 2020 454c 4c41 525f  (.        ELLAR_
-00003390: 434f 4e46 4947 5f4d 4f44 554c 452c 2022  CONFIG_MODULE, "
-000033a0: 6361 7273 6974 652e 636f 6e66 6967 3a44  carsite.config:D
-000033b0: 6576 656c 6f70 6d65 6e74 436f 6e66 6967  evelopmentConfig
-000033c0: 220a 2020 2020 292c 0a29 0a0a 646f 6375  ".    ),.)..docu
-000033d0: 6d65 6e74 5f62 7569 6c64 6572 203d 204f  ment_builder = O
-000033e0: 7065 6e41 5049 446f 6375 6d65 6e74 4275  penAPIDocumentBu
-000033f0: 696c 6465 7228 290a 646f 6375 6d65 6e74  ilder().document
-00003400: 5f62 7569 6c64 6572 2e73 6574 5f74 6974  _builder.set_tit
-00003410: 6c65 2827 4361 7253 6974 6520 4150 4927  le('CarSite API'
-00003420: 2920 5c0a 2020 2020 2e73 6574 5f76 6572  ) \.    .set_ver
-00003430: 7369 6f6e 2827 312e 302e 3027 2920 5c0a  sion('1.0.0') \.
-00003440: 2020 2020 2e73 6574 5f63 6f6e 7461 6374      .set_contact
-00003450: 286e 616d 653d 2745 6164 7769 6e27 2c20  (name='Eadwin', 
-00003460: 7572 6c3d 2768 7474 7073 3a2f 2f77 7777  url='https://www
-00003470: 2e79 6168 6f6f 2e63 6f6d 272c 2065 6d61  .yahoo.com', ema
-00003480: 696c 3d27 6561 6477 696e 4067 6d61 696c  il='eadwin@gmail
-00003490: 2e63 6f6d 2729 205c 0a20 2020 202e 7365  .com') \.    .se
-000034a0: 745f 6c69 6365 6e73 6528 274d 4954 204c  t_license('MIT L
-000034b0: 6963 656e 6365 272c 2075 726c 3d27 6874  icence', url='ht
-000034c0: 7470 733a 2f2f 7777 772e 676f 6f67 6c65  tps://www.google
-000034d0: 2e63 6f6d 2729 0a0a 646f 6375 6d65 6e74  .com')..document
-000034e0: 203d 2064 6f63 756d 656e 745f 6275 696c   = document_buil
-000034f0: 6465 722e 6275 696c 645f 646f 6375 6d65  der.build_docume
-00003500: 6e74 2861 7070 6c69 6361 7469 6f6e 290a  nt(application).
-00003510: 6d6f 6475 6c65 203d 204f 7065 6e41 5049  module = OpenAPI
-00003520: 446f 6375 6d65 6e74 4d6f 6475 6c65 2e73  DocumentModule.s
-00003530: 6574 7570 280a 2020 2020 646f 6375 6d65  etup(.    docume
-00003540: 6e74 3d64 6f63 756d 656e 742c 0a20 2020  nt=document,.   
-00003550: 2064 6f63 756d 656e 745f 6765 6e65 7261   document_genera
-00003560: 746f 723d 5377 6167 6765 7244 6f63 756d  tor=SwaggerDocum
-00003570: 656e 7447 656e 6572 6174 6f72 2829 2c0a  entGenerator(),.
-00003580: 2020 2020 6775 6172 6473 3d5b 5d0a 290a      guards=[].).
-00003590: 6170 706c 6963 6174 696f 6e2e 696e 7374  application.inst
-000035a0: 616c 6c5f 6d6f 6475 6c65 286d 6f64 756c  all_module(modul
-000035b0: 6529 0a60 6060 0a0a 4e6f 7720 7765 2063  e).```..Now we c
-000035c0: 616e 2074 6573 7420 6f75 7220 4150 4920  an test our API 
-000035d0: 6174 205b 6874 7470 3a2f 2f31 3237 2e30  at [http://127.0
-000035e0: 2e30 2e31 3a38 3030 302f 646f 6373 5d28  .0.1:8000/docs](
-000035f0: 6874 7470 3a2f 2f31 3237 2e30 2e30 2e31  http://127.0.0.1
-00003600: 3a38 3030 302f 646f 6373 232f 290a 506c  :8000/docs#/).Pl
-00003610: 6561 7365 2065 6e73 7572 6520 796f 7572  ease ensure your
-00003620: 2073 6572 7665 7220 6973 2072 756e 6e69   server is runni
-00003630: 6e67 0a21 5b53 7761 6767 6572 2055 495d  ng.![Swagger UI]
-00003640: 2864 6f63 732f 696d 672f 6361 725f 6170  (docs/img/car_ap
-00003650: 692e 706e 6729 0a0a 2323 2048 544d 4c20  i.png)..## HTML 
-00003660: 5465 6d70 6c61 7469 6e67 0a45 6c6c 6172  Templating.Ellar
-00003670: 2068 6173 2062 7569 6c74 2d69 6e20 7375   has built-in su
-00003680: 7070 6f72 7420 666f 7220 4a69 6e6a 6132  pport for Jinja2
-00003690: 2c20 7768 6963 6820 6973 2061 2070 6f70  , which is a pop
-000036a0: 756c 6172 2074 656d 706c 6174 6520 656e  ular template en
-000036b0: 6769 6e65 2066 6f72 2048 544d 4c2e 2054  gine for HTML. T
-000036c0: 6869 7320 6665 6174 7572 6520 616c 6c6f  his feature allo
-000036d0: 7773 2066 6f72 2065 6173 7920 616e 6420  ws for easy and 
-000036e0: 6566 6669 6369 656e 7420 4854 4d4c 2074  efficient HTML t
-000036f0: 656d 706c 6174 696e 6720 7369 6d69 6c61  emplating simila
-00003700: 7220 746f 2074 6861 7420 6f66 2046 6c61  r to that of Fla
-00003710: 736b 2e20 4a69 6e6a 6132 2063 616e 2062  sk. Jinja2 can b
-00003720: 6520 7573 6564 2074 6f20 6372 6561 7465  e used to create
-00003730: 2072 6575 7361 626c 6520 7465 6d70 6c61   reusable templa
-00003740: 7465 732c 2061 6e64 2074 6f20 696e 7365  tes, and to inse
-00003750: 7274 2064 796e 616d 6963 2064 6174 6120  rt dynamic data 
-00003760: 696e 746f 2048 544d 4c20 7061 6765 732e  into HTML pages.
-00003770: 2049 7420 616c 736f 2068 6173 2073 7570   It also has sup
-00003780: 706f 7274 2066 6f72 2074 656d 706c 6174  port for templat
-00003790: 6520 696e 6865 7269 7461 6e63 652c 2063  e inheritance, c
-000037a0: 6f6e 7472 6f6c 2073 7472 7563 7475 7265  ontrol structure
-000037b0: 732c 2061 6e64 206f 7468 6572 2075 7365  s, and other use
-000037c0: 6675 6c20 6665 6174 7572 6573 2074 6861  ful features tha
-000037d0: 7420 6361 6e20 6865 6c70 2074 6f20 7369  t can help to si
-000037e0: 6d70 6c69 6679 2061 6e64 2073 7472 6561  mplify and strea
-000037f0: 6d6c 696e 6520 7468 6520 7072 6f63 6573  mline the proces
-00003800: 7320 6f66 2063 7265 6174 696e 6720 4854  s of creating HT
-00003810: 4d4c 2074 656d 706c 6174 6573 2e0a 0a60  ML templates...`
-00003820: 6060 6874 6d6c 0a3c 6874 6d6c 3e0a 2020  ``html.<html>.  
-00003830: 3c62 6f64 793e 0a20 2020 203c 756c 3e0a  <body>.    <ul>.
-00003840: 2020 2020 2020 7b25 2066 6f72 2069 7465        {% for ite
-00003850: 6d20 696e 2069 7465 6d73 2025 7d0a 2020  m in items %}.  
-00003860: 2020 2020 3c6c 693e 7b7b 2069 7465 6d20      <li>{{ item 
-00003870: 7d7d 3c2f 6c69 3e0a 2020 2020 2020 7b25  }}</li>.      {%
-00003880: 2065 6e64 666f 7220 257d 0a20 2020 203c   endfor %}.    <
-00003890: 2f75 6c3e 0a20 203c 2f62 6f64 793e 0a3c  /ul>.  </body>.<
-000038a0: 2f68 746d 6c3e 0a60 6060 0a0a 5365 6520  /html>.```..See 
-000038b0: 7468 6520 5b44 6f63 5d28 6874 7470 733a  the [Doc](https:
-000038c0: 2f2f 6561 6477 696e 636f 6465 2e67 6974  //eadwincode.git
-000038d0: 6875 622e 696f 2f65 6c6c 6172 2f74 656d  hub.io/ellar/tem
-000038e0: 706c 6174 696e 672f 7465 6d70 6c61 7469  plating/templati
-000038f0: 6e67 2f29 2066 6f72 206d 6f72 6520 6578  ng/) for more ex
-00003900: 616d 706c 6573 2e0a 0a23 2320 5072 6f6a  amples...## Proj
-00003910: 6563 7420 5374 6174 7573 0a50 726f 6a65  ect Status.Proje
-00003920: 6374 2069 7320 7374 696c 6c20 696e 2064  ct is still in d
-00003930: 6576 656c 6f70 6d65 6e74 0a2d 2044 6f63  evelopment.- Doc
-00003940: 756d 656e 7461 7469 6f6e 202d 2028 696e  umentation - (in
-00003950: 2070 726f 6772 6573 7329 0a2d 2049 6e74   progress).- Int
-00003960: 6572 6365 7074 6f72 7320 202d 2020 5b41  erceptors  -  [A
-00003970: 7370 6563 7420 4f72 6965 6e74 6564 2050  spect Oriented P
-00003980: 726f 6772 616d 6d69 6e67 5d28 6874 7470  rogramming](http
-00003990: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
-000039a0: 2e6f 7267 2f77 696b 692f 4173 7065 6374  .org/wiki/Aspect
-000039b0: 2d6f 7269 656e 7465 645f 7072 6f67 7261  -oriented_progra
-000039c0: 6d6d 696e 6729 2028 414f 5029 2074 6563  mming) (AOP) tec
-000039d0: 686e 6971 7565 0a2d 2044 6174 6162 6173  hnique.- Databas
-000039e0: 6520 506c 7567 696e 2077 6974 6820 5b45  e Plugin with [E
-000039f0: 6e63 6f64 652f 4f52 4d5d 2868 7474 7073  ncode/ORM](https
-00003a00: 3a2f 2f67 6974 6875 622e 636f 6d2f 656e  ://github.com/en
-00003a10: 636f 6465 2f6f 726d 290a 0a              code/orm)..
+00000870: 392c 3c31 302e 302e 3020 3b20 6578 7472  9,<10.0.0 ; extr
+00000880: 6120 3d3d 2022 646f 6322 0a52 6571 7569  a == "doc".Requi
+00000890: 7265 732d 4469 7374 3a20 6d64 782d 696e  res-Dist: mdx-in
+000008a0: 636c 7564 6520 3e3d 312e 342e 312c 3c32  clude >=1.4.1,<2
+000008b0: 2e30 2e30 203b 2065 7874 7261 203d 3d20  .0.0 ; extra == 
+000008c0: 2264 6f63 220a 5265 7175 6972 6573 2d44  "doc".Requires-D
+000008d0: 6973 743a 206d 6b64 6f63 732d 6d61 726b  ist: mkdocs-mark
+000008e0: 646f 776e 6578 7472 6164 6174 612d 706c  downextradata-pl
+000008f0: 7567 696e 203e 3d30 2e31 2e37 2c3c 302e  ugin >=0.1.7,<0.
+00000900: 332e 3020 3b20 6578 7472 6120 3d3d 2022  3.0 ; extra == "
+00000910: 646f 6322 0a52 6571 7569 7265 732d 4469  doc".Requires-Di
+00000920: 7374 3a20 6d61 726b 646f 776e 2d69 6e63  st: markdown-inc
+00000930: 6c75 6465 203b 2065 7874 7261 203d 3d20  lude ; extra == 
+00000940: 2264 6f63 220a 5265 7175 6972 6573 2d44  "doc".Requires-D
+00000950: 6973 743a 206d 6b64 6f63 7374 7269 6e67  ist: mkdocstring
+00000960: 7320 3b20 6578 7472 6120 3d3d 2022 646f  s ; extra == "do
+00000970: 6322 0a52 6571 7569 7265 732d 4469 7374  c".Requires-Dist
+00000980: 3a20 6d6b 646f 6373 2d6d 696e 6966 792d  : mkdocs-minify-
+00000990: 706c 7567 696e 203b 2065 7874 7261 203d  plugin ; extra =
+000009a0: 3d20 2264 6f63 220a 5265 7175 6972 6573  = "doc".Requires
+000009b0: 2d44 6973 743a 206d 6b64 6f63 732d 6769  -Dist: mkdocs-gi
+000009c0: 742d 7265 7669 7369 6f6e 2d64 6174 652d  t-revision-date-
+000009d0: 6c6f 6361 6c69 7a65 642d 706c 7567 696e  localized-plugin
+000009e0: 203b 2065 7874 7261 203d 3d20 2264 6f63   ; extra == "doc
+000009f0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000a00: 2070 7974 6573 7420 3e3d 362e 322e 342c   pytest >=6.2.4,
+00000a10: 3c38 2e30 2e30 203b 2065 7874 7261 203d  <8.0.0 ; extra =
+00000a20: 3d20 2274 6573 7422 0a52 6571 7569 7265  = "test".Require
+00000a30: 732d 4469 7374 3a20 7079 7465 7374 2d63  s-Dist: pytest-c
+00000a40: 6f76 203e 3d32 2e31 322e 302c 3c35 2e30  ov >=2.12.0,<5.0
+00000a50: 2e30 203b 2065 7874 7261 203d 3d20 2274  .0 ; extra == "t
+00000a60: 6573 7422 0a52 6571 7569 7265 732d 4469  est".Requires-Di
+00000a70: 7374 3a20 6d79 7079 203d 3d30 2e39 3731  st: mypy ==0.971
+00000a80: 203b 2065 7874 7261 203d 3d20 2274 6573   ; extra == "tes
+00000a90: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
+00000aa0: 3a20 666c 616b 6538 203e 3d33 2e38 2e33  : flake8 >=3.8.3
+00000ab0: 2c3c 372e 302e 3020 3b20 6578 7472 6120  ,<7.0.0 ; extra 
+00000ac0: 3d3d 2022 7465 7374 220a 5265 7175 6972  == "test".Requir
+00000ad0: 6573 2d44 6973 743a 2062 6c61 636b 203d  es-Dist: black =
+00000ae0: 3d32 322e 3132 2e30 203b 2065 7874 7261  =22.12.0 ; extra
+00000af0: 203d 3d20 2274 6573 7422 0a52 6571 7569   == "test".Requi
+00000b00: 7265 732d 4469 7374 3a20 6973 6f72 7420  res-Dist: isort 
+00000b10: 3e3d 352e 302e 362c 3c36 2e30 2e30 203b  >=5.0.6,<6.0.0 ;
+00000b20: 2065 7874 7261 203d 3d20 2274 6573 7422   extra == "test"
+00000b30: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000b40: 7079 7465 7374 2d61 7379 6e63 696f 203b  pytest-asyncio ;
+00000b50: 2065 7874 7261 203d 3d20 2274 6573 7422   extra == "test"
+00000b60: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000b70: 6461 7461 6261 7365 735b 7371 6c69 7465  databases[sqlite
+00000b80: 5d20 3e3d 2030 2e33 2e32 203b 2065 7874  ] >= 0.3.2 ; ext
+00000b90: 7261 203d 3d20 2274 6573 7422 0a52 6571  ra == "test".Req
+00000ba0: 7569 7265 732d 4469 7374 3a20 6f72 6a73  uires-Dist: orjs
+00000bb0: 6f6e 203e 3d20 332e 322e 3120 3b20 6578  on >= 3.2.1 ; ex
+00000bc0: 7472 6120 3d3d 2022 7465 7374 220a 5265  tra == "test".Re
+00000bd0: 7175 6972 6573 2d44 6973 743a 2075 6a73  quires-Dist: ujs
+00000be0: 6f6e 203e 3d20 342e 302e 3120 3b20 6578  on >= 4.0.1 ; ex
+00000bf0: 7472 6120 3d3d 2022 7465 7374 220a 5265  tra == "test".Re
+00000c00: 7175 6972 6573 2d44 6973 743a 2070 7974  quires-Dist: pyt
+00000c10: 686f 6e2d 6d75 6c74 6970 6172 7420 3e3d  hon-multipart >=
+00000c20: 2030 2e30 2e35 203b 2065 7874 7261 203d   0.0.5 ; extra =
+00000c30: 3d20 2274 6573 7422 0a52 6571 7569 7265  = "test".Require
+00000c40: 732d 4469 7374 3a20 616e 7969 6f5b 7472  s-Dist: anyio[tr
+00000c50: 696f 5d20 3e3d 2033 2e32 2e31 203b 2065  io] >= 3.2.1 ; e
+00000c60: 7874 7261 203d 3d20 2274 6573 7422 0a52  xtra == "test".R
+00000c70: 6571 7569 7265 732d 4469 7374 3a20 6175  equires-Dist: au
+00000c80: 746f 666c 616b 6520 3b20 6578 7472 6120  toflake ; extra 
+00000c90: 3d3d 2022 7465 7374 220a 5265 7175 6972  == "test".Requir
+00000ca0: 6573 2d44 6973 743a 2065 6d61 696c 5f76  es-Dist: email_v
+00000cb0: 616c 6964 6174 6f72 203e 3d31 2e31 2e31  alidator >=1.1.1
+00000cc0: 203b 2065 7874 7261 203d 3d20 2274 6573   ; extra == "tes
+00000cd0: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
+00000ce0: 3a20 7079 6c69 626d 6320 3b20 6578 7472  : pylibmc ; extr
+00000cf0: 6120 3d3d 2022 7465 7374 220a 5265 7175  a == "test".Requ
+00000d00: 6972 6573 2d44 6973 743a 2070 796d 656d  ires-Dist: pymem
+00000d10: 6361 6368 6520 3b20 6578 7472 6120 3d3d  cache ; extra ==
+00000d20: 2022 7465 7374 220a 5265 7175 6972 6573   "test".Requires
+00000d30: 2d44 6973 743a 2061 696f 6d63 6163 6865  -Dist: aiomcache
+00000d40: 203b 2065 7874 7261 203d 3d20 2274 6573   ; extra == "tes
+00000d50: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
+00000d60: 3a20 7265 6469 7320 3b20 6578 7472 6120  : redis ; extra 
+00000d70: 3d3d 2022 7465 7374 220a 5265 7175 6972  == "test".Requir
+00000d80: 6573 2d44 6973 743a 2069 7473 6461 6e67  es-Dist: itsdang
+00000d90: 6572 6f75 7320 3e3d 312e 312e 302c 3c33  erous >=1.1.0,<3
+00000da0: 2e30 2e30 203b 2065 7874 7261 203d 3d20  .0.0 ; extra == 
+00000db0: 2274 6573 7422 0a52 6571 7569 7265 732d  "test".Requires-
+00000dc0: 4469 7374 3a20 7479 7065 732d 756a 736f  Dist: types-ujso
+00000dd0: 6e20 3d3d 352e 372e 302e 3520 3b20 6578  n ==5.7.0.5 ; ex
+00000de0: 7472 6120 3d3d 2022 7465 7374 220a 5265  tra == "test".Re
+00000df0: 7175 6972 6573 2d44 6973 743a 2074 7970  quires-Dist: typ
+00000e00: 6573 2d6f 726a 736f 6e20 3d3d 332e 362e  es-orjson ==3.6.
+00000e10: 3220 3b20 6578 7472 6120 3d3d 2022 7465  2 ; extra == "te
+00000e20: 7374 220a 5265 7175 6972 6573 2d44 6973  st".Requires-Dis
+00000e30: 743a 2074 7970 6573 2d64 6174 6163 6c61  t: types-datacla
+00000e40: 7373 6573 203d 3d30 2e36 2e36 203b 2065  sses ==0.6.6 ; e
+00000e50: 7874 7261 203d 3d20 2274 6573 7422 0a52  xtra == "test".R
+00000e60: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
+00000e70: 7468 6f6e 2d73 6f63 6b65 7469 6f20 3b20  thon-socketio ; 
+00000e80: 6578 7472 6120 3d3d 2022 7465 7374 220a  extra == "test".
+00000e90: 5265 7175 6972 6573 2d44 6973 743a 2075  Requires-Dist: u
+00000ea0: 7669 636f 726e 5b73 7461 6e64 6172 645d  vicorn[standard]
+00000eb0: 203d 3d20 302e 3230 2e30 203b 2065 7874   == 0.20.0 ; ext
+00000ec0: 7261 203d 3d20 2274 6573 7422 0a52 6571  ra == "test".Req
+00000ed0: 7569 7265 732d 4469 7374 3a20 6169 6f68  uires-Dist: aioh
+00000ee0: 7474 7020 3d3d 2033 2e38 2e34 203b 2065  ttp == 3.8.4 ; e
+00000ef0: 7874 7261 203d 3d20 2274 6573 7422 0a50  xtra == "test".P
+00000f00: 726f 6a65 6374 2d55 524c 3a20 446f 6375  roject-URL: Docu
+00000f10: 6d65 6e74 6174 696f 6e2c 2068 7474 7073  mentation, https
+00000f20: 3a2f 2f67 6974 6875 622e 636f 6d2f 6561  ://github.com/ea
+00000f30: 6477 696e 436f 6465 2f65 6c6c 6172 0a50  dwinCode/ellar.P
+00000f40: 726f 6a65 6374 2d55 524c 3a20 486f 6d65  roject-URL: Home
+00000f50: 7061 6765 2c20 6874 7470 733a 2f2f 6561  page, https://ea
+00000f60: 6477 696e 636f 6465 2e67 6974 6875 622e  dwincode.github.
+00000f70: 696f 2f65 6c6c 6172 2f0a 5072 6f6a 6563  io/ellar/.Projec
+00000f80: 742d 5552 4c3a 2053 6f75 7263 652c 2068  t-URL: Source, h
+00000f90: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000fa0: 6d2f 6561 6477 696e 436f 6465 2f65 6c6c  m/eadwinCode/ell
+00000fb0: 6172 0a50 726f 7669 6465 732d 4578 7472  ar.Provides-Extr
+00000fc0: 613a 2061 6c6c 0a50 726f 7669 6465 732d  a: all.Provides-
+00000fd0: 4578 7472 613a 2064 6576 0a50 726f 7669  Extra: dev.Provi
+00000fe0: 6465 732d 4578 7472 613a 2064 6f63 0a50  des-Extra: doc.P
+00000ff0: 726f 7669 6465 732d 4578 7472 613a 2074  rovides-Extra: t
+00001000: 6573 740a 0a3c 7020 616c 6967 6e3d 2263  est..<p align="c
+00001010: 656e 7465 7222 3e0a 2020 3c61 2068 7265  enter">.  <a hre
+00001020: 663d 2223 2220 7461 7267 6574 3d22 626c  f="#" target="bl
+00001030: 616e 6b22 3e3c 696d 6720 7372 633d 2264  ank"><img src="d
+00001040: 6f63 732f 696d 672f 456c 6c61 724c 6f67  ocs/img/EllarLog
+00001050: 6f42 2e70 6e67 2220 7769 6474 683d 2232  oB.png" width="2
+00001060: 3030 2220 616c 743d 2245 6c6c 6172 204c  00" alt="Ellar L
+00001070: 6f67 6f22 202f 3e3c 2f61 3e0a 3c2f 703e  ogo" /></a>.</p>
+00001080: 0a0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
+00001090: 6572 223e 2045 6c6c 6172 202d 2050 7974  er"> Ellar - Pyt
+000010a0: 686f 6e20 4153 4749 2077 6562 2066 7261  hon ASGI web fra
+000010b0: 6d65 776f 726b 2066 6f72 2062 7569 6c64  mework for build
+000010c0: 696e 6720 6661 7374 2c20 6566 6669 6369  ing fast, effici
+000010d0: 656e 7420 616e 6420 7363 616c 6162 6c65  ent and scalable
+000010e0: 2052 4553 5441 5049 7320 616e 6420 7365   RESTAPIs and se
+000010f0: 7276 6572 2d73 6964 6520 6170 706c 6963  rver-side applic
+00001100: 6174 696f 6e2e 203c 2f70 3e0a 0a21 5b54  ation. </p>..![T
+00001110: 6573 745d 2868 7474 7073 3a2f 2f67 6974  est](https://git
+00001120: 6875 622e 636f 6d2f 6561 6477 696e 436f  hub.com/eadwinCo
+00001130: 6465 2f65 6c6c 6172 2f61 6374 696f 6e73  de/ellar/actions
+00001140: 2f77 6f72 6b66 6c6f 7773 2f74 6573 745f  /workflows/test_
+00001150: 6675 6c6c 2e79 6d6c 2f62 6164 6765 2e73  full.yml/badge.s
+00001160: 7667 290a 215b 436f 7665 7261 6765 5d28  vg).![Coverage](
+00001170: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00001180: 6c64 732e 696f 2f63 6f64 6563 6f76 2f63  lds.io/codecov/c
+00001190: 2f67 6974 6875 622f 6561 6477 696e 436f  /github/eadwinCo
+000011a0: 6465 2f65 6c6c 6172 290a 5b21 5b50 7950  de/ellar).[![PyP
+000011b0: 4920 7665 7273 696f 6e5d 2868 7474 7073  I version](https
+000011c0: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
+000011d0: 2f70 792f 656c 6c61 722e 7376 6729 5d28  /py/ellar.svg)](
+000011e0: 6874 7470 733a 2f2f 6261 6467 652e 6675  https://badge.fu
+000011f0: 7279 2e69 6f2f 7079 2f65 6c6c 6172 290a  ry.io/py/ellar).
+00001200: 5b21 5b50 7950 4920 7665 7273 696f 6e5d  [![PyPI version]
+00001210: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00001220: 656c 6473 2e69 6f2f 7079 7069 2f76 2f65  elds.io/pypi/v/e
+00001230: 6c6c 6172 2e73 7667 295d 2868 7474 7073  llar.svg)](https
+00001240: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
+00001250: 7267 2f70 7970 692f 656c 6c61 7229 0a5b  rg/pypi/ellar).[
+00001260: 215b 5079 5049 2076 6572 7369 6f6e 5d28  ![PyPI version](
+00001270: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00001280: 6c64 732e 696f 2f70 7970 692f 7079 7665  lds.io/pypi/pyve
+00001290: 7273 696f 6e73 2f65 6c6c 6172 2e73 7667  rsions/ellar.svg
+000012a0: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
+000012b0: 7079 7468 6f6e 2e6f 7267 2f70 7970 692f  python.org/pypi/
+000012c0: 656c 6c61 7229 0a0a 2323 202a 2a49 6e74  ellar)..## **Int
+000012d0: 726f 6475 6374 696f 6e2a 2a0a 0a45 6c6c  roduction**..Ell
+000012e0: 6172 2069 7320 6120 6c69 6768 7477 6569  ar is a lightwei
+000012f0: 6768 7420 4153 4749 2066 7261 6d65 776f  ght ASGI framewo
+00001300: 726b 2066 6f72 2062 7569 6c64 696e 6720  rk for building 
+00001310: 6566 6669 6369 656e 7420 616e 6420 7363  efficient and sc
+00001320: 616c 6162 6c65 2073 6572 7665 722d 7369  alable server-si
+00001330: 6465 2070 7974 686f 6e20 6170 706c 6963  de python applic
+00001340: 6174 696f 6e73 2e0a 4974 2073 7570 706f  ations..It suppo
+00001350: 7274 7320 626f 7468 204f 4f50 2028 4f62  rts both OOP (Ob
+00001360: 6a65 6374 2d4f 7269 656e 7465 6420 5072  ject-Oriented Pr
+00001370: 6f67 7261 6d6d 696e 6729 2061 6e64 2046  ogramming) and F
+00001380: 5020 2846 756e 6374 696f 6e61 6c20 5072  P (Functional Pr
+00001390: 6f67 7261 6d6d 696e 6729 0a0a 456c 6c61  ogramming)..Ella
+000013a0: 7220 6973 2062 6173 6564 206f 6e20 5b53  r is based on [S
+000013b0: 7461 726c 6574 7465 2028 4153 4749 2074  tarlette (ASGI t
+000013c0: 6f6f 6c6b 6974 295d 2868 7474 7073 3a2f  oolkit)](https:/
+000013d0: 2f77 7777 2e73 7461 726c 6574 7465 2e69  /www.starlette.i
+000013e0: 6f2f 292c 2061 206c 6967 6874 7765 6967  o/), a lightweig
+000013f0: 6874 2041 5347 4920 6672 616d 6577 6f72  ht ASGI framewor
+00001400: 6b2f 746f 6f6c 6b69 7420 7765 6c6c 2d73  k/toolkit well-s
+00001410: 7569 7465 6420 666f 7220 6465 7665 6c6f  uited for develo
+00001420: 7069 6e67 2061 7379 6e63 6872 6f6e 6f75  ping asynchronou
+00001430: 7320 7765 6220 7365 7276 6963 6573 2077  s web services w
+00001440: 6974 6820 5079 7468 6f6e 2e20 0a0a 2323  ith Python. ..##
+00001450: 202a 2a46 6561 7475 7265 7320 5375 6d6d   **Features Summ
+00001460: 6172 792a 2a0a 0a2d 202a 2a45 6173 7920  ary**..- **Easy 
+00001470: 746f 2055 7365 2a2a 3a20 456c 6c61 7220  to Use**: Ellar 
+00001480: 6861 7320 6120 7369 6d70 6c65 2061 6e64  has a simple and
+00001490: 2069 6e74 7569 7469 7665 2041 5049 2074   intuitive API t
+000014a0: 6861 7420 6d61 6b65 7320 6974 2065 6173  hat makes it eas
+000014b0: 7920 746f 2067 6574 2073 7461 7274 6564  y to get started
+000014c0: 2077 6974 6820 6275 696c 6469 6e67 2061   with building a
+000014d0: 2066 6173 7420 616e 6420 7363 616c 6162   fast and scalab
+000014e0: 6c65 2077 6562 2061 7070 6c69 6361 7469  le web applicati
+000014f0: 6f6e 7320 6f72 2077 6562 2041 5049 7320  ons or web APIs 
+00001500: 696e 2050 7974 686f 6e2e 0a2d 202a 2a44  in Python..- **D
+00001510: 6570 656e 6465 6e63 7920 496e 6a65 6374  ependency Inject
+00001520: 696f 6e20 2844 4929 2a2a 3a20 4974 2063  ion (DI)**: It c
+00001530: 6f6d 6573 2077 6974 6820 4449 2073 7973  omes with DI sys
+00001540: 7465 6d20 6d61 6b65 7320 6974 2065 6173  tem makes it eas
+00001550: 7920 746f 206d 616e 6167 6520 6465 7065  y to manage depe
+00001560: 6e64 656e 6369 6573 2061 6e64 2072 6564  ndencies and red
+00001570: 7563 6520 636f 7570 6c69 6e67 2062 6574  uce coupling bet
+00001580: 7765 656e 2063 6f6d 706f 6e65 6e74 732e  ween components.
+00001590: 0a2d 202a 2a50 7964 616e 7469 6320 496e  .- **Pydantic In
+000015a0: 7465 6772 6174 696f 6e2a 2a3a 2049 7420  tegration**: It 
+000015b0: 6973 2070 726f 7065 726c 7920 696e 7465  is properly inte
+000015c0: 6772 6174 6564 2077 6974 6820 5079 6461  grated with Pyda
+000015d0: 6e74 6963 2c20 6120 706f 7075 6c61 7220  ntic, a popular 
+000015e0: 5079 7468 6f6e 206c 6962 7261 7279 2066  Python library f
+000015f0: 6f72 2064 6174 6120 7661 6c69 6461 7469  or data validati
+00001600: 6f6e 2c20 746f 2065 6e73 7572 6520 7468  on, to ensure th
+00001610: 6174 2069 6e70 7574 2064 6174 6120 6973  at input data is
+00001620: 2076 616c 6964 2e0a 2d20 2a2a 5465 6d70   valid..- **Temp
+00001630: 6c61 7469 6e67 2077 6974 6820 4a69 6e6a  lating with Jinj
+00001640: 6132 2a2a 3a20 456c 6c61 7220 7072 6f76  a2**: Ellar prov
+00001650: 6964 6573 2062 7569 6c74 2d69 6e20 7375  ides built-in su
+00001660: 7070 6f72 7420 666f 7220 4a69 6e6a 6132  pport for Jinja2
+00001670: 2074 656d 706c 6174 6573 2c20 6d61 6b69   templates, maki
+00001680: 6e67 2069 7420 6561 7379 2074 6f20 6372  ng it easy to cr
+00001690: 6561 7465 2064 796e 616d 6963 2077 6562  eate dynamic web
+000016a0: 2070 6167 6573 2e0a 2d20 2a2a 4f70 656e   pages..- **Open
+000016b0: 4150 4920 446f 6375 6d65 6e74 6174 696f  API Documentatio
+000016c0: 6e2a 2a3a 2049 7420 636f 6d65 7320 7769  n**: It comes wi
+000016d0: 7468 2062 7569 6c74 2d69 6e20 7375 7070  th built-in supp
+000016e0: 6f72 7420 666f 7220 4f70 656e 4150 4920  ort for OpenAPI 
+000016f0: 646f 6375 6d65 6e74 6174 696f 6e2c 206d  documentation, m
+00001700: 616b 696e 6720 6974 2065 6173 7920 746f  aking it easy to
+00001710: 2067 656e 6572 6174 6520 6053 7761 6767   generate `Swagg
+00001720: 6572 6020 6f72 2060 5265 446f 6360 2064  er` or `ReDoc` d
+00001730: 6f63 756d 656e 7461 7469 6f6e 2066 6f72  ocumentation for
+00001740: 2079 6f75 7220 4150 492e 2041 6e64 206d   your API. And m
+00001750: 6f72 6520 6361 6e20 6265 2061 6464 6564  ore can be added
+00001760: 2077 6974 6820 6561 7365 2069 6620 6e65   with ease if ne
+00001770: 6365 7373 6172 792e 0a2d 202a 2a43 6f6e  cessary..- **Con
+00001780: 7472 6f6c 6c65 7220 284d 5643 2920 4172  troller (MVC) Ar
+00001790: 6368 6974 6563 7475 7265 2a2a 3a20 456c  chitecture**: El
+000017a0: 6c61 7227 7320 636f 6e74 726f 6c6c 6572  lar's controller
+000017b0: 2061 7263 6869 7465 6374 7572 6520 666f   architecture fo
+000017c0: 6c6c 6f77 7320 7468 6520 4d6f 6465 6c2d  llows the Model-
+000017d0: 5669 6577 2d43 6f6e 7472 6f6c 6c65 7220  View-Controller 
+000017e0: 284d 5643 2920 7061 7474 6572 6e2c 206d  (MVC) pattern, m
+000017f0: 616b 696e 6720 6974 2065 6173 7920 746f  aking it easy to
+00001800: 206f 7267 616e 697a 6520 796f 7572 2063   organize your c
+00001810: 6f64 652e 0a2d 202a 2a47 7561 7264 7320  ode..- **Guards 
+00001820: 666f 7220 4175 7468 656e 7469 6361 7469  for Authenticati
+00001830: 6f6e 2061 6e64 2041 7574 686f 7269 7a61  on and Authoriza
+00001840: 7469 6f6e 2a2a 3a20 4974 2070 726f 7669  tion**: It provi
+00001850: 6465 7320 6275 696c 742d 696e 2073 7570  des built-in sup
+00001860: 706f 7274 2066 6f72 2067 7561 7264 732c  port for guards,
+00001870: 2061 6c6c 6f77 696e 6720 796f 7520 746f   allowing you to
+00001880: 2065 6173 696c 7920 696d 706c 656d 656e   easily implemen
+00001890: 7420 6175 7468 656e 7469 6361 7469 6f6e  t authentication
+000018a0: 2061 6e64 2061 7574 686f 7269 7a61 7469   and authorizati
+000018b0: 6f6e 2069 6e20 796f 7572 2061 7070 6c69  on in your appli
+000018c0: 6361 7469 6f6e 2e0a 2d20 2a2a 4d6f 6475  cation..- **Modu
+000018d0: 6c61 7269 7479 2a2a 3a20 456c 6c61 7220  larity**: Ellar 
+000018e0: 666f 6c6c 6f77 7320 6120 6d6f 6475 6c61  follows a modula
+000018f0: 7220 6172 6368 6974 6563 7475 7265 2069  r architecture i
+00001900: 6e73 7069 7265 6420 6279 204e 6573 744a  nspired by NestJ
+00001910: 532c 206d 616b 696e 6720 6974 2065 6173  S, making it eas
+00001920: 7920 746f 206f 7267 616e 697a 6520 796f  y to organize yo
+00001930: 7572 2063 6f64 6520 696e 746f 2072 6575  ur code into reu
+00001940: 7361 626c 6520 6d6f 6475 6c65 732e 0a2d  sable modules..-
+00001950: 202a 2a41 7379 6e63 6872 6f6e 6f75 7320   **Asynchronous 
+00001960: 7072 6f67 7261 6d6d 696e 672a 2a3a 2049  programming**: I
+00001970: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
+00001980: 7461 6b65 7320 6164 7661 6e74 6167 6520  takes advantage 
+00001990: 6f66 2050 7974 686f 6e27 7320 6061 7379  of Python's `asy
+000019a0: 6e63 2f61 7761 6974 6020 6665 6174 7572  nc/await` featur
+000019b0: 6520 746f 2077 7269 7465 2065 6666 6963  e to write effic
+000019c0: 6965 6e74 2061 6e64 2066 6173 7420 636f  ient and fast co
+000019d0: 6465 2074 6861 7420 6361 6e20 6861 6e64  de that can hand
+000019e0: 6c65 206c 6172 6765 206e 756d 6265 7273  le large numbers
+000019f0: 206f 6620 636f 6e63 7572 7265 6e74 2072   of concurrent r
+00001a00: 6571 7565 7374 730a 0a23 2320 2a2a 4465  equests..## **De
+00001a10: 7065 6e64 656e 6369 6573 2a2a 0a2d 2050  pendencies**.- P
+00001a20: 7974 686f 6e20 3e3d 2033 2e37 0a2d 2053  ython >= 3.7.- S
+00001a30: 7461 726c 6574 7465 0a2d 2049 6e6a 6563  tarlette.- Injec
+00001a40: 746f 720a 2d20 5079 6461 6e74 6963 0a0a  tor.- Pydantic..
+00001a50: 2323 202a 2a49 6e73 7461 6c6c 6174 696f  ## **Installatio
+00001a60: 6e2a 2a0a 2323 2320 506f 6574 7279 2049  n**.### Poetry I
+00001a70: 6e73 7461 6c6c 6174 696f 6e0a 466f 7220  nstallation.For 
+00001a80: 5b50 6f65 7472 795d 2868 7474 7073 3a2f  [Poetry](https:/
+00001a90: 2f70 7974 686f 6e2d 706f 6574 7279 2e6f  /python-poetry.o
+00001aa0: 7267 2f29 2075 7361 6765 730a 0a60 6060  rg/) usages..```
+00001ab0: 7368 656c 6c0a 706f 6574 7279 2061 6464  shell.poetry add
+00001ac0: 2065 6c6c 6172 2d63 6c69 0a60 6060 0a0a   ellar-cli.```..
+00001ad0: 2323 2320 5069 7020 496e 7374 616c 6c61  ### Pip Installa
+00001ae0: 7469 6f6e 0a46 6f72 206e 6f72 6d61 6c20  tion.For normal 
+00001af0: 7069 7020 696e 7374 616c 6c61 7469 6f6e  pip installation
+00001b00: 0a60 6060 7368 656c 6c0a 7069 7020 696e  .```shell.pip in
+00001b10: 7374 616c 6c20 656c 6c61 722d 636c 690a  stall ellar-cli.
+00001b20: 6060 600a 0a23 2320 4372 6561 7469 6e67  ```..## Creating
+00001b30: 2061 2070 726f 6a65 6374 0a54 6f20 6372   a project.To cr
+00001b40: 6561 7465 2061 6e20 656c 6c61 7220 7072  eate an ellar pr
+00001b50: 6f6a 6563 742c 2079 6f75 206e 6565 6420  oject, you need 
+00001b60: 746f 2068 6176 6520 6120 6070 7970 726f  to have a `pypro
+00001b70: 6a65 6374 2e74 6f6d 6c60 2061 7661 696c  ject.toml` avail
+00001b80: 6162 6c65 206f 6e20 796f 7572 2072 6f6f  able on your roo
+00001b90: 7420 6469 7265 6374 6f72 792e 0a54 6869  t directory..Thi
+00001ba0: 7320 6973 206e 6563 6573 7361 7279 2066  s is necessary f
+00001bb0: 6f72 2065 6c6c 6172 2074 6f20 7374 6f72  or ellar to stor
+00001bc0: 6520 736f 6d65 2060 6d65 7461 6461 7461  e some `metadata
+00001bd0: 6020 6162 6f75 7420 796f 7572 2070 726f  ` about your pro
+00001be0: 6a65 6374 2e20 0a0a 466f 7220 5069 7020  ject. ..For Pip 
+00001bf0: 5573 6572 732c 2079 6f75 206e 6565 6420  Users, you need 
+00001c00: 746f 2063 7265 6174 6520 6070 7970 726f  to create `pypro
+00001c10: 6a65 6374 2e74 6f6d 6c60 2066 696c 650a  ject.toml` file.
+00001c20: 6060 6073 6865 6c6c 0a65 6c6c 6172 206e  ```shell.ellar n
+00001c30: 6577 2063 6172 7369 7465 0a60 6060 0a49  ew carsite.```.I
+00001c40: 6620 796f 7520 6172 6520 7573 696e 6720  f you are using 
+00001c50: 6050 6f65 7472 7960 2c20 6174 2079 6f75  `Poetry`, at you
+00001c60: 7220 7072 6f6a 6563 7420 726f 6f74 2064  r project root d
+00001c70: 6972 6563 746f 7279 2077 6974 6820 6070  irectory with `p
+00001c80: 7970 726f 6a65 6374 2e74 6f6d 6c60 2c0a  yproject.toml`,.
+00001c90: 7275 6e20 7468 6520 656c 6c61 7220 6372  run the ellar cr
+00001ca0: 6561 7465 2070 726f 6a65 6374 2063 6c69  eate project cli
+00001cb0: 2063 6f6d 6d61 6e64 2c0a 6060 6073 6865   command,.```she
+00001cc0: 6c6c 0a65 6c6c 6172 2063 7265 6174 652d  ll.ellar create-
+00001cd0: 7072 6f6a 6563 7420 6361 7273 6974 650a  project carsite.
+00001ce0: 6060 600a 0a23 2320 2a2a 5275 6e20 796f  ```..## **Run yo
+00001cf0: 7572 2070 726f 6a65 6374 2a2a 0a45 6c6c  ur project**.Ell
+00001d00: 6172 2072 756e 7320 5b55 5649 434f 524e  ar runs [UVICORN
+00001d10: 202d 2041 5347 4920 5365 7276 6572 5d28   - ASGI Server](
+00001d20: 6874 7470 733a 2f2f 7777 772e 7576 6963  https://www.uvic
+00001d30: 6f72 6e2e 6f72 672f 2920 756e 6465 7220  orn.org/) under 
+00001d40: 7468 6520 686f 6f64 2e0a 6060 6073 6865  the hood..```she
+00001d50: 6c6c 0a65 6c6c 6172 2072 756e 7365 7276  ll.ellar runserv
+00001d60: 6572 202d 2d72 656c 6f61 640a 6060 600a  er --reload.```.
+00001d70: 602d 2d72 656c 6f61 6460 2069 7320 746f  `--reload` is to
+00001d80: 2077 6174 6368 2066 6f72 2066 696c 6520   watch for file 
+00001d90: 6368 616e 6765 730a 0a4e 6f77 2067 6f20  changes..Now go 
+00001da0: 746f 205b 6874 7470 3a2f 2f31 3237 2e30  to [http://127.0
+00001db0: 2e30 2e31 3a38 3030 305d 2868 7474 703a  .0.1:8000](http:
+00001dc0: 2f2f 3132 372e 302e 302e 313a 3830 3030  //127.0.0.1:8000
+00001dd0: 290a 215b 5377 6167 6765 7220 5549 5d28  ).![Swagger UI](
+00001de0: 646f 6373 2f69 6d67 2f65 6c6c 6172 5f66  docs/img/ellar_f
+00001df0: 7261 6d65 776f 726b 2e70 6e67 290a 0a46  ramework.png)..F
+00001e00: 6f72 206d 6f72 6520 696e 666f 206f 6e20  or more info on 
+00001e10: 456c 6c61 7220 434c 492c 2063 6c69 636b  Ellar CLI, click
+00001e20: 205b 6865 7265 5d28 6874 7470 733a 2f2f   [here](https://
+00001e30: 6769 7468 7562 2e63 6f6d 2f65 6164 7769  github.com/eadwi
+00001e40: 6e43 6f64 652f 656c 6c61 722d 636c 6929  nCode/ellar-cli)
+00001e50: 0a0a 2323 202a 2a41 6464 696e 6720 6120  ..## **Adding a 
+00001e60: 7072 6f6a 6563 7420 6d6f 6475 6c65 2a2a  project module**
+00001e70: 0a41 2070 726f 6a65 6374 206d 6f64 756c  .A project modul
+00001e80: 6520 6973 2061 2070 726f 6a65 6374 2061  e is a project a
+00001e90: 7070 2064 6566 696e 696e 6720 6120 6772  pp defining a gr
+00001ea0: 6f75 7020 6f66 2063 6f6e 7472 6f6c 6c65  oup of controlle
+00001eb0: 7273 206f 7220 7365 7276 6963 6573 2069  rs or services i
+00001ec0: 6e63 6c75 6469 6e67 2074 656d 706c 6174  ncluding templat
+00001ed0: 6573 2061 6e64 2073 7461 7469 6320 6669  es and static fi
+00001ee0: 6c65 732e 0a53 6f2c 206e 6f77 2077 6520  les..So, now we 
+00001ef0: 6861 7665 2061 2070 726f 6a65 6374 2063  have a project c
+00001f00: 7265 6174 6564 2c20 6c65 7473 2061 6464  reated, lets add
+00001f10: 2061 6e20 6170 7020 746f 2074 6865 2070   an app to the p
+00001f20: 726f 6a65 6374 2e0a 6060 6073 6865 6c6c  roject..```shell
+00001f30: 0a65 6c6c 6172 2063 7265 6174 652d 6d6f  .ellar create-mo
+00001f40: 6475 6c65 2063 6172 0a60 6060 0a0a 2323  dule car.```..##
+00001f50: 202a 2a41 6464 2053 6368 656d 612a 2a0a   **Add Schema**.
+00001f60: 496e 2060 6361 722f 7363 6865 6d61 2e70  In `car/schema.p
+00001f70: 7960 2c20 6c65 7473 2061 6464 2073 6f6d  y`, lets add som
+00001f80: 6520 7365 7269 616c 697a 6572 2066 6f72  e serializer for
+00001f90: 2063 6172 2069 6e70 7574 2061 6e64 206f   car input and o
+00001fa0: 7574 7075 7420 6461 7461 0a60 6060 7079  utput data.```py
+00001fb0: 7468 6f6e 0a66 726f 6d20 656c 6c61 722e  thon.from ellar.
+00001fc0: 636f 6d6d 6f6e 2069 6d70 6f72 7420 5365  common import Se
+00001fd0: 7269 616c 697a 6572 0a0a 636c 6173 7320  rializer..class 
+00001fe0: 4361 7253 6572 6961 6c69 7a65 7228 5365  CarSerializer(Se
+00001ff0: 7269 616c 697a 6572 293a 0a20 2020 206e  rializer):.    n
+00002000: 616d 653a 2073 7472 0a20 2020 206d 6f64  ame: str.    mod
+00002010: 656c 3a20 7374 720a 2020 2020 6272 616e  el: str.    bran
+00002020: 643a 2073 7472 0a0a 0a63 6c61 7373 2052  d: str...class R
+00002030: 6574 7269 6576 6543 6172 5365 7269 616c  etrieveCarSerial
+00002040: 697a 6572 2843 6172 5365 7269 616c 697a  izer(CarSerializ
+00002050: 6572 293a 0a20 2020 2070 6b3a 2073 7472  er):.    pk: str
+00002060: 0a60 6060 0a0a 2323 202a 2a41 6464 2053  .```..## **Add S
+00002070: 6572 7669 6365 732a 2a0a 496e 2060 6361  ervices**.In `ca
+00002080: 722f 7365 7276 6963 6573 2e70 7960 2c20  r/services.py`, 
+00002090: 6c65 7473 2063 7265 6174 6520 6120 6475  lets create a du
+000020a0: 6d6d 7920 7265 706f 7369 746f 7279 2060  mmy repository `
+000020b0: 4361 7244 756d 6d79 4442 6020 746f 206d  CarDummyDB` to m
+000020c0: 616e 6167 6520 6f75 7220 6361 7220 6461  anage our car da
+000020d0: 7461 2e0a 6060 6070 7974 686f 6e0a 696d  ta..```python.im
+000020e0: 706f 7274 2074 7970 696e 6720 6173 2074  port typing as t
+000020f0: 0a69 6d70 6f72 7420 7575 6964 0a66 726f  .import uuid.fro
+00002100: 6d20 656c 6c61 722e 6469 2069 6d70 6f72  m ellar.di impor
+00002110: 7420 696e 6a65 6374 6162 6c65 2c20 7369  t injectable, si
+00002120: 6e67 6c65 746f 6e5f 7363 6f70 650a 0a0a  ngleton_scope...
+00002130: 4069 6e6a 6563 7461 626c 6528 7363 6f70  @injectable(scop
+00002140: 653d 7369 6e67 6c65 746f 6e5f 7363 6f70  e=singleton_scop
+00002150: 6529 0a63 6c61 7373 2043 6172 4475 6d6d  e).class CarDumm
+00002160: 7944 423a 0a20 2020 2063 6c61 7373 2043  yDB:.    class C
+00002170: 6172 4475 6d6d 7944 4249 7465 6d3a 0a20  arDummyDBItem:. 
+00002180: 2020 2020 2020 2070 6b3a 2073 7472 0a0a         pk: str..
+00002190: 2020 2020 2020 2020 6465 6620 5f5f 696e          def __in
+000021a0: 6974 5f5f 2873 656c 662c 202a 2a64 6174  it__(self, **dat
+000021b0: 613a 2074 2e44 6963 7429 202d 3e20 4e6f  a: t.Dict) -> No
+000021c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000021d0: 7365 6c66 2e5f 5f64 6963 745f 5f20 3d20  self.__dict__ = 
+000021e0: 6461 7461 0a0a 2020 2020 2020 2020 6465  data..        de
+000021f0: 6620 5f5f 6571 5f5f 2873 656c 662c 206f  f __eq__(self, o
+00002200: 7468 6572 293a 0a20 2020 2020 2020 2020  ther):.         
+00002210: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00002220: 286f 7468 6572 2c20 4361 7244 756d 6d79  (other, CarDummy
+00002230: 4442 2e43 6172 4475 6d6d 7944 4249 7465  DB.CarDummyDBIte
+00002240: 6d29 3a0a 2020 2020 2020 2020 2020 2020  m):.            
+00002250: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00002260: 706b 203d 3d20 6f74 6865 722e 706b 0a20  pk == other.pk. 
+00002270: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00002280: 6e20 7365 6c66 2e70 6b20 3d3d 2073 7472  n self.pk == str
+00002290: 286f 7468 6572 290a 0a20 2020 2064 6566  (other)..    def
+000022a0: 205f 5f69 6e69 745f 5f28 7365 6c66 2920   __init__(self) 
+000022b0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+000022c0: 2073 656c 662e 5f64 6174 613a 2074 2e4c   self._data: t.L
+000022d0: 6973 745b 4361 7244 756d 6d79 4442 2e43  ist[CarDummyDB.C
+000022e0: 6172 4475 6d6d 7944 4249 7465 6d5d 203d  arDummyDBItem] =
+000022f0: 205b 5d0a 0a20 2020 2064 6566 2061 6464   []..    def add
+00002300: 5f63 6172 2873 656c 662c 2064 6174 613a  _car(self, data:
+00002310: 2074 2e44 6963 7429 202d 3e20 7374 723a   t.Dict) -> str:
+00002320: 0a20 2020 2020 2020 2070 6b20 3d20 7575  .        pk = uu
+00002330: 6964 2e75 7569 6434 2829 0a20 2020 2020  id.uuid4().     
+00002340: 2020 205f 6461 7461 203d 2064 6963 7428     _data = dict(
+00002350: 6461 7461 290a 2020 2020 2020 2020 5f64  data).        _d
+00002360: 6174 612e 7570 6461 7465 2870 6b3d 7374  ata.update(pk=st
+00002370: 7228 706b 2929 0a20 2020 2020 2020 2069  r(pk)).        i
+00002380: 7465 6d20 3d20 7365 6c66 2e43 6172 4475  tem = self.CarDu
+00002390: 6d6d 7944 4249 7465 6d28 2a2a 5f64 6174  mmyDBItem(**_dat
+000023a0: 6129 0a20 2020 2020 2020 2073 656c 662e  a).        self.
+000023b0: 5f64 6174 612e 6170 7065 6e64 2869 7465  _data.append(ite
+000023c0: 6d29 0a20 2020 2020 2020 2072 6574 7572  m).        retur
+000023d0: 6e20 6974 656d 2e70 6b0a 0a20 2020 2064  n item.pk..    d
+000023e0: 6566 206c 6973 7428 7365 6c66 2920 2d3e  ef list(self) ->
+000023f0: 2074 2e4c 6973 745b 2243 6172 4475 6d6d   t.List["CarDumm
+00002400: 7944 422e 4361 7244 756d 6d79 4442 4974  yDB.CarDummyDBIt
+00002410: 656d 225d 3a0a 2020 2020 2020 2020 7265  em"]:.        re
+00002420: 7475 726e 2073 656c 662e 5f64 6174 610a  turn self._data.
+00002430: 0a20 2020 2064 6566 2075 7064 6174 6528  .    def update(
+00002440: 7365 6c66 2c20 6361 725f 6964 3a20 7374  self, car_id: st
+00002450: 722c 2064 6174 613a 2074 2e44 6963 7429  r, data: t.Dict)
+00002460: 202d 3e20 742e 4f70 7469 6f6e 616c 5b22   -> t.Optional["
+00002470: 4361 7244 756d 6d79 4442 2e43 6172 4475  CarDummyDB.CarDu
+00002480: 6d6d 7944 4249 7465 6d22 5d3a 0a20 2020  mmyDBItem"]:.   
+00002490: 2020 2020 2069 6478 203d 2073 656c 662e       idx = self.
+000024a0: 5f64 6174 612e 696e 6465 7828 6361 725f  _data.index(car_
+000024b0: 6964 290a 2020 2020 2020 2020 6966 2069  id).        if i
+000024c0: 6478 203e 3d20 303a 0a20 2020 2020 2020  dx >= 0:.       
+000024d0: 2020 2020 205f 6461 7461 203d 2064 6963       _data = dic
+000024e0: 7428 6461 7461 290a 2020 2020 2020 2020  t(data).        
+000024f0: 2020 2020 5f64 6174 612e 7570 6461 7465      _data.update
+00002500: 2870 6b3d 7374 7228 6361 725f 6964 2929  (pk=str(car_id))
+00002510: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00002520: 662e 5f64 6174 615b 6964 785d 203d 2073  f._data[idx] = s
+00002530: 656c 662e 4361 7244 756d 6d79 4442 4974  elf.CarDummyDBIt
+00002540: 656d 282a 2a5f 6461 7461 290a 2020 2020  em(**_data).    
+00002550: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00002560: 656c 662e 5f64 6174 615b 6964 785d 0a0a  elf._data[idx]..
+00002570: 2020 2020 6465 6620 6765 7428 7365 6c66      def get(self
+00002580: 2c20 6361 725f 6964 3a20 7374 7229 202d  , car_id: str) -
+00002590: 3e20 742e 4f70 7469 6f6e 616c 5b22 4361  > t.Optional["Ca
+000025a0: 7244 756d 6d79 4442 2e43 6172 4475 6d6d  rDummyDB.CarDumm
+000025b0: 7944 4249 7465 6d22 5d3a 0a20 2020 2020  yDBItem"]:.     
+000025c0: 2020 2069 6478 203d 2073 656c 662e 5f64     idx = self._d
+000025d0: 6174 612e 696e 6465 7828 6361 725f 6964  ata.index(car_id
+000025e0: 290a 2020 2020 2020 2020 6966 2069 6478  ).        if idx
+000025f0: 203e 3d20 303a 0a20 2020 2020 2020 2020   >= 0:.         
+00002600: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00002610: 6461 7461 5b69 6478 5d0a 0a20 2020 2064  data[idx]..    d
+00002620: 6566 2072 656d 6f76 6528 7365 6c66 2c20  ef remove(self, 
+00002630: 6361 725f 6964 3a20 7374 7229 202d 3e20  car_id: str) -> 
+00002640: 742e 4f70 7469 6f6e 616c 5b22 4361 7244  t.Optional["CarD
+00002650: 756d 6d79 4442 2e43 6172 4475 6d6d 7944  ummyDB.CarDummyD
+00002660: 4249 7465 6d22 5d3a 0a20 2020 2020 2020  BItem"]:.       
+00002670: 2069 6478 203d 2073 656c 662e 5f64 6174   idx = self._dat
+00002680: 612e 696e 6465 7828 6361 725f 6964 290a  a.index(car_id).
+00002690: 2020 2020 2020 2020 6966 2069 6478 203e          if idx >
+000026a0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+000026b0: 2072 6574 7572 6e20 7365 6c66 2e5f 6461   return self._da
+000026c0: 7461 2e70 6f70 2869 6478 290a 6060 600a  ta.pop(idx).```.
+000026d0: 2323 202a 2a41 6464 2043 6f6e 7472 6f6c  ## **Add Control
+000026e0: 6c65 722a 2a0a 496e 2060 6361 722f 636f  ler**.In `car/co
+000026f0: 6e74 726f 6c6c 6572 732e 7079 602c 206c  ntrollers.py`, l
+00002700: 6574 7320 6372 6561 7465 2060 4361 7243  ets create `CarC
+00002710: 6f6e 7472 6f6c 6c65 7260 0a0a 6060 6070  ontroller`..```p
+00002720: 7974 686f 6e0a 696d 706f 7274 2074 7970  ython.import typ
+00002730: 696e 6720 6173 2074 0a66 726f 6d20 656c  ing as t.from el
+00002740: 6c61 722e 636f 6d6d 6f6e 2069 6d70 6f72  lar.common impor
+00002750: 7420 436f 6e74 726f 6c6c 6572 2c20 6465  t Controller, de
+00002760: 6c65 7465 2c20 6765 742c 2070 7574 2c20  lete, get, put, 
+00002770: 706f 7374 2c20 436f 6e74 726f 6c6c 6572  post, Controller
+00002780: 4261 7365 0a66 726f 6d20 656c 6c61 722e  Base.from ellar.
+00002790: 636f 6d6d 6f6e 2e65 7863 6570 7469 6f6e  common.exception
+000027a0: 7320 696d 706f 7274 204e 6f74 466f 756e  s import NotFoun
+000027b0: 640a 6672 6f6d 202e 7363 6865 6d61 7320  d.from .schemas 
+000027c0: 696d 706f 7274 2043 6172 5365 7269 616c  import CarSerial
+000027d0: 697a 6572 2c20 5265 7472 6965 7665 4361  izer, RetrieveCa
+000027e0: 7253 6572 6961 6c69 7a65 720a 6672 6f6d  rSerializer.from
+000027f0: 202e 7365 7276 6963 6573 2069 6d70 6f72   .services impor
+00002800: 7420 4361 7244 756d 6d79 4442 0a0a 0a40  t CarDummyDB...@
+00002810: 436f 6e74 726f 6c6c 6572 0a63 6c61 7373  Controller.class
+00002820: 2043 6172 436f 6e74 726f 6c6c 6572 2843   CarController(C
+00002830: 6f6e 7472 6f6c 6c65 7242 6173 6529 3a0a  ontrollerBase):.
+00002840: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00002850: 2873 656c 662c 2064 623a 2043 6172 4475  (self, db: CarDu
+00002860: 6d6d 7944 4229 202d 3e20 4e6f 6e65 3a0a  mmyDB) -> None:.
+00002870: 2020 2020 2020 2020 7365 6c66 2e63 6172          self.car
+00002880: 5f64 6220 3d20 6462 0a0a 2020 2020 4070  _db = db..    @p
+00002890: 6f73 7428 222f 6372 6561 7465 222c 2072  ost("/create", r
+000028a0: 6573 706f 6e73 653d 7b32 3030 3a20 7374  esponse={200: st
+000028b0: 727d 290a 2020 2020 6173 796e 6320 6465  r}).    async de
+000028c0: 6620 6372 6561 7465 5f63 6174 2873 656c  f create_cat(sel
+000028d0: 662c 2070 6179 6c6f 6164 3a20 4361 7253  f, payload: CarS
+000028e0: 6572 6961 6c69 7a65 7229 3a0a 2020 2020  erializer):.    
+000028f0: 2020 2020 706b 203d 2073 656c 662e 6361      pk = self.ca
+00002900: 725f 6462 2e61 6464 5f63 6172 2870 6179  r_db.add_car(pay
+00002910: 6c6f 6164 2e64 6963 7428 2929 0a20 2020  load.dict()).   
+00002920: 2020 2020 2072 6574 7572 6e20 706b 0a0a       return pk..
+00002930: 2020 2020 4070 7574 2822 2f7b 6361 725f      @put("/{car_
+00002940: 6964 3a73 7472 7d22 2c20 7265 7370 6f6e  id:str}", respon
+00002950: 7365 3d7b 3230 303a 2052 6574 7269 6576  se={200: Retriev
+00002960: 6543 6172 5365 7269 616c 697a 6572 7d29  eCarSerializer})
+00002970: 0a20 2020 2061 7379 6e63 2064 6566 2075  .    async def u
+00002980: 7064 6174 655f 6361 7428 7365 6c66 2c20  pdate_cat(self, 
+00002990: 6361 725f 6964 3a20 7374 722c 2070 6179  car_id: str, pay
+000029a0: 6c6f 6164 3a20 4361 7253 6572 6961 6c69  load: CarSeriali
+000029b0: 7a65 7229 3a0a 2020 2020 2020 2020 6361  zer):.        ca
+000029c0: 7220 3d20 7365 6c66 2e63 6172 5f64 622e  r = self.car_db.
+000029d0: 7570 6461 7465 2863 6172 5f69 642c 2070  update(car_id, p
+000029e0: 6179 6c6f 6164 2e64 6963 7428 2929 0a20  ayload.dict()). 
+000029f0: 2020 2020 2020 2069 6620 6e6f 7420 6361         if not ca
+00002a00: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
+00002a10: 6169 7365 204e 6f74 466f 756e 6428 2249  aise NotFound("I
+00002a20: 7465 6d20 6e6f 7420 666f 756e 6422 290a  tem not found").
+00002a30: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00002a40: 6172 0a0a 2020 2020 4067 6574 2822 2f7b  ar..    @get("/{
+00002a50: 6361 725f 6964 3a73 7472 7d22 2c20 7265  car_id:str}", re
+00002a60: 7370 6f6e 7365 3d7b 3230 303a 2052 6574  sponse={200: Ret
+00002a70: 7269 6576 6543 6172 5365 7269 616c 697a  rieveCarSerializ
+00002a80: 6572 7d29 0a20 2020 2061 7379 6e63 2064  er}).    async d
+00002a90: 6566 2067 6574 5f63 6172 5f62 795f 6964  ef get_car_by_id
+00002aa0: 2873 656c 662c 2063 6172 5f69 643a 2073  (self, car_id: s
+00002ab0: 7472 293a 0a20 2020 2020 2020 2063 6172  tr):.        car
+00002ac0: 203d 2073 656c 662e 6361 725f 6462 2e67   = self.car_db.g
+00002ad0: 6574 2863 6172 5f69 6429 0a20 2020 2020  et(car_id).     
+00002ae0: 2020 2069 6620 6e6f 7420 6361 723a 0a20     if not car:. 
+00002af0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00002b00: 204e 6f74 466f 756e 6428 2749 7465 6d20   NotFound('Item 
+00002b10: 6e6f 7420 666f 756e 642e 2729 0a20 2020  not found.').   
+00002b20: 2020 2020 2072 6574 7572 6e20 6361 720a       return car.
+00002b30: 0a20 2020 2040 6465 6c65 7465 2822 2f7b  .    @delete("/{
+00002b40: 6361 725f 6964 3a73 7472 7d22 2c20 7265  car_id:str}", re
+00002b50: 7370 6f6e 7365 3d7b 3230 343a 2064 6963  sponse={204: dic
+00002b60: 747d 290a 2020 2020 6173 796e 6320 6465  t}).    async de
+00002b70: 6620 6465 6c65 7465 645f 6361 7428 7365  f deleted_cat(se
+00002b80: 6c66 2c20 6361 725f 6964 3a20 7374 7229  lf, car_id: str)
+00002b90: 3a0a 2020 2020 2020 2020 6361 7220 3d20  :.        car = 
+00002ba0: 7365 6c66 2e63 6172 5f64 622e 7265 6d6f  self.car_db.remo
+00002bb0: 7665 2863 6172 5f69 6429 0a20 2020 2020  ve(car_id).     
+00002bc0: 2020 2069 6620 6e6f 7420 6361 723a 0a20     if not car:. 
+00002bd0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00002be0: 204e 6f74 466f 756e 6428 2749 7465 6d20   NotFound('Item 
+00002bf0: 6e6f 7420 666f 756e 642e 2729 0a20 2020  not found.').   
+00002c00: 2020 2020 2072 6574 7572 6e20 3230 342c       return 204,
+00002c10: 207b 7d0a 0a20 2020 2040 6765 7428 222f   {}..    @get("/
+00002c20: 222c 2072 6573 706f 6e73 653d 7b32 3030  ", response={200
+00002c30: 3a20 742e 4c69 7374 5b52 6574 7269 6576  : t.List[Retriev
+00002c40: 6543 6172 5365 7269 616c 697a 6572 5d7d  eCarSerializer]}
+00002c50: 290a 2020 2020 6173 796e 6320 6465 6620  ).    async def 
+00002c60: 6c69 7374 2873 656c 6629 3a0a 2020 2020  list(self):.    
+00002c70: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00002c80: 6361 725f 6462 2e6c 6973 7428 290a 0a60  car_db.list()..`
+00002c90: 6060 0a23 2320 2a2a 5265 6769 7374 6572  ``.## **Register
+00002ca0: 2053 6572 7669 6365 2061 6e64 2043 6f6e   Service and Con
+00002cb0: 7472 6f6c 6c65 722a 2a0a 496e 2060 6361  troller**.In `ca
+00002cc0: 722f 6d6f 6475 6c65 2e70 7960 2c20 6c65  r/module.py`, le
+00002cd0: 7473 2072 6567 6973 7465 7220 6043 6172  ts register `Car
+00002ce0: 436f 6e74 726f 6c6c 6572 6020 616e 6420  Controller` and 
+00002cf0: 6043 6172 4475 6d6d 7944 4260 0a0a 6060  `CarDummyDB`..``
+00002d00: 6070 7974 686f 6e0a 6672 6f6d 2065 6c6c  `python.from ell
+00002d10: 6172 2e63 6f6d 6d6f 6e20 696d 706f 7274  ar.common import
+00002d20: 204d 6f64 756c 650a 6672 6f6d 2065 6c6c   Module.from ell
+00002d30: 6172 2e63 6f72 6520 696d 706f 7274 204d  ar.core import M
+00002d40: 6f64 756c 6542 6173 650a 6672 6f6d 2065  oduleBase.from e
+00002d50: 6c6c 6172 2e64 6920 696d 706f 7274 2043  llar.di import C
+00002d60: 6f6e 7461 696e 6572 0a0a 6672 6f6d 202e  ontainer..from .
+00002d70: 636f 6e74 726f 6c6c 6572 7320 696d 706f  controllers impo
+00002d80: 7274 2043 6172 436f 6e74 726f 6c6c 6572  rt CarController
+00002d90: 0a66 726f 6d20 2e73 6572 7669 6365 7320  .from .services 
+00002da0: 696d 706f 7274 2043 6172 4475 6d6d 7944  import CarDummyD
+00002db0: 420a 0a0a 404d 6f64 756c 6528 0a20 2020  B...@Module(.   
+00002dc0: 2063 6f6e 7472 6f6c 6c65 7273 3d5b 4361   controllers=[Ca
+00002dd0: 7243 6f6e 7472 6f6c 6c65 725d 2c0a 2020  rController],.  
+00002de0: 2020 7072 6f76 6964 6572 733d 5b43 6172    providers=[Car
+00002df0: 4475 6d6d 7944 425d 2c0a 2020 2020 726f  DummyDB],.    ro
+00002e00: 7574 6572 733d 5b5d 2c0a 290a 636c 6173  uters=[],.).clas
+00002e10: 7320 4361 724d 6f64 756c 6528 4d6f 6475  s CarModule(Modu
+00002e20: 6c65 4261 7365 293a 0a20 2020 2064 6566  leBase):.    def
+00002e30: 2072 6567 6973 7465 725f 7072 6f76 6964   register_provid
+00002e40: 6572 7328 7365 6c66 2c20 636f 6e74 6169  ers(self, contai
+00002e50: 6e65 723a 2043 6f6e 7461 696e 6572 2920  ner: Container) 
+00002e60: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00002e70: 2023 2066 6f72 206d 6f72 6520 636f 6d70   # for more comp
+00002e80: 6c69 6361 7465 6420 7072 6f76 6964 6572  licated provider
+00002e90: 2072 6567 6973 7472 6174 696f 6e73 0a20   registrations. 
+00002ea0: 2020 2020 2020 2023 2063 6f6e 7461 696e         # contain
+00002eb0: 6572 2e72 6567 6973 7465 725f 696e 7374  er.register_inst
+00002ec0: 616e 6365 282e 2e2e 290a 2020 2020 2020  ance(...).      
+00002ed0: 2020 7061 7373 0a60 6060 0a0a 2323 202a    pass.```..## *
+00002ee0: 2a52 6567 6973 7465 7269 6e67 204d 6f64  *Registering Mod
+00002ef0: 756c 652a 2a0a 456c 6c61 7220 6973 206e  ule**.Ellar is n
+00002f00: 6f74 2061 7761 7265 206f 6620 6043 6172  ot aware of `Car
+00002f10: 4d6f 6475 6c65 6020 7965 742c 2073 6f20  Module` yet, so 
+00002f20: 7765 206e 6565 6420 746f 2061 6464 2069  we need to add i
+00002f30: 7420 746f 2074 6865 2060 6d6f 6475 6c65  t to the `module
+00002f40: 7360 206c 6973 7420 6f66 2060 4170 706c  s` list of `Appl
+00002f50: 6963 6174 696f 6e4d 6f64 756c 6560 2061  icationModule` a
+00002f60: 7420 7468 6520 6063 6172 7369 7465 2f72  t the `carsite/r
+00002f70: 6f6f 745f 6d6f 6475 6c65 2e70 7960 2e0a  oot_module.py`..
+00002f80: 6060 6070 7974 686f 6e0a 6672 6f6d 2065  ```python.from e
+00002f90: 6c6c 6172 2e63 6f6d 6d6f 6e20 696d 706f  llar.common impo
+00002fa0: 7274 204d 6f64 756c 652c 2065 7863 6570  rt Module, excep
+00002fb0: 7469 6f6e 5f68 616e 646c 6572 2c20 4a53  tion_handler, JS
+00002fc0: 4f4e 5265 7370 6f6e 7365 2c20 5265 7370  ONResponse, Resp
+00002fd0: 6f6e 7365 2c20 4948 6f73 7443 6f6e 7465  onse, IHostConte
+00002fe0: 7874 0a66 726f 6d20 656c 6c61 722e 636f  xt.from ellar.co
+00002ff0: 7265 2069 6d70 6f72 7420 4d6f 6475 6c65  re import Module
+00003000: 4261 7365 0a0a 6672 6f6d 2065 6c6c 6172  Base..from ellar
+00003010: 2e73 616d 706c 6573 2e6d 6f64 756c 6573  .samples.modules
+00003020: 2069 6d70 6f72 7420 486f 6d65 4d6f 6475   import HomeModu
+00003030: 6c65 0a66 726f 6d20 2e61 7070 732e 6361  le.from .apps.ca
+00003040: 722e 6d6f 6475 6c65 2069 6d70 6f72 7420  r.module import 
+00003050: 4361 724d 6f64 756c 650a 0a0a 404d 6f64  CarModule...@Mod
+00003060: 756c 6528 6d6f 6475 6c65 733d 5b48 6f6d  ule(modules=[Hom
+00003070: 654d 6f64 756c 652c 2043 6172 4d6f 6475  eModule, CarModu
+00003080: 6c65 5d29 0a63 6c61 7373 2041 7070 6c69  le]).class Appli
+00003090: 6361 7469 6f6e 4d6f 6475 6c65 284d 6f64  cationModule(Mod
+000030a0: 756c 6542 6173 6529 3a0a 2020 2020 4065  uleBase):.    @e
+000030b0: 7863 6570 7469 6f6e 5f68 616e 646c 6572  xception_handler
+000030c0: 2834 3034 290a 2020 2020 6465 6620 6578  (404).    def ex
+000030d0: 6365 7074 696f 6e5f 3430 345f 6861 6e64  ception_404_hand
+000030e0: 6c65 7228 636c 732c 2063 6f6e 7465 7874  ler(cls, context
+000030f0: 3a20 4948 6f73 7443 6f6e 7465 7874 2c20  : IHostContext, 
+00003100: 6578 633a 2045 7863 6570 7469 6f6e 2920  exc: Exception) 
+00003110: 2d3e 2052 6573 706f 6e73 653a 0a20 2020  -> Response:.   
+00003120: 2020 2020 2072 6574 7572 6e20 4a53 4f4e       return JSON
+00003130: 5265 7370 6f6e 7365 2864 6963 7428 6465  Response(dict(de
+00003140: 7461 696c 3d22 5265 736f 7572 6365 206e  tail="Resource n
+00003150: 6f74 2066 6f75 6e64 2e22 2929 0a0a 6060  ot found."))..``
+00003160: 600a 2323 202a 2a45 6e61 626c 696e 6720  `.## **Enabling 
+00003170: 4f70 656e 4150 4920 446f 6373 2a2a 0a54  OpenAPI Docs**.T
+00003180: 6f20 7374 6172 7420 7570 206f 7065 6e61  o start up opena
+00003190: 7069 2c20 7765 206e 6565 6420 746f 2067  pi, we need to g
+000031a0: 6f20 6261 636b 2074 6f20 7072 6f6a 6563  o back to projec
+000031b0: 7420 666f 6c64 6572 2069 6e20 7468 6520  t folder in the 
+000031c0: 6073 6572 7665 722e 7079 600a 7468 656e  `server.py`.then
+000031d0: 2061 6464 2074 6865 2066 6f6c 6c6f 7769   add the followi
+000031e0: 6e67 2062 656c 6f77 2e0a 6060 6070 7974  ng below..```pyt
+000031f0: 686f 6e0a 696d 706f 7274 206f 730a 0a66  hon.import os..f
+00003200: 726f 6d20 656c 6c61 722e 636f 6e73 7461  rom ellar.consta
+00003210: 6e74 7320 696d 706f 7274 2045 4c4c 4152  nts import ELLAR
+00003220: 5f43 4f4e 4649 475f 4d4f 4455 4c45 0a66  _CONFIG_MODULE.f
+00003230: 726f 6d20 656c 6c61 722e 636f 7265 2069  rom ellar.core i
+00003240: 6d70 6f72 7420 4170 7046 6163 746f 7279  mport AppFactory
+00003250: 0a66 726f 6d20 656c 6c61 722e 6f70 656e  .from ellar.open
+00003260: 6170 6920 696d 706f 7274 204f 7065 6e41  api import OpenA
+00003270: 5049 446f 6375 6d65 6e74 4d6f 6475 6c65  PIDocumentModule
+00003280: 2c20 4f70 656e 4150 4944 6f63 756d 656e  , OpenAPIDocumen
+00003290: 7442 7569 6c64 6572 2c20 5377 6167 6765  tBuilder, Swagge
+000032a0: 7244 6f63 756d 656e 7447 656e 6572 6174  rDocumentGenerat
+000032b0: 6f72 0a66 726f 6d20 2e72 6f6f 745f 6d6f  or.from .root_mo
+000032c0: 6475 6c65 2069 6d70 6f72 7420 4170 706c  dule import Appl
+000032d0: 6963 6174 696f 6e4d 6f64 756c 650a 0a61  icationModule..a
+000032e0: 7070 6c69 6361 7469 6f6e 203d 2041 7070  pplication = App
+000032f0: 4661 6374 6f72 792e 6372 6561 7465 5f66  Factory.create_f
+00003300: 726f 6d5f 6170 705f 6d6f 6475 6c65 280a  rom_app_module(.
+00003310: 2020 2020 4170 706c 6963 6174 696f 6e4d      ApplicationM
+00003320: 6f64 756c 652c 0a20 2020 2063 6f6e 6669  odule,.    confi
+00003330: 675f 6d6f 6475 6c65 3d6f 732e 656e 7669  g_module=os.envi
+00003340: 726f 6e2e 6765 7428 0a20 2020 2020 2020  ron.get(.       
+00003350: 2045 4c4c 4152 5f43 4f4e 4649 475f 4d4f   ELLAR_CONFIG_MO
+00003360: 4455 4c45 2c20 2263 6172 7369 7465 2e63  DULE, "carsite.c
+00003370: 6f6e 6669 673a 4465 7665 6c6f 706d 656e  onfig:Developmen
+00003380: 7443 6f6e 6669 6722 0a20 2020 2029 2c0a  tConfig".    ),.
+00003390: 290a 0a64 6f63 756d 656e 745f 6275 696c  )..document_buil
+000033a0: 6465 7220 3d20 4f70 656e 4150 4944 6f63  der = OpenAPIDoc
+000033b0: 756d 656e 7442 7569 6c64 6572 2829 0a64  umentBuilder().d
+000033c0: 6f63 756d 656e 745f 6275 696c 6465 722e  ocument_builder.
+000033d0: 7365 745f 7469 746c 6528 2743 6172 5369  set_title('CarSi
+000033e0: 7465 2041 5049 2729 205c 0a20 2020 202e  te API') \.    .
+000033f0: 7365 745f 7665 7273 696f 6e28 2731 2e30  set_version('1.0
+00003400: 2e30 2729 205c 0a20 2020 202e 7365 745f  .0') \.    .set_
+00003410: 636f 6e74 6163 7428 6e61 6d65 3d27 4561  contact(name='Ea
+00003420: 6477 696e 272c 2075 726c 3d27 6874 7470  dwin', url='http
+00003430: 733a 2f2f 7777 772e 7961 686f 6f2e 636f  s://www.yahoo.co
+00003440: 6d27 2c20 656d 6169 6c3d 2765 6164 7769  m', email='eadwi
+00003450: 6e40 676d 6169 6c2e 636f 6d27 2920 5c0a  n@gmail.com') \.
+00003460: 2020 2020 2e73 6574 5f6c 6963 656e 7365      .set_license
+00003470: 2827 4d49 5420 4c69 6365 6e63 6527 2c20  ('MIT Licence', 
+00003480: 7572 6c3d 2768 7474 7073 3a2f 2f77 7777  url='https://www
+00003490: 2e67 6f6f 676c 652e 636f 6d27 290a 0a64  .google.com')..d
+000034a0: 6f63 756d 656e 7420 3d20 646f 6375 6d65  ocument = docume
+000034b0: 6e74 5f62 7569 6c64 6572 2e62 7569 6c64  nt_builder.build
+000034c0: 5f64 6f63 756d 656e 7428 6170 706c 6963  _document(applic
+000034d0: 6174 696f 6e29 0a6d 6f64 756c 6520 3d20  ation).module = 
+000034e0: 4f70 656e 4150 4944 6f63 756d 656e 744d  OpenAPIDocumentM
+000034f0: 6f64 756c 652e 7365 7475 7028 0a20 2020  odule.setup(.   
+00003500: 2064 6f63 756d 656e 743d 646f 6375 6d65   document=docume
+00003510: 6e74 2c0a 2020 2020 646f 6375 6d65 6e74  nt,.    document
+00003520: 5f67 656e 6572 6174 6f72 3d53 7761 6767  _generator=Swagg
+00003530: 6572 446f 6375 6d65 6e74 4765 6e65 7261  erDocumentGenera
+00003540: 746f 7228 292c 0a20 2020 2067 7561 7264  tor(),.    guard
+00003550: 733d 5b5d 0a29 0a61 7070 6c69 6361 7469  s=[].).applicati
+00003560: 6f6e 2e69 6e73 7461 6c6c 5f6d 6f64 756c  on.install_modul
+00003570: 6528 6d6f 6475 6c65 290a 6060 600a 0a4e  e(module).```..N
+00003580: 6f77 2077 6520 6361 6e20 7465 7374 206f  ow we can test o
+00003590: 7572 2041 5049 2061 7420 5b68 7474 703a  ur API at [http:
+000035a0: 2f2f 3132 372e 302e 302e 313a 3830 3030  //127.0.0.1:8000
+000035b0: 2f64 6f63 735d 2868 7474 703a 2f2f 3132  /docs](http://12
+000035c0: 372e 302e 302e 313a 3830 3030 2f64 6f63  7.0.0.1:8000/doc
+000035d0: 7323 2f29 0a50 6c65 6173 6520 656e 7375  s#/).Please ensu
+000035e0: 7265 2079 6f75 7220 7365 7276 6572 2069  re your server i
+000035f0: 7320 7275 6e6e 696e 670a 215b 5377 6167  s running.![Swag
+00003600: 6765 7220 5549 5d28 646f 6373 2f69 6d67  ger UI](docs/img
+00003610: 2f63 6172 5f61 7069 2e70 6e67 290a 0a23  /car_api.png)..#
+00003620: 2320 2a2a 4854 4d4c 2054 656d 706c 6174  # **HTML Templat
+00003630: 696e 672a 2a0a 456c 6c61 7220 6861 7320  ing**.Ellar has 
+00003640: 6275 696c 742d 696e 2073 7570 706f 7274  built-in support
+00003650: 2066 6f72 204a 696e 6a61 322c 2077 6869   for Jinja2, whi
+00003660: 6368 2069 7320 6120 706f 7075 6c61 7220  ch is a popular 
+00003670: 7465 6d70 6c61 7465 2065 6e67 696e 6520  template engine 
+00003680: 666f 7220 4854 4d4c 2e20 5468 6973 2066  for HTML. This f
+00003690: 6561 7475 7265 2061 6c6c 6f77 7320 666f  eature allows fo
+000036a0: 7220 6561 7379 2061 6e64 2065 6666 6963  r easy and effic
+000036b0: 6965 6e74 2048 544d 4c20 7465 6d70 6c61  ient HTML templa
+000036c0: 7469 6e67 2073 696d 696c 6172 2074 6f20  ting similar to 
+000036d0: 7468 6174 206f 6620 466c 6173 6b2e 204a  that of Flask. J
+000036e0: 696e 6a61 3220 6361 6e20 6265 2075 7365  inja2 can be use
+000036f0: 6420 746f 2063 7265 6174 6520 7265 7573  d to create reus
+00003700: 6162 6c65 2074 656d 706c 6174 6573 2c20  able templates, 
+00003710: 616e 6420 746f 2069 6e73 6572 7420 6479  and to insert dy
+00003720: 6e61 6d69 6320 6461 7461 2069 6e74 6f20  namic data into 
+00003730: 4854 4d4c 2070 6167 6573 2e20 4974 2061  HTML pages. It a
+00003740: 6c73 6f20 6861 7320 7375 7070 6f72 7420  lso has support 
+00003750: 666f 7220 7465 6d70 6c61 7465 2069 6e68  for template inh
+00003760: 6572 6974 616e 6365 2c20 636f 6e74 726f  eritance, contro
+00003770: 6c20 7374 7275 6374 7572 6573 2c20 616e  l structures, an
+00003780: 6420 6f74 6865 7220 7573 6566 756c 2066  d other useful f
+00003790: 6561 7475 7265 7320 7468 6174 2063 616e  eatures that can
+000037a0: 2068 656c 7020 746f 2073 696d 706c 6966   help to simplif
+000037b0: 7920 616e 6420 7374 7265 616d 6c69 6e65  y and streamline
+000037c0: 2074 6865 2070 726f 6365 7373 206f 6620   the process of 
+000037d0: 6372 6561 7469 6e67 2048 544d 4c20 7465  creating HTML te
+000037e0: 6d70 6c61 7465 732e 0a0a 6060 6068 746d  mplates...```htm
+000037f0: 6c0a 3c68 746d 6c3e 0a20 203c 626f 6479  l.<html>.  <body
+00003800: 3e0a 2020 2020 3c75 6c3e 0a20 2020 2020  >.    <ul>.     
+00003810: 207b 2520 666f 7220 6974 656d 2069 6e20   {% for item in 
+00003820: 6974 656d 7320 257d 0a20 2020 2020 203c  items %}.      <
+00003830: 6c69 3e7b 7b20 6974 656d 207d 7d3c 2f6c  li>{{ item }}</l
+00003840: 693e 0a20 2020 2020 207b 2520 656e 6466  i>.      {% endf
+00003850: 6f72 2025 7d0a 2020 2020 3c2f 756c 3e0a  or %}.    </ul>.
+00003860: 2020 3c2f 626f 6479 3e0a 3c2f 6874 6d6c    </body>.</html
+00003870: 3e0a 6060 600a 0a53 6565 2074 6865 205b  >.```..See the [
+00003880: 446f 635d 2868 7474 7073 3a2f 2f65 6164  Doc](https://ead
+00003890: 7769 6e63 6f64 652e 6769 7468 7562 2e69  wincode.github.i
+000038a0: 6f2f 656c 6c61 722f 7465 6d70 6c61 7469  o/ellar/templati
+000038b0: 6e67 2f74 656d 706c 6174 696e 672f 2920  ng/templating/) 
+000038c0: 666f 7220 6d6f 7265 2065 7861 6d70 6c65  for more example
+000038d0: 732e 0a0a 2323 2050 726f 6a65 6374 2053  s...## Project S
+000038e0: 7461 7475 730a 5072 6f6a 6563 7420 6973  tatus.Project is
+000038f0: 2073 7469 6c6c 2069 6e20 6465 7665 6c6f   still in develo
+00003900: 706d 656e 740a 2d20 446f 6375 6d65 6e74  pment.- Document
+00003910: 6174 696f 6e20 2d20 2869 6e20 7072 6f67  ation - (in prog
+00003920: 7265 7373 290a 2d20 496e 7465 7263 6570  ress).- Intercep
+00003930: 746f 7273 2020 2d20 205b 4173 7065 6374  tors  -  [Aspect
+00003940: 204f 7269 656e 7465 6420 5072 6f67 7261   Oriented Progra
+00003950: 6d6d 696e 675d 2868 7474 7073 3a2f 2f65  mming](https://e
+00003960: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
+00003970: 7769 6b69 2f41 7370 6563 742d 6f72 6965  wiki/Aspect-orie
+00003980: 6e74 6564 5f70 726f 6772 616d 6d69 6e67  nted_programming
+00003990: 2920 2841 4f50 2920 7465 6368 6e69 7175  ) (AOP) techniqu
+000039a0: 650a 2d20 4461 7461 6261 7365 2050 6c75  e.- Database Plu
+000039b0: 6769 6e20 7769 7468 205b 456e 636f 6465  gin with [Encode
+000039c0: 2f4f 524d 5d28 6874 7470 733a 2f2f 6769  /ORM](https://gi
+000039d0: 7468 7562 2e63 6f6d 2f65 6e63 6f64 652f  thub.com/encode/
+000039e0: 6f72 6d29 0a0a                           orm)..
```

