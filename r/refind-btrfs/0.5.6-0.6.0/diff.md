# Comparing `tmp/refind-btrfs-0.5.6.tar.gz` & `tmp/refind-btrfs-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refind-btrfs-0.5.6.tar", last modified: Sat Nov  5 09:52:26 2022, max compression
+gzip compressed data, was "refind-btrfs-0.6.0.tar", last modified: Thu May 11 09:58:28 2023, max compression
```

## Comparing `refind-btrfs-0.5.6.tar` & `refind-btrfs-0.6.0.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.600179 refind-btrfs-0.5.6/
--rw-rw-rw-   0        0        0    35823 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/LICENSE.txt
--rw-rw-rw-   0        0        0      266 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/MANIFEST.in
--rw-rw-rw-   0        0        0    28634 2022-11-05 09:52:26.601169 refind-btrfs-0.5.6/PKG-INFO
--rw-rw-rw-   0        0        0    27743 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/README.md
--rw-rw-rw-   0        0        0       93 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/pyproject.toml
--rw-rw-rw-   0        0        0     1294 2022-11-05 09:52:26.609167 refind-btrfs-0.5.6/setup.cfg
--rw-rw-rw-   0        0        0     2387 2022-11-05 09:27:13.000000 refind-btrfs-0.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.372170 refind-btrfs-0.5.6/src/
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.403169 refind-btrfs-0.5.6/src/refind_btrfs/
--rw-rw-rw-   0        0        0     3011 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/__init__.py
--rw-rw-rw-   0        0        0      992 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/__main__.py
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.451167 refind-btrfs-0.5.6/src/refind_btrfs/boot/
--rw-rw-rw-   0        0        0     1054 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/boot/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.460175 refind-btrfs-0.5.6/src/refind_btrfs/boot/antlr4/
--rw-rw-rw-   0        0        0    28269 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/boot/antlr4/RefindConfigLexer.py
--rw-rw-rw-   0        0        0    42214 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/boot/antlr4/RefindConfigParser.py
--rw-rw-rw-   0        0        0     4234 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/boot/antlr4/RefindConfigParserVisitor.py
--rw-rw-rw-   0        0        0     1074 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/boot/antlr4/__init__.py
--rw-rw-rw-   0        0        0     8852 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/boot/boot_options.py
--rw-rw-rw-   0        0        0    14136 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/boot/boot_stanza.py
--rw-rw-rw-   0        0        0    14292 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/boot/file_refind_config_provider.py
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.469169 refind-btrfs-0.5.6/src/refind_btrfs/boot/migrations/
--rw-rw-rw-   0        0        0      940 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/boot/migrations/__init__.py
--rw-rw-rw-   0        0        0     4335 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/boot/migrations/icon_migration_strategies.py
--rw-rw-rw-   0        0        0    12664 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/boot/migrations/main_migration_strategies.py
--rw-rw-rw-   0        0        0     6741 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/boot/migrations/migration.py
--rw-rw-rw-   0        0        0     1214 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/boot/migrations/state.py
--rw-rw-rw-   0        0        0     7325 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/boot/refind_config.py
--rw-rw-rw-   0        0        0     1241 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/boot/refind_listeners.py
--rw-rw-rw-   0        0        0    12436 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/boot/refind_visitors.py
--rw-rw-rw-   0        0        0     6309 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/boot/sub_menu.py
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.484170 refind-btrfs-0.5.6/src/refind_btrfs/common/
--rw-rw-rw-   0        0        0     1223 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.490169 refind-btrfs-0.5.6/src/refind_btrfs/common/abc/
--rw-rw-rw-   0        0        0      980 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/abc/__init__.py
--rw-rw-rw-   0        0        0     3604 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/abc/base_config.py
--rw-rw-rw-   0        0        0     1033 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/abc/base_runner.py
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.498168 refind-btrfs-0.5.6/src/refind_btrfs/common/abc/commands/
--rw-rw-rw-   0        0        0     1037 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/abc/commands/__init__.py
--rw-rw-rw-   0        0        0     2236 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/abc/commands/device_command.py
--rw-rw-rw-   0        0        0     1397 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/abc/commands/icon_command.py
--rw-rw-rw-   0        0        0     1548 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/abc/commands/subvolume_command.py
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.508187 refind-btrfs-0.5.6/src/refind_btrfs/common/abc/factories/
--rw-rw-rw-   0        0        0     1161 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/abc/factories/__init__.py
--rw-rw-rw-   0        0        0     1394 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/abc/factories/base_device_command_factory.py
--rw-rw-rw-   0        0        0     1195 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/abc/factories/base_icon_command_factory.py
--rw-rw-rw-   0        0        0     1647 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/abc/factories/base_logger_factory.py
--rw-rw-rw-   0        0        0     1215 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/abc/factories/base_subvolume_command_factory.py
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.516167 refind-btrfs-0.5.6/src/refind_btrfs/common/abc/providers/
--rw-rw-rw-   0        0        0     1106 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/abc/providers/__init__.py
--rw-rw-rw-   0        0        0     1209 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/abc/providers/base_package_config_provider.py
--rw-rw-rw-   0        0        0     1904 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/abc/providers/base_persistence_provider.py
--rw-rw-rw-   0        0        0     1468 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/abc/providers/base_refind_config_provider.py
--rw-rw-rw-   0        0        0     1285 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/boot_files_check_result.py
--rw-rw-rw-   0        0        0     1394 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/checkable_observer.py
--rw-rw-rw-   0        0        0     1490 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/configurable_mixin.py
--rw-rw-rw-   0        0        0     3280 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/constants.py
--rw-rw-rw-   0        0        0     5474 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/enums.py
--rw-rw-rw-   0        0        0     2626 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/exceptions.py
--rw-rw-rw-   0        0        0     5101 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/common/package_config.py
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.519168 refind-btrfs-0.5.6/src/refind_btrfs/console/
--rw-rw-rw-   0        0        0      941 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/console/__init__.py
--rw-rw-rw-   0        0        0     1991 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/console/cli_runner.py
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.524169 refind-btrfs-0.5.6/src/refind_btrfs/data/
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.383178 refind-btrfs-0.5.6/src/refind_btrfs/data/icons/
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.536184 refind-btrfs-0.5.6/src/refind_btrfs/data/icons/btrfs_logo/
--rw-rw-rw-   0        0        0     1112 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/data/icons/btrfs_logo/inverted_large.png
--rw-rw-rw-   0        0        0      903 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/data/icons/btrfs_logo/inverted_medium.png
--rw-rw-rw-   0        0        0      613 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/data/icons/btrfs_logo/inverted_small.png
--rw-rw-rw-   0        0        0     1048 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/data/icons/btrfs_logo/original_large.png
--rw-rw-rw-   0        0        0      835 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/data/icons/btrfs_logo/original_medium.png
--rw-rw-rw-   0        0        0      562 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/data/icons/btrfs_logo/original_small.png
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.539170 refind-btrfs-0.5.6/src/refind_btrfs/data/images/
--rw-rw-rw-   0        0        0    81467 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/data/images/refind_screenshot_default.png
--rw-rw-rw-   0        0        0    31538 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/data/images/refind_screenshot_nord.png
--rw-rw-rw-   0        0        0       57 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/data/refind-btrfs
--rw-rw-rw-   0        0        0     9555 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/data/refind-btrfs.conf-sample
--rw-rw-rw-   0        0        0      346 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/data/refind-btrfs.service
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.553168 refind-btrfs-0.5.6/src/refind_btrfs/device/
--rw-rw-rw-   0        0        0     1164 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/device/__init__.py
--rw-rw-rw-   0        0        0     5051 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/device/block_device.py
--rw-rw-rw-   0        0        0     3725 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/device/filesystem.py
--rw-rw-rw-   0        0        0     6391 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/device/mount_options.py
--rw-rw-rw-   0        0        0     4432 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/device/partition.py
--rw-rw-rw-   0        0        0     6375 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/device/partition_table.py
--rw-rw-rw-   0        0        0    13682 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/device/subvolume.py
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.567167 refind-btrfs-0.5.6/src/refind_btrfs/service/
--rw-rw-rw-   0        0        0     1058 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/service/__init__.py
--rw-rw-rw-   0        0        0     7054 2022-11-04 21:02:00.000000 refind-btrfs-0.5.6/src/refind_btrfs/service/snapshot_event_handler.py
--rw-rw-rw-   0        0        0     2312 2022-11-05 09:49:03.000000 refind-btrfs-0.5.6/src/refind_btrfs/service/snapshot_observer.py
--rw-rw-rw-   0        0        0     5096 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/service/watchdog_runner.py
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.574169 refind-btrfs-0.5.6/src/refind_btrfs/state_management/
--rw-rw-rw-   0        0        0      994 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/state_management/__init__.py
--rw-rw-rw-   0        0        0    10283 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/state_management/conditions.py
--rw-rw-rw-   0        0        0    18402 2022-11-04 21:07:46.000000 refind-btrfs-0.5.6/src/refind_btrfs/state_management/model.py
--rw-rw-rw-   0        0        0     3570 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/state_management/refind_btrfs_machine.py
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.586167 refind-btrfs-0.5.6/src/refind_btrfs/system/
--rw-rw-rw-   0        0        0     1046 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/system/__init__.py
--rw-rw-rw-   0        0        0    12526 2022-11-04 21:08:02.000000 refind-btrfs-0.5.6/src/refind_btrfs/system/btrfsutil_command.py
--rw-rw-rw-   0        0        0     2998 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/system/command_factories.py
--rw-rw-rw-   0        0        0     6401 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/system/findmnt_command.py
--rw-rw-rw-   0        0        0     5577 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/system/fstab_command.py
--rw-rw-rw-   0        0        0     9147 2022-11-04 21:08:14.000000 refind-btrfs-0.5.6/src/refind_btrfs/system/lsblk_command.py
--rw-rw-rw-   0        0        0    12415 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/system/pillow_command.py
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.598168 refind-btrfs-0.5.6/src/refind_btrfs/utility/
--rw-rw-rw-   0        0        0      962 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/utility/__init__.py
--rw-rw-rw-   0        0        0    22433 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/utility/file_package_config_provider.py
--rw-rw-rw-   0        0        0     8128 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/utility/helpers.py
--rw-rw-rw-   0        0        0     4022 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/utility/injector_modules.py
--rw-rw-rw-   0        0        0     1513 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/utility/level_aware_formatter.py
--rw-rw-rw-   0        0        0     1462 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/utility/logger_factories.py
--rw-rw-rw-   0        0        0     5513 2022-10-30 13:59:50.000000 refind-btrfs-0.5.6/src/refind_btrfs/utility/shelve_persistence_provider.py
-drwxrwxrwx   0        0        0        0 2022-11-05 09:52:26.438182 refind-btrfs-0.5.6/src/refind_btrfs.egg-info/
--rw-rw-rw-   0        0        0    28634 2022-11-05 09:52:26.000000 refind-btrfs-0.5.6/src/refind_btrfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4317 2022-11-05 09:52:26.000000 refind-btrfs-0.5.6/src/refind_btrfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-05 09:52:26.000000 refind-btrfs-0.5.6/src/refind_btrfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2022-11-05 09:52:26.000000 refind-btrfs-0.5.6/src/refind_btrfs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      144 2022-11-05 09:52:26.000000 refind-btrfs-0.5.6/src/refind_btrfs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-11-05 09:52:26.000000 refind-btrfs-0.5.6/src/refind_btrfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:28.570603 refind-btrfs-0.6.0/
+-rw-rw-rw-   0        0        0    35823 2022-10-30 13:59:50.000000 refind-btrfs-0.6.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      266 2022-10-30 13:59:50.000000 refind-btrfs-0.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    28636 2023-05-11 09:58:28.571600 refind-btrfs-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0    27743 2022-10-30 13:59:50.000000 refind-btrfs-0.6.0/README.md
+-rw-rw-rw-   0        0        0       93 2022-10-30 13:59:50.000000 refind-btrfs-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1296 2023-05-11 09:58:28.582604 refind-btrfs-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     2388 2023-03-28 10:52:10.000000 refind-btrfs-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:27.605022 refind-btrfs-0.6.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:27.664022 refind-btrfs-0.6.0/src/refind_btrfs/
+-rw-rw-rw-   0        0        0     3010 2023-03-27 23:04:48.000000 refind-btrfs-0.6.0/src/refind_btrfs/__init__.py
+-rw-rw-rw-   0        0        0      991 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:27.792028 refind-btrfs-0.6.0/src/refind_btrfs/boot/
+-rw-rw-rw-   0        0        0     1053 2023-03-11 14:33:58.000000 refind-btrfs-0.6.0/src/refind_btrfs/boot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:27.835544 refind-btrfs-0.6.0/src/refind_btrfs/boot/antlr4/
+-rw-rw-rw-   0        0        0    29295 2023-03-27 23:07:26.000000 refind-btrfs-0.6.0/src/refind_btrfs/boot/antlr4/RefindConfigLexer.py
+-rw-rw-rw-   0        0        0    42221 2023-03-27 23:06:00.000000 refind-btrfs-0.6.0/src/refind_btrfs/boot/antlr4/RefindConfigParser.py
+-rw-rw-rw-   0        0        0     4237 2023-03-27 23:06:00.000000 refind-btrfs-0.6.0/src/refind_btrfs/boot/antlr4/RefindConfigParserVisitor.py
+-rw-rw-rw-   0        0        0     1073 2023-03-27 23:05:17.000000 refind-btrfs-0.6.0/src/refind_btrfs/boot/antlr4/__init__.py
+-rw-rw-rw-   0        0        0     8850 2023-03-28 10:40:51.000000 refind-btrfs-0.6.0/src/refind_btrfs/boot/boot_options.py
+-rw-rw-rw-   0        0        0    14129 2023-03-28 10:41:38.000000 refind-btrfs-0.6.0/src/refind_btrfs/boot/boot_stanza.py
+-rw-rw-rw-   0        0        0    14215 2023-03-28 10:40:02.000000 refind-btrfs-0.6.0/src/refind_btrfs/boot/file_refind_config_provider.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:27.887548 refind-btrfs-0.6.0/src/refind_btrfs/boot/migrations/
+-rw-rw-rw-   0        0        0      939 2023-03-11 14:33:58.000000 refind-btrfs-0.6.0/src/refind_btrfs/boot/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4334 2023-03-28 10:35:35.000000 refind-btrfs-0.6.0/src/refind_btrfs/boot/migrations/icon_migration_strategies.py
+-rw-rw-rw-   0        0        0    12663 2023-03-28 10:35:37.000000 refind-btrfs-0.6.0/src/refind_btrfs/boot/migrations/main_migration_strategies.py
+-rw-rw-rw-   0        0        0     6740 2023-03-28 10:35:38.000000 refind-btrfs-0.6.0/src/refind_btrfs/boot/migrations/migration.py
+-rw-rw-rw-   0        0        0     1213 2023-03-28 10:35:40.000000 refind-btrfs-0.6.0/src/refind_btrfs/boot/migrations/state.py
+-rw-rw-rw-   0        0        0     7298 2023-03-28 10:41:44.000000 refind-btrfs-0.6.0/src/refind_btrfs/boot/refind_config.py
+-rw-rw-rw-   0        0        0     1240 2023-03-28 10:40:07.000000 refind-btrfs-0.6.0/src/refind_btrfs/boot/refind_listeners.py
+-rw-rw-rw-   0        0        0    12435 2023-03-28 10:40:06.000000 refind-btrfs-0.6.0/src/refind_btrfs/boot/refind_visitors.py
+-rw-rw-rw-   0        0        0     6308 2023-03-28 10:40:05.000000 refind-btrfs-0.6.0/src/refind_btrfs/boot/sub_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:27.968194 refind-btrfs-0.6.0/src/refind_btrfs/common/
+-rw-rw-rw-   0        0        0     1222 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:27.998196 refind-btrfs-0.6.0/src/refind_btrfs/common/abc/
+-rw-rw-rw-   0        0        0      979 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/abc/__init__.py
+-rw-rw-rw-   0        0        0     3479 2023-03-28 10:41:52.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/abc/base_config.py
+-rw-rw-rw-   0        0        0     1032 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/abc/base_runner.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:28.036194 refind-btrfs-0.6.0/src/refind_btrfs/common/abc/commands/
+-rw-rw-rw-   0        0        0     1036 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/abc/commands/__init__.py
+-rw-rw-rw-   0        0        0     2235 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/abc/commands/device_command.py
+-rw-rw-rw-   0        0        0     1396 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/abc/commands/icon_command.py
+-rw-rw-rw-   0        0        0     1642 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/abc/commands/subvolume_command.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:28.093198 refind-btrfs-0.6.0/src/refind_btrfs/common/abc/factories/
+-rw-rw-rw-   0        0        0     1160 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/abc/factories/__init__.py
+-rw-rw-rw-   0        0        0     1393 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/abc/factories/base_device_command_factory.py
+-rw-rw-rw-   0        0        0     1194 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/abc/factories/base_icon_command_factory.py
+-rw-rw-rw-   0        0        0     1646 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/abc/factories/base_logger_factory.py
+-rw-rw-rw-   0        0        0     1214 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/abc/factories/base_subvolume_command_factory.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:28.139145 refind-btrfs-0.6.0/src/refind_btrfs/common/abc/providers/
+-rw-rw-rw-   0        0        0     1105 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/abc/providers/__init__.py
+-rw-rw-rw-   0        0        0     1208 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/abc/providers/base_package_config_provider.py
+-rw-rw-rw-   0        0        0     1903 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/abc/providers/base_persistence_provider.py
+-rw-rw-rw-   0        0        0     1467 2023-03-27 23:04:48.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/abc/providers/base_refind_config_provider.py
+-rw-rw-rw-   0        0        0     1284 2023-03-28 10:40:19.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/boot_files_check_result.py
+-rw-rw-rw-   0        0        0     1393 2023-03-28 10:40:21.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/checkable_observer.py
+-rw-rw-rw-   0        0        0     1489 2023-03-28 10:40:23.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/configurable_mixin.py
+-rw-rw-rw-   0        0        0     3279 2023-03-28 10:40:24.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/constants.py
+-rw-rw-rw-   0        0        0     5473 2023-03-28 10:40:25.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/enums.py
+-rw-rw-rw-   0        0        0     2625 2023-03-28 10:40:26.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/exceptions.py
+-rw-rw-rw-   0        0        0     5074 2023-03-28 10:41:47.000000 refind-btrfs-0.6.0/src/refind_btrfs/common/package_config.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:28.164149 refind-btrfs-0.6.0/src/refind_btrfs/console/
+-rw-rw-rw-   0        0        0      940 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/console/__init__.py
+-rw-rw-rw-   0        0        0     1990 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/console/cli_runner.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:28.194146 refind-btrfs-0.6.0/src/refind_btrfs/data/
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:27.615024 refind-btrfs-0.6.0/src/refind_btrfs/data/icons/
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:28.212871 refind-btrfs-0.6.0/src/refind_btrfs/data/icons/btrfs_logo/
+-rw-rw-rw-   0        0        0     1112 2022-10-30 13:59:50.000000 refind-btrfs-0.6.0/src/refind_btrfs/data/icons/btrfs_logo/inverted_large.png
+-rw-rw-rw-   0        0        0      903 2022-10-30 13:59:50.000000 refind-btrfs-0.6.0/src/refind_btrfs/data/icons/btrfs_logo/inverted_medium.png
+-rw-rw-rw-   0        0        0      613 2022-10-30 13:59:50.000000 refind-btrfs-0.6.0/src/refind_btrfs/data/icons/btrfs_logo/inverted_small.png
+-rw-rw-rw-   0        0        0     1048 2022-10-30 13:59:50.000000 refind-btrfs-0.6.0/src/refind_btrfs/data/icons/btrfs_logo/original_large.png
+-rw-rw-rw-   0        0        0      835 2022-10-30 13:59:50.000000 refind-btrfs-0.6.0/src/refind_btrfs/data/icons/btrfs_logo/original_medium.png
+-rw-rw-rw-   0        0        0      562 2022-10-30 13:59:50.000000 refind-btrfs-0.6.0/src/refind_btrfs/data/icons/btrfs_logo/original_small.png
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:28.219876 refind-btrfs-0.6.0/src/refind_btrfs/data/images/
+-rw-rw-rw-   0        0        0    81467 2022-10-30 13:59:50.000000 refind-btrfs-0.6.0/src/refind_btrfs/data/images/refind_screenshot_default.png
+-rw-rw-rw-   0        0        0    31538 2022-10-30 13:59:50.000000 refind-btrfs-0.6.0/src/refind_btrfs/data/images/refind_screenshot_nord.png
+-rw-rw-rw-   0        0        0       57 2022-10-30 13:59:50.000000 refind-btrfs-0.6.0/src/refind_btrfs/data/refind-btrfs
+-rw-rw-rw-   0        0        0     9555 2022-10-30 13:59:50.000000 refind-btrfs-0.6.0/src/refind_btrfs/data/refind-btrfs.conf-sample
+-rw-rw-rw-   0        0        0      346 2022-10-30 13:59:50.000000 refind-btrfs-0.6.0/src/refind_btrfs/data/refind-btrfs.service
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:28.305594 refind-btrfs-0.6.0/src/refind_btrfs/device/
+-rw-rw-rw-   0        0        0     1163 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/device/__init__.py
+-rw-rw-rw-   0        0        0     5052 2023-03-28 10:42:13.000000 refind-btrfs-0.6.0/src/refind_btrfs/device/block_device.py
+-rw-rw-rw-   0        0        0     3718 2023-03-28 10:42:19.000000 refind-btrfs-0.6.0/src/refind_btrfs/device/filesystem.py
+-rw-rw-rw-   0        0        0     6390 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/device/mount_options.py
+-rw-rw-rw-   0        0        0     4427 2023-03-28 10:42:27.000000 refind-btrfs-0.6.0/src/refind_btrfs/device/partition.py
+-rw-rw-rw-   0        0        0     6350 2023-03-28 10:42:23.000000 refind-btrfs-0.6.0/src/refind_btrfs/device/partition_table.py
+-rw-rw-rw-   0        0        0    13652 2023-03-28 10:42:30.000000 refind-btrfs-0.6.0/src/refind_btrfs/device/subvolume.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:28.345594 refind-btrfs-0.6.0/src/refind_btrfs/service/
+-rw-rw-rw-   0        0        0     1057 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/service/__init__.py
+-rw-rw-rw-   0        0        0     7053 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/service/snapshot_event_handler.py
+-rw-rw-rw-   0        0        0     1940 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/service/snapshot_observer.py
+-rw-rw-rw-   0        0        0     5095 2023-03-27 23:04:48.000000 refind-btrfs-0.6.0/src/refind_btrfs/service/watchdog_runner.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:28.396599 refind-btrfs-0.6.0/src/refind_btrfs/state_management/
+-rw-rw-rw-   0        0        0      993 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/state_management/__init__.py
+-rw-rw-rw-   0        0        0    10282 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/state_management/conditions.py
+-rw-rw-rw-   0        0        0    18387 2023-03-28 10:42:36.000000 refind-btrfs-0.6.0/src/refind_btrfs/state_management/model.py
+-rw-rw-rw-   0        0        0     3569 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/state_management/refind_btrfs_machine.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:28.485599 refind-btrfs-0.6.0/src/refind_btrfs/system/
+-rw-rw-rw-   0        0        0     1045 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/system/__init__.py
+-rw-rw-rw-   0        0        0    12525 2023-03-27 23:04:48.000000 refind-btrfs-0.6.0/src/refind_btrfs/system/btrfsutil_command.py
+-rw-rw-rw-   0        0        0     2997 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/system/command_factories.py
+-rw-rw-rw-   0        0        0     6400 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/system/findmnt_command.py
+-rw-rw-rw-   0        0        0     5576 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/system/fstab_command.py
+-rw-rw-rw-   0        0        0     9146 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/system/lsblk_command.py
+-rw-rw-rw-   0        0        0    12414 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/system/pillow_command.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:28.568601 refind-btrfs-0.6.0/src/refind_btrfs/utility/
+-rw-rw-rw-   0        0        0      961 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/utility/__init__.py
+-rw-rw-rw-   0        0        0    22362 2023-03-28 10:34:48.000000 refind-btrfs-0.6.0/src/refind_btrfs/utility/file_package_config_provider.py
+-rw-rw-rw-   0        0        0     8118 2023-03-29 08:31:29.000000 refind-btrfs-0.6.0/src/refind_btrfs/utility/helpers.py
+-rw-rw-rw-   0        0        0     4021 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/utility/injector_modules.py
+-rw-rw-rw-   0        0        0     1512 2023-03-11 14:33:57.000000 refind-btrfs-0.6.0/src/refind_btrfs/utility/level_aware_formatter.py
+-rw-rw-rw-   0        0        0     1461 2023-03-27 23:04:48.000000 refind-btrfs-0.6.0/src/refind_btrfs/utility/logger_factories.py
+-rw-rw-rw-   0        0        0     5512 2023-03-27 22:48:41.000000 refind-btrfs-0.6.0/src/refind_btrfs/utility/shelve_persistence_provider.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:58:27.702021 refind-btrfs-0.6.0/src/refind_btrfs.egg-info/
+-rw-rw-rw-   0        0        0    28636 2023-05-11 09:58:27.000000 refind-btrfs-0.6.0/src/refind_btrfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4317 2023-05-11 09:58:27.000000 refind-btrfs-0.6.0/src/refind_btrfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 09:58:27.000000 refind-btrfs-0.6.0/src/refind_btrfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-11 09:58:27.000000 refind-btrfs-0.6.0/src/refind_btrfs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      144 2023-05-11 09:58:27.000000 refind-btrfs-0.6.0/src/refind_btrfs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-11 09:58:27.000000 refind-btrfs-0.6.0/src/refind_btrfs.egg-info/top_level.txt
```

### Comparing `refind-btrfs-0.5.6/LICENSE.txt` & `refind-btrfs-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `refind-btrfs-0.5.6/PKG-INFO` & `refind-btrfs-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: refind-btrfs
-Version: 0.5.6
+Version: 0.6.0
 Summary: Generate rEFInd manual boot stanzas from Btrfs snapshots
 Home-page: https://github.com/Venom1991/refind-btrfs
 Author: Luka Žaja
 Author-email: luka.zaja@protonmail.com
 Maintainer: Luka Žaja
 Maintainer-email: luka.zaja@protonmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Keywords: rEFInd,btrfs
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Boot
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: custom_icon
 License-File: LICENSE.txt
 
 # refind-btrfs
 
 ### Table of Contents
```

