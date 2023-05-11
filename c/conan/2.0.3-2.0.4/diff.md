# Comparing `tmp/conan-2.0.3.tar.gz` & `tmp/conan-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/conan-2.0.3.tar", last modified: Mon Apr  3 13:44:47 2023, max compression
+gzip compressed data, was "dist/conan-2.0.4.tar", last modified: Tue Apr 11 14:41:59 2023, max compression
```

## Comparing `conan-2.0.3.tar` & `conan-2.0.4.tar`

### file list

```diff
@@ -1,349 +1,349 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.029551 conan-2.0.3/
--rw-r--r--   0 root         (0) root         (0)     1084 2023-04-03 13:44:40.000000 conan-2.0.3/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-03 13:44:40.000000 conan-2.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8324 2023-04-03 13:44:47.030551 conan-2.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6041 2023-04-03 13:44:40.000000 conan-2.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:46.993548 conan-2.0.3/conan/
--rw-r--r--   0 root         (0) root         (0)      152 2023-04-03 13:44:40.000000 conan-2.0.3/conan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:46.994547 conan-2.0.3/conan/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 13:44:40.000000 conan-2.0.3/conan/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2360 2023-04-03 13:44:40.000000 conan-2.0.3/conan/api/conan_api.py
--rw-r--r--   0 root         (0) root         (0)     5892 2023-04-03 13:44:40.000000 conan-2.0.3/conan/api/model.py
--rw-r--r--   0 root         (0) root         (0)     6824 2023-04-03 13:44:40.000000 conan-2.0.3/conan/api/output.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:46.996548 conan-2.0.3/conan/api/subapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 13:44:40.000000 conan-2.0.3/conan/api/subapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3735 2023-04-03 13:44:40.000000 conan-2.0.3/conan/api/subapi/cache.py
--rw-r--r--   0 root         (0) root         (0)     1101 2023-04-03 13:44:40.000000 conan-2.0.3/conan/api/subapi/config.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-04-03 13:44:40.000000 conan-2.0.3/conan/api/subapi/download.py
--rw-r--r--   0 root         (0) root         (0)     2309 2023-04-03 13:44:40.000000 conan-2.0.3/conan/api/subapi/export.py
--rw-r--r--   0 root         (0) root         (0)    10921 2023-04-03 13:44:40.000000 conan-2.0.3/conan/api/subapi/graph.py
--rw-r--r--   0 root         (0) root         (0)     3144 2023-04-03 13:44:40.000000 conan-2.0.3/conan/api/subapi/install.py
--rw-r--r--   0 root         (0) root         (0)     7652 2023-04-03 13:44:40.000000 conan-2.0.3/conan/api/subapi/list.py
--rw-r--r--   0 root         (0) root         (0)     4784 2023-04-03 13:44:40.000000 conan-2.0.3/conan/api/subapi/local.py
--rw-r--r--   0 root         (0) root         (0)     4029 2023-04-03 13:44:40.000000 conan-2.0.3/conan/api/subapi/lockfile.py
--rw-r--r--   0 root         (0) root         (0)     4780 2023-04-03 13:44:40.000000 conan-2.0.3/conan/api/subapi/new.py
--rw-r--r--   0 root         (0) root         (0)     4426 2023-04-03 13:44:40.000000 conan-2.0.3/conan/api/subapi/profiles.py
--rw-r--r--   0 root         (0) root         (0)     4425 2023-04-03 13:44:40.000000 conan-2.0.3/conan/api/subapi/remotes.py
--rw-r--r--   0 root         (0) root         (0)     2361 2023-04-03 13:44:40.000000 conan-2.0.3/conan/api/subapi/remove.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-04-03 13:44:40.000000 conan-2.0.3/conan/api/subapi/search.py
--rw-r--r--   0 root         (0) root         (0)     3907 2023-04-03 13:44:40.000000 conan-2.0.3/conan/api/subapi/upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:46.997548 conan-2.0.3/conan/cli/
--rw-r--r--   0 root         (0) root         (0)      397 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7473 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/args.py
--rw-r--r--   0 root         (0) root         (0)    11022 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/cli.py
--rw-r--r--   0 root         (0) root         (0)     7513 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:46.999548 conan-2.0.3/conan/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3161 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/build.py
--rw-r--r--   0 root         (0) root         (0)     4419 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/cache.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/config.py
--rw-r--r--   0 root         (0) root         (0)     8119 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/create.py
--rw-r--r--   0 root         (0) root         (0)     3065 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/download.py
--rw-r--r--   0 root         (0) root         (0)     2708 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/editable.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/export.py
--rw-r--r--   0 root         (0) root         (0)     5483 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/export_pkg.py
--rw-r--r--   0 root         (0) root         (0)     8176 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/graph.py
--rw-r--r--   0 root         (0) root         (0)     1361 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/inspect.py
--rw-r--r--   0 root         (0) root         (0)     4411 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/install.py
--rw-r--r--   0 root         (0) root         (0)     5192 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/list.py
--rw-r--r--   0 root         (0) root         (0)     5125 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/lock.py
--rw-r--r--   0 root         (0) root         (0)     4222 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/new.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/profile.py
--rw-r--r--   0 root         (0) root         (0)    11692 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/remote.py
--rw-r--r--   0 root         (0) root         (0)     2410 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/remove.py
--rw-r--r--   0 root         (0) root         (0)     1753 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/search.py
--rw-r--r--   0 root         (0) root         (0)      648 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/source.py
--rw-r--r--   0 root         (0) root         (0)     3584 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/test.py
--rw-r--r--   0 root         (0) root         (0)     3830 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/commands/upload.py
--rw-r--r--   0 root         (0) root         (0)      490 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/exit_codes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:46.999548 conan-2.0.3/conan/cli/formatters/
--rw-r--r--   0 root         (0) root         (0)      158 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/formatters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.000548 conan-2.0.3/conan/cli/formatters/graph/
--rw-r--r--   0 root         (0) root         (0)      110 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/formatters/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5019 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/formatters/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/formatters/graph/graph_info_text.py
--rw-r--r--   0 root         (0) root         (0)      144 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/formatters/graph/info_graph_dot.py
--rw-r--r--   0 root         (0) root         (0)     5583 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/formatters/graph/info_graph_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.001548 conan-2.0.3/conan/cli/formatters/list/
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/formatters/list/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4612 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/formatters/list/binary_html_table.py
--rw-r--r--   0 root         (0) root         (0)      939 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/formatters/list/list.py
--rw-r--r--   0 root         (0) root         (0)    12687 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/formatters/list/search_table_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.001548 conan-2.0.3/conan/cli/printers/
--rw-r--r--   0 root         (0) root         (0)      331 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/printers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4741 2023-04-03 13:44:40.000000 conan-2.0.3/conan/cli/printers/graph.py
--rw-r--r--   0 root         (0) root         (0)      139 2023-04-03 13:44:40.000000 conan-2.0.3/conan/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.001548 conan-2.0.3/conan/internal/
--rw-r--r--   0 root         (0) root         (0)      419 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.001548 conan-2.0.3/conan/internal/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.003548 conan-2.0.3/conan/internal/api/new/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/api/new/__init__.py
--rw-r--r--   0 root         (0) root         (0)      293 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/api/new/alias_new.py
--rw-r--r--   0 root         (0) root         (0)     2716 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/api/new/autoools_exe.py
--rw-r--r--   0 root         (0) root         (0)     3781 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/api/new/autotools_lib.py
--rw-r--r--   0 root         (0) root         (0)     2133 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/api/new/basic.py
--rw-r--r--   0 root         (0) root         (0)     2066 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/api/new/bazel_exe.py
--rw-r--r--   0 root         (0) root         (0)     3596 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/api/new/bazel_lib.py
--rw-r--r--   0 root         (0) root         (0)     2732 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/api/new/cmake_exe.py
--rw-r--r--   0 root         (0) root         (0)     6875 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/api/new/cmake_lib.py
--rw-r--r--   0 root         (0) root         (0)     2334 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/api/new/meson_exe.py
--rw-r--r--   0 root         (0) root         (0)     2740 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/api/new/meson_lib.py
--rw-r--r--   0 root         (0) root         (0)     2207 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/api/new/msbuild_exe.py
--rw-r--r--   0 root         (0) root         (0)    12247 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/api/new/msbuild_lib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.003548 conan-2.0.3/conan/internal/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10068 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/cache/cache.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/cache/conan_reference_layout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.004548 conan-2.0.3/conan/internal/cache/db/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/cache/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3820 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/cache/db/cache_database.py
--rw-r--r--   0 root         (0) root         (0)     7931 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/cache/db/packages_table.py
--rw-r--r--   0 root         (0) root         (0)     5264 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/cache/db/recipes_table.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/cache/db/table.py
--rw-r--r--   0 root         (0) root         (0)     2476 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/conan_app.py
--rw-r--r--   0 root         (0) root         (0)     3410 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/deploy.py
--rw-r--r--   0 root         (0) root         (0)     2468 2023-04-03 13:44:40.000000 conan-2.0.3/conan/internal/integrity_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.004548 conan-2.0.3/conan/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.004548 conan-2.0.3/conan/tools/android/
--rw-r--r--   0 root         (0) root         (0)       50 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/android/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1138 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/android/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.005549 conan-2.0.3/conan/tools/apple/
--rw-r--r--   0 root         (0) root         (0)      534 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/apple/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11201 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/apple/apple.py
--rw-r--r--   0 root         (0) root         (0)     2907 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/apple/xcodebuild.py
--rw-r--r--   0 root         (0) root         (0)    16202 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/apple/xcodedeps.py
--rw-r--r--   0 root         (0) root         (0)     5683 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/apple/xcodetoolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.006549 conan-2.0.3/conan/tools/build/
--rw-r--r--   0 root         (0) root         (0)     4143 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/build/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11104 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/build/cppstd.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/build/cpu.py
--rw-r--r--   0 root         (0) root         (0)     2043 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/build/cross_building.py
--rw-r--r--   0 root         (0) root         (0)    15410 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/build/flags.py
--rw-r--r--   0 root         (0) root         (0)      563 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/build/stdcpp_library.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.007549 conan-2.0.3/conan/tools/cmake/
--rw-r--r--   0 root         (0) root         (0)      269 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/cmake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9956 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/cmake/cmake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.007549 conan-2.0.3/conan/tools/cmake/cmakedeps/
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/cmake/cmakedeps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7931 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/cmake/cmakedeps/cmakedeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.008549 conan-2.0.3/conan/tools/cmake/cmakedeps/templates/
--rw-r--r--   0 root         (0) root         (0)     3848 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/cmake/cmakedeps/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4451 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/cmake/cmakedeps/templates/config.py
--rw-r--r--   0 root         (0) root         (0)     1613 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/cmake/cmakedeps/templates/config_version.py
--rw-r--r--   0 root         (0) root         (0)     5802 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/cmake/cmakedeps/templates/macros.py
--rw-r--r--   0 root         (0) root         (0)    14925 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/cmake/cmakedeps/templates/target_configuration.py
--rw-r--r--   0 root         (0) root         (0)    19890 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/cmake/cmakedeps/templates/target_data.py
--rw-r--r--   0 root         (0) root         (0)     3916 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/cmake/cmakedeps/templates/targets.py
--rw-r--r--   0 root         (0) root         (0)     5365 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/cmake/file_api.py
--rw-r--r--   0 root         (0) root         (0)     4045 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/cmake/layout.py
--rw-r--r--   0 root         (0) root         (0)    14423 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/cmake/presets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.008549 conan-2.0.3/conan/tools/cmake/toolchain/
--rw-r--r--   0 root         (0) root         (0)       52 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/cmake/toolchain/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36011 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/cmake/toolchain/blocks.py
--rw-r--r--   0 root         (0) root         (0)    11043 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/cmake/toolchain/toolchain.py
--rw-r--r--   0 root         (0) root         (0)      171 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/cmake/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.009549 conan-2.0.3/conan/tools/env/
--rw-r--r--   0 root         (0) root         (0)      168 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/env/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25247 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/env/environment.py
--rw-r--r--   0 root         (0) root         (0)     3233 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/env/virtualbuildenv.py
--rw-r--r--   0 root         (0) root         (0)     3394 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/env/virtualrunenv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.010549 conan-2.0.3/conan/tools/files/
--rw-r--r--   0 root         (0) root         (0)      544 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/files/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1468 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/files/conandata.py
--rw-r--r--   0 root         (0) root         (0)     6009 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/files/copy_pattern.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/files/cpp_package.py
--rw-r--r--   0 root         (0) root         (0)    23908 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/files/files.py
--rw-r--r--   0 root         (0) root         (0)     3904 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/files/packager.py
--rw-r--r--   0 root         (0) root         (0)     5824 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/files/patches.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.010549 conan-2.0.3/conan/tools/files/symlinks/
--rw-r--r--   0 root         (0) root         (0)      148 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/files/symlinks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2456 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/files/symlinks/symlinks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.011549 conan-2.0.3/conan/tools/gnu/
--rw-r--r--   0 root         (0) root         (0)      274 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/gnu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6234 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/gnu/autotools.py
--rw-r--r--   0 root         (0) root         (0)     2954 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/gnu/autotoolsdeps.py
--rw-r--r--   0 root         (0) root         (0)    13040 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/gnu/autotoolstoolchain.py
--rw-r--r--   0 root         (0) root         (0)     3557 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/gnu/get_gnu_triplet.py
--rw-r--r--   0 root         (0) root         (0)     3596 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/gnu/gnudeps_flags.py
--rw-r--r--   0 root         (0) root         (0)     4029 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/gnu/pkgconfig.py
--rw-r--r--   0 root         (0) root         (0)    17816 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/gnu/pkgconfigdeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.012549 conan-2.0.3/conan/tools/google/
--rw-r--r--   0 root         (0) root         (0)      201 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/google/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1806 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/google/bazel.py
--rw-r--r--   0 root         (0) root         (0)    10956 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/google/bazeldeps.py
--rw-r--r--   0 root         (0) root         (0)      585 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/google/layout.py
--rw-r--r--   0 root         (0) root         (0)      857 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/google/toolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.012549 conan-2.0.3/conan/tools/intel/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/intel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6499 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/intel/intel_cc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.012549 conan-2.0.3/conan/tools/layout/
--rw-r--r--   0 root         (0) root         (0)      605 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/layout/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.012549 conan-2.0.3/conan/tools/meson/
--rw-r--r--   0 root         (0) root         (0)       98 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/meson/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4073 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/meson/helpers.py
--rw-r--r--   0 root         (0) root         (0)     3880 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/meson/meson.py
--rw-r--r--   0 root         (0) root         (0)    22075 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/meson/toolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.014549 conan-2.0.3/conan/tools/microsoft/
--rw-r--r--   0 root         (0) root         (0)      558 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/microsoft/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/microsoft/layout.py
--rw-r--r--   0 root         (0) root         (0)     3789 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/microsoft/msbuild.py
--rw-r--r--   0 root         (0) root         (0)    19194 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/microsoft/msbuilddeps.py
--rw-r--r--   0 root         (0) root         (0)     2962 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/microsoft/nmakedeps.py
--rw-r--r--   0 root         (0) root         (0)     4989 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/microsoft/nmaketoolchain.py
--rw-r--r--   0 root         (0) root         (0)      596 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/microsoft/subsystems.py
--rw-r--r--   0 root         (0) root         (0)    10844 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/microsoft/toolchain.py
--rw-r--r--   0 root         (0) root         (0)    13070 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/microsoft/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.014549 conan-2.0.3/conan/tools/premake/
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/premake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/premake/premake.py
--rw-r--r--   0 root         (0) root         (0)     5331 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/premake/premakedeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.014549 conan-2.0.3/conan/tools/qbs/
--rw-r--r--   0 root         (0) root         (0)      152 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/qbs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/qbs/qbs.py
--rw-r--r--   0 root         (0) root         (0)     9874 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/qbs/qbsprofile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.015550 conan-2.0.3/conan/tools/scm/
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/scm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8619 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/scm/git.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.015550 conan-2.0.3/conan/tools/system/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/system/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16286 2023-04-03 13:44:40.000000 conan-2.0.3/conan/tools/system/package_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:46.993548 conan-2.0.3/conan.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8324 2023-04-03 13:44:46.000000 conan-2.0.3/conan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9035 2023-04-03 13:44:46.000000 conan-2.0.3/conan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 13:44:46.000000 conan-2.0.3/conan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-03 13:44:46.000000 conan-2.0.3/conan.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      470 2023-04-03 13:44:46.000000 conan-2.0.3/conan.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-03 13:44:46.000000 conan-2.0.3/conan.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.016550 conan-2.0.3/conans/
--rw-r--r--   0 root         (0) root         (0)      201 2023-04-03 13:44:40.000000 conan-2.0.3/conans/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.017550 conan-2.0.3/conans/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.018550 conan-2.0.3/conans/client/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9791 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/cache/cache.py
--rw-r--r--   0 root         (0) root         (0)     2033 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/cache/editable.py
--rw-r--r--   0 root         (0) root         (0)     6843 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/cache/remote_registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.018550 conan-2.0.3/conans/client/cmd/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/cmd/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7619 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/cmd/export.py
--rw-r--r--   0 root         (0) root         (0)    12827 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/cmd/uploader.py
--rw-r--r--   0 root         (0) root         (0)      968 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/cmd/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.019550 conan-2.0.3/conans/client/conanfile/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/conanfile/__init__.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/conanfile/build.py
--rw-r--r--   0 root         (0) root         (0)     2208 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/conanfile/configure.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/conanfile/package.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.020550 conan-2.0.3/conans/client/conf/
--rw-r--r--   0 root         (0) root         (0)     6307 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9195 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/conf/config_installer.py
--rw-r--r--   0 root         (0) root         (0)    14016 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/conf/detect.py
--rw-r--r--   0 root         (0) root         (0)     5473 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/conf/detect_vs.py
--rw-r--r--   0 root         (0) root         (0)     1363 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/conf/required_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.020550 conan-2.0.3/conans/client/downloaders/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/downloaders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9235 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/downloaders/caching_file_downloader.py
--rw-r--r--   0 root         (0) root         (0)     3341 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/downloaders/download_cache.py
--rw-r--r--   0 root         (0) root         (0)     6124 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/downloaders/file_downloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.020550 conan-2.0.3/conans/client/generators/
--rw-r--r--   0 root         (0) root         (0)     8044 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/generators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.022550 conan-2.0.3/conans/client/graph/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4818 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/graph/build_mode.py
--rw-r--r--   0 root         (0) root         (0)     4571 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/graph/compatibility.py
--rw-r--r--   0 root         (0) root         (0)     3685 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/graph/compute_pid.py
--rw-r--r--   0 root         (0) root         (0)    11839 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)    16237 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/graph/graph_binaries.py
--rw-r--r--   0 root         (0) root         (0)    16599 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/graph/graph_builder.py
--rw-r--r--   0 root         (0) root         (0)     2626 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/graph/graph_error.py
--rw-r--r--   0 root         (0) root         (0)    11680 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/graph/install_graph.py
--rw-r--r--   0 root         (0) root         (0)     3877 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/graph/profile_node_definer.py
--rw-r--r--   0 root         (0) root         (0)     1524 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/graph/provides.py
--rw-r--r--   0 root         (0) root         (0)     6536 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/graph/proxy.py
--rw-r--r--   0 root         (0) root         (0)     5636 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/graph/python_requires.py
--rw-r--r--   0 root         (0) root         (0)     4692 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/graph/range_resolver.py
--rw-r--r--   0 root         (0) root         (0)     2595 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/hook_manager.py
--rw-r--r--   0 root         (0) root         (0)    21352 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/installer.py
--rw-r--r--   0 root         (0) root         (0)    15815 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/loader.py
--rw-r--r--   0 root         (0) root         (0)     1829 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/loader_txt.py
--rw-r--r--   0 root         (0) root         (0)     1860 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/migrations.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/pkg_sign.py
--rw-r--r--   0 root         (0) root         (0)    16751 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/profile_loader.py
--rw-r--r--   0 root         (0) root         (0)    10984 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/remote_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.023550 conan-2.0.3/conans/client/rest/
--rw-r--r--   0 root         (0) root         (0)      838 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5954 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/rest/auth_manager.py
--rw-r--r--   0 root         (0) root         (0)     6132 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/rest/client_routes.py
--rw-r--r--   0 root         (0) root         (0)     6894 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/rest/conan_requester.py
--rw-r--r--   0 root         (0) root         (0)     4245 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/rest/file_uploader.py
--rw-r--r--   0 root         (0) root         (0)     5388 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/rest/rest_client.py
--rw-r--r--   0 root         (0) root         (0)    10003 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/rest/rest_client_common.py
--rw-r--r--   0 root         (0) root         (0)    13493 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/rest/rest_client_v2.py
--rw-r--r--   0 root         (0) root         (0)     3606 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.023550 conan-2.0.3/conans/client/store/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/store/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4305 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/store/localdb.py
--rw-r--r--   0 root         (0) root         (0)     8798 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/subsystems.py
--rw-r--r--   0 root         (0) root         (0)     5457 2023-04-03 13:44:40.000000 conan-2.0.3/conans/client/userio.py
--rwxr-xr-x   0 root         (0) root         (0)      118 2023-04-03 13:44:40.000000 conan-2.0.3/conans/conan.py
--rw-r--r--   0 root         (0) root         (0)      699 2023-04-03 13:44:40.000000 conan-2.0.3/conans/conan_server.py
--rw-r--r--   0 root         (0) root         (0)     7819 2023-04-03 13:44:40.000000 conan-2.0.3/conans/errors.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-04-03 13:44:40.000000 conan-2.0.3/conans/migrations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.026551 conan-2.0.3/conans/model/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 13:44:40.000000 conan-2.0.3/conans/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21687 2023-04-03 13:44:40.000000 conan-2.0.3/conans/model/build_info.py
--rw-r--r--   0 root         (0) root         (0)    11676 2023-04-03 13:44:40.000000 conan-2.0.3/conans/model/conan_file.py
--rw-r--r--   0 root         (0) root         (0)     2775 2023-04-03 13:44:40.000000 conan-2.0.3/conans/model/conanfile_interface.py
--rw-r--r--   0 root         (0) root         (0)    29539 2023-04-03 13:44:40.000000 conan-2.0.3/conans/model/conf.py
--rw-r--r--   0 root         (0) root         (0)     5901 2023-04-03 13:44:40.000000 conan-2.0.3/conans/model/dependencies.py
--rw-r--r--   0 root         (0) root         (0)     9578 2023-04-03 13:44:40.000000 conan-2.0.3/conans/model/graph_lock.py
--rw-r--r--   0 root         (0) root         (0)    13067 2023-04-03 13:44:40.000000 conan-2.0.3/conans/model/info.py
--rw-r--r--   0 root         (0) root         (0)     5193 2023-04-03 13:44:40.000000 conan-2.0.3/conans/model/layout.py
--rw-r--r--   0 root         (0) root         (0)     4883 2023-04-03 13:44:40.000000 conan-2.0.3/conans/model/manifest.py
--rw-r--r--   0 root         (0) root         (0)    17065 2023-04-03 13:44:40.000000 conan-2.0.3/conans/model/options.py
--rw-r--r--   0 root         (0) root         (0)     3861 2023-04-03 13:44:40.000000 conan-2.0.3/conans/model/package_ref.py
--rw-r--r--   0 root         (0) root         (0)     2320 2023-04-03 13:44:40.000000 conan-2.0.3/conans/model/pkg_type.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-04-03 13:44:40.000000 conan-2.0.3/conans/model/profile.py
--rw-r--r--   0 root         (0) root         (0)     7583 2023-04-03 13:44:40.000000 conan-2.0.3/conans/model/recipe_ref.py
--rw-r--r--   0 root         (0) root         (0)    23711 2023-04-03 13:44:40.000000 conan-2.0.3/conans/model/requires.py
--rw-r--r--   0 root         (0) root         (0)     2171 2023-04-03 13:44:40.000000 conan-2.0.3/conans/model/rest_routes.py
--rw-r--r--   0 root         (0) root         (0)    13231 2023-04-03 13:44:40.000000 conan-2.0.3/conans/model/settings.py
--rw-r--r--   0 root         (0) root         (0)     6038 2023-04-03 13:44:40.000000 conan-2.0.3/conans/model/version.py
--rw-r--r--   0 root         (0) root         (0)     4350 2023-04-03 13:44:40.000000 conan-2.0.3/conans/model/version_range.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.026551 conan-2.0.3/conans/paths/
--rw-r--r--   0 root         (0) root         (0)     2184 2023-04-03 13:44:40.000000 conan-2.0.3/conans/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2883 2023-04-03 13:44:40.000000 conan-2.0.3/conans/pylint_plugin.py
--rw-r--r--   0 root         (0) root         (0)      252 2023-04-03 13:44:40.000000 conan-2.0.3/conans/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      146 2023-04-03 13:44:40.000000 conan-2.0.3/conans/requirements_dev.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-04-03 13:44:40.000000 conan-2.0.3/conans/requirements_server.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.027551 conan-2.0.3/conans/search/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 13:44:40.000000 conan-2.0.3/conans/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3814 2023-04-03 13:44:40.000000 conan-2.0.3/conans/search/query_parse.py
--rw-r--r--   0 root         (0) root         (0)     4340 2023-04-03 13:44:40.000000 conan-2.0.3/conans/search/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.027551 conan-2.0.3/conans/test/
--rw-r--r--   0 root         (0) root         (0)      203 2023-04-03 13:44:40.000000 conan-2.0.3/conans/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13174 2023-04-03 13:44:40.000000 conan-2.0.3/conans/test/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.028551 conan-2.0.3/conans/test/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 13:44:40.000000 conan-2.0.3/conans/test/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4868 2023-04-03 13:44:40.000000 conan-2.0.3/conans/test/utils/artifactory.py
--rw-r--r--   0 root         (0) root         (0)     4971 2023-04-03 13:44:40.000000 conan-2.0.3/conans/test/utils/mocks.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-04-03 13:44:40.000000 conan-2.0.3/conans/test/utils/profiles.py
--rw-r--r--   0 root         (0) root         (0)     2038 2023-04-03 13:44:40.000000 conan-2.0.3/conans/test/utils/scm.py
--rw-r--r--   0 root         (0) root         (0)     3858 2023-04-03 13:44:40.000000 conan-2.0.3/conans/test/utils/server_launcher.py
--rw-r--r--   0 root         (0) root         (0)     3071 2023-04-03 13:44:40.000000 conan-2.0.3/conans/test/utils/test_files.py
--rw-r--r--   0 root         (0) root         (0)    34736 2023-04-03 13:44:40.000000 conan-2.0.3/conans/test/utils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:44:47.029551 conan-2.0.3/conans/util/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 13:44:40.000000 conan-2.0.3/conans/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-04-03 13:44:40.000000 conan-2.0.3/conans/util/config_parser.py
--rw-r--r--   0 root         (0) root         (0)     1516 2023-04-03 13:44:40.000000 conan-2.0.3/conans/util/dates.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-04-03 13:44:40.000000 conan-2.0.3/conans/util/encrypt.py
--rw-r--r--   0 root         (0) root         (0)     1437 2023-04-03 13:44:40.000000 conan-2.0.3/conans/util/env.py
--rw-r--r--   0 root         (0) root         (0)    11263 2023-04-03 13:44:40.000000 conan-2.0.3/conans/util/files.py
--rw-r--r--   0 root         (0) root         (0)     3657 2023-04-03 13:44:40.000000 conan-2.0.3/conans/util/locks.py
--rw-r--r--   0 root         (0) root         (0)     3688 2023-04-03 13:44:40.000000 conan-2.0.3/conans/util/runners.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-04-03 13:44:40.000000 conan-2.0.3/conans/util/sha.py
--rw-r--r--   0 root         (0) root         (0)      325 2023-04-03 13:44:40.000000 conan-2.0.3/conans/util/thread.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-04-03 13:44:40.000000 conan-2.0.3/conans/util/windows.py
--rw-r--r--   0 root         (0) root         (0)      101 2023-04-03 13:44:47.030551 conan-2.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5058 2023-04-03 13:44:40.000000 conan-2.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.097133 conan-2.0.4/
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-04-11 14:41:51.000000 conan-2.0.4/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-11 14:41:51.000000 conan-2.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8324 2023-04-11 14:41:59.097133 conan-2.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6041 2023-04-11 14:41:51.000000 conan-2.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.052132 conan-2.0.4/conan/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-04-11 14:41:51.000000 conan-2.0.4/conan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.053132 conan-2.0.4/conan/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2360 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/conan_api.py
+-rw-r--r--   0 root         (0) root         (0)     5892 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/model.py
+-rw-r--r--   0 root         (0) root         (0)     6824 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/output.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.056132 conan-2.0.4/conan/api/subapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/cache.py
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/config.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/download.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/export.py
+-rw-r--r--   0 root         (0) root         (0)    11124 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/graph.py
+-rw-r--r--   0 root         (0) root         (0)     3144 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/install.py
+-rw-r--r--   0 root         (0) root         (0)     7652 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/list.py
+-rw-r--r--   0 root         (0) root         (0)     4784 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/local.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/lockfile.py
+-rw-r--r--   0 root         (0) root         (0)     4864 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/new.py
+-rw-r--r--   0 root         (0) root         (0)     4426 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/profiles.py
+-rw-r--r--   0 root         (0) root         (0)     4425 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/remotes.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/remove.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/search.py
+-rw-r--r--   0 root         (0) root         (0)     3907 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.057132 conan-2.0.4/conan/cli/
+-rw-r--r--   0 root         (0) root         (0)      397 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7473 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/args.py
+-rw-r--r--   0 root         (0) root         (0)    11022 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     7512 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.061132 conan-2.0.4/conan/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3161 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/build.py
+-rw-r--r--   0 root         (0) root         (0)     4419 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/cache.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/config.py
+-rw-r--r--   0 root         (0) root         (0)     8119 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/create.py
+-rw-r--r--   0 root         (0) root         (0)     3065 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/download.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/editable.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/export.py
+-rw-r--r--   0 root         (0) root         (0)     5483 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/export_pkg.py
+-rw-r--r--   0 root         (0) root         (0)     8437 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/inspect.py
+-rw-r--r--   0 root         (0) root         (0)     4666 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/install.py
+-rw-r--r--   0 root         (0) root         (0)     5192 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/list.py
+-rw-r--r--   0 root         (0) root         (0)     5381 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/lock.py
+-rw-r--r--   0 root         (0) root         (0)     4239 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/new.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/profile.py
+-rw-r--r--   0 root         (0) root         (0)    11692 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/remote.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/remove.py
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/search.py
+-rw-r--r--   0 root         (0) root         (0)      648 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/source.py
+-rw-r--r--   0 root         (0) root         (0)     3584 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/test.py
+-rw-r--r--   0 root         (0) root         (0)     3830 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/upload.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/exit_codes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.061132 conan-2.0.4/conan/cli/formatters/
+-rw-r--r--   0 root         (0) root         (0)      158 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/formatters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.062132 conan-2.0.4/conan/cli/formatters/graph/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/formatters/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5019 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/formatters/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/formatters/graph/graph_info_text.py
+-rw-r--r--   0 root         (0) root         (0)      144 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/formatters/graph/info_graph_dot.py
+-rw-r--r--   0 root         (0) root         (0)     5583 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/formatters/graph/info_graph_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.062132 conan-2.0.4/conan/cli/formatters/list/
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/formatters/list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4612 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/formatters/list/binary_html_table.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/formatters/list/list.py
+-rw-r--r--   0 root         (0) root         (0)    12834 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/formatters/list/search_table_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.063132 conan-2.0.4/conan/cli/printers/
+-rw-r--r--   0 root         (0) root         (0)      331 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/printers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4741 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/printers/graph.py
+-rw-r--r--   0 root         (0) root         (0)      139 2023-04-11 14:41:51.000000 conan-2.0.4/conan/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.063132 conan-2.0.4/conan/internal/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.063132 conan-2.0.4/conan/internal/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.065132 conan-2.0.4/conan/internal/api/new/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      293 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/alias_new.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/autoools_exe.py
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/autotools_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2843 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/basic.py
+-rw-r--r--   0 root         (0) root         (0)     2066 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/bazel_exe.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/bazel_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/cmake_exe.py
+-rw-r--r--   0 root         (0) root         (0)     7076 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/cmake_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/meson_exe.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/meson_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/msbuild_exe.py
+-rw-r--r--   0 root         (0) root         (0)    12247 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/msbuild_lib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.066132 conan-2.0.4/conan/internal/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10153 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/cache/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/cache/conan_reference_layout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.067133 conan-2.0.4/conan/internal/cache/db/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/cache/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3820 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/cache/db/cache_database.py
+-rw-r--r--   0 root         (0) root         (0)     7931 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/cache/db/packages_table.py
+-rw-r--r--   0 root         (0) root         (0)     5264 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/cache/db/recipes_table.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/cache/db/table.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/conan_app.py
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/deploy.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/integrity_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.067133 conan-2.0.4/conan/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.067133 conan-2.0.4/conan/tools/android/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/android/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/android/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.068132 conan-2.0.4/conan/tools/apple/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/apple/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11201 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/apple/apple.py
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/apple/xcodebuild.py
+-rw-r--r--   0 root         (0) root         (0)    16202 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/apple/xcodedeps.py
+-rw-r--r--   0 root         (0) root         (0)     5683 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/apple/xcodetoolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.069133 conan-2.0.4/conan/tools/build/
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/build/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11104 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/build/cppstd.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/build/cpu.py
+-rw-r--r--   0 root         (0) root         (0)     2043 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/build/cross_building.py
+-rw-r--r--   0 root         (0) root         (0)    15410 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/build/flags.py
+-rw-r--r--   0 root         (0) root         (0)      563 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/build/stdcpp_library.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.070133 conan-2.0.4/conan/tools/cmake/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9956 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/cmake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.070133 conan-2.0.4/conan/tools/cmake/cmakedeps/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/cmakedeps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8152 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/cmakedeps/cmakedeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.071133 conan-2.0.4/conan/tools/cmake/cmakedeps/templates/
+-rw-r--r--   0 root         (0) root         (0)     3848 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/cmakedeps/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4451 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/cmakedeps/templates/config.py
+-rw-r--r--   0 root         (0) root         (0)     1613 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/cmakedeps/templates/config_version.py
+-rw-r--r--   0 root         (0) root         (0)     5802 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/cmakedeps/templates/macros.py
+-rw-r--r--   0 root         (0) root         (0)    14925 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/cmakedeps/templates/target_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    19484 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/cmakedeps/templates/target_data.py
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/cmakedeps/templates/targets.py
+-rw-r--r--   0 root         (0) root         (0)     5365 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/file_api.py
+-rw-r--r--   0 root         (0) root         (0)     4045 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/layout.py
+-rw-r--r--   0 root         (0) root         (0)    14423 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/presets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.072133 conan-2.0.4/conan/tools/cmake/toolchain/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/toolchain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35862 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/toolchain/blocks.py
+-rw-r--r--   0 root         (0) root         (0)    11205 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/toolchain/toolchain.py
+-rw-r--r--   0 root         (0) root         (0)      171 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.073133 conan-2.0.4/conan/tools/env/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25269 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/env/environment.py
+-rw-r--r--   0 root         (0) root         (0)     3233 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/env/virtualbuildenv.py
+-rw-r--r--   0 root         (0) root         (0)     3394 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/env/virtualrunenv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.074133 conan-2.0.4/conan/tools/files/
+-rw-r--r--   0 root         (0) root         (0)      572 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/files/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1468 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/files/conandata.py
+-rw-r--r--   0 root         (0) root         (0)     6009 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/files/copy_pattern.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/files/cpp_package.py
+-rw-r--r--   0 root         (0) root         (0)    24621 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/files/files.py
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/files/packager.py
+-rw-r--r--   0 root         (0) root         (0)     5824 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/files/patches.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.074133 conan-2.0.4/conan/tools/files/symlinks/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/files/symlinks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/files/symlinks/symlinks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.075133 conan-2.0.4/conan/tools/gnu/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/gnu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6234 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/gnu/autotools.py
+-rw-r--r--   0 root         (0) root         (0)     2954 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/gnu/autotoolsdeps.py
+-rw-r--r--   0 root         (0) root         (0)    13040 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/gnu/autotoolstoolchain.py
+-rw-r--r--   0 root         (0) root         (0)     3557 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/gnu/get_gnu_triplet.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/gnu/gnudeps_flags.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/gnu/pkgconfig.py
+-rw-r--r--   0 root         (0) root         (0)    17816 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/gnu/pkgconfigdeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.076133 conan-2.0.4/conan/tools/google/
+-rw-r--r--   0 root         (0) root         (0)      201 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/google/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/google/bazel.py
+-rw-r--r--   0 root         (0) root         (0)    10956 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/google/bazeldeps.py
+-rw-r--r--   0 root         (0) root         (0)      585 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/google/layout.py
+-rw-r--r--   0 root         (0) root         (0)      857 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/google/toolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.076133 conan-2.0.4/conan/tools/intel/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/intel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6499 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/intel/intel_cc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.076133 conan-2.0.4/conan/tools/layout/
+-rw-r--r--   0 root         (0) root         (0)      605 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/layout/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.077133 conan-2.0.4/conan/tools/meson/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/meson/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4073 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/meson/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     3880 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/meson/meson.py
+-rw-r--r--   0 root         (0) root         (0)    22075 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/meson/toolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.078133 conan-2.0.4/conan/tools/microsoft/
+-rw-r--r--   0 root         (0) root         (0)      558 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/microsoft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/microsoft/layout.py
+-rw-r--r--   0 root         (0) root         (0)     3789 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/microsoft/msbuild.py
+-rw-r--r--   0 root         (0) root         (0)    19194 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/microsoft/msbuilddeps.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/microsoft/nmakedeps.py
+-rw-r--r--   0 root         (0) root         (0)     4989 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/microsoft/nmaketoolchain.py
+-rw-r--r--   0 root         (0) root         (0)      596 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/microsoft/subsystems.py
+-rw-r--r--   0 root         (0) root         (0)    10844 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/microsoft/toolchain.py
+-rw-r--r--   0 root         (0) root         (0)    13070 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/microsoft/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.078133 conan-2.0.4/conan/tools/premake/
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/premake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/premake/premake.py
+-rw-r--r--   0 root         (0) root         (0)    11503 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/premake/premakedeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.079133 conan-2.0.4/conan/tools/qbs/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/qbs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/qbs/qbs.py
+-rw-r--r--   0 root         (0) root         (0)     9874 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/qbs/qbsprofile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.079133 conan-2.0.4/conan/tools/scm/
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/scm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8619 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/scm/git.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.079133 conan-2.0.4/conan/tools/system/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/system/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16286 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/system/package_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.053132 conan-2.0.4/conan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8324 2023-04-11 14:41:58.000000 conan-2.0.4/conan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9035 2023-04-11 14:41:59.000000 conan-2.0.4/conan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 14:41:58.000000 conan-2.0.4/conan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-11 14:41:58.000000 conan-2.0.4/conan.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      470 2023-04-11 14:41:58.000000 conan-2.0.4/conan.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 14:41:58.000000 conan-2.0.4/conan.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.080133 conan-2.0.4/conans/
+-rw-r--r--   0 root         (0) root         (0)      201 2023-04-11 14:41:51.000000 conan-2.0.4/conans/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.083133 conan-2.0.4/conans/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.083133 conan-2.0.4/conans/client/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9791 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/cache/cache.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/cache/editable.py
+-rw-r--r--   0 root         (0) root         (0)     6843 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/cache/remote_registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.084133 conan-2.0.4/conans/client/cmd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/cmd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7619 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/cmd/export.py
+-rw-r--r--   0 root         (0) root         (0)    12827 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/cmd/uploader.py
+-rw-r--r--   0 root         (0) root         (0)      968 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/cmd/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.085133 conan-2.0.4/conans/client/conanfile/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/conanfile/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/conanfile/build.py
+-rw-r--r--   0 root         (0) root         (0)     2208 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/conanfile/configure.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/conanfile/package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.086133 conan-2.0.4/conans/client/conf/
+-rw-r--r--   0 root         (0) root         (0)     6307 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/conf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9195 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/conf/config_installer.py
+-rw-r--r--   0 root         (0) root         (0)    14016 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/conf/detect.py
+-rw-r--r--   0 root         (0) root         (0)     5473 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/conf/detect_vs.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/conf/required_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.086133 conan-2.0.4/conans/client/downloaders/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/downloaders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9235 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/downloaders/caching_file_downloader.py
+-rw-r--r--   0 root         (0) root         (0)     3341 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/downloaders/download_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6124 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/downloaders/file_downloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.086133 conan-2.0.4/conans/client/generators/
+-rw-r--r--   0 root         (0) root         (0)     8621 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/generators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.089133 conan-2.0.4/conans/client/graph/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4818 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/build_mode.py
+-rw-r--r--   0 root         (0) root         (0)     4571 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/compatibility.py
+-rw-r--r--   0 root         (0) root         (0)     3832 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/compute_pid.py
+-rw-r--r--   0 root         (0) root         (0)    12000 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)    16237 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/graph_binaries.py
+-rw-r--r--   0 root         (0) root         (0)    16785 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/graph_builder.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/graph_error.py
+-rw-r--r--   0 root         (0) root         (0)    11680 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/install_graph.py
+-rw-r--r--   0 root         (0) root         (0)     4163 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/profile_node_definer.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/provides.py
+-rw-r--r--   0 root         (0) root         (0)     6536 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/proxy.py
+-rw-r--r--   0 root         (0) root         (0)     5726 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/python_requires.py
+-rw-r--r--   0 root         (0) root         (0)     4692 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/range_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/hook_manager.py
+-rw-r--r--   0 root         (0) root         (0)    21352 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/installer.py
+-rw-r--r--   0 root         (0) root         (0)    15815 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/loader.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/loader_txt.py
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/migrations.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/pkg_sign.py
+-rw-r--r--   0 root         (0) root         (0)    16751 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/profile_loader.py
+-rw-r--r--   0 root         (0) root         (0)    11423 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/remote_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.090133 conan-2.0.4/conans/client/rest/
+-rw-r--r--   0 root         (0) root         (0)      838 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5987 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/rest/auth_manager.py
+-rw-r--r--   0 root         (0) root         (0)     6132 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/rest/client_routes.py
+-rw-r--r--   0 root         (0) root         (0)     6894 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/rest/conan_requester.py
+-rw-r--r--   0 root         (0) root         (0)     4245 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/rest/file_uploader.py
+-rw-r--r--   0 root         (0) root         (0)     5388 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/rest/rest_client.py
+-rw-r--r--   0 root         (0) root         (0)    10011 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/rest/rest_client_common.py
+-rw-r--r--   0 root         (0) root         (0)    13590 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/rest/rest_client_v2.py
+-rw-r--r--   0 root         (0) root         (0)     3606 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.090133 conan-2.0.4/conans/client/store/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/store/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4305 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/store/localdb.py
+-rw-r--r--   0 root         (0) root         (0)     8798 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/subsystems.py
+-rw-r--r--   0 root         (0) root         (0)     5457 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/userio.py
+-rwxr-xr-x   0 root         (0) root         (0)      118 2023-04-11 14:41:51.000000 conan-2.0.4/conans/conan.py
+-rw-r--r--   0 root         (0) root         (0)      699 2023-04-11 14:41:51.000000 conan-2.0.4/conans/conan_server.py
+-rw-r--r--   0 root         (0) root         (0)     7819 2023-04-11 14:41:51.000000 conan-2.0.4/conans/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-04-11 14:41:51.000000 conan-2.0.4/conans/migrations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.093133 conan-2.0.4/conans/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21687 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/build_info.py
+-rw-r--r--   0 root         (0) root         (0)    11676 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/conan_file.py
+-rw-r--r--   0 root         (0) root         (0)     2775 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/conanfile_interface.py
+-rw-r--r--   0 root         (0) root         (0)    29539 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/conf.py
+-rw-r--r--   0 root         (0) root         (0)     5901 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/dependencies.py
+-rw-r--r--   0 root         (0) root         (0)     9578 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/graph_lock.py
+-rw-r--r--   0 root         (0) root         (0)    13067 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/info.py
+-rw-r--r--   0 root         (0) root         (0)     5193 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/layout.py
+-rw-r--r--   0 root         (0) root         (0)     4883 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    17065 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/options.py
+-rw-r--r--   0 root         (0) root         (0)     3861 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/package_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/pkg_type.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/profile.py
+-rw-r--r--   0 root         (0) root         (0)     7583 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/recipe_ref.py
+-rw-r--r--   0 root         (0) root         (0)    23711 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/requires.py
+-rw-r--r--   0 root         (0) root         (0)     2171 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/rest_routes.py
+-rw-r--r--   0 root         (0) root         (0)    13231 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/settings.py
+-rw-r--r--   0 root         (0) root         (0)     6038 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/version.py
+-rw-r--r--   0 root         (0) root         (0)     4350 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/version_range.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.093133 conan-2.0.4/conans/paths/
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-04-11 14:41:51.000000 conan-2.0.4/conans/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2023-04-11 14:41:51.000000 conan-2.0.4/conans/pylint_plugin.py
+-rw-r--r--   0 root         (0) root         (0)      252 2023-04-11 14:41:51.000000 conan-2.0.4/conans/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      146 2023-04-11 14:41:51.000000 conan-2.0.4/conans/requirements_dev.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-11 14:41:51.000000 conan-2.0.4/conans/requirements_server.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.094133 conan-2.0.4/conans/search/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3814 2023-04-11 14:41:51.000000 conan-2.0.4/conans/search/query_parse.py
+-rw-r--r--   0 root         (0) root         (0)     4384 2023-04-11 14:41:51.000000 conan-2.0.4/conans/search/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.094133 conan-2.0.4/conans/test/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-04-11 14:41:51.000000 conan-2.0.4/conans/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13174 2023-04-11 14:41:51.000000 conan-2.0.4/conans/test/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.095133 conan-2.0.4/conans/test/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/test/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4868 2023-04-11 14:41:51.000000 conan-2.0.4/conans/test/utils/artifactory.py
+-rw-r--r--   0 root         (0) root         (0)     4971 2023-04-11 14:41:51.000000 conan-2.0.4/conans/test/utils/mocks.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-04-11 14:41:51.000000 conan-2.0.4/conans/test/utils/profiles.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-04-11 14:41:51.000000 conan-2.0.4/conans/test/utils/scm.py
+-rw-r--r--   0 root         (0) root         (0)     3858 2023-04-11 14:41:51.000000 conan-2.0.4/conans/test/utils/server_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-04-11 14:41:51.000000 conan-2.0.4/conans/test/utils/test_files.py
+-rw-r--r--   0 root         (0) root         (0)    34736 2023-04-11 14:41:51.000000 conan-2.0.4/conans/test/utils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.096134 conan-2.0.4/conans/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/config_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/dates.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/encrypt.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/env.py
+-rw-r--r--   0 root         (0) root         (0)    11263 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/files.py
+-rw-r--r--   0 root         (0) root         (0)     3657 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/locks.py
+-rw-r--r--   0 root         (0) root         (0)     3688 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/runners.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/sha.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/thread.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/windows.py
+-rw-r--r--   0 root         (0) root         (0)      101 2023-04-11 14:41:59.097133 conan-2.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     5058 2023-04-11 14:41:51.000000 conan-2.0.4/setup.py
```

### Comparing `conan-2.0.3/LICENSE.md` & `conan-2.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/PKG-INFO` & `conan-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan
-Version: 2.0.3
+Version: 2.0.4
 Summary: Conan C/C++ package manager
 Home-page: https://conan.io
 Author: JFrog LTD
 Author-email: luism@jfrog.com
 License: MIT
 Project-URL: Documentation, https://docs.conan.io
 Project-URL: Source, https://github.com/conan-io/conan
