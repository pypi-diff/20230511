# Comparing `tmp/clickable-ut-7.8.0.tar.gz` & `tmp/clickable-ut-7.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickable-ut-7.8.0.tar", last modified: Tue Dec 20 19:12:27 2022, max compression
+gzip compressed data, was "clickable-ut-7.9.0.tar", last modified: Fri Dec 30 04:03:35 2022, max compression
```

## Comparing `clickable-ut-7.8.0.tar` & `clickable-ut-7.9.0.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 19:12:27.980471 clickable-ut-7.8.0/
--rw-rw-rw-   0 root         (0) root         (0)    35121 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      390 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3723 2022-12-20 19:12:27.980471 clickable-ut-7.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2486 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 19:12:27.934466 clickable-ut-7.8.0/clickable/
--rw-rw-rw-   0 root         (0) root         (0)     2773 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 19:12:27.939466 clickable-ut-7.8.0/clickable/builders/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/builders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      937 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/builders/base.py
--rw-rw-rw-   0 root         (0) root         (0)      769 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/builders/cmake.py
--rw-rw-rw-   0 root         (0) root         (0)     2298 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/builders/cordova.py
--rw-rw-rw-   0 root         (0) root         (0)      240 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/builders/custom.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/builders/go.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/builders/make.py
--rw-rw-rw-   0 root         (0) root         (0)     1577 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/builders/pure.py
--rw-rw-rw-   0 root         (0) root         (0)     1077 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/builders/qbs.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/builders/qmake.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/builders/rust.py
--rw-rw-rw-   0 root         (0) root         (0)     4361 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      880 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/command_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 19:12:27.950468 clickable-ut-7.8.0/clickable/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1729 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/base.py
--rw-rw-rw-   0 root         (0) root         (0)    15154 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/build.py
--rw-rw-rw-   0 root         (0) root         (0)     2042 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/chain.py
--rw-rw-rw-   0 root         (0) root         (0)     2770 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/ci.py
--rw-rw-rw-   0 root         (0) root         (0)     6105 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/clean.py
--rw-rw-rw-   0 root         (0) root         (0)     5277 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/create.py
--rw-rw-rw-   0 root         (0) root         (0)    15590 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/desktop.py
--rw-rw-rw-   0 root         (0) root         (0)      481 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/devices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 19:12:27.954468 clickable-ut-7.8.0/clickable/commands/docker/
--rw-rw-rw-   0 root         (0) root         (0)      811 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/docker/debug_gdb_support.py
--rw-rw-rw-   0 root         (0) root         (0)      279 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/docker/debug_valgrind_support.py
--rw-rw-rw-   0 root         (0) root         (0)     3606 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/docker/docker_config.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/docker/docker_support.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/docker/go_support.py
--rw-rw-rw-   0 root         (0) root         (0)     1292 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/docker/multimedia_support.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 19:12:27.955468 clickable-ut-7.8.0/clickable/commands/docker/nvidia/
--rw-rw-rw-   0 root         (0) root         (0)      663 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/docker/nvidia/legacy_nvidia_support.py
--rw-rw-rw-   0 root         (0) root         (0)      617 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/docker/nvidia/nvidia_support_since_docker_version_1903.py
--rw-rw-rw-   0 root         (0) root         (0)      956 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/docker/nvidia_support.py
--rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/docker/rust_support.py
--rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/docker/theme_support.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/docker/webapp_support.py
--rw-rw-rw-   0 root         (0) root         (0)     6933 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/gdb.py
--rw-rw-rw-   0 root         (0) root         (0)     9703 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/gdbserver.py
--rw-rw-rw-   0 root         (0) root         (0)     2842 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/ide.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 19:12:27.956468 clickable-ut-7.8.0/clickable/commands/idedelegates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/idedelegates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/idedelegates/idedelegate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 19:12:27.957469 clickable-ut-7.8.0/clickable/commands/idedelegates/qtcreator/
--rw-rw-rw-   0 root         (0) root         (0)    18503 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/idedelegates/qtcreator/CMakeLists.txt.user.shared.in
--rw-rw-rw-   0 root         (0) root         (0)    31576 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/idedelegates/qtcreator/QtProject.tar.xz
--rw-rw-rw-   0 root         (0) root         (0)      412 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/idedelegates/qtcreator/Readme.md
--rw-rw-rw-   0 root         (0) root         (0)     7910 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/idedelegates/qtcreator.py
--rw-rw-rw-   0 root         (0) root         (0)     4066 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/install.py
--rw-rw-rw-   0 root         (0) root         (0)     2674 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/launch.py
--rw-rw-rw-   0 root         (0) root         (0)     1203 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/log.py
--rw-rw-rw-   0 root         (0) root         (0)     1180 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/logs.py
--rw-rw-rw-   0 root         (0) root         (0)      477 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/no_lock.py
--rw-rw-rw-   0 root         (0) root         (0)     4040 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/publish.py
--rw-rw-rw-   0 root         (0) root         (0)     2268 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/review.py
--rw-rw-rw-   0 root         (0) root         (0)     1859 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/run.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/screenshots.py
--rw-rw-rw-   0 root         (0) root         (0)     1019 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/script.py
--rw-rw-rw-   0 root         (0) root         (0)     3465 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     4688 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/shell.py
--rw-rw-rw-   0 root         (0) root         (0)     2400 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/test.py
--rw-rw-rw-   0 root         (0) root         (0)      739 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/update_images.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/commands/writable_image.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 19:12:27.963469 clickable-ut-7.8.0/clickable/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/config/base.py
--rw-rw-rw-   0 root         (0) root         (0)      264 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/config/build.py
--rw-rw-rw-   0 root         (0) root         (0)      273 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/config/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2286 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/config/clickable.schema
--rw-rw-rw-   0 root         (0) root         (0)      124 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/config/command_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3842 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/config/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      350 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/config/device.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/config/environment.py
--rw-rw-rw-   0 root         (0) root         (0)     6345 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/config/file_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1536 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/config/global_config.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/config/ide.py
--rw-rw-rw-   0 root         (0) root         (0)     8829 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/config/libconfig.py
--rw-rw-rw-   0 root         (0) root         (0)    37063 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/config/project.py
--rw-rw-rw-   0 root         (0) root         (0)     6188 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/config/project.schema
--rw-rw-rw-   0 root         (0) root         (0)    21005 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/container.py
--rw-rw-rw-   0 root         (0) root         (0)     5048 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/device.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1541 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 19:12:27.964469 clickable-ut-7.8.0/clickable/system/
--rw-rw-rw-   0 root         (0) root         (0)      104 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/system/access.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 19:12:27.965469 clickable-ut-7.8.0/clickable/system/queries/
--rw-rw-rw-   0 root         (0) root         (0)     1286 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/system/queries/legacy_docker_version.py
--rw-rw-rw-   0 root         (0) root         (0)      537 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/system/queries/nvidia_drivers_in_use.py
--rw-rw-rw-   0 root         (0) root         (0)      182 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/system/query.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/system/require.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 19:12:27.966470 clickable-ut-7.8.0/clickable/system/requirements/
--rw-rw-rw-   0 root         (0) root         (0)      386 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/system/requirements/nvidia_container_toolkit.py
--rw-rw-rw-   0 root         (0) root         (0)      477 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/system/requirements/nvidia_docker.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/system/requirements/nvidia_modprobe.py
--rw-rw-rw-   0 root         (0) root         (0)     9739 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4015 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/clickable/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 19:12:27.969470 clickable-ut-7.8.0/clickable_ut.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3723 2022-12-20 19:12:27.000000 clickable-ut-7.8.0/clickable_ut.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3811 2022-12-20 19:12:27.000000 clickable-ut-7.8.0/clickable_ut.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-20 19:12:27.000000 clickable-ut-7.8.0/clickable_ut.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2022-12-20 19:12:27.000000 clickable-ut-7.8.0/clickable_ut.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-20 19:12:27.000000 clickable-ut-7.8.0/clickable_ut.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       61 2022-12-20 19:12:27.000000 clickable-ut-7.8.0/clickable_ut.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-12-20 19:12:27.000000 clickable-ut-7.8.0/clickable_ut.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 19:12:27.971470 clickable-ut-7.8.0/debian/
--rw-rw-rw-   0 root         (0) root         (0)    36229 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/debian/changelog
--rw-rw-rw-   0 root         (0) root         (0)        2 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/debian/compat
--rw-rw-rw-   0 root         (0) root         (0)     1019 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/debian/control
--rw-rw-rw-   0 root         (0) root         (0)     1439 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/debian/copyright
--rwxrwxrwx   0 root         (0) root         (0)      728 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/debian/rules
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 19:12:27.971470 clickable-ut-7.8.0/debian/source/
--rw-rw-rw-   0 root         (0) root         (0)       13 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/debian/source/format
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 19:12:27.978471 clickable-ut-7.8.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      606 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 19:12:27.979471 clickable-ut-7.8.0/docs/_static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/_static/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 19:12:27.979471 clickable-ut-7.8.0/docs/_static/images/
--rw-rw-rw-   0 root         (0) root         (0)     2647 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/_static/images/logo.png
--rw-rw-rw-   0 root         (0) root         (0)       26 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/_static/version.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 19:12:27.980471 clickable-ut-7.8.0/docs/_templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/_templates/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      300 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/_templates/layout.html
--rw-rw-rw-   0 root         (0) root         (0)     1017 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/app-templates.rst
--rwxrwxrwx   0 root         (0) root         (0)       45 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/autobuild.sh
--rw-rw-rw-   0 root         (0) root         (0)     1181 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/builders.rst
--rw-rw-rw-   0 root         (0) root         (0)    21268 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     7065 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/commands.rst
--rw-rw-rw-   0 root         (0) root         (0)     5310 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2680 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/config.rst
--rw-rw-rw-   0 root         (0) root         (0)      736 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/continuous-integration.rst
--rw-rw-rw-   0 root         (0) root         (0)     1504 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/debugging.rst
--rw-rw-rw-   0 root         (0) root         (0)     3670 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/env-vars.rst
--rw-rw-rw-   0 root         (0) root         (0)     2857 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/getting-started.rst
--rw-rw-rw-   0 root         (0) root         (0)     2271 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1891 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/install.rst
--rw-rw-rw-   0 root         (0) root         (0)     8683 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/migration.rst
--rw-rw-rw-   0 root         (0) root         (0)    17067 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/project-config.rst
--rw-rw-rw-   0 root         (0) root         (0)     4781 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/docs/usage.rst
--rw-rw-rw-   0 root         (0) root         (0)      175 2022-12-20 19:12:27.981471 clickable-ut-7.8.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2082 2022-12-20 19:12:26.000000 clickable-ut-7.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 04:03:35.327335 clickable-ut-7.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35121 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      390 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3723 2022-12-30 04:03:35.327335 clickable-ut-7.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2486 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 04:03:35.284342 clickable-ut-7.9.0/clickable/
+-rw-rw-rw-   0 root         (0) root         (0)     2773 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 04:03:35.288342 clickable-ut-7.9.0/clickable/builders/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/builders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      937 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/builders/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      769 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/builders/cmake.py
+-rw-rw-rw-   0 root         (0) root         (0)     2298 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/builders/cordova.py
+-rw-rw-rw-   0 root         (0) root         (0)      240 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/builders/custom.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/builders/go.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/builders/make.py
+-rw-rw-rw-   0 root         (0) root         (0)     1577 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/builders/pure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/builders/qbs.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/builders/qmake.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/builders/rust.py
+-rw-rw-rw-   0 root         (0) root         (0)     4361 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      880 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/command_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 04:03:35.298340 clickable-ut-7.9.0/clickable/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1729 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    15154 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/build.py
+-rw-rw-rw-   0 root         (0) root         (0)     2042 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/chain.py
+-rw-rw-rw-   0 root         (0) root         (0)     2770 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     6105 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/clean.py
+-rw-rw-rw-   0 root         (0) root         (0)     5277 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/create.py
+-rw-rw-rw-   0 root         (0) root         (0)    15629 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/desktop.py
+-rw-rw-rw-   0 root         (0) root         (0)      481 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/devices.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 04:03:35.301339 clickable-ut-7.9.0/clickable/commands/docker/
+-rw-rw-rw-   0 root         (0) root         (0)      811 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/docker/debug_gdb_support.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/docker/debug_valgrind_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     3606 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/docker/docker_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/docker/docker_support.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/docker/go_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     1292 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/docker/multimedia_support.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 04:03:35.302339 clickable-ut-7.9.0/clickable/commands/docker/nvidia/
+-rw-rw-rw-   0 root         (0) root         (0)      663 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/docker/nvidia/legacy_nvidia_support.py
+-rw-rw-rw-   0 root         (0) root         (0)      617 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/docker/nvidia/nvidia_support_since_docker_version_1903.py
+-rw-rw-rw-   0 root         (0) root         (0)      956 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/docker/nvidia_support.py
+-rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/docker/rust_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/docker/theme_support.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/docker/webapp_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     6933 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/gdb.py
+-rw-rw-rw-   0 root         (0) root         (0)     9703 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/gdbserver.py
+-rw-rw-rw-   0 root         (0) root         (0)     2842 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/ide.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 04:03:35.303339 clickable-ut-7.9.0/clickable/commands/idedelegates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/idedelegates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/idedelegates/idedelegate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 04:03:35.305339 clickable-ut-7.9.0/clickable/commands/idedelegates/qtcreator/
+-rw-rw-rw-   0 root         (0) root         (0)    18503 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/idedelegates/qtcreator/CMakeLists.txt.user.shared.in
+-rw-rw-rw-   0 root         (0) root         (0)    31576 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/idedelegates/qtcreator/QtProject.tar.xz
+-rw-rw-rw-   0 root         (0) root         (0)      412 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/idedelegates/qtcreator/Readme.md
+-rw-rw-rw-   0 root         (0) root         (0)     7910 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/idedelegates/qtcreator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4066 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/install.py
+-rw-rw-rw-   0 root         (0) root         (0)     2674 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1203 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/log.py
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/logs.py
+-rw-rw-rw-   0 root         (0) root         (0)      477 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/no_lock.py
+-rw-rw-rw-   0 root         (0) root         (0)     4040 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/publish.py
+-rw-rw-rw-   0 root         (0) root         (0)     2268 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/review.py
+-rw-rw-rw-   0 root         (0) root         (0)     1859 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/run.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/screenshots.py
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/script.py
+-rw-rw-rw-   0 root         (0) root         (0)     3465 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     4688 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/shell.py
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      739 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/update_images.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/commands/writable_image.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 04:03:35.310338 clickable-ut-7.9.0/clickable/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/config/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      264 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/config/build.py
+-rw-rw-rw-   0 root         (0) root         (0)      273 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/config/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2286 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/config/clickable.schema
+-rw-rw-rw-   0 root         (0) root         (0)      124 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/config/command_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3842 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/config/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      350 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/config/device.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/config/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)     6345 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/config/file_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/config/global_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/config/ide.py
+-rw-rw-rw-   0 root         (0) root         (0)     8829 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/config/libconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)    37063 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/config/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     6188 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/config/project.schema
+-rw-rw-rw-   0 root         (0) root         (0)    21005 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     5048 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/device.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 04:03:35.311338 clickable-ut-7.9.0/clickable/system/
+-rw-rw-rw-   0 root         (0) root         (0)      104 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/system/access.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 04:03:35.312338 clickable-ut-7.9.0/clickable/system/queries/
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/system/queries/legacy_docker_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      537 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/system/queries/nvidia_drivers_in_use.py
+-rw-rw-rw-   0 root         (0) root         (0)      182 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/system/query.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/system/require.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 04:03:35.313338 clickable-ut-7.9.0/clickable/system/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)      386 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/system/requirements/nvidia_container_toolkit.py
+-rw-rw-rw-   0 root         (0) root         (0)      477 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/system/requirements/nvidia_docker.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/system/requirements/nvidia_modprobe.py
+-rw-rw-rw-   0 root         (0) root         (0)     9739 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4015 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/clickable/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 04:03:35.316337 clickable-ut-7.9.0/clickable_ut.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3723 2022-12-30 04:03:35.000000 clickable-ut-7.9.0/clickable_ut.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3811 2022-12-30 04:03:35.000000 clickable-ut-7.9.0/clickable_ut.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-30 04:03:35.000000 clickable-ut-7.9.0/clickable_ut.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2022-12-30 04:03:35.000000 clickable-ut-7.9.0/clickable_ut.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-30 04:03:35.000000 clickable-ut-7.9.0/clickable_ut.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       61 2022-12-30 04:03:35.000000 clickable-ut-7.9.0/clickable_ut.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2022-12-30 04:03:35.000000 clickable-ut-7.9.0/clickable_ut.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 04:03:35.318337 clickable-ut-7.9.0/debian/
+-rw-rw-rw-   0 root         (0) root         (0)    36477 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/debian/changelog
+-rw-rw-rw-   0 root         (0) root         (0)        2 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/debian/compat
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/debian/control
+-rw-rw-rw-   0 root         (0) root         (0)     1439 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/debian/copyright
+-rwxrwxrwx   0 root         (0) root         (0)      728 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/debian/rules
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 04:03:35.318337 clickable-ut-7.9.0/debian/source/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/debian/source/format
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 04:03:35.325336 clickable-ut-7.9.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      606 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 04:03:35.325336 clickable-ut-7.9.0/docs/_static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/_static/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 04:03:35.326336 clickable-ut-7.9.0/docs/_static/images/
+-rw-rw-rw-   0 root         (0) root         (0)     2647 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/_static/images/logo.png
+-rw-rw-rw-   0 root         (0) root         (0)       26 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/_static/version.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 04:03:35.327335 clickable-ut-7.9.0/docs/_templates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/_templates/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      300 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/_templates/layout.html
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/app-templates.rst
+-rwxrwxrwx   0 root         (0) root         (0)       45 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/autobuild.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/builders.rst
+-rw-rw-rw-   0 root         (0) root         (0)    21424 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7065 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/commands.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5310 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2680 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/config.rst
+-rw-rw-rw-   0 root         (0) root         (0)      736 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/continuous-integration.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/debugging.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3670 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/env-vars.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2857 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/getting-started.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1891 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/install.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8683 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/migration.rst
+-rw-rw-rw-   0 root         (0) root         (0)    17067 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/project-config.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4781 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/docs/usage.rst
+-rw-rw-rw-   0 root         (0) root         (0)      175 2022-12-30 04:03:35.327335 clickable-ut-7.9.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2082 2022-12-30 04:03:34.000000 clickable-ut-7.9.0/setup.py
```

### Comparing `clickable-ut-7.8.0/LICENSE` & `clickable-ut-7.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/PKG-INFO` & `clickable-ut-7.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickable-ut
-Version: 7.8.0
+Version: 7.9.0
 Summary: Compile, build, and deploy Ubuntu Touch click packages all from the command line.
 Home-page: https://clickable-ut.dev/
 Author: Brian Douglass
 License: GPL3
 Project-URL: Documentation, https://clickable-ut.dev/en/latest/
 Project-URL: Source, https://gitlab.com/clickable/clickable
 Project-URL: Bug Tracker, https://gitlab.com/clickable/clickable/-/issues