### Comparing `refind-btrfs-0.5.6/README.md` & `refind-btrfs-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `refind-btrfs-0.5.6/setup.cfg` & `refind-btrfs-0.6.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2072 6566 696e 645f 6274 7266 730d   = refind_btrfs.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e35 2e36  .version = 0.5.6
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e36 2e30  .version = 0.6.0
 00000030: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000040: 4765 6e65 7261 7465 2072 4546 496e 6420  Generate rEFInd 
 00000050: 6d61 6e75 616c 2062 6f6f 7420 7374 616e  manual boot stan
 00000060: 7a61 7320 6672 6f6d 2042 7472 6673 2073  zas from Btrfs s
 00000070: 6e61 7073 686f 7473 0d0a 6c6f 6e67 5f64  napshots..long_d
 00000080: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
 00000090: 653a 2052 4541 444d 452e 6d64 0d0a 6b65  e: README.md..ke
@@ -40,42 +40,42 @@
 00000270: 7465 7220 2847 504c 7633 2b29 0d0a 094e  ter (GPLv3+)...N
 00000280: 6174 7572 616c 204c 616e 6775 6167 6520  atural Language 
 00000290: 3a3a 2045 6e67 6c69 7368 0d0a 094f 7065  :: English...Ope
 000002a0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
 000002b0: 2050 4f53 4958 203a 3a20 4c69 6e75 780d   POSIX :: Linux.
 000002c0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
 000002d0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000002e0: 203a 3a20 332e 390d 0a09 546f 7069 6320   :: 3.9...Topic 
