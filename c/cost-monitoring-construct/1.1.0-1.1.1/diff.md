# Comparing `tmp/cost-monitoring-construct-1.1.0.tar.gz` & `tmp/cost-monitoring-construct-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cost-monitoring-construct-1.1.0.tar", last modified: Thu Mar 23 08:01:50 2023, max compression
+gzip compressed data, was "cost-monitoring-construct-1.1.1.tar", last modified: Thu May 11 07:48:04 2023, max compression
```

## Comparing `cost-monitoring-construct-1.1.0.tar` & `cost-monitoring-construct-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:01:50.112618 cost-monitoring-construct-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-23 08:01:34.000000 cost-monitoring-construct-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-23 08:01:34.000000 cost-monitoring-construct-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-03-23 08:01:50.112618 cost-monitoring-construct-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-03-23 08:01:34.000000 cost-monitoring-construct-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-23 08:01:34.000000 cost-monitoring-construct-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 08:01:50.112618 cost-monitoring-construct-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-03-23 08:01:34.000000 cost-monitoring-construct-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:01:50.108618 cost-monitoring-construct-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:01:50.108618 cost-monitoring-construct-1.1.0/src/cost_monitoring_construct/
--rw-r--r--   0 runner    (1001) docker     (123)    60447 2023-03-23 08:01:34.000000 cost-monitoring-construct-1.1.0/src/cost_monitoring_construct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:01:50.112618 cost-monitoring-construct-1.1.0/src/cost_monitoring_construct/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-23 08:01:34.000000 cost-monitoring-construct-1.1.0/src/cost_monitoring_construct/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37349 2023-03-23 08:01:34.000000 cost-monitoring-construct-1.1.0/src/cost_monitoring_construct/_jsii/cost-monitoring-construct@1.1.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 08:01:34.000000 cost-monitoring-construct-1.1.0/src/cost_monitoring_construct/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:01:50.112618 cost-monitoring-construct-1.1.0/src/cost_monitoring_construct.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-03-23 08:01:50.000000 cost-monitoring-construct-1.1.0/src/cost_monitoring_construct.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-23 08:01:50.000000 cost-monitoring-construct-1.1.0/src/cost_monitoring_construct.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 08:01:50.000000 cost-monitoring-construct-1.1.0/src/cost_monitoring_construct.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-23 08:01:50.000000 cost-monitoring-construct-1.1.0/src/cost_monitoring_construct.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-23 08:01:50.000000 cost-monitoring-construct-1.1.0/src/cost_monitoring_construct.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:48:04.958860 cost-monitoring-construct-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-11 07:47:48.000000 cost-monitoring-construct-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 07:47:48.000000 cost-monitoring-construct-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-05-11 07:48:04.958860 cost-monitoring-construct-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-11 07:47:48.000000 cost-monitoring-construct-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-11 07:47:48.000000 cost-monitoring-construct-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 07:48:04.958860 cost-monitoring-construct-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-11 07:47:48.000000 cost-monitoring-construct-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:48:04.958860 cost-monitoring-construct-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:48:04.958860 cost-monitoring-construct-1.1.1/src/cost_monitoring_construct/
+-rw-r--r--   0 runner    (1001) docker     (123)    61281 2023-05-11 07:47:48.000000 cost-monitoring-construct-1.1.1/src/cost_monitoring_construct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:48:04.958860 cost-monitoring-construct-1.1.1/src/cost_monitoring_construct/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-11 07:47:48.000000 cost-monitoring-construct-1.1.1/src/cost_monitoring_construct/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75246 2023-05-11 07:47:48.000000 cost-monitoring-construct-1.1.1/src/cost_monitoring_construct/_jsii/cost-monitoring-construct@1.1.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 07:47:48.000000 cost-monitoring-construct-1.1.1/src/cost_monitoring_construct/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:48:04.958860 cost-monitoring-construct-1.1.1/src/cost_monitoring_construct.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-05-11 07:48:04.000000 cost-monitoring-construct-1.1.1/src/cost_monitoring_construct.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-11 07:48:04.000000 cost-monitoring-construct-1.1.1/src/cost_monitoring_construct.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 07:48:04.000000 cost-monitoring-construct-1.1.1/src/cost_monitoring_construct.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-11 07:48:04.000000 cost-monitoring-construct-1.1.1/src/cost_monitoring_construct.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-11 07:48:04.000000 cost-monitoring-construct-1.1.1/src/cost_monitoring_construct.egg-info/top_level.txt
```

### Comparing `cost-monitoring-construct-1.1.0/LICENSE` & `cost-monitoring-construct-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cost-monitoring-construct-1.1.0/PKG-INFO` & `cost-monitoring-construct-1.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cost-monitoring-construct
-Version: 1.1.0
+Version: 1.1.1
 Summary: A CDK construct that helps track applications' costs separately and receive alerts in case of unpredicted resource usage
 Home-page: https://github.com/DataChefHQ/cost-monitoring-construct.git
 Author: DataChef<support@datachef.co>
 License: Apache-2.0
 Project-URL: Source, https://github.com/DataChefHQ/cost-monitoring-construct.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,20 @@
 
 # What is Cost Monitoring Construct?
 
 Cost Monitoring Construct is a CDK library that helps monitor costs for AWS cloud infrastructure resources, such as virtual machines, storage, and network traffic. It allows you to set budgets and alerts to ensure that you don't overspend on your cloud resources.
 
 With the Cost Monitoring Construct, you can share the responsibility of cost management between developers and business holders. This is achieved through the creation of meaningful reports that enable the business team to make informed decisions. Additionally, the Construct generates boilerplate code that can be used to apply these decisions in practice, making it easier to stay on top of your budget.
 
