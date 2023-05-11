# Comparing `tmp/upstash_py-0.1.0.tar.gz` & `tmp/upstash_py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_py-0.1.0.tar", max compression
+gzip compressed data, was "upstash_py-0.2.0.tar", max compression
```

## Comparing `upstash_py-0.1.0.tar` & `upstash_py-0.2.0.tar`

### file list

```diff
@@ -1,274 +1,18 @@
--rw-r--r--   0        0        0       37 2023-03-04 10:43:41.243570 upstash_py-0.1.0/README.md
--rw-r--r--   0        0        0      379 2023-04-12 16:47:29.139107 upstash_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       34 2023-04-14 15:22:48.038542 upstash_py-0.1.0/upstash_py/.mypy_cache/.gitignore
--rw-r--r--   0        0        0        2 2023-04-14 15:22:48.037927 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   196618 2023-04-14 15:22:47.784324 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1781 2023-04-14 15:22:47.784491 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    57299 2023-04-14 15:22:47.782063 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1827 2023-04-14 15:22:47.782208 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    19772 2023-04-14 15:22:47.781164 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1735 2023-04-14 15:22:47.781316 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     3403 2023-04-14 15:22:47.780667 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1737 2023-04-14 15:22:47.780825 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0    99739 2023-04-14 15:22:47.833324 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/_socket.data.json
--rw-r--r--   0        0        0     1811 2023-04-14 15:22:47.833492 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/_socket.meta.json
--rw-r--r--   0        0        0    25969 2023-04-14 15:22:47.825168 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/_thread.data.json
--rw-r--r--   0        0        0     1779 2023-04-14 15:22:47.825342 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/_thread.meta.json
--rw-r--r--   0        0        0    96971 2023-04-14 15:22:47.780365 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1859 2023-04-14 15:22:47.780508 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    29970 2023-04-14 15:22:47.806928 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/_weakref.data.json
--rw-r--r--   0        0        0     1763 2023-04-14 15:22:47.807088 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/_weakref.meta.json
--rw-r--r--   0        0        0    55210 2023-04-14 15:22:47.805405 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/_weakrefset.data.json
--rw-r--r--   0        0        0     1769 2023-04-14 15:22:47.805567 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/_weakrefset.meta.json
--rw-r--r--   0        0        0    22341 2023-04-14 15:22:47.779110 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1723 2023-04-14 15:22:47.779247 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    66373 2023-04-14 15:22:47.778583 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1790 2023-04-14 15:22:47.778725 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0    12196 2023-04-14 15:22:47.991637 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/__init__.data.json
--rw-r--r--   0        0        0     2159 2023-04-14 15:22:47.991833 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/__init__.meta.json
--rw-r--r--   0        0        0   113323 2023-04-14 15:22:47.987312 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/base_events.data.json
--rw-r--r--   0        0        0     2050 2023-04-14 15:22:47.987495 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/base_events.meta.json
--rw-r--r--   0        0        0    24748 2023-04-14 15:22:47.843432 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/coroutines.data.json
--rw-r--r--   0        0        0     1768 2023-04-14 15:22:47.843615 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/coroutines.meta.json
--rw-r--r--   0        0        0   218498 2023-04-14 15:22:47.985726 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/events.data.json
--rw-r--r--   0        0        0     2075 2023-04-14 15:22:47.985945 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/events.meta.json
--rw-r--r--   0        0        0    10657 2023-04-14 15:22:47.842377 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/exceptions.data.json
--rw-r--r--   0        0        0     1717 2023-04-14 15:22:47.842560 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/exceptions.meta.json
--rw-r--r--   0        0        0    40110 2023-04-14 15:22:47.983088 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/futures.data.json
--rw-r--r--   0        0        0     1908 2023-04-14 15:22:47.983267 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/futures.meta.json
--rw-r--r--   0        0        0    41814 2023-04-14 15:22:47.990472 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/locks.data.json
--rw-r--r--   0        0        0     1884 2023-04-14 15:22:47.990674 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/locks.meta.json
--rw-r--r--   0        0        0     2789 2023-04-14 15:22:47.881046 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/mixins.data.json
--rw-r--r--   0        0        0     1755 2023-04-14 15:22:47.881202 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/mixins.meta.json
--rw-r--r--   0        0        0    18708 2023-04-14 15:22:47.979191 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/protocols.data.json
--rw-r--r--   0        0        0     1811 2023-04-14 15:22:47.979343 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/protocols.meta.json
--rw-r--r--   0        0        0    25195 2023-04-14 15:22:47.989607 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/queues.data.json
--rw-r--r--   0        0        0     1747 2023-04-14 15:22:47.989838 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/queues.meta.json
--rw-r--r--   0        0        0    11832 2023-04-14 15:22:47.988985 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/runners.data.json
--rw-r--r--   0        0        0     1806 2023-04-14 15:22:47.989175 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/runners.meta.json
--rw-r--r--   0        0        0     4141 2023-04-14 15:22:47.978615 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/selector_events.data.json
--rw-r--r--   0        0        0     1785 2023-04-14 15:22:47.978837 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/selector_events.meta.json
--rw-r--r--   0        0        0    39191 2023-04-14 15:22:47.988509 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/streams.data.json
--rw-r--r--   0        0        0     1904 2023-04-14 15:22:47.988692 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/streams.meta.json
--rw-r--r--   0        0        0    26311 2023-04-14 15:22:47.991144 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/subprocess.data.json
--rw-r--r--   0        0        0     1927 2023-04-14 15:22:47.991332 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/subprocess.meta.json
--rw-r--r--   0        0        0     9031 2023-04-14 15:22:47.987753 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/taskgroups.data.json
--rw-r--r--   0        0        0     1818 2023-04-14 15:22:47.987924 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/taskgroups.meta.json
--rw-r--r--   0        0        0   111224 2023-04-14 15:22:47.982354 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/tasks.data.json
--rw-r--r--   0        0        0     1930 2023-04-14 15:22:47.982511 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/tasks.meta.json
--rw-r--r--   0        0        0     6093 2023-04-14 15:22:47.841376 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/threads.data.json
--rw-r--r--   0        0        0     1727 2023-04-14 15:22:47.841541 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/threads.meta.json
--rw-r--r--   0        0        0    10390 2023-04-14 15:22:47.840810 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/timeouts.data.json
--rw-r--r--   0        0        0     1720 2023-04-14 15:22:47.840984 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/timeouts.meta.json
--rw-r--r--   0        0        0    29769 2023-04-14 15:22:47.980776 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/transports.data.json
--rw-r--r--   0        0        0     1774 2023-04-14 15:22:47.980934 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/transports.meta.json
--rw-r--r--   0        0        0    63934 2023-04-14 15:22:47.980164 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/unix_events.data.json
--rw-r--r--   0        0        0     1892 2023-04-14 15:22:47.980324 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/asyncio/unix_events.meta.json
--rw-r--r--   0        0        0    17875 2023-04-14 15:22:47.837703 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/base64.data.json
--rw-r--r--   0        0        0     1756 2023-04-14 15:22:47.837897 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/base64.meta.json
--rw-r--r--   0        0        0  1223266 2023-04-14 15:22:47.797669 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1900 2023-04-14 15:22:47.797893 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   134209 2023-04-14 15:22:47.777603 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1841 2023-04-14 15:22:47.777763 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   446262 2023-04-14 15:22:47.775858 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1870 2023-04-14 15:22:47.776017 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     4047 2023-04-14 15:22:47.771157 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1701 2023-04-14 15:22:47.771292 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0     1670 2023-04-14 15:22:47.833736 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/concurrent/__init__.data.json
--rw-r--r--   0        0        0     1673 2023-04-14 15:22:47.833900 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/concurrent/__init__.meta.json
--rw-r--r--   0        0        0     4911 2023-04-14 15:22:47.947438 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/concurrent/futures/__init__.data.json
--rw-r--r--   0        0        0     1832 2023-04-14 15:22:47.947591 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/concurrent/futures/__init__.meta.json
--rw-r--r--   0        0        0    65898 2023-04-14 15:22:47.903569 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/concurrent/futures/_base.data.json
--rw-r--r--   0        0        0     1831 2023-04-14 15:22:47.903729 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/concurrent/futures/_base.meta.json
--rw-r--r--   0        0        0    65956 2023-04-14 15:22:47.946858 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/concurrent/futures/process.data.json
--rw-r--r--   0        0        0     2075 2023-04-14 15:22:47.947021 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/concurrent/futures/process.meta.json
--rw-r--r--   0        0        0    23814 2023-04-14 15:22:47.921308 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/concurrent/futures/thread.data.json
--rw-r--r--   0        0        0     1876 2023-04-14 15:22:47.921478 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/concurrent/futures/thread.meta.json
--rw-r--r--   0        0        0   119168 2023-04-14 15:22:47.770822 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1778 2023-04-14 15:22:47.770972 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    41327 2023-04-14 15:22:47.835959 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/contextvars.data.json
--rw-r--r--   0        0        0     1769 2023-04-14 15:22:47.836171 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/contextvars.meta.json
--rw-r--r--   0        0        0    12987 2023-04-14 15:22:47.799025 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/copyreg.data.json
--rw-r--r--   0        0        0     1731 2023-04-14 15:22:47.799174 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/copyreg.meta.json
--rw-r--r--   0        0        0   140935 2023-04-14 15:22:47.769091 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1833 2023-04-14 15:22:47.769439 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0    63404 2023-04-14 15:22:47.767307 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1783 2023-04-14 15:22:47.767450 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0     8133 2023-04-14 15:22:47.766361 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1762 2023-04-14 15:22:47.766499 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    13285 2023-04-14 15:22:47.766015 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1698 2023-04-14 15:22:47.766150 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7907 2023-04-14 15:22:47.765614 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1733 2023-04-14 15:22:47.765752 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    26998 2023-04-14 15:22:47.765277 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1705 2023-04-14 15:22:47.765410 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9999 2023-04-14 15:22:47.764783 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1718 2023-04-14 15:22:47.764922 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    86490 2023-04-14 15:22:47.764398 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1836 2023-04-14 15:22:47.764541 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    33584 2023-04-14 15:22:47.763227 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1791 2023-04-14 15:22:47.763359 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0    98681 2023-04-14 15:22:47.762576 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1755 2023-04-14 15:22:47.762716 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    24396 2023-04-14 15:22:47.761248 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1752 2023-04-14 15:22:47.761381 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     6693 2023-04-14 15:22:47.760730 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1736 2023-04-14 15:22:47.760866 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    75976 2023-04-14 15:22:47.760379 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1884 2023-04-14 15:22:47.760530 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    69939 2023-04-14 15:22:47.759328 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1895 2023-04-14 15:22:47.759474 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    98826 2023-04-14 15:22:47.758351 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1901 2023-04-14 15:22:47.758489 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12943 2023-04-14 15:22:47.757071 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1718 2023-04-14 15:22:47.757215 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    93255 2023-04-14 15:22:47.756596 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1846 2023-04-14 15:22:47.756746 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    16868 2023-04-14 15:22:47.888927 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1751 2023-04-14 15:22:47.889076 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    15835 2023-04-14 15:22:47.839851 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1695 2023-04-14 15:22:47.840033 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    11857 2023-04-14 15:22:47.838745 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1707 2023-04-14 15:22:47.838940 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   157586 2023-04-14 15:22:47.880437 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/logging/__init__.data.json
--rw-r--r--   0        0        0     1859 2023-04-14 15:22:47.880659 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/logging/__init__.meta.json
--rw-r--r--   0        0        0    29356 2023-04-14 15:22:47.755285 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1789 2023-04-14 15:22:47.755430 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    34052 2023-04-14 15:22:47.943121 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/__init__.data.json
--rw-r--r--   0        0        0     2144 2023-04-14 15:22:47.943264 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/__init__.meta.json
--rw-r--r--   0        0        0    33231 2023-04-14 15:22:47.900246 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/connection.data.json
--rw-r--r--   0        0        0     1899 2023-04-14 15:22:47.900409 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/connection.meta.json
--rw-r--r--   0        0        0   103601 2023-04-14 15:22:47.942467 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/context.data.json
--rw-r--r--   0        0        0     2308 2023-04-14 15:22:47.942619 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/context.meta.json
--rw-r--r--   0        0        0   160947 2023-04-14 15:22:47.940575 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/managers.data.json
--rw-r--r--   0        0        0     1941 2023-04-14 15:22:47.940754 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/managers.meta.json
--rw-r--r--   0        0        0    56132 2023-04-14 15:22:47.811211 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/pool.data.json
--rw-r--r--   0        0        0     1787 2023-04-14 15:22:47.811382 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/pool.meta.json
--rw-r--r--   0        0        0     9790 2023-04-14 15:22:47.919868 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/popen_fork.data.json
--rw-r--r--   0        0        0     1774 2023-04-14 15:22:47.920025 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json
--rw-r--r--   0        0        0     6214 2023-04-14 15:22:47.937621 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json
--rw-r--r--   0        0        0     1816 2023-04-14 15:22:47.937764 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json
--rw-r--r--   0        0        0     6935 2023-04-14 15:22:47.937290 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json
--rw-r--r--   0        0        0     1818 2023-04-14 15:22:47.937432 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json
--rw-r--r--   0        0        0     2143 2023-04-14 15:22:47.918910 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json
--rw-r--r--   0        0        0     1788 2023-04-14 15:22:47.919101 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json
--rw-r--r--   0        0        0    19213 2023-04-14 15:22:47.808256 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/process.data.json
--rw-r--r--   0        0        0     1751 2023-04-14 15:22:47.808415 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/process.meta.json
--rw-r--r--   0        0        0    21459 2023-04-14 15:22:47.898229 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/queues.data.json
--rw-r--r--   0        0        0     1755 2023-04-14 15:22:47.898384 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/queues.meta.json
--rw-r--r--   0        0        0    31415 2023-04-14 15:22:47.936870 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/reduction.data.json
--rw-r--r--   0        0        0     1961 2023-04-14 15:22:47.937079 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/reduction.meta.json
--rw-r--r--   0        0        0    31816 2023-04-14 15:22:47.801600 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/shared_memory.data.json
--rw-r--r--   0        0        0     1805 2023-04-14 15:22:47.801757 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json
--rw-r--r--   0        0        0    73276 2023-04-14 15:22:47.938652 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json
--rw-r--r--   0        0        0     1876 2023-04-14 15:22:47.938857 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json
--rw-r--r--   0        0        0    10702 2023-04-14 15:22:47.802489 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/spawn.data.json
--rw-r--r--   0        0        0     1727 2023-04-14 15:22:47.802639 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/spawn.meta.json
--rw-r--r--   0        0        0    27899 2023-04-14 15:22:47.941175 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/synchronize.data.json
--rw-r--r--   0        0        0     1841 2023-04-14 15:22:47.941328 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/synchronize.meta.json
--rw-r--r--   0        0        0    25649 2023-04-14 15:22:47.896692 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/util.data.json
--rw-r--r--   0        0        0     1794 2023-04-14 15:22:47.896861 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/multiprocessing/util.meta.json
--rw-r--r--   0        0        0   352499 2023-04-14 15:22:47.754657 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1904 2023-04-14 15:22:47.754818 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     5326 2023-04-14 15:22:47.750641 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1693 2023-04-14 15:22:47.750781 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0    95722 2023-04-14 15:22:47.750302 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1855 2023-04-14 15:22:47.750442 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    48547 2023-04-14 15:22:47.749034 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1791 2023-04-14 15:22:47.749174 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    82104 2023-04-14 15:22:47.748216 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1785 2023-04-14 15:22:47.748363 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0    33288 2023-04-14 15:22:47.862660 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/queue.data.json
--rw-r--r--   0        0        0     1724 2023-04-14 15:22:47.862832 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/queue.meta.json
--rw-r--r--   0        0        0   183331 2023-04-14 15:22:47.747066 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1877 2023-04-14 15:22:47.747233 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    60510 2023-04-14 15:22:47.819615 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/selectors.data.json
--rw-r--r--   0        0        0     1813 2023-04-14 15:22:47.819784 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/selectors.meta.json
--rw-r--r--   0        0        0    88668 2023-04-14 15:22:47.887279 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/socket.data.json
--rw-r--r--   0        0        0     1864 2023-04-14 15:22:47.887456 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/socket.meta.json
--rw-r--r--   0        0        0    15466 2023-04-14 15:22:47.744883 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1721 2023-04-14 15:22:47.745023 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    30763 2023-04-14 15:22:47.744460 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1733 2023-04-14 15:22:47.744602 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    54036 2023-04-14 15:22:47.743864 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1785 2023-04-14 15:22:47.744008 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   204600 2023-04-14 15:22:47.915799 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/ssl.data.json
--rw-r--r--   0        0        0     1866 2023-04-14 15:22:47.916064 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/ssl.meta.json
--rw-r--r--   0        0        0    30299 2023-04-14 15:22:47.816171 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/string.data.json
--rw-r--r--   0        0        0     1770 2023-04-14 15:22:47.816330 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/string.meta.json
--rw-r--r--   0        0        0   177852 2023-04-14 15:22:47.742966 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1845 2023-04-14 15:22:47.743131 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   154772 2023-04-14 15:22:47.740716 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1824 2023-04-14 15:22:47.740902 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    70535 2023-04-14 15:22:47.826249 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/threading.data.json
--rw-r--r--   0        0        0     1755 2023-04-14 15:22:47.826415 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/threading.meta.json
--rw-r--r--   0        0        0    46601 2023-04-14 15:22:47.814271 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1714 2023-04-14 15:22:47.814442 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0   260903 2023-04-14 15:22:47.738839 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1796 2023-04-14 15:22:47.739020 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   461617 2023-04-14 15:22:47.735777 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1862 2023-04-14 15:22:47.735980 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    56462 2023-04-14 15:22:47.730343 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1786 2023-04-14 15:22:47.730597 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0     1609 2023-04-14 15:22:47.860298 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/__init__.data.json
--rw-r--r--   0        0        0     1612 2023-04-14 15:22:47.860447 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/__init__.meta.json
--rw-r--r--   0        0        0     2826 2023-04-14 15:22:47.846025 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/config.data.json
--rw-r--r--   0        0        0     1619 2023-04-14 15:22:47.846205 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/config.meta.json
--rw-r--r--   0        0        0     2258 2023-04-14 15:22:47.844386 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/exception.data.json
--rw-r--r--   0        0        0     1624 2023-04-14 15:22:47.844565 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/exception.meta.json
--rw-r--r--   0        0        0     1381 2023-04-14 15:22:47.844780 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/http.data.json
--rw-r--r--   0        0        0     1548 2023-04-14 15:22:47.844941 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/http.meta.json
--rw-r--r--   0        0        0     3412 2023-04-14 15:22:47.859900 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/schema/commands/parameters.data.json
--rw-r--r--   0        0        0     1658 2023-04-14 15:22:47.860077 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/schema/commands/parameters.meta.json
--rw-r--r--   0        0        0     3874 2023-04-14 15:22:47.859396 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/schema/commands/returns.data.json
--rw-r--r--   0        0        0     1673 2023-04-14 15:22:47.859564 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/schema/commands/returns.meta.json
--rw-r--r--   0        0        0     1458 2023-04-14 15:22:47.845551 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/schema/commands.data.json
--rw-r--r--   0        0        0     1570 2023-04-14 15:22:47.845712 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/schema/commands.meta.json
--rw-r--r--   0        0        0     5203 2023-04-14 15:22:47.858382 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/schema/http.data.json
--rw-r--r--   0        0        0     1628 2023-04-14 15:22:47.858555 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/schema/http.meta.json
--rw-r--r--   0        0        0     1395 2023-04-14 15:22:47.845155 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/schema.data.json
--rw-r--r--   0        0        0     1552 2023-04-14 15:22:47.845317 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/schema.meta.json
--rw-r--r--   0        0        0     2193 2023-04-14 15:22:47.887787 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/utils/base.data.json
--rw-r--r--   0        0        0     1708 2023-04-14 15:22:47.887940 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/utils/base.meta.json
--rw-r--r--   0        0        0     2370 2023-04-14 15:22:47.857718 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/utils/comparison.data.json
--rw-r--r--   0        0        0     1658 2023-04-14 15:22:47.857896 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/utils/comparison.meta.json
--rw-r--r--   0        0        0     5730 2023-04-14 15:22:47.890457 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/utils/exception.data.json
--rw-r--r--   0        0        0     1814 2023-04-14 15:22:47.890622 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/utils/exception.meta.json
--rw-r--r--   0        0        0    11156 2023-04-14 15:22:47.894952 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/utils/format.data.json
--rw-r--r--   0        0        0     1788 2023-04-14 15:22:47.895120 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/utils/format.meta.json
--rw-r--r--   0        0        0     1388 2023-04-14 15:22:47.843918 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/utils.data.json
--rw-r--r--   0        0        0     1550 2023-04-14 15:22:47.844092 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/upstash_py/utils.meta.json
--rw-r--r--   0        0        0   156310 2023-04-14 15:22:47.868896 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/weakref.data.json
--rw-r--r--   0        0        0     1788 2023-04-14 15:22:47.869177 upstash_py-0.1.0/upstash_py/.mypy_cache/3.11/weakref.meta.json
--rw-r--r--   0        0        0      190 2023-04-14 15:22:48.038609 upstash_py-0.1.0/upstash_py/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       37 2023-05-03 17:42:58.569347 upstash_py-0.1.0/upstash_py/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-05-03 17:42:58.569412 upstash_py-0.1.0/upstash_py/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2023-05-03 17:42:58.569275 upstash_py-0.1.0/upstash_py/.pytest_cache/README.md
--rw-r--r--   0        0        0       37 2023-05-03 17:42:58.569575 upstash_py-0.1.0/upstash_py/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0       31 2023-05-03 17:43:01.529574 upstash_py-0.1.0/upstash_py/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-05-03 17:43:01.529834 upstash_py-0.1.0/upstash_py/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2023-03-04 11:23:56.540070 upstash_py-0.1.0/upstash_py/__init__.py
--rw-r--r--   0        0        0    83890 2023-05-04 15:37:13.577946 upstash_py-0.1.0/upstash_py/client.py
--rw-r--r--   0        0        0      309 2023-04-13 12:10:18.424930 upstash_py-0.1.0/upstash_py/config.py
--rw-r--r--   0        0        0       44 2023-03-08 07:44:02.265644 upstash_py-0.1.0/upstash_py/exception.py
--rw-r--r--   0        0        0     1477 2023-05-04 15:53:50.306646 upstash_py-0.1.0/upstash_py/http/__pycache__/decode.cpython-311.pyc
--rw-r--r--   0        0        0     2767 2023-04-13 15:52:55.300519 upstash_py-0.1.0/upstash_py/http/__pycache__/execute.cpython-311.pyc
--rw-r--r--   0        0        0      755 2023-05-04 15:53:00.952164 upstash_py-0.1.0/upstash_py/http/decode.py
--rw-r--r--   0        0        0     1629 2023-04-13 15:37:48.050511 upstash_py-0.1.0/upstash_py/http/execute.py
--rw-r--r--   0        0        0     1030 2023-05-04 15:39:39.039487 upstash_py-0.1.0/upstash_py/play.py
--rw-r--r--   0        0        0      115 2023-05-03 17:44:20.513271 upstash_py-0.1.0/upstash_py/play2.py
--rw-r--r--   0        0        0      955 2023-04-13 15:52:55.302528 upstash_py-0.1.0/upstash_py/schema/__pycache__/http.cpython-311.pyc
--rw-r--r--   0        0        0      787 2023-04-14 12:24:16.330346 upstash_py-0.1.0/upstash_py/schema/commands/__pycache__/parameters.cpython-311.pyc
--rw-r--r--   0        0        0      829 2023-04-14 15:10:31.988058 upstash_py-0.1.0/upstash_py/schema/commands/__pycache__/returns.cpython-311.pyc
--rw-r--r--   0        0        0      409 2023-04-14 12:17:17.899972 upstash_py-0.1.0/upstash_py/schema/commands/parameters.py
--rw-r--r--   0        0        0      932 2023-04-14 14:37:49.938942 upstash_py-0.1.0/upstash_py/schema/commands/returns.py
--rw-r--r--   0        0        0      761 2023-04-13 15:35:06.241703 upstash_py-0.1.0/upstash_py/schema/http.py
--rw-r--r--   0        0        0      498 2023-04-13 16:21:42.465103 upstash_py-0.1.0/upstash_py/utils/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0      806 2023-04-14 15:10:31.968199 upstash_py-0.1.0/upstash_py/utils/__pycache__/comparison.cpython-311.pyc
--rw-r--r--   0        0        0     4592 2023-05-04 09:53:23.644989 upstash_py-0.1.0/upstash_py/utils/__pycache__/exception.cpython-311.pyc
--rw-r--r--   0        0        0     6553 2023-05-04 15:29:10.957427 upstash_py-0.1.0/upstash_py/utils/__pycache__/format.cpython-311.pyc
--rw-r--r--   0        0        0      107 2023-04-13 16:18:51.335437 upstash_py-0.1.0/upstash_py/utils/base.py
--rw-r--r--   0        0        0      242 2023-04-14 14:58:16.064260 upstash_py-0.1.0/upstash_py/utils/comparison.py
--rw-r--r--   0        0        0     3333 2023-05-04 07:39:00.163434 upstash_py-0.1.0/upstash_py/utils/exception.py
--rw-r--r--   0        0        0     4088 2023-05-04 15:26:27.420397 upstash_py-0.1.0/upstash_py/utils/format.py
--rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 upstash_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       37 2023-03-04 10:43:41.243570 upstash_py-0.2.0/README.md
+-rw-r--r--   0        0        0      379 2023-05-11 14:14:38.035799 upstash_py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-04 11:23:56.540070 upstash_py-0.2.0/upstash_py/__init__.py
+-rw-r--r--   0        0        0    83393 2023-05-11 14:06:26.783008 upstash_py-0.2.0/upstash_py/client.py
+-rw-r--r--   0        0        0      308 2023-05-11 14:05:49.019292 upstash_py-0.2.0/upstash_py/config.py
+-rw-r--r--   0        0        0       44 2023-03-08 07:44:02.265644 upstash_py-0.2.0/upstash_py/exception.py
+-rw-r--r--   0        0        0      755 2023-05-04 15:53:00.952164 upstash_py-0.2.0/upstash_py/http/decode.py
+-rw-r--r--   0        0        0     1629 2023-04-13 15:37:48.050511 upstash_py-0.2.0/upstash_py/http/execute.py
+-rw-r--r--   0        0        0     1030 2023-05-04 15:39:39.039487 upstash_py-0.2.0/upstash_py/play.py
+-rw-r--r--   0        0        0      115 2023-05-03 17:44:20.513271 upstash_py-0.2.0/upstash_py/play2.py
+-rw-r--r--   0        0        0      409 2023-04-14 12:17:17.899972 upstash_py-0.2.0/upstash_py/schema/commands/parameters.py
+-rw-r--r--   0        0        0      932 2023-04-14 14:37:49.938942 upstash_py-0.2.0/upstash_py/schema/commands/returns.py
+-rw-r--r--   0        0        0      761 2023-04-13 15:35:06.241703 upstash_py-0.2.0/upstash_py/schema/http.py
+-rw-r--r--   0        0        0      107 2023-04-13 16:18:51.335437 upstash_py-0.2.0/upstash_py/utils/base.py
+-rw-r--r--   0        0        0      242 2023-04-14 14:58:16.064260 upstash_py-0.2.0/upstash_py/utils/comparison.py
+-rw-r--r--   0        0        0     3333 2023-05-04 07:39:00.163434 upstash_py-0.2.0/upstash_py/utils/exception.py
+-rw-r--r--   0        0        0     4088 2023-05-04 15:26:27.420397 upstash_py-0.2.0/upstash_py/utils/format.py
+-rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 upstash_py-0.2.0/PKG-INFO
```

### Comparing `upstash_py-0.1.0/upstash_py/client.py` & `upstash_py-0.2.0/upstash_py/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from upstash_py.http.execute import execute
 from upstash_py.schema.http import RESTResult, RESTEncoding
 from upstash_py.config import (
-    ENABLE_TELEMETRY,
     REST_ENCODING,
     REST_RETRIES,
     REST_RETRY_INTERVAL,
+    ALLOW_TELEMETRY,
     ALLOW_DEPRECATED,
     FORMAT_RETURN
 )
 from upstash_py.utils.format import (
     format_geo_positions_return,
     format_geo_members_return,
     format_hash_return,
@@ -32,40 +32,66 @@
     HashReturn,
     FormattedHashReturn,
     SortedSetReturn,
     FormattedSortedSetReturn
 )
 from aiohttp import ClientSession
 from typing import Type, Any, Self, Literal