-000002f0: 3a3a 2053 7973 7465 6d20 3a3a 2042 6f6f  :: System :: Boo
-00000300: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
-00000310: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
-00000320: 093d 7372 630d 0a70 6163 6b61 6765 7320  .=src..packages 
-00000330: 3d20 6669 6e64 3a0d 0a69 6e63 6c75 6465  = find:..include
-00000340: 5f70 6163 6b61 6765 5f64 6174 6120 3d20  _package_data = 
-00000350: 5472 7565 0d0a 696e 7374 616c 6c5f 7265  True..install_re
-00000360: 7175 6972 6573 203d 200d 0a09 616e 746c  quires = ...antl
-00000370: 7234 2d70 7974 686f 6e33 2d72 756e 7469  r4-python3-runti
-00000380: 6d65 0d0a 0969 6e6a 6563 746f 720d 0a09  me...injector...
-00000390: 6d6f 7265 2d69 7465 7274 6f6f 6c73 0d0a  more-itertools..
-000003a0: 0970 6964 0d0a 0973 656d 616e 7469 632d  .pid...semantic-
-000003b0: 7665 7273 696f 6e0d 0a09 7379 7374 656d  version...system
-000003c0: 642d 7079 7468 6f6e 0d0a 0974 6f6d 6c6b  d-python...tomlk
-000003d0: 6974 0d0a 0974 7261 6e73 6974 696f 6e73  it...transitions
-000003e0: 0d0a 0974 7970 6567 7561 7264 0d0a 0977  ...typeguard...w
-000003f0: 6174 6368 646f 670d 0a70 7974 686f 6e5f  atchdog..python_
-00000400: 7265 7175 6972 6573 203d 203e 3d20 332e  requires = >= 3.
-00000410: 390d 0a0d 0a5b 6f70 7469 6f6e 732e 6578  9....[options.ex
-00000420: 7472 6173 5f72 6571 7569 7265 5d0d 0a63  tras_require]..c
-00000430: 7573 746f 6d5f 6963 6f6e 203d 2050 696c  ustom_icon = Pil
-00000440: 6c6f 770d 0a0d 0a5b 6f70 7469 6f6e 732e  low....[options.
-00000450: 656e 7472 795f 706f 696e 7473 5d0d 0a63  entry_points]..c
-00000460: 6f6e 736f 6c65 5f73 6372 6970 7473 203d  onsole_scripts =
-00000470: 200d 0a09 7265 6669 6e64 2d62 7472 6673   ...refind-btrfs
-00000480: 203d 2072 6566 696e 645f 6274 7266 733a   = refind_btrfs:
-00000490: 6d61 696e 0d0a 0d0a 5b6f 7074 696f 6e73  main....[options
-000004a0: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
-000004b0: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
-000004c0: 5b62 6469 7374 5f77 6865 656c 5d0d 0a75  [bdist_wheel]..u
-000004d0: 6e69 7665 7273 616c 203d 2046 616c 7365  niversal = False
-000004e0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-000004f0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000500: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+000002e0: 203a 3a20 332e 3131 0d0a 0954 6f70 6963   :: 3.11...Topic
+000002f0: 203a 3a20 5379 7374 656d 203a 3a20 426f   :: System :: Bo
+00000300: 6f74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  ot....[options].
+00000310: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
+00000320: 0a09 3d73 7263 0d0a 7061 636b 6167 6573  ..=src..packages
+00000330: 203d 2066 696e 643a 0d0a 696e 636c 7564   = find:..includ
+00000340: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
+00000350: 2054 7275 650d 0a69 6e73 7461 6c6c 5f72   True..install_r
+00000360: 6571 7569 7265 7320 3d20 0d0a 0961 6e74  equires = ...ant
+00000370: 6c72 342d 7079 7468 6f6e 332d 7275 6e74  lr4-python3-runt
+00000380: 696d 650d 0a09 696e 6a65 6374 6f72 0d0a  ime...injector..
+00000390: 096d 6f72 652d 6974 6572 746f 6f6c 730d  .more-itertools.
+000003a0: 0a09 7069 640d 0a09 7365 6d61 6e74 6963  ..pid...semantic
+000003b0: 2d76 6572 7369 6f6e 0d0a 0973 7973 7465  -version...syste
+000003c0: 6d64 2d70 7974 686f 6e0d 0a09 746f 6d6c  md-python...toml
+000003d0: 6b69 740d 0a09 7472 616e 7369 7469 6f6e  kit...transition
+000003e0: 730d 0a09 7479 7065 6775 6172 640d 0a09  s...typeguard...
+000003f0: 7761 7463 6864 6f67 0d0a 7079 7468 6f6e  watchdog..python
+00000400: 5f72 6571 7569 7265 7320 3d20 3e3d 2033  _requires = >= 3
+00000410: 2e31 310d 0a0d 0a5b 6f70 7469 6f6e 732e  .11....[options.
+00000420: 6578 7472 6173 5f72 6571 7569 7265 5d0d  extras_require].
+00000430: 0a63 7573 746f 6d5f 6963 6f6e 203d 2050  .custom_icon = P
+00000440: 696c 6c6f 770d 0a0d 0a5b 6f70 7469 6f6e  illow....[option
+00000450: 732e 656e 7472 795f 706f 696e 7473 5d0d  s.entry_points].
+00000460: 0a63 6f6e 736f 6c65 5f73 6372 6970 7473  .console_scripts
+00000470: 203d 200d 0a09 7265 6669 6e64 2d62 7472   = ...refind-btr
+00000480: 6673 203d 2072 6566 696e 645f 6274 7266  fs = refind_btrf
+00000490: 733a 6d61 696e 0d0a 0d0a 5b6f 7074 696f  s:main....[optio
+000004a0: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
+000004b0: 5d0d 0a77 6865 7265 203d 2073 7263 0d0a  ]..where = src..
+000004c0: 0d0a 5b62 6469 7374 5f77 6865 656c 5d0d  ..[bdist_wheel].
+000004d0: 0a75 6e69 7665 7273 616c 203d 2046 616c  .universal = Fal
+000004e0: 7365 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  se....[egg_info]
+000004f0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+00000500: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `refind-btrfs-0.5.6/setup.py` & `refind-btrfs-0.6.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -24,29 +24,29 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="refind-btrfs",
-    version="0.5.6",
+    version="0.6.0",
     author="Luka Žaja",
     author_email="luka.zaja@protonmail.com",
     description="Generate rEFInd manual boot stanzas from Btrfs snapshots",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="rEFInd, btrfs",
     url="https://github.com/Venom1991/refind-btrfs",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: End Users/Desktop",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Natural Language :: English",
         "Operating System :: POSIX :: Linux",
-        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.11",
         "Topic :: System :: Boot",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     include_package_data=True,
     install_requires=[
         "antlr4-python3-runtime",
@@ -62,9 +62,9 @@
     ],
     entry_points={
         "console_scripts": [
             "refind-btrfs=refind_btrfs:main",
         ],
     },
     extras_require={"custom_icon": ["Pillow"]},
-    python_requires=">=3.9",
+    python_requires=">=3.11",
 )
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/__init__.py` & `refind-btrfs-0.6.0/src/refind_btrfs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/__main__.py` & `refind-btrfs-0.6.0/src/refind_btrfs/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/boot/__init__.py` & `refind-btrfs-0.6.0/src/refind_btrfs/boot/migrations/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -17,11 +17,8 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # endregion
 
-from .boot_options import BootOptions
-from .boot_stanza import BootStanza
-from .refind_config import RefindConfig
-from .sub_menu import SubMenu
+from .migration import Migration
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/boot/antlr4/RefindConfigLexer.py` & `refind-btrfs-0.6.0/src/refind_btrfs/boot/antlr4/RefindConfigLexer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,361 +1,375 @@
-# Generated from /home/luka/Projects/Python/refind-btrfs/src/refind_btrfs/boot/antlr4/RefindConfigLexer.g4 by ANTLR 4.11.1
+# Generated from c:\Users\Luka\Projects\Python\refind-btrfs\src\refind_btrfs\boot\antlr4\RefindConfigLexer.g4 by ANTLR 4.12.0
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
 
 
 def serializedATN():
     return [
-        4,0,23,969,6,-1,6,-1,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,
-        7,5,2,6,7,6,2,7,7,7,2,8,7,8,2,9,7,9,2,10,7,10,2,11,7,11,2,12,7,12,
-        2,13,7,13,2,14,7,14,2,15,7,15,2,16,7,16,2,17,7,17,2,18,7,18,2,19,
-        7,19,2,20,7,20,2,21,7,21,2,22,7,22,2,23,7,23,2,24,7,24,2,25,7,25,
-        2,26,7,26,2,27,7,27,2,28,7,28,1,0,4,0,62,8,0,11,0,12,0,63,1,0,1,
-        0,1,1,3,1,69,8,1,1,1,1,1,1,1,1,1,1,2,3,2,76,8,2,1,2,1,2,1,2,1,2,
-        1,3,1,3,5,3,84,8,3,10,3,12,3,87,9,3,1,3,3,3,90,8,3,1,3,1,3,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,3,
-        4,751,8,4,1,4,5,4,754,8,4,10,4,12,4,757,9,4,1,4,3,4,760,8,4,1,4,
-        1,4,1,5,1,5,3,5,766,8,5,1,6,1,6,1,6,1,6,1,6,1,6,1,6,1,6,1,6,1,6,
-        1,7,1,7,1,7,1,7,1,7,1,7,1,7,1,7,1,7,1,7,1,7,1,7,1,7,1,8,1,8,1,8,
-        1,8,1,8,1,8,1,8,1,9,1,9,1,9,1,9,1,9,1,9,1,9,1,10,1,10,1,10,1,10,
-        1,10,1,10,1,10,1,11,1,11,1,11,1,11,1,11,1,12,1,12,1,12,1,12,1,12,
-        1,12,1,12,1,12,1,12,1,12,1,12,1,13,1,13,1,13,1,13,1,13,1,13,1,13,
-        1,13,1,13,1,13,1,13,1,13,1,13,1,14,1,14,1,14,1,14,1,14,1,14,1,14,
-        1,14,1,15,1,15,1,15,1,15,1,15,1,15,1,15,1,15,1,15,1,15,1,15,1,15,
-        1,16,1,16,1,16,1,16,1,16,1,16,1,16,1,16,1,16,1,16,1,16,1,16,1,16,
-        1,16,1,16,1,16,1,16,1,17,1,17,1,17,1,17,1,17,1,17,1,17,1,17,1,17,
-        1,18,1,18,1,18,1,18,1,18,1,18,1,18,1,18,1,19,1,19,1,20,1,20,1,21,
-        4,21,900,8,21,11,21,12,21,901,1,22,1,22,1,23,1,23,1,23,3,23,909,
-        8,23,1,24,1,24,4,24,913,8,24,11,24,12,24,914,1,24,1,24,1,25,1,25,
-        4,25,921,8,25,11,25,12,25,922,1,25,1,25,1,26,4,26,928,8,26,11,26,
-        12,26,929,1,27,1,27,1,27,1,27,1,27,1,27,1,27,1,27,1,27,1,27,1,27,
+        4,0,23,1007,6,-1,6,-1,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,
+        5,7,5,2,6,7,6,2,7,7,7,2,8,7,8,2,9,7,9,2,10,7,10,2,11,7,11,2,12,7,
+        12,2,13,7,13,2,14,7,14,2,15,7,15,2,16,7,16,2,17,7,17,2,18,7,18,2,
+        19,7,19,2,20,7,20,2,21,7,21,2,22,7,22,2,23,7,23,2,24,7,24,2,25,7,
+        25,2,26,7,26,2,27,7,27,2,28,7,28,1,0,4,0,62,8,0,11,0,12,0,63,1,0,
+        1,0,1,1,3,1,69,8,1,1,1,1,1,1,1,1,1,1,2,3,2,76,8,2,1,2,1,2,1,2,1,
+        2,1,3,1,3,5,3,84,8,3,10,3,12,3,87,9,3,1,3,3,3,90,8,3,1,3,1,3,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,
+        1,4,1,4,1,4,1,4,1,4,1,4,3,4,789,8,4,1,4,5,4,792,8,4,10,4,12,4,795,
+        9,4,1,4,3,4,798,8,4,1,4,1,4,1,5,1,5,3,5,804,8,5,1,6,1,6,1,6,1,6,
+        1,6,1,6,1,6,1,6,1,6,1,6,1,7,1,7,1,7,1,7,1,7,1,7,1,7,1,7,1,7,1,7,
+        1,7,1,7,1,7,1,8,1,8,1,8,1,8,1,8,1,8,1,8,1,9,1,9,1,9,1,9,1,9,1,9,
+        1,9,1,10,1,10,1,10,1,10,1,10,1,10,1,10,1,11,1,11,1,11,1,11,1,11,
+        1,12,1,12,1,12,1,12,1,12,1,12,1,12,1,12,1,12,1,12,1,12,1,13,1,13,
+        1,13,1,13,1,13,1,13,1,13,1,13,1,13,1,13,1,13,1,13,1,13,1,14,1,14,
+        1,14,1,14,1,14,1,14,1,14,1,14,1,15,1,15,1,15,1,15,1,15,1,15,1,15,
+        1,15,1,15,1,15,1,15,1,15,1,16,1,16,1,16,1,16,1,16,1,16,1,16,1,16,
+        1,16,1,16,1,16,1,16,1,16,1,16,1,16,1,16,1,16,1,17,1,17,1,17,1,17,
+        1,17,1,17,1,17,1,17,1,17,1,18,1,18,1,18,1,18,1,18,1,18,1,18,1,18,
+        1,19,1,19,1,20,1,20,1,21,4,21,938,8,21,11,21,12,21,939,1,22,1,22,
+        1,23,1,23,1,23,3,23,947,8,23,1,24,1,24,4,24,951,8,24,11,24,12,24,
+        952,1,24,1,24,1,25,1,25,4,25,959,8,25,11,25,12,25,960,1,25,1,25,
+        1,26,4,26,966,8,26,11,26,12,26,967,1,27,1,27,1,27,1,27,1,27,1,27,
         1,27,1,27,1,27,1,27,1,27,1,27,1,27,1,27,1,27,1,27,1,27,1,27,1,27,
-        1,27,3,27,957,8,27,1,27,1,27,1,28,1,28,1,28,1,28,1,28,3,28,966,8,
-        28,1,28,1,28,0,0,29,2,1,4,2,6,3,8,4,10,5,12,6,14,0,16,0,18,7,20,
-        8,22,9,24,10,26,11,28,12,30,13,32,14,34,15,36,16,38,17,40,18,42,
-        19,44,20,46,0,48,21,50,0,52,0,54,0,56,22,58,23,2,0,1,4,2,0,9,9,32,
-        32,1,0,10,10,3,0,48,57,65,70,97,102,2,0,9,10,32,32,1027,0,2,1,0,
-        0,0,0,4,1,0,0,0,0,6,1,0,0,0,0,8,1,0,0,0,0,10,1,0,0,0,0,12,1,0,0,
-        0,0,18,1,0,0,0,0,20,1,0,0,0,0,22,1,0,0,0,0,24,1,0,0,0,0,26,1,0,0,
-        0,0,28,1,0,0,0,0,30,1,0,0,0,0,32,1,0,0,0,0,34,1,0,0,0,0,36,1,0,0,
-        0,0,38,1,0,0,0,0,40,1,0,0,0,0,42,1,0,0,0,0,44,1,0,0,0,0,48,1,0,0,
-        0,1,56,1,0,0,0,1,58,1,0,0,0,2,61,1,0,0,0,4,68,1,0,0,0,6,75,1,0,0,
-        0,8,81,1,0,0,0,10,750,1,0,0,0,12,765,1,0,0,0,14,767,1,0,0,0,16,777,
-        1,0,0,0,18,790,1,0,0,0,20,797,1,0,0,0,22,804,1,0,0,0,24,811,1,0,
-        0,0,26,816,1,0,0,0,28,827,1,0,0,0,30,840,1,0,0,0,32,848,1,0,0,0,
-        34,860,1,0,0,0,36,877,1,0,0,0,38,886,1,0,0,0,40,894,1,0,0,0,42,896,
-        1,0,0,0,44,899,1,0,0,0,46,903,1,0,0,0,48,908,1,0,0,0,50,910,1,0,
-        0,0,52,918,1,0,0,0,54,927,1,0,0,0,56,956,1,0,0,0,58,965,1,0,0,0,
-        60,62,7,0,0,0,61,60,1,0,0,0,62,63,1,0,0,0,63,61,1,0,0,0,63,64,1,
-        0,0,0,64,65,1,0,0,0,65,66,6,0,0,0,66,3,1,0,0,0,67,69,5,13,0,0,68,
-        67,1,0,0,0,68,69,1,0,0,0,69,70,1,0,0,0,70,71,5,10,0,0,71,72,1,0,
-        0,0,72,73,6,1,0,0,73,5,1,0,0,0,74,76,3,2,0,0,75,74,1,0,0,0,75,76,
-        1,0,0,0,76,77,1,0,0,0,77,78,3,4,1,0,78,79,1,0,0,0,79,80,6,2,0,0,
-        80,7,1,0,0,0,81,85,5,35,0,0,82,84,8,1,0,0,83,82,1,0,0,0,84,87,1,
-        0,0,0,85,83,1,0,0,0,85,86,1,0,0,0,86,89,1,0,0,0,87,85,1,0,0,0,88,
-        90,3,4,1,0,89,88,1,0,0,0,89,90,1,0,0,0,90,91,1,0,0,0,91,92,6,3,0,
-        0,92,9,1,0,0,0,93,94,5,116,0,0,94,95,5,105,0,0,95,96,5,109,0,0,96,
-        97,5,101,0,0,97,98,5,111,0,0,98,99,5,117,0,0,99,751,5,116,0,0,100,
-        101,5,97,0,0,101,102,5,108,0,0,102,103,5,115,0,0,103,104,5,111,0,
-        0,104,105,5,95,0,0,105,106,5,115,0,0,106,107,5,99,0,0,107,108,5,
-        97,0,0,108,109,5,110,0,0,109,110,5,95,0,0,110,111,5,100,0,0,111,
-        112,5,105,0,0,112,113,5,114,0,0,113,751,5,115,0,0,114,115,5,98,0,
-        0,115,116,5,97,0,0,116,117,5,110,0,0,117,118,5,110,0,0,118,119,5,
-        101,0,0,119,751,5,114,0,0,120,121,5,98,0,0,121,122,5,97,0,0,122,
-        123,5,110,0,0,123,124,5,110,0,0,124,125,5,101,0,0,125,126,5,114,
-        0,0,126,127,5,95,0,0,127,128,5,115,0,0,128,129,5,99,0,0,129,130,
-        5,97,0,0,130,131,5,108,0,0,131,751,5,101,0,0,132,133,5,98,0,0,133,
-        134,5,105,0,0,134,135,5,103,0,0,135,136,5,95,0,0,136,137,5,105,0,
-        0,137,138,5,99,0,0,138,139,5,111,0,0,139,140,5,110,0,0,140,141,5,
-        95,0,0,141,142,5,115,0,0,142,143,5,105,0,0,143,144,5,122,0,0,144,
-        751,5,101,0,0,145,146,5,99,0,0,146,147,5,115,0,0,147,148,5,114,0,
-        0,148,149,5,95,0,0,149,150,5,118,0,0,150,151,5,97,0,0,151,152,5,
-        108,0,0,152,153,5,117,0,0,153,154,5,101,0,0,154,751,5,115,0,0,155,
-        156,5,100,0,0,156,157,5,101,0,0,157,158,5,102,0,0,158,159,5,97,0,
-        0,159,160,5,117,0,0,160,161,5,108,0,0,161,162,5,116,0,0,162,163,
-        5,95,0,0,163,164,5,115,0,0,164,165,5,101,0,0,165,166,5,108,0,0,166,
-        167,5,101,0,0,167,168,5,99,0,0,168,169,5,116,0,0,169,170,5,105,0,
-        0,170,171,5,111,0,0,171,751,5,110,0,0,172,173,5,100,0,0,173,174,
-        5,111,0,0,174,175,5,110,0,0,175,176,5,39,0,0,176,177,5,116,0,0,177,
-        178,5,95,0,0,178,179,5,115,0,0,179,180,5,99,0,0,180,181,5,97,0,0,
-        181,182,5,110,0,0,182,183,5,95,0,0,183,184,5,100,0,0,184,185,5,105,
-        0,0,185,186,5,114,0,0,186,751,5,115,0,0,187,188,5,100,0,0,188,189,
-        5,111,0,0,189,190,5,110,0,0,190,191,5,39,0,0,191,192,5,116,0,0,192,
-        193,5,95,0,0,193,194,5,115,0,0,194,195,5,99,0,0,195,196,5,97,0,0,
-        196,197,5,110,0,0,197,198,5,95,0,0,198,199,5,102,0,0,199,200,5,105,
-        0,0,200,201,5,108,0,0,201,202,5,101,0,0,202,751,5,115,0,0,203,204,
-        5,100,0,0,204,205,5,111,0,0,205,206,5,110,0,0,206,207,5,39,0,0,207,
-        208,5,116,0,0,208,209,5,95,0,0,209,210,5,115,0,0,210,211,5,99,0,
-        0,211,212,5,97,0,0,212,213,5,110,0,0,213,214,5,95,0,0,214,215,5,
-        102,0,0,215,216,5,105,0,0,216,217,5,114,0,0,217,218,5,109,0,0,218,
-        219,5,119,0,0,219,220,5,97,0,0,220,221,5,114,0,0,221,751,5,101,0,
-        0,222,223,5,100,0,0,223,224,5,111,0,0,224,225,5,110,0,0,225,226,
-        5,39,0,0,226,227,5,116,0,0,227,228,5,95,0,0,228,229,5,115,0,0,229,
-        230,5,99,0,0,230,231,5,97,0,0,231,232,5,110,0,0,232,233,5,95,0,0,
-        233,234,5,116,0,0,234,235,5,111,0,0,235,236,5,111,0,0,236,237,5,
-        108,0,0,237,751,5,115,0,0,238,239,5,100,0,0,239,240,5,111,0,0,240,
-        241,5,110,0,0,241,242,5,39,0,0,242,243,5,116,0,0,243,244,5,95,0,
-        0,244,245,5,115,0,0,245,246,5,99,0,0,246,247,5,97,0,0,247,248,5,
-        110,0,0,248,249,5,95,0,0,249,250,5,118,0,0,250,251,5,111,0,0,251,
-        252,5,108,0,0,252,253,5,117,0,0,253,254,5,109,0,0,254,255,5,101,
-        0,0,255,751,5,115,0,0,256,257,5,100,0,0,257,258,5,111,0,0,258,259,
-        5,110,0,0,259,260,5,116,0,0,260,261,5,95,0,0,261,262,5,115,0,0,262,
-        263,5,99,0,0,263,264,5,97,0,0,264,265,5,110,0,0,265,266,5,95,0,0,
-        266,267,5,100,0,0,267,268,5,105,0,0,268,269,5,114,0,0,269,751,5,
-        115,0,0,270,271,5,100,0,0,271,272,5,111,0,0,272,273,5,110,0,0,273,
-        274,5,116,0,0,274,275,5,95,0,0,275,276,5,115,0,0,276,277,5,99,0,
-        0,277,278,5,97,0,0,278,279,5,110,0,0,279,280,5,95,0,0,280,281,5,
-        102,0,0,281,282,5,105,0,0,282,283,5,108,0,0,283,284,5,101,0,0,284,
-        751,5,115,0,0,285,286,5,100,0,0,286,287,5,111,0,0,287,288,5,110,
-        0,0,288,289,5,116,0,0,289,290,5,95,0,0,290,291,5,115,0,0,291,292,
-        5,99,0,0,292,293,5,97,0,0,293,294,5,110,0,0,294,295,5,95,0,0,295,
-        296,5,102,0,0,296,297,5,105,0,0,297,298,5,114,0,0,298,299,5,109,
-        0,0,299,300,5,119,0,0,300,301,5,97,0,0,301,302,5,114,0,0,302,751,
-        5,101,0,0,303,304,5,100,0,0,304,305,5,111,0,0,305,306,5,110,0,0,
-        306,307,5,116,0,0,307,308,5,95,0,0,308,309,5,115,0,0,309,310,5,99,
-        0,0,310,311,5,97,0,0,311,312,5,110,0,0,312,313,5,95,0,0,313,314,
-        5,116,0,0,314,315,5,111,0,0,315,316,5,111,0,0,316,317,5,108,0,0,
-        317,751,5,115,0,0,318,319,5,100,0,0,319,320,5,111,0,0,320,321,5,
-        110,0,0,321,322,5,116,0,0,322,323,5,95,0,0,323,324,5,115,0,0,324,
-        325,5,99,0,0,325,326,5,97,0,0,326,327,5,110,0,0,327,328,5,95,0,0,
-        328,329,5,118,0,0,329,330,5,111,0,0,330,331,5,108,0,0,331,332,5,
-        117,0,0,332,333,5,109,0,0,333,334,5,101,0,0,334,751,5,115,0,0,335,
-        336,5,101,0,0,336,337,5,110,0,0,337,338,5,97,0,0,338,339,5,98,0,
-        0,339,340,5,108,0,0,340,341,5,101,0,0,341,342,5,95,0,0,342,343,5,
-        97,0,0,343,344,5,110,0,0,344,345,5,100,0,0,345,346,5,95,0,0,346,
-        347,5,108,0,0,347,348,5,111,0,0,348,349,5,99,0,0,349,350,5,107,0,
-        0,350,351,5,95,0,0,351,352,5,118,0,0,352,353,5,109,0,0,353,751,5,
-        120,0,0,354,355,5,101,0,0,355,356,5,110,0,0,356,357,5,97,0,0,357,
-        358,5,98,0,0,358,359,5,108,0,0,359,360,5,101,0,0,360,361,5,95,0,
-        0,361,362,5,109,0,0,362,363,5,111,0,0,363,364,5,117,0,0,364,365,
-        5,115,0,0,365,751,5,101,0,0,366,367,5,101,0,0,367,368,5,110,0,0,
-        368,369,5,97,0,0,369,370,5,98,0,0,370,371,5,108,0,0,371,372,5,101,
-        0,0,372,373,5,95,0,0,373,374,5,116,0,0,374,375,5,111,0,0,375,376,
-        5,117,0,0,376,377,5,99,0,0,377,751,5,104,0,0,378,379,5,101,0,0,379,
-        380,5,120,0,0,380,381,5,116,0,0,381,382,5,114,0,0,382,383,5,97,0,
-        0,383,384,5,95,0,0,384,385,5,107,0,0,385,386,5,101,0,0,386,387,5,
-        114,0,0,387,388,5,110,0,0,388,389,5,101,0,0,389,390,5,108,0,0,390,
-        391,5,95,0,0,391,392,5,118,0,0,392,393,5,101,0,0,393,394,5,114,0,
-        0,394,395,5,115,0,0,395,396,5,105,0,0,396,397,5,111,0,0,397,398,
-        5,110,0,0,398,399,5,95,0,0,399,400,5,115,0,0,400,401,5,116,0,0,401,
-        402,5,114,0,0,402,403,5,105,0,0,403,404,5,110,0,0,404,405,5,103,
-        0,0,405,751,5,115,0,0,406,407,5,102,0,0,407,408,5,111,0,0,408,409,
-        5,108,0,0,409,410,5,100,0,0,410,411,5,95,0,0,411,412,5,108,0,0,412,
-        413,5,105,0,0,413,414,5,110,0,0,414,415,5,117,0,0,415,416,5,120,
-        0,0,416,417,5,95,0,0,417,418,5,107,0,0,418,419,5,101,0,0,419,420,
-        5,114,0,0,420,421,5,110,0,0,421,422,5,101,0,0,422,423,5,108,0,0,
-        423,751,5,115,0,0,424,425,5,102,0,0,425,426,5,111,0,0,426,427,5,
-        110,0,0,427,751,5,116,0,0,428,429,5,104,0,0,429,430,5,105,0,0,430,
-        431,5,100,0,0,431,432,5,101,0,0,432,433,5,117,0,0,433,751,5,105,
-        0,0,434,435,5,105,0,0,435,436,5,99,0,0,436,437,5,111,0,0,437,438,
-        5,110,0,0,438,439,5,115,0,0,439,440,5,95,0,0,440,441,5,100,0,0,441,
-        442,5,105,0,0,442,751,5,114,0,0,443,444,5,108,0,0,444,445,5,111,
-        0,0,445,446,5,103,0,0,446,447,5,95,0,0,447,448,5,108,0,0,448,449,
-        5,101,0,0,449,450,5,118,0,0,450,451,5,101,0,0,451,751,5,108,0,0,
-        452,453,5,109,0,0,453,454,5,97,0,0,454,455,5,120,0,0,455,456,5,95,
-        0,0,456,457,5,116,0,0,457,458,5,97,0,0,458,459,5,103,0,0,459,751,
-        5,115,0,0,460,461,5,109,0,0,461,462,5,111,0,0,462,463,5,117,0,0,
-        463,464,5,115,0,0,464,465,5,101,0,0,465,466,5,95,0,0,466,467,5,115,
-        0,0,467,468,5,105,0,0,468,469,5,122,0,0,469,751,5,101,0,0,470,471,
-        5,109,0,0,471,472,5,111,0,0,472,473,5,117,0,0,473,474,5,115,0,0,
-        474,475,5,101,0,0,475,476,5,95,0,0,476,477,5,115,0,0,477,478,5,112,
-        0,0,478,479,5,101,0,0,479,480,5,101,0,0,480,751,5,100,0,0,481,482,
-        5,114,0,0,482,483,5,101,0,0,483,484,5,115,0,0,484,485,5,111,0,0,
-        485,486,5,108,0,0,486,487,5,117,0,0,487,488,5,116,0,0,488,489,5,
-        105,0,0,489,490,5,111,0,0,490,751,5,110,0,0,491,492,5,115,0,0,492,
-        493,5,99,0,0,493,494,5,97,0,0,494,495,5,110,0,0,495,496,5,95,0,0,
-        496,497,5,97,0,0,497,498,5,108,0,0,498,499,5,108,0,0,499,500,5,95,
-        0,0,500,501,5,108,0,0,501,502,5,105,0,0,502,503,5,110,0,0,503,504,
-        5,117,0,0,504,505,5,120,0,0,505,506,5,95,0,0,506,507,5,107,0,0,507,
-        508,5,101,0,0,508,509,5,114,0,0,509,510,5,110,0,0,510,511,5,101,
-        0,0,511,512,5,108,0,0,512,751,5,115,0,0,513,514,5,115,0,0,514,515,
-        5,99,0,0,515,516,5,97,0,0,516,517,5,110,0,0,517,518,5,95,0,0,518,
-        519,5,100,0,0,519,520,5,101,0,0,520,521,5,108,0,0,521,522,5,97,0,
-        0,522,751,5,121,0,0,523,524,5,115,0,0,524,525,5,99,0,0,525,526,5,
-        97,0,0,526,527,5,110,0,0,527,528,5,95,0,0,528,529,5,100,0,0,529,
-        530,5,114,0,0,530,531,5,105,0,0,531,532,5,118,0,0,532,533,5,101,
-        0,0,533,534,5,114,0,0,534,535,5,95,0,0,535,536,5,100,0,0,536,537,
-        5,105,0,0,537,538,5,114,0,0,538,751,5,115,0,0,539,540,5,115,0,0,
-        540,541,5,99,0,0,541,542,5,97,0,0,542,543,5,110,0,0,543,544,5,102,
-        0,0,544,545,5,111,0,0,545,751,5,114,0,0,546,547,5,115,0,0,547,548,
-        5,99,0,0,548,549,5,114,0,0,549,550,5,101,0,0,550,551,5,101,0,0,551,
-        552,5,110,0,0,552,553,5,115,0,0,553,554,5,97,0,0,554,555,5,118,0,
-        0,555,556,5,101,0,0,556,751,5,114,0,0,557,558,5,115,0,0,558,559,
-        5,101,0,0,559,560,5,108,0,0,560,561,5,101,0,0,561,562,5,99,0,0,562,
-        563,5,116,0,0,563,564,5,105,0,0,564,565,5,111,0,0,565,566,5,110,
-        0,0,566,567,5,95,0,0,567,568,5,98,0,0,568,569,5,105,0,0,569,751,
-        5,103,0,0,570,571,5,115,0,0,571,572,5,101,0,0,572,573,5,108,0,0,
-        573,574,5,101,0,0,574,575,5,99,0,0,575,576,5,116,0,0,576,577,5,105,
-        0,0,577,578,5,111,0,0,578,579,5,110,0,0,579,580,5,95,0,0,580,581,
-        5,115,0,0,581,582,5,109,0,0,582,583,5,97,0,0,583,584,5,108,0,0,584,
-        751,5,108,0,0,585,586,5,115,0,0,586,587,5,104,0,0,587,588,5,111,
-        0,0,588,589,5,119,0,0,589,590,5,116,0,0,590,591,5,111,0,0,591,592,
-        5,111,0,0,592,593,5,108,0,0,593,751,5,115,0,0,594,595,5,115,0,0,
-        595,596,5,104,0,0,596,597,5,117,0,0,597,598,5,116,0,0,598,599,5,
-        100,0,0,599,600,5,111,0,0,600,601,5,119,0,0,601,602,5,110,0,0,602,
-        603,5,95,0,0,603,604,5,97,0,0,604,605,5,102,0,0,605,606,5,116,0,
-        0,606,607,5,101,0,0,607,608,5,114,0,0,608,609,5,95,0,0,609,610,5,
-        116,0,0,610,611,5,105,0,0,611,612,5,109,0,0,612,613,5,101,0,0,613,
-        614,5,111,0,0,614,615,5,117,0,0,615,751,5,116,0,0,616,617,5,115,
-        0,0,617,618,5,109,0,0,618,619,5,97,0,0,619,620,5,108,0,0,620,621,
-        5,108,0,0,621,622,5,95,0,0,622,623,5,105,0,0,623,624,5,99,0,0,624,
-        625,5,111,0,0,625,626,5,110,0,0,626,627,5,95,0,0,627,628,5,115,0,
-        0,628,629,5,105,0,0,629,630,5,122,0,0,630,751,5,101,0,0,631,632,
-        5,115,0,0,632,633,5,112,0,0,633,634,5,111,0,0,634,635,5,111,0,0,
-        635,636,5,102,0,0,636,637,5,95,0,0,637,638,5,111,0,0,638,639,5,115,
-        0,0,639,640,5,120,0,0,640,641,5,95,0,0,641,642,5,118,0,0,642,643,
-        5,101,0,0,643,644,5,114,0,0,644,645,5,115,0,0,645,646,5,105,0,0,
-        646,647,5,111,0,0,647,751,5,110,0,0,648,649,5,116,0,0,649,650,5,
-        101,0,0,650,651,5,120,0,0,651,652,5,116,0,0,652,653,5,109,0,0,653,
-        654,5,111,0,0,654,655,5,100,0,0,655,751,5,101,0,0,656,657,5,116,
-        0,0,657,658,5,101,0,0,658,659,5,120,0,0,659,660,5,116,0,0,660,661,
-        5,111,0,0,661,662,5,110,0,0,662,663,5,108,0,0,663,751,5,121,0,0,
-        664,665,5,117,0,0,665,666,5,101,0,0,666,667,5,102,0,0,667,668,5,
-        105,0,0,668,669,5,95,0,0,669,670,5,100,0,0,670,671,5,101,0,0,671,
-        672,5,101,0,0,672,673,5,112,0,0,673,674,5,95,0,0,674,675,5,108,0,
-        0,675,676,5,101,0,0,676,677,5,103,0,0,677,678,5,97,0,0,678,679,5,
-        99,0,0,679,680,5,121,0,0,680,681,5,95,0,0,681,682,5,115,0,0,682,
-        683,5,99,0,0,683,684,5,97,0,0,684,751,5,110,0,0,685,686,5,117,0,
-        0,686,687,5,115,0,0,687,688,5,101,0,0,688,689,5,95,0,0,689,690,5,
-        103,0,0,690,691,5,114,0,0,691,692,5,97,0,0,692,693,5,112,0,0,693,
-        694,5,104,0,0,694,695,5,105,0,0,695,696,5,99,0,0,696,697,5,115,0,
-        0,697,698,5,95,0,0,698,699,5,102,0,0,699,700,5,111,0,0,700,751,5,
-        114,0,0,701,702,5,117,0,0,702,703,5,115,0,0,703,704,5,101,0,0,704,
-        705,5,95,0,0,705,706,5,110,0,0,706,707,5,118,0,0,707,708,5,114,0,
-        0,708,709,5,97,0,0,709,751,5,109,0,0,710,711,5,119,0,0,711,712,5,
-        105,0,0,712,713,5,110,0,0,713,714,5,100,0,0,714,715,5,111,0,0,715,
-        716,5,119,0,0,716,717,5,115,0,0,717,718,5,95,0,0,718,719,5,114,0,
-        0,719,720,5,101,0,0,720,721,5,99,0,0,721,722,5,111,0,0,722,723,5,
-        118,0,0,723,724,5,101,0,0,724,725,5,114,0,0,725,726,5,121,0,0,726,
-        727,5,95,0,0,727,728,5,102,0,0,728,729,5,105,0,0,729,730,5,108,0,
-        0,730,731,5,101,0,0,731,751,5,115,0,0,732,733,5,119,0,0,733,734,
-        5,114,0,0,734,735,5,105,0,0,735,736,5,116,0,0,736,737,5,101,0,0,
-        737,738,5,95,0,0,738,739,5,115,0,0,739,740,5,121,0,0,740,741,5,115,
-        0,0,741,742,5,116,0,0,742,743,5,101,0,0,743,744,5,109,0,0,744,745,
-        5,100,0,0,745,746,5,95,0,0,746,747,5,118,0,0,747,748,5,97,0,0,748,
-        749,5,114,0,0,749,751,5,115,0,0,750,93,1,0,0,0,750,100,1,0,0,0,750,
-        114,1,0,0,0,750,120,1,0,0,0,750,132,1,0,0,0,750,145,1,0,0,0,750,
-        155,1,0,0,0,750,172,1,0,0,0,750,187,1,0,0,0,750,203,1,0,0,0,750,
-        222,1,0,0,0,750,238,1,0,0,0,750,256,1,0,0,0,750,270,1,0,0,0,750,
-        285,1,0,0,0,750,303,1,0,0,0,750,318,1,0,0,0,750,335,1,0,0,0,750,
-        354,1,0,0,0,750,366,1,0,0,0,750,378,1,0,0,0,750,406,1,0,0,0,750,
-        424,1,0,0,0,750,428,1,0,0,0,750,434,1,0,0,0,750,443,1,0,0,0,750,
-        452,1,0,0,0,750,460,1,0,0,0,750,470,1,0,0,0,750,481,1,0,0,0,750,
-        491,1,0,0,0,750,513,1,0,0,0,750,523,1,0,0,0,750,539,1,0,0,0,750,
-        546,1,0,0,0,750,557,1,0,0,0,750,570,1,0,0,0,750,585,1,0,0,0,750,
-        594,1,0,0,0,750,616,1,0,0,0,750,631,1,0,0,0,750,648,1,0,0,0,750,
-        656,1,0,0,0,750,664,1,0,0,0,750,685,1,0,0,0,750,701,1,0,0,0,750,
-        710,1,0,0,0,750,732,1,0,0,0,751,755,1,0,0,0,752,754,8,1,0,0,753,
-        752,1,0,0,0,754,757,1,0,0,0,755,753,1,0,0,0,755,756,1,0,0,0,756,
-        759,1,0,0,0,757,755,1,0,0,0,758,760,3,4,1,0,759,758,1,0,0,0,759,
-        760,1,0,0,0,760,761,1,0,0,0,761,762,6,4,0,0,762,11,1,0,0,0,763,766,
-        3,14,6,0,764,766,3,16,7,0,765,763,1,0,0,0,765,764,1,0,0,0,766,13,
-        1,0,0,0,767,768,5,109,0,0,768,769,5,101,0,0,769,770,5,110,0,0,770,
-        771,5,117,0,0,771,772,5,101,0,0,772,773,5,110,0,0,773,774,5,116,
-        0,0,774,775,5,114,0,0,775,776,5,121,0,0,776,15,1,0,0,0,777,778,5,
-        115,0,0,778,779,5,117,0,0,779,780,5,98,0,0,780,781,5,109,0,0,781,
-        782,5,101,0,0,782,783,5,110,0,0,783,784,5,117,0,0,784,785,5,101,
-        0,0,785,786,5,110,0,0,786,787,5,116,0,0,787,788,5,114,0,0,788,789,
-        5,121,0,0,789,17,1,0,0,0,790,791,5,118,0,0,791,792,5,111,0,0,792,
-        793,5,108,0,0,793,794,5,117,0,0,794,795,5,109,0,0,795,796,5,101,
-        0,0,796,19,1,0,0,0,797,798,5,108,0,0,798,799,5,111,0,0,799,800,5,
-        97,0,0,800,801,5,100,0,0,801,802,5,101,0,0,802,803,5,114,0,0,803,
-        21,1,0,0,0,804,805,5,105,0,0,805,806,5,110,0,0,806,807,5,105,0,0,
-        807,808,5,116,0,0,808,809,5,114,0,0,809,810,5,100,0,0,810,23,1,0,
-        0,0,811,812,5,105,0,0,812,813,5,99,0,0,813,814,5,111,0,0,814,815,
-        5,110,0,0,815,25,1,0,0,0,816,817,5,111,0,0,817,818,5,115,0,0,818,
-        819,5,116,0,0,819,820,5,121,0,0,820,821,5,112,0,0,821,822,5,101,
-        0,0,822,823,1,0,0,0,823,824,3,2,0,0,824,825,1,0,0,0,825,826,6,12,
-        1,0,826,27,1,0,0,0,827,828,5,103,0,0,828,829,5,114,0,0,829,830,5,
-        97,0,0,830,831,5,112,0,0,831,832,5,104,0,0,832,833,5,105,0,0,833,
-        834,5,99,0,0,834,835,5,115,0,0,835,836,1,0,0,0,836,837,3,2,0,0,837,
-        838,1,0,0,0,838,839,6,13,1,0,839,29,1,0,0,0,840,841,5,111,0,0,841,
-        842,5,112,0,0,842,843,5,116,0,0,843,844,5,105,0,0,844,845,5,111,
-        0,0,845,846,5,110,0,0,846,847,5,115,0,0,847,31,1,0,0,0,848,849,5,
-        97,0,0,849,850,5,100,0,0,850,851,5,100,0,0,851,852,5,95,0,0,852,
-        853,5,111,0,0,853,854,5,112,0,0,854,855,5,116,0,0,855,856,5,105,
-        0,0,856,857,5,111,0,0,857,858,5,110,0,0,858,859,5,115,0,0,859,33,
-        1,0,0,0,860,861,5,102,0,0,861,862,5,105,0,0,862,863,5,114,0,0,863,
-        864,5,109,0,0,864,865,5,119,0,0,865,866,5,97,0,0,866,867,5,114,0,
-        0,867,868,5,101,0,0,868,869,5,95,0,0,869,870,5,98,0,0,870,871,5,
-        111,0,0,871,872,5,111,0,0,872,873,5,116,0,0,873,874,5,110,0,0,874,
-        875,5,117,0,0,875,876,5,109,0,0,876,35,1,0,0,0,877,878,5,100,0,0,
-        878,879,5,105,0,0,879,880,5,115,0,0,880,881,5,97,0,0,881,882,5,98,
-        0,0,882,883,5,108,0,0,883,884,5,101,0,0,884,885,5,100,0,0,885,37,
-        1,0,0,0,886,887,5,105,0,0,887,888,5,110,0,0,888,889,5,99,0,0,889,
-        890,5,108,0,0,890,891,5,117,0,0,891,892,5,100,0,0,892,893,5,101,
-        0,0,893,39,1,0,0,0,894,895,5,123,0,0,895,41,1,0,0,0,896,897,5,125,
-        0,0,897,43,1,0,0,0,898,900,3,46,22,0,899,898,1,0,0,0,900,901,1,0,
-        0,0,901,899,1,0,0,0,901,902,1,0,0,0,902,45,1,0,0,0,903,904,7,2,0,
-        0,904,47,1,0,0,0,905,909,3,50,24,0,906,909,3,52,25,0,907,909,3,54,
-        26,0,908,905,1,0,0,0,908,906,1,0,0,0,908,907,1,0,0,0,909,49,1,0,
-        0,0,910,912,5,39,0,0,911,913,8,1,0,0,912,911,1,0,0,0,913,914,1,0,
-        0,0,914,912,1,0,0,0,914,915,1,0,0,0,915,916,1,0,0,0,916,917,5,39,
-        0,0,917,51,1,0,0,0,918,920,5,34,0,0,919,921,8,1,0,0,920,919,1,0,
-        0,0,921,922,1,0,0,0,922,920,1,0,0,0,922,923,1,0,0,0,923,924,1,0,
-        0,0,924,925,5,34,0,0,925,53,1,0,0,0,926,928,8,3,0,0,927,926,1,0,
-        0,0,928,929,1,0,0,0,929,927,1,0,0,0,929,930,1,0,0,0,930,55,1,0,0,
-        0,931,932,5,77,0,0,932,933,5,97,0,0,933,934,5,99,0,0,934,935,5,79,
-        0,0,935,957,5,83,0,0,936,937,5,76,0,0,937,938,5,105,0,0,938,939,
-        5,110,0,0,939,940,5,117,0,0,940,957,5,120,0,0,941,942,5,69,0,0,942,
-        943,5,76,0,0,943,944,5,73,0,0,944,945,5,76,0,0,945,957,5,79,0,0,
-        946,947,5,87,0,0,947,948,5,105,0,0,948,949,5,110,0,0,949,950,5,100,
-        0,0,950,951,5,111,0,0,951,952,5,119,0,0,952,957,5,115,0,0,953,954,
-        5,88,0,0,954,955,5,79,0,0,955,957,5,77,0,0,956,931,1,0,0,0,956,936,
-        1,0,0,0,956,941,1,0,0,0,956,946,1,0,0,0,956,953,1,0,0,0,957,958,
-        1,0,0,0,958,959,6,27,2,0,959,57,1,0,0,0,960,961,5,111,0,0,961,966,
-        5,110,0,0,962,963,5,111,0,0,963,964,5,102,0,0,964,966,5,102,0,0,
-        965,960,1,0,0,0,965,962,1,0,0,0,966,967,1,0,0,0,967,968,6,28,2,0,
-        968,59,1,0,0,0,18,0,1,63,68,75,85,89,750,755,759,765,901,908,914,
-        922,929,956,965,3,6,0,0,5,1,0,4,0,0
+        1,27,1,27,1,27,1,27,1,27,1,27,3,27,995,8,27,1,27,1,27,1,28,1,28,
+        1,28,1,28,1,28,3,28,1004,8,28,1,28,1,28,0,0,29,2,1,4,2,6,3,8,4,10,
+        5,12,6,14,0,16,0,18,7,20,8,22,9,24,10,26,11,28,12,30,13,32,14,34,
+        15,36,16,38,17,40,18,42,19,44,20,46,0,48,21,50,0,52,0,54,0,56,22,
+        58,23,2,0,1,4,2,0,9,9,32,32,1,0,10,10,3,0,48,57,65,70,97,102,2,0,
+        9,10,32,32,1067,0,2,1,0,0,0,0,4,1,0,0,0,0,6,1,0,0,0,0,8,1,0,0,0,
+        0,10,1,0,0,0,0,12,1,0,0,0,0,18,1,0,0,0,0,20,1,0,0,0,0,22,1,0,0,0,
+        0,24,1,0,0,0,0,26,1,0,0,0,0,28,1,0,0,0,0,30,1,0,0,0,0,32,1,0,0,0,
+        0,34,1,0,0,0,0,36,1,0,0,0,0,38,1,0,0,0,0,40,1,0,0,0,0,42,1,0,0,0,
+        0,44,1,0,0,0,0,48,1,0,0,0,1,56,1,0,0,0,1,58,1,0,0,0,2,61,1,0,0,0,
+        4,68,1,0,0,0,6,75,1,0,0,0,8,81,1,0,0,0,10,788,1,0,0,0,12,803,1,0,
+        0,0,14,805,1,0,0,0,16,815,1,0,0,0,18,828,1,0,0,0,20,835,1,0,0,0,
+        22,842,1,0,0,0,24,849,1,0,0,0,26,854,1,0,0,0,28,865,1,0,0,0,30,878,
+        1,0,0,0,32,886,1,0,0,0,34,898,1,0,0,0,36,915,1,0,0,0,38,924,1,0,
+        0,0,40,932,1,0,0,0,42,934,1,0,0,0,44,937,1,0,0,0,46,941,1,0,0,0,
+        48,946,1,0,0,0,50,948,1,0,0,0,52,956,1,0,0,0,54,965,1,0,0,0,56,994,
+        1,0,0,0,58,1003,1,0,0,0,60,62,7,0,0,0,61,60,1,0,0,0,62,63,1,0,0,
+        0,63,61,1,0,0,0,63,64,1,0,0,0,64,65,1,0,0,0,65,66,6,0,0,0,66,3,1,
+        0,0,0,67,69,5,13,0,0,68,67,1,0,0,0,68,69,1,0,0,0,69,70,1,0,0,0,70,
+        71,5,10,0,0,71,72,1,0,0,0,72,73,6,1,0,0,73,5,1,0,0,0,74,76,3,2,0,
+        0,75,74,1,0,0,0,75,76,1,0,0,0,76,77,1,0,0,0,77,78,3,4,1,0,78,79,
+        1,0,0,0,79,80,6,2,0,0,80,7,1,0,0,0,81,85,5,35,0,0,82,84,8,1,0,0,
+        83,82,1,0,0,0,84,87,1,0,0,0,85,83,1,0,0,0,85,86,1,0,0,0,86,89,1,
+        0,0,0,87,85,1,0,0,0,88,90,3,4,1,0,89,88,1,0,0,0,89,90,1,0,0,0,90,
+        91,1,0,0,0,91,92,6,3,0,0,92,9,1,0,0,0,93,94,5,97,0,0,94,95,5,108,
+        0,0,95,96,5,115,0,0,96,97,5,111,0,0,97,98,5,95,0,0,98,99,5,115,0,
+        0,99,100,5,99,0,0,100,101,5,97,0,0,101,102,5,110,0,0,102,103,5,95,
+        0,0,103,104,5,100,0,0,104,105,5,105,0,0,105,106,5,114,0,0,106,789,
+        5,115,0,0,107,108,5,98,0,0,108,109,5,97,0,0,109,110,5,110,0,0,110,
+        111,5,110,0,0,111,112,5,101,0,0,112,789,5,114,0,0,113,114,5,98,0,
+        0,114,115,5,97,0,0,115,116,5,110,0,0,116,117,5,110,0,0,117,118,5,
+        101,0,0,118,119,5,114,0,0,119,120,5,95,0,0,120,121,5,115,0,0,121,
+        122,5,99,0,0,122,123,5,97,0,0,123,124,5,108,0,0,124,789,5,101,0,
+        0,125,126,5,98,0,0,126,127,5,105,0,0,127,128,5,103,0,0,128,129,5,
+        95,0,0,129,130,5,105,0,0,130,131,5,99,0,0,131,132,5,111,0,0,132,
+        133,5,110,0,0,133,134,5,95,0,0,134,135,5,115,0,0,135,136,5,105,0,
+        0,136,137,5,122,0,0,137,789,5,101,0,0,138,139,5,99,0,0,139,140,5,
+        115,0,0,140,141,5,114,0,0,141,142,5,95,0,0,142,143,5,118,0,0,143,
+        144,5,97,0,0,144,145,5,108,0,0,145,146,5,117,0,0,146,147,5,101,0,
+        0,147,789,5,115,0,0,148,149,5,100,0,0,149,150,5,101,0,0,150,151,
+        5,102,0,0,151,152,5,97,0,0,152,153,5,117,0,0,153,154,5,108,0,0,154,
+        155,5,116,0,0,155,156,5,95,0,0,156,157,5,115,0,0,157,158,5,101,0,
+        0,158,159,5,108,0,0,159,160,5,101,0,0,160,161,5,99,0,0,161,162,5,
+        116,0,0,162,163,5,105,0,0,163,164,5,111,0,0,164,789,5,110,0,0,165,
+        166,5,100,0,0,166,167,5,111,0,0,167,168,5,110,0,0,168,169,5,39,0,
+        0,169,170,5,116,0,0,170,171,5,95,0,0,171,172,5,115,0,0,172,173,5,
+        99,0,0,173,174,5,97,0,0,174,175,5,110,0,0,175,176,5,95,0,0,176,177,
+        5,100,0,0,177,178,5,105,0,0,178,179,5,114,0,0,179,789,5,115,0,0,
+        180,181,5,100,0,0,181,182,5,111,0,0,182,183,5,110,0,0,183,184,5,
+        39,0,0,184,185,5,116,0,0,185,186,5,95,0,0,186,187,5,115,0,0,187,
+        188,5,99,0,0,188,189,5,97,0,0,189,190,5,110,0,0,190,191,5,95,0,0,
+        191,192,5,102,0,0,192,193,5,105,0,0,193,194,5,108,0,0,194,195,5,
+        101,0,0,195,789,5,115,0,0,196,197,5,100,0,0,197,198,5,111,0,0,198,
+        199,5,110,0,0,199,200,5,39,0,0,200,201,5,116,0,0,201,202,5,95,0,
+        0,202,203,5,115,0,0,203,204,5,99,0,0,204,205,5,97,0,0,205,206,5,
+        110,0,0,206,207,5,95,0,0,207,208,5,102,0,0,208,209,5,105,0,0,209,
+        210,5,114,0,0,210,211,5,109,0,0,211,212,5,119,0,0,212,213,5,97,0,
+        0,213,214,5,114,0,0,214,789,5,101,0,0,215,216,5,100,0,0,216,217,
+        5,111,0,0,217,218,5,110,0,0,218,219,5,39,0,0,219,220,5,116,0,0,220,
+        221,5,95,0,0,221,222,5,115,0,0,222,223,5,99,0,0,223,224,5,97,0,0,
+        224,225,5,110,0,0,225,226,5,95,0,0,226,227,5,116,0,0,227,228,5,111,
+        0,0,228,229,5,111,0,0,229,230,5,108,0,0,230,789,5,115,0,0,231,232,
+        5,100,0,0,232,233,5,111,0,0,233,234,5,110,0,0,234,235,5,39,0,0,235,
+        236,5,116,0,0,236,237,5,95,0,0,237,238,5,115,0,0,238,239,5,99,0,
+        0,239,240,5,97,0,0,240,241,5,110,0,0,241,242,5,95,0,0,242,243,5,
+        118,0,0,243,244,5,111,0,0,244,245,5,108,0,0,245,246,5,117,0,0,246,
+        247,5,109,0,0,247,248,5,101,0,0,248,789,5,115,0,0,249,250,5,100,
+        0,0,250,251,5,111,0,0,251,252,5,110,0,0,252,253,5,116,0,0,253,254,
+        5,95,0,0,254,255,5,115,0,0,255,256,5,99,0,0,256,257,5,97,0,0,257,
+        258,5,110,0,0,258,259,5,95,0,0,259,260,5,100,0,0,260,261,5,105,0,
+        0,261,262,5,114,0,0,262,789,5,115,0,0,263,264,5,100,0,0,264,265,
+        5,111,0,0,265,266,5,110,0,0,266,267,5,116,0,0,267,268,5,95,0,0,268,
+        269,5,115,0,0,269,270,5,99,0,0,270,271,5,97,0,0,271,272,5,110,0,
+        0,272,273,5,95,0,0,273,274,5,102,0,0,274,275,5,105,0,0,275,276,5,
+        108,0,0,276,277,5,101,0,0,277,789,5,115,0,0,278,279,5,100,0,0,279,
+        280,5,111,0,0,280,281,5,110,0,0,281,282,5,116,0,0,282,283,5,95,0,
+        0,283,284,5,115,0,0,284,285,5,99,0,0,285,286,5,97,0,0,286,287,5,
+        110,0,0,287,288,5,95,0,0,288,289,5,102,0,0,289,290,5,105,0,0,290,
+        291,5,114,0,0,291,292,5,109,0,0,292,293,5,119,0,0,293,294,5,97,0,
+        0,294,295,5,114,0,0,295,789,5,101,0,0,296,297,5,100,0,0,297,298,
+        5,111,0,0,298,299,5,110,0,0,299,300,5,116,0,0,300,301,5,95,0,0,301,
+        302,5,115,0,0,302,303,5,99,0,0,303,304,5,97,0,0,304,305,5,110,0,
+        0,305,306,5,95,0,0,306,307,5,116,0,0,307,308,5,111,0,0,308,309,5,
+        111,0,0,309,310,5,108,0,0,310,789,5,115,0,0,311,312,5,100,0,0,312,
+        313,5,111,0,0,313,314,5,110,0,0,314,315,5,116,0,0,315,316,5,95,0,
+        0,316,317,5,115,0,0,317,318,5,99,0,0,318,319,5,97,0,0,319,320,5,
+        110,0,0,320,321,5,95,0,0,321,322,5,118,0,0,322,323,5,111,0,0,323,
+        324,5,108,0,0,324,325,5,117,0,0,325,326,5,109,0,0,326,327,5,101,
+        0,0,327,789,5,115,0,0,328,329,5,101,0,0,329,330,5,110,0,0,330,331,
+        5,97,0,0,331,332,5,98,0,0,332,333,5,108,0,0,333,334,5,101,0,0,334,
+        335,5,95,0,0,335,336,5,97,0,0,336,337,5,110,0,0,337,338,5,100,0,
+        0,338,339,5,95,0,0,339,340,5,108,0,0,340,341,5,111,0,0,341,342,5,
+        99,0,0,342,343,5,107,0,0,343,344,5,95,0,0,344,345,5,118,0,0,345,
+        346,5,109,0,0,346,789,5,120,0,0,347,348,5,101,0,0,348,349,5,110,
+        0,0,349,350,5,97,0,0,350,351,5,98,0,0,351,352,5,108,0,0,352,353,
+        5,101,0,0,353,354,5,95,0,0,354,355,5,109,0,0,355,356,5,111,0,0,356,
+        357,5,117,0,0,357,358,5,115,0,0,358,789,5,101,0,0,359,360,5,101,
+        0,0,360,361,5,110,0,0,361,362,5,97,0,0,362,363,5,98,0,0,363,364,
+        5,108,0,0,364,365,5,101,0,0,365,366,5,95,0,0,366,367,5,116,0,0,367,
+        368,5,111,0,0,368,369,5,117,0,0,369,370,5,99,0,0,370,789,5,104,0,
+        0,371,372,5,101,0,0,372,373,5,120,0,0,373,374,5,116,0,0,374,375,
+        5,114,0,0,375,376,5,97,0,0,376,377,5,95,0,0,377,378,5,107,0,0,378,
+        379,5,101,0,0,379,380,5,114,0,0,380,381,5,110,0,0,381,382,5,101,
+        0,0,382,383,5,108,0,0,383,384,5,95,0,0,384,385,5,118,0,0,385,386,
+        5,101,0,0,386,387,5,114,0,0,387,388,5,115,0,0,388,389,5,105,0,0,
+        389,390,5,111,0,0,390,391,5,110,0,0,391,392,5,95,0,0,392,393,5,115,
+        0,0,393,394,5,116,0,0,394,395,5,114,0,0,395,396,5,105,0,0,396,397,
+        5,110,0,0,397,398,5,103,0,0,398,789,5,115,0,0,399,400,5,102,0,0,
+        400,401,5,111,0,0,401,402,5,108,0,0,402,403,5,100,0,0,403,404,5,
+        95,0,0,404,405,5,108,0,0,405,406,5,105,0,0,406,407,5,110,0,0,407,
+        408,5,117,0,0,408,409,5,120,0,0,409,410,5,95,0,0,410,411,5,107,0,
+        0,411,412,5,101,0,0,412,413,5,114,0,0,413,414,5,110,0,0,414,415,
+        5,101,0,0,415,416,5,108,0,0,416,789,5,115,0,0,417,418,5,102,0,0,
+        418,419,5,111,0,0,419,420,5,108,0,0,420,421,5,108,0,0,421,422,5,
+        111,0,0,422,423,5,119,0,0,423,424,5,95,0,0,424,425,5,115,0,0,425,
+        426,5,121,0,0,426,427,5,109,0,0,427,428,5,108,0,0,428,429,5,105,
+        0,0,429,430,5,110,0,0,430,431,5,107,0,0,431,789,5,115,0,0,432,433,
+        5,102,0,0,433,434,5,111,0,0,434,435,5,110,0,0,435,789,5,116,0,0,
+        436,437,5,104,0,0,437,438,5,105,0,0,438,439,5,100,0,0,439,440,5,
+        101,0,0,440,441,5,117,0,0,441,789,5,105,0,0,442,443,5,105,0,0,443,
+        444,5,99,0,0,444,445,5,111,0,0,445,446,5,110,0,0,446,447,5,115,0,
+        0,447,448,5,95,0,0,448,449,5,100,0,0,449,450,5,105,0,0,450,789,5,
+        114,0,0,451,452,5,108,0,0,452,453,5,111,0,0,453,454,5,103,0,0,454,
+        455,5,95,0,0,455,456,5,108,0,0,456,457,5,101,0,0,457,458,5,118,0,
+        0,458,459,5,101,0,0,459,789,5,108,0,0,460,461,5,109,0,0,461,462,
+        5,97,0,0,462,463,5,120,0,0,463,464,5,95,0,0,464,465,5,116,0,0,465,
+        466,5,97,0,0,466,467,5,103,0,0,467,789,5,115,0,0,468,469,5,109,0,
+        0,469,470,5,111,0,0,470,471,5,117,0,0,471,472,5,115,0,0,472,473,
+        5,101,0,0,473,474,5,95,0,0,474,475,5,115,0,0,475,476,5,105,0,0,476,
+        477,5,122,0,0,477,789,5,101,0,0,478,479,5,109,0,0,479,480,5,111,
+        0,0,480,481,5,117,0,0,481,482,5,115,0,0,482,483,5,101,0,0,483,484,
+        5,95,0,0,484,485,5,115,0,0,485,486,5,112,0,0,486,487,5,101,0,0,487,
+        488,5,101,0,0,488,789,5,100,0,0,489,490,5,114,0,0,490,491,5,101,
+        0,0,491,492,5,115,0,0,492,493,5,111,0,0,493,494,5,108,0,0,494,495,
+        5,117,0,0,495,496,5,116,0,0,496,497,5,105,0,0,497,498,5,111,0,0,
+        498,789,5,110,0,0,499,500,5,115,0,0,500,501,5,99,0,0,501,502,5,97,
+        0,0,502,503,5,110,0,0,503,504,5,95,0,0,504,505,5,97,0,0,505,506,
+        5,108,0,0,506,507,5,108,0,0,507,508,5,95,0,0,508,509,5,108,0,0,509,
+        510,5,105,0,0,510,511,5,110,0,0,511,512,5,117,0,0,512,513,5,120,
+        0,0,513,514,5,95,0,0,514,515,5,107,0,0,515,516,5,101,0,0,516,517,
+        5,114,0,0,517,518,5,110,0,0,518,519,5,101,0,0,519,520,5,108,0,0,
+        520,789,5,115,0,0,521,522,5,115,0,0,522,523,5,99,0,0,523,524,5,97,
+        0,0,524,525,5,110,0,0,525,526,5,95,0,0,526,527,5,100,0,0,527,528,
+        5,101,0,0,528,529,5,108,0,0,529,530,5,97,0,0,530,789,5,121,0,0,531,
+        532,5,115,0,0,532,533,5,99,0,0,533,534,5,97,0,0,534,535,5,110,0,
+        0,535,536,5,95,0,0,536,537,5,100,0,0,537,538,5,114,0,0,538,539,5,
+        105,0,0,539,540,5,118,0,0,540,541,5,101,0,0,541,542,5,114,0,0,542,
+        543,5,95,0,0,543,544,5,100,0,0,544,545,5,105,0,0,545,546,5,114,0,
+        0,546,789,5,115,0,0,547,548,5,115,0,0,548,549,5,99,0,0,549,550,5,
+        97,0,0,550,551,5,110,0,0,551,552,5,102,0,0,552,553,5,111,0,0,553,
+        789,5,114,0,0,554,555,5,115,0,0,555,556,5,99,0,0,556,557,5,114,0,
+        0,557,558,5,101,0,0,558,559,5,101,0,0,559,560,5,110,0,0,560,561,
+        5,115,0,0,561,562,5,97,0,0,562,563,5,118,0,0,563,564,5,101,0,0,564,
+        789,5,114,0,0,565,566,5,115,0,0,566,567,5,101,0,0,567,568,5,108,
+        0,0,568,569,5,101,0,0,569,570,5,99,0,0,570,571,5,116,0,0,571,572,
+        5,105,0,0,572,573,5,111,0,0,573,574,5,110,0,0,574,575,5,95,0,0,575,
+        576,5,98,0,0,576,577,5,105,0,0,577,789,5,103,0,0,578,579,5,115,0,
+        0,579,580,5,101,0,0,580,581,5,108,0,0,581,582,5,101,0,0,582,583,
+        5,99,0,0,583,584,5,116,0,0,584,585,5,105,0,0,585,586,5,111,0,0,586,
+        587,5,110,0,0,587,588,5,95,0,0,588,589,5,115,0,0,589,590,5,109,0,
+        0,590,591,5,97,0,0,591,592,5,108,0,0,592,789,5,108,0,0,593,594,5,
+        115,0,0,594,595,5,104,0,0,595,596,5,111,0,0,596,597,5,119,0,0,597,
+        598,5,116,0,0,598,599,5,111,0,0,599,600,5,111,0,0,600,601,5,108,
+        0,0,601,789,5,115,0,0,602,603,5,115,0,0,603,604,5,104,0,0,604,605,
+        5,117,0,0,605,606,5,116,0,0,606,607,5,100,0,0,607,608,5,111,0,0,
+        608,609,5,119,0,0,609,610,5,110,0,0,610,611,5,95,0,0,611,612,5,97,
+        0,0,612,613,5,102,0,0,613,614,5,116,0,0,614,615,5,101,0,0,615,616,
+        5,114,0,0,616,617,5,95,0,0,617,618,5,116,0,0,618,619,5,105,0,0,619,
+        620,5,109,0,0,620,621,5,101,0,0,621,622,5,111,0,0,622,623,5,117,
+        0,0,623,789,5,116,0,0,624,625,5,115,0,0,625,626,5,109,0,0,626,627,
+        5,97,0,0,627,628,5,108,0,0,628,629,5,108,0,0,629,630,5,95,0,0,630,
+        631,5,105,0,0,631,632,5,99,0,0,632,633,5,111,0,0,633,634,5,110,0,
+        0,634,635,5,95,0,0,635,636,5,115,0,0,636,637,5,105,0,0,637,638,5,
+        122,0,0,638,789,5,101,0,0,639,640,5,115,0,0,640,641,5,112,0,0,641,
+        642,5,111,0,0,642,643,5,111,0,0,643,644,5,102,0,0,644,645,5,95,0,
+        0,645,646,5,111,0,0,646,647,5,115,0,0,647,648,5,120,0,0,648,649,
+        5,95,0,0,649,650,5,118,0,0,650,651,5,101,0,0,651,652,5,114,0,0,652,
+        653,5,115,0,0,653,654,5,105,0,0,654,655,5,111,0,0,655,789,5,110,
+        0,0,656,657,5,115,0,0,657,658,5,117,0,0,658,659,5,112,0,0,659,660,
+        5,112,0,0,660,661,5,111,0,0,661,662,5,114,0,0,662,663,5,116,0,0,
+        663,664,5,95,0,0,664,665,5,103,0,0,665,666,5,122,0,0,666,667,5,105,
+        0,0,667,668,5,112,0,0,668,669,5,112,0,0,669,670,5,101,0,0,670,671,
+        5,100,0,0,671,672,5,95,0,0,672,673,5,108,0,0,673,674,5,111,0,0,674,
+        675,5,97,0,0,675,676,5,100,0,0,676,677,5,101,0,0,677,678,5,114,0,
+        0,678,789,5,115,0,0,679,680,5,116,0,0,680,681,5,101,0,0,681,682,
+        5,120,0,0,682,683,5,116,0,0,683,684,5,109,0,0,684,685,5,111,0,0,
+        685,686,5,100,0,0,686,789,5,101,0,0,687,688,5,116,0,0,688,689,5,
+        101,0,0,689,690,5,120,0,0,690,691,5,116,0,0,691,692,5,111,0,0,692,
+        693,5,110,0,0,693,694,5,108,0,0,694,789,5,121,0,0,695,696,5,116,
+        0,0,696,697,5,105,0,0,697,698,5,109,0,0,698,699,5,101,0,0,699,700,
+        5,111,0,0,700,701,5,117,0,0,701,789,5,116,0,0,702,703,5,117,0,0,
+        703,704,5,101,0,0,704,705,5,102,0,0,705,706,5,105,0,0,706,707,5,
+        95,0,0,707,708,5,100,0,0,708,709,5,101,0,0,709,710,5,101,0,0,710,
+        711,5,112,0,0,711,712,5,95,0,0,712,713,5,108,0,0,713,714,5,101,0,
+        0,714,715,5,103,0,0,715,716,5,97,0,0,716,717,5,99,0,0,717,718,5,
+        121,0,0,718,719,5,95,0,0,719,720,5,115,0,0,720,721,5,99,0,0,721,
+        722,5,97,0,0,722,789,5,110,0,0,723,724,5,117,0,0,724,725,5,115,0,
+        0,725,726,5,101,0,0,726,727,5,95,0,0,727,728,5,103,0,0,728,729,5,
+        114,0,0,729,730,5,97,0,0,730,731,5,112,0,0,731,732,5,104,0,0,732,
+        733,5,105,0,0,733,734,5,99,0,0,734,735,5,115,0,0,735,736,5,95,0,
+        0,736,737,5,102,0,0,737,738,5,111,0,0,738,789,5,114,0,0,739,740,
+        5,117,0,0,740,741,5,115,0,0,741,742,5,101,0,0,742,743,5,95,0,0,743,
+        744,5,110,0,0,744,745,5,118,0,0,745,746,5,114,0,0,746,747,5,97,0,
+        0,747,789,5,109,0,0,748,749,5,119,0,0,749,750,5,105,0,0,750,751,
+        5,110,0,0,751,752,5,100,0,0,752,753,5,111,0,0,753,754,5,119,0,0,
+        754,755,5,115,0,0,755,756,5,95,0,0,756,757,5,114,0,0,757,758,5,101,
+        0,0,758,759,5,99,0,0,759,760,5,111,0,0,760,761,5,118,0,0,761,762,
+        5,101,0,0,762,763,5,114,0,0,763,764,5,121,0,0,764,765,5,95,0,0,765,
+        766,5,102,0,0,766,767,5,105,0,0,767,768,5,108,0,0,768,769,5,101,
+        0,0,769,789,5,115,0,0,770,771,5,119,0,0,771,772,5,114,0,0,772,773,
+        5,105,0,0,773,774,5,116,0,0,774,775,5,101,0,0,775,776,5,95,0,0,776,
+        777,5,115,0,0,777,778,5,121,0,0,778,779,5,115,0,0,779,780,5,116,
+        0,0,780,781,5,101,0,0,781,782,5,109,0,0,782,783,5,100,0,0,783,784,
+        5,95,0,0,784,785,5,118,0,0,785,786,5,97,0,0,786,787,5,114,0,0,787,
+        789,5,115,0,0,788,93,1,0,0,0,788,107,1,0,0,0,788,113,1,0,0,0,788,
+        125,1,0,0,0,788,138,1,0,0,0,788,148,1,0,0,0,788,165,1,0,0,0,788,
+        180,1,0,0,0,788,196,1,0,0,0,788,215,1,0,0,0,788,231,1,0,0,0,788,
+        249,1,0,0,0,788,263,1,0,0,0,788,278,1,0,0,0,788,296,1,0,0,0,788,
+        311,1,0,0,0,788,328,1,0,0,0,788,347,1,0,0,0,788,359,1,0,0,0,788,
+        371,1,0,0,0,788,399,1,0,0,0,788,417,1,0,0,0,788,432,1,0,0,0,788,
+        436,1,0,0,0,788,442,1,0,0,0,788,451,1,0,0,0,788,460,1,0,0,0,788,
+        468,1,0,0,0,788,478,1,0,0,0,788,489,1,0,0,0,788,499,1,0,0,0,788,
+        521,1,0,0,0,788,531,1,0,0,0,788,547,1,0,0,0,788,554,1,0,0,0,788,
+        565,1,0,0,0,788,578,1,0,0,0,788,593,1,0,0,0,788,602,1,0,0,0,788,
+        624,1,0,0,0,788,639,1,0,0,0,788,656,1,0,0,0,788,679,1,0,0,0,788,
+        687,1,0,0,0,788,695,1,0,0,0,788,702,1,0,0,0,788,723,1,0,0,0,788,
+        739,1,0,0,0,788,748,1,0,0,0,788,770,1,0,0,0,789,793,1,0,0,0,790,
+        792,8,1,0,0,791,790,1,0,0,0,792,795,1,0,0,0,793,791,1,0,0,0,793,
+        794,1,0,0,0,794,797,1,0,0,0,795,793,1,0,0,0,796,798,3,4,1,0,797,
+        796,1,0,0,0,797,798,1,0,0,0,798,799,1,0,0,0,799,800,6,4,0,0,800,
+        11,1,0,0,0,801,804,3,14,6,0,802,804,3,16,7,0,803,801,1,0,0,0,803,
+        802,1,0,0,0,804,13,1,0,0,0,805,806,5,109,0,0,806,807,5,101,0,0,807,
+        808,5,110,0,0,808,809,5,117,0,0,809,810,5,101,0,0,810,811,5,110,
+        0,0,811,812,5,116,0,0,812,813,5,114,0,0,813,814,5,121,0,0,814,15,
+        1,0,0,0,815,816,5,115,0,0,816,817,5,117,0,0,817,818,5,98,0,0,818,
+        819,5,109,0,0,819,820,5,101,0,0,820,821,5,110,0,0,821,822,5,117,
+        0,0,822,823,5,101,0,0,823,824,5,110,0,0,824,825,5,116,0,0,825,826,
+        5,114,0,0,826,827,5,121,0,0,827,17,1,0,0,0,828,829,5,118,0,0,829,
+        830,5,111,0,0,830,831,5,108,0,0,831,832,5,117,0,0,832,833,5,109,
+        0,0,833,834,5,101,0,0,834,19,1,0,0,0,835,836,5,108,0,0,836,837,5,
+        111,0,0,837,838,5,97,0,0,838,839,5,100,0,0,839,840,5,101,0,0,840,
+        841,5,114,0,0,841,21,1,0,0,0,842,843,5,105,0,0,843,844,5,110,0,0,
+        844,845,5,105,0,0,845,846,5,116,0,0,846,847,5,114,0,0,847,848,5,
+        100,0,0,848,23,1,0,0,0,849,850,5,105,0,0,850,851,5,99,0,0,851,852,
+        5,111,0,0,852,853,5,110,0,0,853,25,1,0,0,0,854,855,5,111,0,0,855,
+        856,5,115,0,0,856,857,5,116,0,0,857,858,5,121,0,0,858,859,5,112,
+        0,0,859,860,5,101,0,0,860,861,1,0,0,0,861,862,3,2,0,0,862,863,1,
+        0,0,0,863,864,6,12,1,0,864,27,1,0,0,0,865,866,5,103,0,0,866,867,
+        5,114,0,0,867,868,5,97,0,0,868,869,5,112,0,0,869,870,5,104,0,0,870,
+        871,5,105,0,0,871,872,5,99,0,0,872,873,5,115,0,0,873,874,1,0,0,0,
+        874,875,3,2,0,0,875,876,1,0,0,0,876,877,6,13,1,0,877,29,1,0,0,0,
+        878,879,5,111,0,0,879,880,5,112,0,0,880,881,5,116,0,0,881,882,5,
+        105,0,0,882,883,5,111,0,0,883,884,5,110,0,0,884,885,5,115,0,0,885,
+        31,1,0,0,0,886,887,5,97,0,0,887,888,5,100,0,0,888,889,5,100,0,0,
+        889,890,5,95,0,0,890,891,5,111,0,0,891,892,5,112,0,0,892,893,5,116,
+        0,0,893,894,5,105,0,0,894,895,5,111,0,0,895,896,5,110,0,0,896,897,
+        5,115,0,0,897,33,1,0,0,0,898,899,5,102,0,0,899,900,5,105,0,0,900,
+        901,5,114,0,0,901,902,5,109,0,0,902,903,5,119,0,0,903,904,5,97,0,
+        0,904,905,5,114,0,0,905,906,5,101,0,0,906,907,5,95,0,0,907,908,5,
+        98,0,0,908,909,5,111,0,0,909,910,5,111,0,0,910,911,5,116,0,0,911,
+        912,5,110,0,0,912,913,5,117,0,0,913,914,5,109,0,0,914,35,1,0,0,0,
+        915,916,5,100,0,0,916,917,5,105,0,0,917,918,5,115,0,0,918,919,5,
+        97,0,0,919,920,5,98,0,0,920,921,5,108,0,0,921,922,5,101,0,0,922,
+        923,5,100,0,0,923,37,1,0,0,0,924,925,5,105,0,0,925,926,5,110,0,0,
+        926,927,5,99,0,0,927,928,5,108,0,0,928,929,5,117,0,0,929,930,5,100,
+        0,0,930,931,5,101,0,0,931,39,1,0,0,0,932,933,5,123,0,0,933,41,1,
+        0,0,0,934,935,5,125,0,0,935,43,1,0,0,0,936,938,3,46,22,0,937,936,
+        1,0,0,0,938,939,1,0,0,0,939,937,1,0,0,0,939,940,1,0,0,0,940,45,1,
+        0,0,0,941,942,7,2,0,0,942,47,1,0,0,0,943,947,3,50,24,0,944,947,3,
+        52,25,0,945,947,3,54,26,0,946,943,1,0,0,0,946,944,1,0,0,0,946,945,
+        1,0,0,0,947,49,1,0,0,0,948,950,5,39,0,0,949,951,8,1,0,0,950,949,
+        1,0,0,0,951,952,1,0,0,0,952,950,1,0,0,0,952,953,1,0,0,0,953,954,
+        1,0,0,0,954,955,5,39,0,0,955,51,1,0,0,0,956,958,5,34,0,0,957,959,
+        8,1,0,0,958,957,1,0,0,0,959,960,1,0,0,0,960,958,1,0,0,0,960,961,
+        1,0,0,0,961,962,1,0,0,0,962,963,5,34,0,0,963,53,1,0,0,0,964,966,
+        8,3,0,0,965,964,1,0,0,0,966,967,1,0,0,0,967,965,1,0,0,0,967,968,
+        1,0,0,0,968,55,1,0,0,0,969,970,5,77,0,0,970,971,5,97,0,0,971,972,
+        5,99,0,0,972,973,5,79,0,0,973,995,5,83,0,0,974,975,5,76,0,0,975,
+        976,5,105,0,0,976,977,5,110,0,0,977,978,5,117,0,0,978,995,5,120,
+        0,0,979,980,5,69,0,0,980,981,5,76,0,0,981,982,5,73,0,0,982,983,5,
+        76,0,0,983,995,5,79,0,0,984,985,5,87,0,0,985,986,5,105,0,0,986,987,
+        5,110,0,0,987,988,5,100,0,0,988,989,5,111,0,0,989,990,5,119,0,0,
+        990,995,5,115,0,0,991,992,5,88,0,0,992,993,5,79,0,0,993,995,5,77,
+        0,0,994,969,1,0,0,0,994,974,1,0,0,0,994,979,1,0,0,0,994,984,1,0,
+        0,0,994,991,1,0,0,0,995,996,1,0,0,0,996,997,6,27,2,0,997,57,1,0,
+        0,0,998,999,5,111,0,0,999,1004,5,110,0,0,1000,1001,5,111,0,0,1001,
+        1002,5,102,0,0,1002,1004,5,102,0,0,1003,998,1,0,0,0,1003,1000,1,
+        0,0,0,1004,1005,1,0,0,0,1005,1006,6,28,2,0,1006,59,1,0,0,0,18,0,
+        1,63,68,75,85,89,788,793,797,803,939,946,952,960,967,994,1003,3,
+        6,0,0,5,1,0,4,0,0
     ]
 
 class RefindConfigLexer(Lexer):
 
     atn = ATNDeserializer().deserialize(serializedATN())
 
     decisionsToDFA = [ DFA(ds, i) for i, ds in enumerate(atn.decisionToState) ]
@@ -409,13 +423,13 @@
                   "STRING", "SINGLE_QUOTED_STRING", "DOUBLE_QUOTED_STRING", 
                   "UNQUOTED_STRING", "OS_TYPE_PARAMETER", "GRAPHICS_PARAMETER" ]
 
     grammarFileName = "RefindConfigLexer.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.11.1")
+        self.checkVersion("4.12.0")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
         self._actions = None
         self._predicates = None
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/boot/antlr4/RefindConfigParser.py` & `refind-btrfs-0.6.0/src/refind_btrfs/boot/antlr4/RefindConfigParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from /home/luka/Projects/Python/refind-btrfs/src/refind_btrfs/boot/antlr4/RefindConfigParser.g4 by ANTLR 4.11.1
+# Generated from c:\Users\Luka\Projects\Python\refind-btrfs\src\refind_btrfs\boot\antlr4\RefindConfigParser.g4 by ANTLR 4.12.0
 # encoding: utf-8
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
@@ -128,15 +128,15 @@
     HEX_INTEGER=20
     STRING=21
     OS_TYPE_PARAMETER=22
     GRAPHICS_PARAMETER=23
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.11.1")
+        self.checkVersion("4.12.0")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
 
 
 
     class RefindContext(ParserRuleContext):
@@ -305,15 +305,15 @@
             _la = self._input.LA(1)
             while True:
                 self.state = 54
                 self.main_option()
                 self.state = 57 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if not (((_la) & ~0x3f) == 0 and ((1 << _la) & 114624) != 0):
+                if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 114624) != 0)):
                     break
 
             self.state = 59
             self.match(RefindConfigParser.CLOSE_BRACE)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
@@ -939,15 +939,15 @@
             _la = self._input.LA(1)
             while True:
                 self.state = 104
                 self.sub_option()
                 self.state = 107 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if not (((_la) & ~0x3f) == 0 and ((1 << _la) & 94976) != 0):
+                if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 94976) != 0)):
                     break
 
             self.state = 109
             self.match(RefindConfigParser.CLOSE_BRACE)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/boot/antlr4/RefindConfigParserVisitor.py` & `refind-btrfs-0.6.0/src/refind_btrfs/boot/antlr4/RefindConfigParserVisitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from /home/luka/Projects/Python/refind-btrfs/src/refind_btrfs/boot/antlr4/RefindConfigParser.g4 by ANTLR 4.11.1
+# Generated from c:\Users\Luka\Projects\Python\refind-btrfs\src\refind_btrfs\boot\antlr4\RefindConfigParser.g4 by ANTLR 4.12.0
 from antlr4 import *
 if __name__ is not None and "." in __name__:
     from .RefindConfigParser import RefindConfigParser
 else:
     from RefindConfigParser import RefindConfigParser
 
 # This class defines a complete generic visitor for a parse tree produced by RefindConfigParser.
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/boot/antlr4/__init__.py` & `refind-btrfs-0.6.0/src/refind_btrfs/boot/antlr4/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/boot/boot_options.py` & `refind-btrfs-0.6.0/src/refind_btrfs/boot/boot_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -19,15 +19,15 @@
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # endregion
 
 from __future__ import annotations
 
-from typing import Iterable, Optional
+from typing import Iterable, Optional, Self
 
 from more_itertools import last
 
 from refind_btrfs.common import constants
 from refind_btrfs.common.exceptions import RefindConfigError
 from refind_btrfs.device import BlockDevice, MountOptions, Subvolume
 from refind_btrfs.utility.helpers import (
@@ -192,15 +192,15 @@
                             ),
                         ),
                     )
                     for initrd_option in initrd_options
                 ]
 
     @classmethod
-    def merge(cls, all_boot_options: Iterable[BootOptions]) -> BootOptions:
+    def merge(cls, all_boot_options: Iterable[BootOptions]) -> Self:
         all_boot_options_str = [
             strip_quotes(str(boot_options)) for boot_options in all_boot_options
         ]
 
         return cls(constants.SPACE.join(all_boot_options_str).strip())
 
     @property
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/boot/boot_stanza.py` & `refind-btrfs-0.6.0/src/refind_btrfs/boot/boot_stanza.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -24,15 +24,15 @@
 from __future__ import annotations
 
 import inspect
 import re
 from collections import defaultdict
 from functools import cached_property, singledispatchmethod
 from itertools import chain
-from typing import Any, DefaultDict, Iterable, Iterator, Optional, Set
+from typing import Any, DefaultDict, Iterable, Iterator, Optional, Self, Set
 
 from more_itertools import always_iterable, last
 
 from refind_btrfs.common import BootFilesCheckResult, constants
 from refind_btrfs.common.enums import (
     BootFilePathSource,
     BootStanzaIconGenerationMode,
@@ -170,15 +170,15 @@
 
         result.append(f"{main_indent}}}")
 
         return constants.NEWLINE.join(result)
 
     def with_boot_files_check_result(
         self, subvolume: Subvolume, include_sub_menus: bool
-    ) -> BootStanza:
+    ) -> Self:
         normalized_name = self.normalized_name
         all_boot_file_paths = self.all_boot_file_paths
         logical_path = subvolume.logical_path
         matched_boot_files: list[str] = []
         unmatched_boot_files: list[str] = []
         sources = [BootFilePathSource.BOOT_STANZA]
 
@@ -199,15 +199,15 @@
 
         self._boot_files_check_result = BootFilesCheckResult(
             normalized_name, logical_path, matched_boot_files, unmatched_boot_files
         )
 
         return self
 
-    def with_sub_menus(self, sub_menus: Iterable[SubMenu]) -> BootStanza:
+    def with_sub_menus(self, sub_menus: Iterable[SubMenu]) -> Self:
         self._sub_menus = list(sub_menus)
 
         return self
 
     @singledispatchmethod
     def is_matched_with(self, argument: Any) -> bool:
         frame = none_throws(inspect.currentframe())
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/boot/file_refind_config_provider.py` & `refind-btrfs-0.6.0/src/refind_btrfs/boot/file_refind_config_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -266,23 +266,21 @@
                     config_file_path.parent, includes
                 )
 
                 current_refind_config = (
                     RefindConfig(config_file_path)
                     .with_boot_stanzas(boot_stanzas)
                     .with_included_configs(included_configs)
-                    .with_initialization_type(
-                        ConfigInitializationType.PARSED, RefindConfig
-                    )
+                    .with_initialization_type(ConfigInitializationType.PARSED)
                 )
 
                 persistence_provider.save_refind_config(current_refind_config)
         elif current_refind_config is None:
             current_refind_config = persisted_refind_config.with_initialization_type(
-                ConfigInitializationType.PERSISTED, RefindConfig
+                ConfigInitializationType.PERSISTED
             )
 
             if current_refind_config.has_included_configs():
                 current_included_configs = none_throws(
                     current_refind_config.included_configs
                 )
                 actual_included_configs = [
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/boot/migrations/__init__.py` & `refind-btrfs-0.6.0/src/refind_btrfs/service/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -17,8 +17,10 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # endregion
 
-from .migration import Migration
+from .snapshot_event_handler import SnapshotEventHandler
+from .snapshot_observer import SnapshotObserver
+from .watchdog_runner import WatchdogRunner
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/boot/migrations/icon_migration_strategies.py` & `refind-btrfs-0.6.0/src/refind_btrfs/boot/migrations/icon_migration_strategies.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/boot/migrations/main_migration_strategies.py` & `refind-btrfs-0.6.0/src/refind_btrfs/boot/migrations/main_migration_strategies.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/boot/migrations/migration.py` & `refind-btrfs-0.6.0/src/refind_btrfs/boot/migrations/migration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/boot/migrations/state.py` & `refind-btrfs-0.6.0/src/refind_btrfs/boot/migrations/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/boot/refind_config.py` & `refind-btrfs-0.6.0/src/refind_btrfs/boot/refind_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -22,15 +22,15 @@
 # endregion
 
 from __future__ import annotations
 
 from copy import copy
 from itertools import chain
 from pathlib import Path
-from typing import Collection, Iterable, Iterator, Optional
+from typing import Collection, Iterable, Iterator, Optional, Self
 
 from more_itertools import always_iterable
 
 from refind_btrfs.common import BootStanzaGeneration, constants
 from refind_btrfs.common.abc import BaseConfig
 from refind_btrfs.common.abc.factories import BaseIconCommandFactory
 from refind_btrfs.common.enums import ConfigInitializationType
@@ -49,22 +49,20 @@
 class RefindConfig(BaseConfig):
     def __init__(self, file_path: Path) -> None:
         super().__init__(file_path)
 
         self._boot_stanzas: Optional[list[BootStanza]] = None
         self._included_configs: Optional[list[RefindConfig]] = None
 
-    def with_boot_stanzas(self, boot_stanzas: Iterable[BootStanza]) -> RefindConfig:
+    def with_boot_stanzas(self, boot_stanzas: Iterable[BootStanza]) -> Self:
         self._boot_stanzas = list(boot_stanzas)
 
         return self
 
-    def with_included_configs(
-        self, include_configs: Iterable[RefindConfig]
-    ) -> RefindConfig:
+    def with_included_configs(self, include_configs: Iterable[RefindConfig]) -> Self:
         self._included_configs = list(include_configs)
 
         return self
 
     def get_boot_stanzas_matched_with(
         self, block_device: BlockDevice
     ) -> Iterator[BootStanza]:
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/boot/refind_listeners.py` & `refind-btrfs-0.6.0/src/refind_btrfs/boot/refind_listeners.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/boot/refind_visitors.py` & `refind-btrfs-0.6.0/src/refind_btrfs/boot/refind_visitors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/boot/sub_menu.py` & `refind-btrfs-0.6.0/src/refind_btrfs/boot/sub_menu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/__init__.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/abc/__init__.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/abc/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/abc/base_config.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/abc/base_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -22,21 +22,19 @@
 # endregion
 
 from __future__ import annotations
 
 from abc import ABC
 from os import stat_result
 from pathlib import Path
-from typing import Any, Optional, Type, TypeVar
+from typing import Any, Optional, Self
 
 from refind_btrfs.common.enums import ConfigInitializationType
 from refind_btrfs.utility.helpers import checked_cast, none_throws
 
-TDerived = TypeVar("TDerived")
-
 
 class BaseConfig(ABC):
     def __init__(self, file_path: Path) -> None:
         self._file_path = file_path
         self._file_stat: Optional[stat_result] = None
         self._initialization_type: Optional[ConfigInitializationType] = None
 
@@ -63,21 +61,19 @@
 
         if initialization_type_key in state:
             del state[initialization_type_key]
 
         return state
 
     def with_initialization_type(
-        self,
-        initialization_type: ConfigInitializationType,
-        derived_type: Type[TDerived],
-    ) -> TDerived:
+        self, initialization_type: ConfigInitializationType
+    ) -> Self:
         self._initialization_type = initialization_type
 
-        return checked_cast(derived_type, self)
+        return self
 
     def refresh_file_stat(self):
         file_path = self.file_path
 
         if file_path.exists():
             self._file_stat = file_path.stat()
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/abc/base_runner.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/abc/base_runner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/abc/commands/__init__.py` & `refind-btrfs-0.6.0/src/refind_btrfs/console/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -17,10 +17,8 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # endregion
 
-from .device_command import DeviceCommand
-from .icon_command import IconCommand
-from .subvolume_command import SubvolumeCommand
+from .cli_runner import CLIRunner
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/abc/commands/device_command.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/abc/commands/device_command.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/abc/commands/icon_command.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/abc/commands/icon_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/abc/commands/subvolume_command.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/abc/commands/subvolume_command.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+# region Licensing
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/abc/factories/__init__.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/abc/factories/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/abc/factories/base_device_command_factory.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/abc/factories/base_device_command_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/abc/factories/base_icon_command_factory.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/abc/factories/base_icon_command_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/abc/factories/base_logger_factory.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/abc/factories/base_logger_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/abc/factories/base_subvolume_command_factory.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/abc/factories/base_subvolume_command_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/abc/providers/__init__.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/abc/providers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/abc/providers/base_package_config_provider.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/checkable_observer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -17,20 +17,25 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # endregion
 
-from __future__ import annotations
+from typing import Optional
 
-from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING
+from watchdog.observers import Observer
+from watchdog.observers.api import DEFAULT_OBSERVER_TIMEOUT
 
-if TYPE_CHECKING:
-    from refind_btrfs.common import PackageConfig
 
+class CheckableObserver(Observer):
+    def __init__(self):
+        super().__init__(timeout=DEFAULT_OBSERVER_TIMEOUT)
 
-class BasePackageConfigProvider(ABC):
-    @abstractmethod
-    def get_config(self) -> PackageConfig:
-        pass
+        self._exception: Optional[Exception] = None
+
+    # pylint: disable=raising-bad-type
+    def check(self) -> None:
+        exception = self._exception
+
+        if exception is not None:
+            raise exception
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/abc/providers/base_persistence_provider.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/abc/providers/base_persistence_provider.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/abc/providers/base_refind_config_provider.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/abc/providers/base_refind_config_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/boot_files_check_result.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/boot_files_check_result.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/checkable_observer.py` & `refind-btrfs-0.6.0/src/refind_btrfs/service/snapshot_observer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -17,25 +17,39 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # endregion
 
-from typing import Optional
+import queue
 
-from watchdog.observers import Observer
-from watchdog.observers.api import DEFAULT_OBSERVER_TIMEOUT
+from injector import inject
 
-
-class CheckableObserver(Observer):
-    def __init__(self):
-        super().__init__(timeout=DEFAULT_OBSERVER_TIMEOUT)
-
-        self._exception: Optional[Exception] = None
-
-    # pylint: disable=raising-bad-type
-    def check(self) -> None:
-        exception = self._exception
-
-        if exception is not None:
-            raise exception
+from refind_btrfs.common import CheckableObserver, constants
+from refind_btrfs.common.abc.factories import BaseLoggerFactory
+from refind_btrfs.common.exceptions import SnapshotMountedAsRootError
+
+
+class SnapshotObserver(CheckableObserver):
+    @inject
+    def __init__(self, logger_factory: BaseLoggerFactory):
+        super().__init__()
+
+        self._logger = logger_factory.logger(__name__)
+
+    def run(self) -> None:
+        logger = self._logger
+
+        while self.should_keep_running():
+            try:
+                self.dispatch_events(self.event_queue)
+            except queue.Empty:
+                continue
+            except SnapshotMountedAsRootError as e:
+                logger.warning(e.formatted_message)
+                self._exception = e
+                self.stop()
+            except Exception as e:
+                logger.exception(constants.MESSAGE_UNEXPECTED_ERROR)
+                self._exception = e
+                self.stop()
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/configurable_mixin.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/configurable_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/constants.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/enums.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/exceptions.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/common/package_config.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/package_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -21,15 +21,15 @@
 """
 # endregion
 
 from __future__ import annotations
 
 from functools import cached_property
 from pathlib import Path
-from typing import Iterable, Iterator, NamedTuple, Optional, Set
+from typing import Iterable, Iterator, NamedTuple, Optional, Self, Set
 from uuid import UUID
 
 from refind_btrfs.common import constants
 from refind_btrfs.common.abc import BaseConfig
 from refind_btrfs.common.enums import (
     BootStanzaIconGenerationMode,
     BtrfsLogoHorizontalAlignment,
@@ -82,17 +82,15 @@
 class BootStanzaGeneration(NamedTuple):
     refind_config: str
     include_paths: bool
     include_sub_menus: bool
     source_exclusion: Set[str]
     icon: Icon
 
-    def with_include_paths(
-        self, boot_device: Optional[BlockDevice]
-    ) -> BootStanzaGeneration:
+    def with_include_paths(self, boot_device: Optional[BlockDevice]) -> Self:
         include_paths = self.include_paths
 
         if include_paths:
             include_paths = boot_device is None
 
         return BootStanzaGeneration(
             self.refind_config,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/console/__init__.py` & `refind-btrfs-0.6.0/src/refind_btrfs/state_management/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -17,8 +17,9 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # endregion
 
-from .cli_runner import CLIRunner
+from .model import Model
+from .refind_btrfs_machine import RefindBtrfsMachine, States
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/console/cli_runner.py` & `refind-btrfs-0.6.0/src/refind_btrfs/console/cli_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/data/icons/btrfs_logo/inverted_large.png` & `refind-btrfs-0.6.0/src/refind_btrfs/data/icons/btrfs_logo/inverted_large.png`

 * *Files identical despite different names*

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/data/icons/btrfs_logo/inverted_medium.png` & `refind-btrfs-0.6.0/src/refind_btrfs/data/icons/btrfs_logo/inverted_medium.png`

 * *Files identical despite different names*

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/data/icons/btrfs_logo/inverted_small.png` & `refind-btrfs-0.6.0/src/refind_btrfs/data/icons/btrfs_logo/inverted_small.png`

 * *Files identical despite different names*

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/data/icons/btrfs_logo/original_large.png` & `refind-btrfs-0.6.0/src/refind_btrfs/data/icons/btrfs_logo/original_large.png`

 * *Files identical despite different names*

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/data/icons/btrfs_logo/original_medium.png` & `refind-btrfs-0.6.0/src/refind_btrfs/data/icons/btrfs_logo/original_medium.png`

 * *Files identical despite different names*

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/data/icons/btrfs_logo/original_small.png` & `refind-btrfs-0.6.0/src/refind_btrfs/data/icons/btrfs_logo/original_small.png`

 * *Files identical despite different names*

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/data/images/refind_screenshot_default.png` & `refind-btrfs-0.6.0/src/refind_btrfs/data/images/refind_screenshot_default.png`

 * *Files identical despite different names*

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/data/images/refind_screenshot_nord.png` & `refind-btrfs-0.6.0/src/refind_btrfs/data/images/refind_screenshot_nord.png`

 * *Files identical despite different names*

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/data/refind-btrfs.conf-sample` & `refind-btrfs-0.6.0/src/refind_btrfs/data/refind-btrfs.conf-sample`

 * *Files identical despite different names*

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/device/__init__.py` & `refind-btrfs-0.6.0/src/refind_btrfs/device/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/device/block_device.py` & `refind-btrfs-0.6.0/src/refind_btrfs/device/block_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -20,15 +20,15 @@
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # endregion
 
 from __future__ import annotations
 
 import re
-from typing import Iterable, Optional, Union
+from typing import Iterable, Optional, Self, Union
 
 from refind_btrfs.common.abc.factories import BaseDeviceCommandFactory
 from refind_btrfs.utility.helpers import has_items, none_throws
 
 from .partition import Partition
 from .partition_table import PartitionTable
 
@@ -42,32 +42,32 @@
 
         self._major_number = major_minor_parsed[0]
         self._minor_number = major_minor_parsed[1]
         self._physical_partition_table: Optional[PartitionTable] = None
         self._live_partition_table: Optional[PartitionTable] = None
         self._dependencies: Optional[list[BlockDevice]] = None
 
-    def with_dependencies(self, dependencies: Iterable[BlockDevice]) -> BlockDevice:
+    def with_dependencies(self, dependencies: Iterable[BlockDevice]) -> Self:
         self._dependencies = list(dependencies)
 
         return self
 
     def initialize_partition_tables_using(
         self,
-        device_comand_factory: BaseDeviceCommandFactory,
+        device_command_factory: BaseDeviceCommandFactory,
     ) -> None:
         if not self.has_physical_partition_table():
-            physical_device_command = device_comand_factory.physical_device_command()
+            physical_device_command = device_command_factory.physical_device_command()
 
             self._physical_partition_table = (
                 physical_device_command.get_partition_table_for(self)
             )
 
         if not self.has_live_partition_table():
-            live_device_command = device_comand_factory.live_device_command()
+            live_device_command = device_command_factory.live_device_command()
 
             self._live_partition_table = live_device_command.get_partition_table_for(
                 self
             )
 
     def is_matched_with(self, name: str) -> bool:
         if self.name == name:
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/device/filesystem.py` & `refind-btrfs-0.6.0/src/refind_btrfs/device/filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -20,15 +20,15 @@
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # endregion
 
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Self
 
 from refind_btrfs.common.abc.factories import BaseSubvolumeCommandFactory
 from refind_btrfs.utility.helpers import is_none_or_whitespace
 
 from .mount_options import MountOptions
 from .subvolume import Subvolume
 
@@ -40,21 +40,21 @@
         self._fs_type = fs_type
         self._mount_point = mount_point
         self._dump: Optional[int] = None
         self._fsck: Optional[int] = None
         self._mount_options: Optional[MountOptions] = None
         self._subvolume: Optional[Subvolume] = None
 
-    def with_dump_and_fsck(self, dump: int, fsck: int) -> Filesystem:
+    def with_dump_and_fsck(self, dump: int, fsck: int) -> Self:
         self._dump = dump
         self._fsck = fsck
 
         return self
 
-    def with_mount_options(self, raw_mount_options: str) -> Filesystem:
+    def with_mount_options(self, raw_mount_options: str) -> Self:
         self._mount_options = (
             MountOptions(raw_mount_options)
             if not is_none_or_whitespace(raw_mount_options)
             else None
         )
 
         return self
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/device/mount_options.py` & `refind-btrfs-0.6.0/src/refind_btrfs/device/mount_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/device/partition.py` & `refind-btrfs-0.6.0/src/refind_btrfs/device/partition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -20,15 +20,15 @@
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # endregion
 
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Self
 from uuid import UUID
 
 from refind_btrfs.common import constants
 from refind_btrfs.utility.helpers import (
     find_all_matched_files_in,
     is_none_or_whitespace,
     none_throws,
@@ -56,21 +56,21 @@
             return self.uuid == other.uuid
 
         return False
 
     def __hash__(self) -> int:
         return hash(self.uuid)
 
-    def with_part_type(self, part_type: str) -> Partition:
+    def with_part_type(self, part_type: str) -> Self:
         self._part_type_code = try_parse_int(part_type, base=16)
         self._part_type_uuid = try_parse_uuid(part_type)
 
         return self
 
-    def with_filesystem(self, filesystem: Filesystem) -> Partition:
+    def with_filesystem(self, filesystem: Filesystem) -> Self:
         self._filesystem = filesystem
 
         return self
 
     def is_esp(self, uuid: UUID) -> bool:
         filesystem = self.filesystem
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/device/partition_table.py` & `refind-btrfs-0.6.0/src/refind_btrfs/device/partition_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -22,15 +22,15 @@
 # endregion
 
 from __future__ import annotations
 
 import re
 from functools import cached_property
 from pathlib import Path
-from typing import Iterable, Optional
+from typing import Iterable, Optional, Self
 from uuid import UUID
 
 from more_itertools import only, take
 
 from refind_btrfs.common import constants
 from refind_btrfs.common.enums import FstabColumn
 from refind_btrfs.utility.helpers import has_items, is_none_or_whitespace, none_throws
@@ -55,25 +55,25 @@
             return self.uuid == other.uuid
 
         return False
 
     def __hash__(self) -> int:
         return hash(self.uuid)
 
-    def with_esp_uuid(self, esp_uuid: UUID) -> PartitionTable:
+    def with_esp_uuid(self, esp_uuid: UUID) -> Self:
         self._esp_uuid = esp_uuid
 
         return self
 
-    def with_fstab_file_path(self, fstab_file_path: Path) -> PartitionTable:
+    def with_fstab_file_path(self, fstab_file_path: Path) -> Self:
         self._fstab_file_path = fstab_file_path
 
         return self
 
-    def with_partitions(self, partitions: Iterable[Partition]) -> PartitionTable:
+    def with_partitions(self, partitions: Iterable[Partition]) -> Self:
         self._partitions = list(partitions)
 
         return self
 
     def is_matched_with(self, subvolume: Subvolume) -> bool:
         root = self.root
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/device/subvolume.py` & `refind-btrfs-0.6.0/src/refind_btrfs/device/subvolume.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -22,15 +22,15 @@
 # endregion
 
 from __future__ import annotations
 
 from copy import deepcopy
 from datetime import datetime
 from pathlib import Path
-from typing import TYPE_CHECKING, Iterable, NamedTuple, Optional, Set
+from typing import TYPE_CHECKING, Iterable, NamedTuple, Optional, Self, Set
 from uuid import UUID
 
 from more_itertools import take
 
 from refind_btrfs.common import BootFilesCheckResult, constants
 from refind_btrfs.common.abc.factories import BaseDeviceCommandFactory
 from refind_btrfs.common.enums import PathRelation
@@ -104,15 +104,15 @@
                 for subvolume in (self, other)
             ]
 
             return attributes_for_comparison[0] < attributes_for_comparison[1]
 
         return False
 
-    def with_boot_files_check_result(self, boot_stanza: BootStanza) -> Subvolume:
+    def with_boot_files_check_result(self, boot_stanza: BootStanza) -> Self:
         boot_stanza_check_result = boot_stanza.boot_files_check_result
 
         if boot_stanza_check_result is not None:
             self_filesystem_path_str = str(self.filesystem_path)
             self_logical_path = self.logical_path
             boot_stanza_name = boot_stanza_check_result.required_by_boot_stanza_name
             expected_logical_path = boot_stanza_check_result.expected_logical_path
@@ -139,20 +139,20 @@
                 self_logical_path,
                 matched_boot_files,
                 unmatched_boot_files,
             )
 
         return self
 
