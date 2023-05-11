# Comparing `tmp/rltest-0.6.0.tar.gz` & `tmp/rltest-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rltest-0.6.0.tar", max compression
+gzip compressed data, was "rltest-0.7.0.tar", max compression
```

## Comparing `rltest-0.6.0.tar` & `rltest-0.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1518 2023-03-02 16:45:06.503491 rltest-0.6.0/LICENSE
--rw-r--r--   0        0        0    12026 2023-03-02 16:45:06.503491 rltest-0.6.0/README.md
--rw-r--r--   0        0        0     8112 2023-03-02 16:45:06.503491 rltest-0.6.0/RLTest/Enterprise/CcsMock.py
--rw-r--r--   0        0        0     1835 2023-03-02 16:45:06.503491 rltest-0.6.0/RLTest/Enterprise/Dmc.py
--rw-r--r--   0        0        0     6393 2023-03-02 16:45:06.503491 rltest-0.6.0/RLTest/Enterprise/EnterpriseClusterEnv.py
--rw-r--r--   0        0        0       96 2023-03-02 16:45:06.503491 rltest-0.6.0/RLTest/Enterprise/__init__.py
--rw-r--r--   0        0        0     2705 2023-03-02 16:45:06.503491 rltest-0.6.0/RLTest/Enterprise/binaryrepo.py
--rw-r--r--   0        0        0      173 2023-03-02 16:45:06.503491 rltest-0.6.0/RLTest/__init__.py
--rw-r--r--   0        0        0    30128 2023-03-02 16:45:06.503491 rltest-0.6.0/RLTest/__main__.py
--rw-r--r--   0        0        0      361 2023-03-02 16:45:06.503491 rltest-0.6.0/RLTest/_version.py
--rw-r--r--   0        0        0     2398 2023-03-02 16:45:06.503491 rltest-0.6.0/RLTest/debuggers.py
--rw-r--r--   0        0        0    21757 2023-03-02 16:45:06.503491 rltest-0.6.0/RLTest/env.py
--rw-r--r--   0        0        0     3592 2023-03-02 16:45:06.507491 rltest-0.6.0/RLTest/exists_redis.py
--rw-r--r--   0        0        0     5623 2023-03-02 16:45:06.507491 rltest-0.6.0/RLTest/loader.py
--rw-r--r--   0        0        0     1620 2023-03-02 16:45:06.507491 rltest-0.6.0/RLTest/random_port.py
--rw-r--r--   0        0        0     7559 2023-03-02 16:45:06.507491 rltest-0.6.0/RLTest/redis_cluster.py
--rw-r--r--   0        0        0     5245 2023-03-02 16:45:06.507491 rltest-0.6.0/RLTest/redis_enterprise_cluster.py
--rw-r--r--   0        0        0    22954 2023-03-02 16:45:06.507491 rltest-0.6.0/RLTest/redis_std.py
--rw-r--r--   0        0        0     5976 2023-03-02 16:45:06.507491 rltest-0.6.0/RLTest/utils.py
--rw-r--r--   0        0        0     1231 2023-03-02 16:45:07.111495 rltest-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    13236 1970-01-01 00:00:00.000000 rltest-0.6.0/setup.py
--rw-r--r--   0        0        0    13308 1970-01-01 00:00:00.000000 rltest-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1518 2023-05-11 09:39:09.720089 rltest-0.7.0/LICENSE
+-rw-r--r--   0        0        0    12026 2023-05-11 09:39:09.720089 rltest-0.7.0/README.md
+-rw-r--r--   0        0        0     8112 2023-05-11 09:39:09.720089 rltest-0.7.0/RLTest/Enterprise/CcsMock.py
+-rw-r--r--   0        0        0     1835 2023-05-11 09:39:09.720089 rltest-0.7.0/RLTest/Enterprise/Dmc.py
+-rw-r--r--   0        0        0     6393 2023-05-11 09:39:09.720089 rltest-0.7.0/RLTest/Enterprise/EnterpriseClusterEnv.py
+-rw-r--r--   0        0        0       96 2023-05-11 09:39:09.720089 rltest-0.7.0/RLTest/Enterprise/__init__.py
+-rw-r--r--   0        0        0     2705 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/Enterprise/binaryrepo.py
+-rw-r--r--   0        0        0      173 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/__init__.py
+-rw-r--r--   0        0        0    30478 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/__main__.py
+-rw-r--r--   0        0        0      361 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/_version.py
+-rw-r--r--   0        0        0     2398 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/debuggers.py
+-rw-r--r--   0        0        0    22355 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/env.py
+-rw-r--r--   0        0        0     3592 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/exists_redis.py
+-rw-r--r--   0        0        0     5623 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/loader.py
+-rw-r--r--   0        0        0     1620 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/random_port.py
+-rw-r--r--   0        0        0     8030 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/redis_cluster.py
+-rw-r--r--   0        0        0     5245 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/redis_enterprise_cluster.py
+-rw-r--r--   0        0        0    23199 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/redis_std.py
+-rw-r--r--   0        0        0     5976 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/utils.py
+-rw-r--r--   0        0        0     1217 2023-05-11 09:39:10.184093 rltest-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    13238 1970-01-01 00:00:00.000000 rltest-0.7.0/setup.py
+-rw-r--r--   0        0        0    13310 1970-01-01 00:00:00.000000 rltest-0.7.0/PKG-INFO
```

### Comparing `rltest-0.6.0/LICENSE` & `rltest-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rltest-0.6.0/README.md` & `rltest-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `rltest-0.6.0/RLTest/Enterprise/CcsMock.py` & `rltest-0.7.0/RLTest/Enterprise/CcsMock.py`

 * *Files identical despite different names*