+from os import environ
 
 
 class Redis:
     def __init__(
         self,
         url: str,
         token: str,
-        enable_telemetry: bool = ENABLE_TELEMETRY,
         rest_encoding: RESTEncoding = REST_ENCODING,
         rest_retries: int = REST_RETRIES,
         rest_retry_interval: int = REST_RETRY_INTERVAL,
         allow_deprecated: bool = ALLOW_DEPRECATED,
-        format_return: bool = FORMAT_RETURN
+        format_return: bool = FORMAT_RETURN,
+        allow_telemetry: bool = ALLOW_TELEMETRY
     ):
         self.url = url
         self.token = token
 
-        self.enable_telemetry = enable_telemetry
+        self.allow_telemetry = allow_telemetry
 
         self.allow_deprecated = allow_deprecated
         self.format_return = format_return
 
         self.rest_encoding = rest_encoding
         self.rest_retries = rest_retries
         self.rest_retry_interval = rest_retry_interval
 
+    @classmethod
+    def from_env(
+        cls,
+        rest_encoding: RESTEncoding = REST_ENCODING,
+        rest_retries: int = REST_RETRIES,
+        rest_retry_interval: int = REST_RETRY_INTERVAL,
+        allow_deprecated: bool = ALLOW_DEPRECATED,
+        format_return: bool = FORMAT_RETURN,
+        allow_telemetry: bool = ALLOW_TELEMETRY,
+    ):
+        """
+        Load the credentials from environment.
+        """
+
+        return cls(
+            environ["UPSTASH_REDIS_REST_URL"],
+            environ["UPSTASH_REDIS_REST_TOKEN"],
+            rest_encoding,
+            rest_retries,
+            rest_retry_interval,
+            allow_deprecated,
+            format_return,
+            allow_telemetry
+        )
+
     async def __aenter__(self) -> ClientSession:
         """
         Enter the async context.
         """
 
         self._session: ClientSession = ClientSession()
         # It needs to return the session object because it will be used in "async with" statements.
