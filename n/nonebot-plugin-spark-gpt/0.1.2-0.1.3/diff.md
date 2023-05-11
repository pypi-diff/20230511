# Comparing `tmp/nonebot_plugin_spark_gpt-0.1.2.tar.gz` & `tmp/nonebot_plugin_spark_gpt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_spark_gpt-0.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_spark_gpt-0.1.3.tar", max compression
```

## Comparing `nonebot_plugin_spark_gpt-0.1.2.tar` & `nonebot_plugin_spark_gpt-0.1.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1894 2023-05-11 03:29:22.094362 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/__init__.py
--rw-r--r--   0        0        0       16 2023-05-10 17:23:53.939876 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/chatgpt_web/__init__.py
--rw-r--r--   0        0        0     3919 2023-05-08 16:53:49.475522 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/chatgpt_web/chatgpt_web_func.py
--rw-r--r--   0        0        0     8228 2023-05-10 17:23:58.319737 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/chatgpt_web/config.py
--rw-r--r--   0        0        0    28144 2023-05-10 17:24:00.050884 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/chatgpt_web/main.py
--rw-r--r--   0        0        0     6131 2023-05-10 17:24:01.276809 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/chatgpt_web/web_api.py
--rw-r--r--   0        0        0       16 2023-05-10 17:24:06.325142 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/claude_slack/__init__.py
--rw-r--r--   0        0        0     3036 2023-05-10 17:24:07.826903 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/claude_slack/claude_func.py
--rw-r--r--   0        0        0     8094 2023-05-10 17:24:09.084792 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/claude_slack/config.py
--rw-r--r--   0        0        0    25921 2023-05-10 17:24:10.744126 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/claude_slack/main.py
--rw-r--r--   0        0        0     4309 2023-05-10 17:24:12.141727 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/claude_slack/slack_api.py
--rw-r--r--   0        0        0       16 2023-05-10 17:24:16.477844 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/__init__.py
--rw-r--r--   0        0        0     2633 2023-05-10 17:24:17.515144 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/common_func.py
--rw-r--r--   0        0        0     6158 2023-05-10 16:32:44.366675 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/config.py
--rw-r--r--   0        0        0     5563 2023-05-11 03:26:38.959437 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/main.py
--rw-r--r--   0        0        0     3936 2023-05-09 11:11:17.903494 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/__pycache__/render.cpython-310.pyc
--rw-r--r--   0        0        0     4066 2023-05-09 11:11:11.036002 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/render.py
--rw-r--r--   0        0        0    18464 2023-05-09 08:51:42.987873 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/github-markdown-light.css
--rw-r--r--   0        0        0  1458204 2023-04-22 14:17:13.496635 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.b64_fonts.css
--rw-r--r--   0        0        0   270288 2023-04-22 14:17:13.497555 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.js
--rw-r--r--   0        0        0     1290 2023-04-22 14:17:13.498611 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/katex/mathtex-script-type.min.js
--rw-r--r--   0        0        0      670 2023-05-09 08:51:13.189256 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/markdown.html
--rw-r--r--   0        0        0     1253 2023-05-09 05:07:59.973080 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/markdown_.html
--rw-r--r--   0        0        0     4625 2023-05-09 09:23:49.857905 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/pygments-default.css
--rw-r--r--   0        0        0    86342 2023-04-22 05:34:37.774678 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/source/background.png
--rw-r--r--   0        0        0     1137 2023-04-22 05:34:37.774678 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/source/banner.png
--rw-r--r--   0        0        0    86342 2023-04-22 05:34:37.775678 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/source/mi_background.png
--rw-r--r--   0        0        0      125 2023-04-22 14:17:13.500554 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/text.css
--rw-r--r--   0        0        0      233 2023-04-22 14:17:13.500554 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/text.html
--rw-r--r--   0        0        0     4244 2023-05-10 17:24:24.469959 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/newbing/config.py
--rw-r--r--   0        0        0    18363 2023-05-10 17:24:26.071103 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/newbing/main.py
--rw-r--r--   0        0        0     3068 2023-05-08 16:16:37.378665 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/newbing/newbing_func.py
--rw-r--r--   0        0        0       16 2023-05-08 03:59:58.447201 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/__init__.py
--rw-r--r--   0        0        0     9719 2023-05-10 14:13:15.440356 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/config.py
--rw-r--r--   0        0        0    29872 2023-05-10 16:30:34.806983 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/main.py
--rw-r--r--   0        0        0    10706 2023-05-08 03:59:52.713874 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/poe_api.py
--rw-r--r--   0        0        0     6332 2023-05-10 17:24:38.505890 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/poe_func.py
--rw-r--r--   0        0        0     2147 2023-05-08 03:59:48.875662 nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/pwframework.py
--rw-r--r--   0        0        0      920 2023-05-11 03:29:11.350702 nonebot_plugin_spark_gpt-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3042 2023-05-11 03:31:13.216645 nonebot_plugin_spark_gpt-0.1.2/README.md
--rw-r--r--   0        0        0     4173 1970-01-01 00:00:00.000000 nonebot_plugin_spark_gpt-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1894 2023-05-11 03:29:22.094362 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/__init__.py
+-rw-r--r--   0        0        0       16 2023-05-10 17:23:53.939876 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/chatgpt_web/__init__.py
+-rw-r--r--   0        0        0     3919 2023-05-08 16:53:49.475522 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/chatgpt_web/chatgpt_web_func.py
+-rw-r--r--   0        0        0     8228 2023-05-10 17:23:58.319737 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/chatgpt_web/config.py
+-rw-r--r--   0        0        0    28144 2023-05-10 17:24:00.050884 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/chatgpt_web/main.py
+-rw-r--r--   0        0        0     6131 2023-05-10 17:24:01.276809 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/chatgpt_web/web_api.py
+-rw-r--r--   0        0        0       16 2023-05-10 17:24:06.325142 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/claude_slack/__init__.py
+-rw-r--r--   0        0        0     3036 2023-05-10 17:24:07.826903 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/claude_slack/claude_func.py
+-rw-r--r--   0        0        0     8094 2023-05-10 17:24:09.084792 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/claude_slack/config.py
+-rw-r--r--   0        0        0    25921 2023-05-10 17:24:10.744126 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/claude_slack/main.py
+-rw-r--r--   0        0        0     4309 2023-05-10 17:24:12.141727 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/claude_slack/slack_api.py
+-rw-r--r--   0        0        0       16 2023-05-10 17:24:16.477844 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/__init__.py
+-rw-r--r--   0        0        0     2633 2023-05-10 17:24:17.515144 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/common_func.py
+-rw-r--r--   0        0        0     6158 2023-05-10 16:32:44.366675 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/config.py
+-rw-r--r--   0        0        0     5563 2023-05-11 03:26:38.959437 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/main.py
+-rw-r--r--   0        0        0     3936 2023-05-09 11:11:17.903494 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/__pycache__/render.cpython-310.pyc
+-rw-r--r--   0        0        0     4066 2023-05-09 11:11:11.036002 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/render.py
+-rw-r--r--   0        0        0    18464 2023-05-09 08:51:42.987873 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/github-markdown-light.css
+-rw-r--r--   0        0        0  1458204 2023-04-22 14:17:13.496635 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.b64_fonts.css
+-rw-r--r--   0        0        0   270288 2023-04-22 14:17:13.497555 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.js
+-rw-r--r--   0        0        0     1290 2023-04-22 14:17:13.498611 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/katex/mathtex-script-type.min.js
+-rw-r--r--   0        0        0      670 2023-05-09 08:51:13.189256 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/markdown.html
+-rw-r--r--   0        0        0     1253 2023-05-09 05:07:59.973080 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/markdown_.html
+-rw-r--r--   0        0        0     4625 2023-05-09 09:23:49.857905 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/pygments-default.css
+-rw-r--r--   0        0        0    86342 2023-04-22 05:34:37.774678 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/source/background.png
+-rw-r--r--   0        0        0     1137 2023-04-22 05:34:37.774678 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/source/banner.png
+-rw-r--r--   0        0        0    86342 2023-04-22 05:34:37.775678 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/source/mi_background.png
+-rw-r--r--   0        0        0      125 2023-04-22 14:17:13.500554 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/text.css
+-rw-r--r--   0        0        0      233 2023-04-22 14:17:13.500554 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/text.html
+-rw-r--r--   0        0        0     4244 2023-05-10 17:24:24.469959 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/newbing/config.py
+-rw-r--r--   0        0        0    18363 2023-05-10 17:24:26.071103 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/newbing/main.py
+-rw-r--r--   0        0        0     3068 2023-05-08 16:16:37.378665 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/newbing/newbing_func.py
+-rw-r--r--   0        0        0       16 2023-05-08 03:59:58.447201 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/__init__.py
+-rw-r--r--   0        0        0     9719 2023-05-10 14:13:15.440356 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/config.py
+-rw-r--r--   0        0        0    29872 2023-05-11 03:40:59.740884 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/main.py
+-rw-r--r--   0        0        0    10706 2023-05-08 03:59:52.713874 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/poe_api.py
+-rw-r--r--   0        0        0     6332 2023-05-10 17:24:38.505890 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/poe_func.py
+-rw-r--r--   0        0        0     2147 2023-05-08 03:59:48.875662 nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/pwframework.py
+-rw-r--r--   0        0        0      920 2023-05-11 03:43:01.601909 nonebot_plugin_spark_gpt-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3042 2023-05-11 03:31:13.216645 nonebot_plugin_spark_gpt-0.1.3/README.md
+-rw-r--r--   0        0        0     4173 1970-01-01 00:00:00.000000 nonebot_plugin_spark_gpt-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/__init__.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/chatgpt_web/chatgpt_web_func.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/chatgpt_web/chatgpt_web_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/chatgpt_web/config.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/chatgpt_web/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/chatgpt_web/main.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/chatgpt_web/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/chatgpt_web/web_api.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/chatgpt_web/web_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/claude_slack/claude_func.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/claude_slack/claude_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/claude_slack/config.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/claude_slack/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/claude_slack/main.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/claude_slack/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/claude_slack/slack_api.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/claude_slack/slack_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/common_func.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/common_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/config.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/main.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/__pycache__/render.cpython-310.pyc` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/__pycache__/render.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/render.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/render.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/github-markdown-light.css` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/github-markdown-light.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.b64_fonts.css` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.b64_fonts.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.js` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/katex/mathtex-script-type.min.js` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/katex/mathtex-script-type.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/markdown.html` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/markdown.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/markdown_.html` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/markdown_.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/pygments-default.css` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/pygments-default.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/source/background.png` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/source/background.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/source/banner.png` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/source/banner.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/common/render/templates/source/mi_background.png` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/common/render/templates/source/mi_background.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/newbing/config.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/newbing/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/newbing/main.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/newbing/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/newbing/newbing_func.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/newbing/newbing_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/config.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/main.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     create_msgs = state["create_msgs"]
     user_id = str(event.user_id)
     if infos in ["取消", "算了"]:
         create_msgs.append(await matcher.send(reply_out(event, "取消创建")))
         await delete_messages(bot, str(event.user_id), create_msgs)
         await poe_create_.finish()
 
-    infos = infos.split(" ", 1)
+    infos = infos.split(" ", 2)
     if not (len(infos) == 3 and infos[1] in ["1", "2"]):
         create_msgs.append(await matcher.send(reply_out(event, "输入信息有误，请检查后重新输入")))
         await poe_create_.reject()
 
     # 获取创建所需信息
 
     nickname = str(infos[0])
```

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/poe_api.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/poe_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/poe_func.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/poe_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/nonebot_plugin_spark_gpt/poe/pwframework.py` & `nonebot_plugin_spark_gpt-0.1.3/nonebot_plugin_spark_gpt/poe/pwframework.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/pyproject.toml` & `nonebot_plugin_spark_gpt-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_spark_gpt"
-version = "0.1.2"
+version = "0.1.3"
 description = "Spark-GPT,将多来源的gpt接入qq及更多平台,使用便捷,管理完善,功能强大"
 authors = ["canxin121 <1969730106@qq.com>"]
 readme = "README.md"
 packages = [{include = "nonebot_plugin_spark_gpt"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `nonebot_plugin_spark_gpt-0.1.2/README.md` & `nonebot_plugin_spark_gpt-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.2/PKG-INFO` & `nonebot_plugin_spark_gpt-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-spark-gpt
-Version: 0.1.2
+Version: 0.1.3
 Summary: Spark-GPT,将多来源的gpt接入qq及更多平台,使用便捷,管理完善,功能强大
 Author: canxin121
 Author-email: 1969730106@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-spark-gpt Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-spark-gpt Version: 0.1.3 Summary:
 Spark-
 GPT,å°å¤æ¥æºçgptæ¥å¥qqåæ´å¤å¹³å°,ä½¿ç¨ä¾¿æ·,ç®¡çå®å,åè½å¼ºå¤§
 Author: canxin121 Author-email: 1969730106@qq.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: onebot Requires-Dist: aiofiles (>=23.1.0,<24.0.0) Requires-
 Dist: aiohttp (>=3.8.4,<4.0.0) Requires-Dist: bidict (>=0.22.1,<0.23.0)
```

