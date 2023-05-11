# Comparing `tmp/volttron_lib_dnp3_driver-0.1.1a2.tar.gz` & `tmp/volttron_lib_dnp3_driver-0.1.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_lib_dnp3_driver-0.1.1a2.tar", max compression
+gzip compressed data, was "volttron_lib_dnp3_driver-0.1.1a3.tar", max compression
```

## Comparing `volttron_lib_dnp3_driver-0.1.1a2.tar` & `volttron_lib_dnp3_driver-0.1.1a3.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    11928 2023-04-28 17:37:22.395838 volttron_lib_dnp3_driver-0.1.1a2/LICENSE
--rw-r--r--   0        0        0    20538 2023-04-28 17:37:22.395838 volttron_lib_dnp3_driver-0.1.1a2/README.md
--rw-r--r--   0        0        0     1584 2023-04-28 17:39:27.532901 volttron_lib_dnp3_driver-0.1.1a2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-28 17:37:22.395838 volttron_lib_dnp3_driver-0.1.1a2/src/volttron/driver/interfaces/dnp3/__init__.py
--rw-r--r--   0        0        0     9189 2023-04-28 17:37:22.395838 volttron_lib_dnp3_driver-0.1.1a2/src/volttron/driver/interfaces/dnp3/dnp3.py
--rw-r--r--   0        0        0    22231 1970-01-01 00:00:00.000000 volttron_lib_dnp3_driver-0.1.1a2/setup.py
--rw-r--r--   0        0        0    21656 1970-01-01 00:00:00.000000 volttron_lib_dnp3_driver-0.1.1a2/PKG-INFO
+-rw-r--r--   0        0        0    11928 2023-05-10 20:42:47.741844 volttron_lib_dnp3_driver-0.1.1a3/LICENSE
+-rw-r--r--   0        0        0    21060 2023-05-10 20:42:47.741844 volttron_lib_dnp3_driver-0.1.1a3/README.md
+-rw-r--r--   0        0        0     1579 2023-05-10 20:43:55.010271 volttron_lib_dnp3_driver-0.1.1a3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-10 20:42:47.741844 volttron_lib_dnp3_driver-0.1.1a3/src/volttron/driver/interfaces/dnp3/__init__.py
+-rw-r--r--   0        0        0     9189 2023-05-10 20:42:47.741844 volttron_lib_dnp3_driver-0.1.1a3/src/volttron/driver/interfaces/dnp3/dnp3.py
+-rw-r--r--   0        0        0    22079 1970-01-01 00:00:00.000000 volttron_lib_dnp3_driver-0.1.1a3/PKG-INFO
```

### Comparing `volttron_lib_dnp3_driver-0.1.1a2/LICENSE` & `volttron_lib_dnp3_driver-0.1.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_lib_dnp3_driver-0.1.1a2/README.md` & `volttron_lib_dnp3_driver-0.1.1a3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # volttron-lib-dnp3-driver
 