```

### Comparing `conan-2.0.3/README.md` & `conan-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/api/conan_api.py` & `conan-2.0.4/conan/api/conan_api.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/api/model.py` & `conan-2.0.4/conan/api/model.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/api/output.py` & `conan-2.0.4/conan/api/output.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/api/subapi/cache.py` & `conan-2.0.4/conan/api/subapi/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         :param download: boolen, remove the "download (.tgz)" folder if True
         :param temp: boolean, remove the temporary folders
         :return:
         """
 
         app = ConanApp(self.conan_api.cache_folder)
         if temp:
-            shutil.rmtree(app.cache.temp_folder)
+            rmdir(app.cache.temp_folder)
         for ref, ref_bundle in package_list.refs():
             ref_layout = app.cache.ref_layout(ref)
             if source:
                 rmdir(ref_layout.source())
             if download:
                 rmdir(ref_layout.download_export())
             for pref, _ in package_list.prefs(ref, ref_bundle):
```

### Comparing `conan-2.0.3/conan/api/subapi/config.py` & `conan-2.0.4/conan/api/subapi/config.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/api/subapi/download.py` & `conan-2.0.4/conan/api/subapi/download.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/api/subapi/export.py` & `conan-2.0.4/conan/api/subapi/export.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/api/subapi/graph.py` & `conan-2.0.4/conan/api/subapi/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 
 from conan.api.output import ConanOutput
 from conan.internal.conan_app import ConanApp
-from conans.client.graph.graph import Node, RECIPE_CONSUMER, CONTEXT_HOST, RECIPE_VIRTUAL
+from conans.client.graph.graph import Node, RECIPE_CONSUMER, CONTEXT_HOST, RECIPE_VIRTUAL, \
+    CONTEXT_BUILD
 from conans.client.graph.graph_binaries import GraphBinariesAnalyzer
 from conans.client.graph.graph_builder import DepsGraphBuilder
 from conans.client.graph.profile_node_definer import initialize_conanfile_profile, consumer_definer
 from conans.client.loader import parse_conanfile
 
 from conans.errors import ConanException
 
@@ -31,23 +32,24 @@
                                                  user=user,
                                                  channel=channel,
                                                  graph_lock=lockfile,
                                                  remotes=remotes,
                                                  update=update)
             ref = RecipeReference(conanfile.name, conanfile.version,
                                   conanfile.user, conanfile.channel)
-            initialize_conanfile_profile(conanfile, profile_build, profile_host, CONTEXT_HOST,
+            context = CONTEXT_BUILD if is_build_require else CONTEXT_HOST
+            initialize_conanfile_profile(conanfile, profile_build, profile_host, context,
                                          is_build_require, ref)
             if ref.name:
                 profile_host.options.scope(ref)
-            root_node = Node(ref, conanfile, context=CONTEXT_HOST, recipe=RECIPE_CONSUMER, path=path)
+            root_node = Node(ref, conanfile, context=context, recipe=RECIPE_CONSUMER, path=path)
             root_node.should_build = True  # It is a consumer, this is something we are building
         else:
             conanfile = app.loader.load_conanfile_txt(path)
-            consumer_definer(conanfile, profile_host)
+            consumer_definer(conanfile, profile_host, profile_build)
             root_node = Node(None, conanfile, context=CONTEXT_HOST, recipe=RECIPE_CONSUMER,
                              path=path)
         return root_node
 
     def load_root_test_conanfile(self, path, tested_reference, profile_host, profile_build,
                                  update=None, remotes=None, lockfile=None,
                                  tested_python_requires=None):
@@ -82,20 +84,20 @@
         conanfile.tested_reference_str = repr(tested_reference)
 
         ref = RecipeReference(conanfile.name, conanfile.version, tested_reference.user,
                               tested_reference.channel)
         root_node = Node(ref, conanfile, recipe=RECIPE_CONSUMER, context=CONTEXT_HOST, path=path)
         return root_node
 
-    def _load_root_virtual_conanfile(self, profile_host, requires=None, tool_requires=None):
+    def _load_root_virtual_conanfile(self, profile_host, profile_build, requires, tool_requires):
         if not requires and not tool_requires:
             raise ConanException("Provide requires or tool_requires")
         app = ConanApp(self.conan_api.cache_folder)
         conanfile = app.loader.load_virtual(requires=requires,  tool_requires=tool_requires)
-        consumer_definer(conanfile, profile_host)
+        consumer_definer(conanfile, profile_host, profile_build)
         root_node = Node(ref=None, conanfile=conanfile, context=CONTEXT_HOST, recipe=RECIPE_VIRTUAL)
         return root_node
 
     @staticmethod
     def _scope_options(profile, requires, tool_requires):
         """
         Command line helper to scope options when ``command -o myoption=myvalue`` is used,