```

### Comparing `clickable-ut-7.8.0/README.md` & `clickable-ut-7.9.0/README.md`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/__init__.py` & `clickable-ut-7.9.0/clickable/__init__.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/builders/base.py` & `clickable-ut-7.9.0/clickable/builders/base.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/builders/cmake.py` & `clickable-ut-7.9.0/clickable/builders/cmake.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/builders/cordova.py` & `clickable-ut-7.9.0/clickable/builders/cordova.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/builders/make.py` & `clickable-ut-7.9.0/clickable/builders/make.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/builders/pure.py` & `clickable-ut-7.9.0/clickable/builders/pure.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/builders/qbs.py` & `clickable-ut-7.9.0/clickable/builders/qbs.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/builders/qmake.py` & `clickable-ut-7.9.0/clickable/builders/qmake.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/builders/rust.py` & `clickable-ut-7.9.0/clickable/builders/rust.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/cli.py` & `clickable-ut-7.9.0/clickable/cli.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/command_utils.py` & `clickable-ut-7.9.0/clickable/command_utils.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/base.py` & `clickable-ut-7.9.0/clickable/commands/base.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/build.py` & `clickable-ut-7.9.0/clickable/commands/build.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/chain.py` & `clickable-ut-7.9.0/clickable/commands/chain.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/ci.py` & `clickable-ut-7.9.0/clickable/commands/ci.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/clean.py` & `clickable-ut-7.9.0/clickable/commands/clean.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/create.py` & `clickable-ut-7.9.0/clickable/commands/create.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/desktop.py` & `clickable-ut-7.9.0/clickable/commands/desktop.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,14 +315,15 @@
             'DISPLAY': os.environ['DISPLAY'],
             'QML2_IMPORT_PATH': lib_path,
             'LD_LIBRARY_PATH': lib_path,
             'PATH': self.get_docker_path_env(working_directory) + self.get_image_path_var(),
             'HOME': Constants.device_home,
             'OXIDE_NO_SANDBOX': '1',
             'UBUNTU_APP_LAUNCH_ARCH': self.config.arch_triplet,
+            'UITK_ICON_THEME': 'suru',
         }
 
         if self.custom_mode:
             env_vars.update(self.config.get_env_vars())
             env_vars['HOME'] = os.environ['HOME']
 
         return env_vars
```

