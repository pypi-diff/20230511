# Comparing `tmp/cupid_matching-1.0.8.tar.gz` & `tmp/cupid_matching-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cupid_matching-1.0.8.tar", max compression
+gzip compressed data, was "cupid_matching-1.1.0.tar", max compression
```

## Comparing `cupid_matching-1.0.8.tar` & `cupid_matching-1.1.0.tar`

### file list

```diff
@@ -1,1722 +1,21 @@
--rw-r--r--   0        0        0     2376 2023-04-13 19:22:13.234033 cupid_matching-1.0.8/README.md
--rw-r--r--   0        0        0     6148 2023-04-03 19:49:27.937336 cupid_matching-1.0.8/cupid_matching/.DS_Store
--rw-r--r--   0        0        0      176 2023-04-01 13:41:41.834338 cupid_matching-1.0.8/cupid_matching/.idea/.gitignore
--rw-r--r--   0        0        0      539 2023-04-01 14:33:58.454731 cupid_matching-1.0.8/cupid_matching/.idea/cupid_matching.iml
--rw-r--r--   0        0        0     1446 2023-04-01 14:28:21.412476 cupid_matching-1.0.8/cupid_matching/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2023-04-01 14:28:21.442115 cupid_matching-1.0.8/cupid_matching/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      198 2023-04-01 14:28:21.437713 cupid_matching-1.0.8/cupid_matching/.idea/misc.xml
--rw-r--r--   0        0        0      280 2023-04-01 14:28:21.431899 cupid_matching-1.0.8/cupid_matching/.idea/modules.xml
--rw-r--r--   0        0        0      183 2023-04-01 14:28:21.446055 cupid_matching-1.0.8/cupid_matching/.idea/vcs.xml
--rw-r--r--   0        0        0      368 2023-04-01 14:33:58.460060 cupid_matching-1.0.8/cupid_matching/.idea/webResources.xml
--rw-r--r--   0        0        0     7536 2023-04-01 22:41:08.541782 cupid_matching-1.0.8/cupid_matching/.idea/workspace.xml
--rw-r--r--   0        0        0       34 2023-03-24 00:10:22.896173 cupid_matching-1.0.8/cupid_matching/.mypy_cache/.gitignore
--rw-r--r--   0        0        0        2 2023-03-31 20:06:15.815653 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0     8533 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/__future__.data.json
--rw-r--r--   0        0        0     1723 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/__future__.meta.json
--rw-r--r--   0        0        0     2266 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/__main__.data.json
--rw-r--r--   0        0        0     1690 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/__main__.meta.json
--rw-r--r--   0        0        0   193710 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1811 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    57330 2023-03-26 00:13:29.546583 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1857 2023-03-26 00:13:29.546903 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    19803 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1765 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0    11687 2023-03-24 00:33:08.242231 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_compression.data.json
--rw-r--r--   0        0        0     1537 2023-03-24 00:33:08.242423 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_compression.meta.json
--rw-r--r--   0        0        0    21518 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_csv.data.json
--rw-r--r--   0        0        0     1820 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_csv.meta.json
--rw-r--r--   0        0        0     3216 2023-03-26 00:13:29.544331 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1767 2023-03-26 00:13:29.544643 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0   209809 2023-03-24 00:33:08.226273 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_curses.data.json
--rw-r--r--   0        0        0     1545 2023-03-24 00:33:08.226582 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_curses.meta.json
--rw-r--r--   0        0        0   186643 2023-03-26 00:13:34.785852 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_decimal.data.json
--rw-r--r--   0        0        0     1812 2023-03-26 00:13:34.786283 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_decimal.meta.json
--rw-r--r--   0        0        0   122130 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_operator.data.json
--rw-r--r--   0        0        0     1779 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_operator.meta.json
--rw-r--r--   0        0        0     6702 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_random.data.json
--rw-r--r--   0        0        0     1717 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_random.meta.json
--rw-r--r--   0        0        0    99552 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_socket.data.json
--rw-r--r--   0        0        0     1841 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_socket.meta.json
--rw-r--r--   0        0        0    21636 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_stat.data.json
--rw-r--r--   0        0        0     1728 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_stat.meta.json
--rw-r--r--   0        0        0    26000 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_thread.data.json
--rw-r--r--   0        0        0     1809 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_thread.meta.json
--rw-r--r--   0        0        0    97013 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1889 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    14346 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_warnings.data.json
--rw-r--r--   0        0        0     1694 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_warnings.meta.json
--rw-r--r--   0        0        0    30012 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_weakref.data.json
--rw-r--r--   0        0        0     1793 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_weakref.meta.json
--rw-r--r--   0        0        0    55252 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_weakrefset.data.json
--rw-r--r--   0        0        0     1799 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/_weakrefset.meta.json
--rw-r--r--   0        0        0    22398 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1753 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0   165859 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/argparse.data.json
--rw-r--r--   0        0        0     1856 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/argparse.meta.json
--rw-r--r--   0        0        0    66415 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1820 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0   149483 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/ast.data.json
--rw-r--r--   0        0        0     1860 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/ast.meta.json
--rw-r--r--   0        0        0    11609 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/__init__.data.json
--rw-r--r--   0        0        0     2133 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/__init__.meta.json
--rw-r--r--   0        0        0   108563 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/base_events.data.json
--rw-r--r--   0        0        0     2080 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/base_events.meta.json
--rw-r--r--   0        0        0    27666 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/coroutines.data.json
--rw-r--r--   0        0        0     1798 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/coroutines.meta.json
--rw-r--r--   0        0        0   210031 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/events.data.json
--rw-r--r--   0        0        0     2118 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/events.meta.json
--rw-r--r--   0        0        0     9803 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/exceptions.data.json
--rw-r--r--   0        0        0     1747 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/exceptions.meta.json
--rw-r--r--   0        0        0    40152 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/futures.data.json
--rw-r--r--   0        0        0     1938 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/futures.meta.json
--rw-r--r--   0        0        0    29212 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/locks.data.json
--rw-r--r--   0        0        0     1889 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/locks.meta.json
--rw-r--r--   0        0        0    18739 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/protocols.data.json
--rw-r--r--   0        0        0     1841 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/protocols.meta.json
--rw-r--r--   0        0        0    25226 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/queues.data.json
--rw-r--r--   0        0        0     1777 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/queues.meta.json
--rw-r--r--   0        0        0     5100 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/runners.data.json
--rw-r--r--   0        0        0     1836 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/runners.meta.json
--rw-r--r--   0        0        0     4172 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/selector_events.data.json
--rw-r--r--   0        0        0     1815 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/selector_events.meta.json
--rw-r--r--   0        0        0    37972 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/streams.data.json
--rw-r--r--   0        0        0     1947 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/streams.meta.json
--rw-r--r--   0        0        0    26110 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/subprocess.data.json
--rw-r--r--   0        0        0     1957 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/subprocess.meta.json
--rw-r--r--   0        0        0   109221 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/tasks.data.json
--rw-r--r--   0        0        0     1938 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/tasks.meta.json
--rw-r--r--   0        0        0     6124 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/threads.data.json
--rw-r--r--   0        0        0     1757 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/threads.meta.json
--rw-r--r--   0        0        0    29800 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/transports.data.json
--rw-r--r--   0        0        0     1804 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/transports.meta.json
--rw-r--r--   0        0        0    63976 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/unix_events.data.json
--rw-r--r--   0        0        0     1922 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/asyncio/unix_events.meta.json
--rw-r--r--   0        0        0     6876 2023-03-24 00:33:08.293024 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/atexit.data.json
--rw-r--r--   0        0        0     1521 2023-03-24 00:33:08.293214 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/atexit.meta.json
--rw-r--r--   0        0        0   223621 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/attr/__init__.data.json
--rw-r--r--   0        0        0     1930 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/attr/__init__.meta.json
--rw-r--r--   0        0        0     4320 2023-03-26 00:13:34.354724 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/attr/_cmp.data.json
--rw-r--r--   0        0        0     1672 2023-03-26 00:13:34.355096 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/attr/_cmp.meta.json
--rw-r--r--   0        0        0     3311 2023-03-26 00:13:34.354000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/attr/_typing_compat.data.json
--rw-r--r--   0        0        0     1692 2023-03-26 00:13:34.354215 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/attr/_typing_compat.meta.json
--rw-r--r--   0        0        0     7637 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/attr/_version_info.data.json
--rw-r--r--   0        0        0     1691 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/attr/_version_info.meta.json
--rw-r--r--   0        0        0     9098 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/attr/converters.data.json
--rw-r--r--   0        0        0     1698 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/attr/converters.meta.json
--rw-r--r--   0        0        0    11099 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/attr/exceptions.data.json
--rw-r--r--   0        0        0     1684 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/attr/exceptions.meta.json
--rw-r--r--   0        0        0     3904 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/attr/filters.data.json
--rw-r--r--   0        0        0     1692 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/attr/filters.meta.json
--rw-r--r--   0        0        0     8436 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/attr/setters.data.json
--rw-r--r--   0        0        0     1692 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/attr/setters.meta.json
--rw-r--r--   0        0        0    45671 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/attr/validators.data.json
--rw-r--r--   0        0        0     1734 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/attr/validators.meta.json
--rw-r--r--   0        0        0    13545 2023-03-24 00:33:08.329875 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/base64.data.json
--rw-r--r--   0        0        0     1543 2023-03-24 00:33:08.330150 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/base64.meta.json
--rw-r--r--   0        0        0    15400 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/binascii.data.json
--rw-r--r--   0        0        0     1818 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/binascii.meta.json
--rw-r--r--   0        0        0  1141247 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1917 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0    62654 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/calendar.data.json
--rw-r--r--   0        0        0     1810 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/calendar.meta.json
--rw-r--r--   0        0        0     8399 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/__init__.data.json
--rw-r--r--   0        0        0     1889 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/__init__.meta.json
--rw-r--r--   0        0        0    51443 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/_compat.data.json
--rw-r--r--   0        0        0     1950 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/_compat.meta.json
--rw-r--r--   0        0        0    48731 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/_termui_impl.data.json
--rw-r--r--   0        0        0     2228 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/_termui_impl.meta.json
--rw-r--r--   0        0        0     5845 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/_textwrap.data.json
--rw-r--r--   0        0        0     1772 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/_textwrap.meta.json
--rw-r--r--   0        0        0   197021 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/core.data.json
--rw-r--r--   0        0        0     2286 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/core.meta.json
--rw-r--r--   0        0        0    61474 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/decorators.data.json
--rw-r--r--   0        0        0     1978 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/decorators.meta.json
--rw-r--r--   0        0        0    30027 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/exceptions.data.json
--rw-r--r--   0        0        0     1906 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/exceptions.meta.json
--rw-r--r--   0        0        0    19110 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/formatting.data.json
--rw-r--r--   0        0        0     1922 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/formatting.meta.json
--rw-r--r--   0        0        0     7702 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/globals.data.json
--rw-r--r--   0        0        0     1749 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/globals.meta.json
--rw-r--r--   0        0        0    31268 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/parser.data.json
--rw-r--r--   0        0        0     1938 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/parser.meta.json
--rw-r--r--   0        0        0    36601 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/shell_completion.data.json
--rw-r--r--   0        0        0     1997 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/shell_completion.meta.json
--rw-r--r--   0        0        0    25539 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/termui.data.json
--rw-r--r--   0        0        0     2113 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/termui.meta.json
--rw-r--r--   0        0        0    88334 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/types.data.json
--rw-r--r--   0        0        0     2135 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/types.meta.json
--rw-r--r--   0        0        0    34946 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/utils.data.json
--rw-r--r--   0        0        0     2014 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/click/utils.meta.json
--rw-r--r--   0        0        0   134251 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1871 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   446304 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1900 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     4078 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1731 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0     8295 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/colorsys.data.json
--rw-r--r--   0        0        0     1692 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/colorsys.meta.json
--rw-r--r--   0        0        0     1701 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/concurrent/__init__.data.json
--rw-r--r--   0        0        0     1703 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/concurrent/__init__.meta.json
--rw-r--r--   0        0        0     4942 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/concurrent/futures/__init__.data.json
--rw-r--r--   0        0        0     1862 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/concurrent/futures/__init__.meta.json
--rw-r--r--   0        0        0    65940 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/concurrent/futures/_base.data.json
--rw-r--r--   0        0        0     1861 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/concurrent/futures/_base.meta.json
--rw-r--r--   0        0        0    65236 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/concurrent/futures/process.data.json
--rw-r--r--   0        0        0     2105 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/concurrent/futures/process.meta.json
--rw-r--r--   0        0        0    23845 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/concurrent/futures/thread.data.json
--rw-r--r--   0        0        0     1906 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/concurrent/futures/thread.meta.json
--rw-r--r--   0        0        0   135261 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/configparser.data.json
--rw-r--r--   0        0        0     1811 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/configparser.meta.json
--rw-r--r--   0        0        0   113709 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1795 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0    41358 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/contextvars.data.json
--rw-r--r--   0        0        0     1799 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/contextvars.meta.json
--rw-r--r--   0        0        0     5981 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/copy.data.json
--rw-r--r--   0        0        0     1683 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/copy.meta.json
--rw-r--r--   0        0        0    13018 2023-03-26 00:13:34.335416 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/copyreg.data.json
--rw-r--r--   0        0        0     1761 2023-03-26 00:13:34.335692 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/copyreg.meta.json
--rw-r--r--   0        0        0    32485 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/csv.data.json
--rw-r--r--   0        0        0     1786 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/csv.meta.json
--rw-r--r--   0        0        0   140977 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1863 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0    59518 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/ctypes/wintypes.data.json
--rw-r--r--   0        0        0     1751 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/ctypes/wintypes.meta.json
--rw-r--r--   0        0        0     1886 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/__init__.data.json
--rw-r--r--   0        0        0     1627 2023-03-26 00:20:01.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/__init__.meta.json
--rw-r--r--   0        0        0    19942 2023-03-31 00:13:20.670231 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/choo_siow.data.json
--rw-r--r--   0        0        0     1973 2023-03-31 00:13:35.679368 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/choo_siow.meta.json
--rw-r--r--   0        0        0    11868 2023-03-26 00:15:21.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/choo_siow_gender_heteroskedastic.data.json
--rw-r--r--   0        0        0     1960 2023-03-26 00:15:21.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/choo_siow_gender_heteroskedastic.meta.json
--rw-r--r--   0        0        0    11469 2023-03-26 00:15:38.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/choo_siow_heteroskedastic.data.json
--rw-r--r--   0        0        0     1987 2023-03-26 00:15:38.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/choo_siow_heteroskedastic.meta.json
--rw-r--r--   0        0        0    26170 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/entropy.data.json
--rw-r--r--   0        0        0     1950 2023-03-26 00:15:04.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/entropy.meta.json
--rw-r--r--   0        0        0    14219 2023-03-31 00:09:30.605965 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/example_choosiow.data.json
--rw-r--r--   0        0        0     2268 2023-03-31 20:06:15.715703 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/example_choosiow.meta.json
--rw-r--r--   0        0        0    41751 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/ipfp_solvers.data.json
--rw-r--r--   0        0        0     2171 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/ipfp_solvers.meta.json
--rw-r--r--   0        0        0    23713 2023-03-31 00:08:02.284018 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/matching_utils.data.json
--rw-r--r--   0        0        0     2060 2023-03-31 00:08:38.022513 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/matching_utils.meta.json
--rw-r--r--   0        0        0     6582 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/min_distance.data.json
--rw-r--r--   0        0        0     2090 2023-03-31 00:01:19.623758 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/min_distance.meta.json
--rw-r--r--   0        0        0    18530 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/min_distance_utils.data.json
--rw-r--r--   0        0        0     1761 2023-03-31 00:04:47.598975 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/min_distance_utils.meta.json
--rw-r--r--   0        0        0    30249 2023-03-26 00:19:58.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/model_classes.data.json
--rw-r--r--   0        0        0     2073 2023-03-30 20:37:53.188328 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/model_classes.meta.json
--rw-r--r--   0        0        0    14091 2023-03-30 19:44:48.506574 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/nested_logit.data.json
--rw-r--r--   0        0        0     1976 2023-03-30 20:20:57.768148 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/nested_logit.meta.json
--rw-r--r--   0        0        0     4723 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/poisson_glm.data.json
--rw-r--r--   0        0        0     2083 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/poisson_glm.meta.json
--rw-r--r--   0        0        0    26002 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/poisson_glm_utils.data.json
--rw-r--r--   0        0        0     1979 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/poisson_glm_utils.meta.json
--rw-r--r--   0        0        0    52498 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/utils.data.json
--rw-r--r--   0        0        0     2031 2023-03-30 21:15:39.004804 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/cupid_matching/utils.meta.json
--rw-r--r--   0        0        0    36090 2023-03-24 00:33:08.700532 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/curses/__init__.data.json
--rw-r--r--   0        0        0     1548 2023-03-24 00:33:08.700758 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/curses/__init__.meta.json
--rw-r--r--   0        0        0    63289 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/dataclasses.data.json
--rw-r--r--   0        0        0     1813 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/dataclasses.meta.json
--rw-r--r--   0        0        0   154595 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/datetime.data.json
--rw-r--r--   0        0        0     1767 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/datetime.meta.json
--rw-r--r--   0        0        0     5337 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/decimal.data.json
--rw-r--r--   0        0        0     1708 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/decimal.meta.json
--rw-r--r--   0        0        0    63796 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/difflib.data.json
--rw-r--r--   0        0        0     1764 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/difflib.meta.json
--rw-r--r--   0        0        0    44121 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/dis.data.json
--rw-r--r--   0        0        0     1800 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/dis.meta.json
--rw-r--r--   0        0        0     1693 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/distutils/__init__.data.json
--rw-r--r--   0        0        0     1701 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/distutils/__init__.meta.json
--rw-r--r--   0        0        0     3146 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/distutils/spawn.data.json
--rw-r--r--   0        0        0     1706 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/distutils/spawn.meta.json
--rw-r--r--   0        0        0    73586 2023-03-24 00:33:09.975572 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/doctest.data.json
--rw-r--r--   0        0        0     1546 2023-03-24 00:33:09.975824 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/doctest.meta.json
--rw-r--r--   0        0        0     8164 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1792 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    13316 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1728 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7938 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1763 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    27029 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1735 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0    10030 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1748 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    86532 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1866 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    33615 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1821 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0    21539 2023-03-24 00:33:08.825139 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/email/utils.data.json
--rw-r--r--   0        0        0     1595 2023-03-24 00:33:08.825355 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/email/utils.meta.json
--rw-r--r--   0        0        0    66878 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1785 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0    21276 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/errno.data.json
--rw-r--r--   0        0        0     1746 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/errno.meta.json
--rw-r--r--   0        0        0     6702 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/fnmatch.data.json
--rw-r--r--   0        0        0     1714 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/fnmatch.meta.json
--rw-r--r--   0        0        0    95820 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/fractions.data.json
--rw-r--r--   0        0        0     1833 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/fractions.meta.json
--rw-r--r--   0        0        0   139322 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/functools.data.json
--rw-r--r--   0        0        0     1794 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/functools.meta.json
--rw-r--r--   0        0        0    17518 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/gc.data.json
--rw-r--r--   0        0        0     1766 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/gc.meta.json
--rw-r--r--   0        0        0    24438 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1782 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0     4118 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/getpass.data.json
--rw-r--r--   0        0        0     1689 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/getpass.meta.json
--rw-r--r--   0        0        0    58377 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/gettext.data.json
--rw-r--r--   0        0        0     1801 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/gettext.meta.json
--rw-r--r--   0        0        0    11610 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/__init__.data.json
--rw-r--r--   0        0        0     2229 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/__init__.meta.json
--rw-r--r--   0        0        0    94624 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/cmd.data.json
--rw-r--r--   0        0        0     2161 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/cmd.meta.json
--rw-r--r--   0        0        0    16991 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/compat.data.json
--rw-r--r--   0        0        0     1860 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/compat.meta.json
--rw-r--r--   0        0        0    70918 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/config.data.json
--rw-r--r--   0        0        0     2222 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/config.meta.json
--rw-r--r--   0        0        0     8500 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/db.data.json
--rw-r--r--   0        0        0     1809 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/db.meta.json
--rw-r--r--   0        0        0    44019 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/diff.data.json
--rw-r--r--   0        0        0     2230 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/diff.meta.json
--rw-r--r--   0        0        0    26547 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/exc.data.json
--rw-r--r--   0        0        0     1932 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/exc.meta.json
--rw-r--r--   0        0        0     2289 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/index/__init__.data.json
--rw-r--r--   0        0        0     1727 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/index/__init__.meta.json
--rw-r--r--   0        0        0    68238 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/index/base.data.json
--rw-r--r--   0        0        0     2696 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/index/base.meta.json
--rw-r--r--   0        0        0    19414 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/index/fun.data.json
--rw-r--r--   0        0        0     2286 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/index/fun.meta.json
--rw-r--r--   0        0        0    54611 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/index/typ.data.json
--rw-r--r--   0        0        0     2038 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/index/typ.meta.json
--rw-r--r--   0        0        0    14692 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/index/util.data.json
--rw-r--r--   0        0        0     2051 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/index/util.meta.json
--rw-r--r--   0        0        0     3806 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/__init__.data.json
--rw-r--r--   0        0        0     2108 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/__init__.meta.json
--rw-r--r--   0        0        0    29422 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/base.data.json
--rw-r--r--   0        0        0     2277 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/base.meta.json
--rw-r--r--   0        0        0     6454 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/blob.data.json
--rw-r--r--   0        0        0     1851 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/blob.meta.json
--rw-r--r--   0        0        0    42768 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/commit.data.json
--rw-r--r--   0        0        0     2418 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/commit.meta.json
--rw-r--r--   0        0        0    13624 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/fun.data.json
--rw-r--r--   0        0        0     1896 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/fun.meta.json
--rw-r--r--   0        0        0     1768 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/submodule/__init__.data.json
--rw-r--r--   0        0        0     1704 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/submodule/__init__.meta.json
--rw-r--r--   0        0        0    68535 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/submodule/base.data.json
--rw-r--r--   0        0        0     2644 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/submodule/base.meta.json
--rw-r--r--   0        0        0    13516 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/submodule/root.data.json
--rw-r--r--   0        0        0     2410 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/submodule/root.meta.json
--rw-r--r--   0        0        0    12286 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/submodule/util.data.json
--rw-r--r--   0        0        0     2362 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/submodule/util.meta.json
--rw-r--r--   0        0        0     9168 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/tag.data.json
--rw-r--r--   0        0        0     2013 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/tag.meta.json
--rw-r--r--   0        0        0    39730 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/tree.data.json
--rw-r--r--   0        0        0     2231 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/tree.meta.json
--rw-r--r--   0        0        0    95020 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/util.data.json
--rw-r--r--   0        0        0     2344 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/objects/util.meta.json
--rw-r--r--   0        0        0     2571 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/refs/__init__.data.json
--rw-r--r--   0        0        0     1826 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/refs/__init__.meta.json
--rw-r--r--   0        0        0    18553 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/refs/head.data.json
--rw-r--r--   0        0        0     2206 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/refs/head.meta.json
--rw-r--r--   0        0        0    42003 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/refs/log.data.json
--rw-r--r--   0        0        0     2160 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/refs/log.meta.json
--rw-r--r--   0        0        0    18680 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/refs/reference.data.json
--rw-r--r--   0        0        0     2157 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/refs/reference.meta.json
--rw-r--r--   0        0        0    10734 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/refs/remote.data.json
--rw-r--r--   0        0        0     1979 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/refs/remote.meta.json
--rw-r--r--   0        0        0    62889 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/refs/symbolic.data.json
--rw-r--r--   0        0        0     2392 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/refs/symbolic.meta.json
--rw-r--r--   0        0        0    13602 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/refs/tag.data.json
--rw-r--r--   0        0        0     2072 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/refs/tag.meta.json
--rw-r--r--   0        0        0    88392 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/remote.data.json
--rw-r--r--   0        0        0     2552 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/remote.meta.json
--rw-r--r--   0        0        0     1754 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/repo/__init__.data.json
--rw-r--r--   0        0        0     1701 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/repo/__init__.meta.json
--rw-r--r--   0        0        0   113367 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/repo/base.data.json
--rw-r--r--   0        0        0     2753 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/repo/base.meta.json
--rw-r--r--   0        0        0    12926 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/repo/fun.data.json
--rw-r--r--   0        0        0     2490 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/repo/fun.meta.json
--rw-r--r--   0        0        0    12850 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/types.data.json
--rw-r--r--   0        0        0     1786 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/types.meta.json
--rw-r--r--   0        0        0   116599 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/util.data.json
--rw-r--r--   0        0        0     2393 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/git/util.meta.json
--rw-r--r--   0        0        0    10323 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/glob.data.json
--rw-r--r--   0        0        0     1755 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/glob.meta.json
--rw-r--r--   0        0        0    46028 2023-03-24 00:33:08.706805 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/gzip.data.json
--rw-r--r--   0        0        0     1615 2023-03-24 00:33:08.707126 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/gzip.meta.json
--rw-r--r--   0        0        0    30047 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/hashlib.data.json
--rw-r--r--   0        0        0     1840 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/hashlib.meta.json
--rw-r--r--   0        0        0    12366 2023-03-24 00:33:08.231680 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/heapq.data.json
--rw-r--r--   0        0        0     1511 2023-03-24 00:33:08.231868 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/heapq.meta.json
--rw-r--r--   0        0        0    18362 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/hmac.data.json
--rw-r--r--   0        0        0     1849 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/hmac.meta.json
--rw-r--r--   0        0        0     4601 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/html/__init__.data.json
--rw-r--r--   0        0        0     1692 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/html/__init__.meta.json
--rw-r--r--   0        0        0     2995 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/html/entities.data.json
--rw-r--r--   0        0        0     1702 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/html/entities.meta.json
--rw-r--r--   0        0        0    19707 2023-03-24 00:33:08.703443 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/http/__init__.data.json
--rw-r--r--   0        0        0     1590 2023-03-24 00:33:08.703699 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/http/__init__.meta.json
--rw-r--r--   0        0        0    64975 2023-03-24 00:33:08.911213 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/http/client.data.json
--rw-r--r--   0        0        0     1651 2023-03-24 00:33:08.911418 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/http/client.meta.json
--rw-r--r--   0        0        0    29585 2023-03-24 00:33:08.308792 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/http/cookies.data.json
--rw-r--r--   0        0        0     1570 2023-03-24 00:33:08.309022 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/http/cookies.meta.json
--rw-r--r--   0        0        0     9461 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/imghdr.data.json
--rw-r--r--   0        0        0     1744 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/imghdr.meta.json
--rw-r--r--   0        0        0     6724 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1766 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    75569 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1849 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    69970 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1925 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    97936 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1931 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12974 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1748 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    82375 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib_metadata/__init__.data.json
--rw-r--r--   0        0        0     2532 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib_metadata/__init__.meta.json
--rw-r--r--   0        0        0     7079 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib_metadata/_adapters.data.json
--rw-r--r--   0        0        0     2008 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib_metadata/_adapters.meta.json
--rw-r--r--   0        0        0    24836 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib_metadata/_collections.data.json
--rw-r--r--   0        0        0     1803 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib_metadata/_collections.meta.json
--rw-r--r--   0        0        0     6087 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib_metadata/_compat.data.json
--rw-r--r--   0        0        0     1767 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib_metadata/_compat.meta.json
--rw-r--r--   0        0        0     2330 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib_metadata/_functools.data.json
--rw-r--r--   0        0        0     1769 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib_metadata/_functools.meta.json
--rw-r--r--   0        0        0     2314 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib_metadata/_itertools.data.json
--rw-r--r--   0        0        0     1861 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib_metadata/_itertools.meta.json
--rw-r--r--   0        0        0    20089 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib_metadata/_meta.data.json
--rw-r--r--   0        0        0     1738 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib_metadata/_meta.meta.json
--rw-r--r--   0        0        0     3598 2023-03-26 00:13:35.270572 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib_metadata/_py39compat.data.json
--rw-r--r--   0        0        0     1778 2023-03-26 00:13:35.270946 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib_metadata/_py39compat.meta.json
--rw-r--r--   0        0        0     5913 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib_metadata/_text.data.json
--rw-r--r--   0        0        0     1835 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/importlib_metadata/_text.meta.json
--rw-r--r--   0        0        0   370620 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/inspect.data.json
--rw-r--r--   0        0        0     1844 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/inspect.meta.json
--rw-r--r--   0        0        0    93297 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1876 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0   292387 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/itertools.data.json
--rw-r--r--   0        0        0     1796 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/itertools.meta.json
--rw-r--r--   0        0        0    16899 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/json/__init__.data.json
--rw-r--r--   0        0        0     1781 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/json/__init__.meta.json
--rw-r--r--   0        0        0    15866 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/json/decoder.data.json
--rw-r--r--   0        0        0     1725 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/json/decoder.meta.json
--rw-r--r--   0        0        0    11888 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/json/encoder.data.json
--rw-r--r--   0        0        0     1737 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/json/encoder.meta.json
--rw-r--r--   0        0        0    10180 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/linecache.data.json
--rw-r--r--   0        0        0     1754 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/linecache.meta.json
--rw-r--r--   0        0        0    35009 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/locale.data.json
--rw-r--r--   0        0        0     1798 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/locale.meta.json
--rw-r--r--   0        0        0   154306 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/logging/__init__.data.json
--rw-r--r--   0        0        0     1889 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/logging/__init__.meta.json
--rw-r--r--   0        0        0    75364 2023-03-24 00:33:08.951159 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/logging/handlers.data.json
--rw-r--r--   0        0        0     1739 2023-03-24 00:33:08.951619 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/logging/handlers.meta.json
--rw-r--r--   0        0        0     2660 2023-03-26 00:13:35.201449 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/__init__.data.json
--rw-r--r--   0        0        0     1711 2023-03-26 00:13:35.201999 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/__init__.meta.json
--rw-r--r--   0        0        0     2238 2023-03-26 00:13:34.704258 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/_compat.data.json
--rw-r--r--   0        0        0     1770 2023-03-26 00:13:34.704668 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/_compat.meta.json
--rw-r--r--   0        0        0     5115 2023-03-26 00:13:34.328133 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/_punycode.data.json
--rw-r--r--   0        0        0     1837 2023-03-26 00:13:34.328527 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/_punycode.meta.json
--rw-r--r--   0        0        0     1744 2023-03-26 00:13:34.328945 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/common/__init__.data.json
--rw-r--r--   0        0        0     1697 2023-03-26 00:13:34.329370 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/common/__init__.meta.json
--rw-r--r--   0        0        0     1924 2023-03-26 00:13:34.697644 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/common/entities.data.json
--rw-r--r--   0        0        0     1774 2023-03-26 00:13:34.698031 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/common/entities.meta.json
--rw-r--r--   0        0        0     1865 2023-03-26 00:13:34.322693 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/common/html_blocks.data.json
--rw-r--r--   0        0        0     1714 2023-03-26 00:13:34.322941 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/common/html_blocks.meta.json
--rw-r--r--   0        0        0     5411 2023-03-26 00:13:34.321727 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/common/html_re.data.json
--rw-r--r--   0        0        0     1734 2023-03-26 00:13:34.322180 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/common/html_re.meta.json
--rw-r--r--   0        0        0     6261 2023-03-26 00:13:35.198922 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/common/normalize_url.data.json
--rw-r--r--   0        0        0     2000 2023-03-26 00:13:35.199527 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/common/normalize_url.meta.json
--rw-r--r--   0        0        0    15438 2023-03-26 00:13:34.946088 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/common/utils.data.json
--rw-r--r--   0        0        0     1896 2023-03-26 00:13:34.946457 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/common/utils.meta.json
--rw-r--r--   0        0        0     2817 2023-03-26 00:13:35.195811 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/helpers/__init__.data.json
--rw-r--r--   0        0        0     1845 2023-03-26 00:13:35.196197 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/helpers/__init__.meta.json
--rw-r--r--   0        0        0     5696 2023-03-26 00:13:35.030599 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/helpers/parse_link_destination.data.json
--rw-r--r--   0        0        0     1802 2023-03-26 00:13:35.031132 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/helpers/parse_link_destination.meta.json
--rw-r--r--   0        0        0     2547 2023-03-26 00:13:35.194368 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/helpers/parse_link_label.data.json
--rw-r--r--   0        0        0     1900 2023-03-26 00:13:35.194789 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/helpers/parse_link_label.meta.json
--rw-r--r--   0        0        0     5856 2023-03-26 00:13:35.027634 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/helpers/parse_link_title.data.json
--rw-r--r--   0        0        0     1790 2023-03-26 00:13:35.028204 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/helpers/parse_link_title.meta.json
--rw-r--r--   0        0        0    27407 2023-03-26 00:13:35.200484 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/main.data.json
--rw-r--r--   0        0        0     2499 2023-03-26 00:13:35.200956 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/main.meta.json
--rw-r--r--   0        0        0     6421 2023-03-26 00:13:35.197836 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/parser_block.data.json
--rw-r--r--   0        0        0     2409 2023-03-26 00:13:35.198249 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/parser_block.meta.json
--rw-r--r--   0        0        0     5356 2023-03-26 00:13:35.195248 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/parser_core.data.json
--rw-r--r--   0        0        0     2083 2023-03-26 00:13:35.195518 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/parser_core.meta.json
--rw-r--r--   0        0        0     7763 2023-03-26 00:13:35.196945 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/parser_inline.data.json
--rw-r--r--   0        0        0     2513 2023-03-26 00:13:35.197330 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/parser_inline.meta.json
--rw-r--r--   0        0        0     4548 2023-03-26 00:13:34.702779 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/presets/__init__.data.json
--rw-r--r--   0        0        0     1831 2023-03-26 00:13:34.703316 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/presets/__init__.meta.json
--rw-r--r--   0        0        0     1830 2023-03-26 00:13:34.326115 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/presets/commonmark.data.json
--rw-r--r--   0        0        0     1715 2023-03-26 00:13:34.326357 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/presets/commonmark.meta.json
--rw-r--r--   0        0        0     1806 2023-03-26 00:13:34.325135 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/presets/default.data.json
--rw-r--r--   0        0        0     1709 2023-03-26 00:13:34.325437 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/presets/default.meta.json
--rw-r--r--   0        0        0     1782 2023-03-26 00:13:34.324317 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/presets/zero.data.json
--rw-r--r--   0        0        0     1703 2023-03-26 00:13:34.324602 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/presets/zero.meta.json
--rw-r--r--   0        0        0    22321 2023-03-26 00:13:35.038870 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/renderer.data.json
--rw-r--r--   0        0        0     1974 2023-03-26 00:13:35.039452 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/renderer.meta.json
--rw-r--r--   0        0        0    26281 2023-03-26 00:13:35.166315 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/ruler.data.json
--rw-r--r--   0        0        0     1947 2023-03-26 00:13:35.166749 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/ruler.meta.json
--rw-r--r--   0        0        0     3958 2023-03-26 00:13:35.192419 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/__init__.data.json
--rw-r--r--   0        0        0     2213 2023-03-26 00:13:35.192972 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/__init__.meta.json
--rw-r--r--   0        0        0     3156 2023-03-26 00:13:35.184176 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/blockquote.data.json
--rw-r--r--   0        0        0     2003 2023-03-26 00:13:35.184769 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/blockquote.meta.json
--rw-r--r--   0        0        0     2857 2023-03-26 00:13:35.183157 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/code.data.json
--rw-r--r--   0        0        0     1845 2023-03-26 00:13:35.183599 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/code.meta.json
--rw-r--r--   0        0        0     2870 2023-03-26 00:13:35.182393 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/fence.data.json
--rw-r--r--   0        0        0     1848 2023-03-26 00:13:35.182800 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/fence.meta.json
--rw-r--r--   0        0        0     3117 2023-03-26 00:13:35.181647 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/heading.data.json
--rw-r--r--   0        0        0     2000 2023-03-26 00:13:35.182044 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/heading.meta.json
--rw-r--r--   0        0        0     2938 2023-03-26 00:13:35.180958 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/hr.data.json
--rw-r--r--   0        0        0     1905 2023-03-26 00:13:35.181274 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/hr.meta.json
--rw-r--r--   0        0        0     4228 2023-03-26 00:13:35.180356 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/html_block.data.json
--rw-r--r--   0        0        0     2102 2023-03-26 00:13:35.180659 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/html_block.meta.json
--rw-r--r--   0        0        0     3005 2023-03-26 00:13:35.179741 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/lheading.data.json
--rw-r--r--   0        0        0     1980 2023-03-26 00:13:35.180033 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/lheading.meta.json
--rw-r--r--   0        0        0     5541 2023-03-26 00:13:35.179097 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/list.data.json
--rw-r--r--   0        0        0     2084 2023-03-26 00:13:35.179429 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/list.meta.json
--rw-r--r--   0        0        0     3018 2023-03-26 00:13:35.178477 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/paragraph.data.json
--rw-r--r--   0        0        0     1917 2023-03-26 00:13:35.178727 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/paragraph.meta.json
--rw-r--r--   0        0        0     3494 2023-03-26 00:13:35.177979 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/reference.data.json
--rw-r--r--   0        0        0     2009 2023-03-26 00:13:35.178217 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/reference.meta.json
--rw-r--r--   0        0        0    15095 2023-03-26 00:13:35.168633 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/state_block.data.json
--rw-r--r--   0        0        0     1889 2023-03-26 00:13:35.168938 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/state_block.meta.json
--rw-r--r--   0        0        0     4568 2023-03-26 00:13:35.177270 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/table.data.json
--rw-r--r--   0        0        0     1995 2023-03-26 00:13:35.177647 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/table.meta.json
--rw-r--r--   0        0        0     3303 2023-03-26 00:13:35.193444 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/__init__.data.json
--rw-r--r--   0        0        0     2005 2023-03-26 00:13:35.193933 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/__init__.meta.json
--rw-r--r--   0        0        0     2440 2023-03-26 00:13:35.190239 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/block.data.json
--rw-r--r--   0        0        0     1870 2023-03-26 00:13:35.190802 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/block.meta.json
--rw-r--r--   0        0        0     2356 2023-03-26 00:13:35.189364 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/inline.data.json
--rw-r--r--   0        0        0     1874 2023-03-26 00:13:35.189820 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/inline.meta.json
--rw-r--r--   0        0        0     5499 2023-03-26 00:13:35.188306 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/linkify.data.json
--rw-r--r--   0        0        0     2003 2023-03-26 00:13:35.188885 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/linkify.meta.json
--rw-r--r--   0        0        0     3060 2023-03-26 00:13:35.187283 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/normalize.data.json
--rw-r--r--   0        0        0     1817 2023-03-26 00:13:35.187768 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/normalize.meta.json
--rw-r--r--   0        0        0     8849 2023-03-26 00:13:35.185383 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/replacements.data.json
--rw-r--r--   0        0        0     1949 2023-03-26 00:13:35.185879 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/replacements.meta.json
--rw-r--r--   0        0        0     5686 2023-03-26 00:13:35.186361 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/smartquotes.data.json
--rw-r--r--   0        0        0     2015 2023-03-26 00:13:35.186806 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/smartquotes.meta.json
--rw-r--r--   0        0        0     4895 2023-03-26 00:13:35.169337 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/state_core.data.json
--rw-r--r--   0        0        0     1868 2023-03-26 00:13:35.169670 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/state_core.meta.json
--rw-r--r--   0        0        0     4261 2023-03-26 00:13:35.191396 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/__init__.data.json
--rw-r--r--   0        0        0     2336 2023-03-26 00:13:35.191840 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/__init__.meta.json
--rw-r--r--   0        0        0     3119 2023-03-26 00:13:35.175685 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/autolink.data.json
--rw-r--r--   0        0        0     1851 2023-03-26 00:13:35.175898 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/autolink.meta.json
--rw-r--r--   0        0        0     2814 2023-03-26 00:13:35.175202 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/backticks.data.json
--rw-r--r--   0        0        0     1854 2023-03-26 00:13:35.175433 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/backticks.meta.json
--rw-r--r--   0        0        0     3502 2023-03-26 00:13:35.174694 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/balance_pairs.data.json
--rw-r--r--   0        0        0     1806 2023-03-26 00:13:35.174958 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/balance_pairs.meta.json
--rw-r--r--   0        0        0     3744 2023-03-26 00:13:35.176693 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/emphasis.data.json
--rw-r--r--   0        0        0     1901 2023-03-26 00:13:35.176946 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/emphasis.meta.json
--rw-r--r--   0        0        0     3519 2023-03-26 00:13:35.174171 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/entity.data.json
--rw-r--r--   0        0        0     2033 2023-03-26 00:13:35.174393 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/entity.meta.json
--rw-r--r--   0        0        0     3090 2023-03-26 00:13:35.173649 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/escape.data.json
--rw-r--r--   0        0        0     1883 2023-03-26 00:13:35.173916 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/escape.meta.json
--rw-r--r--   0        0        0     3399 2023-03-26 00:13:35.173129 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/html_inline.data.json
--rw-r--r--   0        0        0     1906 2023-03-26 00:13:35.173368 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/html_inline.meta.json
--rw-r--r--   0        0        0     2929 2023-03-26 00:13:35.172339 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/image.data.json
--rw-r--r--   0        0        0     1991 2023-03-26 00:13:35.172799 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/image.meta.json
--rw-r--r--   0        0        0     2707 2023-03-26 00:13:35.171848 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/link.data.json
--rw-r--r--   0        0        0     1942 2023-03-26 00:13:35.172084 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/link.meta.json
--rw-r--r--   0        0        0     3094 2023-03-26 00:13:35.171354 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/newline.data.json
--rw-r--r--   0        0        0     1885 2023-03-26 00:13:35.171598 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/newline.meta.json
--rw-r--r--   0        0        0    38094 2023-03-26 00:13:35.167623 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/state_inline.data.json
--rw-r--r--   0        0        0     2013 2023-03-26 00:13:35.168040 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/state_inline.meta.json
--rw-r--r--   0        0        0     4517 2023-03-26 00:13:35.176219 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/strikethrough.data.json
--rw-r--r--   0        0        0     1882 2023-03-26 00:13:35.176431 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/strikethrough.meta.json
--rw-r--r--   0        0        0     2893 2023-03-26 00:13:35.170654 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/text.data.json
--rw-r--r--   0        0        0     1788 2023-03-26 00:13:35.171004 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/text.meta.json
--rw-r--r--   0        0        0     2648 2023-03-26 00:13:35.170037 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/text_collapse.data.json
--rw-r--r--   0        0        0     1862 2023-03-26 00:13:35.170304 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/text_collapse.meta.json
--rw-r--r--   0        0        0    24990 2023-03-26 00:13:34.957331 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/token.data.json
--rw-r--r--   0        0        0     1959 2023-03-26 00:13:34.957714 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/token.meta.json
--rw-r--r--   0        0        0    32194 2023-03-26 00:13:34.701622 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/utils.data.json
--rw-r--r--   0        0        0     1792 2023-03-26 00:13:34.702039 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/markdown_it/utils.meta.json
--rw-r--r--   0        0        0     7022 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/marshal.data.json
--rw-r--r--   0        0        0     1817 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/marshal.meta.json
--rw-r--r--   0        0        0    56212 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/math.data.json
--rw-r--r--   0        0        0     1770 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/math.meta.json
--rw-r--r--   0        0        0     3581 2023-03-26 00:13:35.031927 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/mdurl/__init__.data.json
--rw-r--r--   0        0        0     1789 2023-03-26 00:13:35.032492 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/mdurl/__init__.meta.json
--rw-r--r--   0        0        0     5037 2023-03-26 00:13:34.696335 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/mdurl/_decode.data.json
--rw-r--r--   0        0        0     1887 2023-03-26 00:13:34.696773 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/mdurl/_decode.meta.json
--rw-r--r--   0        0        0     4664 2023-03-26 00:13:34.691750 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/mdurl/_encode.data.json
--rw-r--r--   0        0        0     1809 2023-03-26 00:13:34.692113 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/mdurl/_encode.meta.json
--rw-r--r--   0        0        0     2420 2023-03-26 00:13:34.941038 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/mdurl/_format.data.json
--rw-r--r--   0        0        0     1720 2023-03-26 00:13:34.941544 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/mdurl/_format.meta.json
--rw-r--r--   0        0        0    13572 2023-03-26 00:13:34.938741 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/mdurl/_parse.data.json
--rw-r--r--   0        0        0     1902 2023-03-26 00:13:34.939219 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/mdurl/_parse.meta.json
--rw-r--r--   0        0        0    28653 2023-03-26 00:13:34.688064 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/mdurl/_url.data.json
--rw-r--r--   0        0        0     1693 2023-03-26 00:13:34.688461 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/mdurl/_url.meta.json
--rw-r--r--   0        0        0    16653 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/mimetypes.data.json
--rw-r--r--   0        0        0     1765 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/mimetypes.meta.json
--rw-r--r--   0        0        0    29398 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1819 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0     1681 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/msvcrt.data.json
--rw-r--r--   0        0        0     1729 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/msvcrt.meta.json
--rw-r--r--   0        0        0    34101 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/__init__.data.json
--rw-r--r--   0        0        0     2174 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/__init__.meta.json
--rw-r--r--   0        0        0    33273 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/connection.data.json
--rw-r--r--   0        0        0     1929 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/connection.meta.json
--rw-r--r--   0        0        0   103632 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/context.data.json
--rw-r--r--   0        0        0     2338 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/context.meta.json
--rw-r--r--   0        0        0   160925 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/managers.data.json
--rw-r--r--   0        0        0     1971 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/managers.meta.json
--rw-r--r--   0        0        0    56174 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/pool.data.json
--rw-r--r--   0        0        0     1817 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/pool.meta.json
--rw-r--r--   0        0        0     9821 2023-03-26 00:13:35.045882 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/popen_fork.data.json
--rw-r--r--   0        0        0     1804 2023-03-26 00:13:35.046398 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/popen_fork.meta.json
--rw-r--r--   0        0        0     6245 2023-03-26 00:13:35.236763 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/popen_forkserver.data.json
--rw-r--r--   0        0        0     1846 2023-03-26 00:13:35.237096 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/popen_forkserver.meta.json
--rw-r--r--   0        0        0     6966 2023-03-26 00:13:35.235943 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/popen_spawn_posix.data.json
--rw-r--r--   0        0        0     1848 2023-03-26 00:13:35.236346 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/popen_spawn_posix.meta.json
--rw-r--r--   0        0        0     2174 2023-03-26 00:13:35.043965 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/popen_spawn_win32.data.json
--rw-r--r--   0        0        0     1818 2023-03-26 00:13:35.044410 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/popen_spawn_win32.meta.json
--rw-r--r--   0        0        0    19244 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/process.data.json
--rw-r--r--   0        0        0     1781 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/process.meta.json
--rw-r--r--   0        0        0    21490 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/queues.data.json
--rw-r--r--   0        0        0     1785 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/queues.meta.json
--rw-r--r--   0        0        0    31446 2023-03-26 00:13:35.234761 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/reduction.data.json
--rw-r--r--   0        0        0     1991 2023-03-26 00:13:35.235355 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/reduction.meta.json
--rw-r--r--   0        0        0    31858 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/shared_memory.data.json
--rw-r--r--   0        0        0     1835 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/shared_memory.meta.json
--rw-r--r--   0        0        0    73307 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/sharedctypes.data.json
--rw-r--r--   0        0        0     1906 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/sharedctypes.meta.json
--rw-r--r--   0        0        0    10733 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/spawn.data.json
--rw-r--r--   0        0        0     1757 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/spawn.meta.json
--rw-r--r--   0        0        0    27930 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/synchronize.data.json
--rw-r--r--   0        0        0     1871 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/synchronize.meta.json
--rw-r--r--   0        0        0    25680 2023-03-26 00:13:34.959930 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/util.data.json
--rw-r--r--   0        0        0     1889 2023-03-26 00:13:34.960296 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/multiprocessing/util.meta.json
--rw-r--r--   0        0        0    86302 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numbers.data.json
--rw-r--r--   0        0        0     1689 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numbers.meta.json
--rw-r--r--   0        0        0  2421905 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/__init__.data.json
--rw-r--r--   0        0        0     3371 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/__init__.meta.json
--rw-r--r--   0        0        0     5414 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_pytesttester.data.json
--rw-r--r--   0        0        0     1717 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_pytesttester.meta.json
--rw-r--r--   0        0        0    22920 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/__init__.data.json
--rw-r--r--   0        0        0     2096 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/__init__.meta.json
--rw-r--r--   0        0        0     4030 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_add_docstring.data.json
--rw-r--r--   0        0        0     1876 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_add_docstring.meta.json
--rw-r--r--   0        0        0    27511 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_array_like.data.json
--rw-r--r--   0        0        0     1867 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_array_like.meta.json
--rw-r--r--   0        0        0   282284 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_callable.data.json
--rw-r--r--   0        0        0     1907 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_callable.meta.json
--rw-r--r--   0        0        0    45448 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_char_codes.data.json
--rw-r--r--   0        0        0     1704 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_char_codes.meta.json
--rw-r--r--   0        0        0    33086 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_dtype_like.data.json
--rw-r--r--   0        0        0     1855 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_dtype_like.meta.json
--rw-r--r--   0        0        0     6267 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_extended_precision.data.json
--rw-r--r--   0        0        0     1761 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_extended_precision.meta.json
--rw-r--r--   0        0        0    37579 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_generic_alias.data.json
--rw-r--r--   0        0        0     1906 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_generic_alias.meta.json
--rw-r--r--   0        0        0     4798 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_nbit.data.json
--rw-r--r--   0        0        0     1691 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_nbit.meta.json
--rw-r--r--   0        0        0    18116 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_nested_sequence.data.json
--rw-r--r--   0        0        0     1762 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_nested_sequence.meta.json
--rw-r--r--   0        0        0     6416 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_scalars.data.json
--rw-r--r--   0        0        0     1713 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_scalars.meta.json
--rw-r--r--   0        0        0     2539 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_shape.data.json
--rw-r--r--   0        0        0     1693 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_shape.meta.json
--rw-r--r--   0        0        0   283387 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_ufunc.data.json
--rw-r--r--   0        0        0     1913 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_typing/_ufunc.meta.json
--rw-r--r--   0        0        0     2043 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_version.data.json
--rw-r--r--   0        0        0     1720 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/_version.meta.json
--rw-r--r--   0        0        0     5478 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/compat/__init__.data.json
--rw-r--r--   0        0        0     1747 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/compat/__init__.meta.json
--rw-r--r--   0        0        0     6378 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/compat/_inspect.data.json
--rw-r--r--   0        0        0     1806 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/compat/_inspect.meta.json
--rw-r--r--   0        0        0    12882 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/compat/py3k.data.json
--rw-r--r--   0        0        0     1973 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/compat/py3k.meta.json
--rw-r--r--   0        0        0     1680 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/__init__.data.json
--rw-r--r--   0        0        0     1684 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/__init__.meta.json
--rw-r--r--   0        0        0    14899 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/_asarray.data.json
--rw-r--r--   0        0        0     1828 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/_asarray.meta.json
--rw-r--r--   0        0        0    23856 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/_internal.data.json
--rw-r--r--   0        0        0     1752 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/_internal.meta.json
--rw-r--r--   0        0        0     5260 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/_type_aliases.data.json
--rw-r--r--   0        0        0     1717 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json
--rw-r--r--   0        0        0    12223 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json
--rw-r--r--   0        0        0     1743 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json
--rw-r--r--   0        0        0    30585 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/arrayprint.data.json
--rw-r--r--   0        0        0     1796 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/arrayprint.meta.json
--rw-r--r--   0        0        0   184203 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/defchararray.data.json
--rw-r--r--   0        0        0     1849 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/defchararray.meta.json
--rw-r--r--   0        0        0    39308 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/einsumfunc.data.json
--rw-r--r--   0        0        0     1874 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json
--rw-r--r--   0        0        0   361315 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/fromnumeric.data.json
--rw-r--r--   0        0        0     1896 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json
--rw-r--r--   0        0        0    53986 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/function_base.data.json
--rw-r--r--   0        0        0     1855 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/function_base.meta.json
--rw-r--r--   0        0        0   328547 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/multiarray.data.json
--rw-r--r--   0        0        0     1954 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/multiarray.meta.json
--rw-r--r--   0        0        0   214165 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/numeric.data.json
--rw-r--r--   0        0        0     1898 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/numeric.meta.json
--rw-r--r--   0        0        0    49786 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/numerictypes.data.json
--rw-r--r--   0        0        0     1964 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/numerictypes.meta.json
--rw-r--r--   0        0        0    27436 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/overrides.data.json
--rw-r--r--   0        0        0     1969 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/overrides.meta.json
--rw-r--r--   0        0        0    57493 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/records.data.json
--rw-r--r--   0        0        0     1913 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/records.meta.json
--rw-r--r--   0        0        0    57514 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/shape_base.data.json
--rw-r--r--   0        0        0     1873 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/shape_base.meta.json
--rw-r--r--   0        0        0     3341 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/umath.data.json
--rw-r--r--   0        0        0     1744 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/core/umath.meta.json
--rw-r--r--   0        0        0   122428 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/ctypeslib.data.json
--rw-r--r--   0        0        0     1990 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/ctypeslib.meta.json
--rw-r--r--   0        0        0     4677 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/fft/__init__.data.json
--rw-r--r--   0        0        0     1768 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/fft/__init__.meta.json
--rw-r--r--   0        0        0    20509 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json
--rw-r--r--   0        0        0     1835 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json
--rw-r--r--   0        0        0    23676 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/fft/helper.data.json
--rw-r--r--   0        0        0     1802 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/fft/helper.meta.json
--rw-r--r--   0        0        0    26198 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/__init__.data.json
--rw-r--r--   0        0        0     2402 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/__init__.meta.json
--rw-r--r--   0        0        0     9746 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/_version.data.json
--rw-r--r--   0        0        0     1691 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/_version.meta.json
--rw-r--r--   0        0        0    19706 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/arraypad.data.json
--rw-r--r--   0        0        0     1807 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/arraypad.meta.json
--rw-r--r--   0        0        0   168368 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/arraysetops.data.json
--rw-r--r--   0        0        0     1813 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json
--rw-r--r--   0        0        0    28208 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/arrayterator.data.json
--rw-r--r--   0        0        0     1799 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json
--rw-r--r--   0        0        0     7697 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/format.data.json
--rw-r--r--   0        0        0     1686 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/format.meta.json
--rw-r--r--   0        0        0   244009 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/function_base.data.json
--rw-r--r--   0        0        0     2008 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/function_base.meta.json
--rw-r--r--   0        0        0     9712 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/histograms.data.json
--rw-r--r--   0        0        0     1819 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/histograms.meta.json
--rw-r--r--   0        0        0    69132 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/index_tricks.data.json
--rw-r--r--   0        0        0     1909 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json
--rw-r--r--   0        0        0    51587 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/mixins.data.json
--rw-r--r--   0        0        0     1701 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/mixins.meta.json
--rw-r--r--   0        0        0    97165 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json
--rw-r--r--   0        0        0     1923 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json
--rw-r--r--   0        0        0   105441 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/npyio.data.json
--rw-r--r--   0        0        0     2039 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/npyio.meta.json
--rw-r--r--   0        0        0   105129 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/polynomial.data.json
--rw-r--r--   0        0        0     1812 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/polynomial.meta.json
--rw-r--r--   0        0        0    67786 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/scimath.data.json
--rw-r--r--   0        0        0     1804 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/scimath.meta.json
--rw-r--r--   0        0        0    96870 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/shape_base.data.json
--rw-r--r--   0        0        0     1925 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/shape_base.meta.json
--rw-r--r--   0        0        0    25590 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json
--rw-r--r--   0        0        0     1841 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json
--rw-r--r--   0        0        0    83910 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/twodim_base.data.json
--rw-r--r--   0        0        0     1874 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json
--rw-r--r--   0        0        0   106065 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/type_check.data.json
--rw-r--r--   0        0        0     1873 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/type_check.meta.json
--rw-r--r--   0        0        0    27144 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/ufunclike.data.json
--rw-r--r--   0        0        0     1808 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json
--rw-r--r--   0        0        0    28586 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/utils.data.json
--rw-r--r--   0        0        0     1788 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/lib/utils.meta.json
--rw-r--r--   0        0        0     5785 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/linalg/__init__.data.json
--rw-r--r--   0        0        0     1747 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/linalg/__init__.meta.json
--rw-r--r--   0        0        0   117226 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/linalg/linalg.data.json
--rw-r--r--   0        0        0     1858 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/linalg/linalg.meta.json
--rw-r--r--   0        0        0    29906 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/ma/__init__.data.json
--rw-r--r--   0        0        0     1758 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/ma/__init__.meta.json
--rw-r--r--   0        0        0   148307 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/ma/core.data.json
--rw-r--r--   0        0        0     1780 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/ma/core.meta.json
--rw-r--r--   0        0        0    25456 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/ma/extras.data.json
--rw-r--r--   0        0        0     1760 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/ma/extras.meta.json
--rw-r--r--   0        0        0    15603 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/ma/mrecords.data.json
--rw-r--r--   0        0        0     1746 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/ma/mrecords.meta.json
--rw-r--r--   0        0        0     3019 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json
--rw-r--r--   0        0        0     1773 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json
--rw-r--r--   0        0        0     6757 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json
--rw-r--r--   0        0        0     1880 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json
--rw-r--r--   0        0        0     4444 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/polynomial/__init__.data.json
--rw-r--r--   0        0        0     1938 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json
--rw-r--r--   0        0        0    29448 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json
--rw-r--r--   0        0        0     1707 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json
--rw-r--r--   0        0        0    18024 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json
--rw-r--r--   0        0        0     1794 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json
--rw-r--r--   0        0        0    15533 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/polynomial/hermite.data.json
--rw-r--r--   0        0        0     1790 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json
--rw-r--r--   0        0        0    15586 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json
--rw-r--r--   0        0        0     1794 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json
--rw-r--r--   0        0        0    15361 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json
--rw-r--r--   0        0        0     1792 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json
--rw-r--r--   0        0        0    15361 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/polynomial/legendre.data.json
--rw-r--r--   0        0        0     1792 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json
--rw-r--r--   0        0        0    14340 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json
--rw-r--r--   0        0        0     1796 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json
--rw-r--r--   0        0        0     5080 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json
--rw-r--r--   0        0        0     1707 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json
--rw-r--r--   0        0        0    10596 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/random/__init__.data.json
--rw-r--r--   0        0        0     1939 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/random/__init__.meta.json
--rw-r--r--   0        0        0   275132 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/random/_generator.data.json
--rw-r--r--   0        0        0     1939 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/random/_generator.meta.json
--rw-r--r--   0        0        0    11488 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/random/_mt19937.data.json
--rw-r--r--   0        0        0     1847 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/random/_mt19937.meta.json
--rw-r--r--   0        0        0    16790 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/random/_pcg64.data.json
--rw-r--r--   0        0        0     1752 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/random/_pcg64.meta.json
--rw-r--r--   0        0        0    12381 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/random/_philox.data.json
--rw-r--r--   0        0        0     1845 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/random/_philox.meta.json
--rw-r--r--   0        0        0     9750 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/random/_sfc64.data.json
--rw-r--r--   0        0        0     1766 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/random/_sfc64.meta.json
--rw-r--r--   0        0        0    73561 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/random/bit_generator.data.json
--rw-r--r--   0        0        0     1904 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/random/bit_generator.meta.json
--rw-r--r--   0        0        0   351985 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/random/mtrand.data.json
--rw-r--r--   0        0        0     1908 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/random/mtrand.meta.json
--rw-r--r--   0        0        0     9368 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/testing/__init__.data.json
--rw-r--r--   0        0        0     1776 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/testing/__init__.meta.json
--rw-r--r--   0        0        0     1776 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json
--rw-r--r--   0        0        0     1705 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json
--rw-r--r--   0        0        0   124418 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/testing/_private/utils.data.json
--rw-r--r--   0        0        0     2086 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json
--rw-r--r--   0        0        0     3098 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/typing/__init__.data.json
--rw-r--r--   0        0        0     1784 2023-03-26 00:13:30.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/typing/__init__.meta.json
--rw-r--r--   0        0        0     3560 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/version.data.json
--rw-r--r--   0        0        0     1752 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/numpy/version.meta.json
--rw-r--r--   0        0        0     6700 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/opcode.data.json
--rw-r--r--   0        0        0     1750 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/opcode.meta.json
--rw-r--r--   0        0        0    51076 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/operator.data.json
--rw-r--r--   0        0        0     1774 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/operator.meta.json
--rw-r--r--   0        0        0   351910 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1934 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     5357 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1723 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0     3259 2023-03-24 00:33:08.332130 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/packaging/__about__.data.json
--rw-r--r--   0        0        0     1513 2023-03-24 00:33:08.332307 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/packaging/__about__.meta.json
--rw-r--r--   0        0        0     3503 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/packaging/__init__.data.json
--rw-r--r--   0        0        0     1681 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/packaging/__init__.meta.json
--rw-r--r--   0        0        0    15159 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/packaging/_structures.data.json
--rw-r--r--   0        0        0     1713 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/packaging/_structures.meta.json
--rw-r--r--   0        0        0    71022 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/packaging/version.data.json
--rw-r--r--   0        0        0     1924 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/packaging/version.meta.json
--rw-r--r--   0        0        0    96612 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1885 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    48578 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1821 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    30250 2023-03-24 00:33:08.234375 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/pkgutil.data.json
--rw-r--r--   0        0        0     1587 2023-03-24 00:33:08.234588 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/pkgutil.meta.json
--rw-r--r--   0        0        0    38194 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/platform.data.json
--rw-r--r--   0        0        0     1726 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/platform.meta.json
--rw-r--r--   0        0        0    82146 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1815 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0     8260 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/pty.data.json
--rw-r--r--   0        0        0     1748 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/pty.meta.json
--rw-r--r--   0        0        0   113333 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/pydoc.data.json
--rw-r--r--   0        0        0     1803 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/pydoc.meta.json
--rw-r--r--   0        0        0    33319 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/queue.data.json
--rw-r--r--   0        0        0     1754 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/queue.meta.json
--rw-r--r--   0        0        0    45145 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/random.data.json
--rw-r--r--   0        0        0     1801 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/random.meta.json
--rw-r--r--   0        0        0   182959 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1907 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    18010 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/reprlib.data.json
--rw-r--r--   0        0        0     1778 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/reprlib.meta.json
--rw-r--r--   0        0        0     9126 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/__init__.data.json
--rw-r--r--   0        0        0     1863 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/__init__.meta.json
--rw-r--r--   0        0        0     8318 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/__main__.data.json
--rw-r--r--   0        0        0     2154 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/__main__.meta.json
--rw-r--r--   0        0        0     1948 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_cell_widths.data.json
--rw-r--r--   0        0        0     1690 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_cell_widths.meta.json
--rw-r--r--   0        0        0     1759 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_emoji_codes.data.json
--rw-r--r--   0        0        0     1691 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_emoji_codes.meta.json
--rw-r--r--   0        0        0     4481 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_emoji_replace.data.json
--rw-r--r--   0        0        0     1747 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_emoji_replace.meta.json
--rw-r--r--   0        0        0     2539 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_export_format.data.json
--rw-r--r--   0        0        0     1693 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_export_format.meta.json
--rw-r--r--   0        0        0     2306 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_extension.data.json
--rw-r--r--   0        0        0     1769 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_extension.meta.json
--rw-r--r--   0        0        0     2488 2023-03-26 00:13:34.787247 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_fileno.data.json
--rw-r--r--   0        0        0     1697 2023-03-26 00:13:34.787510 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_fileno.meta.json
--rw-r--r--   0        0        0    15312 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_inspect.data.json
--rw-r--r--   0        0        0     2047 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_inspect.meta.json
--rw-r--r--   0        0        0     8941 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_log_render.data.json
--rw-r--r--   0        0        0     1877 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_log_render.meta.json
--rw-r--r--   0        0        0     6328 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_loop.data.json
--rw-r--r--   0        0        0     1694 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_loop.meta.json
--rw-r--r--   0        0        0    16768 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_null_file.data.json
--rw-r--r--   0        0        0     1719 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_null_file.meta.json
--rw-r--r--   0        0        0     2290 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_palettes.data.json
--rw-r--r--   0        0        0     1705 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_palettes.meta.json
--rw-r--r--   0        0        0     2212 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_pick.data.json
--rw-r--r--   0        0        0     1673 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_pick.meta.json
--rw-r--r--   0        0        0    10962 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_ratio.data.json
--rw-r--r--   0        0        0     1831 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_ratio.meta.json
--rw-r--r--   0        0        0     1826 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_spinners.data.json
--rw-r--r--   0        0        0     1684 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_spinners.meta.json
--rw-r--r--   0        0        0     6122 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_stack.data.json
--rw-r--r--   0        0        0     1675 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_stack.meta.json
--rw-r--r--   0        0        0     3088 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_timer.data.json
--rw-r--r--   0        0        0     1730 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_timer.meta.json
--rw-r--r--   0        0        0    57564 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_win32_console.data.json
--rw-r--r--   0        0        0     1992 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_win32_console.meta.json
--rw-r--r--   0        0        0     7305 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_windows.data.json
--rw-r--r--   0        0        0     1798 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_windows.meta.json
--rw-r--r--   0        0        0     3297 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_windows_renderer.data.json
--rw-r--r--   0        0        0     1785 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_windows_renderer.meta.json
--rw-r--r--   0        0        0     4369 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_wrap.data.json
--rw-r--r--   0        0        0     1889 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/_wrap.meta.json
--rw-r--r--   0        0        0     4896 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/abc.data.json
--rw-r--r--   0        0        0     1769 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/abc.meta.json
--rw-r--r--   0        0        0    24794 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/align.data.json
--rw-r--r--   0        0        0     2038 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/align.meta.json
--rw-r--r--   0        0        0    26527 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/ansi.data.json
--rw-r--r--   0        0        0     2118 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/ansi.meta.json
--rw-r--r--   0        0        0    21994 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/box.data.json
--rw-r--r--   0        0        0     1954 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/box.meta.json
--rw-r--r--   0        0        0     9223 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/cells.data.json
--rw-r--r--   0        0        0     1796 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/cells.meta.json
--rw-r--r--   0        0        0    58324 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/color.data.json
--rw-r--r--   0        0        0     2194 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/color.meta.json
--rw-r--r--   0        0        0    21961 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/color_triplet.data.json
--rw-r--r--   0        0        0     1690 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/color_triplet.meta.json
--rw-r--r--   0        0        0    11070 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/columns.data.json
--rw-r--r--   0        0        0     2182 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/columns.meta.json
--rw-r--r--   0        0        0   186847 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/console.data.json
--rw-r--r--   0        0        0     3053 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/console.meta.json
--rw-r--r--   0        0        0     6278 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/constrain.data.json
--rw-r--r--   0        0        0     1828 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/constrain.meta.json
--rw-r--r--   0        0        0    21205 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/containers.data.json
--rw-r--r--   0        0        0     1884 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/containers.meta.json
--rw-r--r--   0        0        0    23721 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/control.data.json
--rw-r--r--   0        0        0     1936 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/control.meta.json
--rw-r--r--   0        0        0     3941 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/default_styles.data.json
--rw-r--r--   0        0        0     2104 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/default_styles.meta.json
--rw-r--r--   0        0        0    11474 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/emoji.data.json
--rw-r--r--   0        0        0     2019 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/emoji.meta.json
--rw-r--r--   0        0        0     8738 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/errors.data.json
--rw-r--r--   0        0        0     1676 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/errors.meta.json
--rw-r--r--   0        0        0     9182 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/file_proxy.data.json
--rw-r--r--   0        0        0     1911 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/file_proxy.meta.json
--rw-r--r--   0        0        0    15677 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/highlighter.data.json
--rw-r--r--   0        0        0     1961 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/highlighter.meta.json
--rw-r--r--   0        0        0    10567 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/json.data.json
--rw-r--r--   0        0        0     2065 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/json.meta.json
--rw-r--r--   0        0        0    10569 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/jupyter.data.json
--rw-r--r--   0        0        0     1902 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/jupyter.meta.json
--rw-r--r--   0        0        0    29952 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/live.data.json
--rw-r--r--   0        0        0     2404 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/live.meta.json
--rw-r--r--   0        0        0     9724 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/live_render.data.json
--rw-r--r--   0        0        0     1889 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/live_render.meta.json
--rw-r--r--   0        0        0    70924 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/markdown.data.json
--rw-r--r--   0        0        0     2386 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/markdown.meta.json
--rw-r--r--   0        0        0    27131 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/markup.data.json
--rw-r--r--   0        0        0     2182 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/markup.meta.json
--rw-r--r--   0        0        0    24993 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/measure.data.json
--rw-r--r--   0        0        0     1964 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/measure.meta.json
--rw-r--r--   0        0        0    13387 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/padding.data.json
--rw-r--r--   0        0        0     1951 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/padding.meta.json
--rw-r--r--   0        0        0     6426 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/pager.data.json
--rw-r--r--   0        0        0     1860 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/pager.meta.json
--rw-r--r--   0        0        0     9629 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/palette.data.json
--rw-r--r--   0        0        0     2099 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/palette.meta.json
--rw-r--r--   0        0        0    18465 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/panel.data.json
--rw-r--r--   0        0        0     2069 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/panel.meta.json
--rw-r--r--   0        0        0   119636 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/pretty.data.json
--rw-r--r--   0        0        0     2275 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/pretty.meta.json
--rw-r--r--   0        0        0     3686 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/protocol.data.json
--rw-r--r--   0        0        0     1801 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/protocol.meta.json
--rw-r--r--   0        0        0    16692 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/region.data.json
--rw-r--r--   0        0        0     1675 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/region.meta.json
--rw-r--r--   0        0        0    21469 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/repr.data.json
--rw-r--r--   0        0        0     1868 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/repr.meta.json
--rw-r--r--   0        0        0     9054 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/rule.data.json
--rw-r--r--   0        0        0     1937 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/rule.meta.json
--rw-r--r--   0        0        0     4556 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/scope.data.json
--rw-r--r--   0        0        0     1955 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/scope.meta.json
--rw-r--r--   0        0        0     5794 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/screen.data.json
--rw-r--r--   0        0        0     1776 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/screen.meta.json
--rw-r--r--   0        0        0   104321 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/segment.data.json
--rw-r--r--   0        0        0     2104 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/segment.meta.json
--rw-r--r--   0        0        0    10929 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/spinner.data.json
--rw-r--r--   0        0        0     2089 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/spinner.meta.json
--rw-r--r--   0        0        0    13397 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/status.data.json
--rw-r--r--   0        0        0     1872 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/status.meta.json
--rw-r--r--   0        0        0    59267 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/style.data.json
--rw-r--r--   0        0        0     2047 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/style.meta.json
--rw-r--r--   0        0        0     6501 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/styled.data.json
--rw-r--r--   0        0        0     1876 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/styled.meta.json
--rw-r--r--   0        0        0    80766 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/syntax.data.json
--rw-r--r--   0        0        0     2467 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/syntax.meta.json
--rw-r--r--   0        0        0    82010 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/table.data.json
--rw-r--r--   0        0        0     2326 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/table.meta.json
--rw-r--r--   0        0        0     6941 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/terminal_theme.data.json
--rw-r--r--   0        0        0     1742 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/terminal_theme.meta.json
--rw-r--r--   0        0        0    93178 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/text.data.json
--rw-r--r--   0        0        0     2352 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/text.meta.json
--rw-r--r--   0        0        0    15049 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/theme.data.json
--rw-r--r--   0        0        0     1935 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/theme.meta.json
--rw-r--r--   0        0        0     1847 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/themes.data.json
--rw-r--r--   0        0        0     1746 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/themes.meta.json
--rw-r--r--   0        0        0    51566 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/traceback.data.json
--rw-r--r--   0        0        0     2448 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/rich/traceback.meta.json
--rw-r--r--   0        0        0     9600 2023-03-24 00:33:08.232672 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/runpy.data.json
--rw-r--r--   0        0        0     1540 2023-03-24 00:33:08.232853 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/runpy.meta.json
--rw-r--r--   0        0        0     7090 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/secrets.data.json
--rw-r--r--   0        0        0     1738 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/secrets.meta.json
--rw-r--r--   0        0        0    26327 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/select.data.json
--rw-r--r--   0        0        0     1788 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/select.meta.json
--rw-r--r--   0        0        0    60552 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/selectors.data.json
--rw-r--r--   0        0        0     1843 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/selectors.meta.json
--rw-r--r--   0        0        0    17828 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/shlex.data.json
--rw-r--r--   0        0        0     1772 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/shlex.meta.json
--rw-r--r--   0        0        0    77642 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/shutil.data.json
--rw-r--r--   0        0        0     1786 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/shutil.meta.json
--rw-r--r--   0        0        0    34601 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/signal.data.json
--rw-r--r--   0        0        0     1802 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/signal.meta.json
--rw-r--r--   0        0        0    88591 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/socket.data.json
--rw-r--r--   0        0        0     1894 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/socket.meta.json
--rw-r--r--   0        0        0    15241 2023-03-26 00:13:29.482092 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1751 2023-03-26 00:13:29.483122 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    30295 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1763 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    53745 2023-03-26 00:13:29.479485 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1815 2023-03-26 00:13:29.480046 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0   204523 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/ssl.data.json
--rw-r--r--   0        0        0     1896 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/ssl.meta.json
--rw-r--r--   0        0        0     7131 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/stat.data.json
--rw-r--r--   0        0        0     1698 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/stat.meta.json
--rw-r--r--   0        0        0   114247 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/__init__.data.json
--rw-r--r--   0        0        0     4548 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/__init__.meta.json
--rw-r--r--   0        0        0    38223 2023-03-24 00:33:11.235567 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/app_session.data.json
--rw-r--r--   0        0        0     2871 2023-03-24 00:33:11.236153 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/app_session.meta.json
--rw-r--r--   0        0        0     6267 2023-03-24 00:33:11.184072 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/beta_util.data.json
--rw-r--r--   0        0        0     3342 2023-03-24 00:33:11.184298 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/beta_util.meta.json
--rw-r--r--   0        0        0     5147 2023-03-24 00:33:11.196584 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/caching/__init__.data.json
--rw-r--r--   0        0        0     3441 2023-03-24 00:33:11.196842 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/caching/__init__.meta.json
--rw-r--r--   0        0        0    12287 2023-03-24 00:33:11.161229 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/caching/cache_errors.data.json
--rw-r--r--   0        0        0     1648 2023-03-24 00:33:11.161484 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/caching/cache_errors.meta.json
--rw-r--r--   0        0        0    25111 2023-03-24 00:33:11.183505 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/caching/cache_utils.data.json
--rw-r--r--   0        0        0     3717 2023-03-24 00:33:11.183755 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/caching/cache_utils.meta.json
--rw-r--r--   0        0        0    19603 2023-03-24 00:33:11.175281 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/caching/hashing.data.json
--rw-r--r--   0        0        0     2384 2023-03-24 00:33:11.175553 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/caching/hashing.meta.json
--rw-r--r--   0        0        0    50384 2023-03-24 00:33:11.193544 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/caching/memo_decorator.data.json
--rw-r--r--   0        0        0     2027 2023-03-24 00:33:11.193781 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/caching/memo_decorator.meta.json
--rw-r--r--   0        0        0    38434 2023-03-24 00:33:11.192508 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/caching/singleton_decorator.data.json
--rw-r--r--   0        0        0     1798 2023-03-24 00:33:11.192767 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/caching/singleton_decorator.meta.json
--rw-r--r--   0        0        0     2885 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/case_converters.data.json
--rw-r--r--   0        0        0     1819 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/case_converters.meta.json
--rw-r--r--   0        0        0     2185 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/code_util.data.json
--rw-r--r--   0        0        0     1787 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/code_util.meta.json
--rw-r--r--   0        0        0     1744 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/commands/__init__.data.json
--rw-r--r--   0        0        0     1699 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/commands/__init__.meta.json
--rw-r--r--   0        0        0     3562 2023-03-26 00:13:37.420195 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/commands/execution_control.data.json
--rw-r--r--   0        0        0     1968 2023-03-26 00:13:37.420613 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/commands/execution_control.meta.json
--rw-r--r--   0        0        0    16913 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/commands/page_config.data.json
--rw-r--r--   0        0        0     2353 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/commands/page_config.meta.json
--rw-r--r--   0        0        0     7357 2023-03-26 00:13:37.423152 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/commands/query_params.data.json
--rw-r--r--   0        0        0     2044 2023-03-26 00:13:37.423532 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/commands/query_params.meta.json
--rw-r--r--   0        0        0     1357 2023-03-24 00:33:08.290021 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/components/__init__.data.json
--rw-r--r--   0        0        0     1493 2023-03-24 00:33:08.290207 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/components/__init__.meta.json
--rw-r--r--   0        0        0     3250 2023-03-24 00:33:11.233959 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/components/v1/__init__.data.json
--rw-r--r--   0        0        0     3345 2023-03-24 00:33:11.234486 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/components/v1/__init__.meta.json
--rw-r--r--   0        0        0     6382 2023-03-24 00:33:11.224336 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/components/v1/component_arrow.data.json
--rw-r--r--   0        0        0     1746 2023-03-24 00:33:11.225051 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/components/v1/component_arrow.meta.json
--rw-r--r--   0        0        0    27360 2023-03-24 00:33:11.233213 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/components/v1/components.data.json
--rw-r--r--   0        0        0     4180 2023-03-24 00:33:11.233587 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/components/v1/components.meta.json
--rw-r--r--   0        0        0    29269 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/config.data.json
--rw-r--r--   0        0        0     2263 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/config.meta.json
--rw-r--r--   0        0        0    15521 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/config_option.data.json
--rw-r--r--   0        0        0     2021 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/config_option.meta.json
--rw-r--r--   0        0        0     4578 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/config_util.data.json
--rw-r--r--   0        0        0     1862 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/config_util.meta.json
--rw-r--r--   0        0        0    28996 2023-03-24 00:33:11.229307 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/credentials.data.json
--rw-r--r--   0        0        0     1888 2023-03-24 00:33:11.230186 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/credentials.meta.json
--rw-r--r--   0        0        0    34252 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/cursor.data.json
--rw-r--r--   0        0        0     1863 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/cursor.meta.json
--rw-r--r--   0        0        0    75557 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/delta_generator.data.json
--rw-r--r--   0        0        0     4519 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/delta_generator.meta.json
--rw-r--r--   0        0        0    16198 2023-03-26 00:13:37.381681 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/deprecation_util.data.json
--rw-r--r--   0        0        0     3713 2023-03-26 00:13:37.381997 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/deprecation_util.meta.json
--rw-r--r--   0        0        0     1767 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/development.data.json
--rw-r--r--   0        0        0     1696 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/development.meta.json
--rw-r--r--   0        0        0     5352 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/echo.data.json
--rw-r--r--   0        0        0     1914 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/echo.meta.json
--rw-r--r--   0        0        0     2339 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/__init__.data.json
--rw-r--r--   0        0        0     1700 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/__init__.meta.json
--rw-r--r--   0        0        0    12100 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/alert.data.json
--rw-r--r--   0        0        0     3738 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/alert.meta.json
--rw-r--r--   0        0        0    21585 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/arrow.data.json
--rw-r--r--   0        0        0     3970 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/arrow.meta.json
--rw-r--r--   0        0        0    26183 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/arrow_altair.data.json
--rw-r--r--   0        0        0     4067 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/arrow_altair.meta.json
--rw-r--r--   0        0        0    10690 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/arrow_vega_lite.data.json
--rw-r--r--   0        0        0     4056 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/arrow_vega_lite.meta.json
--rw-r--r--   0        0        0     5751 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/balloons.data.json
--rw-r--r--   0        0        0     3654 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/balloons.meta.json
--rw-r--r--   0        0        0     8407 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/bokeh_chart.data.json
--rw-r--r--   0        0        0     3844 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/bokeh_chart.meta.json
--rw-r--r--   0        0        0    23639 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/button.data.json
--rw-r--r--   0        0        0     4199 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/button.meta.json
--rw-r--r--   0        0        0    17690 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/camera_input.data.json
--rw-r--r--   0        0        0     4044 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/camera_input.meta.json
--rw-r--r--   0        0        0    16413 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/checkbox.data.json
--rw-r--r--   0        0        0     3902 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/checkbox.meta.json
--rw-r--r--   0        0        0    16942 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/color_picker.data.json
--rw-r--r--   0        0        0     4066 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/color_picker.meta.json
--rw-r--r--   0        0        0    47722 2023-03-26 00:13:37.432111 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/data_editor.data.json
--rw-r--r--   0        0        0     4323 2023-03-26 00:13:37.432887 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/data_editor.meta.json
--rw-r--r--   0        0        0    24938 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/dataframe_selector.data.json
--rw-r--r--   0        0        0     3676 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/dataframe_selector.meta.json
--rw-r--r--   0        0        0     9889 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/deck_gl_json_chart.data.json
--rw-r--r--   0        0        0     3790 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/deck_gl_json_chart.meta.json
--rw-r--r--   0        0        0     9550 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/doc_string.data.json
--rw-r--r--   0        0        0     3836 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/doc_string.meta.json
--rw-r--r--   0        0        0     4812 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/empty.data.json
--rw-r--r--   0        0        0     3607 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/empty.meta.json
--rw-r--r--   0        0        0    12639 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/exception.data.json
--rw-r--r--   0        0        0     3913 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/exception.meta.json
--rw-r--r--   0        0        0    37030 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/file_uploader.data.json
--rw-r--r--   0        0        0     4203 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/file_uploader.meta.json
--rw-r--r--   0        0        0    28764 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/form.data.json
--rw-r--r--   0        0        0     3910 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/form.meta.json
--rw-r--r--   0        0        0     9193 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/graphviz_chart.data.json
--rw-r--r--   0        0        0     3935 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/graphviz_chart.meta.json
--rw-r--r--   0        0        0    10380 2023-03-26 00:13:37.401938 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/heading.data.json
--rw-r--r--   0        0        0     3714 2023-03-26 00:13:37.402350 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/heading.meta.json
--rw-r--r--   0        0        0     9416 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/iframe.data.json
--rw-r--r--   0        0        0     3650 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/iframe.meta.json
--rw-r--r--   0        0        0    27006 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/image.data.json
--rw-r--r--   0        0        0     4317 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/image.meta.json
--rw-r--r--   0        0        0     7184 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/json.data.json
--rw-r--r--   0        0        0     3871 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/json.meta.json
--rw-r--r--   0        0        0    14359 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/layouts.data.json
--rw-r--r--   0        0        0     3768 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/layouts.meta.json
--rw-r--r--   0        0        0    17515 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/legacy_altair.data.json
--rw-r--r--   0        0        0     4015 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/legacy_altair.meta.json
--rw-r--r--   0        0        0    37328 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/legacy_data_frame.data.json
--rw-r--r--   0        0        0     4210 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/legacy_data_frame.meta.json
--rw-r--r--   0        0        0     9896 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/legacy_vega_lite.data.json
--rw-r--r--   0        0        0     4027 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/legacy_vega_lite.meta.json
--rw-r--r--   0        0        0     1776 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/lib/__init__.data.json
--rw-r--r--   0        0        0     1707 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/lib/__init__.meta.json
--rw-r--r--   0        0        0     2482 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/lib/dicttools.data.json
--rw-r--r--   0        0        0     1755 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/lib/dicttools.meta.json
--rw-r--r--   0        0        0    13495 2023-03-26 00:13:34.547467 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/lib/streamlit_plotly_theme.data.json
--rw-r--r--   0        0        0     1814 2023-03-26 00:13:34.547859 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/lib/streamlit_plotly_theme.meta.json
--rw-r--r--   0        0        0    11719 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/map.data.json
--rw-r--r--   0        0        0     3985 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/map.meta.json
--rw-r--r--   0        0        0    11870 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/markdown.data.json
--rw-r--r--   0        0        0     3731 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/markdown.meta.json
--rw-r--r--   0        0        0    17601 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/media.data.json
--rw-r--r--   0        0        0     4282 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/media.meta.json
--rw-r--r--   0        0        0    17986 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/metric.data.json
--rw-r--r--   0        0        0     3961 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/metric.meta.json
--rw-r--r--   0        0        0    33284 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/multiselect.data.json
--rw-r--r--   0        0        0     4030 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/multiselect.meta.json
--rw-r--r--   0        0        0    20638 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/number_input.data.json
--rw-r--r--   0        0        0     4135 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/number_input.meta.json
--rw-r--r--   0        0        0    16593 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/plotly_chart.data.json
--rw-r--r--   0        0        0     4478 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/plotly_chart.meta.json
--rw-r--r--   0        0        0     7025 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/progress.data.json
--rw-r--r--   0        0        0     3801 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/progress.meta.json
--rw-r--r--   0        0        0    11709 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/pyplot.data.json
--rw-r--r--   0        0        0     4035 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/pyplot.meta.json
--rw-r--r--   0        0        0    23192 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/radio.data.json
--rw-r--r--   0        0        0     4077 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/radio.meta.json
--rw-r--r--   0        0        0    29955 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/select_slider.data.json
--rw-r--r--   0        0        0     4087 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/select_slider.meta.json
--rw-r--r--   0        0        0    23468 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/selectbox.data.json
--rw-r--r--   0        0        0     4085 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/selectbox.meta.json
--rw-r--r--   0        0        0     3425 2023-03-26 00:13:37.394260 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/show.data.json
--rw-r--r--   0        0        0     3731 2023-03-26 00:13:37.394655 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/show.meta.json
--rw-r--r--   0        0        0    34759 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/slider.data.json
--rw-r--r--   0        0        0     4238 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/slider.meta.json
--rw-r--r--   0        0        0     5567 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/snow.data.json
--rw-r--r--   0        0        0     3646 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/snow.meta.json
--rw-r--r--   0        0        0     3415 2023-03-26 00:13:37.422434 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/spinner.data.json
--rw-r--r--   0        0        0     3904 2023-03-26 00:13:37.422751 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/spinner.meta.json
--rw-r--r--   0        0        0     5858 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/text.data.json
--rw-r--r--   0        0        0     3709 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/text.meta.json
--rw-r--r--   0        0        0    28974 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/text_widgets.data.json
--rw-r--r--   0        0        0     4059 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/text_widgets.meta.json
--rw-r--r--   0        0        0    43633 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/time_widgets.data.json
--rw-r--r--   0        0        0     4055 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/time_widgets.meta.json
--rw-r--r--   0        0        0     7402 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/utils.data.json
--rw-r--r--   0        0        0     3804 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/utils.meta.json
--rw-r--r--   0        0        0     7967 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/write.data.json
--rw-r--r--   0        0        0     4137 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/elements/write.meta.json
--rw-r--r--   0        0        0     1749 2023-03-26 00:13:34.621890 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/emojis.data.json
--rw-r--r--   0        0        0     1688 2023-03-26 00:13:34.622285 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/emojis.meta.json
--rw-r--r--   0        0        0     3539 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/env_util.data.json
--rw-r--r--   0        0        0     1916 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/env_util.meta.json
--rw-r--r--   0        0        0     4816 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/error_util.data.json
--rw-r--r--   0        0        0     3998 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/error_util.meta.json
--rw-r--r--   0        0        0    14122 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/errors.data.json
--rw-r--r--   0        0        0     1790 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/errors.meta.json
--rw-r--r--   0        0        0    10558 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/file_util.data.json
--rw-r--r--   0        0        0     2019 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/file_util.meta.json
--rw-r--r--   0        0        0     4750 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/folder_black_list.data.json
--rw-r--r--   0        0        0     1829 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/folder_black_list.meta.json
--rw-r--r--   0        0        0    17523 2023-03-24 00:33:11.167304 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/forward_msg_cache.data.json
--rw-r--r--   0        0        0     1926 2023-03-24 00:33:11.167577 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/forward_msg_cache.meta.json
--rw-r--r--   0        0        0     9129 2023-03-24 00:33:11.167906 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/forward_msg_queue.data.json
--rw-r--r--   0        0        0     1716 2023-03-24 00:33:11.168291 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/forward_msg_queue.meta.json
--rw-r--r--   0        0        0    12587 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/git_util.data.json
--rw-r--r--   0        0        0     1877 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/git_util.meta.json
--rw-r--r--   0        0        0     1684 2023-03-24 00:33:11.230825 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/hello/Hello.data.json
--rw-r--r--   0        0        0     3432 2023-03-24 00:33:11.231328 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/hello/Hello.meta.json
--rw-r--r--   0        0        0     1322 2023-03-24 00:33:08.326679 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/hello/__init__.data.json
--rw-r--r--   0        0        0     1483 2023-03-24 00:33:08.326887 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/hello/__init__.meta.json
--rw-r--r--   0        0        0    25656 2023-03-24 00:33:11.169916 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/in_memory_file_manager.data.json
--rw-r--r--   0        0        0     1947 2023-03-24 00:33:11.170159 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/in_memory_file_manager.meta.json
--rw-r--r--   0        0        0     8447 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/js_number.data.json
--rw-r--r--   0        0        0     1821 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/js_number.meta.json
--rw-r--r--   0        0        0     1923 2023-03-24 00:33:11.197063 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/legacy_caching/__init__.data.json
--rw-r--r--   0        0        0     1544 2023-03-24 00:33:11.197278 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/legacy_caching/__init__.meta.json
--rw-r--r--   0        0        0    81624 2023-03-24 00:33:11.195463 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/legacy_caching/caching.data.json
--rw-r--r--   0        0        0     4084 2023-03-24 00:33:11.195710 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/legacy_caching/caching.meta.json
--rw-r--r--   0        0        0    67319 2023-03-24 00:33:11.177361 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/legacy_caching/hashing.data.json
--rw-r--r--   0        0        0     2600 2023-03-24 00:33:11.177632 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/legacy_caching/hashing.meta.json
--rw-r--r--   0        0        0     6303 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/logger.data.json
--rw-r--r--   0        0        0     1960 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/logger.meta.json
--rw-r--r--   0        0        0     3048 2023-03-24 00:33:08.740984 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/magic.data.json
--rw-r--r--   0        0        0     1571 2023-03-24 00:33:08.741375 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/magic.meta.json
--rw-r--r--   0        0        0     7174 2023-03-24 00:33:11.227597 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/metrics_util.data.json
--rw-r--r--   0        0        0     1631 2023-03-24 00:33:11.228235 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/metrics_util.meta.json
--rw-r--r--   0        0        0     5633 2023-03-24 00:33:11.166511 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/net_util.data.json
--rw-r--r--   0        0        0     1717 2023-03-24 00:33:11.166808 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/net_util.meta.json
--rw-r--r--   0        0        0     5266 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Alert_pb2.data.json
--rw-r--r--   0        0        0     1728 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Alert_pb2.meta.json
--rw-r--r--   0        0        0     4861 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/AppPage_pb2.data.json
--rw-r--r--   0        0        0     1732 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/AppPage_pb2.meta.json
--rw-r--r--   0        0        0     5318 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/ArrowNamedDataSet_pb2.data.json
--rw-r--r--   0        0        0     1816 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/ArrowNamedDataSet_pb2.meta.json
--rw-r--r--   0        0        0     5502 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/ArrowVegaLiteChart_pb2.data.json
--rw-r--r--   0        0        0     1867 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/ArrowVegaLiteChart_pb2.meta.json
--rw-r--r--   0        0        0     6184 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Arrow_pb2.data.json
--rw-r--r--   0        0        0     1728 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Arrow_pb2.meta.json
--rw-r--r--   0        0        0     4795 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Audio_pb2.data.json
--rw-r--r--   0        0        0     1728 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Audio_pb2.meta.json
--rw-r--r--   0        0        0     5000 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/BackMsg_pb2.data.json
--rw-r--r--   0        0        0     1802 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/BackMsg_pb2.meta.json
--rw-r--r--   0        0        0     4894 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Balloons_pb2.data.json
--rw-r--r--   0        0        0     1734 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Balloons_pb2.meta.json
--rw-r--r--   0        0        0     8125 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Block_pb2.data.json
--rw-r--r--   0        0        0     1822 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Block_pb2.meta.json
--rw-r--r--   0        0        0     4960 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/BokehChart_pb2.data.json
--rw-r--r--   0        0        0     1738 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/BokehChart_pb2.meta.json
--rw-r--r--   0        0        0     4828 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Button_pb2.data.json
--rw-r--r--   0        0        0     1730 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Button_pb2.meta.json
--rw-r--r--   0        0        0     5154 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/CameraInput_pb2.data.json
--rw-r--r--   0        0        0     1821 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/CameraInput_pb2.meta.json
--rw-r--r--   0        0        0     5055 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Checkbox_pb2.data.json
--rw-r--r--   0        0        0     1815 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Checkbox_pb2.meta.json
--rw-r--r--   0        0        0     5134 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/ClientState_pb2.data.json
--rw-r--r--   0        0        0     1811 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/ClientState_pb2.meta.json
--rw-r--r--   0        0        0     5154 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/ColorPicker_pb2.data.json
--rw-r--r--   0        0        0     1821 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/ColorPicker_pb2.meta.json
--rw-r--r--   0        0        0    11485 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Common_pb2.data.json
--rw-r--r--   0        0        0     1731 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Common_pb2.meta.json
--rw-r--r--   0        0        0     8890 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Components_pb2.data.json
--rw-r--r--   0        0        0     1739 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Components_pb2.meta.json
--rw-r--r--   0        0        0    18358 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/DataFrame_pb2.data.json
--rw-r--r--   0        0        0     1802 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/DataFrame_pb2.meta.json
--rw-r--r--   0        0        0     5088 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/DateInput_pb2.data.json
--rw-r--r--   0        0        0     1817 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/DateInput_pb2.meta.json
--rw-r--r--   0        0        0     5125 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/DeckGlJsonChart_pb2.data.json
--rw-r--r--   0        0        0     1748 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/DeckGlJsonChart_pb2.meta.json
--rw-r--r--   0        0        0     5345 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Delta_pb2.data.json
--rw-r--r--   0        0        0     1924 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Delta_pb2.meta.json
--rw-r--r--   0        0        0     4927 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/DocString_pb2.data.json
--rw-r--r--   0        0        0     1736 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/DocString_pb2.meta.json
--rw-r--r--   0        0        0     5092 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/DownloadButton_pb2.data.json
--rw-r--r--   0        0        0     1746 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/DownloadButton_pb2.meta.json
--rw-r--r--   0        0        0    10485 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Element_pb2.data.json
--rw-r--r--   0        0        0     3459 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Element_pb2.meta.json
--rw-r--r--   0        0        0     4795 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Empty_pb2.data.json
--rw-r--r--   0        0        0     1728 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Empty_pb2.meta.json
--rw-r--r--   0        0        0     4927 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Exception_pb2.data.json
--rw-r--r--   0        0        0     1736 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Exception_pb2.meta.json
--rw-r--r--   0        0        0     4861 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Favicon_pb2.data.json
--rw-r--r--   0        0        0     1732 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Favicon_pb2.meta.json
--rw-r--r--   0        0        0     5187 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/FileUploader_pb2.data.json
--rw-r--r--   0        0        0     1823 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/FileUploader_pb2.meta.json
--rw-r--r--   0        0        0     8895 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/ForwardMsg_pb2.data.json
--rw-r--r--   0        0        0     2186 2023-03-26 00:13:36.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/ForwardMsg_pb2.meta.json
--rw-r--r--   0        0        0     5353 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/GitInfo_pb2.data.json
--rw-r--r--   0        0        0     1732 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/GitInfo_pb2.meta.json
--rw-r--r--   0        0        0     5059 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/GraphVizChart_pb2.data.json
--rw-r--r--   0        0        0     1744 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/GraphVizChart_pb2.meta.json
--rw-r--r--   0        0        0     4861 2023-03-26 00:13:34.563723 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Heading_pb2.data.json
--rw-r--r--   0        0        0     1732 2023-03-26 00:13:34.564231 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Heading_pb2.meta.json
--rw-r--r--   0        0        0     4828 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/IFrame_pb2.data.json
--rw-r--r--   0        0        0     1823 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/IFrame_pb2.meta.json
--rw-r--r--   0        0        0     5716 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Image_pb2.data.json
--rw-r--r--   0        0        0     1728 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Image_pb2.meta.json
--rw-r--r--   0        0        0     4762 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Json_pb2.data.json
--rw-r--r--   0        0        0     1726 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Json_pb2.meta.json
--rw-r--r--   0        0        0     5977 2023-03-26 00:13:34.528173 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/LabelVisibilityMessage_pb2.data.json
--rw-r--r--   0        0        0     1762 2023-03-26 00:13:34.528567 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/LabelVisibilityMessage_pb2.meta.json
--rw-r--r--   0        0        0     5377 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Markdown_pb2.data.json
--rw-r--r--   0        0        0     1734 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Markdown_pb2.meta.json
--rw-r--r--   0        0        0     5985 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Metric_pb2.data.json
--rw-r--r--   0        0        0     1811 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Metric_pb2.meta.json
--rw-r--r--   0        0        0     5154 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/MultiSelect_pb2.data.json
--rw-r--r--   0        0        0     1821 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/MultiSelect_pb2.meta.json
--rw-r--r--   0        0        0     5161 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/NamedDataSet_pb2.data.json
--rw-r--r--   0        0        0     1810 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/NamedDataSet_pb2.meta.json
--rw-r--r--   0        0        0    11120 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/NewSession_pb2.data.json
--rw-r--r--   0        0        0     1850 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/NewSession_pb2.meta.json
--rw-r--r--   0        0        0     5667 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/NumberInput_pb2.data.json
--rw-r--r--   0        0        0     1915 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/NumberInput_pb2.meta.json
--rw-r--r--   0        0        0     6490 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/PageConfig_pb2.data.json
--rw-r--r--   0        0        0     1738 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/PageConfig_pb2.meta.json
--rw-r--r--   0        0        0     4894 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/PageInfo_pb2.data.json
--rw-r--r--   0        0        0     1734 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/PageInfo_pb2.meta.json
--rw-r--r--   0        0        0     5026 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/PageNotFound_pb2.data.json
--rw-r--r--   0        0        0     1742 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/PageNotFound_pb2.meta.json
--rw-r--r--   0        0        0     6889 2023-03-26 00:13:34.673552 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/PageProfile_pb2.data.json
--rw-r--r--   0        0        0     1741 2023-03-26 00:13:34.673892 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/PageProfile_pb2.meta.json
--rw-r--r--   0        0        0     5157 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/PagesChanged_pb2.data.json
--rw-r--r--   0        0        0     1808 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/PagesChanged_pb2.meta.json
--rw-r--r--   0        0        0     5932 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/PlotlyChart_pb2.data.json
--rw-r--r--   0        0        0     1740 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/PlotlyChart_pb2.meta.json
--rw-r--r--   0        0        0     4894 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Progress_pb2.data.json
--rw-r--r--   0        0        0     1734 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Progress_pb2.meta.json
--rw-r--r--   0        0        0     4956 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Radio_pb2.data.json
--rw-r--r--   0        0        0     1809 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Radio_pb2.meta.json
--rw-r--r--   0        0        0     5952 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/RootContainer_pb2.data.json
--rw-r--r--   0        0        0     1778 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/RootContainer_pb2.meta.json
--rw-r--r--   0        0        0     5088 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Selectbox_pb2.data.json
--rw-r--r--   0        0        0     1817 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Selectbox_pb2.meta.json
--rw-r--r--   0        0        0     5161 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/SessionEvent_pb2.data.json
--rw-r--r--   0        0        0     1810 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/SessionEvent_pb2.meta.json
--rw-r--r--   0        0        0     4491 2023-03-24 00:33:08.644534 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/SessionState_pb2.data.json
--rw-r--r--   0        0        0     1563 2023-03-24 00:33:08.644878 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/SessionState_pb2.meta.json
--rw-r--r--   0        0        0     5059 2023-03-26 00:13:34.629158 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/SessionStatus_pb2.data.json
--rw-r--r--   0        0        0     1744 2023-03-26 00:13:34.629557 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/SessionStatus_pb2.meta.json
--rw-r--r--   0        0        0     5943 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Slider_pb2.data.json
--rw-r--r--   0        0        0     1905 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Slider_pb2.meta.json
--rw-r--r--   0        0        0     4762 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Snow_pb2.data.json
--rw-r--r--   0        0        0     1726 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Snow_pb2.meta.json
--rw-r--r--   0        0        0     4861 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Spinner_pb2.data.json
--rw-r--r--   0        0        0     1732 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Spinner_pb2.meta.json
--rw-r--r--   0        0        0     5055 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/TextArea_pb2.data.json
--rw-r--r--   0        0        0     1815 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/TextArea_pb2.meta.json
--rw-r--r--   0        0        0     5577 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/TextInput_pb2.data.json
--rw-r--r--   0        0        0     1817 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/TextInput_pb2.meta.json
--rw-r--r--   0        0        0     4762 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Text_pb2.data.json
--rw-r--r--   0        0        0     1726 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Text_pb2.meta.json
--rw-r--r--   0        0        0     5088 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/TimeInput_pb2.data.json
--rw-r--r--   0        0        0     1817 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/TimeInput_pb2.meta.json
--rw-r--r--   0        0        0     5335 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/VegaLiteChart_pb2.data.json
--rw-r--r--   0        0        0     1856 2023-03-26 00:13:35.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/VegaLiteChart_pb2.meta.json
--rw-r--r--   0        0        0     5260 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Video_pb2.data.json
--rw-r--r--   0        0        0     1728 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/Video_pb2.meta.json
--rw-r--r--   0        0        0     6267 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/WidgetStates_pb2.data.json
--rw-r--r--   0        0        0     1943 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/WidgetStates_pb2.meta.json
--rw-r--r--   0        0        0     1720 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/__init__.data.json
--rw-r--r--   0        0        0     1693 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/__init__.meta.json
--rw-r--r--   0        0        0    23305 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/openmetrics_data_model_pb2.data.json
--rw-r--r--   0        0        0     1890 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/proto/openmetrics_data_model_pb2.meta.json
--rw-r--r--   0        0        0     3622 2023-03-26 00:13:37.475226 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/__init__.data.json
--rw-r--r--   0        0        0     1778 2023-03-26 00:13:37.475447 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/__init__.meta.json
--rw-r--r--   0        0        0    47947 2023-03-26 00:13:37.416393 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/app_session.data.json
--rw-r--r--   0        0        0     3440 2023-03-26 00:13:37.416722 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/app_session.meta.json
--rw-r--r--   0        0        0    11952 2023-03-26 00:13:37.470050 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/__init__.data.json
--rw-r--r--   0        0        0     3939 2023-03-26 00:13:37.470406 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/__init__.meta.json
--rw-r--r--   0        0        0    62627 2023-03-26 00:13:37.467437 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cache_data_api.data.json
--rw-r--r--   0        0        0     4580 2023-03-26 00:13:37.467777 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cache_data_api.meta.json
--rw-r--r--   0        0        0    20074 2023-03-26 00:13:37.393520 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cache_errors.data.json
--rw-r--r--   0        0        0     1889 2023-03-26 00:13:37.393840 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cache_errors.meta.json
--rw-r--r--   0        0        0    60641 2023-03-26 00:13:37.466040 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cache_resource_api.data.json
--rw-r--r--   0        0        0     4290 2023-03-26 00:13:37.466429 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cache_resource_api.meta.json
--rw-r--r--   0        0        0     4153 2023-03-26 00:13:34.647066 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cache_type.data.json
--rw-r--r--   0        0        0     1743 2023-03-26 00:13:34.647439 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cache_type.meta.json
--rw-r--r--   0        0        0    36688 2023-03-26 00:13:37.425161 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cache_utils.data.json
--rw-r--r--   0        0        0     2469 2023-03-26 00:13:37.425418 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cache_utils.meta.json
--rw-r--r--   0        0        0    60878 2023-03-26 00:13:37.414680 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cached_message_replay.data.json
--rw-r--r--   0        0        0     4502 2023-03-26 00:13:37.415002 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cached_message_replay.meta.json
--rw-r--r--   0        0        0    22736 2023-03-26 00:13:37.396721 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/hashing.data.json
--rw-r--r--   0        0        0     2646 2023-03-26 00:13:37.397214 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/hashing.meta.json
--rw-r--r--   0        0        0     2679 2023-03-26 00:13:35.004924 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/storage/__init__.data.json
--rw-r--r--   0        0        0     1797 2023-03-26 00:13:35.005393 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/storage/__init__.meta.json
--rw-r--r--   0        0        0    25069 2023-03-26 00:13:34.881357 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/storage/cache_storage_protocol.data.json
--rw-r--r--   0        0        0     1838 2023-03-26 00:13:34.881717 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/storage/cache_storage_protocol.meta.json
--rw-r--r--   0        0        0    11536 2023-03-26 00:13:37.397861 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/storage/dummy_cache_storage.data.json
--rw-r--r--   0        0        0     1925 2023-03-26 00:13:37.398299 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/storage/dummy_cache_storage.meta.json
--rw-r--r--   0        0        0    19726 2023-03-26 00:13:37.378167 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.data.json
--rw-r--r--   0        0        0     2203 2023-03-26 00:13:37.378498 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.meta.json
--rw-r--r--   0        0        0    32388 2023-03-26 00:13:37.355764 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/credentials.data.json
--rw-r--r--   0        0        0     2164 2023-03-26 00:13:37.356181 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/credentials.meta.json
--rw-r--r--   0        0        0    20508 2023-03-26 00:13:37.359680 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/forward_msg_cache.data.json
--rw-r--r--   0        0        0     2154 2023-03-26 00:13:37.360349 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/forward_msg_cache.meta.json
--rw-r--r--   0        0        0    10750 2023-03-26 00:13:37.345044 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/forward_msg_queue.data.json
--rw-r--r--   0        0        0     1911 2023-03-26 00:13:37.345464 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/forward_msg_queue.meta.json
--rw-r--r--   0        0        0     2426 2023-03-26 00:13:37.474663 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/legacy_caching/__init__.data.json
--rw-r--r--   0        0        0     1778 2023-03-26 00:13:37.474947 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/legacy_caching/__init__.meta.json
--rw-r--r--   0        0        0   110850 2023-03-26 00:13:37.472220 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/legacy_caching/caching.data.json
--rw-r--r--   0        0        0     4531 2023-03-26 00:13:37.472574 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/legacy_caching/caching.meta.json
--rw-r--r--   0        0        0    71781 2023-03-26 00:13:37.380485 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/legacy_caching/hashing.data.json
--rw-r--r--   0        0        0     2807 2023-03-26 00:13:37.380985 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/legacy_caching/hashing.meta.json
--rw-r--r--   0        0        0    17093 2023-03-26 00:13:37.346718 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/media_file_manager.data.json
--rw-r--r--   0        0        0     2043 2023-03-26 00:13:37.347131 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/media_file_manager.meta.json
--rw-r--r--   0        0        0    10898 2023-03-26 00:13:34.539053 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/media_file_storage.data.json
--rw-r--r--   0        0        0     1770 2023-03-26 00:13:34.539564 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/media_file_storage.meta.json
--rw-r--r--   0        0        0     8150 2023-03-26 00:13:37.436038 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/memory_session_storage.data.json
--rw-r--r--   0        0        0     1838 2023-03-26 00:13:37.436984 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/memory_session_storage.meta.json
--rw-r--r--   0        0        0    36631 2023-03-26 00:13:37.361370 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/metrics_util.data.json
--rw-r--r--   0        0        0     2411 2023-03-26 00:13:37.361930 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/metrics_util.meta.json
--rw-r--r--   0        0        0    77488 2023-03-26 00:13:37.473898 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/runtime.data.json
--rw-r--r--   0        0        0     3195 2023-03-26 00:13:37.474283 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/runtime.meta.json
--rw-r--r--   0        0        0     7560 2023-03-26 00:13:37.362673 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/runtime_util.data.json
--rw-r--r--   0        0        0     2061 2023-03-26 00:13:37.363439 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/runtime_util.meta.json
--rw-r--r--   0        0        0     7309 2023-03-26 00:13:34.537538 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/script_data.data.json
--rw-r--r--   0        0        0     1814 2023-03-26 00:13:34.537921 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/script_data.meta.json
--rw-r--r--   0        0        0     2995 2023-03-26 00:13:37.415328 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/scriptrunner/__init__.data.json
--rw-r--r--   0        0        0     1896 2023-03-26 00:13:37.415570 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/scriptrunner/__init__.meta.json
--rw-r--r--   0        0        0     4709 2023-03-26 00:13:34.816131 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/scriptrunner/magic.data.json
--rw-r--r--   0        0        0     1898 2023-03-26 00:13:34.816601 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/scriptrunner/magic.meta.json
--rw-r--r--   0        0        0    21983 2023-03-26 00:13:37.410985 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/scriptrunner/script_requests.data.json
--rw-r--r--   0        0        0     1924 2023-03-26 00:13:37.411314 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/scriptrunner/script_requests.meta.json
--rw-r--r--   0        0        0    27392 2023-03-26 00:13:37.411974 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/scriptrunner/script_run_context.data.json
--rw-r--r--   0        0        0     4113 2023-03-26 00:13:37.412362 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/scriptrunner/script_run_context.meta.json
--rw-r--r--   0        0        0    34061 2023-03-26 00:13:37.413129 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/scriptrunner/script_runner.data.json
--rw-r--r--   0        0        0     4846 2023-03-26 00:13:37.413544 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/scriptrunner/script_runner.meta.json
--rw-r--r--   0        0        0    32814 2023-03-26 00:13:37.395426 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/secrets.data.json
--rw-r--r--   0        0        0     3996 2023-03-26 00:13:37.395975 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/secrets.meta.json
--rw-r--r--   0        0        0    41402 2023-03-26 00:13:37.426412 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/session_manager.data.json
--rw-r--r--   0        0        0     1977 2023-03-26 00:13:37.426935 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/session_manager.meta.json
--rw-r--r--   0        0        0     3424 2023-03-26 00:13:37.409874 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/__init__.data.json
--rw-r--r--   0        0        0     1948 2023-03-26 00:13:37.410309 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/__init__.meta.json
--rw-r--r--   0        0        0    35149 2023-03-26 00:13:37.404119 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/common.data.json
--rw-r--r--   0        0        0     2628 2023-03-26 00:13:37.404509 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/common.meta.json
--rw-r--r--   0        0        0    16743 2023-03-26 00:13:37.408116 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/safe_session_state.data.json
--rw-r--r--   0        0        0     1892 2023-03-26 00:13:37.408556 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/safe_session_state.meta.json
--rw-r--r--   0        0        0    68877 2023-03-26 00:13:37.406818 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/session_state.data.json
--rw-r--r--   0        0        0     4324 2023-03-26 00:13:37.407274 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/session_state.meta.json
--rw-r--r--   0        0        0    16631 2023-03-26 00:13:37.409097 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/session_state_proxy.data.json
--rw-r--r--   0        0        0     2281 2023-03-26 00:13:37.409450 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/session_state_proxy.meta.json
--rw-r--r--   0        0        0    12465 2023-03-26 00:13:37.405151 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/widgets.data.json
--rw-r--r--   0        0        0     2280 2023-03-26 00:13:37.405603 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/widgets.meta.json
--rw-r--r--   0        0        0    25062 2023-03-26 00:13:34.878273 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/stats.data.json
--rw-r--r--   0        0        0     1782 2023-03-26 00:13:34.878954 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/stats.meta.json
--rw-r--r--   0        0        0    37701 2023-03-26 00:13:37.348080 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/uploaded_file_manager.data.json
--rw-r--r--   0        0        0     2019 2023-03-26 00:13:37.348361 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/uploaded_file_manager.meta.json
--rw-r--r--   0        0        0    15599 2023-03-26 00:13:37.434572 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/websocket_session_manager.data.json
--rw-r--r--   0        0        0     2143 2023-03-26 00:13:37.435379 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/runtime/websocket_session_manager.meta.json
--rw-r--r--   0        0        0     2462 2023-03-24 00:33:11.200361 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/scriptrunner/__init__.data.json
--rw-r--r--   0        0        0     1646 2023-03-24 00:33:11.200611 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/scriptrunner/__init__.meta.json
--rw-r--r--   0        0        0    28532 2023-03-24 00:33:11.198312 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/scriptrunner/script_requests.data.json
--rw-r--r--   0        0        0     1730 2023-03-24 00:33:11.198540 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/scriptrunner/script_requests.meta.json
--rw-r--r--   0        0        0    26413 2023-03-24 00:33:11.199038 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/scriptrunner/script_run_context.data.json
--rw-r--r--   0        0        0     3732 2023-03-24 00:33:11.199282 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/scriptrunner/script_run_context.meta.json
--rw-r--r--   0        0        0    32645 2023-03-24 00:33:11.199840 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/scriptrunner/script_runner.data.json
--rw-r--r--   0        0        0     4156 2023-03-24 00:33:11.200115 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/scriptrunner/script_runner.meta.json
--rw-r--r--   0        0        0    21735 2023-03-24 00:33:11.190414 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/secrets.data.json
--rw-r--r--   0        0        0     3682 2023-03-24 00:33:11.190603 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/secrets.meta.json
--rw-r--r--   0        0        0     1329 2023-03-24 00:33:08.330510 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/server/__init__.data.json
--rw-r--r--   0        0        0     1485 2023-03-24 00:33:08.330745 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/server/__init__.meta.json
--rw-r--r--   0        0        0    20265 2023-03-24 00:33:11.180646 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/server/routes.data.json
--rw-r--r--   0        0        0     1995 2023-03-24 00:33:11.180899 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/server/routes.meta.json
--rw-r--r--   0        0        0    49588 2023-03-24 00:33:11.237224 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/server/server.data.json
--rw-r--r--   0        0        0     3456 2023-03-24 00:33:11.237625 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/server/server.meta.json
--rw-r--r--   0        0        0    10330 2023-03-24 00:33:11.174487 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/server/server_util.data.json
--rw-r--r--   0        0        0     1865 2023-03-24 00:33:11.174765 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/server/server_util.meta.json
--rw-r--r--   0        0        0     8995 2023-03-24 00:33:11.231924 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/server/upload_file_request_handler.data.json
--rw-r--r--   0        0        0     1916 2023-03-24 00:33:11.232397 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/server/upload_file_request_handler.meta.json
--rw-r--r--   0        0        0    14813 2023-03-24 00:33:11.175978 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/session_data.data.json
--rw-r--r--   0        0        0     1794 2023-03-24 00:33:11.176250 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/session_data.meta.json
--rw-r--r--   0        0        0     9102 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/source_util.data.json
--rw-r--r--   0        0        0     2058 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/source_util.meta.json
--rw-r--r--   0        0        0     2887 2023-03-24 00:33:11.197493 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/state/__init__.data.json
--rw-r--r--   0        0        0     1649 2023-03-24 00:33:11.197721 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/state/__init__.meta.json
--rw-r--r--   0        0        0    13652 2023-03-24 00:33:11.191613 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/state/safe_session_state.data.json
--rw-r--r--   0        0        0     1648 2023-03-24 00:33:11.191856 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/state/safe_session_state.meta.json
--rw-r--r--   0        0        0   121394 2023-03-24 00:33:11.186461 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/state/session_state.data.json
--rw-r--r--   0        0        0     3939 2023-03-24 00:33:11.186737 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/state/session_state.meta.json
--rw-r--r--   0        0        0    12548 2023-03-24 00:33:11.196058 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/state/session_state_proxy.data.json
--rw-r--r--   0        0        0     1858 2023-03-24 00:33:11.196305 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/state/session_state_proxy.meta.json
--rw-r--r--   0        0        0    15052 2023-03-24 00:33:11.191001 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/state/widgets.data.json
--rw-r--r--   0        0        0     2617 2023-03-24 00:33:11.191238 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/state/widgets.meta.json
--rw-r--r--   0        0        0    28441 2023-03-24 00:33:11.155373 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/stats.data.json
--rw-r--r--   0        0        0     1691 2023-03-24 00:33:11.155677 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/stats.meta.json
--rw-r--r--   0        0        0    10753 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/string_util.data.json
--rw-r--r--   0        0        0     1963 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/string_util.meta.json
--rw-r--r--   0        0        0    79236 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/type_util.data.json
--rw-r--r--   0        0        0     4219 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/type_util.meta.json
--rw-r--r--   0        0        0    34194 2023-03-24 00:33:11.169034 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/uploaded_file_manager.data.json
--rw-r--r--   0        0        0     1751 2023-03-24 00:33:11.169352 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/uploaded_file_manager.meta.json
--rw-r--r--   0        0        0     3012 2023-03-24 00:33:10.296766 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/url_util.data.json
--rw-r--r--   0        0        0     1622 2023-03-24 00:33:10.297013 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/url_util.meta.json
--rw-r--r--   0        0        0     9557 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/user_info.data.json
--rw-r--r--   0        0        0     1869 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/user_info.meta.json
--rw-r--r--   0        0        0    12803 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/util.data.json
--rw-r--r--   0        0        0     2021 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/util.meta.json
--rw-r--r--   0        0        0     1728 2023-03-26 00:13:34.463357 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/vendor/__init__.data.json
--rw-r--r--   0        0        0     1693 2023-03-26 00:13:34.463796 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/vendor/__init__.meta.json
--rw-r--r--   0        0        0     1792 2023-03-26 00:13:34.464360 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/vendor/ipython/__init__.data.json
--rw-r--r--   0        0        0     1709 2023-03-26 00:13:34.464728 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/vendor/ipython/__init__.meta.json
--rw-r--r--   0        0        0     5474 2023-03-26 00:13:37.345826 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/vendor/ipython/modified_sys_path.data.json
--rw-r--r--   0        0        0     1801 2023-03-26 00:13:37.346158 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/vendor/ipython/modified_sys_path.meta.json
--rw-r--r--   0        0        0     5468 2023-03-26 00:13:37.350918 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/version.data.json
--rw-r--r--   0        0        0     1899 2023-03-26 00:13:37.351172 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/version.meta.json
--rw-r--r--   0        0        0     2273 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/watcher/__init__.data.json
--rw-r--r--   0        0        0     1788 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/watcher/__init__.meta.json
--rw-r--r--   0        0        0    34028 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/watcher/event_based_path_watcher.data.json
--rw-r--r--   0        0        0     2074 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/watcher/event_based_path_watcher.meta.json
--rw-r--r--   0        0        0    34345 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/watcher/local_sources_watcher.data.json
--rw-r--r--   0        0        0     2252 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/watcher/local_sources_watcher.meta.json
--rw-r--r--   0        0        0    11709 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/watcher/path_watcher.data.json
--rw-r--r--   0        0        0     2010 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/watcher/path_watcher.meta.json
--rw-r--r--   0        0        0    12311 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/watcher/polling_path_watcher.data.json
--rw-r--r--   0        0        0     2017 2023-03-26 00:13:37.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/watcher/polling_path_watcher.meta.json
--rw-r--r--   0        0        0     6346 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/watcher/util.data.json
--rw-r--r--   0        0        0     1892 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/streamlit/watcher/util.meta.json
--rw-r--r--   0        0        0    28943 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/string.data.json
--rw-r--r--   0        0        0     1800 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/string.meta.json
--rw-r--r--   0        0        0    16772 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/struct.data.json
--rw-r--r--   0        0        0     1797 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/struct.meta.json
--rw-r--r--   0        0        0   173211 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1875 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   152188 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1854 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0   130362 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tempfile.data.json
--rw-r--r--   0        0        0     1819 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tempfile.meta.json
--rw-r--r--   0        0        0    51912 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/termios.data.json
--rw-r--r--   0        0        0     1750 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/termios.meta.json
--rw-r--r--   0        0        0    21203 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/textwrap.data.json
--rw-r--r--   0        0        0     1730 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/textwrap.meta.json
--rw-r--r--   0        0        0    70566 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/threading.data.json
--rw-r--r--   0        0        0     1785 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/threading.meta.json
--rw-r--r--   0        0        0    46632 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/time.data.json
--rw-r--r--   0        0        0     1744 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/time.meta.json
--rw-r--r--   0        0        0    13162 2023-03-26 00:13:34.667375 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/timeit.data.json
--rw-r--r--   0        0        0     1740 2023-03-26 00:13:34.667708 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/timeit.meta.json
--rw-r--r--   0        0        0    16375 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/token.data.json
--rw-r--r--   0        0        0     1721 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/token.meta.json
--rw-r--r--   0        0        0    53728 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tokenize.data.json
--rw-r--r--   0        0        0     1804 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tokenize.meta.json
--rw-r--r--   0        0        0     1954 2023-03-24 00:33:08.349397 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/__init__.data.json
--rw-r--r--   0        0        0     1499 2023-03-24 00:33:08.349676 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/__init__.meta.json
--rw-r--r--   0        0        0     1465 2023-03-24 00:33:08.236672 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/_locale_data.data.json
--rw-r--r--   0        0        0     1516 2023-03-24 00:33:08.236854 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/_locale_data.meta.json
--rw-r--r--   0        0        0    10429 2023-03-24 00:33:10.587668 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/autoreload.data.json
--rw-r--r--   0        0        0     1965 2023-03-24 00:33:10.588033 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/autoreload.meta.json
--rw-r--r--   0        0        0    24381 2023-03-24 00:33:10.548472 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/concurrent.data.json
--rw-r--r--   0        0        0     1811 2023-03-24 00:33:10.548777 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/concurrent.meta.json
--rw-r--r--   0        0        0    28919 2023-03-24 00:33:10.319187 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/escape.data.json
--rw-r--r--   0        0        0     1793 2023-03-24 00:33:10.319467 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/escape.meta.json
--rw-r--r--   0        0        0    53776 2023-03-24 00:33:10.551047 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/gen.data.json
--rw-r--r--   0        0        0     2037 2023-03-24 00:33:10.551230 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/gen.meta.json
--rw-r--r--   0        0        0    49762 2023-03-24 00:33:10.573685 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/http1connection.data.json
--rw-r--r--   0        0        0     2107 2023-03-24 00:33:10.574016 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/http1connection.meta.json
--rw-r--r--   0        0        0    59349 2023-03-24 00:33:10.624283 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/httpclient.data.json
--rw-r--r--   0        0        0     2129 2023-03-24 00:33:10.624687 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/httpclient.meta.json
--rw-r--r--   0        0        0    34361 2023-03-24 00:33:10.630821 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/httpserver.data.json
--rw-r--r--   0        0        0     1855 2023-03-24 00:33:10.631150 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/httpserver.meta.json
--rw-r--r--   0        0        0   106247 2023-03-24 00:33:10.463357 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/httputil.data.json
--rw-r--r--   0        0        0     2122 2023-03-24 00:33:10.463652 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/httputil.meta.json
--rw-r--r--   0        0        0    61006 2023-03-24 00:33:10.549929 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/ioloop.data.json
--rw-r--r--   0        0        0     2182 2023-03-24 00:33:10.550179 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/ioloop.meta.json
--rw-r--r--   0        0        0    72931 2023-03-24 00:33:10.553182 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/iostream.data.json
--rw-r--r--   0        0        0     2237 2023-03-24 00:33:10.553412 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/iostream.meta.json
--rw-r--r--   0        0        0    24382 2023-03-24 00:33:10.444086 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/locale.data.json
--rw-r--r--   0        0        0     1855 2023-03-24 00:33:10.444396 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/locale.meta.json
--rw-r--r--   0        0        0    33199 2023-03-24 00:33:10.593650 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/locks.data.json
--rw-r--r--   0        0        0     1859 2023-03-24 00:33:10.594000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/locks.meta.json
--rw-r--r--   0        0        0     9113 2023-03-24 00:33:10.380448 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/log.data.json
--rw-r--r--   0        0        0     1834 2023-03-24 00:33:10.380730 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/log.meta.json
--rw-r--r--   0        0        0    30772 2023-03-24 00:33:10.551805 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/netutil.data.json
--rw-r--r--   0        0        0     1915 2023-03-24 00:33:10.552049 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/netutil.meta.json
--rw-r--r--   0        0        0    38708 2023-03-24 00:33:10.381446 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/options.data.json
--rw-r--r--   0        0        0     1804 2023-03-24 00:33:10.381656 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/options.meta.json
--rw-r--r--   0        0        0     1329 2023-03-24 00:33:08.293522 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/platform/__init__.data.json
--rw-r--r--   0        0        0     1483 2023-03-24 00:33:08.293705 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/platform/__init__.meta.json
--rw-r--r--   0        0        0    50976 2023-03-24 00:33:10.554192 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/platform/asyncio.data.json
--rw-r--r--   0        0        0     2053 2023-03-24 00:33:10.554376 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/platform/asyncio.meta.json
--rw-r--r--   0        0        0    18440 2023-03-24 00:33:10.554801 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/process.data.json
--rw-r--r--   0        0        0     2080 2023-03-24 00:33:10.555045 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/process.meta.json
--rw-r--r--   0        0        0    35458 2023-03-24 00:33:10.599406 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/queues.data.json
--rw-r--r--   0        0        0     1913 2023-03-24 00:33:10.599665 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/queues.meta.json
--rw-r--r--   0        0        0    53735 2023-03-24 00:33:10.643375 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/routing.data.json
--rw-r--r--   0        0        0     1864 2023-03-24 00:33:10.643867 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/routing.meta.json
--rw-r--r--   0        0        0    46153 2023-03-24 00:33:10.625460 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/simple_httpclient.data.json
--rw-r--r--   0        0        0     2323 2023-03-24 00:33:10.625763 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/simple_httpclient.meta.json
--rw-r--r--   0        0        0    27644 2023-03-24 00:33:10.581631 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/tcpclient.data.json
--rw-r--r--   0        0        0     2026 2023-03-24 00:33:10.581934 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/tcpclient.meta.json
--rw-r--r--   0        0        0    13544 2023-03-24 00:33:10.558702 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/tcpserver.data.json
--rw-r--r--   0        0        0     2010 2023-03-24 00:33:10.558953 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/tcpserver.meta.json
--rw-r--r--   0        0        0    80175 2023-03-24 00:33:10.430612 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/template.data.json
--rw-r--r--   0        0        0     1867 2023-03-24 00:33:10.430920 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/template.meta.json
--rw-r--r--   0        0        0    39039 2023-03-24 00:33:10.305088 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/util.data.json
--rw-r--r--   0        0        0     1818 2023-03-24 00:33:10.305375 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/util.meta.json
--rw-r--r--   0        0        0   207670 2023-03-24 00:33:10.709553 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/web.data.json
--rw-r--r--   0        0        0     2681 2023-03-24 00:33:10.709881 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/web.meta.json
--rw-r--r--   0        0        0   127545 2023-03-24 00:33:10.732419 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/websocket.data.json
--rw-r--r--   0        0        0     2474 2023-03-24 00:33:10.732776 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tornado/websocket.meta.json
--rw-r--r--   0        0        0    56300 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/traceback.data.json
--rw-r--r--   0        0        0     1794 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/traceback.meta.json
--rw-r--r--   0        0        0     5335 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tty.data.json
--rw-r--r--   0        0        0     1722 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/tty.meta.json
--rw-r--r--   0        0        0   248545 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1826 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   444990 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1892 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    73993 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1816 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    46042 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unicodedata.data.json
--rw-r--r--   0        0        0     1758 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unicodedata.meta.json
--rw-r--r--   0        0        0     6507 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/__init__.data.json
--rw-r--r--   0        0        0     1943 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/__init__.meta.json
--rw-r--r--   0        0        0    26183 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/_log.data.json
--rw-r--r--   0        0        0     1791 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/_log.meta.json
--rw-r--r--   0        0        0     8318 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/async_case.data.json
--rw-r--r--   0        0        0     1822 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/async_case.meta.json
--rw-r--r--   0        0        0   225925 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/case.data.json
--rw-r--r--   0        0        0     1942 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/case.meta.json
--rw-r--r--   0        0        0    15918 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/loader.data.json
--rw-r--r--   0        0        0     1853 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/loader.meta.json
--rw-r--r--   0        0        0    12791 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/main.data.json
--rw-r--r--   0        0        0     1862 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/main.meta.json
--rw-r--r--   0        0        0   162909 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/mock.data.json
--rw-r--r--   0        0        0     1824 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/mock.meta.json
--rw-r--r--   0        0        0    22446 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/result.data.json
--rw-r--r--   0        0        0     1809 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/result.meta.json
--rw-r--r--   0        0        0    11707 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/runner.data.json
--rw-r--r--   0        0        0     1852 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/runner.meta.json
--rw-r--r--   0        0        0    12369 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/signals.data.json
--rw-r--r--   0        0        0     1804 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/signals.meta.json
--rw-r--r--   0        0        0    12262 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/suite.data.json
--rw-r--r--   0        0        0     1825 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/unittest/suite.meta.json
--rw-r--r--   0        0        0     1669 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/urllib/__init__.data.json
--rw-r--r--   0        0        0     1695 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/urllib/__init__.meta.json
--rw-r--r--   0        0        0   166627 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/urllib/parse.data.json
--rw-r--r--   0        0        0     1801 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/urllib/parse.meta.json
--rw-r--r--   0        0        0    36729 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/uuid.data.json
--rw-r--r--   0        0        0     1824 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/uuid.meta.json
--rw-r--r--   0        0        0    24197 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/warnings.data.json
--rw-r--r--   0        0        0     1812 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/warnings.meta.json
--rw-r--r--   0        0        0     1664 2023-03-26 00:13:34.521808 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/__init__.data.json
--rw-r--r--   0        0        0     1679 2023-03-26 00:13:34.522180 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/__init__.meta.json
--rw-r--r--   0        0        0    46367 2023-03-26 00:13:34.997032 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/events.data.json
--rw-r--r--   0        0        0     1929 2023-03-26 00:13:34.997400 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/events.meta.json
--rw-r--r--   0        0        0     3080 2023-03-26 00:13:36.411419 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/observers/__init__.data.json
--rw-r--r--   0        0        0     1973 2023-03-26 00:13:36.412251 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/observers/__init__.meta.json
--rw-r--r--   0        0        0    30099 2023-03-26 00:13:35.052601 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/observers/api.data.json
--rw-r--r--   0        0        0     1928 2023-03-26 00:13:35.053337 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/observers/api.meta.json
--rw-r--r--   0        0        0    15395 2023-03-26 00:13:35.249745 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/observers/fsevents.data.json
--rw-r--r--   0        0        0     2102 2023-03-26 00:13:35.250108 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/observers/fsevents.meta.json
--rw-r--r--   0        0        0    31402 2023-03-26 00:13:35.254307 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/observers/kqueue.data.json
--rw-r--r--   0        0        0     2025 2023-03-26 00:13:35.254861 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/observers/kqueue.meta.json
--rw-r--r--   0        0        0     9060 2023-03-26 00:13:35.256351 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/observers/polling.data.json
--rw-r--r--   0        0        0     1945 2023-03-26 00:13:35.256796 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/observers/polling.meta.json
--rw-r--r--   0        0        0     8256 2023-03-26 00:13:34.799645 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/utils/__init__.data.json
--rw-r--r--   0        0        0     1765 2023-03-26 00:13:34.799912 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/utils/__init__.meta.json
--rw-r--r--   0        0        0     3828 2023-03-26 00:13:34.985625 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/utils/bricks.data.json
--rw-r--r--   0        0        0     1735 2023-03-26 00:13:34.986057 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/utils/bricks.meta.json
--rw-r--r--   0        0        0    25330 2023-03-26 00:13:34.963896 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/utils/dirsnapshot.data.json
--rw-r--r--   0        0        0     1897 2023-03-26 00:13:34.964347 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/utils/dirsnapshot.meta.json
--rw-r--r--   0        0        0     2944 2023-03-26 00:13:34.795141 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/utils/patterns.data.json
--rw-r--r--   0        0        0     1752 2023-03-26 00:13:34.795405 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/utils/patterns.meta.json
--rw-r--r--   0        0        0     4705 2023-03-26 00:13:34.730814 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/utils/platform.data.json
--rw-r--r--   0        0        0     1737 2023-03-26 00:13:34.731189 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/watchdog/utils/platform.meta.json
--rw-r--r--   0        0        0    58616 2023-03-26 00:13:34.556028 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/wave.data.json
--rw-r--r--   0        0        0     1809 2023-03-26 00:13:34.556412 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/wave.meta.json
--rw-r--r--   0        0        0   156352 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/weakref.data.json
--rw-r--r--   0        0        0     1818 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/weakref.meta.json
--rw-r--r--   0        0        0    30313 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/webbrowser.data.json
--rw-r--r--   0        0        0     1782 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/webbrowser.meta.json
--rw-r--r--   0        0        0    75700 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/zipfile.data.json
--rw-r--r--   0        0        0     1880 2023-03-26 00:13:29.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/zipfile.meta.json
--rw-r--r--   0        0        0    18708 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/zlib.data.json
--rw-r--r--   0        0        0     1829 2023-03-26 00:13:34.000000 cupid_matching-1.0.8/cupid_matching/.mypy_cache/3.10/zlib.meta.json
--rw-r--r--   0        0        0      190 2023-03-24 00:10:22.896312 cupid_matching-1.0.8/cupid_matching/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       37 2023-04-01 14:40:13.598825 cupid_matching-1.0.8/cupid_matching/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-04-01 14:40:13.598920 cupid_matching-1.0.8/cupid_matching/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2023-04-01 14:40:13.598719 cupid_matching-1.0.8/cupid_matching/.pytest_cache/README.md
--rw-r--r--   0        0        0       68 2023-04-01 14:40:13.599181 cupid_matching-1.0.8/cupid_matching/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0       56 2023-04-01 14:40:35.466759 cupid_matching-1.0.8/cupid_matching/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-04-01 14:40:35.467039 cupid_matching-1.0.8/cupid_matching/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2023-04-02 19:21:40.197779 cupid_matching-1.0.8/cupid_matching/__init__.py
--rw-r--r--   0        0        0     9372 2023-04-13 19:21:37.452172 cupid_matching-1.0.8/cupid_matching/choo_siow.py
--rw-r--r--   0        0        0     5656 2023-04-02 13:02:37.271948 cupid_matching-1.0.8/cupid_matching/choo_siow_gender_heteroskedastic.py
--rw-r--r--   0        0        0     6283 2023-04-02 19:11:25.395323 cupid_matching-1.0.8/cupid_matching/choo_siow_heteroskedastic.py
--rw-r--r--   0        0        0    14162 2023-04-02 13:02:37.272889 cupid_matching-1.0.8/cupid_matching/cupid_streamlit.py
--rw-r--r--   0        0        0       51 2023-03-24 00:22:09.620449 cupid_matching-1.0.8/cupid_matching/docs/choo_siow.md
--rw-r--r--   0        0        0       97 2023-03-24 00:21:48.848158 cupid_matching-1.0.8/cupid_matching/docs/choo_siow_gender_heteroskedastic.md
--rw-r--r--   0        0        0       83 2023-03-24 00:22:03.727712 cupid_matching-1.0.8/cupid_matching/docs/choo_siow_heteroskedastic.md
--rw-r--r--   0        0        0      285 2023-03-24 00:22:15.196968 cupid_matching-1.0.8/cupid_matching/docs/cupid_streamlit.md
--rw-r--r--   0        0        0       46 2023-03-24 00:22:19.670499 cupid_matching-1.0.8/cupid_matching/docs/entropy.md
--rw-r--r--   0        0        0       63 2023-04-02 13:02:37.273230 cupid_matching-1.0.8/cupid_matching/docs/example_choosiow.md
--rw-r--r--   0        0        0       69 2023-04-02 13:02:37.273547 cupid_matching-1.0.8/cupid_matching/docs/example_nestedlogit.md
--rw-r--r--   0        0        0     2376 2023-04-13 19:22:17.507324 cupid_matching-1.0.8/cupid_matching/docs/index.md
--rw-r--r--   0        0        0       57 2023-03-24 00:22:52.962261 cupid_matching-1.0.8/cupid_matching/docs/ipfp_solvers.md
--rw-r--r--   0        0        0       61 2023-03-24 00:22:57.157065 cupid_matching-1.0.8/cupid_matching/docs/matching_utils.md
--rw-r--r--   0        0        0       57 2023-03-24 00:23:07.925133 cupid_matching-1.0.8/cupid_matching/docs/min_distance.md
--rw-r--r--   0        0        0       69 2023-03-24 00:23:01.182377 cupid_matching-1.0.8/cupid_matching/docs/min_distance_utils.md
--rw-r--r--   0        0        0       59 2023-03-24 00:27:46.673143 cupid_matching-1.0.8/cupid_matching/docs/model_classes.md
--rw-r--r--   0        0        0       58 2023-03-24 00:23:19.684703 cupid_matching-1.0.8/cupid_matching/docs/nested_logit.md
--rw-r--r--   0        0        0       55 2023-03-24 00:27:33.384226 cupid_matching-1.0.8/cupid_matching/docs/poisson_glm.md
--rw-r--r--   0        0        0       67 2023-03-24 00:27:42.792605 cupid_matching-1.0.8/cupid_matching/docs/poisson_glm_utils.md
--rw-r--r--   0        0        0       43 2023-03-24 00:27:23.096924 cupid_matching-1.0.8/cupid_matching/docs/utils.md
--rw-r--r--   0        0        0    11551 2023-04-02 19:15:11.050530 cupid_matching-1.0.8/cupid_matching/entropy.py
--rw-r--r--   0        0        0     3531 2023-04-13 19:09:36.869069 cupid_matching-1.0.8/cupid_matching/example_choosiow.py
--rw-r--r--   0        0        0     4133 2023-04-02 19:13:08.597638 cupid_matching-1.0.8/cupid_matching/example_nestedlogit.py
--rw-r--r--   0        0        0    26548 2023-04-02 19:13:28.516760 cupid_matching-1.0.8/cupid_matching/ipfp_solvers.py
--rw-r--r--   0        0        0     8744 2023-04-13 19:02:11.316261 cupid_matching-1.0.8/cupid_matching/matching_utils.py
--rw-r--r--   0        0        0    11551 2023-04-02 19:13:54.856938 cupid_matching-1.0.8/cupid_matching/min_distance.py
--rw-r--r--   0        0        0     5260 2023-04-02 19:13:40.696373 cupid_matching-1.0.8/cupid_matching/min_distance_utils.py
--rw-r--r--   0        0        0     1873 2023-04-02 13:02:37.291292 cupid_matching-1.0.8/cupid_matching/mkdocs.yml
--rw-r--r--   0        0        0    16277 2023-04-02 19:15:11.063645 cupid_matching-1.0.8/cupid_matching/model_classes.py
--rw-r--r--   0        0        0      369 2023-04-02 19:14:11.059995 cupid_matching-1.0.8/cupid_matching/mypy.ini
--rw-r--r--   0        0        0     9515 2023-04-02 19:15:11.064847 cupid_matching-1.0.8/cupid_matching/nested_logit.py
--rw-r--r--   0        0        0     7401 2023-04-02 19:15:11.067470 cupid_matching-1.0.8/cupid_matching/poisson_glm.py
--rw-r--r--   0        0        0     6544 2023-04-02 19:14:50.571051 cupid_matching-1.0.8/cupid_matching/poisson_glm_utils.py
--rw-r--r--   0        0        0    17888 2023-04-13 17:38:40.800414 cupid_matching-1.0.8/cupid_matching/site/404.html
--rw-r--r--   0        0        0      704 2023-04-13 17:38:40.738846 cupid_matching-1.0.8/cupid_matching/site/assets/_mkdocstrings.css
--rw-r--r--   0        0        0     1870 2023-04-13 17:38:40.739462 cupid_matching-1.0.8/cupid_matching/site/assets/images/favicon.png
--rw-r--r--   0        0        0   113254 2023-04-13 17:38:40.739717 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/bundle.407015b8.min.js
--rw-r--r--   0        0        0   950772 2023-04-13 17:38:40.740168 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/bundle.407015b8.min.js.map
--rw-r--r--   0        0        0    17074 2023-04-13 17:38:40.740488 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-r--r--   0        0        0     4654 2023-04-13 17:38:40.740717 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.da.min.js
--rw-r--r--   0        0        0     6119 2023-04-13 17:38:40.740985 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.de.min.js
--rw-r--r--   0        0        0     6208 2023-04-13 17:38:40.741223 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.du.min.js
--rw-r--r--   0        0        0    11499 2023-04-13 17:38:40.741554 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.es.min.js
--rw-r--r--   0        0        0     9342 2023-04-13 17:38:40.741847 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-r--r--   0        0        0    10669 2023-04-13 17:38:40.742074 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-r--r--   0        0        0     3383 2023-04-13 17:38:40.742279 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.hi.min.js
--rw-r--r--   0        0        0     9437 2023-04-13 17:38:40.742506 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-r--r--   0        0        0    11232 2023-04-13 17:38:40.742925 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.it.min.js
--rw-r--r--   0        0        0     2313 2023-04-13 17:38:40.743163 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-r--r--   0        0        0       36 2023-04-13 17:38:40.743404 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-r--r--   0        0        0     7973 2023-04-13 17:38:40.743615 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.ko.min.js
--rw-r--r--   0        0        0      817 2023-04-13 17:38:40.744047 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-r--r--   0        0        0     6026 2023-04-13 17:38:40.744350 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-r--r--   0        0        0     4754 2023-04-13 17:38:40.744583 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.no.min.js
--rw-r--r--   0        0        0    10171 2023-04-13 17:38:40.744799 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-r--r--   0        0        0    10958 2023-04-13 17:38:40.744965 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-r--r--   0        0        0    10331 2023-04-13 17:38:40.745144 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-r--r--   0        0        0     3647 2023-04-13 17:38:40.745369 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-r--r--   0        0        0     4523 2023-04-13 17:38:40.745556 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-r--r--   0        0        0     2406 2023-04-13 17:38:40.745733 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.ta.min.js
--rw-r--r--   0        0        0     1031 2023-04-13 17:38:40.745896 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.th.min.js
--rw-r--r--   0        0        0    15009 2023-04-13 17:38:40.746294 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-r--r--   0        0        0      784 2023-04-13 17:38:40.746526 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-r--r--   0        0        0     2062 2023-04-13 17:38:40.746713 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/min/lunr.zh.min.js
--rw-r--r--   0        0        0    22878 2023-04-13 17:38:40.746964 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/tinyseg.js
--rw-r--r--   0        0        0   677455 2023-04-13 17:38:40.747315 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/lunr/wordcut.js
--rw-r--r--   0        0        0    38916 2023-04-13 17:38:40.747560 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/workers/search.208ed371.min.js
--rw-r--r--   0        0        0   209901 2023-04-13 17:38:40.747802 cupid_matching-1.0.8/cupid_matching/site/assets/javascripts/workers/search.208ed371.min.js.map
--rw-r--r--   0        0        0   113417 2023-04-13 17:38:40.748064 cupid_matching-1.0.8/cupid_matching/site/assets/stylesheets/main.7a7fce14.min.css
--rw-r--r--   0        0        0    38957 2023-04-13 17:38:40.748263 cupid_matching-1.0.8/cupid_matching/site/assets/stylesheets/main.7a7fce14.min.css.map
--rw-r--r--   0        0        0    12355 2023-04-13 17:38:40.748441 cupid_matching-1.0.8/cupid_matching/site/assets/stylesheets/palette.a0c5b2b5.min.css
--rw-r--r--   0        0        0     3646 2023-04-13 17:38:40.748643 cupid_matching-1.0.8/cupid_matching/site/assets/stylesheets/palette.a0c5b2b5.min.css.map
--rw-r--r--   0        0        0    56388 2023-04-13 17:38:40.822437 cupid_matching-1.0.8/cupid_matching/site/choo_siow/index.html
--rw-r--r--   0        0        0    61309 2023-04-13 17:38:40.836416 cupid_matching-1.0.8/cupid_matching/site/choo_siow_gender_heteroskedastic/index.html
--rw-r--r--   0        0        0    67113 2023-04-13 17:38:40.853319 cupid_matching-1.0.8/cupid_matching/site/choo_siow_heteroskedastic/index.html
--rw-r--r--   0        0        0    19453 2023-04-13 17:38:40.854153 cupid_matching-1.0.8/cupid_matching/site/cupid_streamlit/index.html
--rw-r--r--   0        0        0    52734 2023-04-13 17:38:40.863760 cupid_matching-1.0.8/cupid_matching/site/entropy/index.html
--rw-r--r--   0        0        0    33047 2023-04-13 17:38:40.868763 cupid_matching-1.0.8/cupid_matching/site/example_choosiow/index.html
--rw-r--r--   0        0        0    40108 2023-04-13 17:38:40.876280 cupid_matching-1.0.8/cupid_matching/site/example_nestedlogit/index.html
--rw-r--r--   0        0        0    24691 2023-04-13 17:38:40.809070 cupid_matching-1.0.8/cupid_matching/site/index.html
--rw-r--r--   0        0        0   171028 2023-04-13 17:38:40.932202 cupid_matching-1.0.8/cupid_matching/site/ipfp_solvers/index.html
--rw-r--r--   0        0        0    33535 2023-04-13 17:38:40.937827 cupid_matching-1.0.8/cupid_matching/site/matching_utils/index.html
--rw-r--r--   0        0        0    73534 2023-04-13 17:38:40.958010 cupid_matching-1.0.8/cupid_matching/site/min_distance/index.html
--rw-r--r--   0        0        0    48540 2023-04-13 17:38:40.969561 cupid_matching-1.0.8/cupid_matching/site/min_distance_utils/index.html
--rw-r--r--   0        0        0   158026 2023-04-13 17:38:41.025442 cupid_matching-1.0.8/cupid_matching/site/model_classes/index.html
--rw-r--r--   0        0        0    80301 2023-04-13 17:38:41.047356 cupid_matching-1.0.8/cupid_matching/site/nested_logit/index.html
--rw-r--r--   0        0        0      864 2023-04-13 17:38:40.739163 cupid_matching-1.0.8/cupid_matching/site/objects.inv
--rw-r--r--   0        0        0    70696 2023-04-13 17:38:41.068101 cupid_matching-1.0.8/cupid_matching/site/poisson_glm/index.html
--rw-r--r--   0        0        0    52629 2023-04-13 17:38:41.080736 cupid_matching-1.0.8/cupid_matching/site/poisson_glm_utils/index.html
--rw-r--r--   0        0        0   180005 2023-04-13 17:38:41.116311 cupid_matching-1.0.8/cupid_matching/site/search/search_index.json
--rw-r--r--   0        0        0     3235 2023-04-13 17:38:40.750319 cupid_matching-1.0.8/cupid_matching/site/sitemap.xml
--rw-r--r--   0        0        0      354 2023-04-13 17:38:40.750481 cupid_matching-1.0.8/cupid_matching/site/sitemap.xml.gz
--rw-r--r--   0        0        0   120234 2023-04-13 17:38:41.115705 cupid_matching-1.0.8/cupid_matching/site/utils/index.html
--rw-r--r--   0        0        0    12373 2023-04-02 19:15:05.244218 cupid_matching-1.0.8/cupid_matching/utils.py
--rw-r--r--   0        0        0      969 2023-04-13 19:22:41.046163 cupid_matching-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     3119 1970-01-01 00:00:00.000000 cupid_matching-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    10260 2023-05-10 22:37:56.546277 cupid_matching-1.1.0/README.md
+-rw-r--r--   0        0        0        1 2023-05-09 18:41:31.499628 cupid_matching-1.1.0/cupid_matching/__init__.py
+-rw-r--r--   0        0        0     9402 2023-05-09 18:41:31.500025 cupid_matching-1.1.0/cupid_matching/choo_siow.py
+-rw-r--r--   0        0        0     5651 2023-05-09 18:41:31.500175 cupid_matching-1.1.0/cupid_matching/choo_siow_gender_heteroskedastic.py
+-rw-r--r--   0        0        0     6292 2023-05-09 18:41:31.500324 cupid_matching-1.1.0/cupid_matching/choo_siow_heteroskedastic.py
+-rw-r--r--   0        0        0    14110 2023-05-09 18:41:31.500459 cupid_matching-1.1.0/cupid_matching/cupid_streamlit.py
+-rw-r--r--   0        0        0    11660 2023-05-09 18:41:31.500592 cupid_matching-1.1.0/cupid_matching/entropy.py
+-rw-r--r--   0        0        0     5224 2023-05-09 18:41:31.500731 cupid_matching-1.1.0/cupid_matching/example_choo_siow.py
+-rw-r--r--   0        0        0     4124 2023-05-09 18:41:31.500860 cupid_matching-1.1.0/cupid_matching/example_nested_logit.py
+-rw-r--r--   0        0        0    26215 2023-05-09 18:41:31.500997 cupid_matching-1.1.0/cupid_matching/ipfp_solvers.py
+-rw-r--r--   0        0        0    12873 2023-05-09 18:41:31.501150 cupid_matching-1.1.0/cupid_matching/matching_utils.py
+-rw-r--r--   0        0        0    11180 2023-05-09 18:41:31.501577 cupid_matching-1.1.0/cupid_matching/min_distance.py
+-rw-r--r--   0        0        0     5587 2023-05-09 18:41:31.501715 cupid_matching-1.1.0/cupid_matching/min_distance_utils.py
+-rw-r--r--   0        0        0    16046 2023-05-09 18:41:31.501854 cupid_matching-1.1.0/cupid_matching/model_classes.py
+-rw-r--r--   0        0        0      369 2023-05-09 18:40:06.062931 cupid_matching-1.1.0/cupid_matching/mypy.ini
+-rw-r--r--   0        0        0     9516 2023-05-09 18:41:31.501983 cupid_matching-1.1.0/cupid_matching/nested_logit.py
+-rw-r--r--   0        0        0     7443 2023-05-09 18:41:31.502116 cupid_matching-1.1.0/cupid_matching/poisson_glm.py
+-rw-r--r--   0        0        0     6302 2023-05-09 18:41:31.502254 cupid_matching-1.1.0/cupid_matching/poisson_glm_utils.py
+-rw-r--r--   0        0        0     1929 2023-05-09 18:41:31.502386 cupid_matching-1.1.0/cupid_matching/utils.py
+-rw-r--r--   0        0        0     2008 2023-05-10 20:49:34.810410 cupid_matching-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11051 1970-01-01 00:00:00.000000 cupid_matching-1.1.0/PKG-INFO
```

### Comparing `cupid_matching-1.0.8/cupid_matching/choo_siow.py` & `cupid_matching-1.1.0/cupid_matching/choo_siow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """The components of the derivative of the entropy
 for the Choo and Siow homoskedastic model.
 """