### Comparing `rltest-0.6.0/RLTest/Enterprise/Dmc.py` & `rltest-0.7.0/RLTest/Enterprise/Dmc.py`

 * *Files identical despite different names*

### Comparing `rltest-0.6.0/RLTest/Enterprise/EnterpriseClusterEnv.py` & `rltest-0.7.0/RLTest/Enterprise/EnterpriseClusterEnv.py`

 * *Files identical despite different names*

### Comparing `rltest-0.6.0/RLTest/Enterprise/binaryrepo.py` & `rltest-0.7.0/RLTest/Enterprise/binaryrepo.py`

 * *Files identical despite different names*

### Comparing `rltest-0.6.0/RLTest/__main__.py` & `rltest-0.7.0/RLTest/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import print_function
 
 import argparse
+import io
 import os
 import cmd
 import traceback
 import sys
 import shutil
 import inspect
 import unittest
@@ -583,18 +584,19 @@
             Defaults.curr_test_name = testFullName
 
         try:
             # Python < 3.11
             test_args = inspect.getargspec(test.target).args
         except:
             test_args = inspect.getfullargspec(test.target).args
-        
+
         if len(test_args) > 0 and not test.is_method:
             try:
-                env = Env(testName=test.name)
+                # env = Env(testName=test.name)
+                env = Defaults.env_factory(testName=test.name)
             except Exception as e:
                 self.handleFailure(testFullName=testFullName, exception=e, prefix=msgPrefix, testname=test.name)
                 return 0
 
             fn = lambda: test.target(env)
             before_func = (lambda: before(env)) if before is not None else None
             after_func = (lambda: after(env)) if after is not None else None
@@ -670,15 +672,16 @@
     def envScopeGuard(self):
         return EnvScopeGuard(self)
 
     def execute(self):
         Env.RTestInstance = self
         if self.args.env_only:
             Defaults.verbose = 2
-            env = Env(testName='manual test env')
+            # env = Env(testName='manual test env')
+            env = Defaults.env_factory(testName='manual test env')
             if self.args.interactive_debugger:
                 while env.isUp():
                     time.sleep(1)
             else:
                 cmd = MyCmd(env)
                 cmd.cmdloop()
             env.stop()
@@ -782,12 +785,15 @@
         else:
             if self.args.failed_tests_file:
                 with open(self.args.failed_tests_file, 'w') as file:
                     pass
 
 
 def main():
+    # Aviod "UnicodeEncodeError: 'ascii' codec can't encode character" errors
+    sys.stdout = io.open(sys.stdout.fileno(), 'w', encoding='utf8')
+    sys.stderr = io.open(sys.stderr.fileno(), 'w', encoding='utf8')
     RLTest().execute()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `rltest-0.6.0/RLTest/debuggers.py` & `rltest-0.7.0/RLTest/debuggers.py`

 * *Files identical despite different names*

### Comparing `rltest-0.6.0/RLTest/env.py` & `rltest-0.7.0/RLTest/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 
 
 class Defaults:
     module = None
     module_args = None
 
     env = 'oss'
+    env_factory = lambda *args, **kwargs: Env(*args, **kwargs)
     binary = 'redis-server'
     proxy_binary = None
     re_binary = None
     re_libdir = None
     decode_responses = False
     use_aof = False
     use_rdb_preamble = True
@@ -139,14 +140,16 @@
     use_unix = False
     randomize_ports = False
     oss_password = None
     cluster_node_timeout = None
     curr_test_name = None
     port=6379
     enable_debug_command=False
