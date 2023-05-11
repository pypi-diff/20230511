# Comparing `tmp/rabbie-0.0.4.tar.gz` & `tmp/rabbie-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbie-0.0.4.tar", last modified: Thu Apr 27 19:31:56 2023, max compression
+gzip compressed data, was "rabbie-0.0.5.tar", last modified: Thu May 11 11:20:01 2023, max compression
```

## Comparing `rabbie-0.0.4.tar` & `rabbie-0.0.5.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.749215 rabbie-0.0.4/
--rw-rw-rw-   0        0        0     1077 2023-04-24 20:01:12.000000 rabbie-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     7998 2023-04-27 19:31:56.748216 rabbie-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     7522 2023-04-27 19:19:55.000000 rabbie-0.0.4/README.md
--rw-rw-rw-   0        0        0       63 2023-04-02 21:06:34.000000 rabbie-0.0.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.696215 rabbie-0.0.4/rabbie/
--rw-rw-rw-   0        0        0      230 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.715215 rabbie-0.0.4/rabbie/broker_types/
--rw-rw-rw-   0        0        0       60 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/broker_types/__init__.py
--rw-rw-rw-   0        0        0     4632 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/broker_types/channel.py
--rw-rw-rw-   0        0        0      182 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/broker_types/relayed_types.py
-drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.717215 rabbie-0.0.4/rabbie/connection/
--rw-rw-rw-   0        0        0       44 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/connection/__init__.py
--rw-rw-rw-   0        0        0      294 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/connection/details.py
-drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.720218 rabbie-0.0.4/rabbie/consumer/
--rw-rw-rw-   0        0        0      175 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/consumer/__init__.py
--rw-rw-rw-   0        0        0     6274 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/consumer/consumer.py
-drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.724215 rabbie-0.0.4/rabbie/consumer/listener/
--rw-rw-rw-   0        0        0       79 2023-04-24 20:01:12.000000 rabbie-0.0.4/rabbie/consumer/listener/__init__.py
--rw-rw-rw-   0        0        0     5214 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/consumer/listener/listener.py
--rw-rw-rw-   0        0        0      400 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/consumer/listener/listener_details.py
--rw-rw-rw-   0        0        0     3057 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/consumer/microconsumer.py
-drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.726218 rabbie-0.0.4/rabbie/decoder/
--rw-rw-rw-   0        0        0       65 2023-04-24 20:01:12.000000 rabbie-0.0.4/rabbie/decoder/__init__.py
--rw-rw-rw-   0        0        0      132 2023-04-24 20:01:12.000000 rabbie-0.0.4/rabbie/decoder/decoder.py
-drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.728219 rabbie-0.0.4/rabbie/decoder/decoders/
--rw-rw-rw-   0        0        0       39 2023-04-24 20:01:12.000000 rabbie-0.0.4/rabbie/decoder/decoders/__init__.py
--rw-rw-rw-   0        0        0      148 2023-04-24 20:01:12.000000 rabbie-0.0.4/rabbie/decoder/decoders/json_decoder.py
-drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.730215 rabbie-0.0.4/rabbie/decoder/exceptions/
--rw-rw-rw-   0        0        0       94 2023-03-29 12:21:12.000000 rabbie-0.0.4/rabbie/decoder/exceptions/__init__.py
--rw-rw-rw-   0        0        0       44 2023-03-29 12:19:53.000000 rabbie-0.0.4/rabbie/decoder/exceptions/decode_exception.py
-drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.732216 rabbie-0.0.4/rabbie/encoder/
--rw-rw-rw-   0        0        0       65 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/encoder/__init__.py
--rw-rw-rw-   0        0        0      197 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/encoder/encoder.py
-drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.734214 rabbie-0.0.4/rabbie/encoder/encoders/
--rw-rw-rw-   0        0        0       39 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/encoder/encoders/__init__.py
--rw-rw-rw-   0        0        0      215 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/encoder/encoders/json_encoder.py
-drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.735215 rabbie-0.0.4/rabbie/logger/
--rw-rw-rw-   0        0        0      312 2023-04-24 20:01:12.000000 rabbie-0.0.4/rabbie/logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.738215 rabbie-0.0.4/rabbie/producer/
--rw-rw-rw-   0        0        0       46 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/producer/__init__.py
--rw-rw-rw-   0        0        0     2923 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/producer/producer.py
-drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.740245 rabbie-0.0.4/rabbie/producer/publisher/
--rw-rw-rw-   0        0        0       34 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/producer/publisher/__init__.py
--rw-rw-rw-   0        0        0     3176 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/producer/publisher/publisher.py
-drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.742215 rabbie-0.0.4/rabbie/supervisor/
--rw-rw-rw-   0        0        0       50 2023-04-24 20:01:12.000000 rabbie-0.0.4/rabbie/supervisor/__init__.py
--rw-rw-rw-   0        0        0     4560 2023-04-24 20:01:12.000000 rabbie-0.0.4/rabbie/supervisor/supervisor.py
-drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.711215 rabbie-0.0.4/rabbie.egg-info/
--rw-rw-rw-   0        0        0     7998 2023-04-27 19:31:56.000000 rabbie-0.0.4/rabbie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1258 2023-04-27 19:31:56.000000 rabbie-0.0.4/rabbie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 19:31:56.000000 rabbie-0.0.4/rabbie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-27 19:31:56.000000 rabbie-0.0.4/rabbie.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 19:31:56.000000 rabbie-0.0.4/rabbie.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 19:31:56.749215 rabbie-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      854 2023-04-27 19:19:55.000000 rabbie-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.747218 rabbie-0.0.4/tests/
--rw-rw-rw-   0        0        0     4748 2023-04-27 19:19:55.000000 rabbie-0.0.4/tests/test_consumer.py
--rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.4/tests/test_decoder.py
--rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.4/tests/test_listener.py
--rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.4/tests/test_microconsumer.py
--rw-rw-rw-   0        0        0        0 2023-04-27 19:19:55.000000 rabbie-0.0.4/tests/test_producer.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.066102 rabbie-0.0.5/
+-rw-rw-rw-   0        0        0     1077 2023-04-24 20:01:12.000000 rabbie-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     7998 2023-05-11 11:20:01.065103 rabbie-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7522 2023-05-11 11:17:49.000000 rabbie-0.0.5/README.md
+-rw-rw-rw-   0        0        0       63 2023-04-02 21:06:34.000000 rabbie-0.0.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.011103 rabbie-0.0.5/rabbie/
+-rw-rw-rw-   0        0        0      230 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.024105 rabbie-0.0.5/rabbie/broker_types/
+-rw-rw-rw-   0        0        0       60 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/broker_types/__init__.py
+-rw-rw-rw-   0        0        0     4632 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/broker_types/channel.py
+-rw-rw-rw-   0        0        0      182 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/broker_types/relayed_types.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.026104 rabbie-0.0.5/rabbie/connection/
+-rw-rw-rw-   0        0        0       44 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/connection/__init__.py
+-rw-rw-rw-   0        0        0      294 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/connection/details.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.030125 rabbie-0.0.5/rabbie/consumer/
+-rw-rw-rw-   0        0        0      175 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/consumer/__init__.py
+-rw-rw-rw-   0        0        0     6289 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/consumer/consumer.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.034103 rabbie-0.0.5/rabbie/consumer/listener/
+-rw-rw-rw-   0        0        0       79 2023-04-24 20:01:12.000000 rabbie-0.0.5/rabbie/consumer/listener/__init__.py
+-rw-rw-rw-   0        0        0     5200 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/consumer/listener/listener.py
+-rw-rw-rw-   0        0        0      400 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/consumer/listener/listener_details.py
+-rw-rw-rw-   0        0        0     3079 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/consumer/microconsumer.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.036103 rabbie-0.0.5/rabbie/decoder/
+-rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/decoder/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-04-24 20:01:12.000000 rabbie-0.0.5/rabbie/decoder/decoder.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.040103 rabbie-0.0.5/rabbie/decoder/decoders/
+-rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/decoder/decoders/__init__.py
+-rw-rw-rw-   0        0        0      219 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/decoder/decoders/auto_decoder.py
+-rw-rw-rw-   0        0        0      148 2023-04-24 20:01:12.000000 rabbie-0.0.5/rabbie/decoder/decoders/json_decoder.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.042105 rabbie-0.0.5/rabbie/decoder/exceptions/
+-rw-rw-rw-   0        0        0       94 2023-03-29 12:21:12.000000 rabbie-0.0.5/rabbie/decoder/exceptions/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-03-29 12:19:53.000000 rabbie-0.0.5/rabbie/decoder/exceptions/decode_exception.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.045103 rabbie-0.0.5/rabbie/encoder/
+-rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/encoder/__init__.py
+-rw-rw-rw-   0        0        0      197 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/encoder/encoder.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.048106 rabbie-0.0.5/rabbie/encoder/encoders/
+-rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/encoder/encoders/__init__.py
+-rw-rw-rw-   0        0        0      461 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/encoder/encoders/auto_encoder.py
+-rw-rw-rw-   0        0        0      215 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/encoder/encoders/json_encoder.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.049103 rabbie-0.0.5/rabbie/logger/
+-rw-rw-rw-   0        0        0      312 2023-04-24 20:01:12.000000 rabbie-0.0.5/rabbie/logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.052103 rabbie-0.0.5/rabbie/producer/
+-rw-rw-rw-   0        0        0       46 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/producer/__init__.py
+-rw-rw-rw-   0        0        0     4584 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/producer/producer.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.055103 rabbie-0.0.5/rabbie/producer/publisher/
+-rw-rw-rw-   0        0        0       34 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/producer/publisher/__init__.py
+-rw-rw-rw-   0        0        0     3176 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/producer/publisher/publisher.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.058104 rabbie-0.0.5/rabbie/supervisor/
+-rw-rw-rw-   0        0        0       50 2023-04-24 20:01:12.000000 rabbie-0.0.5/rabbie/supervisor/__init__.py
+-rw-rw-rw-   0        0        0     4560 2023-04-24 20:01:12.000000 rabbie-0.0.5/rabbie/supervisor/supervisor.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.020134 rabbie-0.0.5/rabbie.egg-info/
+-rw-rw-rw-   0        0        0     7998 2023-05-11 11:20:00.000000 rabbie-0.0.5/rabbie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1338 2023-05-11 11:20:00.000000 rabbie-0.0.5/rabbie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 11:20:00.000000 rabbie-0.0.5/rabbie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-11 11:20:00.000000 rabbie-0.0.5/rabbie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-11 11:20:00.000000 rabbie-0.0.5/rabbie.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 11:20:01.066102 rabbie-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      854 2023-05-11 11:19:20.000000 rabbie-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.064103 rabbie-0.0.5/tests/
+-rw-rw-rw-   0        0        0     4748 2023-05-11 11:17:49.000000 rabbie-0.0.5/tests/test_consumer.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.5/tests/test_decoder.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.5/tests/test_listener.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.5/tests/test_microconsumer.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 11:17:49.000000 rabbie-0.0.5/tests/test_producer.py
```

### Comparing `rabbie-0.0.4/LICENSE` & `rabbie-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.4/PKG-INFO` & `rabbie-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbie
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple, decorator interface for AMQP based message brokers
 Home-page: https://github.com/scuffi/rabbie
 Author: Archie Ferguson
 Author-email: iamarchieferguson@gmail.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rabbie-0.0.4/README.md` & `rabbie-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.4/rabbie/broker_types/channel.py` & `rabbie-0.0.5/rabbie/broker_types/channel.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.4/rabbie/consumer/consumer.py` & `rabbie-0.0.5/rabbie/consumer/consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from .microconsumer import MicroConsumer
 from ..connection import Details
 from .listener import Listener, ListenerDetails
 
 from ..supervisor import Supervisor
 
