# Comparing `tmp/tdxpy-0.2.0.tar.gz` & `tmp/tdxpy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdxpy-0.2.0.tar", max compression
+gzip compressed data, was "tdxpy-0.2.1.tar", max compression
```

## Comparing `tdxpy-0.2.0.tar` & `tdxpy-0.2.1.tar`

### file list

```diff
@@ -1,56 +1,58 @@
--rw-r--r--   0        0        0     1064 2023-05-08 05:02:45.303090 tdxpy-0.2.0/LICENSE
--rw-r--r--   0        0        0     1289 2023-05-08 05:02:56.770731 tdxpy-0.2.0/README.md
--rw-r--r--   0        0        0      960 2023-05-08 05:02:56.774731 tdxpy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       63 2023-05-08 05:02:56.786730 tdxpy-0.2.0/tdxpy/__init__.py
--rw-r--r--   0        0        0     9372 2023-05-08 05:02:56.786730 tdxpy-0.2.0/tdxpy/base_socket_client.py
--rw-r--r--   0        0        0     6405 2023-05-08 05:02:56.790730 tdxpy-0.2.0/tdxpy/constants.py
--rw-r--r--   0        0        0       48 2023-05-08 05:02:45.307090 tdxpy-0.2.0/tdxpy/crawler/__init__.py
--rw-r--r--   0        0        0     3487 2023-05-08 05:02:56.790730 tdxpy-0.2.0/tdxpy/crawler/base_crawler.py
--rw-r--r--   0        0        0     5975 2023-05-08 05:02:56.790730 tdxpy-0.2.0/tdxpy/crawler/history_financial_crawler.py
--rw-r--r--   0        0        0      419 2023-05-08 05:02:56.790730 tdxpy-0.2.0/tdxpy/exceptions.py
--rw-r--r--   0        0        0     4910 2023-05-08 05:02:56.794730 tdxpy-0.2.0/tdxpy/exhq.py
--rw-r--r--   0        0        0     1391 2023-05-08 05:02:56.794730 tdxpy-0.2.0/tdxpy/heartbeat.py
--rw-r--r--   0        0        0     4495 2023-05-08 05:02:56.794730 tdxpy-0.2.0/tdxpy/helper.py
--rw-r--r--   0        0        0    11429 2023-05-08 05:02:56.794730 tdxpy-0.2.0/tdxpy/hq.py
--rw-r--r--   0        0        0      320 2023-05-08 05:02:56.798730 tdxpy-0.2.0/tdxpy/logger.py
--rw-r--r--   0        0        0        0 2023-05-08 05:02:45.311090 tdxpy-0.2.0/tdxpy/parser/__init__.py
--rw-r--r--   0        0        0     4753 2023-05-08 05:02:56.798730 tdxpy-0.2.0/tdxpy/parser/base.py
--rw-r--r--   0        0        0        0 2023-05-08 05:02:45.311090 tdxpy-0.2.0/tdxpy/parser/ext/__init__.py
--rw-r--r--   0        0        0     2603 2023-05-08 05:02:56.798730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_history_instrument_bars_range.py
--rw-r--r--   0        0        0     1221 2023-05-08 05:02:56.802730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_history_minute_time_data.py
--rw-r--r--   0        0        0     4170 2023-05-08 05:02:56.802730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_history_transaction_data.py
--rw-r--r--   0        0        0     2124 2023-05-08 05:02:56.802730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_instrument_bars.py
--rw-r--r--   0        0        0      342 2023-05-08 05:02:56.802730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_instrument_count.py
--rw-r--r--   0        0        0     1350 2023-05-08 05:02:56.806730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_instrument_info.py
--rw-r--r--   0        0        0     2852 2023-05-08 05:02:56.806730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_instrument_quote.py
--rw-r--r--   0        0        0     6320 2023-05-08 05:02:56.806730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_instrument_quote_list.py
--rw-r--r--   0        0        0     1252 2023-05-08 05:02:56.810730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_markets.py
--rw-r--r--   0        0        0     1330 2023-05-08 05:02:56.810730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_minute_time_data.py
--rw-r--r--   0        0        0     4077 2023-05-08 05:02:56.810730 tdxpy-0.2.0/tdxpy/parser/ext/ex_get_transaction_data.py
--rw-r--r--   0        0        0      396 2023-05-08 05:02:56.810730 tdxpy-0.2.0/tdxpy/parser/raw_parser.py
--rw-r--r--   0        0        0     1316 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/setup_commands.py
--rw-r--r--   0        0        0        0 2023-05-08 05:02:45.315090 tdxpy-0.2.0/tdxpy/parser/std/__init__.py
--rw-r--r--   0        0        0     2324 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_block_info.py
--rw-r--r--   0        0        0     1506 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_company_info_category.py
--rw-r--r--   0        0        0     1071 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_company_info_content.py
--rw-r--r--   0        0        0     3998 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_finance_info.py
--rw-r--r--   0        0        0     1436 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_history_minute_time_data.py
--rw-r--r--   0        0        0     1734 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_history_transaction_data.py
--rw-r--r--   0        0        0     3055 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_index_bars.py
--rw-r--r--   0        0        0     1082 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_minute_time_data.py
--rw-r--r--   0        0        0      975 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_report_file.py
--rw-r--r--   0        0        0     2837 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_security_bars.py
--rw-r--r--   0        0        0      568 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_security_count.py
--rw-r--r--   0        0        0     1411 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_security_list.py
--rw-r--r--   0        0        0     7836 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_security_quotes.py
--rw-r--r--   0        0        0     1687 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_transaction_data.py
--rw-r--r--   0        0        0     3867 2023-05-08 05:02:56.814729 tdxpy-0.2.0/tdxpy/parser/std/get_xdxr_info.py
--rw-r--r--   0        0        0      744 2023-05-08 05:02:45.315090 tdxpy-0.2.0/tdxpy/reader/__init__.py
--rw-r--r--   0        0        0     1301 2023-05-08 05:02:56.818729 tdxpy-0.2.0/tdxpy/reader/base_reader.py
--rw-r--r--   0        0        0     4385 2023-05-08 05:02:56.818729 tdxpy-0.2.0/tdxpy/reader/block_reader.py
--rw-r--r--   0        0        0     5611 2023-05-08 05:02:56.818729 tdxpy-0.2.0/tdxpy/reader/daily_bar_reader.py
--rw-r--r--   0        0        0     1711 2023-05-08 05:02:56.818729 tdxpy-0.2.0/tdxpy/reader/exhq_daily_bar_reader.py
--rw-r--r--   0        0        0      937 2023-05-08 05:02:56.822729 tdxpy-0.2.0/tdxpy/reader/history_financial_reader.py
--rw-r--r--   0        0        0     2587 2023-05-08 05:02:56.822729 tdxpy-0.2.0/tdxpy/reader/lc_min_bar_reader.py
--rw-r--r--   0        0        0     3052 2023-05-08 05:02:56.822729 tdxpy-0.2.0/tdxpy/reader/min_bar_reader.py
--rw-r--r--   0        0        0     1745 1970-01-01 00:00:00.000000 tdxpy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      324 2023-05-11 05:15:33.958134 tdxpy-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1064 2023-05-11 05:15:06.906347 tdxpy-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1289 2023-05-11 05:15:33.958134 tdxpy-0.2.1/README.md
+-rw-r--r--   0        0        0      960 2023-05-11 05:15:33.962134 tdxpy-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       63 2023-05-11 05:15:33.962134 tdxpy-0.2.1/tdxpy/__init__.py
+-rw-r--r--   0        0        0     9372 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/base_socket_client.py
+-rw-r--r--   0        0        0     6405 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/constants.py
+-rw-r--r--   0        0        0       48 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/crawler/__init__.py
+-rw-r--r--   0        0        0     3487 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/crawler/base_crawler.py
+-rw-r--r--   0        0        0     5975 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/crawler/history_financial_crawler.py
+-rw-r--r--   0        0        0      419 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/exceptions.py
+-rw-r--r--   0        0        0     4910 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/exhq.py
+-rw-r--r--   0        0        0     1391 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/heartbeat.py
+-rw-r--r--   0        0        0     4495 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/helper.py
+-rw-r--r--   0        0        0    11429 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/hq.py
+-rw-r--r--   0        0        0      320 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/logger.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/__init__.py
+-rw-r--r--   0        0        0     4753 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/base.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/__init__.py
+-rw-r--r--   0        0        0     2603 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_history_instrument_bars_range.py
+-rw-r--r--   0        0        0     1221 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_history_minute_time_data.py
+-rw-r--r--   0        0        0     4170 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_history_transaction_data.py
+-rw-r--r--   0        0        0     2124 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_instrument_bars.py
+-rw-r--r--   0        0        0      342 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_instrument_count.py
+-rw-r--r--   0        0        0     1350 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_instrument_info.py
+-rw-r--r--   0        0        0     2852 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_instrument_quote.py
+-rw-r--r--   0        0        0     6330 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_instrument_quote_list.py
+-rw-r--r--   0        0        0     1272 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_markets.py
+-rw-r--r--   0        0        0     1330 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_minute_time_data.py
+-rw-r--r--   0        0        0     4077 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/ext/ex_get_transaction_data.py
+-rw-r--r--   0        0        0      396 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/raw_parser.py
+-rw-r--r--   0        0        0     1316 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/setup_commands.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/std/__init__.py
+-rw-r--r--   0        0        0     2324 2023-05-11 05:15:06.910347 tdxpy-0.2.1/tdxpy/parser/std/get_block_info.py
+-rw-r--r--   0        0        0     1516 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_company_info_category.py
+-rw-r--r--   0        0        0     1081 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_company_info_content.py
+-rw-r--r--   0        0        0     3998 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_finance_info.py
+-rw-r--r--   0        0        0     1436 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_history_minute_time_data.py
+-rw-r--r--   0        0        0     1734 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_history_transaction_data.py
+-rw-r--r--   0        0        0     3055 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_index_bars.py
+-rw-r--r--   0        0        0     1082 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_minute_time_data.py
+-rw-r--r--   0        0        0      975 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_report_file.py
+-rw-r--r--   0        0        0     2837 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_security_bars.py
+-rw-r--r--   0        0        0      568 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_security_count.py
+-rw-r--r--   0        0        0     1411 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_security_list.py
+-rw-r--r--   0        0        0     7836 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_security_quotes.py
+-rw-r--r--   0        0        0     1687 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_transaction_data.py
+-rw-r--r--   0        0        0     3867 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/parser/std/get_xdxr_info.py
+-rw-r--r--   0        0        0      744 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/reader/__init__.py
+-rw-r--r--   0        0        0     1301 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/reader/base_reader.py
+-rw-r--r--   0        0        0     4385 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/reader/block_reader.py
+-rw-r--r--   0        0        0     5611 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/reader/daily_bar_reader.py
+-rw-r--r--   0        0        0     1711 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/reader/exhq_daily_bar_reader.py
+-rw-r--r--   0        0        0      937 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/reader/history_financial_reader.py
+-rw-r--r--   0        0        0     2587 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/reader/lc_min_bar_reader.py
+-rw-r--r--   0        0        0     3052 2023-05-11 05:15:06.914347 tdxpy-0.2.1/tdxpy/reader/min_bar_reader.py
+-rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 tdxpy-0.2.1/setup.py
+-rw-r--r--   0        0        0     1795 1970-01-01 00:00:00.000000 tdxpy-0.2.1/PKG-INFO
```

### Comparing `tdxpy-0.2.0/LICENSE` & `tdxpy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/README.md` & `tdxpy-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/pyproject.toml` & `tdxpy-0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "tdxpy"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["bopo <ibopo@126.com>"]
 readme = "README.md"
 packages = [{ include = "tdxpy" }]
 include = ["CHANGELOG.md"]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 pandas = "^1.5.1"
 cryptography = "^38.0.3"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest-datadir = "^1.4.1"
 pytest-cov = "^4.0.0"