-from typing import Literal, Optional, Union, cast, overload
+from typing import Literal, cast, overload
 
 import numpy as np
+from bs_python_utils.bsnputils import FourArrays, ThreeArrays, TwoArrays, bs_error_abort
 
 from cupid_matching.entropy import EntropyFunctions, EntropyHessians
 from cupid_matching.matching_utils import Matching
-from cupid_matching.utils import FourArrays, ThreeArrays, TwoArrays, bs_error_abort
 
 
 @overload
 def _entropy_choo_siow(muhat: Matching, deriv: Literal[0]) -> np.ndarray:
     ...
 
 
@@ -22,23 +22,23 @@
 
 @overload
 def _entropy_choo_siow(muhat: Matching, deriv: Literal[2]) -> FourArrays:
     ...
 
 
 def _entropy_choo_siow(
-    muhat: Matching, deriv: Optional[int] = 0
-) -> Union[None, np.ndarray, TwoArrays, FourArrays]:
+    muhat: Matching, deriv: int | None = 0
+) -> None | np.ndarray | TwoArrays | FourArrays:
     """Returns the values of $\\mathcal{E}$
     and the first (if `deriv` is 1 or 2) and second (if `deriv` is 2) derivatives
     for the Choo and Siow model
 
     Args:
         muhat: a Matching
-        deriv: if equal 1, we compute the first derivatives too;
+        deriv: if equal 1, we compute_ the first derivatives too;
                if equals 2, also the hessian
 
     Returns:
         the value of the generalized entropy
         if deriv = 1 or 2, the (X,Y) matrix of the first derivative of the entropy
         if deriv = 2, the (X,Y,X,Y) array of the second derivative
             wrt $(\\mu,\\mu)$
@@ -62,15 +62,15 @@
     if deriv == 0:
         return val_entropy
     if deriv in [1, 2]:
         der_xy = -2.0 * logxy + log0y
         der_xy += logx0.reshape((-1, 1))
         if deriv == 1:
             return val_entropy, der_xy
-        else:  # we compute the Hessians
+        else:  # we compute_ the Hessians
             X, Y = muxy.shape
             derlogxy = 1.0 / muxy
             derlogx0 = 1.0 / mux0
             derlog0y = 1.0 / mu0y
             der2_xyzt = np.zeros((X, Y, X, Y))
             der2_xyr = np.zeros((X, Y, X + Y))
             for x in range(X):
@@ -86,48 +86,48 @@
             return val_entropy, der_xy, der2_xyzt, der2_xyr
     else:
         bs_error_abort("deriv should be 0, 1, or 2")
         return None
 
 
 def _der_entropy_choo_siow_corrected(
-    muhat: Matching, hessian: Optional[bool] = False
-) -> Union[np.ndarray, ThreeArrays]:
+    muhat: Matching, hessian: bool | None = False
+) -> np.ndarray | ThreeArrays:
     """Returns the corrected first derivative of $\\mathcal{E}$
