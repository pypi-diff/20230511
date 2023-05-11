# Comparing `tmp/volttron_lib_base_driver-0.2.0rc0.tar.gz` & `tmp/volttron_lib_base_driver-0.2.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_lib_base_driver-0.2.0rc0.tar", max compression
+gzip compressed data, was "volttron_lib_base_driver-0.2.1rc0.tar", max compression
```

## Comparing `volttron_lib_base_driver-0.2.0rc0.tar` & `volttron_lib_base_driver-0.2.1rc0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      897 2022-11-29 22:34:26.184384 volttron_lib_base_driver-0.2.0rc0/LICENSE.md
--rw-r--r--   0        0        0     2759 2022-11-29 22:34:26.184384 volttron_lib_base_driver-0.2.0rc0/README.md
--rw-r--r--   0        0        0     2007 2022-11-29 22:34:26.184384 volttron_lib_base_driver-0.2.0rc0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-29 22:34:26.184384 volttron_lib_base_driver-0.2.0rc0/src/volttron/driver/base/__init__.py
--rw-r--r--   0        0        0    16976 2022-11-29 22:34:26.184384 volttron_lib_base_driver-0.2.0rc0/src/volttron/driver/base/driver.py
--rw-r--r--   0        0        0     1019 2022-11-29 22:34:26.184384 volttron_lib_base_driver-0.2.0rc0/src/volttron/driver/base/driver_exceptions.py
--rw-r--r--   0        0        0     2169 2022-11-29 22:34:26.184384 volttron_lib_base_driver-0.2.0rc0/src/volttron/driver/base/driver_locks.py
--rw-r--r--   0        0        0    22949 2022-11-29 22:34:26.184384 volttron_lib_base_driver-0.2.0rc0/src/volttron/driver/base/interfaces.py
--rw-r--r--   0        0        0     3690 1970-01-01 00:00:00.000000 volttron_lib_base_driver-0.2.0rc0/setup.py
--rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 volttron_lib_base_driver-0.2.0rc0/PKG-INFO
+-rw-r--r--   0        0        0    11927 2023-05-11 16:41:41.278327 volttron_lib_base_driver-0.2.1rc0/LICENSE
+-rw-r--r--   0        0        0     3020 2023-05-11 16:41:41.282327 volttron_lib_base_driver-0.2.1rc0/README.md
+-rw-r--r--   0        0        0     1993 2023-05-11 16:42:44.799490 volttron_lib_base_driver-0.2.1rc0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-11 16:41:41.282327 volttron_lib_base_driver-0.2.1rc0/src/volttron/driver/base/__init__.py
+-rw-r--r--   0        0        0    16976 2023-05-11 16:41:41.282327 volttron_lib_base_driver-0.2.1rc0/src/volttron/driver/base/driver.py
+-rw-r--r--   0        0        0     1019 2023-05-11 16:41:41.282327 volttron_lib_base_driver-0.2.1rc0/src/volttron/driver/base/driver_exceptions.py
+-rw-r--r--   0        0        0     2169 2023-05-11 16:41:41.282327 volttron_lib_base_driver-0.2.1rc0/src/volttron/driver/base/driver_locks.py
+-rw-r--r--   0        0        0    22949 2023-05-11 16:41:41.282327 volttron_lib_base_driver-0.2.1rc0/src/volttron/driver/base/interfaces.py
+-rw-r--r--   0        0        0     4006 1970-01-01 00:00:00.000000 volttron_lib_base_driver-0.2.1rc0/PKG-INFO
```

### Comparing `volttron_lib_base_driver-0.2.0rc0/LICENSE.md` & `volttron_lib_base_driver-0.2.1rc0/src/volttron/driver/base/driver_exceptions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,30 @@
-Copyright 2022, Battelle Memorial Institute.
+# -*- coding: utf-8 -*- {{{
+# ===----------------------------------------------------------------------===
+#
+#                 Installable Component of Eclipse VOLTTRON
+#
+# ===----------------------------------------------------------------------===
+#
+# Copyright 2022 Battelle Memorial Institute
+#
+# Licensed under the Apache License, Version 2.0 (the "License"); you may not
+# use this file except in compliance with the License. You may obtain a copy
+# of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+#
+# ===----------------------------------------------------------------------===
+# }}}
 
-Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at
+class DriverError(Exception):
+    pass
 
