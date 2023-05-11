# Comparing `tmp/volttron-testing-0.4.0rc3.tar.gz` & `tmp/volttron_testing-0.4.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron-testing-0.4.0rc3.tar", max compression
+gzip compressed data, was "volttron_testing-0.4.0rc4.tar", max compression
```

## Comparing `volttron-testing-0.4.0rc3.tar` & `volttron_testing-0.4.0rc4.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0    11928 2023-05-07 03:03:05.646266 volttron-testing-0.4.0rc3/LICENSE
--rw-r--r--   0        0        0     3347 2023-05-07 03:03:05.646266 volttron-testing-0.4.0rc3/README.md
--rw-r--r--   0        0        0     1528 2023-05-07 03:05:32.388482 volttron-testing-0.4.0rc3/pyproject.toml
--rw-r--r--   0        0        0     1166 2023-05-07 03:03:05.650267 volttron-testing-0.4.0rc3/src/volttrontesting/__init__.py
--rw-r--r--   0        0        0     5184 2023-05-07 03:03:05.650267 volttron-testing-0.4.0rc3/src/volttrontesting/agent_additions.py
--rw-r--r--   0        0        0     9155 2023-05-07 03:03:05.650267 volttron-testing-0.4.0rc3/src/volttrontesting/certs_utils.py
--rw-r--r--   0        0        0      979 2023-05-07 03:03:05.650267 volttron-testing-0.4.0rc3/src/volttrontesting/client_mock.py
--rw-r--r--   0        0        0        0 2023-05-07 03:03:05.650267 volttron-testing-0.4.0rc3/src/volttrontesting/fixtures/__init__.py
--rw-r--r--   0        0        0     4696 2023-05-07 03:03:05.650267 volttron-testing-0.4.0rc3/src/volttrontesting/fixtures/cert_fixtures.py
--rw-r--r--   0        0        0     4686 2023-05-07 03:03:05.650267 volttron-testing-0.4.0rc3/src/volttrontesting/fixtures/docker_wrapper.py
--rw-r--r--   0        0        0     8103 2023-05-07 03:03:05.650267 volttron-testing-0.4.0rc3/src/volttrontesting/fixtures/rmq_test_setup.py
--rw-r--r--   0        0        0    29475 2023-05-07 03:03:05.650267 volttron-testing-0.4.0rc3/src/volttrontesting/fixtures/volttron_platform_fixtures.py
--rw-r--r--   0        0        0     3422 2023-05-07 03:03:05.650267 volttron-testing-0.4.0rc3/src/volttrontesting/memory_pubsub.py
--rw-r--r--   0        0        0    62220 2023-05-07 03:03:05.650267 volttron-testing-0.4.0rc3/src/volttrontesting/platformwrapper.py
--rw-r--r--   0        0        0    12618 2023-05-07 03:03:05.650267 volttron-testing-0.4.0rc3/src/volttrontesting/server_mock.py
--rw-r--r--   0        0        0     7115 2023-05-07 03:03:05.650267 volttron-testing-0.4.0rc3/src/volttrontesting/utils.py
--rw-r--r--   0        0        0     4424 1970-01-01 00:00:00.000000 volttron-testing-0.4.0rc3/setup.py
--rw-r--r--   0        0        0     4462 1970-01-01 00:00:00.000000 volttron-testing-0.4.0rc3/PKG-INFO
+-rw-r--r--   0        0        0    11928 2023-05-11 16:09:15.446037 volttron_testing-0.4.0rc4/LICENSE
+-rw-r--r--   0        0        0     3607 2023-05-11 16:09:15.446037 volttron_testing-0.4.0rc4/README.md
+-rw-r--r--   0        0        0     1780 2023-05-11 16:10:27.903689 volttron_testing-0.4.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     1166 2023-05-11 16:09:15.446037 volttron_testing-0.4.0rc4/src/volttrontesting/__init__.py
+-rw-r--r--   0        0        0     5184 2023-05-11 16:09:15.446037 volttron_testing-0.4.0rc4/src/volttrontesting/agent_additions.py
+-rw-r--r--   0        0        0     9155 2023-05-11 16:09:15.446037 volttron_testing-0.4.0rc4/src/volttrontesting/certs_utils.py
+-rw-r--r--   0        0        0      979 2023-05-11 16:09:15.446037 volttron_testing-0.4.0rc4/src/volttrontesting/client_mock.py
+-rw-r--r--   0        0        0        0 2023-05-11 16:09:15.446037 volttron_testing-0.4.0rc4/src/volttrontesting/fixtures/__init__.py
+-rw-r--r--   0        0        0     4696 2023-05-11 16:09:15.446037 volttron_testing-0.4.0rc4/src/volttrontesting/fixtures/cert_fixtures.py
+-rw-r--r--   0        0        0     4686 2023-05-11 16:09:15.446037 volttron_testing-0.4.0rc4/src/volttrontesting/fixtures/docker_wrapper.py
+-rw-r--r--   0        0        0     8103 2023-05-11 16:09:15.446037 volttron_testing-0.4.0rc4/src/volttrontesting/fixtures/rmq_test_setup.py
+-rw-r--r--   0        0        0    29475 2023-05-11 16:09:15.446037 volttron_testing-0.4.0rc4/src/volttrontesting/fixtures/volttron_platform_fixtures.py
+-rw-r--r--   0        0        0     3422 2023-05-11 16:09:15.446037 volttron_testing-0.4.0rc4/src/volttrontesting/memory_pubsub.py
+-rw-r--r--   0        0        0    62220 2023-05-11 16:09:15.446037 volttron_testing-0.4.0rc4/src/volttrontesting/platformwrapper.py
+-rw-r--r--   0        0        0    12618 2023-05-11 16:09:15.446037 volttron_testing-0.4.0rc4/src/volttrontesting/server_mock.py
+-rw-r--r--   0        0        0     7115 2023-05-11 16:09:15.446037 volttron_testing-0.4.0rc4/src/volttrontesting/utils.py
+-rw-r--r--   0        0        0     4773 1970-01-01 00:00:00.000000 volttron_testing-0.4.0rc4/PKG-INFO
```

### Comparing `volttron-testing-0.4.0rc3/LICENSE` & `volttron_testing-0.4.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron-testing-0.4.0rc3/README.md` & `volttron_testing-0.4.0rc4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # volttron-testing
 