-    and the corrected second derivative (if `hessian` is True) 
+    and the corrected second derivative (if `hessian` is True)
     for the Choo and Siow model
 
     Args:
         muhat: a Matching
-        hessian: if `True`, also compute the hessian
+        hessian: if `True`, also compute_ the hessian
 
     Returns:
         the (X,Y) matrix of the first derivative of the entropy
         if hessian is True, the (X,Y,X,Y) array of the second derivative
             wrt $(\\mu,\\mu)$
           and the (X,Y,X+Y) second derivatives
             wrt $(\\mu,(n,m))$
     """
     muxy, mux0, mu0y, *_ = muhat.unpack()
     n_households = np.sum(muxy) + np.sum(mux0) + np.sum(mu0y)
 
-    muxy_corr = muxy + (1.0-muxy/n_households)/2.0
+    muxy_corr = muxy + (1.0 - muxy / n_households) / 2.0
     logxy = np.log(muxy_corr)
-    mux0_corr = mux0 + (1.0-mux0/n_households)/2.0
+    mux0_corr = mux0 + (1.0 - mux0 / n_households) / 2.0
     logx0 = np.log(mux0_corr)
-    mu0y_corr = mu0y + (1.0-mu0y/n_households)/2.0
+    mu0y_corr = mu0y + (1.0 - mu0y / n_households) / 2.0
     log0y = np.log(mu0y_corr)
 
     der_xy = -2.0 * logxy + log0y
     der_xy += logx0.reshape((-1, 1))
     if not hessian:
         return der_xy
-    else:  # we compute the Hessians
+    else:  # we compute_ the Hessians
         X, Y = muxy.shape
-        f_corr = 1.0-1.0/n_households/2.0
+        f_corr = 1.0 - 1.0 / n_households / 2.0
         derlogxy = f_corr / muxy_corr
         derlogx0 = f_corr / mux0_corr
         derlog0y = f_corr / mu0y_corr
         der2_xyzt = np.zeros((X, Y, X, Y))
         der2_xyr = np.zeros((X, Y, X + Y))
         for x in range(X):
             dlogx0 = derlogx0[x]
@@ -148,29 +148,28 @@
     Args:
         muhat: a Matching
 
     Returns:
         the (X,Y) matrix of the first derivative of the entropy
     """
     entropy_res = _entropy_choo_siow(muhat, deriv=1)
