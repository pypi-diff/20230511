# Comparing `tmp/femtocrux-0.2.5-py3-none-any.whl.zip` & `tmp/femtocrux-0.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,23 @@
-Zip file size: 15113 bytes, number of entries: 18
--rwxr-xr-x  2.0 unx     1389 b- defN 23-Mar-23 23:20 femtocrux/ENV_REQUIREMENTS.sh
--rw-r--r--  2.0 unx      189 b- defN 23-Mar-23 23:20 femtocrux/PY_REQUIREMENTS
--rw-r--r--  2.0 unx        6 b- defN 23-Mar-23 23:20 femtocrux/VERSION
--rw-r--r--  2.0 unx      229 b- defN 23-Mar-23 23:20 femtocrux/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-23 23:20 femtocrux/client/__init__.py
--rw-r--r--  2.0 unx    15598 b- defN 23-Mar-23 23:20 femtocrux/client/client.py
--rw-r--r--  2.0 unx      168 b- defN 23-Mar-23 23:20 femtocrux/grpc/__init__.py
--rw-r--r--  2.0 unx     3776 b- defN 23-Mar-23 23:25 femtocrux/grpc/compiler_service_pb2.py
--rw-r--r--  2.0 unx     6890 b- defN 23-Mar-23 23:25 femtocrux/grpc/compiler_service_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-23 23:20 femtocrux/server/__init__.py
--rw-r--r--  2.0 unx     8603 b- defN 23-Mar-23 23:20 femtocrux/server/server.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-23 23:20 femtocrux/util/__init__.py
--rw-r--r--  2.0 unx     1086 b- defN 23-Mar-23 23:20 femtocrux/util/utils.py
--rw-r--r--  2.0 unx       36 b- defN 23-Mar-23 23:25 femtocrux-0.2.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     2047 b- defN 23-Mar-23 23:25 femtocrux-0.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-23 23:25 femtocrux-0.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Mar-23 23:25 femtocrux-0.2.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1477 b- defN 23-Mar-23 23:25 femtocrux-0.2.5.dist-info/RECORD
-18 files, 41596 bytes uncompressed, 12673 bytes compressed:  69.5%
+Zip file size: 18540 bytes, number of entries: 21
+-rwxr-xr-x  2.0 unx     1389 b- defN 23-May-11 19:50 femtocrux/ENV_REQUIREMENTS.sh
+-rw-r--r--  2.0 unx      308 b- defN 23-May-11 19:50 femtocrux/PY_REQUIREMENTS
+-rw-r--r--  2.0 unx        6 b- defN 23-May-11 19:50 femtocrux/VERSION
+-rw-r--r--  2.0 unx      100 b- defN 23-May-11 19:50 femtocrux/__init__.py
+-rw-r--r--  2.0 unx      162 b- defN 23-May-11 19:50 femtocrux/version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-11 19:50 femtocrux/client/__init__.py
+-rw-r--r--  2.0 unx    21449 b- defN 23-May-11 19:50 femtocrux/client/client.py
+-rw-r--r--  2.0 unx      168 b- defN 23-May-11 19:50 femtocrux/grpc/__init__.py
+-rw-r--r--  2.0 unx     4033 b- defN 23-May-11 19:55 femtocrux/grpc/compiler_service_pb2.py
+-rw-r--r--  2.0 unx     7002 b- defN 23-May-11 19:55 femtocrux/grpc/compiler_service_pb2_grpc.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-11 19:50 femtocrux/server/__init__.py
+-rw-r--r--  2.0 unx      609 b- defN 23-May-11 19:50 femtocrux/server/exceptions.py
+-rw-r--r--  2.0 unx     1606 b- defN 23-May-11 19:50 femtocrux/server/healthcheck.py
+-rw-r--r--  2.0 unx     8620 b- defN 23-May-11 19:50 femtocrux/server/server.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-11 19:50 femtocrux/util/__init__.py
+-rw-r--r--  2.0 unx     1086 b- defN 23-May-11 19:50 femtocrux/util/utils.py
+-rw-r--r--  2.0 unx       36 b- defN 23-May-11 19:55 femtocrux-0.2.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2122 b- defN 23-May-11 19:55 femtocrux-0.2.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-11 19:55 femtocrux-0.2.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-May-11 19:55 femtocrux-0.2.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1727 b- defN 23-May-11 19:55 femtocrux-0.2.8.dist-info/RECORD
+21 files, 50525 bytes uncompressed, 15710 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: femtocrux/VERSION
 Comment: 
 
 Filename: femtocrux/__init__.py
 Comment: 
 
+Filename: femtocrux/version.py
+Comment: 
+
 Filename: femtocrux/client/__init__.py
 Comment: 
 
 Filename: femtocrux/client/client.py
 Comment: 
 
 Filename: femtocrux/grpc/__init__.py
@@ -24,32 +27,38 @@
 
 Filename: femtocrux/grpc/compiler_service_pb2_grpc.py
 Comment: 
 
 Filename: femtocrux/server/__init__.py
 Comment: 
 
+Filename: femtocrux/server/exceptions.py
+Comment: 
+
+Filename: femtocrux/server/healthcheck.py
+Comment: 
+
 Filename: femtocrux/server/server.py
 Comment: 
 
 Filename: femtocrux/util/__init__.py
 Comment: 
 
 Filename: femtocrux/util/utils.py
 Comment: 
 
-Filename: femtocrux-0.2.5.dist-info/LICENSE
+Filename: femtocrux-0.2.8.dist-info/LICENSE
 Comment: 
 
-Filename: femtocrux-0.2.5.dist-info/METADATA
+Filename: femtocrux-0.2.8.dist-info/METADATA
 Comment: 
 
-Filename: femtocrux-0.2.5.dist-info/WHEEL
+Filename: femtocrux-0.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: femtocrux-0.2.5.dist-info/top_level.txt
+Filename: femtocrux-0.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: femtocrux-0.2.5.dist-info/RECORD
+Filename: femtocrux-0.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## femtocrux/PY_REQUIREMENTS

```diff
@@ -2,7 +2,11 @@
 docker
 fmot>=1.3.0.dev0, ==1.*
 grpcio
 grpcio-tools # New proto required somewhere around here
 numpy>=1.18.0
 protobuf # Newer versions don't work with TF 2.11
 passlib
+
+# DOCKER BUG WORK-AROUND https://github.com/docker/docker-py/issues/3113
+requests<2.29.0 
+urllib3 >= 1.26.0, < 2.0.0
```