@@ -346,21 +372,21 @@
         count: int | None = None,
         scan_type: str | None = None,
         return_cursor: bool = True
     ) -> (list[str | list[str]] | list[int | list[str]]) | list[str]:
         """
         See https://redis.io/commands/scan
 
-        "MATCH" was replaced with "pattern".
+        :param pattern: replacement for "MATCH"
 
-        "COUNT" defaults to 10.
+        :param count: defaults to 10 on the server side
 
-        "TYPE" was replaced with "scan_type".
+        :param scan_type: replacement for "TYPE"
 
-        If "return_cursor" is False, it won't return the cursor.
+        :param return_cursor: if set to False, it won't return the cursor
         """
 
         command: list = ["SCAN", cursor]
 
         if pattern is not None:
             command.extend(["MATCH", pattern])
 
@@ -427,15 +453,15 @@
         nx: bool = False,
         xx: bool = False,
         ch: bool = False,
     ) -> int:
         """
         See https://redis.io/commands/geoadd
 
-        The members should be added as a sequence of GeoMember dict types (longitude, latitude, name).
+        :param members: a sequence of GeoMember dict types (longitude, latitude, name).
         """
 
         if len(members) == 0:
             raise Exception("At least one member must be added.")
 
         if nx and xx:
             raise Exception("\"nx\" and \"xx\" are mutually exclusive.")