+    terminate_retries=None
+    terminate_retry_secs=None
 
     def getKwargs(self):
         kwargs = {
             'modulePath': self.module,
             'moduleArgs': self.module_args,
             'port': self.port,
             'useSlaves': self.use_slaves,
@@ -159,38 +162,40 @@
             'noLog': self.no_log,
             'verbose': self.verbose,
             'useTLS': self.use_TLS,
             'tlsCertFile': self.tls_cert_file,
             'tlsKeyFile': self.tls_key_file,
             'tlsCaCertFile': self.tls_ca_cert_file,
             'tlsPassphrase': self.tls_passphrase,
-            'password': self.oss_password
+            'password': self.oss_password,
+            'terminateRetries': self.terminate_retries,
+            'terminateRetrySecs': self.terminate_retry_secs,
         }
         return kwargs
 
 
 class Env:
     RTestInstance = None
     EnvCompareParams = ['module', 'moduleArgs', 'env', 'useSlaves', 'shardsCount', 'useAof',
-                        'useRdbPreamble', 'forceTcp', 'enableDebugCommand']
+                        'useRdbPreamble', 'forceTcp', 'enableDebugCommand', 'protocol']
 
     def compareEnvs(self, env):
         if env is None:
             return False
         for param in Env.EnvCompareParams:
             if self.__dict__[param] != env.__dict__[param]:
                 return False
         return True
 
     def __init__(self, testName=None, testDescription=None, module=None,
                  moduleArgs=None, env=None, useSlaves=None, shardsCount=None, decodeResponses=None,
                  useAof=None, useRdbPreamble=None, forceTcp=False, useTLS=False, tlsCertFile=None, tlsKeyFile=None,
                  tlsCaCertFile=None, tlsPassphrase=None, logDir=None, redisBinaryPath=None, dmcBinaryPath=None,
                  redisEnterpriseBinaryPath=None, noDefaultModuleArgs=False, clusterNodeTimeout = None,
-                 freshEnv=False, enableDebugCommand=None):
+                 freshEnv=False, enableDebugCommand=None, protocol=2, terminateRetries=None, terminateRetrySecs=None):
 
         self.testName = testName if testName else Defaults.curr_test_name
         if self.testName is None:
             self.testName = '%s.%s' % (inspect.getmodule(inspect.currentframe().f_back).__name__, inspect.currentframe().f_back.f_code.co_name)
         self.testName = self.testName.replace(' ', '_')
 
         if testDescription:
@@ -220,18 +225,22 @@
 
         self.redisBinaryPath = expandBinary(redisBinaryPath) if redisBinaryPath else Defaults.binary
         self.dmcBinaryPath = expandBinary(dmcBinaryPath) if dmcBinaryPath else Defaults.proxy_binary
         self.redisEnterpriseBinaryPath = expandBinary(redisEnterpriseBinaryPath) if redisEnterpriseBinaryPath else Defaults.re_binary
         self.clusterNodeTimeout = clusterNodeTimeout if clusterNodeTimeout else Defaults.cluster_node_timeout
         self.port = Defaults.port
         self.enableDebugCommand = enableDebugCommand if enableDebugCommand else Defaults.enable_debug_command
+        self.terminateRetries = terminateRetries
+        self.terminateRetrySecs = terminateRetrySecs
+
+        self.protocol = protocol
 
         self.assertionFailedSummary = []
 
-        if (not freshEnv) and Env.RTestInstance and Env.RTestInstance.currEnv and self.compareEnvs(Env.RTestInstance.currEnv):
+        if not freshEnv and Env.RTestInstance and Env.RTestInstance.currEnv and self.compareEnvs(Env.RTestInstance.currEnv):
             self.envRunner = Env.RTestInstance.currEnv.envRunner
         else:
             if Env.RTestInstance and Env.RTestInstance.currEnv:
                 Env.RTestInstance.currEnv.stop()
             self.envRunner = self.getEnvByName()
 
         try:
@@ -320,15 +329,18 @@
             'useTLS': self.useTLS,
             'tlsCertFile': self.tlsCertFile,
             'tlsKeyFile': self.tlsKeyFile,
             'tlsCaCertFile': self.tlsCaCertFile,
             'clusterNodeTimeout': self.clusterNodeTimeout,
             'tlsPassphrase': self.tlsPassphrase,
             'port': self.port,
-            'enableDebugCommand': self.enableDebugCommand
+            'enableDebugCommand': self.enableDebugCommand,
+            'protocol': self.protocol,
+            'terminateRetries': self.terminateRetries,
+            'terminateRetrySecs': self.terminateRetrySecs,
         }
         return kwargs
 
     def start(self, masters = True, slaves = True ):
         self.envRunner.startEnv(masters, slaves)
         self.con = self.getConnection()