@@ -33,15 +33,15 @@
 testpaths = "tests"
 addopts = "-p no:warnings"
 
 log_cli = 1
 log_cli_level = "DEBUG"
 
 [tool.commitizen]
-version = "0.2.0"
+version = "0.2.1"
 tag_format = "v$version"
 
 update_changelog_on_bump = true
 changelog_file = "CHANGELOG.md"
 annotated_tag = true
 
 version_files = [
```

### Comparing `tdxpy-0.2.0/tdxpy/base_socket_client.py` & `tdxpy-0.2.1/tdxpy/base_socket_client.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/constants.py` & `tdxpy-0.2.1/tdxpy/constants.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/crawler/base_crawler.py` & `tdxpy-0.2.1/tdxpy/crawler/base_crawler.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/crawler/history_financial_crawler.py` & `tdxpy-0.2.1/tdxpy/crawler/history_financial_crawler.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/exhq.py` & `tdxpy-0.2.1/tdxpy/exhq.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/heartbeat.py` & `tdxpy-0.2.1/tdxpy/heartbeat.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/helper.py` & `tdxpy-0.2.1/tdxpy/helper.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/hq.py` & `tdxpy-0.2.1/tdxpy/hq.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/base.py` & `tdxpy-0.2.1/tdxpy/parser/base.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/ext/ex_get_history_instrument_bars_range.py` & `tdxpy-0.2.1/tdxpy/parser/ext/ex_get_history_instrument_bars_range.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/ext/ex_get_history_minute_time_data.py` & `tdxpy-0.2.1/tdxpy/parser/ext/ex_get_history_minute_time_data.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/ext/ex_get_history_transaction_data.py` & `tdxpy-0.2.1/tdxpy/parser/ext/ex_get_history_transaction_data.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/ext/ex_get_instrument_bars.py` & `tdxpy-0.2.1/tdxpy/parser/ext/ex_get_instrument_bars.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/ext/ex_get_instrument_info.py` & `tdxpy-0.2.1/tdxpy/parser/ext/ex_get_instrument_info.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/ext/ex_get_instrument_quote.py` & `tdxpy-0.2.1/tdxpy/parser/ext/ex_get_instrument_quote.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/ext/ex_get_instrument_quote_list.py` & `tdxpy-0.2.1/tdxpy/parser/ext/ex_get_instrument_quote_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
         if self.category not in [2, 3]:
             return NotImplementedError("暂时不支持期货,港股之外的品类")
 
         for _ in range(num):
             # 每个块一共300bytes
             market, code = struct.unpack("<B9s", body_buf[pos: pos + 10])
-            code = code.strip(b"\0").decode("gbk")  # to unicode
+            code = code.strip(b"\0").decode("gbk", "ignore")  # to unicode
             pos += 10
 
             if self.category == 3:
                 try:
                     pos = self.extract_futures(market, code, body_buf, data_list, pos)
                 except Exception as e:
                     logger.exception(e)
```

### Comparing `tdxpy-0.2.0/tdxpy/parser/ext/ex_get_markets.py` & `tdxpy-0.2.1/tdxpy/parser/ext/ex_get_markets.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         for _ in range(cnt):
             category, raw_name, market, raw_short_name, _, unknown_bytes = struct.unpack("<B32sB2s26s2s", body_buf[pos: pos + 64])
             pos += 64
 
             if category == 0 and market == 0:
                 continue
 
-            name = raw_name.decode("gbk")
-            short_name = raw_short_name.decode("gbk")
+            name = raw_name.decode("gbk", "ignore")
+            short_name = raw_short_name.decode("gbk", "ignore")
 
             result.append(
                 OrderedDict(
                     [
                         ("market", market),
                         ("category", category),
                         ("name", name.rstrip("\x00")),
```

### Comparing `tdxpy-0.2.0/tdxpy/parser/ext/ex_get_minute_time_data.py` & `tdxpy-0.2.1/tdxpy/parser/ext/ex_get_minute_time_data.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/ext/ex_get_transaction_data.py` & `tdxpy-0.2.1/tdxpy/parser/ext/ex_get_transaction_data.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/setup_commands.py` & `tdxpy-0.2.1/tdxpy/parser/setup_commands.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/std/get_block_info.py` & `tdxpy-0.2.1/tdxpy/parser/std/get_block_info.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/std/get_company_info_category.py` & `tdxpy-0.2.1/tdxpy/parser/std/get_company_info_category.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             """
             p = b.find(b"\x00")
 
             if p != -1:
                 b = b[0:p]
 
             try:
-                n = b.decode("gbk")
+                n = b.decode("gbk", "ignore")
             except Exception as e:
                 logger.exception(e)
                 n = "unknown_str"
 
             return n
 
         for _ in range(num):
```

### Comparing `tdxpy-0.2.0/tdxpy/parser/std/get_company_info_content.py` & `tdxpy-0.2.1/tdxpy/parser/std/get_company_info_content.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,10 +37,10 @@
         pos = 0
 
         _, length = struct.unpack("<10sH", body_buf[:12])
 
         pos += 12
 
         content = body_buf[pos: pos + length]
-        content = content.decode("gbk")
+        content = content.decode("gbk", "ignore")
 
         return content
```

### Comparing `tdxpy-0.2.0/tdxpy/parser/std/get_finance_info.py` & `tdxpy-0.2.1/tdxpy/parser/std/get_finance_info.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/std/get_history_minute_time_data.py` & `tdxpy-0.2.1/tdxpy/parser/std/get_history_minute_time_data.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/std/get_history_transaction_data.py` & `tdxpy-0.2.1/tdxpy/parser/std/get_history_transaction_data.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/std/get_index_bars.py` & `tdxpy-0.2.1/tdxpy/parser/std/get_index_bars.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/std/get_minute_time_data.py` & `tdxpy-0.2.1/tdxpy/parser/std/get_minute_time_data.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/std/get_report_file.py` & `tdxpy-0.2.1/tdxpy/parser/std/get_report_file.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/std/get_security_bars.py` & `tdxpy-0.2.1/tdxpy/parser/std/get_security_bars.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/std/get_security_count.py` & `tdxpy-0.2.1/tdxpy/parser/std/get_security_count.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/std/get_security_list.py` & `tdxpy-0.2.1/tdxpy/parser/std/get_security_list.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/std/get_security_quotes.py` & `tdxpy-0.2.1/tdxpy/parser/std/get_security_quotes.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/std/get_transaction_data.py` & `tdxpy-0.2.1/tdxpy/parser/std/get_transaction_data.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/parser/std/get_xdxr_info.py` & `tdxpy-0.2.1/tdxpy/parser/std/get_xdxr_info.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/reader/__init__.py` & `tdxpy-0.2.1/tdxpy/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/reader/base_reader.py` & `tdxpy-0.2.1/tdxpy/reader/base_reader.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/reader/block_reader.py` & `tdxpy-0.2.1/tdxpy/reader/block_reader.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/reader/daily_bar_reader.py` & `tdxpy-0.2.1/tdxpy/reader/daily_bar_reader.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/reader/exhq_daily_bar_reader.py` & `tdxpy-0.2.1/tdxpy/reader/exhq_daily_bar_reader.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/reader/history_financial_reader.py` & `tdxpy-0.2.1/tdxpy/reader/history_financial_reader.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/reader/lc_min_bar_reader.py` & `tdxpy-0.2.1/tdxpy/reader/lc_min_bar_reader.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/tdxpy/reader/min_bar_reader.py` & `tdxpy-0.2.1/tdxpy/reader/min_bar_reader.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.0/PKG-INFO` & `tdxpy-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: tdxpy
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: bopo
 Author-email: ibopo@126.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cryptography (>=38.0.3,<39.0.0)
 Requires-Dist: pandas (>=1.5.1,<2.0.0)
 Description-Content-Type: text/markdown
```