@@ -461,16 +487,14 @@
         key: str,
         first_member: str,
         second_member: str,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"] = "M"
     ) -> str | float | None:
         """
         See https://redis.io/commands/geodist
-
-        The measuring unit can be specified with "unit".
         """
 
         command: list = ["GEODIST", key, first_member, second_member, unit]
 
         raw: str | None = await self.run(command)
 
         return float(raw) if self.format_return else raw
@@ -514,21 +538,18 @@
         sort: Literal["ASC", "DESC"] | None = None,
         store_as: str | None = None,
         store_distance_as: str | None = None
     ) -> GeoMembersReturn | FormattedGeoMembersReturn | int:
         """
         See https://redis.io/commands/georadius
 
-        The measuring unit can be specified with "unit".
-
-        "ANY" was replaced with "count_any".
+        :param count_any: replacement for "ANY"
 
-        The sorting options can be specified with "sort".
-
-        "[STORE and STORE_DIST] key" are written as "store_as" and "store_distance_as".
+        :param store_as: replacement for "STORE"
+        :param store_distance_as: replacement for "STORE_DIST"
         """
 
         if not self.allow_deprecated:
             raise Exception("""From version 6.2.0, this command is deprecated.
 It can be replaced by "geosearch" and "geosearchstore" with the "radius" argument.
 Source: https://redis.io/commands/georadius""")
 