### Comparing `clickable-ut-7.8.0/clickable/commands/docker/debug_gdb_support.py` & `clickable-ut-7.9.0/clickable/commands/docker/debug_gdb_support.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/docker/docker_config.py` & `clickable-ut-7.9.0/clickable/commands/docker/docker_config.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/docker/go_support.py` & `clickable-ut-7.9.0/clickable/commands/docker/go_support.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/docker/multimedia_support.py` & `clickable-ut-7.9.0/clickable/commands/docker/multimedia_support.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/docker/nvidia/legacy_nvidia_support.py` & `clickable-ut-7.9.0/clickable/commands/docker/nvidia/legacy_nvidia_support.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/docker/nvidia/nvidia_support_since_docker_version_1903.py` & `clickable-ut-7.9.0/clickable/commands/docker/nvidia/nvidia_support_since_docker_version_1903.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/docker/nvidia_support.py` & `clickable-ut-7.9.0/clickable/commands/docker/nvidia_support.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/docker/rust_support.py` & `clickable-ut-7.9.0/clickable/commands/docker/rust_support.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/docker/webapp_support.py` & `clickable-ut-7.9.0/clickable/commands/docker/webapp_support.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/gdb.py` & `clickable-ut-7.9.0/clickable/commands/gdb.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/gdbserver.py` & `clickable-ut-7.9.0/clickable/commands/gdbserver.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/ide.py` & `clickable-ut-7.9.0/clickable/commands/ide.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/idedelegates/qtcreator/CMakeLists.txt.user.shared.in` & `clickable-ut-7.9.0/clickable/commands/idedelegates/qtcreator/CMakeLists.txt.user.shared.in`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/idedelegates/qtcreator/QtProject.tar.xz` & `clickable-ut-7.9.0/clickable/commands/idedelegates/qtcreator/QtProject.tar.xz`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/idedelegates/qtcreator.py` & `clickable-ut-7.9.0/clickable/commands/idedelegates/qtcreator.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/install.py` & `clickable-ut-7.9.0/clickable/commands/install.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/launch.py` & `clickable-ut-7.9.0/clickable/commands/launch.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/log.py` & `clickable-ut-7.9.0/clickable/commands/log.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/logs.py` & `clickable-ut-7.9.0/clickable/commands/logs.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/publish.py` & `clickable-ut-7.9.0/clickable/commands/publish.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/review.py` & `clickable-ut-7.9.0/clickable/commands/review.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/run.py` & `clickable-ut-7.9.0/clickable/commands/run.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/script.py` & `clickable-ut-7.9.0/clickable/commands/script.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/setup.py` & `clickable-ut-7.9.0/clickable/commands/setup.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/shell.py` & `clickable-ut-7.9.0/clickable/commands/shell.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/test.py` & `clickable-ut-7.9.0/clickable/commands/test.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/update_images.py` & `clickable-ut-7.9.0/clickable/commands/update_images.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/commands/writable_image.py` & `clickable-ut-7.9.0/clickable/commands/writable_image.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/config/clickable.schema` & `clickable-ut-7.9.0/clickable/config/clickable.schema`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/config/constants.py` & `clickable-ut-7.9.0/clickable/config/constants.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/config/file_helpers.py` & `clickable-ut-7.9.0/clickable/config/file_helpers.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/config/global_config.py` & `clickable-ut-7.9.0/clickable/config/global_config.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/config/libconfig.py` & `clickable-ut-7.9.0/clickable/config/libconfig.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/config/project.py` & `clickable-ut-7.9.0/clickable/config/project.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/config/project.schema` & `clickable-ut-7.9.0/clickable/config/project.schema`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/container.py` & `clickable-ut-7.9.0/clickable/container.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/device.py` & `clickable-ut-7.9.0/clickable/device.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/logger.py` & `clickable-ut-7.9.0/clickable/logger.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/system/queries/legacy_docker_version.py` & `clickable-ut-7.9.0/clickable/system/queries/legacy_docker_version.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/system/queries/nvidia_drivers_in_use.py` & `clickable-ut-7.9.0/clickable/system/queries/nvidia_drivers_in_use.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/utils.py` & `clickable-ut-7.9.0/clickable/utils.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/clickable/version.py` & `clickable-ut-7.9.0/clickable/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 REQUESTS_AVAILABLE = True
 try:
     import requests
 except ImportError:
     REQUESTS_AVAILABLE = False
 