## femtocrux/VERSION

```diff
@@ -1 +1 @@
-0.2.5
+0.2.8
```

## femtocrux/__init__.py

```diff
@@ -1,7 +1,3 @@
 from .client.client import CompilerClient, TFLiteModel, FQIRModel
+from .version import __version__
 
-def _get_dir():
-    import pathlib
-    return pathlib.Path(__file__).parent.resolve()
-
-__version__ = (_get_dir() / 'VERSION').read_text(encoding='utf-8').strip()
```

## femtocrux/client/client.py

```diff
@@ -1,113 +1,196 @@
 from collections.abc import Iterable
 from dataclasses import dataclass
 import docker
 from enum import Enum
+from getpass import getpass
+import google.protobuf
 import grpc
 import logging
 import numpy as np
 import os
+import platform
 import pickle
 import queue
 import socket
 import sys
-from getpass import getpass
-from typing import Any, List
+import time
+from typing import Any, List, Tuple, Union
 
 from fmot.fqir import GraphProto
-import femtocrux
 
 from femtocrux.util.utils import numpy_to_ndarray, ndarray_to_numpy, get_channel_options
 
 # GRPC artifacts
 import femtocrux.grpc.compiler_service_pb2 as cs_pb2
 import femtocrux.grpc.compiler_service_pb2_grpc as cs_pb2_grpc
 
+# Docker info
+__docker_registry__ = "ghcr.io"
+
+def __get_docker_image_name__() -> str:
+    """
+    Returns the docker image name. For testing, override with the
+    FEMTOCRUX_SERVER_IMAGE_NAME environment variable.
+    """
+    try:
+        return os.environ["FEMTOCRUX_SERVER_IMAGE_NAME"]
+    except KeyError:
+        from femtocrux.version import __version__
+        ORG = "femtosense"
+        IMAGE = "femtocrux"
+        remote_image_name = "%s/%s/%s:%s" % (
+            __docker_registry__, 
+            ORG, 
+            IMAGE, 
+            __version__
+        )
+        return remote_image_name
+
+__docker_image_name__ = __get_docker_image_name__()
+
 # Set up logging
 def __init_logger__():
     """ Init a basic logger to stderr. """
     logger = logging.getLogger(__name__)
     logger.setLevel(logging.INFO)
     formatter = logging.Formatter()
     handler = logging.StreamHandler()
     handler.setFormatter(formatter)
     logger.addHandler(handler)
     return logger
 
 logger = __init_logger__()
 
-def env_var_to_bool(varname: str, default: bool = False) -> bool:
+def __env_var_to_bool__(varname: str, default: bool = False) -> bool:
     """ Parse an environment varaible as a boolean. """
     try:
         value = os.environ[varname]
     except KeyError:
         return default
 
     value_lower = value.lower()
-    if value_lower in ('yes', '1', 'true'):
+    if value_lower in {'yes', '1', 'true'}:
         return True
-    elif value_lower in ('no', '0', 'false'):
+    elif value_lower in {'no', '0', 'false'}:
         return False
     else:
-        raise OSError("Failed to parse environment variable %s: %s" % varname, value)
+        raise OSError("Failed to parse value of environment variable %s: '%s'" % (
+            varname, value
+            )
+        )
 
 class Model:
-    def get_message(self) -> cs_pb2.model:
+    """ 
+    Base class wrapping any model to be compiled by femtocrux. Should not be instantiated directly. Instead, use one of its child classes like :class:`~femtocrux.client.client.FQIRModel` or :class:`~femtocrux.client.client.TFLiteModel`.
+    """
+    def __get_message__(self, options: dict = {}) -> cs_pb2.model:
+        # Format the options
+        options_struct = google.protobuf.struct_pb2.Struct()
+        options_struct.update(options)
+
+        # Construct the model with IR
+        return cs_pb2.model(
+            **{self.__ir_name__: self.__get_ir__()},
+            options = options_struct
+        )
+
+    @property
+    def __ir_name__(self) -> str:
         """
-            Subclass overrides this to implement the model's grpc message.
+            Subclass overrides this to tell which 'ir' field is being returned.
+        """
+        return NotImplementedError("Subclass must override with IR type.")
+
+
+    def __get_ir__(self) -> Tuple[str, Any]:
+        """
+            Subclass overrides this to implement the 'ir' field of the model's 
+            grpc message.
         """
         raise NotImplementedError("Must be defined by subclass")
 
 @dataclass
 class FQIRModel(Model):
+    """
+        Wraps an FQIR model to be compiled by femtocrux.
+
+        :type graph_proto: fmot.fqir.GraphProto, required
+        :param graph_proto: The traced FQIR model.
+
+        :type batch_dim: int, optional
+        :param batch_dim: The batch dimension to be squeezed from all inputs.
+
+        :type sequence_dim: int, optional
+        :param sequence_dim: The sequence dimension to squeezed from all inputs.
+    """
+
     graph_proto: GraphProto = None
     batch_dim: int = None
     sequence_dim: int = None
 
-    def get_message(self) -> cs_pb2.model:
+    @property
+    def __ir_name__(self) -> str:
+        return 'fqir'
+
+    def __get_ir__(self) -> Any:
         # Serialize FQIR via pickle
         model = pickle.dumps(self.graph_proto)
 
         # Send the serialized model
-        return cs_pb2.model(
-            fqir = cs_pb2.fqir(
-                model = model,
-                batch_dim = self.batch_dim,
-                sequence_dim = self.sequence_dim,
-            )
+        return cs_pb2.fqir(
+            model = model,
+            batch_dim = self.batch_dim,
+            sequence_dim = self.sequence_dim,
         )
 
 @dataclass
 class TFLiteModel(Model):
+    """
+        Wraps a TFLite model to be compiled by femtocrux.
+
+        :type flatbuffer: bytes, required
+        :param flatbuffer: The TFLite flatbuffer to be compiled.
+
+        :type signature_name: str, optional
+        :param signature_name: The name of the TFLite IO signature to be used for input / output metadata. Must be provided if the model contains multiple signatures.
+    """
+
     flatbuffer: bytes = None
     signature_name: str = None
 
-    def get_message(self) -> cs_pb2.model:
-        return cs_pb2.model(
-            tflite = cs_pb2.tflite(
-                model = self.flatbuffer,
-                signature_name = self.signature_name
-            )
+    @property
+    def __ir_name__(self) -> str:
+        return 'tflite'
+
+    def __get_ir__(self) -> Any:
+        return cs_pb2.tflite(
+            model = self.flatbuffer,
+            signature_name = self.signature_name
         )
 
 class Simulator():
-    def __init__(self, client: "CompilerClient", model: Model):
+    """
+        Simulates a compiled model's behavior on the SPU.
+    """
+    def __init__(self, client: "CompilerClient", model: Model, 
+        options: dict = {}):
         self.client = client
         self.model = model
 
         # Create an event stream fed by a queue
         self.request_queue = queue.SimpleQueue()
         request_iterator = iter(
             self.request_queue.get, 
             self.__request_sentinel__
         ) 
         self.response_iterator = client.__simulate__(request_iterator)
 
         # Compile the model with the first message
-        model_msg = model.get_message()
+        model_msg = model.__get_message__(options)
         simulation_start_msg = cs_pb2.simulation_input(
             model = model_msg
         )
         self.__send_request__(simulation_start_msg)
 
         # Check compilation status
         self.__get_response__()
@@ -125,22 +208,50 @@
         return response
 
     @property
     def __request_sentinel__(self) -> Any:
         """ Sentinel value to close the request queue. """
         return None
 
-    def simulate(self, inputs: List[np.array], quantize_inputs: bool = False, dequantize_outputs: bool = False, input_period: float = None) -> List[np.array]:
+    def simulate(self, inputs: Union[np.array, Iterable[np.array]], quantize_inputs: bool = False, dequantize_outputs: bool = False, sim_duration: float = None) -> List[np.array]:
+        """ 
+        Simulates the model on the given inputs. 
+
+        :type inputs: array or iterable of arrays, required
+        :param inputs: The input tensors.
+
+        :type quantize_inputs: bool, optional
+        :param quantize_inputs: If true, quantizes each input from float to integer using its scale :math:`a` and zero point :math:`z`, according to the formula
+        .. math::
+            f(x) = a (x - z)
+
+        :type dequantize_outputs: bool, optional
+        :param dequantize_outputs: If true, dequantizes each output from integer to float using its scale :math:`a` and zero point :math:`z`, according to the formula
+        .. math::
+            g(x) = \\frac{x}{a} + z.
+
+        :param sim_duration: The total simulation time, in seconds. Used to estimate static power consumption. For example, in a streaming model, this should be the time elapsed between model invocations. By default, this is just the estimated latency of the model.
+        :type sim_duration: float, optional
+        
+        :rtype: list
+        :return: The output tensors.
+
+        """
         #TODO how to handle multiple inputs? What's the proper form for FASMIR? Map inputs to FASMIR indices as in CompilerFrontend?        
+        # Convert a single ndarray to a list containing that input.
+        # Otherwise, this will be interpreted as an iterable of (n-1)-d arrays 
+        if isinstance(inputs, np.ndarray):
+            inputs = [inputs]
+
         simulation_request = cs_pb2.simulation_input(
             data = cs_pb2.simulation_data(
                 data = [numpy_to_ndarray(x) for x in inputs],
                 quantize_inputs = quantize_inputs,
                 dequantize_outputs = dequantize_outputs,
-                input_period = input_period
+                sim_duration = sim_duration
             )
         )
         self.__send_request__(simulation_request)
         response = self.__get_response__()
 
         return [ndarray_to_numpy(x) for x in response.data], response.report
 
@@ -158,55 +269,79 @@
     def __check_status__(self, status):
         """ Check a status response, raising an exception if unsuccessful. """
         if not status.success:
             raise RuntimeError("Client received error from compiler server:\n%s" % status.msg)
 
     def __check_version__(self):
         """ Verify the server's version matches the client. """
-        client_version = femtocrux.__version__
+        from femtocrux.version import __version__ as client_version
         server_version = self.__server_version__()
         assert client_version == server_version, """
         Client-server version mismatch:
             client: %s
             server: %s
         """ % (client_version, server_version)
 
-    def compile(self, model: Model) -> bytes: 
-        response = self.stub.compile(model.get_message())
+    def compile(self, model: Model, options: dict = {}) -> bytes: 
+        """ 
+        Compile the model to a bitstream. 
+
+        :type model: Model, required
+        :param model: The model to be compiled.
+
+        :type options: dict, optional 
+        :param options: Complier options.
+
+        :rtype: bytes
+        :return: A zip archive of compiler artifacts.
+        """
+        response = self.stub.compile(model.__get_message__(options))
         self.__check_status__(response.status)
         return response.bitfile
 
     def __ping__(self, message: bytes) -> None:
         """ Pings the server with a message. """
         response = self.stub.ping(cs_pb2.data(data=message))
         if response.data != message:
             raise RuntimeError("Server response does not match request data!")
 
     def __simulate__(self, in_stream: Iterable) -> Iterable:
         """ Calls the 'simulator' bidirectional streaming RPC. """
         return self.stub.simulate(in_stream)
 
-    def simulate(self, model: Model) -> Simulator:
-        return Simulator(client = self, model = model)
+    def simulate(self, model: Model, options: dict = {}) -> Simulator:
+        """ 
+        Get a simulator for the model. 
+
+        :type model: Model, required
+        :param model: The model to be simulated.
+
+        :type options: dict, optional
+        :param options: Compiler options.
+
+        :rtype: Simulator
+        :return: A simulator for the model.
+        """
+        return Simulator(client=self, model=model, options=options)
 
     def __server_version__(self) -> str:
         """ Queries the femtocrux version running on the server. """
-        response = self.stub.version(cs_pb2.empty())
+        response = self.stub.version(google.protobuf.empty_pb2.Empty())
         return response.version
 
 class CompilerClient(CompilerClientImpl):
     """
-    User-facing compiler client class.
-    Configures the client and server for production use.
+    Client which spawns and interacts with the compiler server. This is the main entrypoint for femtocrux.
     """
     def __init__(self):
         self.container = None
 
         # Start a new docker server
         self.container = self.__create_docker_server__()
+        self.__wait_for_server_ready__()
         self.__init_channel_info__(self.container)
 
         # Establish a connection to the server
         self.channel = self.__connect__()
 
         # Initialize the client on this channel
         self.stub = cs_pb2_grpc.CompileStub(self.channel)
@@ -228,18 +363,28 @@
 
     def __init_channel_info__(self, container):
         """
         For local connections only.
 
         Gets the IP address and port of the container.
         """
-        self.__channel_port__ = self.container_port
+        self.__channel_port__ = self.__container_port__
+
+        # Platform network defaults
+        sys_name = platform.system()
+        try:
+            network_name = {
+                'Linux': 'bridge',
+                'Darwin': 'bridge',
+                'Windows': 'nat'
+            }[sys_name]
+        except KeyError:
+            raise NotImplementedError("Unsupported platform: %s" % sys_name)
 
         # Get the network info
-        network_name = 'bridge'
         client = self.__get_docker_api_client__()
         network = client.networks.get(network_name)
 
         # Search for this container in the network
         network_containers = network.attrs['Containers']
         try:
             container_info = network_containers[container.id]
@@ -276,50 +421,28 @@
         except grpc.FutureTimeoutError as exc:
             raise OSError("Channel timed out after %s seconds. Check that the server is running." % channel_timeout_seconds) from exc
         logger.info("Connection successful.")
 
         return channel
 
     @property
-    def __docker_registry__(self) -> str:
-        return "ghcr.io"
-
-    @property
-    def __docker_image_name__(self) -> str:
-        """
-        Returns the docker image name. For testing, override with the
-        FEMTOCRUX_SERVER_IMAGE_NAME environment variable.
-        """
-        try:
-            return os.environ["FEMTOCRUX_SERVER_IMAGE_NAME"]
-        except KeyError:
-            ORG = "femtosense"
-            IMAGE = "femtocrux"
-            remote_image_name = "%s/%s/%s:%s" % (
-                self.__docker_registry__, 
-                ORG, 
-                IMAGE, 
-                femtocrux.__version__
-            )
-            return remote_image_name
-
-    @property
     def channel_addr(self) -> str:
+        """ IP address used for the gRPC channel. """
         return self.__channel_addr__
 
     @property
     def channel_port(self) -> int:
         """
-        Port used for the gRPC channel, whether container or local socket.
+        Port used for the gRPC channel.
         """
         return self.__channel_port__
 
     @property
-    def container_port(self) -> int:
-        """ Port used for containers. """
+    def __container_port__(self) -> int:
+        """ Port used inside the container. """
         return 50051
 
     @property
     def __container_label__(self) -> str:
         """ Label attached to identify containers started by this client. """
         return 'femtocrux_server'
 
@@ -346,15 +469,15 @@
         logger.info(
             """
             Attempting to pull docker image from remote.
 
             Alternatively, you can pull the image yourself with the command:
                 docker pull %s
             """, 
-            self.__docker_image_name__
+            __docker_image_name__
         )
   
         # Log in to Github
         client = self.__get_docker_api_client__()
         while True:
             # Get the password
             manual_pass = True
@@ -363,15 +486,15 @@
                 manual_pass = False
             else:
                 # Prompt the user for password entry
                 password = getpass("Please enter your Femtosense-provided key:")
 
             # Log in to the client
             try:
-                resp = client.login("femtodaemon", password, registry="https://" + self.__docker_registry__)
+                resp = client.login("femtodaemon", password, registry="https://" + get_docker_registry())
             except docker.errors.APIError as exc:
                 if 'denied' in exc.explanation:
                     logger.error("Docker authetication failed.")
                     # Retry password entry
                     if manual_pass:
                         continue
 
@@ -383,79 +506,122 @@
 
         def image_not_found_error() -> RuntimeError:
             """ Return an exception saying the image wasn't found. """
             return RuntimeError(
             """Docker image not found:
                 %s
             Please notify your Femtosense representative.""" % (
-                self.__docker_image_name__
+                __docker_image_name__
                 )
             )
 
         # Download the image
         logger.info("Downloading image. This could take a few minutes...")
         try:
-            image = client.images.pull(self.__docker_image_name__)
+            image = client.images.pull(__docker_image_name__)
         except docker.errors.ImageNotFound as exc:
             raise image_not_found_error() from exc
         except docker.errors.APIError as exc:
             if exc.explanation == "manifest unknown":
                 logger.error(
                     "Docker image %s not found on the remote. Check if it is published.", 
-                    self.__docker_image_name__
+                    __docker_image_name__
                 )
             raise image_not_found_error() from exc
 
         logger.info("Download completed.")
 
     def __create_docker_server__(self) -> docker.models.containers.Container:
         """
         Starts the server in a new Docker container.
         """
         # Get a client for the Docker daemon
         client = self.__get_docker_api_client__()
 
         # Pull the image, if not available
         existing_image_names = [tag for image in client.images.list() for tag in image.tags]
-        if self.__docker_image_name__ not in existing_image_names:
+        if __docker_image_name__ not in existing_image_names:
             # Check if we are allowed to pull the image.
             # This is disabled for CI builds.
-            image_not_found_msg = 'Failed to find the docker image %s locally.' % self.__docker_image_name__
-            if not env_var_to_bool("FS_ALLOW_DOCKER_PULL", default=True):
+            image_not_found_msg = 'Failed to find the docker image %s locally.' % __docker_image_name__
+            if not __env_var_to_bool__("FS_ALLOW_DOCKER_PULL", default=True):
                 raise RuntimeError(
                     """
                     %s 
                     Docker pull is disabled by the environment.
                     """ %
                     image_not_found_msg
                 )
 
             # Pull the image from remote
             logger.info(image_not_found_msg)    
             self.__pull_docker_image__()
 
         # Start a container running the server
-        command = "--port %s" % self.container_port
+        command = "--port %s" % self.__container_port__
         container = client.containers.run(
-            self.__docker_image_name__,
+            __docker_image_name__,
             command=command, # Appends entrypoint with args 
             detach=True,
             labels=[self.__container_label__],
             stderr=True,
             stdout=True,
             name=self.__get_unused_container_name__(),
             auto_remove=True,
         )
 
-        # Check if the container is running
-        try:
-            top = container.top()
-        except:
-            raise RuntimeError("Failed to start docker container (status: %s)" % container.status)
-        assert len(top['Processes']) > 0, "Docker container is idle"
-
         return container
 
+    def __wait_for_server_ready__(self):
+        """
+        Block until the Docker container is ready to handle requests.
+        """
+
+        container = self.container
+
+        # Block until the container starts
+        num_attempts = 5
+        wait_interval = 1.0 # Seconds
+        print('Checking container status...')
+        for attempt in range(num_attempts):
+            container.reload()
+            status = container.status
+            if status == 'created':
+                # Sleep and try again
+                print('Container starting up. Retrying in %fs...' % wait_interval)
+                time.sleep(wait_interval)
+                continue
+            elif status == 'running':
+                print('Container started successfully.')
+                break
+            elif status == 'exited':
+                raise RuntimeError("Container exited! See logs:\n%d" % container.logs())
+            else:
+                raise RuntimeError("Unrecognized docker container status: %d" % status)
+
+        # Check the final status
+        container.reload()
+        if container.status != 'running':
+            raise RuntimeError("Container failed to start after %d attempts" % num_attempts)
+
+        # Check the container's health
+        for attempt in range(num_attempts):
+            exit_code, output = container.exec_run('python3 /femtocrux/femtocrux/server/healthcheck.py')
+
+            if exit_code == 0:
+                print('Container passed health check.')
+                break
+
+            time.sleep(wait_interval)
+
+        # Check the last return code
+        if exit_code != 0:
+            raise RuntimeError(
+                "Docker container failed %d health check(s)!\nLast output:\n%s" % (
+                    num_attempts, output.decode('utf-8')
+                )
+            )
+
 if __name__ == "__main__":
     logging.basicConfig(stream=sys.stdout, level=logging.INFO)
     client = CompilerClient()
     logger.info('Client started successfully.')
```