```

### Comparing `rltest-0.6.0/RLTest/exists_redis.py` & `rltest-0.7.0/RLTest/exists_redis.py`

 * *Files identical despite different names*

### Comparing `rltest-0.6.0/RLTest/loader.py` & `rltest-0.7.0/RLTest/loader.py`

 * *Files identical despite different names*

### Comparing `rltest-0.6.0/RLTest/random_port.py` & `rltest-0.7.0/RLTest/random_port.py`

 * *Files identical despite different names*

### Comparing `rltest-0.6.0/RLTest/redis_cluster.py` & `rltest-0.7.0/RLTest/redis_cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,17 @@
         self.moduleArgs = kwargs['moduleArgs']
         self.password = kwargs['password']
         self.shardsCount = kwargs.pop('shardsCount')
         useSlaves = kwargs.get('useSlaves', False)
         self.useTLS = kwargs['useTLS']
         self.decodeResponses = kwargs.get('decodeResponses', False)
         self.tlsPassphrase = kwargs.get('tlsPassphrase', None)
+        self.protocol = kwargs.get('protocol', 2)
+        self.terminateRetries = kwargs.get('terminateRetries', None)
+        self.terminateRetrySecs = kwargs.get('terminateRetrySecs', None)
         startPort = kwargs.pop('port', 10000)
         totalRedises = self.shardsCount * (2 if useSlaves else 1)
         randomizePorts = kwargs.pop('randomizePorts', False)
         for i in range(0, totalRedises, (2 if useSlaves else 1)):
             port = 0 if randomizePorts else startPort
             shard = StandardEnv(port=port, serverId=(i + 1),
                                 clusterEnabled=True, **kwargs)
@@ -38,15 +41,14 @@
         if self.moduleArgs:
             print(Colors.Yellow(prefix + '\tmodule args:%s' % self.moduleArgs))
         for i, shard in enumerate(self.shards):
             print(Colors.Yellow(prefix + 'shard: %d' % (i + 1)))
             shard.printEnvData(prefix + '\t')
 
     def waitCluster(self, timeout_sec=40):
-
         st = time.time()
         ok = 0
 
         while st + timeout_sec > time.time():
             ok = 0
             for shard in self.shards:
                 con = shard.getConnection()
@@ -125,20 +127,24 @@
                 ssl_keyfile=self.shards[0].getTLSKeyFile(),
                 ssl_certfile=self.shards[0].getTLSCertFile(),
                 ssl_cert_reqs=None,
                 ssl_ca_certs=self.shards[0].getTLSCACertFile(),
                 ssl_password=self.tlsPassphrase,
                 password=self.password,
                 startup_nodes=statupNode,
-                decode_responses=self.decodeResponses
+                decode_responses=self.decodeResponses,
+                protocol=self.protocol,
+                terminateRetries=self.terminateRetries, terminateRetrySecs=self.terminateRetrySecs
             )
         else:
             return redis.RedisCluster(
                 startup_nodes=statupNode,
-                decode_responses=self.decodeResponses, password=self.password)
+                decode_responses=self.decodeResponses, password=self.password,
+                protocol=self.protocol,
+                terminateRetries=self.terminateRetries, terminateRetrySecs=self.terminateRetrySecs)
 
     def getSlaveConnection(self):
         raise Exception('unsupported')
 
     # List of nodes that initial bootstrapping can be done from
     def getMasterNodesList(self):
         full_master_list = []
```

### Comparing `rltest-0.6.0/RLTest/redis_enterprise_cluster.py` & `rltest-0.7.0/RLTest/redis_enterprise_cluster.py`

 * *Files identical despite different names*

### Comparing `rltest-0.6.0/RLTest/redis_std.py` & `rltest-0.7.0/RLTest/redis_std.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 SLAVE = 'slave'
 
 
 class StandardEnv(object):
     def __init__(self, redisBinaryPath, port=6379, modulePath=None, moduleArgs=None, outputFilesFormat=None,
                  dbDirPath=None, useSlaves=False, serverId=1, password=None, libPath=None, clusterEnabled=False, decodeResponses=False,
                  useAof=False, useRdbPreamble=True, debugger=None, sanitizer=None, noCatch=False, noLog=False, unix=False, verbose=False, useTLS=False,
-                 tlsCertFile=None, tlsKeyFile=None, tlsCaCertFile=None, clusterNodeTimeout=None, tlsPassphrase=None, enableDebugCommand=False):
+                 tlsCertFile=None, tlsKeyFile=None, tlsCaCertFile=None, clusterNodeTimeout=None, tlsPassphrase=None, enableDebugCommand=False, protocol=2,
+                 terminateRetries=None, terminateRetrySecs=None):
         self.uuid = uuid.uuid4().hex
         self.redisBinaryPath = os.path.expanduser(redisBinaryPath) if redisBinaryPath.startswith(
             '~/') else redisBinaryPath
 
         self.modulePath = fix_modules(modulePath)
         self.moduleArgs = fix_modulesArgs(self.modulePath, moduleArgs, haveSeqs=False)
         self.outputFilesFormat = self.uuid + '.' + outputFilesFormat