-from ..decoder import JSONDecoder
+from ..decoder import AutoDecoder
 from ..logger import logger as log
 
 if TYPE_CHECKING:
     from ..decoder import Decoder
 
 
 class Consumer:
@@ -31,25 +31,25 @@
         self,
         *,
         # All parameters below must be passed in as KW args
         host: Optional[str] = Details.HOST,
         port: Optional[str] = Details.PORT,
         username: Optional[str] = Details.USERNAME,
         password: Optional[str] = Details.PASSWORD,
-        default_decoder: Optional["Decoder"] = None,
+        default_decoder: Optional["Decoder"] = AutoDecoder(),
         **kwargs,
     ):
         """Instantiate a new Consumer object with the given connection details.
 
         Args:
             host (Optional[str], optional): The host of the broker. Defaults to Details.HOST.
             port (Optional[str], optional): The port of the broker. Defaults to Details.PORT.
             username (Optional[str], optional): The authenticated username. Defaults to Details.USERNAME.
             password (Optional[str], optional): The authenticated password. Defaults to Details.PASSWORD.
-            default_decoder (Optional[Decoder], optional): The default decoder for decoding messages. Defaults to None.
+            default_decoder (Optional[Decoder], optional): The default decoder for decoding messages. Defaults to AutoDecoder
 
             Any other arguments are passed directly in to the connection parameters.
         """
         self._host = host
         self._port = port
         self._username = username
         self._password = password