@@ -113,15 +115,16 @@
         requires = [RecipeReference.loads(r) if isinstance(r, str) else r for r in requires] \
             if requires else None
         tool_requires = [RecipeReference.loads(r) if isinstance(r, str) else r
                          for r in tool_requires] if tool_requires else None
 
         self._scope_options(profile_host, requires=requires, tool_requires=tool_requires)
         root_node = self._load_root_virtual_conanfile(requires=requires, tool_requires=tool_requires,
-                                                      profile_host=profile_host)
+                                                      profile_host=profile_host,
+                                                      profile_build=profile_build)
 
         # check_updates = args.check_updates if "check_updates" in args else False
         deps_graph = self.load_graph(root_node, profile_host=profile_host,
                                      profile_build=profile_build,
                                      lockfile=lockfile,
                                      remotes=remotes,
                                      update=update,
```

### Comparing `conan-2.0.3/conan/api/subapi/install.py` & `conan-2.0.4/conan/api/subapi/install.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/api/subapi/list.py` & `conan-2.0.4/conan/api/subapi/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/api/subapi/local.py` & `conan-2.0.4/conan/api/subapi/local.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/api/subapi/lockfile.py` & `conan-2.0.4/conan/api/subapi/lockfile.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/api/subapi/new.py` & `conan-2.0.4/conan/api/subapi/new.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,17 +80,22 @@
         return template_files, non_template_files
 
     @staticmethod
     def render(template_files, definitions):
         result = {}
         name = definitions.get("name", "Pkg")
         definitions["conan_version"] = __version__
-        requires = definitions.get("requires")  # Convert to list, and forget about it
-        if requires:
-            definitions["requires"] = [requires] if isinstance(requires, str) else requires
+
+        def ensure_list(key):
+            value = definitions.get(key)  # Convert to list, and forget about it
+            if value:
+                definitions[key] = [value] if isinstance(value, str) else value
+
+        ensure_list("requires")
+        ensure_list("tool_requires")
 
         def as_package_name(n):
             return n.replace("-", "_").replace("+", "_").replace(".", "_")
 
         def as_name(ref):
             ref = as_package_name(ref)
             if '/' in ref:
```

### Comparing `conan-2.0.3/conan/api/subapi/profiles.py` & `conan-2.0.4/conan/api/subapi/profiles.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/api/subapi/remotes.py` & `conan-2.0.4/conan/api/subapi/remotes.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/api/subapi/remove.py` & `conan-2.0.4/conan/api/subapi/remove.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/api/subapi/search.py` & `conan-2.0.4/conan/api/subapi/search.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/api/subapi/upload.py` & `conan-2.0.4/conan/api/subapi/upload.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/args.py` & `conan-2.0.4/conan/cli/args.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/cli.py` & `conan-2.0.4/conan/cli/cli.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/command.py` & `conan-2.0.4/conan/cli/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,16 +113,16 @@
             LEVEL_STATUS, LEVEL_VERBOSE, LEVEL_DEBUG, LEVEL_TRACE
 
         levels = {"quiet": LEVEL_QUIET,  # -vquiet 80
                   "error": LEVEL_ERROR,  # -verror 70
                   "warning": LEVEL_WARNING,  # -vwaring 60
                   "notice": LEVEL_NOTICE,  # -vnotice 50
                   "status": LEVEL_STATUS,  # -vstatus 40
+                  None: LEVEL_STATUS,  # -v 40
                   "verbose": LEVEL_VERBOSE,  # -vverbose 30
-                  None: LEVEL_VERBOSE,  # -v 30
                   "debug": LEVEL_DEBUG,  # -vdebug 20
                   "v": LEVEL_DEBUG,  # -vv 20
                   "trace": LEVEL_TRACE,  # -vtrace 10
                   "vv": LEVEL_TRACE,  # -vvv 10
                   }
 
         level = levels.get(args.v)
```

### Comparing `conan-2.0.3/conan/cli/commands/build.py` & `conan-2.0.4/conan/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/commands/cache.py` & `conan-2.0.4/conan/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/commands/config.py` & `conan-2.0.4/conan/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/commands/create.py` & `conan-2.0.4/conan/cli/commands/create.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/commands/download.py` & `conan-2.0.4/conan/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/commands/editable.py` & `conan-2.0.4/conan/cli/commands/editable.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/commands/export.py` & `conan-2.0.4/conan/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/commands/export_pkg.py` & `conan-2.0.4/conan/cli/commands/export_pkg.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/commands/graph.py` & `conan-2.0.4/conan/cli/commands/graph.py`

 * *Files 7% similar despite different names*

```diff
@@ -114,14 +114,16 @@
                            help="Check if there are recipe updates")
     subparser.add_argument("--filter", action="append",
                            help="Show only the specified fields")
     subparser.add_argument("--package-filter", action="append",
                            help='Print information only for packages that match the patterns')
     subparser.add_argument("--deploy", action="append",
                            help='Deploy using the provided deployer to the output folder')
