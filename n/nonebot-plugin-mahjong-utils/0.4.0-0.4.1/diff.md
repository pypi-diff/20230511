# Comparing `tmp/nonebot_plugin_mahjong_utils-0.4.0.tar.gz` & `tmp/nonebot_plugin_mahjong_utils-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mahjong_utils-0.4.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_mahjong_utils-0.4.1.tar", max compression
```

## Comparing `nonebot_plugin_mahjong_utils-0.4.0.tar` & `nonebot_plugin_mahjong_utils-0.4.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1085 2022-07-09 13:18:24.594000 nonebot_plugin_mahjong_utils-0.4.0/LICENSE
--rw-r--r--   0        0        0      919 2023-05-10 11:35:02.628324 nonebot_plugin_mahjong_utils-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3534 2023-03-16 12:07:47.636668 nonebot_plugin_mahjong_utils-0.4.0/README.MD
--rw-r--r--   0        0        0      941 2022-10-28 10:58:23.689084 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/__init__.py
--rw-r--r--   0        0        0      240 2023-03-16 05:44:00.915248 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/config.py
--rw-r--r--   0        0        0      189 2022-10-12 05:26:13.228000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/errors.py
--rw-r--r--   0        0        0        0 2022-10-25 03:16:47.484405 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/interceptors/__init__.py
--rw-r--r--   0        0        0     1077 2022-10-28 04:43:00.181550 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/interceptors/handle_error.py
--rw-r--r--   0        0        0     2841 2023-03-16 05:33:04.579502 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/__init__.py
--rw-r--r--   0        0        0     5535 2023-05-10 11:12:36.694007 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/__init__.py
--rw-r--r--   0        0        0        0 2023-03-16 08:59:43.174046 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/__init__.py
--rw-r--r--   0        0        0     7596 2023-03-16 08:59:43.175046 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/hora.html
--rw-r--r--   0        0        0     1199 2023-05-10 10:57:35.211129 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/macro.html
--rw-r--r--   0        0        0     4378 2023-05-10 11:12:26.323005 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_with_furo_chance.html
--rw-r--r--   0        0        0     3992 2023-05-10 10:51:21.949420 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_with_got.html
--rw-r--r--   0        0        0     3046 2023-05-10 10:43:58.233027 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_without_got.html
--rw-r--r--   0        0        0     5576 2023-05-10 10:35:32.648208 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/style.css
--rw-r--r--   0        0        0     8950 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1m.png
--rw-r--r--   0        0        0    18795 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1p.png
--rw-r--r--   0        0        0    22413 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1s.png
--rw-r--r--   0        0        0     8811 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1z.png
--rw-r--r--   0        0        0     9745 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2m.png
--rw-r--r--   0        0        0    17356 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2p.png
--rw-r--r--   0        0        0     6209 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2s.png
--rw-r--r--   0        0        0     9551 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2z.png
--rw-r--r--   0        0        0    10515 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3m.png
--rw-r--r--   0        0        0    15690 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3p.png
--rw-r--r--   0        0        0     6826 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3s.png
--rw-r--r--   0        0        0     8325 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3z.png
--rw-r--r--   0        0        0    10864 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4m.png
--rw-r--r--   0        0        0    11817 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4p.png
--rw-r--r--   0        0        0     7292 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4s.png
--rw-r--r--   0        0        0     7796 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4z.png
--rw-r--r--   0        0        0    11368 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5m.png
--rw-r--r--   0        0        0    16208 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5p.png
--rw-r--r--   0        0        0     9209 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5s.png
--rw-r--r--   0        0        0     2378 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5z.png
--rw-r--r--   0        0        0    10639 2023-02-08 09:08:22.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6m.png
--rw-r--r--   0        0        0    24300 2023-02-08 09:08:22.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6p.png
--rw-r--r--   0        0        0     7406 2023-02-08 09:08:22.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6s.png
--rw-r--r--   0        0        0    11157 2023-02-08 09:08:22.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6z.png
--rw-r--r--   0        0        0    10301 2023-02-08 09:08:22.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7m.png
--rw-r--r--   0        0        0    27853 2023-02-08 09:08:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7p.png
--rw-r--r--   0        0        0     8950 2023-02-08 09:08:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7s.png
--rw-r--r--   0        0        0     6974 2023-02-08 09:08:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7z.png
--rw-r--r--   0        0        0     9766 2023-02-08 09:08:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8m.png
--rw-r--r--   0        0        0    29174 2023-02-08 09:09:14.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8p.png
--rw-r--r--   0        0        0    12229 2023-02-08 09:09:14.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8s.png
--rw-r--r--   0        0        0    10729 2023-02-08 09:09:14.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9m.png
--rw-r--r--   0        0        0    15222 2023-02-08 09:09:14.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9p.png
--rw-r--r--   0        0        0    14338 2023-02-08 09:09:30.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9s.png
--rw-r--r--   0        0        0        0 2023-03-16 08:59:43.178047 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/__init__.py
--rw-r--r--   0        0        0     2452 2023-02-08 09:08:48.000000 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/back.png
--rw-r--r--   0        0        0        0 2023-03-16 05:07:09.349989 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/plaintext/__init__.py
--rw-r--r--   0        0        0     1671 2023-02-12 06:44:03.234610 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/plaintext/general.py
--rw-r--r--   0        0        0      523 2023-03-16 05:28:01.956561 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/plaintext/hand.py
--rw-r--r--   0        0        0     2902 2023-03-16 07:03:21.870608 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/plaintext/hora.py
--rw-r--r--   0        0        0     2758 2023-03-16 06:13:12.023382 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/plaintext/point_by_han_hu.py
--rw-r--r--   0        0        0     6120 2023-05-10 11:12:26.318005 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/plaintext/shanten.py
--rw-r--r--   0        0        0       85 2022-11-29 12:28:13.089457 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/matchers/__init__.py
--rw-r--r--   0        0        0     2053 2023-03-16 05:28:01.961565 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/matchers/furo_judge_sniffer.py
--rw-r--r--   0        0        0      903 2023-03-16 05:28:01.950560 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/matchers/han_hu.py
--rw-r--r--   0        0        0     3162 2023-03-16 05:28:01.946563 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/matchers/tiles_sniffer.py
--rw-r--r--   0        0        0        0 2022-10-25 03:16:47.486405 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/utils/__init__.py
--rw-r--r--   0        0        0      447 2022-12-30 05:32:42.206121 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/utils/executor.py
--rw-r--r--   0        0        0      878 2022-10-25 03:16:47.487405 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/utils/parser.py
--rw-r--r--   0        0        0       98 2023-03-15 15:57:29.141134 nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/utils/percentile.py
--rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 nonebot_plugin_mahjong_utils-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-07-09 13:18:24.594000 nonebot_plugin_mahjong_utils-0.4.1/LICENSE
+-rw-r--r--   0        0        0      919 2023-05-11 15:23:00.487212 nonebot_plugin_mahjong_utils-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3534 2023-03-16 12:07:47.636668 nonebot_plugin_mahjong_utils-0.4.1/README.MD
+-rw-r--r--   0        0        0      941 2022-10-28 10:58:23.689084 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/__init__.py
+-rw-r--r--   0        0        0      240 2023-03-16 05:44:00.915248 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/config.py
+-rw-r--r--   0        0        0      189 2022-10-12 05:26:13.228000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/errors.py
+-rw-r--r--   0        0        0        0 2022-10-25 03:16:47.484405 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/interceptors/__init__.py
+-rw-r--r--   0        0        0     1077 2022-10-28 04:43:00.181550 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/interceptors/handle_error.py
+-rw-r--r--   0        0        0     2841 2023-03-16 05:33:04.579502 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/__init__.py
+-rw-r--r--   0        0        0     5535 2023-05-11 15:19:02.882987 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-16 08:59:43.174046 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/__init__.py
+-rw-r--r--   0        0        0     7596 2023-03-16 08:59:43.175046 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/hora.html
+-rw-r--r--   0        0        0     1199 2023-05-10 10:57:35.211129 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/macro.html
+-rw-r--r--   0        0        0     4400 2023-05-11 15:19:18.474961 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_with_furo_chance.html
+-rw-r--r--   0        0        0     4012 2023-05-11 15:19:18.478961 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_with_got.html
+-rw-r--r--   0        0        0     3074 2023-05-11 15:19:18.482962 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_without_got.html
+-rw-r--r--   0        0        0     5576 2023-05-10 10:35:32.648208 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/style.css
+-rw-r--r--   0        0        0     8950 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1m.png
+-rw-r--r--   0        0        0    18795 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1p.png
+-rw-r--r--   0        0        0    22413 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1s.png
+-rw-r--r--   0        0        0     8811 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1z.png
+-rw-r--r--   0        0        0     9745 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2m.png
+-rw-r--r--   0        0        0    17356 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2p.png
+-rw-r--r--   0        0        0     6209 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2s.png
+-rw-r--r--   0        0        0     9551 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2z.png
+-rw-r--r--   0        0        0    10515 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3m.png
+-rw-r--r--   0        0        0    15690 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3p.png
+-rw-r--r--   0        0        0     6826 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3s.png
+-rw-r--r--   0        0        0     8325 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3z.png
+-rw-r--r--   0        0        0    10864 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4m.png
+-rw-r--r--   0        0        0    11817 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4p.png
+-rw-r--r--   0        0        0     7292 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4s.png
+-rw-r--r--   0        0        0     7796 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4z.png
+-rw-r--r--   0        0        0    11368 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5m.png
+-rw-r--r--   0        0        0    16208 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5p.png
+-rw-r--r--   0        0        0     9209 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5s.png
+-rw-r--r--   0        0        0     2378 2023-02-08 09:07:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5z.png
+-rw-r--r--   0        0        0    10639 2023-02-08 09:08:22.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6m.png
+-rw-r--r--   0        0        0    24300 2023-02-08 09:08:22.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6p.png
+-rw-r--r--   0        0        0     7406 2023-02-08 09:08:22.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6s.png
+-rw-r--r--   0        0        0    11157 2023-02-08 09:08:22.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6z.png
+-rw-r--r--   0        0        0    10301 2023-02-08 09:08:22.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7m.png
+-rw-r--r--   0        0        0    27853 2023-02-08 09:08:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7p.png
+-rw-r--r--   0        0        0     8950 2023-02-08 09:08:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7s.png
+-rw-r--r--   0        0        0     6974 2023-02-08 09:08:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7z.png
+-rw-r--r--   0        0        0     9766 2023-02-08 09:08:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8m.png
+-rw-r--r--   0        0        0    29174 2023-02-08 09:09:14.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8p.png
+-rw-r--r--   0        0        0    12229 2023-02-08 09:09:14.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8s.png
+-rw-r--r--   0        0        0    10729 2023-02-08 09:09:14.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9m.png
+-rw-r--r--   0        0        0    15222 2023-02-08 09:09:14.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9p.png
+-rw-r--r--   0        0        0    14338 2023-02-08 09:09:30.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9s.png
+-rw-r--r--   0        0        0        0 2023-03-16 08:59:43.178047 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/__init__.py
+-rw-r--r--   0        0        0     2452 2023-02-08 09:08:48.000000 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/back.png
+-rw-r--r--   0        0        0        0 2023-03-16 05:07:09.349989 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/__init__.py
+-rw-r--r--   0        0        0     1671 2023-02-12 06:44:03.234610 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/general.py
+-rw-r--r--   0        0        0      523 2023-03-16 05:28:01.956561 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/hand.py
+-rw-r--r--   0        0        0     2902 2023-03-16 07:03:21.870608 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/hora.py
+-rw-r--r--   0        0        0     2758 2023-03-16 06:13:12.023382 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/point_by_han_hu.py
+-rw-r--r--   0        0        0     6148 2023-05-11 15:19:18.487961 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/shanten.py
+-rw-r--r--   0        0        0       85 2022-11-29 12:28:13.089457 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/matchers/__init__.py
+-rw-r--r--   0        0        0     2053 2023-03-16 05:28:01.961565 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/matchers/furo_judge_sniffer.py
+-rw-r--r--   0        0        0      903 2023-03-16 05:28:01.950560 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/matchers/han_hu.py
+-rw-r--r--   0        0        0     3162 2023-03-16 05:28:01.946563 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/matchers/tiles_sniffer.py
+-rw-r--r--   0        0        0        0 2022-10-25 03:16:47.486405 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/utils/__init__.py
+-rw-r--r--   0        0        0      628 2023-05-11 15:39:37.142138 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/utils/executor.py
+-rw-r--r--   0        0        0      878 2022-10-25 03:16:47.487405 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/utils/parser.py
+-rw-r--r--   0        0        0       98 2023-03-15 15:57:29.141134 nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/utils/percentile.py
+-rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 nonebot_plugin_mahjong_utils-0.4.1/PKG-INFO
```

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/LICENSE` & `nonebot_plugin_mahjong_utils-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/pyproject.toml` & `nonebot_plugin_mahjong_utils-0.4.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "nonebot-plugin-mahjong-utils"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.MD"
 license = "MIT"
 repository = "https://github.com/ssttkkl/nonebot-plugin-mahjong-utils"
 packages = [
     { include = "nonebot_plugin_mahjong_utils", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 nonebot2 = "^2.0.0rc1"
-mahjong-utils = "^0.5.0"
+mahjong-utils = "^0.5.1"
 nonebot-plugin-htmlrender = { version = "^0.2.0.3", optional = true }
 nonebot-plugin-send-anything-anywhere = { version = "^0.2.1", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 nonebot2 = { version = "^2.0.0rc4", extras = ["fastapi"] }
 nonebot-adapter-onebot = "^2.2.1"
```

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/README.MD` & `nonebot_plugin_mahjong_utils-0.4.1/README.MD`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/__init__.py` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/interceptors/handle_error.py` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/interceptors/handle_error.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/__init__.py` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/__init__.py` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/hora.html` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/hora.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/macro.html` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/macro.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_with_furo_chance.html` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_with_furo_chance.html`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                             <span>共{{ shanten_after_action.advance_num }}张</span>
                         </div>
                     </div>
 
                     {% if shanten_num == 0 %}
                     <div class="table__td" style="flex: 5">
                         <div style="flex-direction: column">
-                            {{ macro.render_improvement(shanten_after_action.improvement, shanten_after_action.improvement_num, convert_improvement_view) }}
+                            {{ macro.render_improvement(shanten_after_action.good_shape_improvement, shanten_after_action.good_shape_improvement_num, convert_improvement_view) }}
                         </div>
                     </div>
                     {% endif %}
                     
                     {% if shanten_num == 1 %}
                     <div class="table__td" style="flex: 3">
                         <div style="flex-direction: column">
```

