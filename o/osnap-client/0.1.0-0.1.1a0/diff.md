# Comparing `tmp/osnap_client-0.1.0.tar.gz` & `tmp/osnap_client-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osnap_client-0.1.0.tar", max compression
+gzip compressed data, was "osnap_client-0.1.1a0.tar", max compression
```

## Comparing `osnap_client-0.1.0.tar` & `osnap_client-0.1.1a0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0    11357 2023-05-08 19:45:21.346835 osnap_client-0.1.0/LICENSE
--rw-r--r--   0        0        0     2100 2023-05-08 19:45:21.347228 osnap_client-0.1.0/README.md
--rw-r--r--   0        0        0      104 2023-04-30 13:42:55.538518 osnap_client-0.1.0/osnap_client/README.md
--rw-r--r--   0        0        0     2487 2023-05-08 19:45:21.354153 osnap_client-0.1.0/osnap_client/SwarmAdapters/BaseSwarmAdapter.py
--rw-r--r--   0        0        0     2781 2023-05-08 19:45:21.354324 osnap_client-0.1.0/osnap_client/SwarmAdapters/DiscordSwarmAdapter.py
--rw-r--r--   0        0        0      116 2023-05-08 19:45:21.354478 osnap_client-0.1.0/osnap_client/SwarmAdapters/__init__.py
--rw-r--r--   0        0        0      185 2023-05-08 19:45:21.354741 osnap_client-0.1.0/osnap_client/__init__.py
--rw-r--r--   0        0        0     3680 2023-05-08 19:45:21.354891 osnap_client-0.1.0/osnap_client/agents/OutboundAgents Spec.md
--rw-r--r--   0        0        0     3193 2023-05-08 19:45:21.355008 osnap_client-0.1.0/osnap_client/agents/PersonalAgent.py
--rw-r--r--   0        0        0     2484 2023-05-08 19:45:21.355126 osnap_client-0.1.0/osnap_client/agents/outbound_agent.py
--rw-r--r--   0        0        0     1365 2023-05-08 19:45:21.355231 osnap_client-0.1.0/osnap_client/agents/planner.py
--rw-r--r--   0        0        0     1419 2023-05-08 19:45:21.355437 osnap_client-0.1.0/osnap_client/core/api.py
--rw-r--r--   0        0        0     1314 2023-05-08 19:45:21.355551 osnap_client-0.1.0/osnap_client/core/crypt.py
--rw-r--r--   0        0        0    10280 2023-05-08 19:45:21.355693 osnap_client-0.1.0/osnap_client/core/osnap.py
--rw-r--r--   0        0        0     4902 2023-05-08 19:45:21.355822 osnap_client-0.1.0/osnap_client/main.py
--rw-r--r--   0        0        0       98 2023-05-08 19:45:21.355950 osnap_client-0.1.0/osnap_client/registry/__init__.py
--rw-r--r--   0        0        0     3149 2023-05-08 19:45:21.356129 osnap_client-0.1.0/osnap_client/registry/agent_registry.py
--rw-r--r--   0        0        0        0 2023-05-08 19:47:42.311354 osnap_client-0.1.0/osnap_client/registry/registry.py
--rw-r--r--   0        0        0     1813 2023-05-08 19:45:21.356252 osnap_client-0.1.0/osnap_client/registry/tool_registry.py
--rw-r--r--   0        0        0        0 2023-05-08 19:45:21.356306 osnap_client-0.1.0/osnap_client/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 19:45:21.356359 osnap_client-0.1.0/osnap_client/tools/main.py
--rw-r--r--   0        0        0     2449 2023-05-08 19:45:21.356653 osnap_client-0.1.0/osnap_client/utils/ai_engines/EngineBase.py
--rw-r--r--   0        0        0     2846 2023-05-08 19:45:21.356776 osnap_client-0.1.0/osnap_client/utils/ai_engines/GPTConversEngine.py
--rw-r--r--   0        0        0     2972 2023-05-08 19:45:21.356913 osnap_client-0.1.0/osnap_client/utils/ai_engines/LanchainGoogleEngine.py
--rw-r--r--   0        0        0      136 2023-05-08 19:45:21.357064 osnap_client-0.1.0/osnap_client/utils/ai_engines/__init__.py
--rw-r--r--   0        0        0     1036 2023-05-11 17:59:56.793343 osnap_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3039 1970-01-01 00:00:00.000000 osnap_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-08 19:45:21.346835 osnap_client-0.1.1a0/LICENSE
+-rw-r--r--   0        0        0     2100 2023-05-08 19:45:21.347228 osnap_client-0.1.1a0/README.md
+-rw-r--r--   0        0        0      104 2023-04-30 13:42:55.538518 osnap_client-0.1.1a0/osnap_client/README.md
+-rw-r--r--   0        0        0     2487 2023-05-08 19:45:21.354153 osnap_client-0.1.1a0/osnap_client/SwarmAdapters/BaseSwarmAdapter.py
+-rw-r--r--   0        0        0     2781 2023-05-08 19:45:21.354324 osnap_client-0.1.1a0/osnap_client/SwarmAdapters/DiscordSwarmAdapter.py
+-rw-r--r--   0        0        0      116 2023-05-08 19:45:21.354478 osnap_client-0.1.1a0/osnap_client/SwarmAdapters/__init__.py
+-rw-r--r--   0        0        0      185 2023-05-08 19:45:21.354741 osnap_client-0.1.1a0/osnap_client/__init__.py
+-rw-r--r--   0        0        0     3680 2023-05-08 19:45:21.354891 osnap_client-0.1.1a0/osnap_client/agents/OutboundAgents Spec.md
+-rw-r--r--   0        0        0     3193 2023-05-08 19:45:21.355008 osnap_client-0.1.1a0/osnap_client/agents/PersonalAgent.py
+-rw-r--r--   0        0        0     2484 2023-05-08 19:45:21.355126 osnap_client-0.1.1a0/osnap_client/agents/outbound_agent.py
+-rw-r--r--   0        0        0     1365 2023-05-08 19:45:21.355231 osnap_client-0.1.1a0/osnap_client/agents/planner.py
+-rw-r--r--   0        0        0     1419 2023-05-08 19:45:21.355437 osnap_client-0.1.1a0/osnap_client/core/api.py
+-rw-r--r--   0        0        0     1314 2023-05-08 19:45:21.355551 osnap_client-0.1.1a0/osnap_client/core/crypt.py
+-rw-r--r--   0        0        0    10280 2023-05-08 19:45:21.355693 osnap_client-0.1.1a0/osnap_client/core/osnap.py
+-rw-r--r--   0        0        0     4902 2023-05-08 19:45:21.355822 osnap_client-0.1.1a0/osnap_client/main.py
+-rw-r--r--   0        0        0       46 2023-05-04 11:18:07.891203 osnap_client-0.1.1a0/osnap_client/pubsub/__init__.py
+-rw-r--r--   0        0        0     2666 2023-05-04 12:56:55.387076 osnap_client-0.1.1a0/osnap_client/pubsub/pubsub.py
+-rw-r--r--   0        0        0       98 2023-05-08 19:45:21.355950 osnap_client-0.1.1a0/osnap_client/registry/__init__.py
+-rw-r--r--   0        0        0     3149 2023-05-08 19:45:21.356129 osnap_client-0.1.1a0/osnap_client/registry/agent_registry.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:47:42.311354 osnap_client-0.1.1a0/osnap_client/registry/registry.py
+-rw-r--r--   0        0        0     1813 2023-05-08 19:45:21.356252 osnap_client-0.1.1a0/osnap_client/registry/tool_registry.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:45:21.356306 osnap_client-0.1.1a0/osnap_client/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:45:21.356359 osnap_client-0.1.1a0/osnap_client/tools/main.py
+-rw-r--r--   0        0        0     2449 2023-05-08 19:45:21.356653 osnap_client-0.1.1a0/osnap_client/utils/ai_engines/EngineBase.py
+-rw-r--r--   0        0        0     2846 2023-05-08 19:45:21.356776 osnap_client-0.1.1a0/osnap_client/utils/ai_engines/GPTConversEngine.py
+-rw-r--r--   0        0        0     2972 2023-05-08 19:45:21.356913 osnap_client-0.1.1a0/osnap_client/utils/ai_engines/LanchainGoogleEngine.py
+-rw-r--r--   0        0        0      136 2023-05-08 19:45:21.357064 osnap_client-0.1.1a0/osnap_client/utils/ai_engines/__init__.py
+-rw-r--r--   0        0        0     1038 2023-05-11 18:23:24.253894 osnap_client-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0     3041 1970-01-01 00:00:00.000000 osnap_client-0.1.1a0/PKG-INFO
```

### Comparing `osnap_client-0.1.0/LICENSE` & `osnap_client-0.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.0/README.md` & `osnap_client-0.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.0/osnap_client/SwarmAdapters/BaseSwarmAdapter.py` & `osnap_client-0.1.1a0/osnap_client/SwarmAdapters/BaseSwarmAdapter.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.0/osnap_client/SwarmAdapters/DiscordSwarmAdapter.py` & `osnap_client-0.1.1a0/osnap_client/SwarmAdapters/DiscordSwarmAdapter.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.0/osnap_client/agents/OutboundAgents Spec.md` & `osnap_client-0.1.1a0/osnap_client/agents/OutboundAgents Spec.md`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.0/osnap_client/agents/PersonalAgent.py` & `osnap_client-0.1.1a0/osnap_client/agents/PersonalAgent.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.0/osnap_client/agents/outbound_agent.py` & `osnap_client-0.1.1a0/osnap_client/agents/outbound_agent.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.0/osnap_client/agents/planner.py` & `osnap_client-0.1.1a0/osnap_client/agents/planner.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.0/osnap_client/core/api.py` & `osnap_client-0.1.1a0/osnap_client/core/api.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.0/osnap_client/core/crypt.py` & `osnap_client-0.1.1a0/osnap_client/core/crypt.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.0/osnap_client/core/osnap.py` & `osnap_client-0.1.1a0/osnap_client/core/osnap.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.0/osnap_client/main.py` & `osnap_client-0.1.1a0/osnap_client/main.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.0/osnap_client/registry/agent_registry.py` & `osnap_client-0.1.1a0/osnap_client/registry/agent_registry.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.0/osnap_client/registry/tool_registry.py` & `osnap_client-0.1.1a0/osnap_client/registry/tool_registry.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.0/osnap_client/utils/ai_engines/EngineBase.py` & `osnap_client-0.1.1a0/osnap_client/utils/ai_engines/EngineBase.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.0/osnap_client/utils/ai_engines/GPTConversEngine.py` & `osnap_client-0.1.1a0/osnap_client/utils/ai_engines/GPTConversEngine.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.0/osnap_client/utils/ai_engines/LanchainGoogleEngine.py` & `osnap_client-0.1.1a0/osnap_client/utils/ai_engines/LanchainGoogleEngine.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.0/pyproject.toml` & `osnap_client-0.1.1a0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "osnap-client"
-version = "0.1.0"
+version = "0.1.1a0"
 description = ""
 authors = ["Forrest Murray <FMurray@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 langchain = "^0.0.154"
```

### Comparing `osnap_client-0.1.0/PKG-INFO` & `osnap_client-0.1.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osnap-client
-Version: 0.1.0
+Version: 0.1.1a0
 Summary: 
 Author: Forrest Murray
 Author-email: FMurray@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