@@ -175,9 +175,9 @@
 
 
 consumer = Consumer(
     host="localhost",
     port=5672,
     username="user",
     password="password",
-    default_decoder=JSONDecoder(),
+    default_decoder=AutoDecoder(),
 )
```

### Comparing `rabbie-0.0.4/rabbie/consumer/listener/listener.py` & `rabbie-0.0.5/rabbie/consumer/listener/listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         try:
             # Create a BlockingConnection into the queue
             connection = pika.BlockingConnection(self.connection_parameters)
 
             # Open a channel to receive messages through
             channel = connection.channel()
 
-            channel.queue_declare(queue=self.details.queue_name, durable=True)
+            channel.queue_declare(queue=self.details.queue_name)
             channel.basic_qos(prefetch_count=1)
 
             channel.basic_consume(
                 queue=self.details.queue_name,
                 on_message_callback=self._callback,
                 auto_ack=self.details.auto_ack,
             )
```

### Comparing `rabbie-0.0.4/rabbie/consumer/microconsumer.py` & `rabbie-0.0.5/rabbie/consumer/microconsumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 from functools import wraps
 
 from pika.connection import ConnectionParameters
 
 from .listener import Listener, ListenerDetails
 from ..connection import Details
-from ..decoder import Decoder
+from ..decoder import Decoder, AutoDecoder
 
 
 class MicroConsumer:
     def __init__(
         self,
-        default_decoder: Optional["Decoder"] = None,
+        default_decoder: Optional["Decoder"] = AutoDecoder(),
     ) -> None:
         """MicroConsumer object holds listeners for a Consumer to pick up
 
         Args:
             default_decoder (Optional[Decoder], optional): The default decoder for decoding messages. Defaults to None.
         """
         self.default_decoder = default_decoder