#### html2text {}

```diff
@@ -16,16 +16,16 @@
 {% if action[0] == 'pass' %} PASS {% elif action[0] == 'chi' %} {
 { macro.tiles_view(action[1].tiles) }}åæ{{ macro.tiles_view([action[2]]) }}
 {% elif action[0] == 'pon' %} ç¢°æ{{ macro.tiles_view([action[1]]) }} {% elif
 action[0] == 'minkan' %} æ  {% endif %}
 {{ macro.tiles_view(shanten_after_action.advance, size='small', style="display:
 block;") }} å±{{ shanten_after_action.advance_num }}å¼ 
 {% if shanten_num == 0 %}
-{{ macro.render_improvement(shanten_after_action.improvement,
-shanten_after_action.improvement_num, convert_improvement_view) }}
+{{ macro.render_improvement(shanten_after_action.good_shape_improvement,
+shanten_after_action.good_shape_improvement_num, convert_improvement_view) }}
 {% endif %} {% if shanten_num == 1 %}
 {{ macro.tiles_view(shanten_after_action.good_shape_advance, size='small',
 style="display: block;") }} å±{{ shanten_after_action.good_shape_advance_num
 }}å¼ 
 {{ macro.percentile_str(shanten_after_action.good_shape_advance_num /
 shanten_after_action.advance_num) }}
 {% endif %}
```

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_with_got.html` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_with_got.html`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
                     <div class="table__head__item" style="flex: {% if shanten_num == 1 or shanten_num == 0 %} 4 {% else %} 9 {% endif %}">
                         进张
                     </div>
 
                     {% if shanten_num == 0 %}
                     <div class="table__head__item" style="flex: 5">
