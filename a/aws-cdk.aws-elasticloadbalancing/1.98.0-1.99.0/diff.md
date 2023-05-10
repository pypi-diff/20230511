# Comparing `tmp/aws-cdk.aws-elasticloadbalancing-1.98.0.tar.gz` & `tmp/aws-cdk.aws-elasticloadbalancing-1.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src518022412/src/packages/@aws-cdk/aws-elasticloadbalancing/dist/python/aws-cdk.aws-elasticloadbalancing-1.98", last modified: Mon Apr 12 10:09:04 2021, max compression
+gzip compressed data, was "/codebuild/output/src875002972/src/packages/@aws-cdk/aws-elasticloadbalancing/dist/python/aws-cdk.aws-elasticloadbalancing-1.99", last modified: Tue Apr 13 17:03:15 2021, max compression
```

## Comparing `aws-cdk.aws-elasticloadbalancing-1.98.0.tar` & `aws-cdk.aws-elasticloadbalancing-1.99.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:04.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/
--rw-r--r--   0 root         (0) root         (0)       23 2021-04-12 10:07:22.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2693 2021-04-12 10:09:04.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1349 2021-04-12 10:07:22.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2021-04-12 10:07:22.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2021-04-12 10:09:04.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1882 2021-04-12 10:07:22.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:04.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:04.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:04.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/src/aws_cdk/aws_elasticloadbalancing/
--rw-r--r--   0 root         (0) root         (0)    93885 2021-04-12 10:07:22.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/src/aws_cdk/aws_elasticloadbalancing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:04.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/src/aws_cdk/aws_elasticloadbalancing/_jsii/
--rw-r--r--   0 root         (0) root         (0)      439 2021-04-12 10:07:22.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/src/aws_cdk/aws_elasticloadbalancing/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49037 2021-04-12 10:07:20.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/src/aws_cdk/aws_elasticloadbalancing/_jsii/aws-elasticloadbalancing@1.98.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-12 10:07:22.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/src/aws_cdk/aws_elasticloadbalancing/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:04.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/src/aws_cdk.aws_elasticloadbalancing.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2693 2021-04-12 10:09:04.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/src/aws_cdk.aws_elasticloadbalancing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      578 2021-04-12 10:09:04.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/src/aws_cdk.aws_elasticloadbalancing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-12 10:09:04.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/src/aws_cdk.aws_elasticloadbalancing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2021-04-12 10:09:04.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/src/aws_cdk.aws_elasticloadbalancing.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2021-04-12 10:09:04.000000 aws-cdk.aws-elasticloadbalancing-1.98.0/src/aws_cdk.aws_elasticloadbalancing.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:15.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2021-04-13 17:02:04.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2021-04-13 17:02:05.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2021-04-13 17:02:04.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     2693 2021-04-13 17:03:15.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1349 2021-04-13 17:02:05.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2021-04-13 17:02:05.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-04-13 17:03:15.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1882 2021-04-13 17:02:05.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:15.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:15.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:15.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/src/aws_cdk/aws_elasticloadbalancing/
+-rw-r--r--   0 root         (0) root         (0)    94863 2021-04-13 17:02:05.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/src/aws_cdk/aws_elasticloadbalancing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:15.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/src/aws_cdk/aws_elasticloadbalancing/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      439 2021-04-13 17:02:05.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/src/aws_cdk/aws_elasticloadbalancing/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49395 2021-04-13 17:02:03.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/src/aws_cdk/aws_elasticloadbalancing/_jsii/aws-elasticloadbalancing@1.99.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 17:02:05.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/src/aws_cdk/aws_elasticloadbalancing/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:15.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/src/aws_cdk.aws_elasticloadbalancing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2693 2021-04-13 17:03:15.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/src/aws_cdk.aws_elasticloadbalancing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      593 2021-04-13 17:03:15.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/src/aws_cdk.aws_elasticloadbalancing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 17:03:15.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/src/aws_cdk.aws_elasticloadbalancing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2021-04-13 17:03:15.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/src/aws_cdk.aws_elasticloadbalancing.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2021-04-13 17:03:15.000000 aws-cdk.aws-elasticloadbalancing-1.99.0/src/aws_cdk.aws_elasticloadbalancing.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-elasticloadbalancing-1.98.0/PKG-INFO` & `aws-cdk.aws-elasticloadbalancing-1.99.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-elasticloadbalancing
-Version: 1.98.0
+Version: 1.99.0
 Summary: The CDK Construct Library for AWS::ElasticLoadBalancing
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: # Amazon Elastic Load Balancing Construct Library
```

### Comparing `aws-cdk.aws-elasticloadbalancing-1.98.0/README.md` & `aws-cdk.aws-elasticloadbalancing-1.99.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-elasticloadbalancing-1.98.0/setup.py` & `aws-cdk.aws-elasticloadbalancing-1.99.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-elasticloadbalancing",
-    "version": "1.98.0",
+    "version": "1.99.0",
     "description": "The CDK Construct Library for AWS::ElasticLoadBalancing",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,26 +22,26 @@
     },
     "packages": [
         "aws_cdk.aws_elasticloadbalancing",
         "aws_cdk.aws_elasticloadbalancing._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_elasticloadbalancing._jsii": [
-            "aws-elasticloadbalancing@1.98.0.jsii.tgz"
+            "aws-elasticloadbalancing@1.99.0.jsii.tgz"
         ],
         "aws_cdk.aws_elasticloadbalancing": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
-        "aws-cdk.aws-ec2==1.98.0",
-        "aws-cdk.core==1.98.0",
+        "aws-cdk.aws-ec2==1.99.0",
+        "aws-cdk.core==1.99.0",
         "constructs>=3.3.69, <4.0.0",
-        "jsii>=1.27.0, <2.0.0",
+        "jsii>=1.28.0, <2.0.0",
         "publication>=0.0.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `aws-cdk.aws-elasticloadbalancing-1.98.0/src/aws_cdk/aws_elasticloadbalancing/__init__.py` & `aws-cdk.aws-elasticloadbalancing-1.99.0/src/aws_cdk/aws_elasticloadbalancing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1589,35 +1589,38 @@
         *,
         external_port: jsii.Number,
         allow_connections_from: typing.Optional[typing.Sequence[aws_cdk.aws_ec2.IConnectable]] = None,
         external_protocol: typing.Optional["LoadBalancingProtocol"] = None,
         internal_port: typing.Optional[jsii.Number] = None,
         internal_protocol: typing.Optional["LoadBalancingProtocol"] = None,
         policy_names: typing.Optional[typing.Sequence[builtins.str]] = None,
+        ssl_certificate_arn: typing.Optional[builtins.str] = None,
         ssl_certificate_id: typing.Optional[builtins.str] = None,
     ) -> ListenerPort:
         '''Add a backend to the load balancer.
 
         :param external_port: External listening port.
         :param allow_connections_from: Allow connections to the load balancer from the given set of connection peers. By default, connections will be allowed from anywhere. Set this to an empty list to deny connections, or supply a custom list of peers to allow connections from (IP ranges or security groups). Default: Anywhere
         :param external_protocol: What public protocol to use for load balancing. Either 'tcp', 'ssl', 'http' or 'https'. May be omitted if the external port is either 80 or 443.
         :param internal_port: Instance listening port. Same as the externalPort if not specified. Default: externalPort
         :param internal_protocol: What public protocol to use for load balancing. Either 'tcp', 'ssl', 'http' or 'https'. May be omitted if the internal port is either 80 or 443. The instance protocol is 'tcp' if the front-end protocol is 'tcp' or 'ssl', the instance protocol is 'http' if the front-end protocol is 'https'.
         :param policy_names: SSL policy names.
-        :param ssl_certificate_id: ID of SSL certificate.
+        :param ssl_certificate_arn: the ARN of the SSL certificate. Default: - none
+        :param ssl_certificate_id: (deprecated) the ARN of the SSL certificate.
 
         :return: A ListenerPort object that controls connections to the listener port
         '''
         listener = LoadBalancerListener(
             external_port=external_port,
             allow_connections_from=allow_connections_from,
             external_protocol=external_protocol,
             internal_port=internal_port,
             internal_protocol=internal_protocol,
             policy_names=policy_names,
+            ssl_certificate_arn=ssl_certificate_arn,
             ssl_certificate_id=ssl_certificate_id,
         )
 
         return typing.cast(ListenerPort, jsii.invoke(self, "addListener", [listener]))
 
     @jsii.member(jsii_name="addTarget")
     def add_target(self, target: ILoadBalancerTarget) -> None:
@@ -1693,52 +1696,57 @@
     name_mapping={
         "external_port": "externalPort",
         "allow_connections_from": "allowConnectionsFrom",
         "external_protocol": "externalProtocol",
         "internal_port": "internalPort",
         "internal_protocol": "internalProtocol",
         "policy_names": "policyNames",
+        "ssl_certificate_arn": "sslCertificateArn",
         "ssl_certificate_id": "sslCertificateId",
     },
 )
 class LoadBalancerListener:
     def __init__(
         self,
         *,
         external_port: jsii.Number,
         allow_connections_from: typing.Optional[typing.Sequence[aws_cdk.aws_ec2.IConnectable]] = None,
         external_protocol: typing.Optional["LoadBalancingProtocol"] = None,
         internal_port: typing.Optional[jsii.Number] = None,
         internal_protocol: typing.Optional["LoadBalancingProtocol"] = None,
         policy_names: typing.Optional[typing.Sequence[builtins.str]] = None,
+        ssl_certificate_arn: typing.Optional[builtins.str] = None,
         ssl_certificate_id: typing.Optional[builtins.str] = None,
     ) -> None:
         '''Add a backend to the load balancer.
 
         :param external_port: External listening port.
         :param allow_connections_from: Allow connections to the load balancer from the given set of connection peers. By default, connections will be allowed from anywhere. Set this to an empty list to deny connections, or supply a custom list of peers to allow connections from (IP ranges or security groups). Default: Anywhere
         :param external_protocol: What public protocol to use for load balancing. Either 'tcp', 'ssl', 'http' or 'https'. May be omitted if the external port is either 80 or 443.
         :param internal_port: Instance listening port. Same as the externalPort if not specified. Default: externalPort
         :param internal_protocol: What public protocol to use for load balancing. Either 'tcp', 'ssl', 'http' or 'https'. May be omitted if the internal port is either 80 or 443. The instance protocol is 'tcp' if the front-end protocol is 'tcp' or 'ssl', the instance protocol is 'http' if the front-end protocol is 'https'.
         :param policy_names: SSL policy names.
-        :param ssl_certificate_id: ID of SSL certificate.
+        :param ssl_certificate_arn: the ARN of the SSL certificate. Default: - none
+        :param ssl_certificate_id: (deprecated) the ARN of the SSL certificate.
         '''
         self._values: typing.Dict[str, typing.Any] = {
             "external_port": external_port,
         }
         if allow_connections_from is not None:
             self._values["allow_connections_from"] = allow_connections_from
         if external_protocol is not None:
             self._values["external_protocol"] = external_protocol
         if internal_port is not None:
             self._values["internal_port"] = internal_port
         if internal_protocol is not None:
             self._values["internal_protocol"] = internal_protocol
         if policy_names is not None:
             self._values["policy_names"] = policy_names