## femtocrux/grpc/compiler_service_pb2.py

```diff
@@ -7,43 +7,43 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x63ompiler_service.proto\x12\nfscompiler\"g\n\x04\x66qir\x12\r\n\x05model\x18\x01 \x01(\x0c\x12\x16\n\tbatch_dim\x18\x02 \x01(\x03H\x00\x88\x01\x01\x12\x19\n\x0csequence_dim\x18\x03 \x01(\x03H\x01\x88\x01\x01\x42\x0c\n\n_batch_dimB\x0f\n\r_sequence_dim\"G\n\x06tflite\x12\r\n\x05model\x18\x01 \x01(\x0c\x12\x1b\n\x0esignature_name\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x11\n\x0f_signature_name\"U\n\x05model\x12 \n\x04\x66qir\x18\x01 \x01(\x0b\x32\x10.fscompiler.fqirH\x00\x12$\n\x06tflite\x18\x02 \x01(\x0b\x32\x12.fscompiler.tfliteH\x00\x42\x04\n\x02ir\"&\n\x06status\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x0b\n\x03msg\x18\x02 \x01(\t\"I\n\x12\x63ompiled_artifacts\x12\x0f\n\x07\x62itfile\x18\x01 \x01(\x0c\x12\"\n\x06status\x18\x02 \x01(\x0b\x32\x12.fscompiler.status\"&\n\x07ndarray\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x02\x12\r\n\x05shape\x18\x02 \x03(\x03\"\x14\n\x04\x64\x61ta\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"\x07\n\x05\x65mpty\"\x95\x01\n\x0fsimulation_data\x12!\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x13.fscompiler.ndarray\x12\x17\n\x0fquantize_inputs\x18\x02 \x01(\x08\x12\x1a\n\x12\x64\x65quantize_outputs\x18\x03 \x01(\x08\x12\x19\n\x0cinput_period\x18\x04 \x01(\x02H\x00\x88\x01\x01\x42\x0f\n\r_input_period\"t\n\x10simulation_input\x12\"\n\x05model\x18\x01 \x01(\x0b\x32\x11.fscompiler.modelH\x00\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.fscompiler.simulation_dataH\x00\x42\x0f\n\rmodel_or_data\"j\n\x11simulation_output\x12!\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x13.fscompiler.ndarray\x12\x0e\n\x06report\x18\x02 \x01(\t\x12\"\n\x06status\x18\x03 \x01(\x0b\x32\x12.fscompiler.status\"\x1f\n\x0cversion_info\x12\x0f\n\x07version\x18\x01 \x01(\t2\x80\x02\n\x07\x43ompile\x12>\n\x07\x63ompile\x12\x11.fscompiler.model\x1a\x1e.fscompiler.compiled_artifacts\"\x00\x12,\n\x04ping\x12\x10.fscompiler.data\x1a\x10.fscompiler.data\"\x00\x12M\n\x08simulate\x12\x1c.fscompiler.simulation_input\x1a\x1d.fscompiler.simulation_output\"\x00(\x01\x30\x01\x12\x38\n\x07version\x12\x11.fscompiler.empty\x1a\x18.fscompiler.version_info\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x63ompiler_service.proto\x12\nfscompiler\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\"g\n\x04\x66qir\x12\r\n\x05model\x18\x01 \x01(\x0c\x12\x16\n\tbatch_dim\x18\x02 \x01(\x03H\x00\x88\x01\x01\x12\x19\n\x0csequence_dim\x18\x03 \x01(\x03H\x01\x88\x01\x01\x42\x0c\n\n_batch_dimB\x0f\n\r_sequence_dim\"G\n\x06tflite\x12\r\n\x05model\x18\x01 \x01(\x0c\x12\x1b\n\x0esignature_name\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x11\n\x0f_signature_name\"\x90\x01\n\x05model\x12 \n\x04\x66qir\x18\x01 \x01(\x0b\x32\x10.fscompiler.fqirH\x00\x12$\n\x06tflite\x18\x02 \x01(\x0b\x32\x12.fscompiler.tfliteH\x00\x12-\n\x07options\x18\x03 \x01(\x0b\x32\x17.google.protobuf.StructH\x01\x88\x01\x01\x42\x04\n\x02irB\n\n\x08_options\"&\n\x06status\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x0b\n\x03msg\x18\x02 \x01(\t\"I\n\x12\x63ompiled_artifacts\x12\x0f\n\x07\x62itfile\x18\x01 \x01(\x0c\x12\"\n\x06status\x18\x02 \x01(\x0b\x32\x12.fscompiler.status\"&\n\x07ndarray\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x02\x12\r\n\x05shape\x18\x02 \x03(\x03\"\x14\n\x04\x64\x61ta\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"\x95\x01\n\x0fsimulation_data\x12!\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x13.fscompiler.ndarray\x12\x17\n\x0fquantize_inputs\x18\x02 \x01(\x08\x12\x1a\n\x12\x64\x65quantize_outputs\x18\x03 \x01(\x08\x12\x19\n\x0csim_duration\x18\x04 \x01(\x02H\x00\x88\x01\x01\x42\x0f\n\r_sim_duration\"t\n\x10simulation_input\x12\"\n\x05model\x18\x01 \x01(\x0b\x32\x11.fscompiler.modelH\x00\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.fscompiler.simulation_dataH\x00\x42\x0f\n\rmodel_or_data\"j\n\x11simulation_output\x12!\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x13.fscompiler.ndarray\x12\x0e\n\x06report\x18\x02 \x01(\t\x12\"\n\x06status\x18\x03 \x01(\x0b\x32\x12.fscompiler.status\"\x1f\n\x0cversion_info\x12\x0f\n\x07version\x18\x01 \x01(\t2\x85\x02\n\x07\x43ompile\x12>\n\x07\x63ompile\x12\x11.fscompiler.model\x1a\x1e.fscompiler.compiled_artifacts\"\x00\x12,\n\x04ping\x12\x10.fscompiler.data\x1a\x10.fscompiler.data\"\x00\x12M\n\x08simulate\x12\x1c.fscompiler.simulation_input\x1a\x1d.fscompiler.simulation_output\"\x00(\x01\x30\x01\x12=\n\x07version\x12\x16.google.protobuf.Empty\x1a\x18.fscompiler.version_info\"\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'compiler_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _FQIR._serialized_start=38
-  _FQIR._serialized_end=141
-  _TFLITE._serialized_start=143
-  _TFLITE._serialized_end=214
-  _MODEL._serialized_start=216
-  _MODEL._serialized_end=301
-  _STATUS._serialized_start=303
-  _STATUS._serialized_end=341
-  _COMPILED_ARTIFACTS._serialized_start=343
-  _COMPILED_ARTIFACTS._serialized_end=416
-  _NDARRAY._serialized_start=418
-  _NDARRAY._serialized_end=456
-  _DATA._serialized_start=458
-  _DATA._serialized_end=478
-  _EMPTY._serialized_start=480
-  _EMPTY._serialized_end=487
-  _SIMULATION_DATA._serialized_start=490
-  _SIMULATION_DATA._serialized_end=639
-  _SIMULATION_INPUT._serialized_start=641
-  _SIMULATION_INPUT._serialized_end=757
-  _SIMULATION_OUTPUT._serialized_start=759
-  _SIMULATION_OUTPUT._serialized_end=865
-  _VERSION_INFO._serialized_start=867
-  _VERSION_INFO._serialized_end=898
-  _COMPILE._serialized_start=901
-  _COMPILE._serialized_end=1157
+  _FQIR._serialized_start=97
+  _FQIR._serialized_end=200
+  _TFLITE._serialized_start=202
+  _TFLITE._serialized_end=273
+  _MODEL._serialized_start=276
+  _MODEL._serialized_end=420
+  _STATUS._serialized_start=422
+  _STATUS._serialized_end=460
+  _COMPILED_ARTIFACTS._serialized_start=462
+  _COMPILED_ARTIFACTS._serialized_end=535
+  _NDARRAY._serialized_start=537
+  _NDARRAY._serialized_end=575
+  _DATA._serialized_start=577
+  _DATA._serialized_end=597
+  _SIMULATION_DATA._serialized_start=600
+  _SIMULATION_DATA._serialized_end=749
+  _SIMULATION_INPUT._serialized_start=751
+  _SIMULATION_INPUT._serialized_end=867
+  _SIMULATION_OUTPUT._serialized_start=869
+  _SIMULATION_OUTPUT._serialized_end=975
+  _VERSION_INFO._serialized_start=977
+  _VERSION_INFO._serialized_end=1008
+  _COMPILE._serialized_start=1011
+  _COMPILE._serialized_end=1272
 # @@protoc_insertion_point(module_scope)
```