-    return entropy_res[1]
+    return cast(np.ndarray, entropy_res[1])
 
 
 def e0_fun_choo_siow_corrected(muhat: Matching) -> np.ndarray:
     """Returns the values of $e_0$ for the Choo and Siow model,
     using the finite-sample correction log(p+(1-p)/(2N))
 
     Args:
         muhat: a Matching
 
     Returns:
         the (X,Y) matrix of the first derivative of the entropy
     """
-    e0_val_corrected \
-        = _der_entropy_choo_siow_corrected(muhat, hessian=False)
+    e0_val_corrected = _der_entropy_choo_siow_corrected(muhat, hessian=False)
     return e0_val_corrected
 
 
 def hessian_mumu_choo_siow(muhat: Matching) -> ThreeArrays:
     """Returns the derivatives of $e_0$ in $\\mu$
     for the Choo and Siow model.
 
@@ -202,16 +201,15 @@
 
     Args:
         muhat: a Matching
 
     Returns:
         the three components of the hessian wrt $(\\mu,\\mu)$ of the entropy
     """
-    _, hessmumu, _ \
-        = _der_entropy_choo_siow_corrected(muhat, hessian=True)
+    _, hessmumu, _ = _der_entropy_choo_siow_corrected(muhat, hessian=True)
     muxy, *_ = muhat.unpack()
     X, Y = muxy.shape
     hess_x = np.zeros((X, Y, Y))
     hess_y = np.zeros((X, Y, X))
     hess_xy = np.zeros((X, Y))
     for x in range(X):
         for y in range(Y):
