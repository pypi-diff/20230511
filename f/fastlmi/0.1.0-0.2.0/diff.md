# Comparing `tmp/fastlmi-0.1.0.tar.gz` & `tmp/fastlmi-0.2.0.tar.gz`

## Comparing `fastlmi-0.1.0.tar` & `fastlmi-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 fastlmi-0.1.0/.gitattributes
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fastlmi-0.1.0/CITATION.cff
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastlmi-0.1.0/requirements.txt
--rw-r--r--   0        0        0   145438 2020-02-02 00:00:00.000000 fastlmi-0.1.0/assets/oai_dice_roller.png
--rw-r--r--   0        0        0    22019 2020-02-02 00:00:00.000000 fastlmi-0.1.0/assets/oai_found_plugin.png
--rw-r--r--   0        0        0    35758 2020-02-02 00:00:00.000000 fastlmi-0.1.0/assets/oai_manifest.png
--rw-r--r--   0        0        0    33188 2020-02-02 00:00:00.000000 fastlmi-0.1.0/assets/oai_select_plugins.png
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 fastlmi-0.1.0/examples/dice_roller.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 fastlmi-0.1.0/fastlmi/__init__.py
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 fastlmi-0.1.0/fastlmi/application.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 fastlmi-0.1.0/fastlmi/utils.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fastlmi-0.1.0/fastlmi/openai/__init__.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 fastlmi-0.1.0/fastlmi/openai/models.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 fastlmi-0.1.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 fastlmi-0.1.0/LICENSE
--rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 fastlmi-0.1.0/README.md
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 fastlmi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6421 2020-02-02 00:00:00.000000 fastlmi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 fastlmi-0.2.0/.gitattributes
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fastlmi-0.2.0/CITATION.cff
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastlmi-0.2.0/requirements.txt
+-rw-r--r--   0        0        0   145438 2020-02-02 00:00:00.000000 fastlmi-0.2.0/assets/oai_dice_roller.png
+-rw-r--r--   0        0        0    22019 2020-02-02 00:00:00.000000 fastlmi-0.2.0/assets/oai_found_plugin.png
+-rw-r--r--   0        0        0    35758 2020-02-02 00:00:00.000000 fastlmi-0.2.0/assets/oai_manifest.png
+-rw-r--r--   0        0        0    33188 2020-02-02 00:00:00.000000 fastlmi-0.2.0/assets/oai_select_plugins.png
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 fastlmi-0.2.0/examples/ai_plugin_auth.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 fastlmi-0.2.0/examples/dice_roller.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 fastlmi-0.2.0/examples/logo.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 fastlmi-0.2.0/fastlmi/__init__.py
+-rw-r--r--   0        0        0     5592 2020-02-02 00:00:00.000000 fastlmi-0.2.0/fastlmi/application.py
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 fastlmi-0.2.0/fastlmi/auth.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fastlmi-0.2.0/fastlmi/typing.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 fastlmi-0.2.0/fastlmi/utils.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 fastlmi-0.2.0/fastlmi/ai_plugin/__init__.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 fastlmi-0.2.0/fastlmi/ai_plugin/models.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 fastlmi-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 fastlmi-0.2.0/LICENSE
+-rw-r--r--   0        0        0     8109 2020-02-02 00:00:00.000000 fastlmi-0.2.0/README.md
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 fastlmi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 fastlmi-0.2.0/PKG-INFO
```

### Comparing `fastlmi-0.1.0/assets/oai_dice_roller.png` & `fastlmi-0.2.0/assets/oai_dice_roller.png`

 * *Files identical despite different names*

### Comparing `fastlmi-0.1.0/assets/oai_found_plugin.png` & `fastlmi-0.2.0/assets/oai_found_plugin.png`

 * *Files identical despite different names*

### Comparing `fastlmi-0.1.0/assets/oai_manifest.png` & `fastlmi-0.2.0/assets/oai_manifest.png`

 * *Files identical despite different names*

### Comparing `fastlmi-0.1.0/assets/oai_select_plugins.png` & `fastlmi-0.2.0/assets/oai_select_plugins.png`

 * *Files identical despite different names*

### Comparing `fastlmi-0.1.0/examples/dice_roller.py` & `fastlmi-0.2.0/examples/dice_roller.py`

 * *Files identical despite different names*

### Comparing `fastlmi-0.1.0/fastlmi/openai/models.py` & `fastlmi-0.2.0/fastlmi/ai_plugin/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,12 +47,12 @@
 # ==== manifest ====
 class PluginManifest(BaseModel):
     schema_version: Literal["v1"]
     name_for_model: str
     name_for_human: str
     description_for_model: str
     description_for_human: str