@@ -53,16 +54,17 @@
         self.useTLS = useTLS
         self.tlsCertFile = tlsCertFile
         self.tlsKeyFile = tlsKeyFile
         self.tlsCaCertFile = tlsCaCertFile
         self.clusterNodeTimeout = clusterNodeTimeout
         self.tlsPassphrase = tlsPassphrase
         self.enableDebugCommand = enableDebugCommand
-        self.terminateRetries = None
-        self.terminateRetrySecs = None
+        self.protocol = protocol
+        self.terminateRetries = terminateRetries
+        self.terminateRetrySecs = terminateRetrySecs
 
         if port > 0:
             self.port = port
             self.slavePort = port + 1 if self.useSlaves else 0
         elif port == 0:
             self.port = get_random_port()
             self.slavePort = get_random_port() if self.useSlaves else 0
@@ -422,29 +424,30 @@
         self.envIsUp = self.masterProcess is not None or self.slaveProcess is not None
         self.envIsHealthy = self.masterProcess is not None and (self.slaveProcess is not None if self.useSlaves else True)
 
 
     def _getConnection(self, role):
         if self.useUnix:
             return redis.StrictRedis(unix_socket_path=self.getUnixPath(role),
-                                     password=self.password, decode_responses=self.decodeResponses)
+                                     password=self.password, decode_responses=self.decodeResponses, protocol=self.protocol)
         elif self.useTLS:
             return redis.StrictRedis('localhost', self.getPort(role),
                                      password=self.password,
                                      ssl=True,
                                      ssl_password=self.tlsPassphrase,
                                      ssl_keyfile=self.getTLSKeyFile(),
                                      ssl_certfile=self.getTLSCertFile(),
                                      ssl_cert_reqs=None,
                                      ssl_ca_certs=self.getTLSCACertFile(),
-                                     decode_responses=self.decodeResponses
+                                     decode_responses=self.decodeResponses,
+                                     protocol=self.protocol
                                      )
         else:
             return redis.StrictRedis('localhost', self.getPort(role),
-                                     password=self.password, decode_responses=self.decodeResponses)
+                                     password=self.password, decode_responses=self.decodeResponses, protocol=self.protocol)
 
     def getConnection(self, shardId=1):
         return self._getConnection(MASTER)
 
     # List containing a connection for each of the master nodes
     def getOSSMasterNodesConnectionList(self):
         return [self.getConnection()]