+    subparser.add_argument("--build-require", action='store_true', default=False,
+                           help='Whether the provided reference is a build-require')
     args = parser.parse_args(*args)
 
     # parameter validation
     validate_common_graph_args(args)
     if args.format in ("html", "dot") and args.filter:
         raise ConanException(f"Formatted output '{args.format}' cannot filter fields")
 
@@ -137,15 +139,16 @@
     profile_host, profile_build = conan_api.profiles.get_profiles_from_args(args)
 
     if path:
         deps_graph = conan_api.graph.load_graph_consumer(path, args.name, args.version,
                                                          args.user, args.channel,
                                                          profile_host, profile_build, lockfile,
                                                          remotes, args.update,
-                                                         check_updates=args.check_updates)
+                                                         check_updates=args.check_updates,
+                                                         is_build_require=args.build_require)
     else:
         deps_graph = conan_api.graph.load_graph_requires(args.requires, args.tool_requires,
                                                          profile_host, profile_build, lockfile,
                                                          remotes, args.update,
                                                          check_updates=args.check_updates)
     print_graph_basic(deps_graph)
     if deps_graph.error:
```

### Comparing `conan-2.0.3/conan/cli/commands/inspect.py` & `conan-2.0.4/conan/cli/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/commands/install.py` & `conan-2.0.4/conan/cli/commands/install.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     common_graph_args(parser)
     parser.add_argument("-g", "--generator", action="append",
                         help='Generators to use')
     parser.add_argument("-of", "--output-folder",
                         help='The root output folder for generated and build files')
     parser.add_argument("--deploy", action="append",
                         help='Deploy using the provided deployer to the output folder')
+    parser.add_argument("--build-require", action='store_true', default=False,
+                        help='Whether the provided reference is a build-require')
     args = parser.parse_args(*args)
 
     validate_common_graph_args(args)
     cwd = os.getcwd()
 
     if args.path:
         path = conan_api.local.get_conanfile_path(args.path, cwd, py=None)
@@ -60,15 +62,16 @@
                                                partial=args.lockfile_partial)
     profile_host, profile_build = conan_api.profiles.get_profiles_from_args(args)
     print_profiles(profile_host, profile_build)
     if path:
         deps_graph = conan_api.graph.load_graph_consumer(path, args.name, args.version,
                                                          args.user, args.channel,
                                                          profile_host, profile_build, lockfile,
-                                                         remotes, args.update)
+                                                         remotes, args.update,
+                                                         is_build_require=args.build_require)
     else:
         deps_graph = conan_api.graph.load_graph_requires(args.requires, args.tool_requires,
                                                          profile_host, profile_build, lockfile,
                                                          remotes, args.update)
     print_graph_basic(deps_graph)
     deps_graph.report_graph_error()
     conan_api.graph.analyze_binaries(deps_graph, args.build, remotes=remotes, update=args.update,
```

### Comparing `conan-2.0.3/conan/cli/commands/list.py` & `conan-2.0.4/conan/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/commands/lock.py` & `conan-2.0.4/conan/cli/commands/lock.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 @conan_subcommand()
 def lock_create(conan_api, parser, subparser, *args):
     """
     Create a lockfile from a conanfile or a reference.
     """
     common_graph_args(subparser)
+    subparser.add_argument("--build-require", action='store_true', default=False,
+                           help='Whether the provided reference is a build-require')
     args = parser.parse_args(*args)
 
     # parameter validation
     validate_common_graph_args(args)
 
     cwd = os.getcwd()
     path = conan_api.local.get_conanfile_path(args.path, cwd, py=None) if args.path else None
@@ -35,15 +37,16 @@
                                                cwd=cwd, partial=True)
     profile_host, profile_build = conan_api.profiles.get_profiles_from_args(args)
 
     if path:
         graph = conan_api.graph.load_graph_consumer(path, args.name, args.version,
                                                     args.user, args.channel,
                                                     profile_host, profile_build, lockfile,
-                                                    remotes, args.build, args.update)
+                                                    remotes, args.build, args.update,
+                                                    is_build_require=args.build_require)
     else:
         graph = conan_api.graph.load_graph_requires(args.requires, args.tool_requires,
                                                     profile_host, profile_build, lockfile,
                                                     remotes, args.build, args.update)
 
     print_graph_basic(graph)
     graph.report_graph_error()