@@ -588,19 +609,15 @@
         count: int | None = None,
         count_any: bool = False,
         sort: Literal["ASC", "DESC"] | None = None
     ) -> GeoMembersReturn | FormattedGeoMembersReturn:
         """
         See https://redis.io/commands/georadius_ro
 
-        The measuring unit can be specified with "unit".
-
-        "ANY" was replaced with "count_any".
-
-        The sorting options can be specified with "sort".
+        :param count_any: replacement for "ANY"
         """
 
         if not self.allow_deprecated:
             raise Exception("""From version 6.2.0, this command is deprecated.
 It can be replaced by "geosearch" with the "radius" argument.
 Source: https://redis.io/commands/georadius_ro""")
 
@@ -648,21 +665,18 @@
         sort: Literal["ASC", "DESC"] | None = None,
         store_as: str | None = None,
         store_distance_as: str | None = None
     ) -> GeoMembersReturn | FormattedGeoMembersReturn:
         """
         See https://redis.io/commands/georadiusbymember
 
-        The measuring unit can be specified with "unit".
-
-        "ANY" was replaced with "count_any".
+        :param count_any: replacement for "ANY"
 
-        The sorting options can be specified with "sort".
-
-        "[STORE and STORE_DIST] key" are written as "store_as" and "store_distance_as".
+        :param store_as: replacement for "STORE"
+        :param store_distance_as: replacement for "STORE_DIST"
         """
 
         if not self.allow_deprecated:
             raise Exception("""From version 6.2.0, this command is deprecated.
 It can be replaced by "geosearch" and "geosearchstore" with the "radius" and "member" arguments.
 Source: https://redis.io/commands/georadiusbymember""")
 