```

### Comparing `rabbie-0.0.4/rabbie/producer/producer.py` & `rabbie-0.0.5/rabbie/producer/producer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
 import pika
 
 
 from ..connection import Details
-from ..encoder import Encoder
+from ..encoder import Encoder, AutoEncoder
 from .publisher import Publisher
 
 
 class Producer:
     """
     Producer is a simple class that holds details required to connect to a message broker.
 
@@ -19,18 +19,39 @@
         self,
         *,
         # All parameters below must be passed in as KW args
         host: Optional[str] = Details.HOST,
         port: Optional[str] = Details.PORT,
         username: Optional[str] = Details.USERNAME,
         password: Optional[str] = Details.PASSWORD,
-        encoder: Optional[Encoder] = None,
+        encoder: Optional[Encoder] = AutoEncoder(),
         connection_type: pika.BaseConnection = pika.BlockingConnection,
         **kwargs,
     ):
+        """
+        This is a constructor function that initializes a connection to a RabbitMQ queue using the given
+        parameters.
+
+        Args:
+          host (Optional[str]): The hostname or IP address of the RabbitMQ server to connect to.
+          port (Optional[str]): The port number used to connect to the RabbitMQ server. If not provided, it
+        will use the default port number specified in the Details.HOST constant.
+          username (Optional[str]): The username used for authentication when connecting to the queue.
+          password (Optional[str]): The password parameter is an optional string that represents the
+        password used to authenticate the connection to the queue. It is one of the parameters that can be
+        passed in as a keyword argument when initializing an instance of the class. If not provided, it
+        defaults to the value of the PASSWORD constant defined in the Details
+          encoder (Optional[Encoder]): The `encoder` parameter is an optional argument that specifies the
+        encoding method to be used for messages sent to the queue. It defaults to an `AutoEncoder` instance,
+        which automatically detects the appropriate encoding method based on the message content.
+          connection_type (pika.BaseConnection): The type of connection to be established with the RabbitMQ
+        server. It is set to `pika.BlockingConnection` by default, which means that the connection will
+        block the execution of the program until it is established. Other options include
+        `pika.SelectConnection` and `pika.AsyncioConnection
+        """
         self._host = host
         self._port = port
         self._username = username
         self._password = password
 
         self.encoder = encoder
```