```

### Comparing `conan-2.0.3/conan/cli/commands/new.py` & `conan-2.0.4/conan/cli/commands/new.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             template_vars = []
             for _, templ_str in template_files.items():
                 env = Environment()
                 ast = env.parse(templ_str)
                 template_vars.extend(meta.find_undeclared_variables(ast))
 
             injected_vars = {"conan_version", "package_name", "as_name"}
-            optional_vars = {"requires"}
+            optional_vars = {"requires", "tool_requires"}
             template_vars = list(set(template_vars) - injected_vars - optional_vars)
             template_vars.sort()
             return template_vars
 
         raise ConanException("Missing definitions for the template. "
                              "Required definitions are: {}"
                              .format(", ".join("'{}'".format(var) for var in get_template_vars())))
```

### Comparing `conan-2.0.3/conan/cli/commands/profile.py` & `conan-2.0.4/conan/cli/commands/profile.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/commands/remote.py` & `conan-2.0.4/conan/cli/commands/remote.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/commands/remove.py` & `conan-2.0.4/conan/cli/commands/remove.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from conan.api.conan_api import ConanAPI
 from conan.api.model import ListPattern
 from conan.cli.command import conan_command, OnceArgument
 from conans.client.userio import UserInput
+from conans.errors import ConanException
 
 
 @conan_command(group="Consumer")
 def remove(conan_api: ConanAPI, parser, *args):
     """
     Remove recipes or packages from local cache or a remote.
 
@@ -32,14 +33,16 @@
     def confirmation(message):
         return args.confirm or ui.request_boolean(message)
 
     ref_pattern = ListPattern(args.reference, rrev="*", prev="*")
     select_bundle = conan_api.list.select(ref_pattern, args.package_query, remote)
 
     if ref_pattern.package_id is None:
+        if args.package_query is not None:
+            raise ConanException('--package-query supplied but the pattern does not match packages')
         for ref, _ in select_bundle.refs():
             if confirmation("Remove the recipe and all the packages of '{}'?"
                             "".format(ref.repr_notime())):
                 conan_api.remove.recipe(ref, remote=remote)
     else:
         for ref, ref_bundle in select_bundle.refs():
             for pref, _ in select_bundle.prefs(ref, ref_bundle):
```

### Comparing `conan-2.0.3/conan/cli/commands/search.py` & `conan-2.0.4/conan/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/commands/source.py` & `conan-2.0.4/conan/cli/commands/source.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/commands/test.py` & `conan-2.0.4/conan/cli/commands/test.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/commands/upload.py` & `conan-2.0.4/conan/cli/commands/upload.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/formatters/graph/graph.py` & `conan-2.0.4/conan/cli/formatters/graph/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/formatters/graph/graph_info_text.py` & `conan-2.0.4/conan/cli/formatters/graph/graph_info_text.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/formatters/graph/info_graph_html.py` & `conan-2.0.4/conan/cli/formatters/graph/info_graph_html.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/formatters/list/binary_html_table.py` & `conan-2.0.4/conan/cli/formatters/list/binary_html_table.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/formatters/list/list.py` & `conan-2.0.4/conan/cli/formatters/list/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/cli/formatters/list/search_table_html.py` & `conan-2.0.4/conan/cli/formatters/list/search_table_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,20 +164,23 @@
             for (const [package, packageInfo] of Object.entries(revInfo["packages"])) {
 
                 if (!isFiltered(packageInfo["info"], filters)) {
                     packageList += `<div class="bg-light">`;
                     packageList += `<h6 class="mb-1">${package}</h6>`;
                     packageList += `${getInfoFieldsBadges(packageInfo["info"])}`;
 
-                    packageList += `<br><br><b>Package revisions:</>`;
-                    packageList += `<ul>`;
-                    for (const [packageRev, packageRevInfo] of Object.entries(packageInfo["revisions"])) {
-                        packageList += `<li>${packageRev}&nbsp(${formatDate(packageRevInfo["timestamp"])})</li>`;
+                    packageList += `<br><br>`;
+                    if ("revisions" in packageInfo) {
+                        packageList += `<br><br><b>Package revisions:</>`;
+                        packageList += `<ul>`;
+                        for (const [packageRev, packageRevInfo] of Object.entries(packageInfo["revisions"])) {
+                            packageList += `<li>${packageRev}&nbsp(${formatDate(packageRevInfo["timestamp"])})</li>`;
+                        }
+                        packageList += `</ul>`;
                     }
-                    packageList += `</ul>`;
                     packageList += `</div>`;
                     packageList += `<br>`;
                 }
             }
             return packageList;
         }
```

### Comparing `conan-2.0.3/conan/cli/printers/graph.py` & `conan-2.0.4/conan/cli/printers/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/internal/api/new/autoools_exe.py` & `conan-2.0.4/conan/internal/api/new/autoools_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/internal/api/new/autotools_lib.py` & `conan-2.0.4/conan/internal/api/new/autotools_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/internal/api/new/basic.py` & `conan-2.0.4/conan/internal/api/new/basic.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,14 +25,29 @@
         {% endfor %}
         {% else -%}
         # Uncommenting this line will add the zlib/1.2.13 dependency to your project
         # self.requires("zlib/1.2.13")
         pass
         {%- endif %}
 
+    # The build_requirements() method is functionally equivalent to the requirements() one,
+    # being executed just after it. It's a good place to define tool requirements,
+    # dependencies necessary at build time, not at application runtime
+    def build_requirements(self):
+        # Each call to self.tool_requires() will add the corresponding build requirement
+        {% if tool_requires is defined -%}
+        {% for require in tool_requires -%}
+        self.tool_requires("{{ require }}")
+        {% endfor %}
+        {% else -%}
+        # Uncommenting this line will add the cmake >=3.15 build dependency to your project
+        # self.requires("cmake/[>=3.15]")
+        pass
+        {%- endif %}
+
     # The purpose of generate() is to prepare the build, generating the necessary files, such as
     # Files containing information to locate the dependencies, environment activation scripts,
     # and specific build system files among others
     def generate(self):
         pass
 
     # This method is used to build the source code of the recipe using the desired commands.
```

### Comparing `conan-2.0.3/conan/internal/api/new/bazel_exe.py` & `conan-2.0.4/conan/internal/api/new/bazel_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/internal/api/new/bazel_lib.py` & `conan-2.0.4/conan/internal/api/new/bazel_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/internal/api/new/cmake_exe.py` & `conan-2.0.4/conan/internal/api/new/cmake_exe.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,21 @@
 
     {% if requires is defined -%}
     def requirements(self):
         {% for require in requires -%}
         self.requires("{{ require }}")
         {% endfor %}
     {%- endif %}
+
+    {% if tool_requires is defined -%}
+    def build_requirements(self):
+        {% for require in tool_requires -%}
+        self.tool_requires("{{ require }}")
+        {% endfor %}
+    {%- endif %}
 '''
 
 cmake_exe_v2 = """cmake_minimum_required(VERSION 3.15)
 project({{name}} CXX)
 
 {% if requires is defined -%}
 {% for require in requires -%}
```

### Comparing `conan-2.0.3/conan/internal/api/new/cmake_lib.py` & `conan-2.0.4/conan/internal/api/new/cmake_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,22 @@
 
     {% if requires is defined -%}
     def requirements(self):
         {% for require in requires -%}
         self.requires("{{ require }}")
         {% endfor %}
     {%- endif %}