@@ -721,19 +735,15 @@
         count: int | None = None,
         count_any: bool = False,
         sort: Literal["ASC", "DESC"] | None = None
     ) -> GeoMembersReturn | FormattedGeoMembersReturn:
         """
         See https://redis.io/commands/georadiusbymember
 
-        The measuring unit can be specified with "unit".
-
-        "ANY" was replaced with "count_any".
-
-        The sorting options can be specified with "sort".
+        :param count_any: replacement for "ANY"
         """
 
         if not self.allow_deprecated:
             raise Exception("""From version 6.2.0, this command is deprecated.
         It can be replaced by "geosearch" with the "radius" and "member" arguments.
         Source: https://redis.io/commands/georadiusbymember""")
 
@@ -783,27 +793,25 @@
         with_distance: bool = False,
         with_hash: bool = False,
         with_coordinates: bool = False
     ) -> GeoMembersReturn | FormattedGeoMembersReturn:
         """
         See https://redis.io/commands/geosearch
 
-        "FROMMEMBER" was replaced with "member".
-
-        "FROMLONLAT" was replaced with "longitude" and "latitude".
-
-        "BYRADIUS" was replaced with "radius".
+        :param member: replacement for "FROMMEMBER"
 
-        "BYBOX" was replaced with "width" and "height".
+        :param longitude: replacement for "FROMLONLAT" together with "latitude"
+        :param latitude: replacement for "FROMLONLAT" together with "longitude"
 
-        The measuring unit can be specified with "unit".
+        :param radius: replacement for "BYRADIUS"
 
-        The sorting options can be specified with "sort".
+        :param width: replacement for "BYBOX" together with "height"
+        :param height: replacement for "BYBOX" together with "width"
 
-        "ANY" was replaced with "count_any".
+        :param count_any: replacement for "ANY"
         """
 
         handle_geosearch_exceptions(member, longitude, latitude, radius, width, height, count, count_any)
 
         command: list = ["GEOSEARCH", key]
 
         if member is not None:
@@ -860,27 +868,27 @@
         count: int | None = None,
         count_any: bool = False,
         store_distance: bool = False
     ) -> int:
         """
         See https://redis.io/commands/geosearchstore
 
-        "FROMMEMBER" was replaced with "member".
+        :param member: replacement for "FROMMEMBER"
 
-        "FROMLONLAT" was replaced with "longitude" and "latitude".
+        :param longitude: replacement for "FROMLONLAT" together with "latitude"
+        :param latitude: replacement for "FROMLONLAT" together with "longitude"
 
-        "BYRADIUS" was replaced with "radius".
+        :param radius: replacement for "BYRADIUS"
 
-        "BYBOX" was replaced with "width" and "height".
+        :param width: replacement for "BYBOX" together with "height"
+        :param height: replacement for "BYBOX" together with "width"
 
-        The measuring unit can be specified with "unit".
+        :param count_any: replacement for "ANY"
 
-        "ASC" and "DESC" are written as sort.
-
-        "ANY" was replaced with "count_any".
+        :param store_distance: replacement for "STOREDIST"
         """
 
         handle_geosearch_exceptions(member, longitude, latitude, radius, width, height, count, count_any)
 
         command: list = ["GEOSEARCHSTORE", destination_key, source_key]
 
         if member is not None:
@@ -1025,17 +1033,15 @@
         key: str,
         count: int | None = None,
         with_values: bool = False
     ) -> (str | None) | (HashReturn | FormattedHashReturn):
         """
         See https://redis.io/commands/hrandfield
 
-        "COUNT" defaults to 1.
-
-        "count" can only be used together with "with_values".
+        :param count: defaults to 1 on the server side
         """
 
         if count is None and with_values:
             raise Exception("\"with_values\" can only be used together with \"count\"")
 
         command: list = ["HRANDFIELD", key]
 
@@ -1058,19 +1064,19 @@
         pattern: str | None = None,
         count: int | None = None,
         return_cursor: bool = True
     ) -> (list[str | HashReturn] | list[int | FormattedHashReturn]) | (HashReturn | FormattedHashReturn):
         """
         See https://redis.io/commands/hscan
 
-        "MATCH" was replaced with "pattern".
+        :param pattern: replacement for "MATCH"
 
-        "COUNT" defaults to 10.
+        :param count: defaults to 10 on the server side
 
-        If "return_cursor" is False, it won't return the cursor.
+        :param return_cursor: if set to False, it won't return the cursor
         """
 
         command: list = ["HSCAN", key, cursor]
 
         if pattern is not None:
             command.extend(["MATCH", pattern])
 
@@ -1172,16 +1178,14 @@
         key: str,
         position: Literal["BEFORE", "AFTER"],
         pivot: Any,
         element: Any
     ) -> int:
         """
         See https://redis.io/commands/linsert
-
-        The positioning can be specified with "position".
         """
 
         command: list = ["LINSERT", key, position, pivot, element]
 
         return await self.run(command)
 
     async def llen(self, key: str) -> int:
@@ -1198,29 +1202,25 @@
         source_key: str,
         destination_key: str,
         source_position: Literal["LEFT", "RIGHT"],
         destination_position: Literal["LEFT", "RIGHT"]
     ) -> str | None:
         """
         See https://redis.io/commands/lmove
-
-        The positioning can be specified with "source_position" and "destination_position".
         """
 
         command: list = ["LMOVE", source_key, destination_key, source_position, destination_position]
 
         return await self.run(command)
 
     async def lpop(self, key: str, count: int | None = None) -> (str | None) | list[str]:
         """
         See https://redis.io/commands/lpop
 
-        "COUNT" defaults to 1.
-
-        If "count" is specified, it will return a list of values.
+        :param count: defaults to 1 on the server side
         """
 
         command: list = ["LPOP", key]
 
         if count is not None:
             command.append(count)
 