```

### Comparing `rltest-0.6.0/RLTest/utils.py` & `rltest-0.7.0/RLTest/utils.py`

 * *Files identical despite different names*

### Comparing `rltest-0.6.0/pyproject.toml` & `rltest-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "RLTest"
-version = "0.6.0"
+version = "0.7.0"
 description = "Redis Modules Test Framework, allow to run tests on redis and modules on a variety of environments"
 authors = [ "Redis, Inc. <oss@redis.com>" ]
 license = "BSD-3-Clause"
 readme = "README.md"
 classifiers = [
   "Topic :: Database",
   "Programming Language :: Python",
@@ -20,26 +20,25 @@
 
   [[tool.poetry.packages]]
   include = "RLTest"
 
   [tool.poetry.dependencies]
   python = ">= 3.7.0"
   distro = "^1.5.0"
-  redis = "^4.5.1"
+  redis = "^5.0.0b3"
   psutil = "5.8.0"
   pytest-cov = "2.5"
 
   [tool.poetry.urls]
   repository = "https://github.com/RedisLabsModules/RLTest"
 
   [tool.poetry.scripts]
   RLTest = "RLTest.__main__:main"
 
   [tool.poetry.dev-dependencies]
-  codecov = "*"
   flake8 = "*"
   rmtest = "^0.7.0"
   nose = "^1.3.7"
   ml2rt = "^0.2.0"
   pytest = "^6.0"
 
 [build-system]
```

### Comparing `rltest-0.6.0/setup.py` & `rltest-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['distro>=1.5.0,<2.0.0',
  'psutil==5.8.0',
  'pytest-cov==2.5',
- 'redis>=4.5.1,<5.0.0']
+ 'redis>=5.0.0b3,<6.0.0']
 
 entry_points = \
 {'console_scripts': ['RLTest = RLTest.__main__:main']}
 
 setup_kwargs = {
     'name': 'rltest',
-    'version': '0.6.0',
+    'version': '0.7.0',
     'description': 'Redis Modules Test Framework, allow to run tests on redis and modules on a variety of environments',
     'long_description': '[![license](https://img.shields.io/github/license/RedisLabsModules/RLTest.svg)](https://github.com/RedisLabsModules/RLTest/blob/master/LICENSE)\n[![PyPI version](https://badge.fury.io/py/rltest.svg)](https://badge.fury.io/py/rltest)\n[![CI](https://github.com/RedisLabsModules/RLTest/workflows/CI/badge.svg)](https://github.com/RedisLabsModules/RLTest/actions)\n[![Version](https://img.shields.io/github/release/RedisLabsModules/RLTest.svg)](https://github.com/RedisLabsModules/RLTest/releases/latest)\n[![Codecov](https://codecov.io/gh/RedisLabsModules/RLTest/branch/master/graph/badge.svg)](https://codecov.io/gh/RedisLabsModules/RLTest)\n[![Known Vulnerabilities](https://snyk.io/test/github/RedisLabsModules/RLTest/badge.svg?targetFile=pyproject.toml)](https://snyk.io/test/github/RedisLabsModules/RLTest?targetFile=pyproject.toml)\n\n\n\n# RLTest\n\nRedis Labs Test Framework, allow running tests on redis and modules on a variety of environments.\n\nSupported Environment: oss, oss-cluster, enterprise, enterprise-cluster\n\nThe framework allow you to write a test without environment specification and then run the test on all supported environment.\n\n\n# Install\n```\n$ pip install git+https://github.com/RedisLabsModules/RLTest.git@master\n\n```\n\n# Usage:\n```\n$ RLTest --help\nusage: RLTest [-h] [--version] [--module MODULE] [--module-args MODULE_ARGS]\n              [--env {oss,oss-cluster,enterprise,enterprise-cluster,existing-env,cluster_existing-env}]\n              [--existing-env-addr EXISTING_ENV_ADDR]\n              [--shards_ports SHARDS_PORTS]\n              [--cluster_address CLUSTER_ADDRESS]\n              [--oss_password OSS_PASSWORD]\n              [--cluster_credentials CLUSTER_CREDENTIALS]\n              [--cluster_node_timeout CLUSTER_NODE_TIMEOUT]\n              [--internal_password INTERNAL_PASSWORD]\n              [--oss-redis-path OSS_REDIS_PATH]\n              [--enterprise-redis-path ENTERPRISE_REDIS_PATH]\n              [--stop-on-failure] [-x] [--verbose] [--debug] [-t TEST]\n              [--env-only] [--clear-logs] [--log-dir LOG_DIR] [--use-slaves]\n              [--shards-count SHARDS_COUNT] [--download-enterprise-binaries]\n              [--proxy-binary-path PROXY_BINARY_PATH]\n              [--enterprise-lib-path ENTERPRISE_LIB_PATH] [-r]\n              [--use-aof] [--use-rdb-preamble]\n              [--debug-print] [-V] [--vg-suppressions VG_SUPPRESSIONS]\n              [--vg-options VG_OPTIONS] [--vg-no-leakcheck] [--vg-verbose]\n              [--vg-no-fail-on-errors] [-i] [--debugger DEBUGGER] [-s]\n              [--check-exitcode] [--unix] [--randomize-ports] [--collect-only]\n              [--tls] [--tls-cert-file TLS_CERT_FILE]\n              [--tls-key-file TLS_KEY_FILE]\n              [--tls-ca-cert-file TLS_CA_CERT_FILE]\n\nTest Framework for redis and redis module\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --version             Print RLTest version and exit (default: False)\n  --module MODULE       path to the module file. You can use `--module` more\n                        than once but it imples that you explicitly specify\n                        `--module-args` as well. Notice that on enterprise the\n                        file should be a zip file packed with\n                        [RAMP](https://github.com/RedisLabs/RAMP). (default:\n                        None)\n  --module-args MODULE_ARGS\n                        arguments to give to the module on loading (default:\n                        None)\n  --env {oss,oss-cluster,enterprise,enterprise-cluster,existing-env,cluster_existing-env}, -e {oss,oss-cluster,enterprise,enterprise-cluster,existing-env,cluster_existing-env}\n                        env on which to run the test (default: oss)\n  --existing-env-addr EXISTING_ENV_ADDR\n                        Address of existing env, relevent only when running\n                        with existing-env, cluster_existing-env (default:\n                        localhost:6379)\n  --shards_ports SHARDS_PORTS\n                        list of ports, the shards are listening to, relevent\n                        only when running with cluster_existing-env (default:\n                        None)\n  --cluster_address CLUSTER_ADDRESS\n                        enterprise cluster ip, relevent only when running with\n                        cluster_existing-env (default: None)\n  --oss_password OSS_PASSWORD\n                        set redis password, relevant for oss and oss-cluster\n                        environment (default: None)\n  --cluster_credentials CLUSTER_CREDENTIALS\n                        enterprise cluster cluster_credentials\n                        "username:password", relevent only when running with\n                        cluster_existing-env (default: None)\n  --cluster_node_timeout CLUSTER_NODE_TIMEOUT\n                        cluster node timeout in milliseconds\n  --internal_password INTERNAL_PASSWORD\n                        Give an ability to execute commands on shards\n                        directly, relevent only when running with\n                        cluster_existing-env (default: )\n  --oss-redis-path OSS_REDIS_PATH\n                        path to the oss redis binary (default: redis-server)\n  --enterprise-redis-path ENTERPRISE_REDIS_PATH\n                        path to the entrprise redis binary (default:\n                        ~/.RLTest/opt/redislabs/bin/redis-server)\n  --stop-on-failure     stop running on failure (default: False)\n  -x, --exit-on-failure\n                        Stop test execution and exit on first assertion\n                        failure (default: False)\n  --verbose, -v         print more information about the test (default: 0)\n  --debug               stop before each test allow gdb attachment (default:\n                        False)\n  -t TEST, --test TEST  Specify test to run, in the form of "file:test"\n                        (default: None)\n  --env-only            start the env but do not run any tests (default:\n                        False)\n  --clear-logs          deleting the log direcotry before the execution\n                        (default: False)\n  --log-dir LOG_DIR     directory to write logs to (default: ./logs)\n  --use-slaves          run env with slaves enabled (default: False)\n  --shards-count SHARDS_COUNT\n                        Number shards in bdb (default: 1)\n  --download-enterprise-binaries\n                        run env with slaves enabled (default: False)\n  --proxy-binary-path PROXY_BINARY_PATH\n                        dmc proxy binary path (default:\n                        ~/.RLTest/opt/redislabs/bin/dmcproxy)\n  --enterprise-lib-path ENTERPRISE_LIB_PATH\n                        path of needed libraries to run enterprise binaries\n                        (default: ~/.RLTest/opt/redislabs/lib/)\n  -r, --env-reuse       reuse exists env, this feature is based on best\n                        efforts, if the env can not be reused then it will be\n                        taken down. (default: False)\n  --use-aof             use aof instead of rdb (default: False)\n  --use-rdb-preamble    use rdb preamble when rewriting aof file (default: True)\n  --debug-print         print debug messages (default: False)\n  -V, --vg, --use-valgrind\n                        running redis under valgrind (assuming valgrind is\n                        install on the machine) (default: False)\n  --vg-suppressions VG_SUPPRESSIONS\n                        path valgrind suppressions file (default: None)\n  --vg-options VG_OPTIONS\n                        valgrind [options] (default: None)\n  --vg-no-leakcheck     Don\'t perform a leak check (default: False)\n  --vg-verbose          Don\'t log valgrind output. Output to screen directly\n                        (default: False)\n  --vg-no-fail-on-errors\n                        Dont Fail test when valgrind reported any errors in\n                        the run.By default on RLTest the return value from\n                        Valgrind will be used to fail the tests.Use this\n                        option when you wish to dry-run valgrind but not fail\n                        the test on valgrind reported errors. (default: False)\n  -i, --interactive-debugger\n                        runs the redis on a debuger (gdb/lldb)\n                        interactivly.debugger interactive mode is only\n                        possible on a single process and so unsupported on\n                        cluste or with slaves.it is also not possible to use\n                        valgrind on interactive mode.interactive mode direcly\n                        applies: --no-output-catch and --stop-on-failure.it is\n                        also implies that only one test will be run (if --env-\n                        only was not specify), an error will be raise\n                        otherwise. (default: False)\n  --debugger DEBUGGER   Run specified command line as the debugger (default:\n                        None)\n  -s, --no-output-catch\n                        all output will be written to the stdout, no log\n                        files. (default: False)\n  --check-exitcode      Check redis process exit code (default: False)\n  --unix                Use Unix domain sockets instead of TCP (default:\n                        False)\n  --randomize-ports     Randomize Redis listening port assignment rather\n                        thanusing default port (default: False)\n  --collect-only        Collect the tests and exit (default: False)\n  --tls                 Enable TLS Support and disable the non-TLS port\n                        completely. TLS connections will be available at the\n                        default non-TLS ports. (default: False)\n  --tls-cert-file TLS_CERT_FILE\n                        /path/to/redis.crt (default: None)\n  --tls-key-file TLS_KEY_FILE\n                        /path/to/redis.key (default: None)\n  --tls-ca-cert-file TLS_CA_CERT_FILE\n                        /path/to/ca.crt (default: None)\n\n```\n\n## Sample usages\n\n### Multiple modules\n\n```\nRLTest --module modules/module1.so --module-args \'\' --module modules/module2.so --module-args \'\'\n```\n\n# Configuration File\nBy default, the framework search for configuration file on the current directory. The configuration file name is: config.txt.\nIt is possible to specify different configuration file on command line using the \'@\' prefix, for example:\n```\nRLTest @myConfig.txt # search for myConfig.txt configuration file\n```\nThe configuration file format is the same as the command line argument, i.e : \'--< param_name > < param_val >\'.\n\nIt is also possible to comment a specific lines in the configuration file using \'#\'.\n\nExample:\n\n```\n-vv\n--clear-logs\n#--debug\n```\n\n\n# Test Example\n\n```python\nfrom RLTest import Env\nimport time\n\n\nclass testExample():\n    \'\'\'\n    run all tests on a single env without taking\n    env down between tests\n    \'\'\'\n    def __init__(self):\n        self.env = Env()\n\n    def testExample(self):\n        con = self.env.getConnection()\n        con.set(\'x\', 1)\n        self.env.assertEqual(con.get(\'x\'), \'1\')\n\n    def testExample1(self):\n        con = self.env.getConnection()\n        con.set(\'x\', 1)\n        self.env.assertEqual(con.get(\'x\'), \'1\')\n        self.env.assertFalse(True)  # check failure\n\n    def testExample2(self):\n        con = self.env.getConnection()\n        con.set(\'x\', 1)\n        self.env.assertEqual(con.get(\'x\'), \'1\')\n\n\n# run each test on different env\ndef test_example():\n    env = Env()\n    con = env.getConnection()\n    con.set(\'x\', 1)\n    env.assertEqual(con.get(\'x\'), \'1\')\n\n\ndef test_example_2():\n    env = Env()\n    env.assertOk(env.cmd(\'set\', \'x\', \'1\'))\n    env.expect(\'get\', \'x\').equal(\'1\')\n\n    env.expect(\'lpush\', \'list\', \'1\', \'2\', \'3\').equal(3)\n    env.expect(\'lrange\', \'list\', \'0\', \'-1\').debugPrint().contains(\'1\')\n    env.debugPrint(\'this is some debug printing\')\n\n\ndef test_example_3():\n    env = Env(useSlaves=True, env=\'oss\')\n    con = env.getConnection()\n    con.set(\'x\', 1)\n    con2 = env.getSlaveConnection()\n    time.sleep(0.1)\n    env.assertEqual(con2.get(\'x\'), \'1\')\n\n```\n',
     'author': 'Redis, Inc.',
     'author_email': 'oss@redis.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `rltest-0.6.0/PKG-INFO` & `rltest-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rltest
-Version: 0.6.0
+Version: 0.7.0
 Summary: Redis Modules Test Framework, allow to run tests on redis and modules on a variety of environments
 License: BSD-3-Clause
 Author: Redis, Inc.
 Author-email: oss@redis.com
 Requires-Python: >=3.7.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database
 Requires-Dist: distro (>=1.5.0,<2.0.0)
 Requires-Dist: psutil (==5.8.0)
 Requires-Dist: pytest-cov (==2.5)
-Requires-Dist: redis (>=4.5.1,<5.0.0)
+Requires-Dist: redis (>=5.0.0b3,<6.0.0)
 Project-URL: repository, https://github.com/RedisLabsModules/RLTest
 Description-Content-Type: text/markdown
 
 [![license](https://img.shields.io/github/license/RedisLabsModules/RLTest.svg)](https://github.com/RedisLabsModules/RLTest/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/rltest.svg)](https://badge.fury.io/py/rltest)
 [![CI](https://github.com/RedisLabsModules/RLTest/workflows/CI/badge.svg)](https://github.com/RedisLabsModules/RLTest/actions)
 [![Version](https://img.shields.io/github/release/RedisLabsModules/RLTest.svg)](https://github.com/RedisLabsModules/RLTest/releases/latest)
```