-[//]: # (TODO: get the badges)
+[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
+[![Pytests](https://github.com/eclipse-volttron/volttron-lib-dnp3-driver/actions/workflows/run-tests.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-lib-dnp3-driver/actions/workflows/run-tests.yml)
+[![pypi version](https://img.shields.io/pypi/v/volttron-lib-dnp3-driver.svg)](https://pypi.org/project/volttron-lib-dnp3-driver/)
+
 
 Distributed Network Protocol (DNP
 or [DNP3](https://en.wikipedia.org/wiki/DNP3))
 has achieved a large-scale acceptance since its introduction in 1993. This
 protocol is an immediately deployable solution for monitoring remote sites because it was developed for communication of
 critical infrastructure status, allowing for reliable remote control.
 
@@ -17,15 +22,15 @@
 Note that the DNP3-Driver requires a DNP3 outstation instance to properly function. e.g., polling data, setting point
 values, etc. The [dnp3-python](https://github.com/VOLTTRON/dnp3-python) can provide the essential outstation
 functionality, and as part of the DNP3-Driver dependency, it is immediately available after the DNP3-Driver is
 installed.
 
 # Prerequisites
 
-* Python 3 (tested with Python3.8, Python3.9, Python3.10)
+* Python 3.10
 
 ## Python
 
 <details>
 <summary>To install specific Python version (e.g., Python 3.8), we recommend using <a href="https://github.com/pyenv/pyenv"><code>pyenv</code></a>.</summary>
 
 ```shell
@@ -33,19 +38,19 @@
 git clone https://github.com/pyenv/pyenv ~/.pyenv
 
 # setup pyenv (you should also put these three lines in .bashrc or similar)
 export PATH="${HOME}/.pyenv/bin:${PATH}"
 export PYENV_ROOT="${HOME}/.pyenv"
 eval "$(pyenv init -)"
 
-# install Python 3.8
-pyenv install 3.8.10
+# install Python 3.10
+pyenv install 3.10
 
 # make it available globally
-pyenv global system 3.8.10
+pyenv global system 3.10
 ```
 
 </details>
 
 # Quick Start
 
 The following recipe walks through the steps to install and configure a DNP3 Driver. Note that it uses default setup to
```

#### html2text {}

```diff
@@ -1,46 +1,53 @@
-# volttron-lib-dnp3-driver [//]: # (TODO: get the badges) Distributed Network
-Protocol (DNP or [DNP3](https://en.wikipedia.org/wiki/DNP3)) has achieved a
-large-scale acceptance since its introduction in 1993. This protocol is an
-immediately deployable solution for monitoring remote sites because it was
-developed for communication of critical infrastructure status, allowing for
-reliable remote control. DNP3 is typically used between centrally located
-masters and distributed remotes. The master provides the interface between the
-human network manager and the monitoring system. The remote (RTUs and
-intelligent electronic devices) provides the interface between the master and
-the physical device(s) being monitored and/or controlled. The DNP3-Driver is a
-wrapper on the DNP3 master following the [VOLTTRON driver framework](https://
-volttron.readthedocs.io/en/develop/agent-framework/driver-framework/drivers-
-overview.html#driver-framework). Note that the DNP3-Driver requires a DNP3
-outstation instance to properly function. e.g., polling data, setting point
-values, etc. The [dnp3-python](https://github.com/VOLTTRON/dnp3-python) can
-provide the essential outstation functionality, and as part of the DNP3-Driver
-dependency, it is immediately available after the DNP3-Driver is installed. #
-Prerequisites * Python 3 (tested with Python3.8, Python3.9, Python3.10) ##
-Python  To install specific Python version (e.g., Python 3.8), we recommend
-using pyenv. ```shell # install pyenv git clone https://github.com/pyenv/pyenv
-~/.pyenv # setup pyenv (you should also put these three lines in .bashrc or
-similar) export PATH="${HOME}/.pyenv/bin:${PATH}" export PYENV_ROOT="$
-{HOME}/.pyenv" eval "$(pyenv init -)" # install Python 3.8 pyenv install 3.8.10
-# make it available globally pyenv global system 3.8.10 ```  # Quick Start The
-following recipe walks through the steps to install and configure a DNP3
-Driver. Note that it uses default setup to work out-of-the-box. Please feel
-free to refer to related documentations for details. 1. Create and activate a
-virtual environment. It is recommended to use a virtual environment for
-installing volttron. ```shell python -m venv env source env/bin/activate pip
-install volttron ``` 1. Install volttron and start the platform. > **Note**: >
-According to [volttron-core#readme](https://github.com/eclipse-volttron/
-volttron-core#readme), setup VOLTTRON_HOME > environment variable is mandatory:
-> ... if you have/had in the past, a monolithic VOLTTRON version that used the
-default VOLTTRON_HOME > $HOME/.volttron. This modular version of VOLTTRON
-cannot work with volttron_home used by monolithic version of > VOLTTRON(version
-8.3 or earlier) ```shell # Setup enviornment variable export VOLTTRON_HOME=/
-path/to/volttron_home/dir # Start platform with output going to volttron.log
-volttron -vv -l volttron.log & ``` 1. Install the volttron platform driver:
-Note: for reproducibility, this demo will install platform driver with `vip-
+# volttron-lib-dnp3-driver [![Eclipse VOLTTRONâ¢](https://img.shields.io/
+badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/
+) ![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg) ![Python
+3.11](https://img.shields.io/badge/python-3.11-blue.svg) [![Pytests](https://
+github.com/eclipse-volttron/volttron-lib-dnp3-driver/actions/workflows/run-
+tests.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-lib-dnp3-
+driver/actions/workflows/run-tests.yml) [![pypi version](https://
+img.shields.io/pypi/v/volttron-lib-dnp3-driver.svg)](https://pypi.org/project/
+volttron-lib-dnp3-driver/) Distributed Network Protocol (DNP or [DNP3](https://
+en.wikipedia.org/wiki/DNP3)) has achieved a large-scale acceptance since its
+introduction in 1993. This protocol is an immediately deployable solution for
+monitoring remote sites because it was developed for communication of critical
+infrastructure status, allowing for reliable remote control. DNP3 is typically
+used between centrally located masters and distributed remotes. The master
+provides the interface between the human network manager and the monitoring
+system. The remote (RTUs and intelligent electronic devices) provides the
+interface between the master and the physical device(s) being monitored and/or
+controlled. The DNP3-Driver is a wrapper on the DNP3 master following the
+[VOLTTRON driver framework](https://volttron.readthedocs.io/en/develop/agent-
+framework/driver-framework/drivers-overview.html#driver-framework). Note that
+the DNP3-Driver requires a DNP3 outstation instance to properly function. e.g.,
+polling data, setting point values, etc. The [dnp3-python](https://github.com/
+VOLTTRON/dnp3-python) can provide the essential outstation functionality, and
+as part of the DNP3-Driver dependency, it is immediately available after the
+DNP3-Driver is installed. # Prerequisites * Python 3.10 ## Python  To install
+specific Python version (e.g., Python 3.8), we recommend using pyenv. ```shell
+# install pyenv git clone https://github.com/pyenv/pyenv ~/.pyenv # setup pyenv
+(you should also put these three lines in .bashrc or similar) export PATH="$
+{HOME}/.pyenv/bin:${PATH}" export PYENV_ROOT="${HOME}/.pyenv" eval "$(pyenv
+init -)" # install Python 3.10 pyenv install 3.10 # make it available globally
+pyenv global system 3.10 ```  # Quick Start The following recipe walks through
+the steps to install and configure a DNP3 Driver. Note that it uses default
+setup to work out-of-the-box. Please feel free to refer to related
+documentations for details. 1. Create and activate a virtual environment. It is
+recommended to use a virtual environment for installing volttron. ```shell
+python -m venv env source env/bin/activate pip install volttron ``` 1. Install
+volttron and start the platform. > **Note**: > According to [volttron-
+core#readme](https://github.com/eclipse-volttron/volttron-core#readme), setup
+VOLTTRON_HOME > environment variable is mandatory: > ... if you have/had in the
+past, a monolithic VOLTTRON version that used the default VOLTTRON_HOME >
+$HOME/.volttron. This modular version of VOLTTRON cannot work with
+volttron_home used by monolithic version of > VOLTTRON(version 8.3 or earlier)
+```shell # Setup enviornment variable export VOLTTRON_HOME=/path/to/
+volttron_home/dir # Start platform with output going to volttron.log volttron -
+vv -l volttron.log & ``` 1. Install the volttron platform driver: Note: for
+reproducibility, this demo will install platform driver with `vip-
 identity==platform_driver_for_dnp3`. Free feel to specify any agent vip-
 identity as desired. ```shell vctl install volttron-platform-driver --vip-
 identity platform_driver_for_dnp3 --start ```  Verify with `vctl status`.
 ```shell (env) kefei@ubuntu-22:~/sandbox/dnp3-driver-sandbox$ vctl status UUID
 AGENT IDENTITY TAG PRIORITY STATUS HEALTH 5 volttron-platform-driver-0.2.0rc1
 platform_driver_for_dnp3 running [23217] GOOD ```  1. Install the "volttron-
 lib-dnp3-driver" library. There are two options to install the DNP3 Driver. You
```

### Comparing `volttron_lib_dnp3_driver-0.1.1a2/pyproject.toml` & `volttron_lib_dnp3_driver-0.1.1a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "volttron-lib-dnp3-driver"
-version = "0.1.1a2"
+version = "0.1.1a3"
 description = "A minimal implementation of a driver for the VOLTTRON platform."
 authors = ["VOLTTRON Team <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/volttron-lib-dnp3-driver"
 homepage = "https://github.com/eclipse-volttron/volttron-lib-dnp3-driver"
 keywords = []
@@ -22,15 +22,15 @@
     "Intended Audience :: Information Technology",
     "Intended Audience :: Developers",
     "Intended Audience :: Other Audience",
     "License :: OSI Approved :: Apache Software License"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = "^3.10"
 volttron-lib-base-driver = "^0.2.0rc0"
 dnp3-python = "^0.2.3b2"
 
 [tool.poetry.group.dev.dependencies]
 volttron-testing = "^0.4.0rc0"
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
```

### Comparing `volttron_lib_dnp3_driver-0.1.1a2/src/volttron/driver/interfaces/dnp3/dnp3.py` & `volttron_lib_dnp3_driver-0.1.1a3/src/volttron/driver/interfaces/dnp3/dnp3.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_dnp3_driver-0.1.1a2/PKG-INFO` & `volttron_lib_dnp3_driver-0.1.1a3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: volttron-lib-dnp3-driver
-Version: 0.1.1a2
+Version: 0.1.1a3
 Summary: A minimal implementation of a driver for the VOLTTRON platform.
 Home-page: https://github.com/eclipse-volttron/volttron-lib-dnp3-driver
 License: Apache-2.0
 Author: VOLTTRON Team
 Author-email: volttron@pnnl.gov
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: dnp3-python (>=0.2.3b2,<0.3.0)
 Requires-Dist: volttron-lib-base-driver (>=0.2.0rc0,<0.3.0)
 Project-URL: Repository, https://github.com/eclipse-volttron/volttron-lib-dnp3-driver
 Description-Content-Type: text/markdown
 
 # volttron-lib-dnp3-driver
 
-[//]: # (TODO: get the badges)
+[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
+[![Pytests](https://github.com/eclipse-volttron/volttron-lib-dnp3-driver/actions/workflows/run-tests.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-lib-dnp3-driver/actions/workflows/run-tests.yml)
+[![pypi version](https://img.shields.io/pypi/v/volttron-lib-dnp3-driver.svg)](https://pypi.org/project/volttron-lib-dnp3-driver/)
+
 
 Distributed Network Protocol (DNP
 or [DNP3](https://en.wikipedia.org/wiki/DNP3))
 has achieved a large-scale acceptance since its introduction in 1993. This
 protocol is an immediately deployable solution for monitoring remote sites because it was developed for communication of
 critical infrastructure status, allowing for reliable remote control.
 
@@ -42,15 +45,15 @@
 Note that the DNP3-Driver requires a DNP3 outstation instance to properly function. e.g., polling data, setting point
 values, etc. The [dnp3-python](https://github.com/VOLTTRON/dnp3-python) can provide the essential outstation
 functionality, and as part of the DNP3-Driver dependency, it is immediately available after the DNP3-Driver is
 installed.
 
 # Prerequisites
 
-* Python 3 (tested with Python3.8, Python3.9, Python3.10)
+* Python 3.10
 
 ## Python
 
 <details>
 <summary>To install specific Python version (e.g., Python 3.8), we recommend using <a href="https://github.com/pyenv/pyenv"><code>pyenv</code></a>.</summary>
 
 ```shell
@@ -58,19 +61,19 @@
 git clone https://github.com/pyenv/pyenv ~/.pyenv
 
 # setup pyenv (you should also put these three lines in .bashrc or similar)
 export PATH="${HOME}/.pyenv/bin:${PATH}"
 export PYENV_ROOT="${HOME}/.pyenv"
 eval "$(pyenv init -)"
 
-# install Python 3.8
-pyenv install 3.8.10
+# install Python 3.10
+pyenv install 3.10
 
 # make it available globally
-pyenv global system 3.8.10
+pyenv global system 3.10
 ```
 
 </details>
 
 # Quick Start
 
 The following recipe walks through the steps to install and configure a DNP3 Driver. Note that it uses default setup to
```

#### html2text {}

```diff
@@ -1,84 +1,89 @@
-Metadata-Version: 2.1 Name: volttron-lib-dnp3-driver Version: 0.1.1a2 Summary:
+Metadata-Version: 2.1 Name: volttron-lib-dnp3-driver Version: 0.1.1a3 Summary:
 A minimal implementation of a driver for the VOLTTRON platform. Home-page:
 https://github.com/eclipse-volttron/volttron-lib-dnp3-driver License: Apache-
 2.0 Author: VOLTTRON Team Author-email: volttron@pnnl.gov Requires-Python:
->=3.8,<4.0 Classifier: Intended Audience :: Developers Classifier: Intended
+>=3.10,<4.0 Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: Other
 Audience Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3 :: Only Requires-Dist: dnp3-python
-(>=0.2.3b2,<0.3.0) Requires-Dist: volttron-lib-base-driver (>=0.2.0rc0,<0.3.0)
-Project-URL: Repository, https://github.com/eclipse-volttron/volttron-lib-dnp3-
-driver Description-Content-Type: text/markdown # volttron-lib-dnp3-driver [//]:
-# (TODO: get the badges) Distributed Network Protocol (DNP or [DNP3](https://
-en.wikipedia.org/wiki/DNP3)) has achieved a large-scale acceptance since its
-introduction in 1993. This protocol is an immediately deployable solution for
-monitoring remote sites because it was developed for communication of critical
-infrastructure status, allowing for reliable remote control. DNP3 is typically
-used between centrally located masters and distributed remotes. The master
-provides the interface between the human network manager and the monitoring
-system. The remote (RTUs and intelligent electronic devices) provides the
-interface between the master and the physical device(s) being monitored and/or
-controlled. The DNP3-Driver is a wrapper on the DNP3 master following the
-[VOLTTRON driver framework](https://volttron.readthedocs.io/en/develop/agent-
-framework/driver-framework/drivers-overview.html#driver-framework). Note that
-the DNP3-Driver requires a DNP3 outstation instance to properly function. e.g.,
-polling data, setting point values, etc. The [dnp3-python](https://github.com/
-VOLTTRON/dnp3-python) can provide the essential outstation functionality, and
-as part of the DNP3-Driver dependency, it is immediately available after the
-DNP3-Driver is installed. # Prerequisites * Python 3 (tested with Python3.8,
-Python3.9, Python3.10) ## Python  To install specific Python version (e.g.,
-Python 3.8), we recommend using pyenv. ```shell # install pyenv git clone
-https://github.com/pyenv/pyenv ~/.pyenv # setup pyenv (you should also put
-these three lines in .bashrc or similar) export PATH="${HOME}/.pyenv/bin:$
+Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3 :: Only Requires-Dist: dnp3-python (>=0.2.3b2,<0.3.0) Requires-
+Dist: volttron-lib-base-driver (>=0.2.0rc0,<0.3.0) Project-URL: Repository,
+https://github.com/eclipse-volttron/volttron-lib-dnp3-driver Description-
+Content-Type: text/markdown # volttron-lib-dnp3-driver [![Eclipse VOLTTRONâ¢]
+(https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://
+volttron.readthedocs.io/en/latest/) ![Python 3.10](https://img.shields.io/
+badge/python-3.10-blue.svg) ![Python 3.11](https://img.shields.io/badge/python-
+3.11-blue.svg) [![Pytests](https://github.com/eclipse-volttron/volttron-lib-
+dnp3-driver/actions/workflows/run-tests.yml/badge.svg)](https://github.com/
+eclipse-volttron/volttron-lib-dnp3-driver/actions/workflows/run-tests.yml) [!
+[pypi version](https://img.shields.io/pypi/v/volttron-lib-dnp3-driver.svg)]
+(https://pypi.org/project/volttron-lib-dnp3-driver/) Distributed Network
+Protocol (DNP or [DNP3](https://en.wikipedia.org/wiki/DNP3)) has achieved a
+large-scale acceptance since its introduction in 1993. This protocol is an
+immediately deployable solution for monitoring remote sites because it was
+developed for communication of critical infrastructure status, allowing for
+reliable remote control. DNP3 is typically used between centrally located
+masters and distributed remotes. The master provides the interface between the
+human network manager and the monitoring system. The remote (RTUs and
+intelligent electronic devices) provides the interface between the master and
+the physical device(s) being monitored and/or controlled. The DNP3-Driver is a
+wrapper on the DNP3 master following the [VOLTTRON driver framework](https://
+volttron.readthedocs.io/en/develop/agent-framework/driver-framework/drivers-
+overview.html#driver-framework). Note that the DNP3-Driver requires a DNP3
+outstation instance to properly function. e.g., polling data, setting point
+values, etc. The [dnp3-python](https://github.com/VOLTTRON/dnp3-python) can
+provide the essential outstation functionality, and as part of the DNP3-Driver
+dependency, it is immediately available after the DNP3-Driver is installed. #
+Prerequisites * Python 3.10 ## Python  To install specific Python version
+(e.g., Python 3.8), we recommend using pyenv. ```shell # install pyenv git
+clone https://github.com/pyenv/pyenv ~/.pyenv # setup pyenv (you should also
+put these three lines in .bashrc or similar) export PATH="${HOME}/.pyenv/bin:$
 {PATH}" export PYENV_ROOT="${HOME}/.pyenv" eval "$(pyenv init -)" # install
-Python 3.8 pyenv install 3.8.10 # make it available globally pyenv global
-system 3.8.10 ```  # Quick Start The following recipe walks through the steps
-to install and configure a DNP3 Driver. Note that it uses default setup to work
-out-of-the-box. Please feel free to refer to related documentations for
-details. 1. Create and activate a virtual environment. It is recommended to use
-a virtual environment for installing volttron. ```shell python -m venv env
-source env/bin/activate pip install volttron ``` 1. Install volttron and start
-the platform. > **Note**: > According to [volttron-core#readme](https://
-github.com/eclipse-volttron/volttron-core#readme), setup VOLTTRON_HOME >
-environment variable is mandatory: > ... if you have/had in the past, a
-monolithic VOLTTRON version that used the default VOLTTRON_HOME >
-$HOME/.volttron. This modular version of VOLTTRON cannot work with
-volttron_home used by monolithic version of > VOLTTRON(version 8.3 or earlier)
-```shell # Setup enviornment variable export VOLTTRON_HOME=/path/to/
-volttron_home/dir # Start platform with output going to volttron.log volttron -
-vv -l volttron.log & ``` 1. Install the volttron platform driver: Note: for
-reproducibility, this demo will install platform driver with `vip-
-identity==platform_driver_for_dnp3`. Free feel to specify any agent vip-
-identity as desired. ```shell vctl install volttron-platform-driver --vip-
-identity platform_driver_for_dnp3 --start ```  Verify with `vctl status`.
-```shell (env) kefei@ubuntu-22:~/sandbox/dnp3-driver-sandbox$ vctl status UUID
-AGENT IDENTITY TAG PRIORITY STATUS HEALTH 5 volttron-platform-driver-0.2.0rc1
-platform_driver_for_dnp3 running [23217] GOOD ```  1. Install the "volttron-
-lib-dnp3-driver" library. There are two options to install the DNP3 Driver. You
-can install this library using the version on PyPi or install it from the
-source code (`git clone` might be required.) ```shell # option 1: install from
-pypi pip install volttron-lib-dnp3-driver # option 2: install from the source
-code pip install /volttron-lib-dnp3-driver/ ``` 1. Install a DNP3 Driver onto
-the Platform Driver. Installing a DNP3 driver in the Platform Driver Agent
-requires adding copies of the device configuration and registry configuration
-files to the Platform Driverâs configuration store. For demo purpose, we will
-use default configure files. Prepare the default config files: ```shell #
-Create config file place holders mkdir config touch config/dnp3-config.json
-touch config/dnp3.csv ``` Edit the `dnp3-config.json` as follows: ```json
-{ "driver_config": { "master_ip": "0.0.0.0", "outstation_ip": "127.0.0.1",
-"master_id": 2, "outstation_id": 1, "port": 20000 }, "registry_config":
-"config://dnp3.csv", "driver_type": "dnp3", "interval": 5, "timezone": "UTC",
-"publish_depth_first_all": true, "heart_beat_point": "random_bool" } ``` Edit
-the `dnp3.csv` as follows: ```csv Point Name,Volttron Point
-Name,Group,Variation,Index,Scaling,Units,Writable,Notes
+Python 3.10 pyenv install 3.10 # make it available globally pyenv global system
+3.10 ```  # Quick Start The following recipe walks through the steps to install
+and configure a DNP3 Driver. Note that it uses default setup to work out-of-
+the-box. Please feel free to refer to related documentations for details. 1.
+Create and activate a virtual environment. It is recommended to use a virtual
+environment for installing volttron. ```shell python -m venv env source env/
+bin/activate pip install volttron ``` 1. Install volttron and start the
+platform. > **Note**: > According to [volttron-core#readme](https://github.com/
+eclipse-volttron/volttron-core#readme), setup VOLTTRON_HOME > environment
+variable is mandatory: > ... if you have/had in the past, a monolithic VOLTTRON
+version that used the default VOLTTRON_HOME > $HOME/.volttron. This modular
+version of VOLTTRON cannot work with volttron_home used by monolithic version
+of > VOLTTRON(version 8.3 or earlier) ```shell # Setup enviornment variable
+export VOLTTRON_HOME=/path/to/volttron_home/dir # Start platform with output
+going to volttron.log volttron -vv -l volttron.log & ``` 1. Install the
+volttron platform driver: Note: for reproducibility, this demo will install
+platform driver with `vip-identity==platform_driver_for_dnp3`. Free feel to
+specify any agent vip-identity as desired. ```shell vctl install volttron-
+platform-driver --vip-identity platform_driver_for_dnp3 --start ```  Verify
+with `vctl status`. ```shell (env) kefei@ubuntu-22:~/sandbox/dnp3-driver-
+sandbox$ vctl status UUID AGENT IDENTITY TAG PRIORITY STATUS HEALTH 5 volttron-
+platform-driver-0.2.0rc1 platform_driver_for_dnp3 running [23217] GOOD ```  1.
+Install the "volttron-lib-dnp3-driver" library. There are two options to
+install the DNP3 Driver. You can install this library using the version on PyPi
+or install it from the source code (`git clone` might be required.) ```shell #
+option 1: install from pypi pip install volttron-lib-dnp3-driver # option 2:
+install from the source code pip install /volttron-lib-dnp3-driver/ ``` 1.
+Install a DNP3 Driver onto the Platform Driver. Installing a DNP3 driver in the
+Platform Driver Agent requires adding copies of the device configuration and
+registry configuration files to the Platform Driverâs configuration store.
+For demo purpose, we will use default configure files. Prepare the default
+config files: ```shell # Create config file place holders mkdir config touch
+config/dnp3-config.json touch config/dnp3.csv ``` Edit the `dnp3-config.json`
+as follows: ```json { "driver_config": { "master_ip": "0.0.0.0",
+"outstation_ip": "127.0.0.1", "master_id": 2, "outstation_id": 1, "port": 20000
+}, "registry_config": "config://dnp3.csv", "driver_type": "dnp3", "interval":
+5, "timezone": "UTC", "publish_depth_first_all": true, "heart_beat_point":
+"random_bool" } ``` Edit the `dnp3.csv` as follows: ```csv Point Name,Volttron
+Point Name,Group,Variation,Index,Scaling,Units,Writable,Notes
 AnalogInput_index0,AnalogInput_index0,30,6,0,1,NA,FALSE,Double Analogue input
 without status AnalogInput_index1,AnalogInput_index1,30,6,1,1,NA,FALSE,Double
 Analogue input without status
 AnalogInput_index2,AnalogInput_index2,30,6,2,1,NA,FALSE,Double Analogue input
 without status AnalogInput_index3,AnalogInput_index3,30,6,3,1,NA,FALSE,Double
 Analogue input without status
 BinaryInput_index0,BinaryInput_index0,1,2,0,1,NA,FALSE,Single bit binary input
```