-__version__ = '7.8.0'
+__version__ = '7.9.0'
 
 __container_minimum_required__ = 9
 
 DATE_FORMAT = '%Y-%m-%dT%H:%M:%S'
 
 
 def show_version():
```

### Comparing `clickable-ut-7.8.0/clickable_ut.egg-info/PKG-INFO` & `clickable-ut-7.9.0/clickable_ut.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickable-ut
-Version: 7.8.0
+Version: 7.9.0
 Summary: Compile, build, and deploy Ubuntu Touch click packages all from the command line.
 Home-page: https://clickable-ut.dev/
 Author: Brian Douglass
 License: GPL3
 Project-URL: Documentation, https://clickable-ut.dev/en/latest/
 Project-URL: Source, https://gitlab.com/clickable/clickable
 Project-URL: Bug Tracker, https://gitlab.com/clickable/clickable/-/issues
```

### Comparing `clickable-ut-7.8.0/clickable_ut.egg-info/SOURCES.txt` & `clickable-ut-7.9.0/clickable_ut.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/debian/changelog` & `clickable-ut-7.9.0/debian/changelog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+clickable (7.9.0) unstable; urgency=medium
+
+  * Added support for dark mode when using Focal based desktop mode
+  * Fixed icons not showing correctly in desktop mode
+
+ -- Clickable <bhdouglass+clickable@gmail.com>  Mon, 26 Dec 2022 23:24:46 -0500
+
 clickable (7.8.0) unstable; urgency=medium
 
   * Added warning when trying to build an app without libraries being built first
   * Dropped Qt 5.9 support
   * Switched to using fully qualified docker image names to fix an issue with Podman
   * Fixed bug cleaning desktop mode directories