@@ -1233,18 +1233,17 @@
         first_return: int | None = None,
         count: int | None = None,
         max_number_of_comparisons: int | None = None
     ) -> (int | None) | list[int]:
         """
         See https://redis.io/commands/lpos
 
-        "RANK" was replaced with "first_return".
-        When set, it will return the positions starting from the specified occurrence.
+        :param first_return: replacement for "RANK"
 
-        "MAXLEN" was replaced with "max_number_of_comparisons".
+        :param max_number_of_comparisons: replacement for "MAXLEN"
         """
 
         command: list = ["LPOS", key, element]
 
         if first_return is not None:
             command.extend(["RANK", first_return])
 
@@ -1316,15 +1315,15 @@
 
         return await self.run(command)
 
     async def rpop(self, key: str, count: int | None = None) -> (str | None) | list[str]:
         """
         See https://redis.io/commands/rpop
 
-        "COUNT" defaults to 1.
+        :param count: defaults to 1 on the server side
         """
 
         command: list = ["RPOP", key]
 
         if count is not None:
             command.append(count)
 
@@ -1384,15 +1383,14 @@
 
         return PubSub(client=self)
 
     async def eval(self, script: str, keys: list[str] | None = None, arguments: list | None = None) -> Any:
         """
         See https://redis.io/commands/eval
 
-        The keys and arguments can be specified with the same-name parameters.
         The number of keys is calculated automatically.
         """
 
         command: list = ["EVAL", script]
 
         if keys:
             command.extend([len(keys), *keys])
@@ -1407,15 +1405,14 @@
         sha1_digest: str,
         keys: list[str] | None = None,
         arguments: list | None = None
     ) -> Any:
         """
         See https://redis.io/commands/evalsha
 
-        The keys and arguments can be specified with the same-name parameters.
         The number of keys is calculated automatically.
         """
 
         command: list = ["EVALSHA", sha1_digest]
 
         if keys:
             command.extend([len(keys), *keys])
@@ -1448,30 +1445,26 @@
         command: list = ["DBSIZE"]
 
         return await self.run(command)
 
     async def flushall(self, mode: Literal["ASYNC", "SYNC"] | None = None) -> str:
         """
         See https://redis.io/commands/flushall
-
-        The mode(ASYNC/SYNC) can be specified with the same-name parameter.
         """
 
         command: list = ["FLUSHALL"]
 
         if mode:
             command.append(mode)
 
         return await self.run(command)
 
     async def flushdb(self, mode: Literal["ASYNC", "SYNC"] | None = None) -> str:
         """
         See https://redis.io/commands/flushdb
-
-        The mode(ASYNC/SYNC) can be specified with the same-name parameter.
         """
 
         command: list = ["FLUSHDB"]
 
         if mode:
             command.append(mode)
 
@@ -1588,29 +1581,29 @@
 
         return bool(raw) if self.format_return else raw
 
     async def spop(self, key: str, count: int | None = None) -> (str | None) | list[str]:
         """
         See https://redis.io/commands/spop
 
-        "COUNT" defaults to 1.
+        :param count: defaults to 1 on the server side
         """
 
         command: list = ["SPOP", key]
 
         if count is not None:
             command.append(count)
 
         return await self.run(command)
 
     async def srandmember(self, key: str, count: int | None = None) -> (str | None) | list[str]:
         """
         See https://redis.io/commands/srandmember
 
-        "COUNT" defaults to 1.
+        :param count: defaults to 1 on the server side
         """
 
         command: list = ["SRANDMEMBER", key]
 
         if count is not None:
             command.append(count)
 
@@ -1635,19 +1628,19 @@
         pattern: str | None = None,
         count: int | None = None,
         return_cursor: bool = True
     ) -> (list[str | list[str]] | list[int | list[str]]) | list[str]:
         """
         See https://redis.io/commands/sscan
 
-        "MATCH" was replaced with "pattern".
+        :param pattern: replacement for "MATCH"
 
-        "COUNT" defaults to 10.
+        :param count: defaults to 10 on the server side
 
-        If "return_cursor" is False, it won't return the cursor.
+        :param return_cursor: if set to False, it won't return the cursor
         """
 
         command: list = ["SSCAN", key, cursor]
 
         if pattern is not None:
             command.extend(["MATCH", pattern])
 
@@ -1696,15 +1689,15 @@
         lt: bool = False,
         ch: bool = False,
         incr: bool = False
     ) -> int | (str | None | float):
         """
         See https://redis.io/commands/zadd
 
-        The members should be specified with a dict containing their names and scores.
+        :param sorted_set_members: a dict containing their names and scores.
         """
 
         if nx and xx:
             raise Exception("\"nx\" and \"xx\" are mutually exclusive.")
 
         if gt and lt:
             raise Exception("\"gt\" and \"lt\" are mutually exclusive.")
@@ -1826,15 +1819,15 @@
         with_scores: bool = False
     ) -> SortedSetReturn | FormattedSortedSetReturn:
         """
         See https://redis.io/commands/zinter
 
         The number of keys is calculated automatically.
 
-        The "WEIGHTS" can be specified with "multiplication_factors".
+        :param multiplication_factors: replacement for "WEIGHTS"
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: list = ["ZINTER", len(keys), *keys]
 
@@ -1861,15 +1854,15 @@
         aggregate: Literal["SUM", "MIN", "MAX"] | None = None
     ) -> int:
         """
         See https://redis.io/commands/zinterstore
 
         The number of keys is calculated automatically.
 
-        The "WEIGHTS" can be specified with "multiplication_factors".
+        :param multiplication_factors: replacement for "WEIGHTS"
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: list = ["ZINTERSTORE", destination_key, len(keys), *keys]
 
@@ -1909,15 +1902,15 @@
 
         return format_float_list(raw) if self.format_return else raw
 
     async def zpopmax(self, key: str, count: int | None = None) -> SortedSetReturn | FormattedSortedSetReturn:
         """
         See https://redis.io/commands/zpopmax
 
-        "COUNT" defaults to 1.
+        :param count: defaults to 1 on the server side
         """
 
         command: list = ["ZPOPMAX", key]
 
         if count is not None:
             command.append(count)
 
@@ -1925,15 +1918,15 @@
 
         return format_sorted_set_return(raw) if self.format_return else raw
 
     async def zpopmin(self, key: str, count: int | None = None) -> SortedSetReturn | FormattedSortedSetReturn:
         """
         See https://redis.io/commands/zpopmin
 
-        "COUNT" defaults to 1.
+        :param count: defaults to 1 on the server side
         """
 
         command: list = ["ZPOPMIN", key]
 
         if count is not None:
             command.append(count)
 