+# How to use Cost Monitoring Construct?
+
+To use Cost Monitoring Construct, all you need is to have the AWS CDK installed and set up. Once you have that, you can install the package from the repository of your choice.
+
+For more information on using this Construct in TypeScript checkout the [TypeScript documentation](docs/typescript.md). You can also check the typescript example from [sample folder](https://github.com/DataChefHQ/cost-monitoring-construct/tree/main/sample) on the GitHub repository.
+
 # Why do you need it?
 
 Cloud services can get very expensive, very quickly, especially if you are not careful with your usage. Cost Monitoring Construct helps you to keep an eye on your cloud infrastructure costs so that you can stay within budget. By setting budgets and defining alert strategies, you can take proactive steps to reduce costs before they become a problem.
 
 # How does Cost Monitoring Construct work?
 
 Cost Monitoring Construct uses AWS Tagging practice to track resources related to an specific application, creates proper alert with respect to the defined budget limit and provide overview dashbords. The tool is highly customizable and allows you to customize it to your budgeting strategy based on your specific needs.
@@ -53,18 +59,18 @@
 
 The Cost Monitoring Construct is not a magical tool that can solve all of your cloud cost problems. In spite of the fact that it can bring clarity and help you to identify areas where you can reduce costs, you must make the necessary decisions about your infrastructure on your own.
 
 # Which programming languages Cost Monitoring Construct supports?
 
 Cost Monitoring Construct has been developed using JSII technolgy to provide interfaces for different modern programming languages. Currently, it supports the following languages:
 
-* TypeScript
-* JavaScript
-* Python
-* .NET
-* Java
+* [TypeScript](https://www.npmjs.com/package/cost-monitoring-construct)
+* [JavaScript](https://www.npmjs.com/package/cost-monitoring-construct)
+* [Python](https://pypi.org/project/cost-monitoring-construct/)
+* [.NET](https://www.nuget.org/packages/DataChef.CostMonitoringConstruct)
+* [Java](https://central.sonatype.com/artifact/co.datachef/costmonitoringconstruct/1.1.0/versions)
 
 > **✏️ Note**
 >
 > Go will be supported soon but for now you can build it from the source.
 
 If you have any questions or need help with Cost Monitoring Construct, you can reach out to our support team at [support@datachef.co](mailto:support@datachef.co).
```

### Comparing `cost-monitoring-construct-1.1.0/README.md` & `cost-monitoring-construct-1.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # What is Cost Monitoring Construct?
 
 Cost Monitoring Construct is a CDK library that helps monitor costs for AWS cloud infrastructure resources, such as virtual machines, storage, and network traffic. It allows you to set budgets and alerts to ensure that you don't overspend on your cloud resources.
 
 With the Cost Monitoring Construct, you can share the responsibility of cost management between developers and business holders. This is achieved through the creation of meaningful reports that enable the business team to make informed decisions. Additionally, the Construct generates boilerplate code that can be used to apply these decisions in practice, making it easier to stay on top of your budget.
 
+# How to use Cost Monitoring Construct?
+
+To use Cost Monitoring Construct, all you need is to have the AWS CDK installed and set up. Once you have that, you can install the package from the repository of your choice.
+
+For more information on using this Construct in TypeScript checkout the [TypeScript documentation](docs/typescript.md). You can also check the typescript example from [sample folder](https://github.com/DataChefHQ/cost-monitoring-construct/tree/main/sample) on the GitHub repository.
+
 # Why do you need it?
 
 Cloud services can get very expensive, very quickly, especially if you are not careful with your usage. Cost Monitoring Construct helps you to keep an eye on your cloud infrastructure costs so that you can stay within budget. By setting budgets and defining alert strategies, you can take proactive steps to reduce costs before they become a problem.
 
 # How does Cost Monitoring Construct work?
 
 Cost Monitoring Construct uses AWS Tagging practice to track resources related to an specific application, creates proper alert with respect to the defined budget limit and provide overview dashbords. The tool is highly customizable and allows you to customize it to your budgeting strategy based on your specific needs.
@@ -30,18 +36,18 @@
 
 The Cost Monitoring Construct is not a magical tool that can solve all of your cloud cost problems. In spite of the fact that it can bring clarity and help you to identify areas where you can reduce costs, you must make the necessary decisions about your infrastructure on your own.
 
 # Which programming languages Cost Monitoring Construct supports?
 
 Cost Monitoring Construct has been developed using JSII technolgy to provide interfaces for different modern programming languages. Currently, it supports the following languages:
 
-* TypeScript
-* JavaScript
-* Python
-* .NET
-* Java
+* [TypeScript](https://www.npmjs.com/package/cost-monitoring-construct)
+* [JavaScript](https://www.npmjs.com/package/cost-monitoring-construct)
+* [Python](https://pypi.org/project/cost-monitoring-construct/)
+* [.NET](https://www.nuget.org/packages/DataChef.CostMonitoringConstruct)
+* [Java](https://central.sonatype.com/artifact/co.datachef/costmonitoringconstruct/1.1.0/versions)
 
 > **✏️ Note**
 >
 > Go will be supported soon but for now you can build it from the source.
 
 If you have any questions or need help with Cost Monitoring Construct, you can reach out to our support team at [support@datachef.co](mailto:support@datachef.co).
```

### Comparing `cost-monitoring-construct-1.1.0/setup.py` & `cost-monitoring-construct-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cost-monitoring-construct",
-    "version": "1.1.0",
+    "version": "1.1.1",
     "description": "A CDK construct that helps track applications' costs separately and receive alerts in case of unpredicted resource usage",
     "license": "Apache-2.0",
     "url": "https://github.com/DataChefHQ/cost-monitoring-construct.git",
     "long_description_content_type": "text/markdown",
     "author": "DataChef<support@datachef.co>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cost_monitoring_construct",
         "cost_monitoring_construct._jsii"
     ],
     "package_data": {
         "cost_monitoring_construct._jsii": [
-            "cost-monitoring-construct@1.1.0.jsii.tgz"
+            "cost-monitoring-construct@1.1.1.jsii.tgz"
         ],
         "cost_monitoring_construct": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cost-monitoring-construct-1.1.0/src/cost_monitoring_construct/__init__.py` & `cost-monitoring-construct-1.1.1/src/cost_monitoring_construct/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 '''
 # What is Cost Monitoring Construct?
 
 Cost Monitoring Construct is a CDK library that helps monitor costs for AWS cloud infrastructure resources, such as virtual machines, storage, and network traffic. It allows you to set budgets and alerts to ensure that you don't overspend on your cloud resources.
 
 With the Cost Monitoring Construct, you can share the responsibility of cost management between developers and business holders. This is achieved through the creation of meaningful reports that enable the business team to make informed decisions. Additionally, the Construct generates boilerplate code that can be used to apply these decisions in practice, making it easier to stay on top of your budget.
 
+# How to use Cost Monitoring Construct?
+
+To use Cost Monitoring Construct, all you need is to have the AWS CDK installed and set up. Once you have that, you can install the package from the repository of your choice.
+
+For more information on using this Construct in TypeScript checkout the [TypeScript documentation](docs/typescript.md). You can also check the typescript example from [sample folder](https://github.com/DataChefHQ/cost-monitoring-construct/tree/main/sample) on the GitHub repository.
+
 # Why do you need it?
 
 Cloud services can get very expensive, very quickly, especially if you are not careful with your usage. Cost Monitoring Construct helps you to keep an eye on your cloud infrastructure costs so that you can stay within budget. By setting budgets and defining alert strategies, you can take proactive steps to reduce costs before they become a problem.
 
 # How does Cost Monitoring Construct work?
 
 Cost Monitoring Construct uses AWS Tagging practice to track resources related to an specific application, creates proper alert with respect to the defined budget limit and provide overview dashbords. The tool is highly customizable and allows you to customize it to your budgeting strategy based on your specific needs.
@@ -31,19 +37,19 @@
 
 The Cost Monitoring Construct is not a magical tool that can solve all of your cloud cost problems. In spite of the fact that it can bring clarity and help you to identify areas where you can reduce costs, you must make the necessary decisions about your infrastructure on your own.
 
 # Which programming languages Cost Monitoring Construct supports?
 
 Cost Monitoring Construct has been developed using JSII technolgy to provide interfaces for different modern programming languages. Currently, it supports the following languages:
 
-* TypeScript
-* JavaScript
-* Python
-* .NET
-* Java
+* [TypeScript](https://www.npmjs.com/package/cost-monitoring-construct)
+* [JavaScript](https://www.npmjs.com/package/cost-monitoring-construct)
+* [Python](https://pypi.org/project/cost-monitoring-construct/)
+* [.NET](https://www.nuget.org/packages/DataChef.CostMonitoringConstruct)
+* [Java](https://central.sonatype.com/artifact/co.datachef/costmonitoringconstruct/1.1.0/versions)
 
 > **✏️ Note**
 >
 > Go will be supported soon but for now you can build it from the source.
 
 If you have any questions or need help with Cost Monitoring Construct, you can reach out to our support team at [support@datachef.co](mailto:support@datachef.co).
 '''
```

### Comparing `cost-monitoring-construct-1.1.0/src/cost_monitoring_construct.egg-info/PKG-INFO` & `cost-monitoring-construct-1.1.1/src/cost_monitoring_construct.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cost-monitoring-construct
-Version: 1.1.0
+Version: 1.1.1
 Summary: A CDK construct that helps track applications' costs separately and receive alerts in case of unpredicted resource usage
 Home-page: https://github.com/DataChefHQ/cost-monitoring-construct.git
 Author: DataChef<support@datachef.co>
 License: Apache-2.0
 Project-URL: Source, https://github.com/DataChefHQ/cost-monitoring-construct.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,20 @@
 
 # What is Cost Monitoring Construct?
 
 Cost Monitoring Construct is a CDK library that helps monitor costs for AWS cloud infrastructure resources, such as virtual machines, storage, and network traffic. It allows you to set budgets and alerts to ensure that you don't overspend on your cloud resources.
 
 With the Cost Monitoring Construct, you can share the responsibility of cost management between developers and business holders. This is achieved through the creation of meaningful reports that enable the business team to make informed decisions. Additionally, the Construct generates boilerplate code that can be used to apply these decisions in practice, making it easier to stay on top of your budget.
 
+# How to use Cost Monitoring Construct?
+
+To use Cost Monitoring Construct, all you need is to have the AWS CDK installed and set up. Once you have that, you can install the package from the repository of your choice.
+
+For more information on using this Construct in TypeScript checkout the [TypeScript documentation](docs/typescript.md). You can also check the typescript example from [sample folder](https://github.com/DataChefHQ/cost-monitoring-construct/tree/main/sample) on the GitHub repository.
+
 # Why do you need it?
 
 Cloud services can get very expensive, very quickly, especially if you are not careful with your usage. Cost Monitoring Construct helps you to keep an eye on your cloud infrastructure costs so that you can stay within budget. By setting budgets and defining alert strategies, you can take proactive steps to reduce costs before they become a problem.
 
 # How does Cost Monitoring Construct work?
 
 Cost Monitoring Construct uses AWS Tagging practice to track resources related to an specific application, creates proper alert with respect to the defined budget limit and provide overview dashbords. The tool is highly customizable and allows you to customize it to your budgeting strategy based on your specific needs.
@@ -53,18 +59,18 @@
 
 The Cost Monitoring Construct is not a magical tool that can solve all of your cloud cost problems. In spite of the fact that it can bring clarity and help you to identify areas where you can reduce costs, you must make the necessary decisions about your infrastructure on your own.
 
 # Which programming languages Cost Monitoring Construct supports?
 
 Cost Monitoring Construct has been developed using JSII technolgy to provide interfaces for different modern programming languages. Currently, it supports the following languages:
 
-* TypeScript
-* JavaScript
-* Python
-* .NET
-* Java
+* [TypeScript](https://www.npmjs.com/package/cost-monitoring-construct)
+* [JavaScript](https://www.npmjs.com/package/cost-monitoring-construct)
+* [Python](https://pypi.org/project/cost-monitoring-construct/)
+* [.NET](https://www.nuget.org/packages/DataChef.CostMonitoringConstruct)
+* [Java](https://central.sonatype.com/artifact/co.datachef/costmonitoringconstruct/1.1.0/versions)
 
 > **✏️ Note**
 >
 > Go will be supported soon but for now you can build it from the source.
 
 If you have any questions or need help with Cost Monitoring Construct, you can reach out to our support team at [support@datachef.co](mailto:support@datachef.co).
```

### Comparing `cost-monitoring-construct-1.1.0/src/cost_monitoring_construct.egg-info/SOURCES.txt` & `cost-monitoring-construct-1.1.1/src/cost_monitoring_construct.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cost_monitoring_construct/py.typed
 src/cost_monitoring_construct.egg-info/PKG-INFO
 src/cost_monitoring_construct.egg-info/SOURCES.txt
 src/cost_monitoring_construct.egg-info/dependency_links.txt
 src/cost_monitoring_construct.egg-info/requires.txt
 src/cost_monitoring_construct.egg-info/top_level.txt
 src/cost_monitoring_construct/_jsii/__init__.py
-src/cost_monitoring_construct/_jsii/cost-monitoring-construct@1.1.0.jsii.tgz
+src/cost_monitoring_construct/_jsii/cost-monitoring-construct@1.1.1.jsii.tgz
```