```

### Comparing `clickable-ut-7.8.0/debian/control` & `clickable-ut-7.9.0/debian/control`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/debian/copyright` & `clickable-ut-7.9.0/debian/copyright`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/debian/rules` & `clickable-ut-7.9.0/debian/rules`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/docs/Makefile` & `clickable-ut-7.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/docs/_static/images/logo.png` & `clickable-ut-7.9.0/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/docs/app-templates.rst` & `clickable-ut-7.9.0/docs/app-templates.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/docs/builders.rst` & `clickable-ut-7.9.0/docs/builders.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/docs/changelog.rst` & `clickable-ut-7.9.0/docs/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. _changelog:
 
 Changelog
 =========
 
+Changes in v7.9.0
+-----------------
+
+- Added support for dark mode when using Focal based desktop mode
+- Fixed icons not showing correctly in desktop mode
+
 Changes in v7.8.0
 -----------------
 
 - Added warning when trying to build an app without libraries being built first
 - Dropped Qt 5.9 support
 - Switched to using fully qualified docker image names to fix an issue with Podman
 - Fixed bug cleaning desktop mode directories
```

### Comparing `clickable-ut-7.8.0/docs/commands.rst` & `clickable-ut-7.9.0/docs/commands.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/docs/conf.py` & `clickable-ut-7.9.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,17 +51,17 @@
 author = 'Clickable Team'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '7.8.0'
+version = '7.9.0'
 # The full version, including alpha/beta/rc tags.
-release = '7.8.0'
+release = '7.9.0'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `clickable-ut-7.8.0/docs/config.rst` & `clickable-ut-7.9.0/docs/config.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/docs/continuous-integration.rst` & `clickable-ut-7.9.0/docs/continuous-integration.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/docs/debugging.rst` & `clickable-ut-7.9.0/docs/debugging.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/docs/env-vars.rst` & `clickable-ut-7.9.0/docs/env-vars.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/docs/getting-started.rst` & `clickable-ut-7.9.0/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/docs/index.rst` & `clickable-ut-7.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/docs/install.rst` & `clickable-ut-7.9.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/docs/migration.rst` & `clickable-ut-7.9.0/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/docs/project-config.rst` & `clickable-ut-7.9.0/docs/project-config.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/docs/usage.rst` & `clickable-ut-7.9.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-7.8.0/setup.py` & `clickable-ut-7.9.0/setup.py`

 * *Files identical despite different names*