-http://www.apache.org/licenses/LICENSE-2.0
 
-The patent license grant shall only be applicable to the following patent and patent application (Battelle IPID 17008-E), as assigned to the Battelle Memorial Institute, as used in conjunction with this Work:  US Patent No. 9,094,385, issued 7/28/15  USPTO Patent App. No. 14/746,577, filed 6/22/15, published as US 2016-0006569.
-
-Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
+class DriverConfigError(DriverError):
+    pass
```

### Comparing `volttron_lib_base_driver-0.2.0rc0/README.md` & `volttron_lib_base_driver-0.2.1rc0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 # volttron-lib-base-driver
 
+[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
 ![Passing?](https://github.com/eclipse-volttron/volttron-lib-base-driver/actions/workflows/run-tests.yml/badge.svg)
 [![pypi version](https://img.shields.io/pypi/v/volttron-lib-base-driver.svg)](https://pypi.org/project/volttron-lib-base-driver/)
 
 
-# Prerequisites
+## Prerequisites
 
-* Python 3.8
+* Python 3.10
 
-## Python
+### Python
 
 <details>
-<summary>To install Python 3.8, we recommend using <a href="https://github.com/pyenv/pyenv"><code>pyenv</code></a>.</summary>
+<summary>To install Python 3.10, we recommend using <a href="https://github.com/pyenv/pyenv"><code>pyenv</code></a>.</summary>
 
 ```bash
 # install pyenv
 git clone https://github.com/pyenv/pyenv ~/.pyenv
 
 # setup pyenv (you should also put these three lines in .bashrc or similar)
 export PATH="${HOME}/.pyenv/bin:${PATH}"
 export PYENV_ROOT="${HOME}/.pyenv"
 eval "$(pyenv init -)"
 
 # install Python 3.8
-pyenv install 3.8.10
+pyenv install 3.10
 
 # make it available globally
-pyenv global system 3.8.10
+pyenv global system 3.10
 ```
 </details>
 
-# Installation
+## Installation
 
 Create and activate a virtual environment.
 
 ```shell
 python -m venv env
 source env/bin/activate
 ```
@@ -56,22 +59,22 @@
 
 Or you can install the local version of this library from this repo:
 
 ```shell
 pip install -e .
 ```
 
-# Development
+## Development
 
 Please see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).
 
 Please see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)
 
 
-# Disclaimer Notice
+## Disclaimer Notice
 
 This material was prepared as an account of work sponsored by an agency of the
 United States Government.  Neither the United States Government nor the United
 States Department of Energy, nor Battelle, nor any of their employees, nor any
 jurisdiction or organization that has cooperated in the development of these
 materials, makes any warranty, express or implied, or assumes any legal
 liability or responsibility for the accuracy, completeness, or usefulness or any
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,33 +1,36 @@
-# volttron-lib-base-driver ![Passing?](https://github.com/eclipse-volttron/
-volttron-lib-base-driver/actions/workflows/run-tests.yml/badge.svg) [![pypi
-version](https://img.shields.io/pypi/v/volttron-lib-base-driver.svg)](https://
-pypi.org/project/volttron-lib-base-driver/) # Prerequisites * Python 3.8 ##
-Python  To install Python 3.8, we recommend using pyenv. ```bash # install
-pyenv git clone https://github.com/pyenv/pyenv ~/.pyenv # setup pyenv (you
-should also put these three lines in .bashrc or similar) export PATH="$
-{HOME}/.pyenv/bin:${PATH}" export PYENV_ROOT="${HOME}/.pyenv" eval "$(pyenv
-init -)" # install Python 3.8 pyenv install 3.8.10 # make it available globally
-pyenv global system 3.8.10 ```  # Installation Create and activate a virtual
-environment. ```shell python -m venv env source env/bin/activate ``` Install
-volttron and start the platform. ```shell pip install volttron # Start platform
-with output going to volttron.log volttron -vv -l volttron.log & ``` Install
-the library. You have two options. You can install this library using the
-version on PyPi: ```shell pip install volttron-lib-base-driver ``` Or you can
-install the local version of this library from this repo: ```shell pip install
--e . ``` # Development Please see the following for contributing guidelines
-[contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/
-CONTRIBUTING.md). Please see the following helpful guide about [developing
-modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/
-blob/develop/DEVELOPING_ON_MODULAR.md) # Disclaimer Notice This material was
-prepared as an account of work sponsored by an agency of the United States
-Government. Neither the United States Government nor the United States
-Department of Energy, nor Battelle, nor any of their employees, nor any
-jurisdiction or organization that has cooperated in the development of these
-materials, makes any warranty, express or implied, or assumes any legal
+# volttron-lib-base-driver [![Eclipse VOLTTRONâ¢](https://img.shields.io/
+badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/
+) ![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg) ![Python
+3.11](https://img.shields.io/badge/python-3.11-blue.svg) ![Passing?](https://
+github.com/eclipse-volttron/volttron-lib-base-driver/actions/workflows/run-
+tests.yml/badge.svg) [![pypi version](https://img.shields.io/pypi/v/volttron-
+lib-base-driver.svg)](https://pypi.org/project/volttron-lib-base-driver/) ##
+Prerequisites * Python 3.10 ### Python  To install Python 3.10, we recommend
+using pyenv. ```bash # install pyenv git clone https://github.com/pyenv/pyenv
+~/.pyenv # setup pyenv (you should also put these three lines in .bashrc or
+similar) export PATH="${HOME}/.pyenv/bin:${PATH}" export PYENV_ROOT="$
+{HOME}/.pyenv" eval "$(pyenv init -)" # install Python 3.8 pyenv install 3.10 #
+make it available globally pyenv global system 3.10 ```  ## Installation Create
+and activate a virtual environment. ```shell python -m venv env source env/bin/
+activate ``` Install volttron and start the platform. ```shell pip install
+volttron # Start platform with output going to volttron.log volttron -vv -
+l volttron.log & ``` Install the library. You have two options. You can install
+this library using the version on PyPi: ```shell pip install volttron-lib-base-
+driver ``` Or you can install the local version of this library from this repo:
+```shell pip install -e . ``` ## Development Please see the following for
+contributing guidelines [contributing](https://github.com/eclipse-volttron/
+volttron-core/blob/develop/CONTRIBUTING.md). Please see the following helpful
+guide about [developing modular VOLTTRON agents](https://github.com/eclipse-
+volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md) ## Disclaimer
+Notice This material was prepared as an account of work sponsored by an agency
+of the United States Government. Neither the United States Government nor the
+United States Department of Energy, nor Battelle, nor any of their employees,
+nor any jurisdiction or organization that has cooperated in the development of
+these materials, makes any warranty, express or implied, or assumes any legal
 liability or responsibility for the accuracy, completeness, or usefulness or
 any information, apparatus, product, software, or process disclosed, or
 represents that its use would not infringe privately owned rights. Reference
 herein to any specific commercial product, process, or service by trade name,
 trademark, manufacturer, or otherwise does not necessarily constitute or imply
 its endorsement, recommendation, or favoring by the United States Government or
 any agency thereof, or Battelle Memorial Institute. The views and opinions of
```

### Comparing `volttron_lib_base_driver-0.2.0rc0/pyproject.toml` & `volttron_lib_base_driver-0.2.1rc0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["poetry-core>=1.2.2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
-python_version = 3.8
+python_version = 3.10
 show_error_context = true
 pretty = true
 show_column_numbers = true
 warn_return_any = true
 warn_unused_configs = true
 show_error_codes = true
 exclude = ['docs/']
@@ -28,15 +28,15 @@
 ignore_missing_imports = true
 
 [tool.mypy-volttron]
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "volttron-lib-base-driver"
-version = "0.2.0-rc"
+version = "0.2.1rc0"
 description = "Volttron Driver libraries used to support development within the Volttron Driver Framework."
 authors = ["Mark Bonicillo <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/volttron-lib-base-driver"
 homepage = "https://github.com/eclipse-volttron/volttron-lib-base-driver"
 keywords = []
@@ -47,16 +47,16 @@
     "Intended Audience :: Information Technology",
     "Intended Audience :: Developers",
     "Intended Audience :: Other Audience",
     "License :: OSI Approved :: Apache Software License"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
-volttron = ">=10.0.2rc0,<11.0"
+python = "^3.10"
+volttron = "^10.0.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.2.5"
 mock = "^4.0.3"
 pre-commit = "^2.17.0"
 yapf = "^0.32.0"
 toml = "^0.10.2"
```

### Comparing `volttron_lib_base_driver-0.2.0rc0/src/volttron/driver/base/driver.py` & `volttron_lib_base_driver-0.2.1rc0/src/volttron/driver/base/driver.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_driver-0.2.0rc0/src/volttron/driver/base/driver_locks.py` & `volttron_lib_base_driver-0.2.1rc0/src/volttron/driver/base/driver_locks.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_driver-0.2.0rc0/src/volttron/driver/base/interfaces.py` & `volttron_lib_base_driver-0.2.1rc0/src/volttron/driver/base/interfaces.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_driver-0.2.0rc0/setup.py` & `volttron_lib_base_driver-0.2.1rc0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,112 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: volttron-lib-base-driver
+Version: 0.2.1rc0
+Summary: Volttron Driver libraries used to support development within the Volttron Driver Framework.
+Home-page: https://github.com/eclipse-volttron/volttron-lib-base-driver
+License: Apache-2.0
+Author: Mark Bonicillo
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
+Requires-Dist: volttron (>=10.0.3,<11.0.0)
+Project-URL: Repository, https://github.com/eclipse-volttron/volttron-lib-base-driver
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# volttron-lib-base-driver
 
-packages = \
-['volttron', 'volttron.driver.base']
+[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
+![Passing?](https://github.com/eclipse-volttron/volttron-lib-base-driver/actions/workflows/run-tests.yml/badge.svg)
+[![pypi version](https://img.shields.io/pypi/v/volttron-lib-base-driver.svg)](https://pypi.org/project/volttron-lib-base-driver/)
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['volttron>=10.0.2rc0,<11.0']
-
-setup_kwargs = {
-    'name': 'volttron-lib-base-driver',
-    'version': '0.2.0rc0',
-    'description': 'Volttron Driver libraries used to support development within the Volttron Driver Framework.',
-    'long_description': '# volttron-lib-base-driver\n\n![Passing?](https://github.com/eclipse-volttron/volttron-lib-base-driver/actions/workflows/run-tests.yml/badge.svg)\n[![pypi version](https://img.shields.io/pypi/v/volttron-lib-base-driver.svg)](https://pypi.org/project/volttron-lib-base-driver/)\n\n\n# Prerequisites\n\n* Python 3.8\n\n## Python\n\n<details>\n<summary>To install Python 3.8, we recommend using <a href="https://github.com/pyenv/pyenv"><code>pyenv</code></a>.</summary>\n\n```bash\n# install pyenv\ngit clone https://github.com/pyenv/pyenv ~/.pyenv\n\n# setup pyenv (you should also put these three lines in .bashrc or similar)\nexport PATH="${HOME}/.pyenv/bin:${PATH}"\nexport PYENV_ROOT="${HOME}/.pyenv"\neval "$(pyenv init -)"\n\n# install Python 3.8\npyenv install 3.8.10\n\n# make it available globally\npyenv global system 3.8.10\n```\n</details>\n\n# Installation\n\nCreate and activate a virtual environment.\n\n```shell\npython -m venv env\nsource env/bin/activate\n```\n\nInstall volttron and start the platform.\n\n```shell\npip install volttron\n\n# Start platform with output going to volttron.log\nvolttron -vv -l volttron.log &\n```\n\nInstall the library. You have two options. You can install this library using the version on PyPi:\n\n```shell\npip install volttron-lib-base-driver\n```\n\nOr you can install the local version of this library from this repo:\n\n```shell\npip install -e .\n```\n\n# Development\n\nPlease see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).\n\nPlease see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)\n\n\n# Disclaimer Notice\n\nThis material was prepared as an account of work sponsored by an agency of the\nUnited States Government.  Neither the United States Government nor the United\nStates Department of Energy, nor Battelle, nor any of their employees, nor any\njurisdiction or organization that has cooperated in the development of these\nmaterials, makes any warranty, express or implied, or assumes any legal\nliability or responsibility for the accuracy, completeness, or usefulness or any\ninformation, apparatus, product, software, or process disclosed, or represents\nthat its use would not infringe privately owned rights.\n\nReference herein to any specific commercial product, process, or service by\ntrade name, trademark, manufacturer, or otherwise does not necessarily\nconstitute or imply its endorsement, recommendation, or favoring by the United\nStates Government or any agency thereof, or Battelle Memorial Institute. The\nviews and opinions of authors expressed herein do not necessarily state or\nreflect those of the United States Government or any agency thereof.\n',
-    'author': 'Mark Bonicillo',
-    'author_email': 'volttron@pnnl.gov',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/eclipse-volttron/volttron-lib-base-driver',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
 
+## Prerequisites
+
+* Python 3.10
+
+### Python
+
+<details>
+<summary>To install Python 3.10, we recommend using <a href="https://github.com/pyenv/pyenv"><code>pyenv</code></a>.</summary>
+
+```bash
+# install pyenv
+git clone https://github.com/pyenv/pyenv ~/.pyenv
+
+# setup pyenv (you should also put these three lines in .bashrc or similar)
+export PATH="${HOME}/.pyenv/bin:${PATH}"
+export PYENV_ROOT="${HOME}/.pyenv"
+eval "$(pyenv init -)"
+
+# install Python 3.8
+pyenv install 3.10
+
+# make it available globally
+pyenv global system 3.10
+```
+</details>
+
+## Installation
+
+Create and activate a virtual environment.
+
+```shell
+python -m venv env
+source env/bin/activate
+```
+
+Install volttron and start the platform.
+
+```shell
+pip install volttron
+
+# Start platform with output going to volttron.log
+volttron -vv -l volttron.log &
+```
+
+Install the library. You have two options. You can install this library using the version on PyPi:
+
+```shell
+pip install volttron-lib-base-driver
+```
+
+Or you can install the local version of this library from this repo:
+
+```shell
+pip install -e .
+```
+
+## Development
+
+Please see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).
+
+Please see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)
+
+
+## Disclaimer Notice
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
 
-setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,48 +1,51 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['volttron', 'volttron.driver.base'] package_data = \ {'':
-['*']} install_requires = \ ['volttron>=10.0.2rc0,<11.0'] setup_kwargs =
-{ 'name': 'volttron-lib-base-driver', 'version': '0.2.0rc0', 'description':
-'Volttron Driver libraries used to support development within the Volttron
-Driver Framework.', 'long_description': '# volttron-lib-base-driver\n\n!
-[Passing?](https://github.com/eclipse-volttron/volttron-lib-base-driver/
-actions/workflows/run-tests.yml/badge.svg)\n[![pypi version](https://
-img.shields.io/pypi/v/volttron-lib-base-driver.svg)](https://pypi.org/project/
-volttron-lib-base-driver/)\n\n\n# Prerequisites\n\n* Python 3.8\n\n##
-Python\n\n\nTo install Python 3.8, we recommend using pyenv.\n\n```bash\n#
-install pyenv\ngit clone https://github.com/pyenv/pyenv ~/.pyenv\n\n# setup
-pyenv (you should also put these three lines in .bashrc or similar)\nexport
-PATH="${HOME}/.pyenv/bin:${PATH}"\nexport PYENV_ROOT="${HOME}/.pyenv"\neval "$
-(pyenv init -)"\n\n# install Python 3.8\npyenv install 3.8.10\n\n# make it
-available globally\npyenv global system 3.8.10\n```\n\n\n#
-Installation\n\nCreate and activate a virtual environment.\n\n```shell\npython
--m venv env\nsource env/bin/activate\n```\n\nInstall volttron and start the
-platform.\n\n```shell\npip install volttron\n\n# Start platform with output
-going to volttron.log\nvolttron -vv -l volttron.log &\n```\n\nInstall the
-library. You have two options. You can install this library using the version
-on PyPi:\n\n```shell\npip install volttron-lib-base-driver\n```\n\nOr you can
-install the local version of this library from this repo:\n\n```shell\npip
-install -e .\n```\n\n# Development\n\nPlease see the following for contributing
-guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/
-blob/develop/CONTRIBUTING.md).\n\nPlease see the following helpful guide about
-[developing modular VOLTTRON agents](https://github.com/eclipse-volttron/
-volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)\n\n\n# Disclaimer
-Notice\n\nThis material was prepared as an account of work sponsored by an
-agency of the\nUnited States Government. Neither the United States Government
-nor the United\nStates Department of Energy, nor Battelle, nor any of their
-employees, nor any\njurisdiction or organization that has cooperated in the
-development of these\nmaterials, makes any warranty, express or implied, or
-assumes any legal\nliability or responsibility for the accuracy, completeness,
-or usefulness or any\ninformation, apparatus, product, software, or process
-disclosed, or represents\nthat its use would not infringe privately owned
-rights.\n\nReference herein to any specific commercial product, process, or
-service by\ntrade name, trademark, manufacturer, or otherwise does not
-necessarily\nconstitute or imply its endorsement, recommendation, or favoring
-by the United\nStates Government or any agency thereof, or Battelle Memorial
-Institute. The\nviews and opinions of authors expressed herein do not
-necessarily state or\nreflect those of the United States Government or any
-agency thereof.\n', 'author': 'Mark Bonicillo', 'author_email':
-'volttron@pnnl.gov', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
-'https://github.com/eclipse-volttron/volttron-lib-base-driver', 'package_dir':
-package_dir, 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.8,<4.0', } setup
-(**setup_kwargs)
+Metadata-Version: 2.1 Name: volttron-lib-base-driver Version: 0.2.1rc0 Summary:
+Volttron Driver libraries used to support development within the Volttron
+Driver Framework. Home-page: https://github.com/eclipse-volttron/volttron-lib-
+base-driver License: Apache-2.0 Author: Mark Bonicillo Author-email:
+volttron@pnnl.gov Requires-Python: >=3.10,<4.0 Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Information Technology Classifier:
+Intended Audience :: Other Audience Classifier: Intended Audience :: Science/
+Research Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only Requires-Dist: volttron
+(>=10.0.3,<11.0.0) Project-URL: Repository, https://github.com/eclipse-
+volttron/volttron-lib-base-driver Description-Content-Type: text/markdown #
+volttron-lib-base-driver [![Eclipse VOLTTRONâ¢](https://img.shields.io/badge/
+Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/) !
+[Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg) ![Python 3.11]
+(https://img.shields.io/badge/python-3.11-blue.svg) ![Passing?](https://
+github.com/eclipse-volttron/volttron-lib-base-driver/actions/workflows/run-
+tests.yml/badge.svg) [![pypi version](https://img.shields.io/pypi/v/volttron-
+lib-base-driver.svg)](https://pypi.org/project/volttron-lib-base-driver/) ##
+Prerequisites * Python 3.10 ### Python  To install Python 3.10, we recommend
+using pyenv. ```bash # install pyenv git clone https://github.com/pyenv/pyenv
+~/.pyenv # setup pyenv (you should also put these three lines in .bashrc or
+similar) export PATH="${HOME}/.pyenv/bin:${PATH}" export PYENV_ROOT="$
+{HOME}/.pyenv" eval "$(pyenv init -)" # install Python 3.8 pyenv install 3.10 #
+make it available globally pyenv global system 3.10 ```  ## Installation Create
+and activate a virtual environment. ```shell python -m venv env source env/bin/
+activate ``` Install volttron and start the platform. ```shell pip install
+volttron # Start platform with output going to volttron.log volttron -vv -
+l volttron.log & ``` Install the library. You have two options. You can install
+this library using the version on PyPi: ```shell pip install volttron-lib-base-
+driver ``` Or you can install the local version of this library from this repo:
+```shell pip install -e . ``` ## Development Please see the following for
+contributing guidelines [contributing](https://github.com/eclipse-volttron/
+volttron-core/blob/develop/CONTRIBUTING.md). Please see the following helpful
+guide about [developing modular VOLTTRON agents](https://github.com/eclipse-
+volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md) ## Disclaimer
+Notice This material was prepared as an account of work sponsored by an agency
+of the United States Government. Neither the United States Government nor the
+United States Department of Energy, nor Battelle, nor any of their employees,
+nor any jurisdiction or organization that has cooperated in the development of
+these materials, makes any warranty, express or implied, or assumes any legal
+liability or responsibility for the accuracy, completeness, or usefulness or
+any information, apparatus, product, software, or process disclosed, or
+represents that its use would not infringe privately owned rights. Reference
+herein to any specific commercial product, process, or service by trade name,
+trademark, manufacturer, or otherwise does not necessarily constitute or imply
+its endorsement, recommendation, or favoring by the United States Government or
+any agency thereof, or Battelle Memorial Institute. The views and opinions of
+authors expressed herein do not necessarily state or reflect those of the
+United States Government or any agency thereof.
```