## femtocrux/grpc/compiler_service_pb2_grpc.py

```diff
@@ -1,12 +1,13 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 import compiler_service_pb2 as compiler__service__pb2
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
 class CompileStub(object):
     """Compiler service
     """
 
     def __init__(self, channel):
@@ -28,15 +29,15 @@
         self.simulate = channel.stream_stream(
                 '/fscompiler.Compile/simulate',
                 request_serializer=compiler__service__pb2.simulation_input.SerializeToString,
                 response_deserializer=compiler__service__pb2.simulation_output.FromString,
                 )
         self.version = channel.unary_unary(
                 '/fscompiler.Compile/version',
-                request_serializer=compiler__service__pb2.empty.SerializeToString,
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
                 response_deserializer=compiler__service__pb2.version_info.FromString,
                 )
 
 
 class CompileServicer(object):
     """Compiler service
     """
@@ -81,15 +82,15 @@
             'simulate': grpc.stream_stream_rpc_method_handler(
                     servicer.simulate,
                     request_deserializer=compiler__service__pb2.simulation_input.FromString,
                     response_serializer=compiler__service__pb2.simulation_output.SerializeToString,
             ),
             'version': grpc.unary_unary_rpc_method_handler(
                     servicer.version,
-                    request_deserializer=compiler__service__pb2.empty.FromString,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                     response_serializer=compiler__service__pb2.version_info.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'fscompiler.Compile', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
@@ -158,11 +159,11 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/fscompiler.Compile/version',
-            compiler__service__pb2.empty.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             compiler__service__pb2.version_info.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

## femtocrux/server/server.py

```diff
@@ -1,30 +1,32 @@
 import argparse
 from collections.abc import Iterable
 import concurrent 