-                        改良
+                        好型改良
                     </div>
                     {% endif %}
                     
                     {% if shanten_num == 1 %}
                     <div class="table__head__item" style="flex: 3">
                         好型进张
                     </div>
@@ -55,25 +55,25 @@
                         <span>打</span>
                         {% elif action[0] == 'ankan' %}
                         <span>暗杠</span>
                         {% endif %}
                         {{ macro.tiles_view([action[1]], size='small') }}
                     </div>
 
-                    <div class="table__head__item" style="flex: {% if shanten_num == 1 or shanten_num == 0 %} 4 {% else %} 9 {% endif %}">
+                    <div class="table__td" style="flex: {% if shanten_num == 1 or shanten_num == 0 %} 4 {% else %} 9 {% endif %}">
                         <div style="flex-direction: column">
                             {{ macro.tiles_view(shanten_after_action.advance, size='small', style="display: block;") }}
                             <span>共{{ shanten_after_action.advance_num }}张</span>
                         </div>
                     </div>
 
                     {% if shanten_num == 0 %}
                     <div class="table__td" style="flex: 5">
                         <div style="flex-direction: column">
-                            {{ macro.render_improvement(shanten_after_action.improvement, shanten_after_action.improvement_num, convert_improvement_view) }}
+                            {{ macro.render_improvement(shanten_after_action.good_shape_improvement, shanten_after_action.good_shape_improvement_num, convert_improvement_view) }}
                         </div>
                     </div>
                     {% endif %}
                     
                     {% if shanten_num == 1 %}
                     <div class="table__td" style="flex: 3">
                         <div style="flex-direction: column">