-    def with_snapshots(self, snapshots: Iterable[Subvolume]) -> Subvolume:
+    def with_snapshots(self, snapshots: Iterable[Subvolume]) -> Self:
         self._snapshots = set(snapshots)
 
         return self
 
-    def as_named(self) -> Subvolume:
+    def as_named(self) -> Self:
         type_prefix = "ro" if self.is_read_only else "rw"
         type_prefix += "snap" if self.is_snapshot() else "subvol"
 
         if self.is_newly_created():
             created_from = none_throws(self.created_from)
             time_created = created_from.time_created
             num_id = created_from.num_id
@@ -162,40 +162,40 @@
 
         formatted_time_created = time_created.strftime("%Y-%m-%d_%H-%M-%S")
 
         self._name = f"{type_prefix}_{formatted_time_created}_ID{num_id}"
 
         return self
 
-    def as_located_in(self, parent_directory: Path) -> Subvolume:
+    def as_located_in(self, parent_directory: Path) -> Self:
         if not self.is_named():
             raise ValueError("The '_name' attribute must be initialized!")
 
         name = none_throws(self.name)
 
         self._filesystem_path = parent_directory / name
 
         return self
 
-    def as_writable(self) -> Subvolume:
+    def as_writable(self) -> Self:
         self._is_read_only = False
 
         return self
 