+
+[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
 [![Run Pytests](https://github.com/eclipse-volttron/volttron-testing/actions/workflows/run-tests.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-testing/actions/workflows/run-tests.yml)
 [![pypi version](https://img.shields.io/pypi/v/volttron-testing.svg)](https://pypi.org/project/volttron-testing/)
 
 The volttron-testing library contains classes and utilities for interacting with a VOLTTRON instance.
 
 ## Prerequisites
 
-* Python >= 3.8
+* Python >= 3.10
 
 ## Installation
 
 Create a virtual environment
 
 ```shell 
 python -m venv env
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `volttron-testing-0.4.0rc3/src/volttrontesting/__init__.py` & `volttron_testing-0.4.0rc4/src/volttrontesting/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron-testing-0.4.0rc3/src/volttrontesting/agent_additions.py` & `volttron_testing-0.4.0rc4/src/volttrontesting/agent_additions.py`

 * *Files identical despite different names*

### Comparing `volttron-testing-0.4.0rc3/src/volttrontesting/certs_utils.py` & `volttron_testing-0.4.0rc4/src/volttrontesting/certs_utils.py`

 * *Files identical despite different names*

### Comparing `volttron-testing-0.4.0rc3/src/volttrontesting/client_mock.py` & `volttron_testing-0.4.0rc4/src/volttrontesting/client_mock.py`

 * *Files identical despite different names*

### Comparing `volttron-testing-0.4.0rc3/src/volttrontesting/fixtures/cert_fixtures.py` & `volttron_testing-0.4.0rc4/src/volttrontesting/fixtures/cert_fixtures.py`

 * *Files identical despite different names*

### Comparing `volttron-testing-0.4.0rc3/src/volttrontesting/fixtures/docker_wrapper.py` & `volttron_testing-0.4.0rc4/src/volttrontesting/fixtures/docker_wrapper.py`

 * *Files identical despite different names*

### Comparing `volttron-testing-0.4.0rc3/src/volttrontesting/fixtures/rmq_test_setup.py` & `volttron_testing-0.4.0rc4/src/volttrontesting/fixtures/rmq_test_setup.py`

 * *Files identical despite different names*

### Comparing `volttron-testing-0.4.0rc3/src/volttrontesting/fixtures/volttron_platform_fixtures.py` & `volttron_testing-0.4.0rc4/src/volttrontesting/fixtures/volttron_platform_fixtures.py`

 * *Files identical despite different names*

### Comparing `volttron-testing-0.4.0rc3/src/volttrontesting/memory_pubsub.py` & `volttron_testing-0.4.0rc4/src/volttrontesting/memory_pubsub.py`

 * *Files identical despite different names*

### Comparing `volttron-testing-0.4.0rc3/src/volttrontesting/platformwrapper.py` & `volttron_testing-0.4.0rc4/src/volttrontesting/platformwrapper.py`

 * *Files identical despite different names*

### Comparing `volttron-testing-0.4.0rc3/src/volttrontesting/server_mock.py` & `volttron_testing-0.4.0rc4/src/volttrontesting/server_mock.py`

 * *Files identical despite different names*

### Comparing `volttron-testing-0.4.0rc3/src/volttrontesting/utils.py` & `volttron_testing-0.4.0rc4/src/volttrontesting/utils.py`

 * *Files identical despite different names*

### Comparing `volttron-testing-0.4.0rc3/setup.py` & `volttron_testing-0.4.0rc4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,120 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: volttron-testing
+Version: 0.4.0rc4
+Summary: The volttron-testing library contains classes and utilities for interacting with a VOLTTRON instance.
+Home-page: https://github.com/eclipse-volttron/volttron-testing
+License: Apache-2.0
+Author: VOLTTRON Team
+Author-email: volttron@pnnl.gov
+Requires-Python: >=3.10,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Other Audience
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Dist: anypubsub (>=0.6,<0.7)
+Requires-Dist: docker (>=6.0.1,<7.0.0)
+Requires-Dist: grequests (>=0.6.0,<0.7.0)
+Requires-Dist: mock (>=4.0.3,<5.0.0)
+Requires-Dist: pytest (>=6.2.5,<7.0.0)
+Requires-Dist: volttron (>=10.0.3a9,<11.0)
+Project-URL: Repository, https://github.com/eclipse-volttron/volttron-testing
+Description-Content-Type: text/markdown
+
+# volttron-testing
+
+
+[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
+[![Run Pytests](https://github.com/eclipse-volttron/volttron-testing/actions/workflows/run-tests.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-testing/actions/workflows/run-tests.yml)
+[![pypi version](https://img.shields.io/pypi/v/volttron-testing.svg)](https://pypi.org/project/volttron-testing/)
+
+The volttron-testing library contains classes and utilities for interacting with a VOLTTRON instance.
+
+## Prerequisites
+
+* Python >= 3.10
+
+## Installation
+
+Create a virtual environment
+
+```shell 
+python -m venv env
+```
+
+Activate the environment
+
+```shell
+source env/bin/activate
+```
+
+Install volttron-testing
+
+```shell
+# Installs volttron and volttron-testing
+pip install volttron-testing
+```
+
+## Developing with TestServer
+
+The following code snippet shows how to utilize the TestServer's internal pubsub to be able to test
+with it outside of the volttron platform.
+
+```python
+def test_send_alert():
+    """ Test that an agent can send an alert through the pubsub message bus."""
+    
+    # Create an agent to run the test with
+    agent = Agent(identity='test-health')
+
+    # Create the server and connect the agent with the server
+    ts = TestServer()
+    ts.connect_agent(agent=agent)
+
+    # The health.send_alert should send a pubsub message through the message bus
+    agent.vip.health.send_alert("my_alert", Status.build(STATUS_BAD, "no context"))
+    
+    # We know that there should only be a single message sent through the bus and
+    # the specifications of the message to test against.
+    messages = ts.get_published_messages()
+    assert len(messages) == 1
+    headers = messages[0].headers
+    message = json.loads(messages[0].message)
+    assert headers['alert_key'] == 'my_alert'
+    assert message['context'] == 'no context'
+    assert message['status'] == 'BAD'
+
+```
+
+Reference the volttrontesting package from within your environment in order to build tests against the TestServer.
+
+## Development
+
+Please see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).
+
+Please see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)
+
+# Disclaimer Notice
+
+This material was prepared as an account of work sponsored by an agency of the
+United States Government.  Neither the United States Government nor the United
+States Department of Energy, nor Battelle, nor any of their employees, nor any
+jurisdiction or organization that has cooperated in the development of these
+materials, makes any warranty, express or implied, or assumes any legal
+liability or responsibility for the accuracy, completeness, or usefulness or any
+information, apparatus, product, software, or process disclosed, or represents
+that its use would not infringe privately owned rights.
+
+Reference herein to any specific commercial product, process, or service by
+trade name, trademark, manufacturer, or otherwise does not necessarily
+constitute or imply its endorsement, recommendation, or favoring by the United
+States Government or any agency thereof, or Battelle Memorial Institute. The
+views and opinions of authors expressed herein do not necessarily state or
+reflect those of the United States Government or any agency thereof.
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['volttrontesting', 'volttrontesting.fixtures']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['anypubsub>=0.6,<0.7',
- 'docker>=6.0.1,<7.0.0',
- 'grequests>=0.6.0,<0.7.0',
- 'mock>=4.0.3,<5.0.0',
- 'pytest>=6.2.5,<7.0.0',
- 'volttron>=10.0.3a9,<11.0']
-
-setup_kwargs = {
-    'name': 'volttron-testing',
-    'version': '0.4.0rc3',
-    'description': 'The volttron-testing library contains classes and utilities for interacting with a VOLTTRON instance.',
-    'long_description': '# volttron-testing\n\n[![Run Pytests](https://github.com/eclipse-volttron/volttron-testing/actions/workflows/run-tests.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-testing/actions/workflows/run-tests.yml)\n[![pypi version](https://img.shields.io/pypi/v/volttron-testing.svg)](https://pypi.org/project/volttron-testing/)\n\nThe volttron-testing library contains classes and utilities for interacting with a VOLTTRON instance.\n\n## Prerequisites\n\n* Python >= 3.8\n\n## Installation\n\nCreate a virtual environment\n\n```shell \npython -m venv env\n```\n\nActivate the environment\n\n```shell\nsource env/bin/activate\n```\n\nInstall volttron-testing\n\n```shell\n# Installs volttron and volttron-testing\npip install volttron-testing\n```\n\n## Developing with TestServer\n\nThe following code snippet shows how to utilize the TestServer\'s internal pubsub to be able to test\nwith it outside of the volttron platform.\n\n```python\ndef test_send_alert():\n    """ Test that an agent can send an alert through the pubsub message bus."""\n    \n    # Create an agent to run the test with\n    agent = Agent(identity=\'test-health\')\n\n    # Create the server and connect the agent with the server\n    ts = TestServer()\n    ts.connect_agent(agent=agent)\n\n    # The health.send_alert should send a pubsub message through the message bus\n    agent.vip.health.send_alert("my_alert", Status.build(STATUS_BAD, "no context"))\n    \n    # We know that there should only be a single message sent through the bus and\n    # the specifications of the message to test against.\n    messages = ts.get_published_messages()\n    assert len(messages) == 1\n    headers = messages[0].headers\n    message = json.loads(messages[0].message)\n    assert headers[\'alert_key\'] == \'my_alert\'\n    assert message[\'context\'] == \'no context\'\n    assert message[\'status\'] == \'BAD\'\n\n```\n\nReference the volttrontesting package from within your environment in order to build tests against the TestServer.\n\n## Development\n\nPlease see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).\n\nPlease see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)\n\n# Disclaimer Notice\n\nThis material was prepared as an account of work sponsored by an agency of the\nUnited States Government.  Neither the United States Government nor the United\nStates Department of Energy, nor Battelle, nor any of their employees, nor any\njurisdiction or organization that has cooperated in the development of these\nmaterials, makes any warranty, express or implied, or assumes any legal\nliability or responsibility for the accuracy, completeness, or usefulness or any\ninformation, apparatus, product, software, or process disclosed, or represents\nthat its use would not infringe privately owned rights.\n\nReference herein to any specific commercial product, process, or service by\ntrade name, trademark, manufacturer, or otherwise does not necessarily\nconstitute or imply its endorsement, recommendation, or favoring by the United\nStates Government or any agency thereof, or Battelle Memorial Institute. The\nviews and opinions of authors expressed herein do not necessarily state or\nreflect those of the United States Government or any agency thereof.\n',
-    'author': 'VOLTTRON Team',
-    'author_email': 'volttron@pnnl.gov',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/eclipse-volttron/volttron-testing',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