```

#### html2text {}

```diff
@@ -2,27 +2,27 @@
 {% import "macro.html" as macro %}
 {{ macro.tiles_view(tiles, sorted=False) }}
 å·²æ¸ç
 {% for shanten_num, shanten in grouped_shanten %}
  {{ macro.shanten_text(shanten_num) }}
 è¿å¼ 
 {% if shanten_num == 0 %}
-æ¹è¯
+å¥½åæ¹è¯
 {% endif %} {% if shanten_num == 1 %}
 å¥½åè¿å¼ 
 å¥½åç
 {% endif %}
 {% for action, shanten_after_action in shanten %}
 {% if action[0] == 'discard' %} æ {% elif action[0] == 'ankan' %} ææ  {%
 endif %} {{ macro.tiles_view([action[1]], size='small') }}
 {{ macro.tiles_view(shanten_after_action.advance, size='small', style="display:
 block;") }} å±{{ shanten_after_action.advance_num }}å¼ 
 {% if shanten_num == 0 %}
-{{ macro.render_improvement(shanten_after_action.improvement,
-shanten_after_action.improvement_num, convert_improvement_view) }}
+{{ macro.render_improvement(shanten_after_action.good_shape_improvement,
+shanten_after_action.good_shape_improvement_num, convert_improvement_view) }}
 {% endif %} {% if shanten_num == 1 %}
 {{ macro.tiles_view(shanten_after_action.good_shape_advance, size='small',
 style="display: block;") }} å±{{ shanten_after_action.good_shape_advance_num
 }}å¼ 
 {{ macro.percentile_str(shanten_after_action.good_shape_advance_num /
 shanten_after_action.advance_num) }}
 {% endif %}
```

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_without_got.html` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/shanten_without_got.html`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                 <div class="table__head">
                     <div class="table__head__item" style="flex: 5">
                         进张
                     </div>
 
                     {% if result.shanten == 0 %}
                     <div class="table__head__item" style="flex: 4">
-                        改良
+                        好型改良
                     </div>
                     {% endif %}
 
                     {% if result.shanten == 1 %}
                     <div class="table__head__item" style="flex: 4">
                         好型进张
                     </div>
@@ -51,15 +51,15 @@
                             <span>共{{ result.advance_num }}张</span>
                         </div>
                     </div>
 
                     {% if result.shanten == 0 %}
                     <div class="table__td" style="flex: 4">
                         <div style="flex-direction: column">
-                            {{ macro.render_improvement(result.improvement, result.improvement_num, convert_improvement_view) }}
+                            {{ macro.render_improvement(result.good_shape_improvement, result.good_shape_improvement_num, convert_improvement_view) }}
                         </div>
                     </div>
                     {% endif %}
 
                     {% if result.shanten == 1 %}
                     <div class="table__td" style="flex: 4">
                         <div style="flex-direction: column">
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
 
 {% import "macro.html" as macro %}
 {{ macro.tiles_view(tiles, sorted=False) }}
 æªæ¸ç
  {{ macro.shanten_text(result.shanten) }}
 è¿å¼ 
 {% if result.shanten == 0 %}
-æ¹è¯
+å¥½åæ¹è¯
 {% endif %} {% if result.shanten == 1 %}
 å¥½åè¿å¼ 
 å¥½åç
 {% endif %}
 {{ macro.tiles_view(result.advance, size='small', style="display: block;") }}
 å±{{ result.advance_num }}å¼ 
 {% if result.shanten == 0 %}
-{{ macro.render_improvement(result.improvement, result.improvement_num,
-convert_improvement_view) }}
+{{ macro.render_improvement(result.good_shape_improvement,
+result.good_shape_improvement_num, convert_improvement_view) }}
 {% endif %} {% if result.shanten == 1 %}
 {{ macro.tiles_view(result.good_shape_advance, size='small', style="display:
 block;") }} å±{{ result.good_shape_advance_num }}å¼ 
 {{ macro.percentile_str(result.good_shape_advance_num / result.advance_num) }}
 {% endif %}
```

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/style.css` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/style.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1m.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1m.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1p.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1p.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1s.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1s.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1z.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/1z.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2m.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2m.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2p.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2p.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2s.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2s.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2z.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/2z.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3m.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3m.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3p.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3p.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3s.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3s.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3z.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/3z.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4m.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4m.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4p.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4p.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4s.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4s.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4z.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/4z.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5m.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5m.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5p.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5p.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5s.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5s.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5z.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/5z.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6m.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6m.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6p.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6p.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6s.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6s.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6z.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/6z.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7m.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7m.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7p.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7p.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7s.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7s.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7z.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/7z.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8m.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8m.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8p.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8p.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8s.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/8s.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9m.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9m.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9p.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9p.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9s.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/9s.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/back.png` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/htmlrender/templates/tiles/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/plaintext/general.py` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/general.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/plaintext/hand.py` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/hand.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/plaintext/hora.py` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/hora.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/plaintext/point_by_han_hu.py` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/point_by_han_hu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/mapper/plaintext/shanten.py` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/mapper/plaintext/shanten.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 def map_shanten_without_got(io: TextIO, shanten: ShantenWithoutGot):
     if shanten.shanten == 1:
         io.write(
             f"进张：{tiles_text(sorted(shanten.advance))} ({shanten.advance_num}张，好型{shanten.good_shape_advance_num}张)")
     else:
         io.write(f"进张：{tiles_text(sorted(shanten.advance))} ({shanten.advance_num}张)")
 
-    if shanten.improvement:
-        io.write("\n改良：")
+    if shanten.good_shape_improvement:
+        io.write("\n好型改良：")
 
         improvement = []
 
-        for t in shanten.improvement:
+        for t in shanten.good_shape_improvement:
             imp = t, [x.discard for x in shanten.improvement[t]], shanten.improvement[t][0].advance_num
             improvement.append(imp)
 
         improvement.sort(key=lambda x: x[0])
 
         for i, (t, discard, advance_num) in enumerate(improvement):
             io.write(f"{t}（打{'/'.join(map(str, discard))}，听{advance_num}张）")
```

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/matchers/furo_judge_sniffer.py` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/matchers/furo_judge_sniffer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/matchers/han_hu.py` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/matchers/han_hu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/matchers/tiles_sniffer.py` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/matchers/tiles_sniffer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/src/nonebot_plugin_mahjong_utils/utils/parser.py` & `nonebot_plugin_mahjong_utils-0.4.1/src/nonebot_plugin_mahjong_utils/utils/parser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_utils-0.4.0/PKG-INFO` & `nonebot_plugin_mahjong_utils-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mahjong-utils
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Home-page: https://github.com/ssttkkl/nonebot-plugin-mahjong-utils
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: htmlrender
-Requires-Dist: mahjong-utils (>=0.5.0,<0.6.0)
+Requires-Dist: mahjong-utils (>=0.5.1,<0.6.0)
 Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0.3,<0.3.0.0) ; extra == "htmlrender"
 Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.1,<0.3.0) ; extra == "htmlrender"
 Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0)
 Project-URL: Repository, https://github.com/ssttkkl/nonebot-plugin-mahjong-utils
 Description-Content-Type: text/plain
 
 nonebot-plugin-mahjong-utils
```