### Comparing `rabbie-0.0.4/rabbie/producer/publisher/publisher.py` & `rabbie-0.0.5/rabbie/producer/publisher/publisher.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.4/rabbie/supervisor/supervisor.py` & `rabbie-0.0.5/rabbie/supervisor/supervisor.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.4/rabbie.egg-info/PKG-INFO` & `rabbie-0.0.5/rabbie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbie
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple, decorator interface for AMQP based message brokers
 Home-page: https://github.com/scuffi/rabbie
 Author: Archie Ferguson
 Author-email: iamarchieferguson@gmail.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rabbie-0.0.4/rabbie.egg-info/SOURCES.txt` & `rabbie-0.0.5/rabbie.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -18,20 +18,22 @@
 rabbie/consumer/microconsumer.py
 rabbie/consumer/listener/__init__.py
 rabbie/consumer/listener/listener.py
 rabbie/consumer/listener/listener_details.py
 rabbie/decoder/__init__.py
 rabbie/decoder/decoder.py
 rabbie/decoder/decoders/__init__.py
+rabbie/decoder/decoders/auto_decoder.py
 rabbie/decoder/decoders/json_decoder.py
 rabbie/decoder/exceptions/__init__.py
 rabbie/decoder/exceptions/decode_exception.py
 rabbie/encoder/__init__.py
 rabbie/encoder/encoder.py
 rabbie/encoder/encoders/__init__.py
+rabbie/encoder/encoders/auto_encoder.py
 rabbie/encoder/encoders/json_encoder.py
 rabbie/logger/__init__.py
 rabbie/producer/__init__.py
 rabbie/producer/producer.py
 rabbie/producer/publisher/__init__.py
 rabbie/producer/publisher/publisher.py
 rabbie/supervisor/__init__.py
```

### Comparing `rabbie-0.0.4/setup.py` & `rabbie-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-version = "0.0.4"
+version = "0.0.5"
 requirements = ["pika", "multiprocess", "rich", "watchdog"]
 
 setup(
     name="rabbie",
     version=version,
     author="Archie Ferguson",
     author_email="iamarchieferguson@gmail.com",
```

### Comparing `rabbie-0.0.4/tests/test_consumer.py` & `rabbie-0.0.5/tests/test_consumer.py`

 * *Files identical despite different names*