+import google.protobuf
 import grpc
-import io
 import logging
 import pickle
 import sys
-import traceback
 from typing import Dict
 
 from femtostack.common import CompilerFrontend, SimIOWrapper, IOConfig
 from femtostack.tflite_api.tflite_frontend import TFLiteCompiler
 from femtostack.torch_api.frontend import TorchCompiler
 from fmot.fqir import GraphProto
 
-import femtocrux
+from femtocrux.server.exceptions import format_exception, format_exception_from_exc
 from femtocrux.util.utils import numpy_to_ndarray, ndarray_to_numpy, field_or_none, get_channel_options
 
 # Import GRPC artifacts
 import femtocrux.grpc.compiler_service_pb2 as cs_pb2
 import femtocrux.grpc.compiler_service_pb2_grpc as cs_pb2_grpc
 
+# Network parameters
+default_port = "50051"
+
 class CompileServicer(cs_pb2_grpc.CompileServicer):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # Initialize the log
         self.logger = logging.getLogger("CompileServicer")
         self.logger.setLevel(logging.DEBUG)
@@ -37,49 +39,59 @@
         graph_proto = pickle.loads(fqir.model)
 
 
         # Compile the FQIR
         return TorchCompiler(
             graph_proto, 
             batch_dim=field_or_none(fqir, 'batch_dim'),
-            sequence_dim=field_or_none(fqir, 'sequence_dim')
+            seq_dim=field_or_none(fqir, 'sequence_dim')
         )
 
     def __get_tflite_compiler__(self, model: cs_pb2.model) -> CompilerFrontend:
         """ Get a TFLite compiler from a model message """
         tflite = model.tflite
         return TFLiteCompiler(
             tflite.model, 
             signature=field_or_none(tflite, 'signature_name') 
         )
 
     def __compile_model__(self, model: cs_pb2.model, context) -> CompilerFrontend:
         """ Compile a model, for simulation or bitfile generation. """