@@ -252,16 +250,15 @@
 
     Args:
         muhat: a Matching
 
     Returns:
         the two components of the hessian wrt $(\\mu,r)$ of the entropy
     """
-    _, _, hessmur \
-        = _der_entropy_choo_siow_corrected(muhat, hessian=True)
+    _, _, hessmur = _der_entropy_choo_siow_corrected(muhat, hessian=True)
     muxy, *_ = muhat.unpack()
     X, Y = muxy.shape
     hess_nx = np.zeros((X, Y))
     hess_my = np.zeros((X, Y))
     for x in range(X):
         for y in range(Y):
             d2r = hessmur[x, y, :]
@@ -283,19 +280,24 @@
     description="Choo and Siow homoskedastic with analytic Hessian",
 )
 
 entropy_choo_siow_corrected = EntropyFunctions(
     e0_fun=e0_fun_choo_siow_corrected,
     hessian="provided",
     e0_derivative=cast(EntropyHessians, e0_derivative_choo_siow_corrected),
-    description="Choo and Siow homoskedastic with analytic Hessian and finite-sample correction",
+    description=(
+        "Choo and Siow homoskedastic with analytic Hessian and finite-sample correction"
+    ),
 )
 
 entropy_choo_siow_numeric = EntropyFunctions(
     e0_fun=e0_fun_choo_siow,
     description="Choo and Siow homoskedastic with numerical Hessian",
 )
 
 entropy_choo_siow_corrected_numeric = EntropyFunctions(
     e0_fun=e0_fun_choo_siow_corrected,
-    description="Choo and Siow homoskedastic with numerical Hessian and finite-sample correction",
+    description=(
+        "Choo and Siow homoskedastic with numerical Hessian and finite-sample"
+        " correction"
+    ),
 )
```

### Comparing `cupid_matching-1.0.8/cupid_matching/choo_siow_gender_heteroskedastic.py` & `cupid_matching-1.1.0/cupid_matching/choo_siow_gender_heteroskedastic.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 We normalize the standard error for the X side at 1,
 and we estimate the standard error on the Y side.
 """
 from typing import cast
 
 import numpy as np