-    auth: Union[ManifestNoAuth, ManifestServiceHttpAuth, ManifestUserHttpAuth, ManifestOAuthAuth]
+    auth: Union[ManifestServiceHttpAuth, ManifestUserHttpAuth, ManifestOAuthAuth, ManifestNoAuth]
     api: ApiSpec
     logo_url: str
     contact_email: str
     legal_info_url: str
```

### Comparing `fastlmi-0.1.0/.gitignore` & `fastlmi-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastlmi-0.1.0/LICENSE` & `fastlmi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastlmi-0.1.0/README.md` & `fastlmi-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -48,16 +48,16 @@
 ```shell
 $ pip install uvicorn
 # or pip install "uvicorn[standard]" for Cython-based extras 
 ```
 
 ## Example (OpenAI/ChatGPT Plugin)
 
-> NOTE: As of v0.1.0 FastLMI includes the OpenAI plugin interface as a default. This may change to an extension-based
-> system in the future as the library develops.
+> NOTE: As of v0.2.0 FastLMI includes the AI Plugin (OpenAI, LangChain) interface as a default. This may change to an
+> extension-based system in the future as the library develops.
 
 To show off just how easy it is to create a plugin, let's make a ChatGPT plugin that gives it the ability to roll dice
 in the d20 format (AIs playing D&D, anyone?).
 
 ### Example Requirements
 
 First, you'll need to install the [`d20`](https://github.com/avrae/d20) library:
@@ -122,50 +122,119 @@
 
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
 INFO:     Started server process [53532]
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 ```
 
-FastLMI automatically handles generating all the plugin metadata needed by OpenAI!
-
 ### Register it
 
 Finally, we need to tell ChatGPT about the new plugin.
 In the ChatGPT interface, select the "Plugins" model, then head to the Plugin Store -> Develop your own plugin.
 
 Here, type in the address of your plugin. By default, it's `localhost:8000`.
 
 ![](assets/oai_manifest.png "Enter your website domain")
 
-Click "Find manifest file," and you should see your plugin appear!
+Click "Find manifest file," and you should see your plugin appear. FastLMI automatically handles generating all the
+plugin metadata needed by OpenAI!
 
 ![](assets/oai_found_plugin.png "Found plugin")
 
-## Chat away
+### Chat away
 
 To use your new plugin, select it from the list of plugins when starting a new chat:
 
 ![](assets/oai_select_plugins.png "Select plugins")
 
 and start chatting. Congratulations! 🎉 You've just created a brand-new ChatGPT plugin - and we're excited to see what
 else you'll make!
 
 ![](assets/oai_dice_roller.png "Conversation with ChatGPT using Dice Roller")
 
+## Example (LangChain Tool)
+
+LangChain supports
+[interfacing with AI plugins](https://python.langchain.com/en/latest/modules/agents/tools/examples/chatgpt_plugins.html)!
+If you've followed the steps above (at least up through "Run it"), you can also expose your new LMI to a LangChain
+agent.
+
+This example assumes that you
+have [LangChain](https://python.langchain.com/en/latest/getting_started/getting_started.html) installed, and that your
+LMI is running at `http://localhost:8000`.
+
+```python
+from langchain.agents import AgentType
+from langchain.agents import initialize_agent, load_tools
+from langchain.chat_models import ChatOpenAI
+from langchain.tools import AIPluginTool
+
+tool = AIPluginTool.from_plugin_url("http://localhost:8000/.well-known/ai-plugin.json")
+llm = ChatOpenAI(temperature=0)
+tools = load_tools(["requests_all"])
+tools += [tool]
+
+agent_chain = initialize_agent(tools, llm, agent=AgentType.CHAT_ZERO_SHOT_REACT_DESCRIPTION, verbose=True)
+agent_chain.run("Can you roll me stats for a D&D character?")
+```
+
+## Authentication
+
+As of v0.2.0, FastLMI has built-in support for service-level auth, where the AI agent or LMI driver will send an
+authorization token you decide as a header with each request.
+
+Enabling authentication is easy! First, define the authentication scheme you wish to use - this will be a subclass of
+`LMIAuth`. For example, to provide service-level auth, you can define the `LMIServiceAuth` scheme:
+
+```python
+from fastlmi import Depends, FastLMI
+from fastlmi.auth import LMIServiceAuth
+
+auth = LMIServiceAuth(
+    access_tokens=["your_secret_token_here"],
+    verification_tokens={"openai": "verification_token_generated_in_the_ChatGPT_UI"}
+)
+```
+
+This auth scheme allows defining a set of allowed access tokens (if one wanted to, for example, have a different
+token for each plugin service). Then, when you define your app, all you have to do is add 2 parameters:
+
+```python
+app = FastLMI(..., auth=auth, dependencies=[Depends(auth)])
+```
+
+Tada! 🎉 Your LMI now tells consumers that it uses the `service_http` auth scheme, and will validate that each request
+to one of your defined routes provides a valid Bearer token.
+
+A complete example is in `examples/ai_plugin_auth.py`. You can read more about OpenAI's service-level
+auth [here](https://platform.openai.com/docs/plugins/authentication/service-level).
+
+### Route-Level Auth
+
+If you wanted to only require that certain routes use auth, you can also define the auth dependency on a route level:
+
+```diff
+- app = FastLMI(..., auth=auth, dependencies=[Depends(auth)])
++ app = FastLMI(..., auth=auth)
+...
+- @app.post("/hello")
++ @app.post("/hello", dependencies=[Depends(auth)])
+def hello():
+    ...
+```
+
 ## Read More
 
 Being based on FastAPI, FastLMI can take full advantage of its superpowers. Check out
 the [FastAPI documentation](https://fastapi.tiangolo.com/) for more!
 
 ## Todo
 
 - scopes
 - script to check for missing docs, over limits, etc
-- auth - for the moment, FastLMI does not support auth
 - logging
 - configure ecosystems
 
 <!--
 For developers:
 
 ## Build and Publish
```

### Comparing `fastlmi-0.1.0/pyproject.toml` & `fastlmi-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastlmi"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     { name = "Andrew Zhu", email = "andrew@zhu.codes" },
 ]
 description = "A FastAPI-based framework for quickly building and iterating on language model interfaces."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `fastlmi-0.1.0/PKG-INFO` & `fastlmi-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastlmi
-Version: 0.1.0
+Version: 0.2.0
 Summary: A FastAPI-based framework for quickly building and iterating on language model interfaces.
 Project-URL: Homepage, https://github.com/zhudotexe/fastlmi
 Project-URL: Bug Tracker, https://github.com/zhudotexe/fastlmi/issues
 Author-email: Andrew Zhu <andrew@zhu.codes>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: FastAPI
@@ -70,16 +70,16 @@
 ```shell
 $ pip install uvicorn
 # or pip install "uvicorn[standard]" for Cython-based extras 
 ```
 
 ## Example (OpenAI/ChatGPT Plugin)
 
-> NOTE: As of v0.1.0 FastLMI includes the OpenAI plugin interface as a default. This may change to an extension-based
-> system in the future as the library develops.
+> NOTE: As of v0.2.0 FastLMI includes the AI Plugin (OpenAI, LangChain) interface as a default. This may change to an
+> extension-based system in the future as the library develops.
 
 To show off just how easy it is to create a plugin, let's make a ChatGPT plugin that gives it the ability to roll dice
 in the d20 format (AIs playing D&D, anyone?).
 
 ### Example Requirements
 
 First, you'll need to install the [`d20`](https://github.com/avrae/d20) library:
@@ -144,50 +144,119 @@
 
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
 INFO:     Started server process [53532]
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 ```
 
-FastLMI automatically handles generating all the plugin metadata needed by OpenAI!
-
 ### Register it
 
 Finally, we need to tell ChatGPT about the new plugin.
 In the ChatGPT interface, select the "Plugins" model, then head to the Plugin Store -> Develop your own plugin.
 
 Here, type in the address of your plugin. By default, it's `localhost:8000`.
 
 ![](assets/oai_manifest.png "Enter your website domain")
 
-Click "Find manifest file," and you should see your plugin appear!
+Click "Find manifest file," and you should see your plugin appear. FastLMI automatically handles generating all the
+plugin metadata needed by OpenAI!
 
 ![](assets/oai_found_plugin.png "Found plugin")
 
-## Chat away
+### Chat away
 
 To use your new plugin, select it from the list of plugins when starting a new chat:
 
 ![](assets/oai_select_plugins.png "Select plugins")
 
 and start chatting. Congratulations! 🎉 You've just created a brand-new ChatGPT plugin - and we're excited to see what
 else you'll make!
 
 ![](assets/oai_dice_roller.png "Conversation with ChatGPT using Dice Roller")
 
+## Example (LangChain Tool)
+
+LangChain supports
+[interfacing with AI plugins](https://python.langchain.com/en/latest/modules/agents/tools/examples/chatgpt_plugins.html)!
+If you've followed the steps above (at least up through "Run it"), you can also expose your new LMI to a LangChain
+agent.
+
+This example assumes that you
+have [LangChain](https://python.langchain.com/en/latest/getting_started/getting_started.html) installed, and that your
+LMI is running at `http://localhost:8000`.
+
+```python
+from langchain.agents import AgentType
+from langchain.agents import initialize_agent, load_tools
+from langchain.chat_models import ChatOpenAI
+from langchain.tools import AIPluginTool
+
+tool = AIPluginTool.from_plugin_url("http://localhost:8000/.well-known/ai-plugin.json")
+llm = ChatOpenAI(temperature=0)
+tools = load_tools(["requests_all"])
+tools += [tool]
+
+agent_chain = initialize_agent(tools, llm, agent=AgentType.CHAT_ZERO_SHOT_REACT_DESCRIPTION, verbose=True)
+agent_chain.run("Can you roll me stats for a D&D character?")
+```
+
+## Authentication
+
+As of v0.2.0, FastLMI has built-in support for service-level auth, where the AI agent or LMI driver will send an
+authorization token you decide as a header with each request.
+
+Enabling authentication is easy! First, define the authentication scheme you wish to use - this will be a subclass of
+`LMIAuth`. For example, to provide service-level auth, you can define the `LMIServiceAuth` scheme:
+
+```python
+from fastlmi import Depends, FastLMI
+from fastlmi.auth import LMIServiceAuth
+
+auth = LMIServiceAuth(
+    access_tokens=["your_secret_token_here"],
+    verification_tokens={"openai": "verification_token_generated_in_the_ChatGPT_UI"}
+)
+```
+
+This auth scheme allows defining a set of allowed access tokens (if one wanted to, for example, have a different
+token for each plugin service). Then, when you define your app, all you have to do is add 2 parameters:
+
+```python
+app = FastLMI(..., auth=auth, dependencies=[Depends(auth)])
+```
+
+Tada! 🎉 Your LMI now tells consumers that it uses the `service_http` auth scheme, and will validate that each request
+to one of your defined routes provides a valid Bearer token.
+
+A complete example is in `examples/ai_plugin_auth.py`. You can read more about OpenAI's service-level
+auth [here](https://platform.openai.com/docs/plugins/authentication/service-level).
+
+### Route-Level Auth
+
+If you wanted to only require that certain routes use auth, you can also define the auth dependency on a route level:
+
+```diff
+- app = FastLMI(..., auth=auth, dependencies=[Depends(auth)])
++ app = FastLMI(..., auth=auth)
+...
+- @app.post("/hello")
++ @app.post("/hello", dependencies=[Depends(auth)])
+def hello():
+    ...
+```
+
 ## Read More
 
 Being based on FastAPI, FastLMI can take full advantage of its superpowers. Check out
 the [FastAPI documentation](https://fastapi.tiangolo.com/) for more!
 
 ## Todo
 
 - scopes
 - script to check for missing docs, over limits, etc
-- auth - for the moment, FastLMI does not support auth
 - logging
 - configure ecosystems
 
 <!--
 For developers:
 
 ## Build and Publish
```