-    def as_newly_created_from(self, other: Subvolume) -> Subvolume:
+    def as_newly_created_from(self, other: Subvolume) -> Self:
         self._created_from = other
 
         if other.has_static_partition_table():
             self._static_partition_table = deepcopy(
                 none_throws(other.static_partition_table)
             )
 
         return self
 
-    def to_destination(self, directory: Path) -> Subvolume:
+    def to_destination(self, directory: Path) -> Self:
         return (
             Subvolume(
                 constants.EMPTY_PATH,
                 constants.EMPTY_STR,
                 datetime.min,
                 UuidRelation(constants.EMPTY_UUID, self.uuid),
                 NumIdRelation(0, self.num_id),
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/service/__init__.py` & `refind-btrfs-0.6.0/src/refind_btrfs/boot/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -17,10 +17,11 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # endregion
 
-from .snapshot_event_handler import SnapshotEventHandler
-from .snapshot_observer import SnapshotObserver
-from .watchdog_runner import WatchdogRunner
+from .boot_options import BootOptions
+from .boot_stanza import BootStanza
+from .refind_config import RefindConfig
+from .sub_menu import SubMenu
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/service/snapshot_event_handler.py` & `refind-btrfs-0.6.0/src/refind_btrfs/service/snapshot_event_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/service/watchdog_runner.py` & `refind-btrfs-0.6.0/src/refind_btrfs/service/watchdog_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/state_management/__init__.py` & `refind-btrfs-0.6.0/src/refind_btrfs/utility/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -17,9 +17,8 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # endregion
 
-from .model import Model
-from .refind_btrfs_machine import RefindBtrfsMachine, States
+from .level_aware_formatter import LevelAwareFormatter
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/state_management/conditions.py` & `refind-btrfs-0.6.0/src/refind_btrfs/state_management/conditions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/state_management/model.py` & `refind-btrfs-0.6.0/src/refind_btrfs/state_management/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -20,15 +20,15 @@
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # endregion
 
 from __future__ import annotations
 
 from itertools import chain
-from typing import Callable, NamedTuple, Optional
+from typing import Callable, NamedTuple, Optional, Self
 
 from injector import inject
 from more_itertools import only
 
 from refind_btrfs.boot import BootStanza, RefindConfig
 from refind_btrfs.common import ConfigurableMixin
 from refind_btrfs.common.abc.factories import (
@@ -52,15 +52,15 @@
 
 class BlockDevices(NamedTuple):
     esp_device: Optional[BlockDevice]
     root_device: Optional[BlockDevice]
     boot_device: Optional[BlockDevice]
 
     @classmethod
-    def none(cls) -> BlockDevices:
+    def none(cls) -> Self:
         return cls(None, None, None)
 
 
 class PreparedSnapshots(NamedTuple):
     snapshots_for_addition: list[Subvolume]
     snapshots_for_removal: list[Subvolume]
 
@@ -93,15 +93,15 @@
         replace_item_in(matched_snapshots, current_snapshot, replacement_snapshot)
 
 
 class ProcessingResult(NamedTuple):
     bootable_snapshots: list[Subvolume]
 
     @classmethod
-    def none(cls) -> ProcessingResult:
+    def none(cls) -> Self:
         return cls([])
 
     def has_bootable_snapshots(self) -> bool:
         return has_items(self.bootable_snapshots)
 
 
 # endregion
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/state_management/refind_btrfs_machine.py` & `refind-btrfs-0.6.0/src/refind_btrfs/state_management/refind_btrfs_machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/system/__init__.py` & `refind-btrfs-0.6.0/src/refind_btrfs/system/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/system/btrfsutil_command.py` & `refind-btrfs-0.6.0/src/refind_btrfs/system/btrfsutil_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/system/command_factories.py` & `refind-btrfs-0.6.0/src/refind_btrfs/system/command_factories.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/system/findmnt_command.py` & `refind-btrfs-0.6.0/src/refind_btrfs/system/findmnt_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/system/fstab_command.py` & `refind-btrfs-0.6.0/src/refind_btrfs/system/fstab_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/system/lsblk_command.py` & `refind-btrfs-0.6.0/src/refind_btrfs/system/lsblk_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/system/pillow_command.py` & `refind-btrfs-0.6.0/src/refind_btrfs/system/pillow_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/utility/__init__.py` & `refind-btrfs-0.6.0/src/refind_btrfs/common/abc/providers/base_package_config_provider.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -17,8 +17,20 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # endregion
 
-from .level_aware_formatter import LevelAwareFormatter
+from __future__ import annotations
+
+from abc import ABC, abstractmethod
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from refind_btrfs.common import PackageConfig
+
+
+class BasePackageConfigProvider(ABC):
+    @abstractmethod
+    def get_config(self) -> PackageConfig:
+        pass
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/utility/file_package_config_provider.py` & `refind-btrfs-0.6.0/src/refind_btrfs/utility/file_package_config_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -145,24 +145,22 @@
                 )
                 raise PackageConfigError(
                     "Could not load the package configuration from file'!"
                 ) from e
             else:
                 current_package_config = FilePackageConfigProvider._read_config_from(
                     toml_document
-                ).with_initialization_type(
-                    ConfigInitializationType.PARSED, PackageConfig
-                )
+                ).with_initialization_type(ConfigInitializationType.PARSED)
 
                 persistence_provider.save_package_config(
                     none_throws(current_package_config)
                 )
         elif current_package_config is None:
             current_package_config = persisted_package_config.with_initialization_type(
-                ConfigInitializationType.PERSISTED, PackageConfig
+                ConfigInitializationType.PERSISTED
             )
 
         self._package_config = current_package_config
 
         return none_throws(current_package_config)
 
     @staticmethod
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/utility/helpers.py` & `refind-btrfs-0.6.0/src/refind_btrfs/utility/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -273,10 +273,10 @@
     if value is None:
         return default
 
     return value
 
 
 def checked_cast(destination_type: Type[TParam], value: Any) -> TParam:
-    check_type("value", value, destination_type)
+    check_type(value, destination_type)
 
     return cast(TParam, value)
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/utility/injector_modules.py` & `refind-btrfs-0.6.0/src/refind_btrfs/utility/injector_modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/utility/level_aware_formatter.py` & `refind-btrfs-0.6.0/src/refind_btrfs/utility/level_aware_formatter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/utility/logger_factories.py` & `refind-btrfs-0.6.0/src/refind_btrfs/utility/logger_factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs/utility/shelve_persistence_provider.py` & `refind-btrfs-0.6.0/src/refind_btrfs/utility/shelve_persistence_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # region Licensing
-# SPDX-FileCopyrightText: 2020-2022 Luka Žaja <luka.zaja@protonmail.com>
+# SPDX-FileCopyrightText: 2020-2023 Luka Žaja <luka.zaja@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """ refind-btrfs - Generate rEFInd manual boot stanzas from Btrfs snapshots
-Copyright (C) 2020-2022  Luka Žaja
+Copyright (C) 2020-2023 Luka Žaja
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs.egg-info/PKG-INFO` & `refind-btrfs-0.6.0/src/refind_btrfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: refind-btrfs
-Version: 0.5.6
+Version: 0.6.0
 Summary: Generate rEFInd manual boot stanzas from Btrfs snapshots
 Home-page: https://github.com/Venom1991/refind-btrfs
 Author: Luka Žaja
 Author-email: luka.zaja@protonmail.com
 Maintainer: Luka Žaja
 Maintainer-email: luka.zaja@protonmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Keywords: rEFInd,btrfs
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Boot
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: custom_icon
 License-File: LICENSE.txt
 
 # refind-btrfs
 
 ### Table of Contents
```

### Comparing `refind-btrfs-0.5.6/src/refind_btrfs.egg-info/SOURCES.txt` & `refind-btrfs-0.6.0/src/refind_btrfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