+from bs_python_utils.bsnputils import ThreeArrays, TwoArrays
 
 from cupid_matching.entropy import EntropyFunctions, EntropyHessians
 from cupid_matching.matching_utils import Matching
-from cupid_matching.utils import ThreeArrays, TwoArrays
 
 
 def e0_choo_siow_gender_heteroskedastic(muhat: Matching) -> np.ndarray:
     """Returns the values of the parameter-independent part $e_0$
     for the Choo and Siow gender-heteroskedastic model; we normalized $\\sigma=1$.
 
     Args:
@@ -22,15 +22,15 @@
 
     Returns:
         the (X,Y) matrix of the parameter-independent part
         of the first derivative of the entropy.
     """
     muxy, mux0, *_ = muhat.unpack()
     e0_vals = -np.log(muxy / mux0.reshape((-1, 1)))
-    return e0_vals
+    return cast(np.ndarray, e0_vals)
 
 
 def e0_derivative_mu_gender_heteroskedastic(
     muhat: Matching,
 ) -> ThreeArrays:
     """Returns the derivatives of the parameter-independent part $e_0$ in $\\mu$.
     for the Choo and Siow gender-heteroskedastic model; we normalized $\\sigma=1$.
@@ -173,20 +173,16 @@
 )
 
 entropy_choo_siow_gender_heteroskedastic = EntropyFunctions(
     e0_fun=e0_choo_siow_gender_heteroskedastic,
     parameter_dependent=True,
     e_fun=e_choo_siow_gender_heteroskedastic,
     hessian="provided",
-    e0_derivative=cast(
-        EntropyHessians, e0_derivative_choo_siow_gender_heteroskedastic
-    ),
-    e_derivative=cast(
-        EntropyHessians, e_derivative_choo_siow_gender_heteroskedastic
-    ),
+    e0_derivative=cast(EntropyHessians, e0_derivative_choo_siow_gender_heteroskedastic),
+    e_derivative=cast(EntropyHessians, e_derivative_choo_siow_gender_heteroskedastic),
     description="Choo and Siow gender-heteroskedastic with analytic Hessian",
 )
 
 entropy_choo_siow_gender_heteroskedastic_numeric = EntropyFunctions(
     e0_fun=e0_choo_siow_gender_heteroskedastic,
     parameter_dependent=True,
     e_fun=e_choo_siow_gender_heteroskedastic,
```

### Comparing `cupid_matching-1.0.8/cupid_matching/choo_siow_heteroskedastic.py` & `cupid_matching-1.1.0/cupid_matching/choo_siow_heteroskedastic.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 We normalize the standard error for X=1 at 1, and we estimate the standard errors
 for all other types on the X side and for all types on the Y side.
 """
 from typing import cast
 
 import numpy as np
+from bs_python_utils.bsnputils import ThreeArrays, TwoArrays
 
 from cupid_matching.entropy import EntropyFunctions, EntropyHessians
 from cupid_matching.matching_utils import Matching
-from cupid_matching.utils import ThreeArrays, TwoArrays
 
 
 def e0_choo_siow_heteroskedastic(muhat: Matching) -> np.ndarray:
     """Returns the values of the parameter-independent part $e_0$
     for the Choo and Siow heteroskedastic model;
     we normalized $\\sigma_1=1$
 
@@ -26,15 +26,15 @@
         of the first derivative of the entropy
     """
     muxy, mux0, *_ = muhat.unpack()
     mu1y = muxy[0, :]
     mu10 = mux0[0]
     e0_vals = np.zeros_like(muxy)
     e0_vals[0, :] = -np.log(mu1y / mu10)
-    return e0_vals
+    return cast(np.ndarray, e0_vals)
 
 
 def e0_derivative_mu_heteroskedastic(
     muhat: Matching,
 ) -> ThreeArrays:
     """Returns the derivatives of the parameter-independent part $e_0$
     wrt $\\mu$ for the Choo and Siow heteroskedastic model;
@@ -210,17 +210,15 @@
 )
 
 entropy_choo_siow_heteroskedastic = EntropyFunctions(
     e0_fun=e0_choo_siow_heteroskedastic,
     parameter_dependent=True,
     e_fun=e_choo_siow_heteroskedastic,
     hessian="provided",
-    e0_derivative=cast(
-        EntropyHessians, e0_derivative_choo_siow_heteroskedastic
-    ),
+    e0_derivative=cast(EntropyHessians, e0_derivative_choo_siow_heteroskedastic),
     e_derivative=cast(EntropyHessians, e_derivative_choo_siow_heteroskedastic),
     description="Choo and Siow heteroskedastic with analytic Hessian",
 )
 
 entropy_choo_siow_heteroskedastic_numeric = EntropyFunctions(
     e0_fun=e0_choo_siow_heteroskedastic,
     parameter_dependent=True,
```

### Comparing `cupid_matching-1.0.8/cupid_matching/cupid_streamlit.py` & `cupid_matching-1.1.0/cupid_matching/cupid_streamlit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from math import pow
-from typing import Any, Optional
+from typing import Any, cast
 
 import altair as alt
 import numpy as np
 import pandas as pd
 import streamlit as st
+from bs_python_utils.bsnputils import (
+    check_matrix,
+    check_vector,
+    nprepeat_col,
+    nprepeat_row,
+)
+from bs_python_utils.bsutils import bs_error_abort
 
 from cupid_matching.choo_siow import entropy_choo_siow
 from cupid_matching.matching_utils import Matching
 from cupid_matching.min_distance import estimate_semilinear_mde
 from cupid_matching.model_classes import ChooSiowPrimitives
 from cupid_matching.poisson_glm import choo_siow_poisson_glm
-from cupid_matching.utils import (
-    bs_error_abort,
-    nprepeat_col,
-    nprepeat_row,
-    test_matrix,
-    test_vector,
-)
 
 
 def _make_profile(lambda_val: float, n: int, ncat: int) -> np.ndarray:
     """
     Creates a profile of numbers of individuals by type
     that changes exponentially
 
@@ -30,17 +30,15 @@
         n: the total number of individuals on that side of the market
         ncat: the number of types on that side of the market
 
     Returns:
         n_types: the number of individuals of each type
     """
     n1 = n * (lambda_val - 1.0) / (pow(lambda_val, ncat) - 1.0)
-    n_types = n1 * np.logspace(
-        base=lambda_val, start=0, stop=ncat - 1, num=ncat
-    )
+    n_types = n1 * np.logspace(base=lambda_val, start=0, stop=ncat - 1, num=ncat)
     return n_types
 
 
 def _make_margins(n: int, ncat: int, scenario: str = "Constant") -> np.ndarray:
     """generates the numbers by type on one side of the market
 
     Args:
@@ -91,46 +89,42 @@
             "Standard errors": stderrs,
         },
         index=coeff_names,
     )
     return st.table(df_coeffs_estimates)
 
 
-def _plot_heatmap(mat: np.ndarray, str_tit: Optional[str] = None) -> alt.Chart:
+def _plot_heatmap(mat: np.ndarray, str_tit: str | None = None) -> alt.Chart:
     """Plots a heatmap of the matrix
 
     Args:
         mat: the matrix to plot
         str_tit: a title, if any
 
     Returns:
         the heatmap
     """
-    ncat_men, ncat_women = test_matrix(mat)
+    ncat_men, ncat_women = check_matrix(mat)
     mat_arr = np.empty((mat.size, 4))
     mat_min = np.min(mat)
     i = 0
     for ix in range(ncat_men):
         for iy in range(ncat_women):
             m = mat[ix, iy]
             s = m - mat_min + 1
             mat_arr[i, :] = np.array([ix, iy, m, s])
             i += 1
 
     mat_df = pd.DataFrame(mat_arr, columns=["Men", "Women", "Value", "Size"])
     mat_df = mat_df.astype(
         dtype={"Men": int, "Women": int, "Value": float, "Size": float}
     )
-    base = alt.Chart(mat_df).encode(
-        x="Men:O", y=alt.Y("Women:O", sort="descending")
-    )
+    base = alt.Chart(mat_df).encode(x="Men:O", y=alt.Y("Women:O", sort="descending"))
     mat_map = base.mark_circle(opacity=0.4).encode(
-        size=alt.Size(
-            "Size:Q", legend=None, scale=alt.Scale(range=[1000, 10000])
-        ),
+        size=alt.Size("Size:Q", legend=None, scale=alt.Scale(range=[1000, 10000])),
         # color=alt.Color("Value:Q"),
         # tooltip=alt.Tooltip('Value', format=".2f")
     )
     text = base.mark_text(baseline="middle", fontSize=16).encode(
         text=alt.Text("Value:Q", format=".2f"),
     )
     if str_tit is None:
@@ -146,26 +140,22 @@
     Args:
         xvals: the numbers of singles by type
         str_gender: the side of the market, "men" or "women"
 
     Returns:
         the histogram
     """
-    ncat = test_vector(xvals)
+    ncat = check_vector(xvals)
     if str_gender not in ["men", "women"]:
         bs_error_abort(f"{str_gender} is not a valid side")
     str_cat = "x" if str_gender == "men" else "y"
     str_val = f"Single {str_gender}"
-    source = pd.DataFrame(
-        {str_cat: np.arange(1, ncat + 1, dtype=int), str_val: xvals}
-    )
+    source = pd.DataFrame({str_cat: np.arange(1, ncat + 1, dtype=int), str_val: xvals})
 
-    g_bars = (
-        alt.Chart(source).mark_bar().encode(y=str_cat + ":O", x=str_val + ":Q")
-    )
+    g_bars = alt.Chart(source).mark_bar().encode(y=str_cat + ":O", x=str_val + ":Q")
     return g_bars.properties(width=300, height=300)
 
 
 def _plot_bars(mux0: np.ndarray, mu0y: np.ndarray) -> alt.Chart:
     """concatenates the two gender singles histograms
 
     Args:
@@ -244,20 +234,20 @@
 
 a minimum distance estimator and a Poisson GLM estimator.
 """
 )
 
 list_nhh = [10_000, 100_000, 1_000_000]
 st.sidebar.subheader("First, choose the total number of households")
-n_households = st.sidebar.radio("Number of households", list_nhh)
+n_households = cast(int, st.sidebar.radio("Number of households", list_nhh))
 
 list_ncat = [2, 3, 5, 10]
 st.sidebar.subheader("Now choose the numbers of types of each gender")
-ncat_men = st.sidebar.radio("Number of categories of men", list_ncat)
-ncat_women = st.sidebar.radio("Number of categories of women", list_ncat)
+ncat_men = cast(int, st.sidebar.radio("Number of categories of men", list_ncat))
+ncat_women = cast(int, st.sidebar.radio("Number of categories of women", list_ncat))
 
 enough_cells = (ncat_men - 1) * (ncat_women - 1) > 6
 
 xvals = np.arange(ncat_men) + 1
 yvals = np.arange(ncat_women) + 1
 
 if enough_cells:
@@ -275,19 +265,19 @@
         """
     By default each category within a gender has the same number of individuals.
     You can also have the number increase by a factor two across categories, or decrease.
     """
     )
 
     list_scenarii = ["Constant", "Increasing", "Decreasing"]
-    scenario_men = st.sidebar.radio(
-        "Profile across categories for men", list_scenarii
+    scenario_men = cast(
+        str, st.sidebar.radio("Profile across categories for men", list_scenarii)
     )
-    scenario_women = st.sidebar.radio(
-        "Profile across categories for women", list_scenarii
+    scenario_women = cast(
+        str, st.sidebar.radio("Profile across categories for women", list_scenarii)
     )
 
     nx = _make_margins(proportion_men, ncat_men, scenario_men)
     my = _make_margins(1.0 - proportion_men, ncat_women, scenario_women)
 
     bases = np.zeros((ncat_men, ncat_women, 6))
     bases[:, :, 0] = 1.0
@@ -295,20 +285,16 @@
     yvals_mat = nprepeat_row(yvals, ncat_men)
     bases[:, :, 1] = xvals_mat
     bases[:, :, 2] = yvals_mat
     bases[:, :, 3] = xvals_mat * xvals_mat
     bases[:, :, 4] = np.outer(xvals, yvals)
     bases[:, :, 5] = yvals_mat * yvals_mat
 
-    st.sidebar.write(
-        "Finally, choose the coefficients of the 6 basis functions:"
-    )
-    st.sidebar.latex(
-        r"\Phi_{xy}=c_0+c_1 x + c_2 y + c_3 x^2 + c_4 x y + c_5 y^2"
-    )
+    st.sidebar.write("Finally, choose the coefficients of the 6 basis functions:")
+    st.sidebar.latex(r"\Phi_{xy}=c_0+c_1 x + c_2 y + c_3 x^2 + c_4 x y + c_5 y^2")
     min_c = np.array([-3.0] + [-2.0 / ncat_men] * 5)
     max_c = np.array([3.0] + [2.0 / ncat_women] * 5)
     true_coeffs = np.zeros(6)
     coeff_names = [f"c[{i}]" for i in range(6)]
 
     if "randoms" not in st.session_state:
         random_coeffs = np.round(min_c + (max_c - min_c) * np.random.rand(6), 2)
@@ -376,56 +362,53 @@
         "Estimating the parameters of the quadratic joint surplus $\\mathbb{\\Phi}$"
     )
 
     if st.button("Estimate"):
         col1, col2 = st.columns(2)
         with col1:
             st.markdown(
-                "#### Below: the minimum distance estimator in Galichon and Salanié (2023)."
+                "#### Below: the minimum distance estimator in Galichon and Salanié"
+                " (2023)."
             )
             st.write("It also gives us a specification test.")
-            mde_results = estimate_semilinear_mde(
-                mus_sim, bases, entropy_choo_siow
-            )
+            mde_results = estimate_semilinear_mde(mus_sim, bases, entropy_choo_siow)
             mde_estimates = mde_results.estimated_coefficients
             mde_stderrs = mde_results.stderrs_coefficients
 
-            _table_estimates(
-                coeff_names, true_coeffs, mde_estimates, mde_stderrs
-            )
+            _table_estimates(coeff_names, true_coeffs, mde_estimates, mde_stderrs)
 
             specif_test_stat = round(mde_results.test_statistic, 2)
             specif_test_pval = round(mde_results.test_pvalue, 2)
             st.write(
-                f"Test statistic: chi2({mde_results.ndf}) = {specif_test_stat} has p-value {specif_test_pval}"
+                f"Test statistic: chi2({mde_results.ndf}) = {specif_test_stat} has"
+                f" p-value {specif_test_pval}"
             )
 
         with col2:
             st.markdown(
                 "#### Here is the Poisson GLM estimator in Galichon and Salanié (2023);"
             )
             st.markdown(
                 """ 
                 as it requires numerical optimization, it is a bit slower.
                 """
             )
             st.write(
-                "It also gives us the estimates of the expected utilities $u_x$ and $v_y$."
+                "It also gives us the estimates of the expected utilities $u_x$ and"
+                " $v_y$."
             )
 
             pglm_results = choo_siow_poisson_glm(mus_sim, bases)
 
             u = pglm_results.estimated_u
             v = pglm_results.estimated_v
             pglm_estimates = pglm_results.estimated_beta
             pglm_stderrs = pglm_results.stderrs_beta
 
-            _table_estimates(
-                coeff_names, true_coeffs, pglm_estimates, pglm_stderrs
-            )
+            _table_estimates(coeff_names, true_coeffs, pglm_estimates, pglm_stderrs)
 
             x_names = [str(x) for x in range(ncat_men)]
             y_names = [str(y) for y in range(ncat_women)]
 
             st.write("The expected utilities are:")
             df_u_estimates = pd.DataFrame(
                 {"Estimated": u, "True": -np.log(mux0_sim / n_sim)},
```

### Comparing `cupid_matching-1.0.8/cupid_matching/entropy.py` & `cupid_matching-1.1.0/cupid_matching/entropy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Entropies and their derivatives. """
 from dataclasses import dataclass
 from functools import partial
-from typing import Any, Callable, Literal, Optional, cast
+from typing import Any, Callable, Literal, cast
 
 import numpy as np
+from bs_python_utils.bsnputils import ThreeArrays, TwoArrays
+from bs_python_utils.bsutils import bs_error_abort
 
 from cupid_matching.matching_utils import (
     Matching,
     MatchingFunction,
     MatchingFunctionParam,
 )
-from cupid_matching.utils import _EPS, _TWO_EPS, ThreeArrays, TwoArrays, bs_error_abort
+from cupid_matching.utils import _EPS, _TWO_EPS
 
 EntropyHessianMuMu = Callable[[Matching], ThreeArrays]
 """The type of a function that takes in a Matching
    and returns the three components of the hessian of the entropy
    wrt $(\\mu,\\mu)$.
 """
 
@@ -59,15 +61,15 @@
         e0_fun: required
         parameter_dependent:  if `True`, the entropy depends on parameters.
             Defaults to `False`
         e_fun: only in entropies that depend on parameters.
             Defaults to `None`
         hessian: defaults to `"numeric"`
             * if `"provided"`, we provide the hessian of the entropy.
-            * if `"numerical"`, it is computed by central differences.
+            * if `"numerical"`, it is compute_d by central differences.
         e0_derivative: the derivative of `e0_fun`, if available.
             Defaults to `None`
         e_derivative: the derivative of `e_fun`, if available.
             Defaults to `None`
         additional_parameters: additional parameters
             that define the distribution of errors.
             Defaults to `None`
@@ -75,30 +77,33 @@
             Defaults to `None`
 
     Examples:
         See `entropy_choo_siow` in `choo_siow.py`
     """
 
     e0_fun: MatchingFunction | MatchingFunctionParam
-    e0_derivative: Optional[EntropyHessians | EntropyHessiansParam] = None
-    additional_parameters: Optional[list] = None
-    description: Optional[str] = None
-    e_fun: Optional[MatchingFunction | MatchingFunctionParam] = None
-    e_derivative: Optional[EntropyHessians | EntropyHessiansParam] = None
-    hessian: Optional[str] = "numerical"
+    e0_derivative: EntropyHessians | EntropyHessiansParam | None = None
+    additional_parameters: list | None = None
+    description: str | None = None
+    e_fun: MatchingFunction | MatchingFunctionParam | None = None
+    e_derivative: EntropyHessians | EntropyHessiansParam | None = None
+    hessian: str | None = "numerical"
     parameter_dependent: bool = False
 
     def __post_init__(self):
-        if not self.parameter_dependent:
-            if self.hessian == "provided" and self.e0_derivative is None:
-                bs_error_abort(
-                    "You claim to provide the hessian "
-                    + "but you did not provide the e0_derivative."
-                )
-        else:
+        if (
+            (not self.parameter_dependent)
+            and self.hessian == "provided"
+            and self.e0_derivative is None
+        ):
+            bs_error_abort(
+                "You claim to provide the hessian "
+                + "but you did not provide the e0_derivative."
+            )
+        if self.parameter_dependent:
             if self.e_fun is None:
                 bs_error_abort(
                     "Your entropy is parameter dependent "
                     + " but you did not provide the e_fun."
                 )
             if self.hessian == "provided" and self.e_derivative is None:
                 bs_error_abort(
@@ -107,16 +112,16 @@
                     + " but I do not see the e_derivative."
                 )
 
 
 def entropy_gradient(
     entropy: EntropyFunctions,
     muhat: Matching,
-    alpha: Optional[np.ndarray] = None,
-    additional_parameters: Optional[list] = None,
+    alpha: np.ndarray | None = None,
+    additional_parameters: list | None = None,
 ) -> np.ndarray:
     """Computes the derivative of the entropy wrt $\\mu$
      at $(\\mu, n, m, \\alpha, p)$
 
     Args:
         entropy: the `EntropyFunctions` object
         muhat: a Matching
@@ -144,15 +149,15 @@
         else:
             if additional_parameters is not None:
                 e_fun = cast(MatchingFunctionParam, e_fun)
                 e_vals = e_fun(muhat, additional_parameters)
             else:
                 e_fun = cast(MatchingFunction, e_fun)
                 e_vals = e_fun(muhat)