+        if ssl_certificate_arn is not None:
+            self._values["ssl_certificate_arn"] = ssl_certificate_arn
         if ssl_certificate_id is not None:
             self._values["ssl_certificate_id"] = ssl_certificate_id
 
     @builtins.property
     def external_port(self) -> jsii.Number:
         '''External listening port.'''
         result = self._values.get("external_port")
@@ -1800,16 +1808,30 @@
     @builtins.property
     def policy_names(self) -> typing.Optional[typing.List[builtins.str]]:
         '''SSL policy names.'''
         result = self._values.get("policy_names")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
+    def ssl_certificate_arn(self) -> typing.Optional[builtins.str]:
+        '''the ARN of the SSL certificate.
+
+        :default: - none
+        '''
+        result = self._values.get("ssl_certificate_arn")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def ssl_certificate_id(self) -> typing.Optional[builtins.str]:
-        '''ID of SSL certificate.'''
+        '''(deprecated) the ARN of the SSL certificate.
+
+        :deprecated: - use sslCertificateArn instead
+
+        :stability: deprecated
+        '''
         result = self._values.get("ssl_certificate_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `aws-cdk.aws-elasticloadbalancing-1.98.0/src/aws_cdk.aws_elasticloadbalancing.egg-info/PKG-INFO` & `aws-cdk.aws-elasticloadbalancing-1.99.0/src/aws_cdk.aws_elasticloadbalancing.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-elasticloadbalancing
-Version: 1.98.0
+Version: 1.99.0
 Summary: The CDK Construct Library for AWS::ElasticLoadBalancing
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: # Amazon Elastic Load Balancing Construct Library
```

### Comparing `aws-cdk.aws-elasticloadbalancing-1.98.0/src/aws_cdk.aws_elasticloadbalancing.egg-info/SOURCES.txt` & `aws-cdk.aws-elasticloadbalancing-1.99.0/src/aws_cdk.aws_elasticloadbalancing.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+LICENSE
 MANIFEST.in
+NOTICE
 README.md
 pyproject.toml
 setup.py
 src/aws_cdk.aws_elasticloadbalancing.egg-info/PKG-INFO
 src/aws_cdk.aws_elasticloadbalancing.egg-info/SOURCES.txt
 src/aws_cdk.aws_elasticloadbalancing.egg-info/dependency_links.txt
 src/aws_cdk.aws_elasticloadbalancing.egg-info/requires.txt
 src/aws_cdk.aws_elasticloadbalancing.egg-info/top_level.txt
 src/aws_cdk/aws_elasticloadbalancing/__init__.py
 src/aws_cdk/aws_elasticloadbalancing/py.typed
 src/aws_cdk/aws_elasticloadbalancing/_jsii/__init__.py
-src/aws_cdk/aws_elasticloadbalancing/_jsii/aws-elasticloadbalancing@1.98.0.jsii.tgz
+src/aws_cdk/aws_elasticloadbalancing/_jsii/aws-elasticloadbalancing@1.99.0.jsii.tgz
```