+        # Get a compiler for the model
         model_type_map = {
             'fqir': self.__get_fqir_compiler__,
             'tflite': self.__get_tflite_compiler__
         }
-        model_type = model.WhichOneof("ir")
+        model_type = model.WhichOneof('ir')
         compiler = model_type_map[model_type](model)
-        compiler.compile() 
+
+        # Get the compiler options
+        options_struct = field_or_none(model, 'options')
+        if options_struct is None:
+            options = {}
+        else: 
+            options = google.protobuf.json_format.MessageToDict(options_struct)
+
+        # Compile the model
+        compiler.compile(options = options) 
         assert compiler.is_compiled, "Expected compilation completed"
         return compiler
 
     def compile(self, model, context):
         """ Compile a model into a bitfile. """
 
         self.logger.debug('Received \'compile\' request.')
 
         # Compile the model
         try:
             compiler = self.__compile_model__(model, context)
             bitfile = compiler.dump_bitfile(encrypt=True)
         except Exception as exc:
             msg = "Compiler raised exception:\n%s" % (
-                format_exception(type(exc), exc, exc.__traceback__)
+                format_exception_from_exc(exc)
             )
             self.logger.error(msg)
             return cs_pb2.compiled_artifacts( 
                 status = cs_pb2.status(
                     success=False, 
                     msg=msg
                 )
@@ -117,15 +129,15 @@
                 continue
 
             # Attempt compilation
             try:
                 compiler = self.__compile_model__(model_request.model, context)
             except Exception as exc:
                 msg = "Compiler raised exception:\n%s" % (
-                    format_exception(type(exc), exc, exc.__traceback__)
+                    format_exception_from_exc(exc)
                 )
                 self.logger.error(msg)
                 yield cs_pb2.simulation_output( 
                     status = cs_pb2.status(
                         success=False, 
                         msg=msg
                     )
@@ -155,27 +167,27 @@
 
             # Convert input data
             sim_data = data_request.data
             data = [ndarray_to_numpy(x) for x in sim_data.data]
             assert len(data) == 1, "Behavioral sim currently only supports 1 input" #FIXME
             data = data[0]
     
-            input_period = None if sim_data.input_period == -1 else sim_data.input_period
+            sim_duration = None if sim_data.sim_duration == -1 else sim_data.sim_duration
 
             # Simulate the model
             try:
                 outputs, metrics = compiler.run_behavioral_simulator(
                     data,
                     quantize_inputs = sim_data.quantize_inputs,
                     dequantize_outputs = sim_data.dequantize_outputs,
-                    input_period = field_or_none(sim_data, 'input_period')
+                    input_period = field_or_none(sim_data, 'sim_duration')
                 )
             except Exception as exc:
                 msg = "Simulator raised exception:\n%s" % (
-                    format_exception(type(exc), exc, exc.__traceback__)
+                    format_exception_from_exc(exc)
                 )
                 self.logger.error(msg)
                 yield cs_pb2.simulation_output(
                     status = cs_pb2.status(
                         success = False,
                         msg = msg
                     )
@@ -187,29 +199,16 @@
                 data = [numpy_to_ndarray(x) for x in outputs],
                 report = metrics.performance_report(),
                 status = cs_pb2.status(success=True)
             )
 
     def version(self, empty, context) -> cs_pb2.version_info:
         """ Return the version of femtocrux running in this server. """
-        return cs_pb2.version_info(version = femtocrux.__version__)
-
-def format_exception(type, value, tb) -> str:
-    """Prints an exception with its traceback."""
-    # Format the exception
-    msg = ""
-    msg += "\t%s: %s\n" % (type, str(value))
-
-    # Format the traceback
-    file_like = io.StringIO(newline='\n')
-    traceback.print_tb(tb, file=file_like)
-    msg += "Traceback:\n"
-    msg += file_like.getvalue()
-
-    return msg
+        from femtocrux.version import __version__
+        return cs_pb2.version_info(version = __version__)
 
 def handle_exception(type, value, tb):
     """Log an uncaught exception before terminating."""
     logger.error("Server raised uncaught exception:\n")
     logger.error(format_exception(type, value, tb))
 
     # Call the default excepthook to terminate the progarm
@@ -221,15 +220,14 @@
     """
     # Set up logs
     logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
     sys.excepthook = handle_exception
 
     # Parse arguments
     parser = argparse.ArgumentParser(description='Configures the gRPC server.')
-    default_port = "50051"
     parser.add_argument(
         '--port', 
         dest="port", 
         default=default_port,
         help="the port used for RPCs (default: %s)" % default_port
     )
     args = parser.parse_args()
```

## Comparing `femtocrux-0.2.5.dist-info/METADATA` & `femtocrux-0.2.8.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femtocrux
-Version: 0.2.5
+Version: 0.2.8
 Summary: Femtosense Compiler
 Home-page: https://github.com/femtosense/femtocrux
 Author: Femtosense
 Author-email: info@femtosense.ai
 Project-URL: Source, https://github.com/femtosense/femtocrux
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,14 +18,16 @@
 Requires-Dist: docker
 Requires-Dist: fmot (==1.*,>=1.3.0.dev0)
 Requires-Dist: grpcio
 Requires-Dist: grpcio-tools
 Requires-Dist: numpy (>=1.18.0)
 Requires-Dist: protobuf
 Requires-Dist: passlib
+Requires-Dist: requests (<2.29.0)
+Requires-Dist: urllib3 (<2.0.0,>=1.26.0)
 
 ![Build Status](https://codebuild.us-west-2.amazonaws.com/badges?uuid=eyJlbmNyeXB0ZWREYXRhIjoiRGpDOFpEOXF1M0prSy9OOVNkZ3F2NkRKM0NNMG8xbmpZU0hZdUp1ejhHOEswdDRhOEZOakMrdWZyaHp1WGVtQ1lVTStzRUpXaFlYeFZPSEJFd21NdjF3PSIsIml2UGFyYW1ldGVyU3BlYyI6InJZYzhuZ3d3a1FUUzBzM0kiLCJtYXRlcmlhbFNldFNlcmlhbCI6MX0%3D&branch=master)
 
 # femtocrux
 
 Compiler API for the Femotsense Sparse Processing Unit (SPU).
```

## Comparing `femtocrux-0.2.5.dist-info/RECORD` & `femtocrux-0.2.8.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 femtocrux/ENV_REQUIREMENTS.sh,sha256=t_O1B4hJAMgxvH9gwp1qls6eVFmhSYBJe64KmuK_H-4,1389
-femtocrux/PY_REQUIREMENTS,sha256=9c2LJjrKSdz0U3vQdv_2OIX3ZtuDvOTonZOQy7M8Xr8,189
-femtocrux/VERSION,sha256=6Vn3UOktu3YUriislvCjcnLK7YHYu7dYeRr3v7thBqA,6
-femtocrux/__init__.py,sha256=FBF3lsVKS8SbD30aUoKFHbY3lo18vJiYDpMfkqoR2K4,229
+femtocrux/PY_REQUIREMENTS,sha256=dwSA37UvBVgyXrAr-ToLV_eJIaVTgf7cnUClX0mn4rE,308
+femtocrux/VERSION,sha256=KDVx0mQvx7O-_SlPRdU7iWodVNNMhiNbExURkrOAYGo,6
+femtocrux/__init__.py,sha256=FISQ-uQRzWFQsUVQ65YrAzS5nFz5kHZahrWzbLegA3U,100
+femtocrux/version.py,sha256=h9UchNl62V-tKFPlf2uyeVqvUBFaSi9yhH15PDy-NaQ,162
 femtocrux/client/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-femtocrux/client/client.py,sha256=uOIagzLiqMadynyxIjRDMPCEd3bmOyhHcSw39NPaOs8,15598
+femtocrux/client/client.py,sha256=JUpZZVSYpmLDZcyw-s0ugT0LDvXmyi-CUXbcgrziDzo,21449
 femtocrux/grpc/__init__.py,sha256=1otI5-T4OaWs68wSUMtwe5IXLAM02Z4hZjIW8kGAVzo,168
-femtocrux/grpc/compiler_service_pb2.py,sha256=WD2YFjDeD0mO6_-8qklscfazuoGnXBD3k-9hn5-JoEg,3776
-femtocrux/grpc/compiler_service_pb2_grpc.py,sha256=vuHSjSMZ2c4RXPOm4bmpt6B5igbvRGtgCz5vMzPpjeU,6890
+femtocrux/grpc/compiler_service_pb2.py,sha256=VIki-K3gP1OdM94tCkbIyJXd2VesdC2y3Mwwssb1QSk,4033
+femtocrux/grpc/compiler_service_pb2_grpc.py,sha256=L9EQFYMFVACngUrAEmSJDgUTSPSi3rDoG7TERg-pFq4,7002
 femtocrux/server/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-femtocrux/server/server.py,sha256=nVc2aLpUn1YxNwKP1aIvz-t-0upOF3DFUmZQxk61gb8,8603
+femtocrux/server/exceptions.py,sha256=Kc6HMDRfebZ1k-d_Ij_BDHZO7QgvXnzEqqgO36oM-kc,609
+femtocrux/server/healthcheck.py,sha256=mzQ_-u8xsc4VcelkvsbDTtJgdSlTBTJrDJ8mQkaGuqA,1606
+femtocrux/server/server.py,sha256=eQSDHXz-A0ucylfvti1CeC1BHRM640gKVbpiEC-O1to,8620
 femtocrux/util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 femtocrux/util/utils.py,sha256=LVgC8nBx4x8GtndFMyczwQojSEVmLpzDieipZb9IPD4,1086
-femtocrux-0.2.5.dist-info/LICENSE,sha256=eN9ZI1xHjUmFvN3TEeop5kBGXRUBfbsl55KBNBYYFqI,36
-femtocrux-0.2.5.dist-info/METADATA,sha256=3FNiPNw8jidXujgOjjtKzB4mxJfuq4u1DZSjbj_NSqU,2047
-femtocrux-0.2.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-femtocrux-0.2.5.dist-info/top_level.txt,sha256=BkTttlioC3je__8577wxRieZqY3Abu7FOOdMnmYbcNI,10
-femtocrux-0.2.5.dist-info/RECORD,,
+femtocrux-0.2.8.dist-info/LICENSE,sha256=eN9ZI1xHjUmFvN3TEeop5kBGXRUBfbsl55KBNBYYFqI,36
+femtocrux-0.2.8.dist-info/METADATA,sha256=nzlqkURhbYQ0KjcPg48qfDbckwTcK_E57jzyu7650C0,2122
+femtocrux-0.2.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+femtocrux-0.2.8.dist-info/top_level.txt,sha256=BkTttlioC3je__8577wxRieZqY3Abu7FOOdMnmYbcNI,10
+femtocrux-0.2.8.dist-info/RECORD,,
```