@@ -1946,15 +1939,15 @@
         key: str,
         count: int | None = None,
         with_scores: bool = False
     ) -> (str | None) | (SortedSetReturn | FormattedSortedSetReturn):
         """
         See https://redis.io/commands/zrandmember
 
-        "COUNT" defaults to 1.
+        :param count: defaults to 1 on the server side
         """
 
         if count is None and with_scores:
             raise Exception("\"with_scores\" can only be used with \"count\".")
 
         command: list = ["ZRANDMEMBER", key]
 
@@ -1985,16 +1978,14 @@
         count: int | None = None,
         with_scores: bool = False
     ) -> SortedSetReturn | FormattedSortedSetReturn:
         """
         See https://redis.io/commands/zrange
 
         If you need to use "-inf" and "+inf", please write them as strings.
-
-        "BYSCORE" and "BYLEX" can be specified with "range_method".
         """
 
         handle_non_deprecated_zrange_exceptions(range_method, start, stop, offset, count)
 
         command: list = ["ZRANGE", key, start, stop]
 
         if range_method:
@@ -2096,17 +2087,16 @@
         count: int | None = None
     ) -> int:
         """
         See https://redis.io/commands/zrangestore
 
         If you need to use "-inf" and "+inf", please write them as strings.
 
-        "min" and "max" were replaced with "start" and "stop" to match "zrange".
-
-        "BYSCORE" and "BYLEX" can be specified with "range_method".
+        :param start: replacement for "min" to match "ZRANGE"
+        :param stop: replacement for "max" to match "ZRANGE"
         """
 
         handle_non_deprecated_zrange_exceptions(range_method, start, stop, offset, count)
 
         command: list = ["ZRANGESTORE", destination_key, source_key, start, stop]
 
         if range_method:
@@ -2293,19 +2283,19 @@
             list[str | SortedSetReturn] | list[int | FormattedSortedSetReturn]
          ) | (
             SortedSetReturn | FormattedSortedSetReturn
          ):
         """
         See https://redis.io/commands/zscan
 
-        "MATCH" was replaced with "pattern".
+        :param pattern: replacement for "MATCH"
 
-        "COUNT" defaults to 10.
+        :param count: defaults to 10 on the server side
 
-        If "return_cursor" is False, it won't return the cursor.
+        :param return_cursor: if set to False, it won't return the cursor
         """
 
         command: list = ["ZSCAN", key, cursor]
 
         if pattern is not None:
             command.extend(["MATCH", pattern])
 
@@ -2343,15 +2333,15 @@
         with_scores: bool = False
     ) -> SortedSetReturn | FormattedSortedSetReturn:
         """
         See https://redis.io/commands/zunion
 
         The number of keys is calculated automatically.
 
-        The "WEIGHTS" can be specified with "multiplication_factors".
+        :param multiplication_factors: replacement for "WEIGHTS"
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: list = ["ZUNION", len(keys), *keys]
 
@@ -2378,15 +2368,15 @@
         aggregate: Literal["SUM", "MIN", "MAX"] | None = None
     ) -> int:
         """
         See https://redis.io/commands/zunionstore
 
         The number of keys is calculated automatically.
 
-        The "WEIGHTS" can be specified with "multiplication_factors".
+        :param multiplication_factors: replacement for "WEIGHTS"
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: list = ["ZUNIONSTORE", destination_key, len(keys), *keys]
 
@@ -2394,15 +2384,15 @@
             command.extend(["WEIGHTS", *multiplication_factors])
 
         if aggregate:
             command.extend(["AGGREGATE", aggregate])
 
         return await self.run(command)
 
-    async def append_to_string(self, key: str, value: Any) -> int:
+    async def append(self, key: str, value: Any) -> int:
         """
         See https://redis.io/commands/append
         """
 
         command: list = ["APPEND", key, value]
 
         return await self.run(command)
@@ -2450,17 +2440,14 @@
         milliseconds: int | None = None,
         unix_time_seconds: int | None = None,
         unix_time_milliseconds: int | None = None,
         persist: bool | None = None
     ) -> str | None:
         """
         See https://redis.io/commands/getex
-
-        The optional expiration settings ("EX", "PX", "EXAT", "PXAT") except for "PERSIST"
-        were replaced with their corresponding units.
         """
 
         if not number_are_not_none(seconds, milliseconds, unix_time_seconds, unix_time_milliseconds, persist, number=1):
             raise Exception("Exactly one of the expiration settings must be specified.")
 
         command: list = ["GETEX", key]
 
@@ -2544,30 +2531,26 @@
         command: list = ["MGET", *keys]
 
         return await self.run(command)
 
     async def mset(self, keys_and_values: dict) -> Literal["OK"]:
         """
         See https://redis.io/commands/mset
-
-        The key-value pairs should be specified as a dict.
         """
 
         command: list = ["MSET"]
 
         for key, value in keys_and_values.items():
             command.extend([key, value])
 
         return await self.run(command)
 
     async def msetnx(self, keys_and_values: dict) -> Literal[1, 0]:
         """
         See https://redis.io/commands/msetnx
-
-        The key-value pairs should be specified as a dict.
         """
 
         command: list = ["MSETNX"]
 
         for key, value in keys_and_values.items():
             command.extend([key, value])
 
@@ -2598,17 +2581,14 @@
         milliseconds: int | None = None,
         unix_time_seconds: int | None = None,
         unix_time_milliseconds: int | None = None,
         keep_ttl: bool = False,
     ) -> str | None:
         """
         See https://redis.io/commands/set
-
-        The optional expiration settings ("EX", "PX", "EXAT", "PXAT") except for "KEEPTTL"
-        were replaced with their corresponding units.
         """
 
         if nx and xx:
             raise Exception("\"nx\" and \"xx\" are mutually exclusive.")
 
         if not number_are_not_none(
             seconds,
@@ -2852,16 +2832,14 @@
         raw: list[Literal[1, 0]] = await self.client.run(command=self.command)
 
         return format_bool_list(raw) if self.client.format_return else raw
 
     async def flush(self, mode: Literal["ASYNC", "SYNC"]) -> str:
         """
         See https://redis.io/commands/script-flush
-
-        The mode(ASYNC/SYNC) can be specified with the same-name parameter.
         """
 
         self.command.append("FLUSH")
 
         if mode:
             self.command.append(mode)
```

### Comparing `upstash_py-0.1.0/upstash_py/http/decode.py` & `upstash_py-0.2.0/upstash_py/http/decode.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.1.0/upstash_py/http/execute.py` & `upstash_py-0.2.0/upstash_py/http/execute.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.1.0/upstash_py/play.py` & `upstash_py-0.2.0/upstash_py/play.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.1.0/upstash_py/schema/commands/returns.py` & `upstash_py-0.2.0/upstash_py/schema/commands/returns.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.1.0/upstash_py/schema/http.py` & `upstash_py-0.2.0/upstash_py/schema/http.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.1.0/upstash_py/utils/exception.py` & `upstash_py-0.2.0/upstash_py/utils/exception.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.1.0/upstash_py/utils/format.py` & `upstash_py-0.2.0/upstash_py/utils/format.py`

 * *Files identical despite different names*