+
+    {% if tool_requires is defined -%}
+    def build_requirements(self):
+        {% for require in tool_requires -%}
+        self.tool_requires("{{ require }}")
+        {% endfor %}
+    {%- endif %}
+
 '''
 
 cmake_v2 = """cmake_minimum_required(VERSION 3.15)
 project({{name}} CXX)
 
 {% if requires is defined -%}
 {% for require in requires -%}
```

### Comparing `conan-2.0.3/conan/internal/api/new/meson_exe.py` & `conan-2.0.4/conan/internal/api/new/meson_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/internal/api/new/meson_lib.py` & `conan-2.0.4/conan/internal/api/new/meson_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/internal/api/new/msbuild_exe.py` & `conan-2.0.4/conan/internal/api/new/msbuild_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/internal/api/new/msbuild_lib.py` & `conan-2.0.4/conan/internal/api/new/msbuild_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/internal/cache/cache.py` & `conan-2.0.4/conan/internal/cache/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,14 +166,15 @@
         return self._db.get_recipe_timestamp(ref)
 
     def get_package_timestamp(self, pref):
         return self._db.get_package_timestamp(pref)
 
     def remove_recipe(self, layout: RecipeLayout):
         layout.remove()
+        # FIXME: This is clearing package binaries from DB, but not from disk/layout
         self._db.remove_recipe(layout.reference)
 
     def remove_package(self, layout: RecipeLayout):
         layout.remove()
         self._db.remove_package(layout.reference)
 
     def assign_prev(self, layout: PackageLayout):
```

### Comparing `conan-2.0.3/conan/internal/cache/conan_reference_layout.py` & `conan-2.0.4/conan/internal/cache/conan_reference_layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/internal/cache/db/cache_database.py` & `conan-2.0.4/conan/internal/cache/db/cache_database.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/internal/cache/db/packages_table.py` & `conan-2.0.4/conan/internal/cache/db/packages_table.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/internal/cache/db/recipes_table.py` & `conan-2.0.4/conan/internal/cache/db/recipes_table.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/internal/cache/db/table.py` & `conan-2.0.4/conan/internal/cache/db/table.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/internal/conan_app.py` & `conan-2.0.4/conan/internal/conan_app.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/internal/deploy.py` & `conan-2.0.4/conan/internal/deploy.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     import shutil
 
     conanfile = graph.root.conanfile
     conanfile.output.info(f"Conan built-in full deployer to {output_folder}")
     for dep in conanfile.dependencies.values():
         if dep.package_folder is None:
             continue
-        folder_name = os.path.join(dep.context, dep.ref.name, str(dep.ref.version))
+        folder_name = os.path.join("full_deploy", dep.context, dep.ref.name, str(dep.ref.version))
         build_type = dep.info.settings.get_safe("build_type")
         arch = dep.info.settings.get_safe("arch")
         if build_type:
             folder_name = os.path.join(folder_name, build_type)
         if arch:
             folder_name = os.path.join(folder_name, arch)
         new_folder = os.path.join(output_folder, folder_name)
@@ -76,14 +76,15 @@
     Deploys to output_folder a single package,
     """
     # TODO: This deployer needs to be put somewhere else
     # TODO: Document that this will NOT work with editables
     import os
     import shutil
 
+    output_folder = os.path.join(output_folder, "direct_deploy")
     conanfile = graph.root.conanfile
     conanfile.output.info(f"Conan built-in pkg deployer to {output_folder}")
     # If the argument is --requires, the current conanfile is a virtual one with 1 single
     # dependency, the "reference" package. If the argument is a local path, then all direct
     # dependencies
     for dep in conanfile.dependencies.filter({"direct": True}).values():
         new_folder = os.path.join(output_folder, dep.ref.name)
```

### Comparing `conan-2.0.3/conan/internal/integrity_check.py` & `conan-2.0.4/conan/internal/integrity_check.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/android/utils.py` & `conan-2.0.4/conan/tools/android/utils.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/apple/__init__.py` & `conan-2.0.4/conan/tools/apple/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/apple/apple.py` & `conan-2.0.4/conan/tools/apple/apple.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/apple/xcodebuild.py` & `conan-2.0.4/conan/tools/apple/xcodebuild.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/apple/xcodedeps.py` & `conan-2.0.4/conan/tools/apple/xcodedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/apple/xcodetoolchain.py` & `conan-2.0.4/conan/tools/apple/xcodetoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/build/__init__.py` & `conan-2.0.4/conan/tools/build/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/build/cppstd.py` & `conan-2.0.4/conan/tools/build/cppstd.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/build/cpu.py` & `conan-2.0.4/conan/tools/build/cpu.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/build/cross_building.py` & `conan-2.0.4/conan/tools/build/cross_building.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/build/flags.py` & `conan-2.0.4/conan/tools/build/flags.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/build/stdcpp_library.py` & `conan-2.0.4/conan/tools/build/stdcpp_library.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/cmake/cmake.py` & `conan-2.0.4/conan/tools/cmake/cmake.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/cmake/cmakedeps/cmakedeps.py` & `conan-2.0.4/conan/tools/cmake/cmakedeps/cmakedeps.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     FIND_MODE_MODULE
 from conan.tools.cmake.cmakedeps.templates.config import ConfigTemplate
 from conan.tools.cmake.cmakedeps.templates.config_version import ConfigVersionTemplate
 from conan.tools.cmake.cmakedeps.templates.macros import MacrosTemplate
 from conan.tools.cmake.cmakedeps.templates.target_configuration import TargetConfigurationTemplate
 from conan.tools.cmake.cmakedeps.templates.target_data import ConfigDataTemplate
 from conan.tools.cmake.cmakedeps.templates.targets import TargetsTemplate
+from conans.client.generators import relativize_generated_file
 from conans.errors import ConanException
 from conans.util.files import save
 
 
 class CMakeDeps(object):
 
     def __init__(self, conanfile):
@@ -90,15 +91,17 @@
 
     def _generate_files(self, require, dep, ret, find_module_mode):
         if not find_module_mode:
             config_version = ConfigVersionTemplate(self, require, dep)
             ret[config_version.filename] = config_version.render()
 
         data_target = ConfigDataTemplate(self, require, dep, find_module_mode)
-        ret[data_target.filename] = data_target.render()
+        data_content = relativize_generated_file(data_target.render(), self._conanfile,
+                                                 "${CMAKE_CURRENT_LIST_DIR}")
+        ret[data_target.filename] = data_content
 
         target_configuration = TargetConfigurationTemplate(self, require, dep, find_module_mode)
         ret[target_configuration.filename] = target_configuration.render()
 
         targets = TargetsTemplate(self, require, dep, find_module_mode)
         ret[targets.filename] = targets.render()
```

### Comparing `conan-2.0.3/conan/tools/cmake/cmakedeps/templates/__init__.py` & `conan-2.0.4/conan/tools/cmake/cmakedeps/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/cmake/cmakedeps/templates/config.py` & `conan-2.0.4/conan/tools/cmake/cmakedeps/templates/config.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/cmake/cmakedeps/templates/config_version.py` & `conan-2.0.4/conan/tools/cmake/cmakedeps/templates/config_version.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/cmake/cmakedeps/templates/macros.py` & `conan-2.0.4/conan/tools/cmake/cmakedeps/templates/macros.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/cmake/cmakedeps/templates/target_configuration.py` & `conan-2.0.4/conan/tools/cmake/cmakedeps/templates/target_configuration.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/cmake/cmakedeps/templates/target_data.py` & `conan-2.0.4/conan/tools/cmake/cmakedeps/templates/target_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,21 +46,15 @@
         # for example a framework test won't be a build require but a "test/not public" require.
         dependency_filenames = self._get_dependency_filenames()
         # Get the nodes that have the property cmake_find_mode=None (no files to generate)
         dependency_find_modes = self._get_dependencies_find_modes()
 
         # Make the root_folder relative to the generated xxx-data.cmake file
         root_folder = self._root_folder
-        generators_folder = self.cmakedeps._conanfile.generators_folder
-        if os.path.commonpath([root_folder, generators_folder]) == generators_folder:
-            rel_path = os.path.relpath(root_folder, generators_folder)
-            rel_path = rel_path.replace('\\', '/').replace('$', '\\$').replace('"', '\\"')
-            root_folder = f"${{CMAKE_CURRENT_LIST_DIR}}/{rel_path}"
-        else:
-            root_folder = root_folder.replace('\\', '/').replace('$', '\\$').replace('"', '\\"')
+        root_folder = root_folder.replace('\\', '/').replace('$', '\\$').replace('"', '\\"')
 
         return {"global_cpp": global_cpp,
                 "has_components": self.conanfile.cpp_info.has_components,
                 "pkg_name": self.pkg_name,
                 "file_name": self.file_name,
                 "package_folder": root_folder,
                 "config_suffix": self.config_suffix,
```

### Comparing `conan-2.0.3/conan/tools/cmake/cmakedeps/templates/targets.py` & `conan-2.0.4/conan/tools/cmake/cmakedeps/templates/targets.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/cmake/file_api.py` & `conan-2.0.4/conan/tools/cmake/file_api.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/cmake/layout.py` & `conan-2.0.4/conan/tools/cmake/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/cmake/presets.py` & `conan-2.0.4/conan/tools/cmake/presets.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/cmake/toolchain/blocks.py` & `conan-2.0.4/conan/tools/cmake/toolchain/blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -516,20 +516,17 @@
         {% endif %}
         """)
 
     def context(self):
         pkg_config = self._conanfile.conf.get("tools.gnu:pkg_config", check_type=str)
         if pkg_config:
             pkg_config = pkg_config.replace("\\", "/")
-        pkg_config_path = self._conanfile.generators_folder
-        if pkg_config_path:
-            # hardcoding scope as "build"
-            subsystem = deduce_subsystem(self._conanfile, "build")
-            pathsep = ":" if subsystem != WINDOWS else ";"
-            pkg_config_path = pkg_config_path.replace("\\", "/") + pathsep
+        subsystem = deduce_subsystem(self._conanfile, "build")
+        pathsep = ":" if subsystem != WINDOWS else ";"
+        pkg_config_path = "${CMAKE_CURRENT_LIST_DIR}" + pathsep
         return {"pkg_config": pkg_config,
                 "pkg_config_path": pkg_config_path}
 
 
 class UserToolchain(Block):
     template = textwrap.dedent("""
         {% for user_toolchain in paths %}
```

### Comparing `conan-2.0.3/conan/tools/cmake/toolchain/toolchain.py` & `conan-2.0.4/conan/tools/cmake/toolchain/toolchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from conan.tools.cmake.toolchain.blocks import ToolchainBlocks, UserToolchain, GenericSystemBlock, \
     AndroidSystemBlock, AppleSystemBlock, FPicBlock, ArchitectureBlock, GLibCXXBlock, VSRuntimeBlock, \
     CppStdBlock, ParallelBlock, CMakeFlagsInitBlock, TryCompileBlock, FindFiles, PkgConfigBlock, \
     SkipRPath, SharedLibBock, OutputDirsBlock, ExtraFlagsBlock, CompilersBlock, LinkerScriptsBlock
 from conan.tools.intel import IntelCC
 from conan.tools.microsoft import VCVars
 from conan.tools.microsoft.visual import vs_ide_version
+from conans.client.generators import relativize_generated_file
 from conans.errors import ConanException
 from conans.model.options import _PackageOption
 from conans.util.files import save
 
 
 class Variables(OrderedDict):
     _configuration_types = None  # Needed for py27 to avoid infinite recursion
@@ -167,14 +168,15 @@
 
         return ctxt_toolchain
 
     @property
     def content(self):
         context = self._context()
         content = Template(self._template, trim_blocks=True, lstrip_blocks=True).render(**context)
+        content = relativize_generated_file(content, self._conanfile, "${CMAKE_CURRENT_LIST_DIR}")
         return content
 
     def generate(self):
         """
           This method will save the generated files to the conanfile.generators_folder
         """
         check_duplicated_generator(self, self._conanfile)
```

### Comparing `conan-2.0.3/conan/tools/env/environment.py` & `conan-2.0.4/conan/tools/env/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import textwrap
 from collections import OrderedDict
 from contextlib import contextmanager
 
+from conans.client.generators import relativize_generated_file
 from conans.client.subsystems import deduce_subsystem, WINDOWS, subsystem_path
 from conans.errors import ConanException
 from conans.model.recipe_ref import ref_matches
 from conans.util.files import save
 
 
 class _EnvVarPlaceHolder:
@@ -410,22 +411,21 @@
             """).format(deactivate_file=deactivate_file, vars=" ".join(self._values.keys()))
         capture = textwrap.dedent("""\
             @echo off
             chcp 65001 > nul
             {deactivate}
             """).format(deactivate=deactivate if generate_deactivate else "")
         result = [capture]
-        location = os.path.abspath(os.path.dirname(file_location))
         for varname, varvalues in self._values.items():
             value = varvalues.get_str("%{name}%", subsystem=self._subsystem, pathsep=self._pathsep)
             # To make the script relocatable
-            value = value.replace(location, "%~dp0")
             result.append('set "{}={}"'.format(varname, value))
 
         content = "\n".join(result)
+        content = relativize_generated_file(content, self._conanfile, "%~dp0")
         # It is very important to save it correctly with utf-8, the Conan util save() is broken
         os.makedirs(os.path.dirname(os.path.abspath(file_location)), exist_ok=True)
         open(file_location, "w", encoding="utf-8").write(content)
 
     def save_ps1(self, file_location, generate_deactivate=True,):
         _, filename = os.path.split(file_location)
         deactivate_file = "deactivate_{}".format(filename)
```

### Comparing `conan-2.0.3/conan/tools/env/virtualbuildenv.py` & `conan-2.0.4/conan/tools/env/virtualbuildenv.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/env/virtualrunenv.py` & `conan-2.0.4/conan/tools/env/virtualrunenv.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/files/__init__.py` & `conan-2.0.4/conan/tools/files/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from conan.tools.files.files import load, save, mkdir, rmdir, rm, ftp_download, download, get, \
-    rename, chdir, unzip, replace_in_file, collect_libs, check_md5, check_sha1, check_sha256
+    rename, chdir, unzip, replace_in_file, collect_libs, check_md5, check_sha1, check_sha256, \
+    move_folder_contents
 
 from conan.tools.files.patches import patch, apply_conandata_patches, export_conandata_patches
 from conan.tools.files.cpp_package import CppPackage
 from conan.tools.files.packager import AutoPackager
 from conan.tools.files.symlinks import symlinks
 from conan.tools.files.copy_pattern import copy
 from conan.tools.files.conandata import update_conandata
```

### Comparing `conan-2.0.3/conan/tools/files/conandata.py` & `conan-2.0.4/conan/tools/files/conandata.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/files/copy_pattern.py` & `conan-2.0.4/conan/tools/files/copy_pattern.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/files/cpp_package.py` & `conan-2.0.4/conan/tools/files/cpp_package.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/files/files.py` & `conan-2.0.4/conan/tools/files/files.py`

 * *Files 5% similar despite different names*

```diff
@@ -519,22 +519,43 @@
             name = name[3:]
         result.append(name)
     result.sort()
     return result
 
 
 # TODO: Do NOT document this yet. It is unclear the interface, maybe should be split
-def swap_child_folder(parent_folder, child_folder):
+def move_folder_contents(src_folder, dst_folder):
     """ replaces the current folder contents with the contents of one child folder. This
     is used in the SCM monorepo flow, when it is necessary to use one subproject subfolder
     to replace the whole cloned git repo
+    /base-folder                       /base-folder
+        /pkg  (src folder)                 /other/<otherfiles>
+          /other/<otherfiles>              /pkg/<pkgfiles>
+          /pkg/<pkgfiles>                  <files>
+          <files>
+        /siblings
+        <siblingsfiles>
     """
-    for f in os.listdir(parent_folder):
-        if f != child_folder:
-            path = os.path.join(parent_folder, f)
-            if os.path.isfile(path):
-                os.remove(path)
+    # Remove potential "siblings" folders not wanted
+    src_folder_name = os.path.basename(src_folder)
+    for f in os.listdir(dst_folder):
+        if f != src_folder_name:  # FIXME: Only works for 1st level subfolder
+            dst = os.path.join(dst_folder, f)
+            if os.path.isfile(dst):
+                os.remove(dst)
             else:
-                _internal_rmdir(path)
-    child = os.path.join(parent_folder, child_folder)
-    for f in os.listdir(child):
-        shutil.move(os.path.join(child, f), os.path.join(parent_folder, f))
+                _internal_rmdir(dst)
+
+    # Move all the contents
+    for f in os.listdir(src_folder):
+        src = os.path.join(src_folder, f)
+        dst = os.path.join(dst_folder, f)
+        if not os.path.exists(dst):
+            shutil.move(src, dst_folder)
+        else:
+            for sub_src in os.listdir(src):
+                shutil.move(os.path.join(src, sub_src), dst)
+            _internal_rmdir(src)
+    try:
+        os.rmdir(src_folder)
+    except OSError:
+        pass
```

### Comparing `conan-2.0.3/conan/tools/files/packager.py` & `conan-2.0.4/conan/tools/files/packager.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/files/patches.py` & `conan-2.0.4/conan/tools/files/patches.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/files/symlinks/symlinks.py` & `conan-2.0.4/conan/tools/files/symlinks/symlinks.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/gnu/autotools.py` & `conan-2.0.4/conan/tools/gnu/autotools.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/gnu/autotoolsdeps.py` & `conan-2.0.4/conan/tools/gnu/autotoolsdeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/gnu/autotoolstoolchain.py` & `conan-2.0.4/conan/tools/gnu/autotoolstoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/gnu/get_gnu_triplet.py` & `conan-2.0.4/conan/tools/gnu/get_gnu_triplet.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/gnu/gnudeps_flags.py` & `conan-2.0.4/conan/tools/gnu/gnudeps_flags.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/gnu/pkgconfig.py` & `conan-2.0.4/conan/tools/gnu/pkgconfig.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/gnu/pkgconfigdeps.py` & `conan-2.0.4/conan/tools/gnu/pkgconfigdeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/google/bazel.py` & `conan-2.0.4/conan/tools/google/bazel.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/google/bazeldeps.py` & `conan-2.0.4/conan/tools/google/bazeldeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/google/layout.py` & `conan-2.0.4/conan/tools/google/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/google/toolchain.py` & `conan-2.0.4/conan/tools/google/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/intel/intel_cc.py` & `conan-2.0.4/conan/tools/intel/intel_cc.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/layout/__init__.py` & `conan-2.0.4/conan/tools/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/meson/helpers.py` & `conan-2.0.4/conan/tools/meson/helpers.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/meson/meson.py` & `conan-2.0.4/conan/tools/meson/meson.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/meson/toolchain.py` & `conan-2.0.4/conan/tools/meson/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/microsoft/__init__.py` & `conan-2.0.4/conan/tools/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/microsoft/layout.py` & `conan-2.0.4/conan/tools/microsoft/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/microsoft/msbuild.py` & `conan-2.0.4/conan/tools/microsoft/msbuild.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/microsoft/msbuilddeps.py` & `conan-2.0.4/conan/tools/microsoft/msbuilddeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/microsoft/nmakedeps.py` & `conan-2.0.4/conan/tools/microsoft/nmakedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/microsoft/nmaketoolchain.py` & `conan-2.0.4/conan/tools/microsoft/nmaketoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/microsoft/subsystems.py` & `conan-2.0.4/conan/tools/microsoft/subsystems.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/microsoft/toolchain.py` & `conan-2.0.4/conan/tools/microsoft/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/microsoft/visual.py` & `conan-2.0.4/conan/tools/microsoft/visual.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/premake/premake.py` & `conan-2.0.4/conan/tools/premake/premake.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/qbs/qbs.py` & `conan-2.0.4/conan/tools/qbs/qbs.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/qbs/qbsprofile.py` & `conan-2.0.4/conan/tools/qbs/qbsprofile.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/scm/git.py` & `conan-2.0.4/conan/tools/scm/git.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan/tools/system/package_manager.py` & `conan-2.0.4/conan/tools/system/package_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conan.egg-info/PKG-INFO` & `conan-2.0.4/conan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan
-Version: 2.0.3
+Version: 2.0.4
 Summary: Conan C/C++ package manager
 Home-page: https://conan.io
 Author: JFrog LTD
 Author-email: luism@jfrog.com
 License: MIT
 Project-URL: Documentation, https://docs.conan.io
 Project-URL: Source, https://github.com/conan-io/conan
```

### Comparing `conan-2.0.3/conan.egg-info/SOURCES.txt` & `conan-2.0.4/conan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/cache/cache.py` & `conan-2.0.4/conans/client/cache/cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/cache/editable.py` & `conan-2.0.4/conans/client/cache/editable.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/cache/remote_registry.py` & `conan-2.0.4/conans/client/cache/remote_registry.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/cmd/export.py` & `conan-2.0.4/conans/client/cmd/export.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/cmd/uploader.py` & `conan-2.0.4/conans/client/cmd/uploader.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/cmd/user.py` & `conan-2.0.4/conans/client/cmd/user.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/conanfile/build.py` & `conan-2.0.4/conans/client/conanfile/build.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/conanfile/configure.py` & `conan-2.0.4/conans/client/conanfile/configure.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/conanfile/package.py` & `conan-2.0.4/conans/client/conanfile/package.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/conf/__init__.py` & `conan-2.0.4/conans/client/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/conf/config_installer.py` & `conan-2.0.4/conans/client/conf/config_installer.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/conf/detect.py` & `conan-2.0.4/conans/client/conf/detect.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/conf/detect_vs.py` & `conan-2.0.4/conans/client/conf/detect_vs.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/conf/required_version.py` & `conan-2.0.4/conans/client/conf/required_version.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/downloaders/caching_file_downloader.py` & `conan-2.0.4/conans/client/downloaders/caching_file_downloader.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/downloaders/download_cache.py` & `conan-2.0.4/conans/client/downloaders/download_cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/downloaders/file_downloader.py` & `conan-2.0.4/conans/client/downloaders/file_downloader.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/generators/__init__.py` & `conan-2.0.4/conans/client/generators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,7 +167,19 @@
             generated.append(filename)
             save(os.path.join(conanfile.generators_folder, filename), ps1_content(ps1s))
             save(os.path.join(conanfile.generators_folder, "deactivate_{}".format(filename)),
                  ps1_content(deactivates(ps1s)))
     if generated:
         conanfile.output.highlight("Generating aggregated env files")
         conanfile.output.info(f"Generated aggregated env files: {generated}")
+
+
+def relativize_generated_file(content, conanfile, placeholder):
+    abs_base_path = conanfile.folders._base_generators
+    if not abs_base_path or not os.path.isabs(abs_base_path):
+        return content
+    generators_folder = conanfile.generators_folder
+    rel_path = os.path.relpath(abs_base_path, generators_folder)
+    new_path = placeholder if rel_path == "." else os.path.join(placeholder, rel_path)
+    content = content.replace(abs_base_path, new_path)
+    content = content.replace(abs_base_path.replace("\\", "/"), new_path.replace("\\", "/"))
+    return content
```

### Comparing `conan-2.0.3/conans/client/graph/build_mode.py` & `conan-2.0.4/conans/client/graph/build_mode.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/graph/compatibility.py` & `conan-2.0.4/conans/client/graph/compatibility.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/graph/compute_pid.py` & `conan-2.0.4/conans/client/graph/compute_pid.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections import OrderedDict
 
 from conans.errors import conanfile_exception_formatter, ConanInvalidConfiguration, \
-    conanfile_remove_attr
+    conanfile_remove_attr, ConanException
 from conans.model.info import ConanInfo, RequirementsInfo, RequirementInfo, PythonRequiresInfo
 
 
 def compute_package_id(node, new_config):
     """
     Compute the binary package ID of this node
     """
@@ -35,17 +35,21 @@
                 build_data[require] = req_info
             else:
                 data[require] = req_info
 
     reqs_info = RequirementsInfo(data)
     build_requires_info = RequirementsInfo(build_data)
     python_requires = PythonRequiresInfo(python_requires, python_mode)
+    try:
+        copied_options = conanfile.options.copy_conaninfo_options()
+    except ConanException as e:
+        raise ConanException(f"{conanfile}: {e}")
 
     conanfile.info = ConanInfo(settings=conanfile.settings.copy_conaninfo_settings(),
-                               options=conanfile.options.copy_conaninfo_options(),
+                               options=copied_options,
                                reqs_info=reqs_info,
                                build_requires_info=build_requires_info,
                                python_requires=python_requires,
                                conf=conanfile.conf.copy_conaninfo_conf())
     conanfile.original_info = conanfile.info.clone()
 
     if hasattr(conanfile, "validate_build"):
```

### Comparing `conan-2.0.3/conans/client/graph/graph.py` & `conan-2.0.4/conans/client/graph/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,16 @@
         return (str(self.ref), self._package_id) < (str(other.ref), other._package_id)
 
     def propagate_closing_loop(self, require, prev_node):
         self.propagate_downstream(require, prev_node)
         # List to avoid mutating the dict
         for transitive in list(prev_node.transitive_deps.values()):
             # TODO: possibly optimize in a bulk propagate
+            if transitive.require.override:
+                continue
             prev_node.propagate_downstream(transitive.require, transitive.node, self)
 
     def propagate_downstream(self, require, node, src_node=None):
         # print("  Propagating downstream ", self, "<-", require)
         assert node is not None
         # This sets the transitive_deps node if it was None (overrides)
         # Take into account that while propagating we can find RUNTIME shared conflicts we
@@ -90,14 +92,15 @@
         existing = self.transitive_deps.get(require)
         if existing is not None and existing.require is not require:
             if existing.node is not None and existing.node.ref != node.ref:
                 # print("  +++++Runtime conflict!", require, "with", node.ref)
                 return True
             require.aggregate(existing.require)
 
+        assert not require.version_range  # No ranges slip into transitive_deps definitions
         # TODO: Might need to move to an update() for performance
         self.transitive_deps.pop(require, None)
         self.transitive_deps[require] = TransitiveRequirement(require, node)
 
         # Check if need to propagate downstream
         if not self.dependants:
             return
```

### Comparing `conan-2.0.3/conans/client/graph/graph_binaries.py` & `conan-2.0.4/conans/client/graph/graph_binaries.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/graph/graph_builder.py` & `conan-2.0.4/conans/client/graph/graph_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import copy
 from collections import deque
 
 from conans.client.conanfile.configure import run_configure_method
 from conans.client.graph.graph import DepsGraph, Node, CONTEXT_HOST, \
     CONTEXT_BUILD, TransitiveRequirement, RECIPE_VIRTUAL
 from conans.client.graph.graph import RECIPE_SYSTEM_TOOL
-from conans.client.graph.graph_error import GraphError
+from conans.client.graph.graph_error import GraphLoopError, GraphConflictError, GraphMissingError, \
+    GraphRuntimeError, GraphError
 from conans.client.graph.profile_node_definer import initialize_conanfile_profile
 from conans.client.graph.provides import check_graph_provides
 from conans.errors import ConanException
 from conans.model.conan_file import ConanFile
 from conans.model.options import Options
 from conans.model.recipe_ref import RecipeReference, ref_matches
 from conans.model.requires import Requirement
@@ -31,18 +32,14 @@
         assert profile_host is not None
         assert profile_build is not None
         assert isinstance(profile_host.options, Options)
         assert isinstance(profile_build.options, Options)
         # print("Loading graph")
         dep_graph = DepsGraph()
 
-        # TODO: Why assign here the settings_build and settings_target?
-        root_node.conanfile.settings_build = profile_build.processed_settings.copy()
-        root_node.conanfile.settings_target = None
-
         self._prepare_node(root_node, profile_host, profile_build, Options())
         self._initialize_requires(root_node, dep_graph, graph_lock)
         dep_graph.add_node(root_node)
 
         open_requires = deque((r, root_node) for r in root_node.conanfile.requires.values())
         try:
             while open_requires:
@@ -73,15 +70,15 @@
         previous = node.check_downstream_exists(require)
         prev_node = None
         if previous is not None:
             prev_require, prev_node, base_previous = previous
             # print("  Existing previous requirements from ", base_previous, "=>", prev_require)
 
             if prev_require is None:
-                raise GraphError.loop(node, require, prev_node)
+                raise GraphLoopError(node, require, prev_node)
 
             prev_ref = prev_node.ref if prev_node else prev_require.ref
             if prev_require.force or prev_require.override:  # override
                 require.ref = prev_ref
             else:
                 self._conflicting_version(require, node, prev_require, prev_node,
                                           prev_ref, base_previous, self._resolve_prereleases)
@@ -108,20 +105,20 @@
             # TODO: Check user/channel conflicts first
             if prev_version_range is not None:
                 pass  # Do nothing, evaluate current as it were a fixed one
             else:
                 if version_range.contains(prev_ref.version, resolve_prereleases):
                     require.ref = prev_ref
                 else:
-                    raise GraphError.conflict(node, require, prev_node, prev_require, base_previous)
+                    raise GraphConflictError(node, require, prev_node, prev_require, base_previous)
 
         elif prev_version_range is not None:
             # TODO: Check user/channel conflicts first
             if not prev_version_range.contains(require.ref.version, resolve_prereleases):
-                raise GraphError.conflict(node, require, prev_node, prev_require, base_previous)
+                raise GraphConflictError(node, require, prev_node, prev_require, base_previous)
         else:
             def _conflicting_refs(ref1, ref2):
                 ref1_norev = copy.copy(ref1)
                 ref1_norev.revision = None
                 ref2_norev = copy.copy(ref2)
                 ref2_norev.revision = None
                 if ref2_norev != ref1_norev:
@@ -131,15 +128,15 @@
                 # a revision, so it's ok any previous_ref
                 if ref1.revision and ref2.revision and ref1.revision != ref2.revision:
                     return True
 
             # As we are closing a diamond, there can be conflicts. This will raise if so
             conflict = _conflicting_refs(prev_ref, require.ref)
             if conflict:  # It is possible to get conflict from alias, try to resolve it
-                raise GraphError.conflict(node, require, prev_node, prev_require, base_previous)
+                raise GraphConflictError(node, require, prev_node, prev_require, base_previous)
 
     @staticmethod
     def _prepare_node(node, profile_host, profile_build, down_options):
 
         # basic node configuration: calling configure() and requirements()
         conanfile, ref = node.conanfile, node.ref
 
@@ -190,15 +187,15 @@
         while alias is not None:
             # if not cached, then resolve
             try:
                 result = self._proxy.get_recipe(alias, self._remotes, self._update,
                                                 self._check_update)
                 conanfile_path, recipe_status, remote, new_ref = result
             except ConanException as e:
-                raise GraphError.missing(node, require, str(e))
+                raise GraphMissingError(node, require, str(e))
 
             dep_conanfile = self._loader.load_basic(conanfile_path)
             try:
                 pointed_ref = RecipeReference.loads(dep_conanfile.alias)
             except Exception as e:
                 raise ConanException(f"Alias definition error in {alias}: {str(e)}")
 
@@ -214,41 +211,45 @@
         dep_conanfile = self._loader.load_conanfile(conanfile_path, ref=ref, graph_lock=graph_lock,
                                                     remotes=self._remotes, update=self._update,
                                                     check_update=self._check_update)
         return new_ref, dep_conanfile, recipe_status, remote
 
     @staticmethod
     def _resolved_system_tool(node, require, profile_build, profile_host, resolve_prereleases):
-        if node.context == CONTEXT_HOST and not require.build:  # Only for tool_requires
+        if node.context == CONTEXT_HOST and not require.build:  # Only for DIRECT tool_requires
             return
         system_tool = profile_build.system_tools if node.context == CONTEXT_BUILD \
             else profile_host.system_tools
         if system_tool:
             version_range = require.version_range
             for d in system_tool:
                 if require.ref.name == d.name:
                     if version_range:
                         if version_range.contains(d.version, resolve_prereleases):
+                            require.ref.version = d.version  # resolved range is replaced by exact
                             return d, ConanFile(str(d)), RECIPE_SYSTEM_TOOL, None
                     elif require.ref.version == d.version:
-                        return d, ConanFile(str(d)), RECIPE_SYSTEM_TOOL, None
+                        if d.revision is None or require.ref.revision is None or \
+                                d.revision == require.ref.revision:
+                            require.ref.revision = d.revision
+                            return d, ConanFile(str(d)), RECIPE_SYSTEM_TOOL, None
 
     def _create_new_node(self, node, require, graph, profile_host, profile_build, graph_lock):
         resolved = self._resolved_system_tool(node, require, profile_build, profile_host,
                                               self._resolve_prereleases)
 
         if resolved is None:
             try:
                 # TODO: If it is locked not resolve range
                 # TODO: This range-resolve might resolve in a given remote or cache
                 # Make sure next _resolve_recipe use it
                 self._resolver.resolve(require, str(node.ref), self._remotes, self._update)
                 resolved = self._resolve_recipe(require.ref, graph_lock)
             except ConanException as e:
-                raise GraphError.missing(node, require, str(e))
+                raise GraphMissingError(node, require, str(e))
 
         new_ref, dep_conanfile, recipe_status, remote = resolved
         # If the node is virtual or a test package, the require is also "root"
         is_test_package = getattr(node.conanfile, "tested_reference_str", False)
         if node.conanfile._conan_is_consumer and (node.recipe == RECIPE_VIRTUAL or is_test_package):
             dep_conanfile._conan_is_consumer = True
         initialize_conanfile_profile(dep_conanfile, profile_build, profile_host, node.context,
@@ -276,20 +277,20 @@
             down_options = node.conanfile.up_options if require.visible else Options()
 
         self._prepare_node(new_node, profile_host, profile_build, down_options)
         require.process_package_type(node, new_node)
         graph.add_node(new_node)
         graph.add_edge(node, new_node, require)
         if node.propagate_downstream(require, new_node):
-            raise GraphError.runtime(node, new_node)
+            raise GraphRuntimeError(node, new_node)
 
         # This is necessary to prevent infinite loops even when visibility is False
         ancestor = node.check_loops(new_node)
         if ancestor is not None:
-            raise GraphError.loop(new_node, require, ancestor)
+            raise GraphLoopError(new_node, require, ancestor)
 
         return new_node
 
     @staticmethod
     def _remove_overrides(dep_graph):
         for node in dep_graph.nodes:
             to_remove = [r for r in node.transitive_deps if r.override]
```

### Comparing `conan-2.0.3/conans/client/graph/install_graph.py` & `conan-2.0.4/conans/client/graph/install_graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/graph/profile_node_definer.py` & `conan-2.0.4/conans/client/graph/profile_node_definer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from conans.client.graph.graph import CONTEXT_HOST, CONTEXT_BUILD
+from conans.client.graph.graph import CONTEXT_BUILD
 from conans.errors import ConanException
 from conans.model.recipe_ref import ref_matches
 
 
 def initialize_conanfile_profile(conanfile, profile_build, profile_host, base_context,
                                  is_build_require, ref=None):
     """ this function fills conanfile information with the profile informaiton
@@ -24,20 +24,16 @@
     # profile host
     profile = profile_build if is_build_require or base_context == CONTEXT_BUILD else profile_host
     _initialize_conanfile(conanfile, profile, ref)
     # profile build
     conanfile.settings_build = profile_build.processed_settings.copy()
     # profile target
     conanfile.settings_target = None
-    if base_context == CONTEXT_HOST:
-        if is_build_require:
-            conanfile.settings_target = profile_host.processed_settings.copy()
-    else:
-        if not is_build_require:
-            conanfile.settings_target = profile_build.processed_settings.copy()
+    if is_build_require or base_context == CONTEXT_BUILD:
+        conanfile.settings_target = profile_host.processed_settings.copy()
 
 
 def _initialize_conanfile(conanfile, profile, ref):
     # Prepare the settings for the loaded conanfile
     # Mixing the global settings with the specified for that name if exist
     tmp_settings = profile.processed_settings.copy()
     package_settings_values = profile.package_settings_values
@@ -61,23 +57,32 @@
     conanfile.settings = tmp_settings
     conanfile.settings._frozen = True
     conanfile._conan_buildenv = profile.buildenv
     conanfile._conan_runenv = profile.runenv
     conanfile.conf = profile.conf.get_conanfile_conf(ref, conanfile._conan_is_consumer)  # Maybe this can be done lazy too
 
 
-def consumer_definer(conanfile, profile_host):
+def consumer_definer(conanfile, profile_host, profile_build):
     """ conanfile.txt does not declare settings, but it assumes it uses all the profile settings
     These settings are very necessary for helpers like generators to produce the right output
     """
     tmp_settings = profile_host.processed_settings.copy()
     package_settings_values = profile_host.package_settings_values
 
     for pattern, settings in package_settings_values.items():
         if ref_matches(ref=None, pattern=pattern, is_consumer=True):
             tmp_settings.update_values(settings)
 
+    tmp_settings_build = profile_build.processed_settings.copy()
+    package_settings_values_build = profile_build.package_settings_values
+
+    for pattern, settings in package_settings_values_build.items():
+        if ref_matches(ref=None, pattern=pattern, is_consumer=True):
+            tmp_settings_build.update_values(settings)
+
     conanfile.settings = tmp_settings
+    conanfile.settings_build = tmp_settings_build
+    conanfile.settings_target = None
     conanfile.settings._frozen = True
     conanfile._conan_buildenv = profile_host.buildenv
     conanfile._conan_runenv = profile_host.runenv
     conanfile.conf = profile_host.conf.get_conanfile_conf(None, is_consumer=True)
```

### Comparing `conan-2.0.3/conans/client/graph/provides.py` & `conan-2.0.4/conans/client/graph/provides.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from conans.client.graph.graph_error import GraphError
+from conans.client.graph.graph_error import GraphProvidesError
 from conans.model.recipe_ref import RecipeReference
 
 
 def check_graph_provides(dep_graph):
     if dep_graph.error:
         return
     for node in dep_graph.nodes:
@@ -14,22 +14,22 @@
 
             dep_provides = dep_node.conanfile.provides
             if dep_provides is None:
                 continue
             for provide in dep_provides:
                 # First check if collides with current node
                 if current_provides is not None and provide in current_provides:
-                    raise GraphError.provides(node, dep_node)
+                    raise GraphProvidesError(node, dep_node)
 
                 # Then, check if collides with other requirements
                 new_req = dep_require.copy_requirement()
                 new_req.ref = RecipeReference(provide, new_req.ref.version, new_req.ref.user,
                                               new_req.ref.channel)
                 existing = node.transitive_deps.get(new_req)
                 if existing is not None:
-                    raise GraphError.provides(existing.node, dep_node)
+                    raise GraphProvidesError(existing.node, dep_node)
                 else:
                     existing_provide = provides.get(new_req)
                     if existing_provide is not None:
-                        raise GraphError.provides(existing_provide, dep_node)
+                        raise GraphProvidesError(existing_provide, dep_node)
                     else:
                         provides[new_req] = dep_node
```

### Comparing `conan-2.0.3/conans/client/graph/proxy.py` & `conan-2.0.4/conans/client/graph/proxy.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/graph/python_requires.py` & `conan-2.0.4/conans/client/graph/python_requires.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,18 +108,19 @@
 
     def _load_pyreq_conanfile(self, loader, graph_lock, ref, remotes, update, check_update):
         try:
             recipe = self._proxy.get_recipe(ref, remotes, update, check_update)
         except ConanException as e:
             raise ConanException(f"Cannot resolve python_requires '{ref}': {str(e)}")
         path, recipe_status, remote, new_ref = recipe
-        conanfile, module = loader.load_basic_module(path, graph_lock, update, check_update)
+        conanfile, module = loader.load_basic_module(path, graph_lock, remotes=remotes,
+                                                     update=update, check_update=check_update)
         conanfile.name = new_ref.name
         conanfile.version = str(new_ref.version)
         conanfile.user = new_ref.user
-        # TODO: Is tihs really necessary?
+        # TODO: Is this really necessary?
         conanfile.channel = new_ref.channel
 
         if getattr(conanfile, "alias", None):
             raise ConanException("python-requires 'alias' are not supported in Conan 2.0. "
                                  "Please use version ranges instead")
         return conanfile, module, new_ref, os.path.dirname(path), recipe_status, remote
```

### Comparing `conan-2.0.3/conans/client/graph/range_resolver.py` & `conan-2.0.4/conans/client/graph/range_resolver.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/hook_manager.py` & `conan-2.0.4/conans/client/hook_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/installer.py` & `conan-2.0.4/conans/client/installer.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/loader.py` & `conan-2.0.4/conans/client/loader.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/loader_txt.py` & `conan-2.0.4/conans/client/loader_txt.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/migrations.py` & `conan-2.0.4/conans/client/migrations.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/pkg_sign.py` & `conan-2.0.4/conans/client/pkg_sign.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/profile_loader.py` & `conan-2.0.4/conans/client/profile_loader.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/remote_manager.py` & `conan-2.0.4/conans/client/remote_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,27 +48,33 @@
 
         assert ref.revision, "get_recipe without revision specified"
 
         layout = self._cache.get_or_create_ref_layout(ref)
         layout.export_remove()
 
         download_export = layout.download_export()
-        zipped_files = self._call_remote(remote, "get_recipe", ref, download_export)
-        remote_refs = self._call_remote(remote, "get_recipe_revisions_references", ref)
-        ref_time = remote_refs[0].timestamp
-        ref.timestamp = ref_time
-        # filter metadata files
-        # This could be also optimized in the download, avoiding downloading them, for performance
-        zipped_files = {k: v for k, v in zipped_files.items() if not k.startswith(METADATA)}
-        # quick server package integrity check:
-        if "conanfile.py" not in zipped_files:
-            raise ConanException(f"Corrupted {ref} in '{remote.name}' remote: no conanfile.py")
-        if "conanmanifest.txt" not in zipped_files:
-            raise ConanException(f"Corrupted {ref} in '{remote.name}' remote: no conanmanifest.txt")
-        self._signer.verify(ref, download_export)
+        try:
+            zipped_files = self._call_remote(remote, "get_recipe", ref, download_export)
+            remote_refs = self._call_remote(remote, "get_recipe_revisions_references", ref)
+            ref_time = remote_refs[0].timestamp
+            ref.timestamp = ref_time
+            # filter metadata files
+            # This could be also optimized in download, avoiding downloading them, for performance
+            zipped_files = {k: v for k, v in zipped_files.items() if not k.startswith(METADATA)}
+            # quick server package integrity check:
+            if "conanfile.py" not in zipped_files:
+                raise ConanException(f"Corrupted {ref} in '{remote.name}' remote: no conanfile.py")
+            if "conanmanifest.txt" not in zipped_files:
+                raise ConanException(f"Corrupted {ref} in '{remote.name}' remote: "
+                                     f"no conanmanifest.txt")
+            self._signer.verify(ref, download_export)
+        except BaseException:  # So KeyboardInterrupt also cleans things
+            ConanOutput(scope=str(ref)).error(f"Error downloading from remote '{remote.name}'")
+            self._cache.remove_recipe_layout(layout)
+            raise
         export_folder = layout.export()
         tgz_file = zipped_files.pop(EXPORT_TGZ_NAME, None)
 
         if tgz_file:
             uncompress_file(tgz_file, export_folder)
         mkdir(export_folder)
         for file_name, file_path in zipped_files.items():  # copy CONANFILE
@@ -122,15 +128,16 @@
             for file_name, file_path in zipped_files.items():  # copy CONANINFO and CONANMANIFEST
                 shutil.move(file_path, os.path.join(package_folder, file_name))
 
             scoped_output.success('Package installed %s' % pref.package_id)
             scoped_output.info("Downloaded package revision %s" % pref.revision)
         except NotFoundException:
             raise PackageNotFoundException(pref)
-        except BaseException as e:
+        except BaseException as e:  # So KeyboardInterrupt also cleans things
+            self._cache.remove_package_layout(layout)
             scoped_output.error("Exception while getting package: %s" % str(pref.package_id))
             scoped_output.error("Exception: %s %s" % (type(e), str(e)))
             raise
 
     def search_recipes(self, remote, pattern):
         return self._call_remote(remote, "search", pattern)
```

### Comparing `conan-2.0.3/conans/client/rest/__init__.py` & `conan-2.0.4/conans/client/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/rest/auth_manager.py` & `conan-2.0.4/conans/client/rest/auth_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,23 +36,23 @@
 
         if method_name == "authenticate":
             return self._authenticate(remote, *args, **kwargs)
 
         try:
             ret = getattr(rest_client, method_name)(*args, **kwargs)
             return ret
-        except ForbiddenException:
-            raise ForbiddenException("Permission denied for user: '%s'" % user)
+        except ForbiddenException as e:
+            raise ForbiddenException(f"Permission denied for user: '{user}': {e}")
         except AuthenticationException:
             # User valid but not enough permissions
             if user is None or token is None:
                 # token is None when you change user with user command
                 # Anonymous is not enough, ask for a user
                 ConanOutput().info('Please log in to "%s" to perform this action. '
-                                   'Execute "conan user" command.' % remote.name)
+                                   'Execute "conan remote login" command.' % remote.name)
                 return self._retry_with_new_token(user, remote, method_name, *args, **kwargs)
             elif token and refresh_token:
                 # If we have a refresh token try to refresh the access token
                 try:
                     self._authenticate(remote, user, None)
                 except AuthenticationException:
                     # logger.info("Cannot refresh the token, cleaning and retrying: {}".format(exc))
@@ -76,15 +76,15 @@
                 self._authenticate(remote, input_user, input_password)
             except AuthenticationException:
                 out = ConanOutput()
                 if user is None:
                     out.error('Wrong user or password')
                 else:
                     out.error('Wrong password for user "%s"' % user)
-                    out.info('You can change username with "conan user <username>"')
+                    out.info('You can change username with "conan remote login <remote> <username>"')
             else:
                 return self.call_rest_api_method(remote, method_name, *args, **kwargs)
 
         raise AuthenticationException("Too many failed login attempts, bye!")
 
     def _get_rest_client(self, remote):
         username, token, refresh_token = self._localdb.get_login(remote.url)
```

### Comparing `conan-2.0.3/conans/client/rest/client_routes.py` & `conan-2.0.4/conans/client/rest/client_routes.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/rest/conan_requester.py` & `conan-2.0.4/conans/client/rest/conan_requester.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/rest/file_uploader.py` & `conan-2.0.4/conans/client/rest/file_uploader.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/rest/rest_client.py` & `conan-2.0.4/conans/client/rest/rest_client.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/rest/rest_client_common.py` & `conan-2.0.4/conans/client/rest/rest_client_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         return ret
 
     def server_capabilities(self, user=None, password=None):
         """Get information about the server: status, version, type and capabilities"""
         url = self.router.ping()
         # logger.debug("REST: ping: %s" % url)
         if user and password:
-            # This can happen in "conan user" cmd. Instead of empty token, use HttpBasic
+            # This can happen in "conan remote login" cmd. Instead of empty token, use HttpBasic
             auth = HTTPBasicAuth(user, password)
         else:
             auth = self.auth
         ret = self.requester.get(url, auth=auth, headers=self.custom_headers, verify=self.verify_ssl)
 
         server_capabilities = ret.headers.get('X-Conan-Server-Capabilities', "")
         if not server_capabilities and not ret.ok:
```

### Comparing `conan-2.0.3/conans/client/rest/rest_client_v2.py` & `conan-2.0.4/conans/client/rest/rest_client_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,14 +157,16 @@
                 threads.append(thread)
                 thread.start()
             else:
                 downloader.download(url=resource_url, file_path=abs_path, auth=self.auth,
                                     verify_ssl=self.verify_ssl, retry=retry, retry_wait=retry_wait)
         for t in threads:
             t.join()
+        for t in threads:  # Need to join all before raising errors
+            t.raise_errors()
 
     def remove_all_packages(self, ref):
         """ Remove all packages from the specified reference"""
         self.check_credentials()
         assert ref.revision is not None, "remove_packages needs RREV"
 
         url = self.router.remove_all_packages(ref)
```

### Comparing `conan-2.0.3/conans/client/source.py` & `conan-2.0.4/conans/client/source.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/store/localdb.py` & `conan-2.0.4/conans/client/store/localdb.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/subsystems.py` & `conan-2.0.4/conans/client/subsystems.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/client/userio.py` & `conan-2.0.4/conans/client/userio.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/conan_server.py` & `conan-2.0.4/conans/conan_server.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/errors.py` & `conan-2.0.4/conans/errors.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/migrations.py` & `conan-2.0.4/conans/migrations.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/model/build_info.py` & `conan-2.0.4/conans/model/build_info.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/model/conan_file.py` & `conan-2.0.4/conans/model/conan_file.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/model/conanfile_interface.py` & `conan-2.0.4/conans/model/conanfile_interface.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/model/conf.py` & `conan-2.0.4/conans/model/conf.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/model/dependencies.py` & `conan-2.0.4/conans/model/dependencies.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/model/graph_lock.py` & `conan-2.0.4/conans/model/graph_lock.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/model/info.py` & `conan-2.0.4/conans/model/info.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/model/layout.py` & `conan-2.0.4/conans/model/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/model/manifest.py` & `conan-2.0.4/conans/model/manifest.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/model/options.py` & `conan-2.0.4/conans/model/options.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/model/package_ref.py` & `conan-2.0.4/conans/model/package_ref.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/model/pkg_type.py` & `conan-2.0.4/conans/model/pkg_type.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/model/profile.py` & `conan-2.0.4/conans/model/profile.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/model/recipe_ref.py` & `conan-2.0.4/conans/model/recipe_ref.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/model/requires.py` & `conan-2.0.4/conans/model/requires.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/model/rest_routes.py` & `conan-2.0.4/conans/model/rest_routes.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/model/settings.py` & `conan-2.0.4/conans/model/settings.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/model/version.py` & `conan-2.0.4/conans/model/version.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/model/version_range.py` & `conan-2.0.4/conans/model/version_range.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/paths/__init__.py` & `conan-2.0.4/conans/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/pylint_plugin.py` & `conan-2.0.4/conans/pylint_plugin.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/search/query_parse.py` & `conan-2.0.4/conans/search/query_parse.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/search/search.py` & `conan-2.0.4/conans/search/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,21 +51,22 @@
     conan_vars_info.serialize_min()
     """
 
     def compatible_prop(setting_value, _prop_value):
         return (_prop_value == setting_value) or (_prop_value == "None" and setting_value is None)
 
     # TODO: Necessary to generalize this query evaluation to include all possible fields
-    info_settings = binary_info.get("settings")
-    info_options = binary_info.get("options")
+    info_settings = binary_info.get("settings", {})
+    info_options = binary_info.get("options", {})
 
     if not prop_name.startswith("options."):
-        return compatible_prop(info_settings.get(prop_name, None), prop_value)
+        return compatible_prop(info_settings.get(prop_name), prop_value)
     else:
-        return compatible_prop(info_options.get(prop_name, None), prop_value)
+        prop_name = prop_name[len("options."):]
+        return compatible_prop(info_options.get(prop_name), prop_value)
 
 
 def search_recipes(cache, pattern=None, ignorecase=True):
     # Conan references in main storage
     if pattern:
         if isinstance(pattern, RecipeReference):
             pattern = repr(pattern)
```

### Comparing `conan-2.0.3/conans/test/conftest.py` & `conan-2.0.4/conans/test/conftest.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/test/utils/artifactory.py` & `conan-2.0.4/conans/test/utils/artifactory.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/test/utils/mocks.py` & `conan-2.0.4/conans/test/utils/mocks.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/test/utils/profiles.py` & `conan-2.0.4/conans/test/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/test/utils/scm.py` & `conan-2.0.4/conans/test/utils/scm.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/test/utils/server_launcher.py` & `conan-2.0.4/conans/test/utils/server_launcher.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/test/utils/test_files.py` & `conan-2.0.4/conans/test/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/test/utils/tools.py` & `conan-2.0.4/conans/test/utils/tools.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/util/config_parser.py` & `conan-2.0.4/conans/util/config_parser.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/util/dates.py` & `conan-2.0.4/conans/util/dates.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/util/encrypt.py` & `conan-2.0.4/conans/util/encrypt.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/util/env.py` & `conan-2.0.4/conans/util/env.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/util/files.py` & `conan-2.0.4/conans/util/files.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/util/locks.py` & `conan-2.0.4/conans/util/locks.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/util/runners.py` & `conan-2.0.4/conans/util/runners.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/util/sha.py` & `conan-2.0.4/conans/util/sha.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/conans/util/windows.py` & `conan-2.0.4/conans/util/windows.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.3/setup.py` & `conan-2.0.4/setup.py`

 * *Files identical despite different names*