-        return e0_vals + e_vals @ alpha
+        return cast(np.ndarray, e0_vals + e_vals @ alpha)
     else:
         return e0_vals
 
 
 def _numeric_component(
     muhat: Matching,
     x: int,
@@ -205,22 +210,22 @@
         mus = Matching(muxy, n, m)
         der_entropy_plus = entropy_deriv(mus)
         m[y] -= _TWO_EPS
     else:
         bs_error_abort("Wrong direction parameter.")
     der_entropy_minus = entropy_deriv(mus)
     deriv_value = (der_entropy_plus[x, y] - der_entropy_minus[x, y]) / _TWO_EPS
-    return deriv_value
+    return cast(float, deriv_value)
 
 
 def _numeric_hessian(
     entropy: EntropyFunctions,
     muhat: Matching,
-    alpha: Optional[np.ndarray] = None,
-    additional_parameters: Optional[list] = None,
+    alpha: np.ndarray | None = None,
+    additional_parameters: list | None = None,
 ) -> EntropyHessianComponents:
     """Evaluates numerically the components of the hessians of the entropy
     wrt $(\\mu,\\mu)$ and $(\\mu,(n,m))$
 
     Args:
         entropy: the `EntropyFunctions` object
         muhat: a Matching
```

### Comparing `cupid_matching-1.0.8/cupid_matching/example_nestedlogit.py` & `cupid_matching-1.1.0/cupid_matching/example_nested_logit.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 One nest on each side must consist of the 0 option.
 The other nests are specified as nested lists.
 E.g. [[1, 3], [2,4]] describes two nests, one with types 1 and 3,
 and the other with types 2 and 4.
 On each side, the nests are the same for each type, with the same parameters.
 """
 
-from typing import Optional, Tuple
+from typing import cast
 
 import numpy as np
+from bs_python_utils.bsutils import print_stars
 
 from cupid_matching.entropy import EntropyFunctions
 from cupid_matching.min_distance import estimate_semilinear_mde
 from cupid_matching.model_classes import Matching, NestedLogitPrimitives
 from cupid_matching.nested_logit import setup_standard_nested_logit
-from cupid_matching.utils import print_stars
 
 
 def create_nestedlogit_population(
     X: int,
     Y: int,
     K: int,
-    std_alphas: Optional[float] = 0.5,
-    std_betas: Optional[float] = 1.0,
-) -> Tuple[
+    std_alphas: float = 0.5,
+    std_betas: float = 1.0,
+) -> tuple[
     NestedLogitPrimitives,
     np.ndarray,
     np.ndarray,
     EntropyFunctions,
     EntropyFunctions,
 ]:
     """
@@ -108,26 +108,26 @@
     mde_results = estimate_semilinear_mde(
         mus_sim,
         phi_bases,
         entropy,
         additional_parameters=entropy.additional_parameters,
     )
     mde_discrepancy = mde_results.print_results(true_coeffs=true_coeffs)
-    return mde_discrepancy
+    return cast(float, mde_discrepancy)
 
 
 (
     nested_logit_instance,
     phi_bases,
     true_coeffs,
     entropy_nested_logit,
     entropy_nested_logit_numeric,
 ) = create_nestedlogit_population(20, 18, 6)
 seed = 6475788
-n_households = 1e6
+n_households = 1_000_000
 mus_sim = nested_logit_instance.simulate(n_households, seed)
 mde_discrepancy = mde_estimate(
     mus_sim,
     phi_bases,
     true_coeffs,
     entropy_nested_logit,
     "RESULTS FOR MDE WITH ANALYTICAL GRADIENT",
```

### Comparing `cupid_matching-1.0.8/cupid_matching/ipfp_solvers.py` & `cupid_matching-1.1.0/cupid_matching/ipfp_solvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,42 +17,40 @@
 in all primitives.
 """
 from math import sqrt
 from typing import Literal, overload
 
 import numpy as np
 import scipy.linalg as spla
-
-from cupid_matching.matching_utils import Matching
-from cupid_matching.utils import (
-    bs_error_abort,
-    der_nppow,
+from bs_python_utils.bsnputils import (
+    FourArrays,
+    ThreeArrays,
+    check_vector,
     npexp,
     npmaxabs,
     nppow,
     nprepeat_col,
     nprepeat_row,
-    test_vector,
 )
+from bs_python_utils.bsutils import bs_error_abort
 
-ThreeArrays = tuple[np.ndarray, np.ndarray, np.ndarray]
-FourArrays = tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]
+from cupid_matching.matching_utils import Matching
 
 IPFPNoGradientResults = tuple[Matching, np.ndarray, np.ndarray]
 IPFPGradientResults = tuple[
     Matching, np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray
 ]
 
 
 def _ipfp_check_sizes(
     men_margins: np.ndarray, women_margins: np.ndarray, Phi: np.ndarray
 ) -> tuple[int, int]:
     """checks that the margins and surplus have the correct shapes and sizes"""
-    X = test_vector(men_margins)
-    Y = test_vector(women_margins)
+    X = check_vector(men_margins)
+    Y = check_vector(women_margins)
     if Phi.shape != (X, Y):
         bs_error_abort(f"The shape of Phi should be ({X}, {Y}")
     return X, Y
 
 
 @overload
 def ipfp_homoskedastic_nosingles_solver(
@@ -109,15 +107,15 @@
     X, Y = _ipfp_check_sizes(men_margins, women_margins, Phi)
     n_couples = np.sum(men_margins)
 
     # check that there are as many men as women
     if np.abs(np.sum(women_margins) - n_couples) > n_couples * tol:
         bs_error_abort("There should be as many men as women")
 
-    ephi2, der_ephi2 = npexp(Phi / 2.0, deriv=True)
+    ephi2, der_ephi2 = npexp(Phi / 2.0, deriv=1)
     ephi2T = ephi2.T
 
     #############################################################################
     # we solve the equilibrium equations muxy = ephi2 * tx * ty
     #   starting with a reasonable initial point for tx and ty: : tx = ty = bigc
     #   it is important that it fit the number of individuals
     #############################################################################
@@ -160,40 +158,36 @@
         lhs[X:, X:] = np.diag(syi)
         lhs[X:, :X] = ephi2T * tyi.reshape((-1, 1))
 
         # now fill the RHS
         n_cols_rhs = n_prod_categories
         rhs = np.zeros((n_sum_categories, n_cols_rhs))
 
-        #  to compute derivatives of (txi, tyi) wrt Phi
+        #  to compute_ derivatives of (txi, tyi) wrt Phi
         der_ephi2 /= 2.0 * ephi2  # 1/2 with safeguards
         ivar = 0
         for iman in range(X):
             rhs[iman, ivar : (ivar + Y)] = -muxy[iman, :] * der_ephi2[iman, :]
             ivar += Y
         ivar1 = X
         ivar2 = 0
         for iwoman in range(Y):
-            rhs[ivar1, ivar2:n_cols_rhs:Y] = (
-                -muxy[:, iwoman] * der_ephi2[:, iwoman]
-            )
+            rhs[ivar1, ivar2:n_cols_rhs:Y] = -muxy[:, iwoman] * der_ephi2[:, iwoman]
             ivar1 += 1
             ivar2 += 1
         # solve for the derivatives of txi and tyi
         dt_dT = spla.solve(lhs, rhs)
         dt = dt_dT[:X, :]
         dT = dt_dT[X:, :]
         # now construct the derivatives of muxy
         dmuxy = np.zeros((n_prod_categories, n_cols_rhs))
         ivar = 0
         for iman in range(X):
             dt_man = dt[iman, :]
-            dmuxy[ivar : (ivar + Y), :] = np.outer(
-                (ephi2[iman, :] * tyi), dt_man
-            )
+            dmuxy[ivar : (ivar + Y), :] = np.outer((ephi2[iman, :] * tyi), dt_man)
             ivar += Y
         for iwoman in range(Y):
             dT_woman = dT[iwoman, :]
             dmuxy[iwoman:n_prod_categories:Y, :] += np.outer(
                 (ephi2[:, iwoman] * txi), dT_woman
             )
         # add the term that comes from differentiating ephi2
@@ -264,15 +258,15 @@
         mus, marg_err_x, marg_err_y = ipfp_homoskedastic_solver(
             true_surplus_matrix, men_margins, women_margins, tol=1e-12
         )
         ```
     """
     X, Y = _ipfp_check_sizes(men_margins, women_margins, Phi)
 
-    ephi2, der_ephi2 = npexp(Phi / 2.0, deriv=True)
+    ephi2, der_ephi2 = npexp(Phi / 2.0, deriv=1)
 
     #############################################################################
     # we solve the equilibrium equations muxy = ephi2 * tx * ty
     #   where mux0=tx**2  and mu0y=ty**2
     #   starting with a reasonable initial point for tx and ty: tx = ty = bigc
     #   it is important that it fit the number of individuals
     #############################################################################
@@ -308,60 +302,56 @@
         print(f"\tMargin error on y: {npmaxabs(marg_err_y)}")
     if not gr:
         return (
             Matching(muxy, men_margins, women_margins),
             marg_err_x,
             marg_err_y,
         )
-    else:  # we compute the derivatives
+    else:  # we compute_ the derivatives
         sxi = ephi2 @ tyi
         syi = ephi2T @ txi
         n_sum_categories = X + Y
         n_prod_categories = X * Y
         # start with the LHS of the linear system
         lhs = np.zeros((n_sum_categories, n_sum_categories))
         lhs[:X, :X] = np.diag(2.0 * txi + sxi)
         lhs[:X, X:] = ephi2 * txi.reshape((-1, 1))
         lhs[X:, X:] = np.diag(2.0 * tyi + syi)
         lhs[X:, :X] = ephi2T * tyi.reshape((-1, 1))
         # now fill the RHS
         n_cols_rhs = n_sum_categories + n_prod_categories
         rhs = np.zeros((n_sum_categories, n_cols_rhs))
-        #  to compute derivatives of (txi, tyi) wrt men_margins
+        #  to compute_ derivatives of (txi, tyi) wrt men_margins
         rhs[:X, :X] = np.eye(X)
-        #  to compute derivatives of (txi, tyi) wrt women_margins
+        #  to compute_ derivatives of (txi, tyi) wrt women_margins
         rhs[X:n_sum_categories, X:n_sum_categories] = np.eye(Y)
-        #  to compute derivatives of (txi, tyi) wrt Phi
+        #  to compute_ derivatives of (txi, tyi) wrt Phi
         der_ephi2 /= 2.0 * ephi2  # 1/2 with safeguards
         ivar = n_sum_categories
         for iman in range(X):
             rhs[iman, ivar : (ivar + Y)] = -muxy[iman, :] * der_ephi2[iman, :]
             ivar += Y
         ivar1 = X
         ivar2 = n_sum_categories
         for iwoman in range(Y):
-            rhs[ivar1, ivar2:n_cols_rhs:Y] = (
-                -muxy[:, iwoman] * der_ephi2[:, iwoman]
-            )
+            rhs[ivar1, ivar2:n_cols_rhs:Y] = -muxy[:, iwoman] * der_ephi2[:, iwoman]
             ivar1 += 1
             ivar2 += 1
         # solve for the derivatives of txi and tyi
         dt_dT = spla.solve(lhs, rhs)
         dt = dt_dT[:X, :]
         dT = dt_dT[X:, :]
         # now construct the derivatives of the mus
         dmux0 = 2.0 * (dt * txi.reshape((-1, 1)))
         dmu0y = 2.0 * (dT * tyi.reshape((-1, 1)))
         dmuxy = np.zeros((n_prod_categories, n_cols_rhs))
         ivar = 0
         for iman in range(X):
             dt_man = dt[iman, :]
-            dmuxy[ivar : (ivar + Y), :] = np.outer(
-                (ephi2[iman, :] * tyi), dt_man
-            )
+            dmuxy[ivar : (ivar + Y), :] = np.outer((ephi2[iman, :] * tyi), dt_man)
             ivar += Y
         for iwoman in range(Y):
             dT_woman = dT[iwoman, :]
             dmuxy[iwoman:n_prod_categories:Y, :] += np.outer(
                 (ephi2[:, iwoman] * txi), dT_woman
             )
         # add the term that comes from differentiating ephi2
@@ -570,15 +560,15 @@
 
     if np.min(sigma_x) <= 0.0:
         bs_error_abort("All elements of sigma_x must be positive")
     if np.min(tau_y) <= 0.0:
         bs_error_abort("All elements of tau_y must be positive")
 
     sumxy1 = 1.0 / np.add.outer(sigma_x, tau_y)
-    ephi2, der_ephi2 = npexp(Phi * sumxy1, deriv=True)
+    ephi2, der_ephi2 = npexp(Phi * sumxy1, deriv=1)
 
     #############################################################################
     # we solve the equilibrium equations muxy = ephi2 * tx * ty
     #   with tx = mux0^(sigma_x/(sigma_x + tau_max))
     #   and ty = mu0y^(tau_y/(sigma_max + tau_y))
     #   starting with a reasonable initial point for tx and ty: tx = ty = bigc
     #   it is important that it fit the number of individuals
@@ -605,44 +595,36 @@
         # Newton iterates for men
         err_newton = bigc
         txin = txi.copy()
         mu0y_in = np.power(np.power(tyi, sigmax_tau), 1.0 / tau_y)
         while err_newton > tol_newton:
             txit = np.power(txin, sig_taumax)
             mux0_in = np.power(txit, 1.0 / sigma_x)
-            out_xy = np.outer(
-                np.power(mux0_in, sigma_x), np.power(mu0y_in, tau_y)
-            )
+            out_xy = np.outer(np.power(mux0_in, sigma_x), np.power(mu0y_in, tau_y))
             muxy_in = ephi2 * np.power(out_xy, sumxy1)
             errxi = mux0_in + np.sum(muxy_in, 1) - men_margins
             err_newton = npmaxabs(errxi)
             txin -= errxi / (
-                sig_taumax
-                * (mux0_in / sigma_x + np.sum(sumxy1 * muxy_in, 1))
-                / txin
+                sig_taumax * (mux0_in / sigma_x + np.sum(sumxy1 * muxy_in, 1)) / txin
             )
         tx = txin
 
         # Newton iterates for women
         err_newton = bigc
         tyin = tyi.copy()
         mux0_in = np.power(np.power(tx, sig_taumax), 1.0 / sigma_x)
         while err_newton > tol_newton:
             tyit = np.power(tyin, sigmax_tau)
             mu0y_in = np.power(tyit, 1.0 / tau_y)
-            out_xy = np.outer(
-                np.power(mux0_in, sigma_x), np.power(mu0y_in, tau_y)
-            )
+            out_xy = np.outer(np.power(mux0_in, sigma_x), np.power(mu0y_in, tau_y))
             muxy_in = ephi2 * np.power(out_xy, sumxy1)
             erryi = mu0y_in + np.sum(muxy_in, 0) - women_margins
             err_newton = npmaxabs(erryi)
             tyin -= erryi / (
-                sigmax_tau
-                * (mu0y_in / tau_y + np.sum(sumxy1 * muxy_in, 0))
-                / tyin
+                sigmax_tau * (mu0y_in / tau_y + np.sum(sumxy1 * muxy_in, 0)) / tyin
             )
 
         ty = tyin
 
         err_x = npmaxabs(tx - txi)
         err_y = npmaxabs(ty - tyi)
         err_diff = err_x + err_y
@@ -664,27 +646,27 @@
         print(f"\tMargin error on y: {npmaxabs(marg_err_y)}")
     if not gr:
         return (
             Matching(muxy, men_margins, women_margins),
             marg_err_x,
             marg_err_y,
         )
-    else:  # we compute the derivatives
+    else:  # we compute_ the derivatives
         n_sum_categories = X + Y
         n_prod_categories = X * Y
         # we work directly with (mux0, mu0y)
         sigrat_xy = sumxy1 * sigma_x.reshape((-1, 1))
         taurat_xy = 1.0 - sigrat_xy
         mux0_mat = nprepeat_col(mux0, Y)
         mu0y_mat = nprepeat_row(mu0y, X)
         # muxy = axy * bxy * ephi2
         axy = nppow(mux0_mat, sigrat_xy)
         bxy = nppow(mu0y_mat, taurat_xy)
-        der_axy1, der_axy2 = der_nppow(mux0_mat, sigrat_xy)
-        der_bxy1, der_bxy2 = der_nppow(mu0y_mat, taurat_xy)
+        der_axy1, der_axy2 = nppow(mux0_mat, sigrat_xy, deriv=1)
+        der_bxy1, der_bxy2 = nppow(mu0y_mat, taurat_xy, deriv=1)
         der_axy1_rat, der_axy2_rat = der_axy1 / axy, der_axy2 / axy
         der_bxy1_rat, der_bxy2_rat = der_bxy1 / bxy, der_bxy2 / bxy
 
         # start with the LHS of the linear system on (dmux0, dmu0y)
         lhs = np.zeros((n_sum_categories, n_sum_categories))
         lhs[:X, :X] = np.diag(1.0 + np.sum(muxy * der_axy1_rat, 1))
         lhs[:X, X:] = muxy * der_bxy1_rat
@@ -692,65 +674,63 @@
         lhs[X:, :X] = (muxy * der_axy1_rat).T
 
         # now fill the RHS (derivatives wrt men_margins, then men_margins,
         #    then Phi, then sigma_x and tau_y)
         n_cols_rhs = n_sum_categories + n_prod_categories + X + Y
         rhs = np.zeros((n_sum_categories, n_cols_rhs))
 
-        #  to compute derivatives of (mux0, mu0y) wrt men_margins
+        #  to compute_ derivatives of (mux0, mu0y) wrt men_margins
         rhs[:X, :X] = np.eye(X)
-        #  to compute derivatives of (mux0, mu0y) wrt women_margins
+        #  to compute_ derivatives of (mux0, mu0y) wrt women_margins
         rhs[X:, X:n_sum_categories] = np.eye(Y)
 
         #   the next line is sumxy1 with safeguards
         sumxy1_safe = sumxy1 * der_ephi2 / ephi2
 
         big_a = muxy * sumxy1_safe
         big_b = der_axy2_rat - der_bxy2_rat
         b_mu_s = big_b * muxy * sumxy1
         a_phi = Phi * big_a
         big_c = sumxy1 * (a_phi - b_mu_s * tau_y)
         big_d = sumxy1 * (a_phi + b_mu_s * sigma_x.reshape((-1, 1)))
 
-        #  to compute derivatives of (mux0, mu0y) wrt Phi
+        #  to compute_ derivatives of (mux0, mu0y) wrt Phi
         ivar = n_sum_categories
         for iman in range(X):
             rhs[iman, ivar : (ivar + Y)] = -big_a[iman, :]
             ivar += Y
         ivar1 = X
         ivar2 = n_sum_categories
         iend_phi = n_sum_categories + n_prod_categories
         for iwoman in range(Y):
             rhs[ivar1, ivar2:iend_phi:Y] = -big_a[:, iwoman]
             ivar1 += 1
             ivar2 += 1
 
-        #  to compute derivatives of (mux0, mu0y) wrt sigma_x
+        #  to compute_ derivatives of (mux0, mu0y) wrt sigma_x
         iend_sig = iend_phi + X
         der_sigx = np.sum(big_c, 1)
         rhs[:X, iend_phi:iend_sig] = np.diag(der_sigx)
         rhs[X:, iend_phi:iend_sig] = big_c.T
-        #  to compute derivatives of (mux0, mu0y) wrt tau_y
+        #  to compute_ derivatives of (mux0, mu0y) wrt tau_y
         der_tauy = np.sum(big_d, 0)
         rhs[X:, iend_sig:] = np.diag(der_tauy)
         rhs[:X, iend_sig:] = big_d
 
         # solve for the derivatives of mux0 and mu0y
         dmu0 = spla.solve(lhs, rhs)
         dmux0 = dmu0[:X, :]
         dmu0y = dmu0[X:, :]
 
         # now construct the derivatives of muxy
         dmuxy = np.zeros((n_prod_categories, n_cols_rhs))
         der1 = ephi2 * der_axy1 * bxy
         ivar = 0
         for iman in range(X):
-            dmuxy[ivar : (ivar + Y), :] = np.outer(
-                der1[iman, :], dmux0[iman, :]
-            )
+            dmuxy[ivar : (ivar + Y), :] = np.outer(der1[iman, :], dmux0[iman, :])
             ivar += Y
         der2 = ephi2 * der_bxy1 * axy
         for iwoman in range(Y):
             dmuxy[iwoman:n_prod_categories:Y, :] += np.outer(
                 der2[:, iwoman], dmu0y[iwoman, :]
             )
```

### Comparing `cupid_matching-1.0.8/cupid_matching/min_distance.py` & `cupid_matching-1.1.0/cupid_matching/min_distance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """ Estimates semilinear separable models with a given entropy function.
 The entropy function and the surplus matrix must both be linear in the parameters.
 """
-from typing import Optional, cast
+from typing import cast
 
 import numpy as np
 import scipy.linalg as spla
 import scipy.stats as sts
+from bs_python_utils.bsutils import bs_error_abort, print_stars
 
 from cupid_matching.entropy import (
     EntropyFunctions,
     EntropyHessianMuMu,
     EntropyHessianMuMuParam,
     EntropyHessianMuR,
     EntropyHessianMuRParam,
@@ -19,27 +20,26 @@
     _fill_hessianMuR_from_components,
     _numeric_hessian,
 )
 from cupid_matching.matching_utils import (
     Matching,
     MatchingFunction,
     MatchingFunctionParam,
-    _make_XY_K_mat,
-    _variance_muhat,
+    variance_muhat,
 )
-from cupid_matching.min_distance_utils import MDEResults, _compute_estimates
-from cupid_matching.utils import bs_error_abort, print_stars
+from cupid_matching.min_distance_utils import MDEResults, compute_estimates
+from cupid_matching.utils import _make_XY_K_mat
 
 
 def estimate_semilinear_mde(
     muhat: Matching,
     phi_bases: np.ndarray,
     entropy: EntropyFunctions,
-    additional_parameters: Optional[list] = None,
-    initial_weights: Optional[np.ndarray] = None,
+    additional_parameters: list | None = None,
+    initial_weights: np.ndarray | None = None,
 ) -> MDEResults:
     """
     Estimates the parameters of the distributions and of the base functions.
 
     Args:
         muhat: the observed Matching
         phi_bases: an (X, Y, K) array of bases
@@ -117,46 +117,41 @@
         hessian = entropy.hessian
         if hessian == "provided":
             e0_derivative = cast(EntropyHessians, entropy.e0_derivative)
             if additional_parameters is None:
                 hessian_components_mumu = e0_derivative[0](muhat)
                 hessian_components_mur = e0_derivative[1](muhat)
             else:
-                e0_derivative1 = cast(
-                    EntropyHessiansParam, entropy.e0_derivative
-                )
+                e0_derivative1 = cast(EntropyHessiansParam, entropy.e0_derivative)
                 hessian_components_mumu = e0_derivative1[0](
                     muhat, additional_parameters
                 )
-                hessian_components_mur = e0_derivative1[1](
-                    muhat, additional_parameters
-                )
+                hessian_components_mur = e0_derivative1[1](muhat, additional_parameters)
         else:
             if additional_parameters is None:
                 hessian_components = _numeric_hessian(entropy, muhat)
             else:
                 hessian_components = _numeric_hessian(
                     entropy,
                     muhat,
                     additional_parameters=additional_parameters,
                 )
             (
                 hessian_components_mumu,
                 hessian_components_mur,
             ) = hessian_components
-        hessian_mumu = _fill_hessianMuMu_from_components(
-            hessian_components_mumu
-        )
+        hessian_mumu = _fill_hessianMuMu_from_components(hessian_components_mumu)
         hessian_mur = _fill_hessianMuR_from_components(hessian_components_mur)
         hessians_both = np.concatenate((hessian_mumu, hessian_mur), axis=1)
 
-        _, var_munm = _variance_muhat(muhat)
+        var_muhat = variance_muhat(muhat)
+        var_munm = var_muhat.var_munm
         var_entropy_gradient = hessians_both @ var_munm @ hessians_both.T
         S_mat = spla.inv(var_entropy_gradient)
-        estimated_coefficients, varcov_coefficients = _compute_estimates(
+        estimated_coefficients, varcov_coefficients = compute_estimates(
             phi_mat, S_mat, e0_hat
         )
         stderrs_coefficients = np.sqrt(np.diag(varcov_coefficients))
         est_Phi = phi_mat @ estimated_coefficients
         residuals = est_Phi + e0_hat
     else:  # parameterized entropy: e0(mu,r) + e(mu,r) . alpha
         # create the F matrix
@@ -167,48 +162,38 @@
             e_fun1 = cast(MatchingFunctionParam, entropy.e_fun)
             e_vals = e_fun1(muhat, additional_parameters)
         e_hat = _make_XY_K_mat(e_vals)
 
         F_hat = np.column_stack((e_hat, phi_mat))
         n_pars = e_hat.shape[1] + K
         # first pass with an initial weighting matrix
-        first_coeffs, _ = _compute_estimates(F_hat, S_mat, e0_hat)
+        first_coeffs, _ = compute_estimates(F_hat, S_mat, e0_hat)
         first_alpha = first_coeffs[:-K]
 
-        # compute the efficient weighting matrix
+        # compute_ the efficient weighting matrix
         hessian = entropy.hessian
         if hessian == "provided":
             if additional_parameters is None:
                 e0_derivative = cast(EntropyHessians, entropy.e0_derivative)
                 e_derivative = cast(EntropyHessians, entropy.e_derivative)
                 e0_derivative_mumu = cast(EntropyHessianMuMu, e0_derivative[0])
                 hessian_components_mumu_e0 = e0_derivative_mumu(muhat)
                 e0_derivative_mur = cast(EntropyHessianMuR, e0_derivative[1])
                 hessian_components_mur_e0 = e0_derivative_mur(muhat)
                 e_derivative_mumu = cast(EntropyHessianMuMu, e_derivative[0])
                 hessian_components_mumu_e = e_derivative_mumu(muhat)
                 e_derivative_mur = cast(EntropyHessianMuR, e_derivative[1])
                 hessian_components_mur_e = e_derivative_mur(muhat)
             else:
-                e0_derivative1 = cast(
-                    EntropyHessiansParam, entropy.e0_derivative
-                )
+                e0_derivative1 = cast(EntropyHessiansParam, entropy.e0_derivative)
                 e_derivative1 = cast(EntropyHessiansParam, entropy.e_derivative)
-                e0_derivative_mumu1 = cast(
-                    EntropyHessianMuMuParam, e0_derivative1[0]
-                )
-                e0_derivative_mur1 = cast(
-                    EntropyHessianMuRParam, e0_derivative1[1]
-                )
-                e_derivative_mumu1 = cast(
-                    EntropyHessianMuMuParam, e_derivative1[0]
-                )
-                e_derivative_mur1 = cast(
-                    EntropyHessianMuRParam, e_derivative1[1]
-                )
+                e0_derivative_mumu1 = cast(EntropyHessianMuMuParam, e0_derivative1[0])
+                e0_derivative_mur1 = cast(EntropyHessianMuRParam, e0_derivative1[1])
+                e_derivative_mumu1 = cast(EntropyHessianMuMuParam, e_derivative1[0])
+                e_derivative_mur1 = cast(EntropyHessianMuRParam, e_derivative1[1])
                 hessian_components_mumu_e0 = e0_derivative_mumu1(
                     muhat, additional_parameters
                 )
                 hessian_components_mur_e0 = e0_derivative_mur1(
                     muhat, additional_parameters
                 )
                 hessian_components_mumu_e = e_derivative_mumu1(
@@ -231,51 +216,42 @@
             )
             hessian_components_mur1 = (
                 hessian_components_mur_e0[0]
                 + hessian_components_mur_e[0] @ first_alpha,
                 hessian_components_mur_e0[1]
                 + hessian_components_mur_e[1] @ first_alpha,
             )
-            hessian_mumu = _fill_hessianMuMu_from_components(
-                hessian_components_mumu1
-            )
-            hessian_mur = _fill_hessianMuR_from_components(
-                hessian_components_mur1
-            )
+            hessian_mumu = _fill_hessianMuMu_from_components(hessian_components_mumu1)
+            hessian_mur = _fill_hessianMuR_from_components(hessian_components_mur1)
         else:  # numeric hessian
             if additional_parameters is None:
-                hessian_components = _numeric_hessian(
-                    entropy, muhat, alpha=first_alpha
-                )
+                hessian_components = _numeric_hessian(entropy, muhat, alpha=first_alpha)
             else:
                 hessian_components = _numeric_hessian(
                     entropy,
                     muhat,
                     alpha=first_alpha,
                     additional_parameters=additional_parameters,
                 )
             (
                 hessian_components_mumu,
                 hessian_components_mur,
             ) = hessian_components
-            hessian_mumu = _fill_hessianMuMu_from_components(
-                hessian_components_mumu
-            )
-            hessian_mur = _fill_hessianMuR_from_components(
-                hessian_components_mur
-            )
+            hessian_mumu = _fill_hessianMuMu_from_components(hessian_components_mumu)
+            hessian_mur = _fill_hessianMuR_from_components(hessian_components_mur)
 
         hessians_both = np.concatenate((hessian_mumu, hessian_mur), axis=1)
 
-        _, var_munm = _variance_muhat(muhat)
+        varmus = variance_muhat(muhat)
+        var_munm = varmus.var_munm
         var_entropy_gradient = hessians_both @ var_munm @ hessians_both.T
         S_mat = spla.inv(var_entropy_gradient)
 
         # second pass
-        estimated_coefficients, varcov_coefficients = _compute_estimates(
+        estimated_coefficients, varcov_coefficients = compute_estimates(
             F_hat, S_mat, e0_hat
         )
         est_alpha, est_beta = (
             estimated_coefficients[:-K],
             estimated_coefficients[-K:],
         )
         stderrs_coefficients = np.sqrt(np.diag(varcov_coefficients))
```

### Comparing `cupid_matching-1.0.8/cupid_matching/min_distance_utils.py` & `cupid_matching-1.1.0/cupid_matching/min_distance_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Utility programs used in `min_distance.py`.
 """
 from dataclasses import dataclass
-from typing import Optional
+from typing import cast
 
 import numpy as np
 import scipy.linalg as spla
+from bs_python_utils.bsnputils import npmaxabs
+from bs_python_utils.bsutils import print_stars
 
-from cupid_matching.utils import npmaxabs, print_stars
 
-
-def _compute_estimates(
+def compute_estimates(
     M: np.ndarray, S_mat: np.ndarray, d: np.ndarray
 ) -> tuple[np.ndarray, np.ndarray]:
     """Returns the QGLS estimates and their variance-covariance.
 
     Args:
         M: an (XY,p) matrix
         S_mat: an (XY, XY) weighting matrix
@@ -32,77 +32,77 @@
 
 @dataclass
 class MDEResults:
     """
     The results from minimum-distance estimation and testing.
 
     Args:
-        X: int
-        Y: int
-        K: int
-        number_households: int
-        estimated_coefficients: np.ndarray
-        varcov_coefficients: np.ndarray
-        stderrs_coefficients: np.ndarray
-        estimated_Phi: np.ndarray
-        test_statistic: float
-        test_pvalue: float
-        ndf: int
-        parameterized_entropy: Optional[bool] = False
+        X: the number of types of men
+        Y: the number of types of women
+        K: the number of bases
+        number_households: the number of households in the sample
+        estimated_coefficients: the estimated coefficients
+        varcov_coefficients: their eetimated var-covar
+        stderrs_coefficients: their estimated stderrs
+        estimated_Phi: the estimated joint surplus
+        test_statistic: the value of the misspecification statistic
+        test_pvalue: the p-value of the test
+        ndf: the number of degrees of freedom
+        parameterized_entropy: True if the derivative of the entropy has unknown parameters
     """
 
     X: int
     Y: int
     K: int
     number_households: int
     estimated_coefficients: np.ndarray
     varcov_coefficients: np.ndarray
     stderrs_coefficients: np.ndarray
     estimated_Phi: np.ndarray
     test_statistic: float
     test_pvalue: float
     ndf: int
-    parameterized_entropy: Optional[bool] = False
+    parameterized_entropy: bool | None = False
 
     def __str__(self):
         line_stars = "*" * 80 + "\n"
         if self.parameterized_entropy:
             n_alpha = self.estimated_coefficients.size - self.K
             entropy_str = f"     The entropy has {n_alpha} parameters."
         else:
             entropy_str = "     The entropy is parameter-free."
             n_alpha = 0
         model_str = f"The data has {self.number_households} households\n\n"
-        model_str += (
-            f"The model has {self.X}x{self.Y} margins\n {entropy_str} \n"
-        )
+        model_str += f"The model has {self.X}x{self.Y} margins\n {entropy_str} \n"
         model_str += f"We use {self.K} basis functions.\n\n"
         repr_str = line_stars + model_str
-        repr_str += (
-            "The estimated coefficients (and their standard errors) are\n\n"
-        )
+        repr_str += "The estimated coefficients (and their standard errors) are\n\n"
         if self.parameterized_entropy:
             for i, coeff in enumerate(self.estimated_coefficients[:n_alpha]):
                 repr_str += (
                     f"   alpha({i + 1}): {coeff: > 10.3f}  "
                     + f"({self.stderrs_coefficients[i]: .3f})\n"
                 )
             repr_str += "\n"
         for i, coeff in enumerate(self.estimated_coefficients[n_alpha:]):
             repr_str += (
                 f"   base {i + 1}: {coeff: > 10.3f} "
                 + f"({self.stderrs_coefficients[n_alpha + i]: .3f})\n"
             )
         repr_str += "\nSpecification test:\n"
-        repr_str += f"   the value of the test statistic is {self.test_statistic: > 10.3f}\n"
-        repr_str += f"     for a chi2({self.ndf}), the p-value is {self.test_pvalue: > 10.3f}\n"
+        repr_str += (
+            f"   the value of the test statistic is {self.test_statistic: > 10.3f}\n"
+        )
+        repr_str += (
+            f"     for a chi2({self.ndf}), the p-value is {self.test_pvalue: > 10.3f}\n"
+        )
         return repr_str + line_stars
 
     def print_results(
-        self, true_coeffs: Optional[np.ndarray] = None, n_alpha: int = 0
+        self, true_coeffs: np.ndarray | None = None, n_alpha: int = 0
     ) -> None | float:
         estimates = self.estimated_coefficients
         stderrs = self.stderrs_coefficients
 
         if true_coeffs is not None:
             repr_str = (
                 "The true and estimated coefficients "
@@ -117,20 +117,20 @@
                 repr_str += (
                     f"   base {i + 1}: {true_coeffs[j]: > 10.3f}  "
                     + f"{coeff: > 10.3f}  ({stderrs[j]: > 10.3f})\n"
                 )
             print_stars(repr_str)
             discrepancy = npmaxabs(true_coeffs - estimates)
             print_stars(
-                f"The largest difference between true and estimated coefficients is {discrepancy: .2e}"
+                "The largest difference between true and estimated coefficients is"
+                f" {discrepancy: .2e}"
             )
         else:
             repr_str = (
-                "The estimated coefficients "
-                + "(and their standard errors) are\n\n"
+                "The estimated coefficients " + "(and their standard errors) are\n\n"
             )
             for i, coeff in enumerate(estimates[:n_alpha]):
                 repr_str + f"{coeff: > 10.3f}  ({stderrs[i]: > 10.3f})\n"
                 repr_str += "\n"
             for i, coeff in enumerate(estimates[n_alpha:]):
                 j = n_alpha + i
                 repr_str += f"{coeff: > 10.3f}  ({stderrs[j]: > 10.3f})\n"
@@ -143,9 +143,9 @@
         )
         repr_str += (
             f"     for a chi2({self.ndf}), "
             + f"the p-value is {self.test_pvalue: > 10.3f}\n"
         )
         print_stars(repr_str)
         if true_coeffs is not None:
-            return discrepancy
+            return cast(float, discrepancy)
         return None
```

### Comparing `cupid_matching-1.0.8/cupid_matching/model_classes.py` & `cupid_matching-1.1.0/cupid_matching/model_classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 from dataclasses import dataclass
-from typing import Optional, cast
+from typing import cast
 
 import numpy as np
+from bs_python_utils.bsnputils import (
+    check_matrix,
+    check_vector,
+    npexp,
+    npmaxabs,
+    nppow,
+)
+from bs_python_utils.bsutils import (
+    bs_error_abort,
+    print_stars,
+)
 
-from cupid_matching.ipfp_solvers import IPFPNoGradientResults, ipfp_homoskedastic_solver
+from cupid_matching.ipfp_solvers import (
+    IPFPNoGradientResults,
+    ipfp_homoskedastic_solver,
+)
 from cupid_matching.matching_utils import (
     Matching,
-    _change_indices,
-    _compute_margins,
-    _find_nest_of,
     _simulate_sample_from_mus,
+    compute_margins,
 )
 from cupid_matching.utils import (
     Nest,
     NestsList,
-    bs_error_abort,
-    npexp,
-    npmaxabs,
-    nppow,
-    print_stars,
-    test_matrix,
-    test_vector,
+    _change_indices,
+    _find_nest_of,
 )
 
 
 @dataclass
 class ChooSiowPrimitives:
     Phi: np.ndarray
     n: np.ndarray
     m: np.ndarray
-    mus: Optional[Matching] = None
+    mus: Matching | None = None
 
     def __post_init__(self):
-        X, Y = test_matrix(self.Phi)
-        Xn = test_vector(self.n)
-        Ym = test_vector(self.m)
+        X, Y = check_matrix(self.Phi)
+        Xn = check_vector(self.n)
+        Ym = check_vector(self.m)
         if Xn != X:
-            bs_error_abort(
-                f"Phi is a ({X}, {Y}) matrix but n has {Xn} elements."
-            )
+            bs_error_abort(f"Phi is a ({X}, {Y}) matrix but n has {Xn} elements.")
         if Ym != Y:
-            bs_error_abort(
-                f"Phi is a ({X}, {Y}) matrix but m has {Ym} elements."
-            )
+            bs_error_abort(f"Phi is a ({X}, {Y}) matrix but m has {Ym} elements.")
 
     def ipfp_solve(self) -> Matching:
         mus, err_x, err_y = cast(
             IPFPNoGradientResults,
             ipfp_homoskedastic_solver(self.Phi, self.n, self.m),
         )
         muxy, mux0, mu0y, _, _ = mus.unpack()
-        n, m = _compute_margins(muxy, mux0, mu0y)
+        n, m = compute_margins(muxy, mux0, mu0y)
         return Matching(muxy, n, m)
 
-    def simulate(
-        self, n_households: int, seed: Optional[int] = None
-    ) -> Matching:
+    def simulate(self, n_households: int, seed: int | None = None) -> Matching:
         self.n_households = n_households
         self.mus = self.ipfp_solve()
         mus_sim = _simulate_sample_from_mus(self.mus, n_households, seed)
         return mus_sim
 
     def describe(self):
         X, Y = self.Phi.shape
@@ -76,59 +77,55 @@
     nests_for_each_x: NestsList  # given by user, e.g. [[1, 3], [2,4]] has y=1 and y=3 in first nest
     nests_for_each_y: NestsList
     nests_over_Y: NestsList  # rebased to zero: the above example becomes [[0, 2], [1,3]]
     nests_over_X: NestsList
     i_nest_of_x: Nest  # mapping x -> n'
     i_nest_of_y: Nest  # mapping y -> n
     n_alphas: int
-    mus: Optional[Matching] = None
-    true_alphas: Optional[np.ndarray] = None
+    mus: Matching | None = None
+    true_alphas: np.ndarray | None = None
 
     def __init__(
         self,
         Phi: np.ndarray,
         n: np.ndarray,
         m: np.ndarray,
         nests_for_each_x: NestsList,
         nests_for_each_y: NestsList,
-        true_alphas: Optional[np.ndarray] = None,
+        true_alphas: np.ndarray | None = None,
     ):
         """
         We only model two-level nested logit, with {0} as the first nest,
         and nests and nests parameters that do not depend on the type.
 
         Args:
             Phi: the (X,Y) joint surplus matrix
             n: the X-vector of men margins
             m: the X-vector of women margins
             nests_for_each_x: the composition of the nests over 1...Y, a list of r lists
             nests_for_each_y: the composition of the nests over 1...X, a list of d lists
             true_alphas: the true nest parameters, if any; should be an (r+d)-vector
         """
-        X, Y = test_matrix(Phi)
-        Xn = test_vector(n)
-        Ym = test_vector(m)
+        X, Y = check_matrix(Phi)
+        Xn = check_vector(n)
+        Ym = check_vector(m)
 
         # we need to rebase the indices to zero
         self.nests_over_X = _change_indices(nests_for_each_y)
         self.nests_over_Y = _change_indices(nests_for_each_x)
 
         self.n_alphas = len(nests_for_each_y) + len(nests_for_each_x)
 
         if Xn != X:
-            bs_error_abort(
-                f"Phi is a ({X}, {Y}) matrix but n has {Xn} elements."
-            )
+            bs_error_abort(f"Phi is a ({X}, {Y}) matrix but n has {Xn} elements.")
         if Ym != Y:
-            bs_error_abort(
-                f"Phi is a ({X}, {Y}) matrix but m has {Ym} elements."
-            )
+            bs_error_abort(f"Phi is a ({X}, {Y}) matrix but m has {Ym} elements.")
 
         if true_alphas is not None:
-            alpha_size = test_vector(true_alphas)
+            alpha_size = check_vector(true_alphas)
             if alpha_size != self.n_alphas:
                 bs_error_abort(
                     f"true_alphas shoud have {self.n_alphas} elements, not {alpha_size}"
                 )
 
         self.Phi = Phi
         self.n = n
@@ -178,15 +175,15 @@
         print_stars(repr_str)
 
     def ipfp_nested_logit_solver(
         self, tol: float = 1e-9, verbose: bool = False, maxiter: int = 1000
     ) -> tuple[Matching, np.ndarray, np.ndarray]:
         """Solves for equilibrium in a two-level nested logit market
         given systematic surplus and margins and nests parameters;
-        does not compute the gradient of the matching patterns
+        does not compute_ the gradient of the matching patterns
 
         Args:
             tol: tolerance on change in solution
             verbose: if `True`, prints information
             maxiter: maximum number of iterations
 
         Returns:
@@ -236,17 +233,15 @@
         for i_nest_x, nest_x in enumerate(nests_over_X):
             muny[i_nest_x, :] = np.sum(muxy[nest_x, :], 0)
 
         err_diff = bigc
         tol_diff = tol * bigc
         tol_newton = tol
         max_newton = 2000
-        MIN_REST = (
-            1e-4 * bigc
-        )  # used to bound mus below in the Newton iterations
+        MIN_REST = 1e-4 * bigc  # used to bound mus below in the Newton iterations
 
         niter = 0
         while (err_diff > tol_diff) and (niter < maxiter):  # IPFP main loop
             # Newton iterates for men
             err_newton = bigc
             i_newton = 0
             while err_newton > tol_newton:
@@ -266,17 +261,15 @@
                             mu_n = muny_x[nest_y]
                             mu0_n = mu0y[nest_y]
                             evec_n = ephi_x[nest_y]
                             rho_n = rhos[i_nest_y]
                             sum_rd = rho_n + delta_x
                             mun_term = nppow(mu_n, (delta_x - 1.0) / sum_rd)
                             mu0_term = nppow(mu0_n, 1.0 / sum_rd)
-                            gbar[x, i_nest_y] = np.sum(
-                                mun_term * mu0_term * evec_n
-                            )
+                            gbar[x, i_nest_y] = np.sum(mun_term * mu0_term * evec_n)
                             gbar_pow[x, i_nest_y] = nppow(
                                 gbar[x, i_nest_y], sum_rd / (delta_x + 1.0)
                             )
                             biga[x] += gbar_pow[x, i_nest_y]
 
                 # now we take one Newton step for all types of men
                 delta_vals1 = 1.0 + delta_vals
@@ -321,17 +314,15 @@
                             mu_n = muxn_y[nest_x]
                             mu0_n = mux0[nest_x]
                             evec_n = ephi_y[nest_x]
                             delta_n = deltas[i_nest_x]
                             sum_rd = rho_y + delta_n
                             mun_term = nppow(mu_n, (rho_n - 1.0) / sum_rd)
                             mu0_term = nppow(mu0_n, 1.0 / sum_rd)
-                            gbar[y, i_nest_x] = np.sum(
-                                mun_term * mu0_term * evec_n
-                            )
+                            gbar[y, i_nest_x] = np.sum(mun_term * mu0_term * evec_n)
                             gbar_pow[y, i_nest_x] = nppow(
                                 gbar[y, i_nest_x], sum_rd / (1.0 + rho_y)
                             )
                             biga[y] += gbar_pow[y, i_nest_x]
 
                 # now we take one Newton step for all types of women
                 rho_vals1 = 1.0 + rho_vals
@@ -375,54 +366,52 @@
                     muny_xy = muny_x[y]
                     mu_term = (
                         mux0_x
                         * mu0y_y
                         * (muxn_xy ** (rho_y - 1.0))
                         * (muny_xy ** (delta_x - 1.0))
                     )
-                    muxy[x, y] = ephi_x[y] * (
-                        mu_term ** (1.0 / (delta_x + rho_y))
-                    )
+                    muxy[x, y] = ephi_x[y] * (mu_term ** (1.0 / (delta_x + rho_y)))
 
-            n_sim, m_sim = _compute_margins(muxy, mux0, mu0y)
+            n_sim, m_sim = compute_margins(muxy, mux0, mu0y)
             marg_err_x, marg_err_y = n_sim - n, m_sim - m
 
             if verbose:
                 print(
                     f"Margin error on men is {marg_err_x} "
                     f" after {niter} IPFP iterations"
                 )
                 print(
                     f"Margin error on women is {marg_err_y} "
                     f" after {niter} IPFP iterations"
                 )
             err_diff = npmaxabs(marg_err_x) + npmaxabs(marg_err_y)
             niter += 1
 
-        n_sim, m_sim = _compute_margins(muxy, mux0, mu0y)
+        n_sim, m_sim = compute_margins(muxy, mux0, mu0y)
         marg_err_x = n_sim - n
         marg_err_y = m_sim - m
 
         if verbose:
             print(
-                f"Margin error on men is {npmaxabs(marg_err_x)} after {niter} IPFP iterations"
+                f"Margin error on men is {npmaxabs(marg_err_x)} after {niter} IPFP"
+                " iterations"
             )
             print(
-                f"Margin error on women is {npmaxabs(marg_err_y)} after {niter} IPFP iterations"
+                f"Margin error on women is {npmaxabs(marg_err_y)} after {niter} IPFP"
+                " iterations"
             )
 
         return Matching(muxy, n, m), marg_err_x, marg_err_y
 
     def ipfp_solve(self) -> Matching:
         if self.true_alphas is None:
             bs_error_abort(
                 "true_alphas must be specified to solve the nested logit by IPFP."
             )
         self.mus, err_x, err_y = self.ipfp_nested_logit_solver(verbose=False)
         return self.mus
 
-    def simulate(
-        self, n_households: int, seed: Optional[int] = None
-    ) -> Matching:
+    def simulate(self, n_households: int, seed: int | None = None) -> Matching:
         self.mus = self.ipfp_solve()
         mus_sim = _simulate_sample_from_mus(self.mus, n_households, seed)
         return mus_sim
```

### Comparing `cupid_matching-1.0.8/cupid_matching/nested_logit.py` & `cupid_matching-1.1.0/cupid_matching/nested_logit.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,22 @@
 and the other with types 2 and 4.
 On each side, the nests are the same for each type, with the same parameters.
 """
 from math import log
 from typing import Any, cast
 
 import numpy as np
+from bs_python_utils.bsnputils import ThreeArrays, TwoArrays
 
 from cupid_matching.entropy import EntropyFunctions, EntropyHessiansParam
-from cupid_matching.matching_utils import Matching, _change_indices
-from cupid_matching.utils import NestsList, ThreeArrays, TwoArrays
+from cupid_matching.matching_utils import Matching
+from cupid_matching.utils import NestsList, _change_indices
 
 
-def e0_nested_logit(
-    muhat: Matching, additional_parameters: list[Any]
-) -> np.ndarray:
+def e0_nested_logit(muhat: Matching, additional_parameters: list[Any]) -> np.ndarray:
     """Returns the values of the parameter-independent part $e_0$
     for the nested logit.
 
     Args:
         muhat: a Matching
         additional_parameters: a list with the nest structure
 
@@ -139,17 +138,15 @@
 
 e0_derivative_nested_logit = (
     e0_derivative_mu_nested_logit,
     e0_derivative_r_nested_logit,
 )
 
 
-def e_nested_logit(
-    muhat: Matching, additional_parameters: list[Any]
-) -> np.ndarray:
+def e_nested_logit(muhat: Matching, additional_parameters: list[Any]) -> np.ndarray:
     """Returns the values of the parameter-dependent part  $e$
     for the nested logit.
 
     Args:
         muhat: a Matching
         additional_parameters: a list with the nest structure
 
@@ -276,28 +273,25 @@
 
     nest_description = "      each x has the same nests over 0, 1, ..., Y:\n"
     for n in nests_for_each_x:
         nest_description += f"      {n}\n"
     nest_description += "      each y has the same nests over 0, 1, ..., X:\n"
     for n in nests_for_each_y:
         nest_description += f"      {n}\n"
-    nest_description += (
-        "       the parameters rho and delta do not depend on the type."
-    )
+    nest_description += "       the parameters rho and delta do not depend on the type."
 
     entropy_nested_logit = EntropyFunctions(
         e0_fun=e0_nested_logit,
         parameter_dependent=True,
         e_fun=e_nested_logit,
         additional_parameters=nests_params,
         hessian="provided",
         e0_derivative=cast(EntropyHessiansParam, e0_derivative_nested_logit),
         e_derivative=cast(EntropyHessiansParam, e_derivative_nested_logit),
-        description="Two-layer nested logit with analytic Hessian\n"
-        + nest_description,
+        description="Two-layer nested logit with analytic Hessian\n" + nest_description,
     )
 
     entropy_nested_logit_numeric = EntropyFunctions(
         e0_fun=e0_nested_logit,
         parameter_dependent=True,
         additional_parameters=nests_params,
         e_fun=e_nested_logit,
```

### Comparing `cupid_matching-1.0.8/cupid_matching/poisson_glm.py` & `cupid_matching-1.1.0/cupid_matching/poisson_glm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Estimates the semilinear Choo and Siow homoskedastic (2006) model
 using Poisson GLM.
 """
 
 from math import sqrt
-from typing import Optional
 
 import numpy as np
 import scipy.linalg as spla
 import scipy.sparse as spr
 from sklearn import linear_model
 
-from cupid_matching.matching_utils import Matching, _make_XY_K_mat, _variance_muhat
+from cupid_matching.matching_utils import Matching, variance_muhat
 from cupid_matching.poisson_glm_utils import PoissonGLMResults, _prepare_data
+from cupid_matching.utils import _make_XY_K_mat
 
 
 def choo_siow_poisson_glm(
     muhat: Matching,
     phi_bases: np.ndarray,
-    tol: Optional[float] = 1e-12,
-    max_iter: Optional[int] = 10000,
-    verbose: Optional[int] = 1,
+    tol: float | None = 1e-12,
+    max_iter: int | None = 10000,
+    verbose: int | None = 1,
 ) -> PoissonGLMResults:
     """Estimates the semilinear Choo and Siow homoskedastic (2006) model
         using Poisson GLM.
 
     Args:
         muhat: the observed Matching
         phi_bases: an (X, Y, K) array of bases
@@ -83,17 +83,15 @@
     # the vector of weights for the Poisson regression
     w = np.concatenate((2 * np.ones(XY), np.ones(X + Y)))
     # reshape the bases
     phi_mat = _make_XY_K_mat(phi_bases)
 
     if try_sparse:
         w_mat = spr.csr_matrix(
-            np.concatenate(
-                (2 * np.ones((XY, n_cols)), np.ones((X + Y, n_cols)))
-            )
+            np.concatenate((2 * np.ones((XY, n_cols)), np.ones((X + Y, n_cols))))
         )
 
         # construct the Z matrix
         ones_X = spr.csr_matrix(np.ones((X, 1)))
         ones_Y = spr.csr_matrix(np.ones((Y, 1)))
         zeros_XK = spr.csr_matrix(np.zeros((X, K)))
         zeros_YK = spr.csr_matrix(np.zeros((Y, K)))
@@ -122,55 +120,53 @@
         zeros_YK = np.zeros((Y, K))
         zeros_XY = np.zeros((X, Y))
         zeros_YX = np.zeros((Y, X))
         id_X = np.eye(X)
         id_Y = np.eye(Y)
         Z_unweighted = np.vstack(
             [
-                np.hstack(
-                    [-np.kron(id_X, ones_Y), -np.kron(ones_X, id_Y), phi_mat]
-                ),
+                np.hstack([-np.kron(id_X, ones_Y), -np.kron(ones_X, id_Y), phi_mat]),
                 np.hstack([-id_X, zeros_XY, zeros_XK]),
                 np.hstack([zeros_YX, -id_Y, zeros_YK]),
             ]
         )
         Z = Z_unweighted / w.reshape((-1, 1))
 
     _, _, _, n, m = muhat.unpack()
-    var_muhat, var_munm = _variance_muhat(muhat)
+    var_muhat = variance_muhat(muhat)
     (
         muxyhat_norm,
         var_muhat_norm,
-        var_munm_norm,
         n_households,
         n_individuals,
-    ) = _prepare_data(muhat, var_muhat, var_munm)
+    ) = _prepare_data(muhat, var_muhat)
 
     clf = linear_model.PoissonRegressor(
         fit_intercept=False,
         tol=tol,
         verbose=verbose,
         alpha=0,
         max_iter=max_iter,
     )
     clf.fit(Z, muxyhat_norm, sample_weight=w)
     gamma_est = clf.coef_
 
-    # we compute the variance-covariance of the estimator
+    # we compute_ the variance-covariance of the estimator
+    var_allmus_norm = var_muhat_norm.var_allmus
     nr, nc = Z.shape
     exp_Zg = np.exp(Z @ gamma_est).reshape(n_rows)
     A_hat = np.zeros((nc, nc))
     B_hat = np.zeros((nc, nc))
     for i in range(nr):
         Zi = Z[i, :]
         wi = w[i]
         A_hat += wi * exp_Zg[i] * np.outer(Zi, Zi)
         for j in range(nr):
             Zj = Z[j, :]
-            B_hat += wi * w[j] * var_muhat_norm[i, j] * np.outer(Zi, Zj)
+            B_hat += wi * w[j] * var_allmus_norm[i, j] * np.outer(Zi, Zj)
 
     A_inv = spla.inv(A_hat)
     varcov_gamma = A_inv @ B_hat @ A_inv
     stderrs_gamma = np.sqrt(np.diag(varcov_gamma))
 
     beta_est = gamma_est[-K:]
     varcov_beta = varcov_gamma[-K:, -K:]
@@ -180,41 +176,40 @@
     # we correct for the effect of the normalization
     n_norm = n / n_individuals
     m_norm = m / n_individuals
     u_est = gamma_est[:X] + np.log(n_norm)
     v_est = gamma_est[X:-K] + np.log(m_norm)
 
     # since u = a + log(n_norm) we also need to adjust the estimated variance
-    z_unweighted_T = Z_unweighted.T
+    var_munm_norm = var_muhat_norm.var_munm
+    var_n_norm = var_munm_norm[XY : (XY + X), XY : (XY + X)]
+    var_m_norm = var_munm_norm[(XY + X) :, (XY + X) :]
+    Z_unweighted_T = Z_unweighted.T
     u_std = np.zeros(X)
     ix = XY
     for x in range(X):
         n_norm_x = n_norm[x]
         A_inv_x = A_inv[x, :]
-        var_log_nx = var_munm_norm[ix, ix] / n_norm_x / n_norm_x
+        var_log_nx = var_n_norm[x, x] / n_norm_x / n_norm_x
         slice_x = slice(x * Y, (x + 1) * Y)
-        covar_term = var_muhat_norm[:, ix] + np.sum(
-            var_muhat_norm[:, slice_x], 1
-        )
-        cov_a_lognx = (A_inv_x @ z_unweighted_T @ covar_term) / n_norm_x
+        covar_term = var_allmus_norm[:, ix] + np.sum(var_allmus_norm[:, slice_x], 1)
+        cov_a_lognx = (A_inv_x @ Z_unweighted_T @ covar_term) / n_norm_x
         ux_var = varcov_gamma[x, x] + var_log_nx + 2.0 * cov_a_lognx
         u_std[x] = sqrt(ux_var)
         ix += 1
 
     v_std = stderrs_gamma[X:-K]
     iy, jy = X, XY + X
     for y in range(Y):
         m_norm_y = m_norm[y]
         A_inv_y = A_inv[iy, :]
-        var_log_my = var_munm_norm[jy, jy] / m_norm_y / m_norm_y
+        var_log_my = var_m_norm[y, y] / m_norm_y / m_norm_y
         slice_y = slice(y, XY, Y)
-        covar_term = var_muhat_norm[:, jy] + np.sum(
-            var_muhat_norm[:, slice_y], 1
-        )
-        cov_b_logmy = (A_inv_y @ z_unweighted_T @ covar_term) / m_norm_y
+        covar_term = var_allmus_norm[:, jy] + np.sum(var_allmus_norm[:, slice_y], 1)
+        cov_b_logmy = (A_inv_y @ Z_unweighted_T @ covar_term) / m_norm_y
         vy_var = varcov_gamma[iy, iy] + var_log_my + 2.0 * cov_b_logmy
         v_std[y] = sqrt(vy_var)
         iy += 1
         jy += 1
 
     results = PoissonGLMResults(
         X=X,
```

### Comparing `cupid_matching-1.0.8/cupid_matching/poisson_glm_utils.py` & `cupid_matching-1.1.0/cupid_matching/poisson_glm_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Utilities for Poisson GLM.
 """
 
 from dataclasses import dataclass
-from typing import Optional, Tuple
+from typing import cast
 
 import numpy as np
+from bs_python_utils.bsnputils import npmaxabs
+from bs_python_utils.bsutils import bs_error_abort, print_stars
 
-from cupid_matching.matching_utils import Matching
-from cupid_matching.utils import npmaxabs, print_stars
+from cupid_matching.matching_utils import Matching, VarianceMatching, var_divide
 
 
 @dataclass
 class PoissonGLMResults:
     """Stores and formats the estimation results.
 
     Args:
@@ -52,41 +53,43 @@
 
     def __str__(self):
         line_stars = "*" * 80 + "\n"
         print_stars("Estimating a Choo and Siow model by Poisson GLM.")
         model_str = f"The data has {self.number_households} households\n\n"
         model_str += f"We use {self.K} basis functions.\n\n"
         repr_str = line_stars + model_str
-        repr_str += "The estimated basis coefficients (and their standard errors) are\n\n"
+        repr_str += (
+            "The estimated basis coefficients (and their standard errors) are\n\n"
+        )
         for i in range(self.K):
             repr_str += (
                 f"   base_{i + 1}: {self.estimated_beta[i]: > 10.3f}  "
                 + f"({self.stderrs_beta[i]: .3f})\n"
             )
-        repr_str += (
-            "The estimated utilities of men (and their standard errors) are\n\n"
-        )
+        repr_str += "The estimated utilities of men (and their standard errors) are\n\n"
         for i in range(self.X):
             repr_str += (
                 f"   u_{i + 1}: {self.estimated_u[i]: > 10.3f}  "
                 + f"({self.stderrs_u[i]: .3f})\n"
             )
-        repr_str += "The estimated utilities of women (and their standard errors) are\n\n"
+        repr_str += (
+            "The estimated utilities of women (and their standard errors) are\n\n"
+        )
         for i in range(self.Y):
             repr_str += (
                 f"   v {i + 1}: {self.estimated_v[i]: > 10.3f}  "
                 + f"({self.stderrs_v[i]: .3f})\n"
             )
         return repr_str + line_stars
 
     def print_results(
         self,
-        lambda_true: Optional[np.ndarray] = None,
-        u_true: Optional[np.ndarray] = None,
-        v_true: Optional[np.ndarray] = None,
+        lambda_true: np.ndarray | None = None,
+        u_true: np.ndarray | None = None,
+        v_true: np.ndarray | None = None,
     ) -> float | None:
         estimates_beta = self.estimated_beta
         stderrs_beta = self.stderrs_beta
 
         if lambda_true is None:
             repr_str = "The  estimated coefficients "
             repr_str += "(and their standard errors) are\n\n"
@@ -97,85 +100,74 @@
             repr_str = "The  true and estimated coefficients "
             repr_str += "(and their standard errors) are\n\n"
             for i, coeff in enumerate(estimates_beta):
                 repr_str += f"   base {i + 1}: {lambda_true[i]: > 10.3f} "
                 repr_str += f" {coeff: > 10.3f}  ({stderrs_beta[i]: > 10.3f})\n"
             print_stars(repr_str)
 
-        estimates_u = self.estimated_u
-        stderrs_u = self.stderrs_u
+        self.report_utilities("men", u_true)
+        self.report_utilities("women", v_true)
 
-        if u_true is None:
-            repr_str = "The estimated utilities for men  "
-            repr_str += "(and their standard errors) are:\n\n"
-            for i, coeff in enumerate(estimates_u):
-                repr_str += f" {coeff: > 10.3f}  ({stderrs_u[i]: > 10.3f})\n"
-            print_stars(repr_str)
+        if lambda_true is None:
+            return None
         else:
-            repr_str = "The true and estimated utilities for men "
-            repr_str += "(and their standard errors) are:\n\n"
-            for i, coeff in enumerate(estimates_u):
-                repr_str += f"   u_{i + 1}: {u_true[i]: > 10.3f} "
-                repr_str += f" {coeff: > 10.3f}  ({stderrs_u[i]: > 10.3f})\n"
-            print_stars(repr_str)
+            discrepancy = npmaxabs(lambda_true - estimates_beta)
+            print_stars(
+                "The largest difference between true and estimated coefficients is"
+                f" {discrepancy: .2e}"
+            )
+            return cast(float, discrepancy)
 
-        estimates_v = self.estimated_v
-        stderrs_v = self.stderrs_v
-        if v_true is None:
-            repr_str = "The estimated utilities for women "
+    def report_utilities(self, gender: str, utils_true: np.ndarray | None) -> None:
+        if gender not in ["men", "women"]:
+            bs_error_abort(f"gender can only be 'men' or 'women', not {gender}")
+        utils_estimates = self.estimated_u if gender == "men" else self.estimated_v
+        utils_stderrs = self.stderrs_u if gender == "men" else self.stderrs_v
+        util_prefix = "u" if gender == "men" else "v"
+        if utils_true is None:
+            repr_str = f"The estimated utilities for {gender} "
             repr_str += "(and their standard errors) are:\n\n"
-            for i, coeff in enumerate(estimates_v):
-                repr_str += f" {coeff: > 10.3f}  ({stderrs_v[i]: > 10.3f})\n"
+            for i, coeff in enumerate(utils_estimates):
+                repr_str += f"   {util_prefix}_{i + 1}: "
+                repr_str += f" {coeff: > 10.3f}  ({utils_stderrs[i]: > 10.3f})\n"
             print_stars(repr_str)
         else:
-            repr_str = "The true and estimated utilities for women "
+            repr_str = f"The true and estimated utilities for {gender} "
             repr_str += "(and their standard errors) are:\n\n"
-            for i, coeff in enumerate(estimates_v):
-                repr_str += f"   v_{i + 1}: {v_true[i]: > 10.3f} "
-                repr_str += f" {coeff: > 10.3f}  ({stderrs_v[i]: > 10.3f})\n"
+            for i, coeff in enumerate(utils_estimates):
+                repr_str += f"   {util_prefix}_{i + 1}: {utils_true[i]: > 10.3f} "
+                repr_str += f" {coeff: > 10.3f}  ({utils_stderrs[i]: > 10.3f})\n"
             print_stars(repr_str)
 
-        if lambda_true is None:
-            return None
-        else:
-            discrepancy = npmaxabs(lambda_true - estimates_beta)
-            print_stars(
-                f"The largest difference between true and estimated coefficients is {discrepancy: .2e}"
-            )
-            return discrepancy
-
 
 def _prepare_data(
     muhat: Matching,
-    var_muhat: np.ndarray,
-    var_munm: np.ndarray,
-) -> Tuple[np.ndarray, np.ndarray, np.ndarray, int, int]:
+    var_muhat: VarianceMatching,
+) -> tuple[np.ndarray, VarianceMatching, int, int]:
     """Normalizes the matching patterns and stacks them.
     We rescale the data so that the total number of individuals is one.
 
     Args:
         muhat: the observed Matching
-        var_muhat: the variance-covariance of $(\\mu_{xy}, \\mu_{x0},\\mu_{0y})$
-        var_munm: the variance-covariance of $(\\mu_{xy},n_x,m_y)$
+        var_muhat: the variance-covariance object for teh observed matching
         phi_bases: an (X, Y, K) array of bases
 
     Returns:
         the stacked muxy, mux0, mu0y
         the corresponding variance-covariance matrix
         the number of households
         the number of individuals
     """
     muxy, mux0, mu0y, _, _ = muhat.unpack()
     n_couples = np.sum(muxy)
     n_households = n_couples + np.sum(mux0) + np.sum(mu0y)
     n_individuals = n_households + n_couples
     # rescale the data so that the total number of individuals is one
     muhat_norm = np.concatenate([muxy.flatten(), mux0, mu0y]) / n_individuals
-    var_muhat_norm = var_muhat / n_individuals / n_individuals
-    var_munm_norm = var_munm / n_individuals / n_individuals
+    n_indivs2 = n_individuals * n_individuals
+    var_muhat_norm = var_divide(var_muhat, n_indivs2)
     return (
         muhat_norm,
         var_muhat_norm,
-        var_munm_norm,
         n_households,
         n_individuals,
     )
```

