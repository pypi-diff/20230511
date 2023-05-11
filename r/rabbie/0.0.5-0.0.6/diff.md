# Comparing `tmp/rabbie-0.0.5.tar.gz` & `tmp/rabbie-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbie-0.0.5.tar", last modified: Thu May 11 11:20:01 2023, max compression
+gzip compressed data, was "rabbie-0.0.6.tar", last modified: Thu May 11 11:34:45 2023, max compression
```

## Comparing `rabbie-0.0.5.tar` & `rabbie-0.0.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.066102 rabbie-0.0.5/
--rw-rw-rw-   0        0        0     1077 2023-04-24 20:01:12.000000 rabbie-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     7998 2023-05-11 11:20:01.065103 rabbie-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     7522 2023-05-11 11:17:49.000000 rabbie-0.0.5/README.md
--rw-rw-rw-   0        0        0       63 2023-04-02 21:06:34.000000 rabbie-0.0.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.011103 rabbie-0.0.5/rabbie/
--rw-rw-rw-   0        0        0      230 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.024105 rabbie-0.0.5/rabbie/broker_types/
--rw-rw-rw-   0        0        0       60 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/broker_types/__init__.py
--rw-rw-rw-   0        0        0     4632 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/broker_types/channel.py
--rw-rw-rw-   0        0        0      182 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/broker_types/relayed_types.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.026104 rabbie-0.0.5/rabbie/connection/
--rw-rw-rw-   0        0        0       44 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/connection/__init__.py
--rw-rw-rw-   0        0        0      294 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/connection/details.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.030125 rabbie-0.0.5/rabbie/consumer/
--rw-rw-rw-   0        0        0      175 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/consumer/__init__.py
--rw-rw-rw-   0        0        0     6289 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/consumer/consumer.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.034103 rabbie-0.0.5/rabbie/consumer/listener/
--rw-rw-rw-   0        0        0       79 2023-04-24 20:01:12.000000 rabbie-0.0.5/rabbie/consumer/listener/__init__.py
--rw-rw-rw-   0        0        0     5200 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/consumer/listener/listener.py
--rw-rw-rw-   0        0        0      400 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/consumer/listener/listener_details.py
--rw-rw-rw-   0        0        0     3079 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/consumer/microconsumer.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.036103 rabbie-0.0.5/rabbie/decoder/
--rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/decoder/__init__.py
--rw-rw-rw-   0        0        0      132 2023-04-24 20:01:12.000000 rabbie-0.0.5/rabbie/decoder/decoder.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.040103 rabbie-0.0.5/rabbie/decoder/decoders/
--rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/decoder/decoders/__init__.py
--rw-rw-rw-   0        0        0      219 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/decoder/decoders/auto_decoder.py
--rw-rw-rw-   0        0        0      148 2023-04-24 20:01:12.000000 rabbie-0.0.5/rabbie/decoder/decoders/json_decoder.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.042105 rabbie-0.0.5/rabbie/decoder/exceptions/
--rw-rw-rw-   0        0        0       94 2023-03-29 12:21:12.000000 rabbie-0.0.5/rabbie/decoder/exceptions/__init__.py
--rw-rw-rw-   0        0        0       44 2023-03-29 12:19:53.000000 rabbie-0.0.5/rabbie/decoder/exceptions/decode_exception.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.045103 rabbie-0.0.5/rabbie/encoder/
--rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/encoder/__init__.py
--rw-rw-rw-   0        0        0      197 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/encoder/encoder.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.048106 rabbie-0.0.5/rabbie/encoder/encoders/
--rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/encoder/encoders/__init__.py
--rw-rw-rw-   0        0        0      461 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/encoder/encoders/auto_encoder.py
--rw-rw-rw-   0        0        0      215 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/encoder/encoders/json_encoder.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.049103 rabbie-0.0.5/rabbie/logger/
--rw-rw-rw-   0        0        0      312 2023-04-24 20:01:12.000000 rabbie-0.0.5/rabbie/logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.052103 rabbie-0.0.5/rabbie/producer/
--rw-rw-rw-   0        0        0       46 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/producer/__init__.py
--rw-rw-rw-   0        0        0     4584 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/producer/producer.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.055103 rabbie-0.0.5/rabbie/producer/publisher/
--rw-rw-rw-   0        0        0       34 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/producer/publisher/__init__.py
--rw-rw-rw-   0        0        0     3176 2023-05-11 11:17:49.000000 rabbie-0.0.5/rabbie/producer/publisher/publisher.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.058104 rabbie-0.0.5/rabbie/supervisor/
--rw-rw-rw-   0        0        0       50 2023-04-24 20:01:12.000000 rabbie-0.0.5/rabbie/supervisor/__init__.py
--rw-rw-rw-   0        0        0     4560 2023-04-24 20:01:12.000000 rabbie-0.0.5/rabbie/supervisor/supervisor.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.020134 rabbie-0.0.5/rabbie.egg-info/
--rw-rw-rw-   0        0        0     7998 2023-05-11 11:20:00.000000 rabbie-0.0.5/rabbie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1338 2023-05-11 11:20:00.000000 rabbie-0.0.5/rabbie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 11:20:00.000000 rabbie-0.0.5/rabbie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-11 11:20:00.000000 rabbie-0.0.5/rabbie.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-11 11:20:00.000000 rabbie-0.0.5/rabbie.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 11:20:01.066102 rabbie-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      854 2023-05-11 11:19:20.000000 rabbie-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:20:01.064103 rabbie-0.0.5/tests/
--rw-rw-rw-   0        0        0     4748 2023-05-11 11:17:49.000000 rabbie-0.0.5/tests/test_consumer.py
--rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.5/tests/test_decoder.py
--rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.5/tests/test_listener.py
--rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.5/tests/test_microconsumer.py
--rw-rw-rw-   0        0        0        0 2023-05-11 11:17:49.000000 rabbie-0.0.5/tests/test_producer.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:34:45.995602 rabbie-0.0.6/
+-rw-rw-rw-   0        0        0     1077 2023-04-24 20:01:12.000000 rabbie-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     7998 2023-05-11 11:34:45.994601 rabbie-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7522 2023-05-11 11:17:49.000000 rabbie-0.0.6/README.md
+-rw-rw-rw-   0        0        0       63 2023-04-02 21:06:34.000000 rabbie-0.0.6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-11 11:34:45.922050 rabbie-0.0.6/rabbie/
+-rw-rw-rw-   0        0        0      230 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:34:45.951049 rabbie-0.0.6/rabbie/broker_types/
+-rw-rw-rw-   0        0        0       60 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/broker_types/__init__.py
+-rw-rw-rw-   0        0        0     4898 2023-05-11 11:34:26.000000 rabbie-0.0.6/rabbie/broker_types/channel.py
+-rw-rw-rw-   0        0        0      182 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/broker_types/relayed_types.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:34:45.954049 rabbie-0.0.6/rabbie/connection/
+-rw-rw-rw-   0        0        0       44 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/connection/__init__.py
+-rw-rw-rw-   0        0        0      294 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/connection/details.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:34:45.958054 rabbie-0.0.6/rabbie/consumer/
+-rw-rw-rw-   0        0        0      175 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/consumer/__init__.py
+-rw-rw-rw-   0        0        0     6289 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/consumer/consumer.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:34:45.962056 rabbie-0.0.6/rabbie/consumer/listener/
+-rw-rw-rw-   0        0        0       79 2023-04-24 20:01:12.000000 rabbie-0.0.6/rabbie/consumer/listener/__init__.py
+-rw-rw-rw-   0        0        0     5200 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/consumer/listener/listener.py
+-rw-rw-rw-   0        0        0      400 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/consumer/listener/listener_details.py
+-rw-rw-rw-   0        0        0     3079 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/consumer/microconsumer.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:34:45.965056 rabbie-0.0.6/rabbie/decoder/
+-rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/decoder/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-04-24 20:01:12.000000 rabbie-0.0.6/rabbie/decoder/decoder.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:34:45.969077 rabbie-0.0.6/rabbie/decoder/decoders/
+-rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/decoder/decoders/__init__.py
+-rw-rw-rw-   0        0        0      219 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/decoder/decoders/auto_decoder.py
+-rw-rw-rw-   0        0        0      148 2023-04-24 20:01:12.000000 rabbie-0.0.6/rabbie/decoder/decoders/json_decoder.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:34:45.971057 rabbie-0.0.6/rabbie/decoder/exceptions/
+-rw-rw-rw-   0        0        0       94 2023-03-29 12:21:12.000000 rabbie-0.0.6/rabbie/decoder/exceptions/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-03-29 12:19:53.000000 rabbie-0.0.6/rabbie/decoder/exceptions/decode_exception.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:34:45.973090 rabbie-0.0.6/rabbie/encoder/
+-rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/encoder/__init__.py
+-rw-rw-rw-   0        0        0      197 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/encoder/encoder.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:34:45.978601 rabbie-0.0.6/rabbie/encoder/encoders/
+-rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/encoder/encoders/__init__.py
+-rw-rw-rw-   0        0        0      461 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/encoder/encoders/auto_encoder.py
+-rw-rw-rw-   0        0        0      215 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/encoder/encoders/json_encoder.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:34:45.979601 rabbie-0.0.6/rabbie/logger/
+-rw-rw-rw-   0        0        0      312 2023-04-24 20:01:12.000000 rabbie-0.0.6/rabbie/logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:34:45.982602 rabbie-0.0.6/rabbie/producer/
+-rw-rw-rw-   0        0        0       46 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/producer/__init__.py
+-rw-rw-rw-   0        0        0     4584 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/producer/producer.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:34:45.984600 rabbie-0.0.6/rabbie/producer/publisher/
+-rw-rw-rw-   0        0        0       34 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/producer/publisher/__init__.py
+-rw-rw-rw-   0        0        0     3176 2023-05-11 11:17:49.000000 rabbie-0.0.6/rabbie/producer/publisher/publisher.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:34:45.987602 rabbie-0.0.6/rabbie/supervisor/
+-rw-rw-rw-   0        0        0       50 2023-04-24 20:01:12.000000 rabbie-0.0.6/rabbie/supervisor/__init__.py
+-rw-rw-rw-   0        0        0     4560 2023-04-24 20:01:12.000000 rabbie-0.0.6/rabbie/supervisor/supervisor.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:34:45.948053 rabbie-0.0.6/rabbie.egg-info/
+-rw-rw-rw-   0        0        0     7998 2023-05-11 11:34:45.000000 rabbie-0.0.6/rabbie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1338 2023-05-11 11:34:45.000000 rabbie-0.0.6/rabbie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 11:34:45.000000 rabbie-0.0.6/rabbie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-11 11:34:45.000000 rabbie-0.0.6/rabbie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-11 11:34:45.000000 rabbie-0.0.6/rabbie.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 11:34:45.995602 rabbie-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      854 2023-05-11 11:34:26.000000 rabbie-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:34:45.993605 rabbie-0.0.6/tests/
+-rw-rw-rw-   0        0        0     4748 2023-05-11 11:17:49.000000 rabbie-0.0.6/tests/test_consumer.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.6/tests/test_decoder.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.6/tests/test_listener.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.6/tests/test_microconsumer.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 11:17:49.000000 rabbie-0.0.6/tests/test_producer.py
```

### Comparing `rabbie-0.0.5/LICENSE` & `rabbie-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.5/PKG-INFO` & `rabbie-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbie
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple, decorator interface for AMQP based message brokers
 Home-page: https://github.com/scuffi/rabbie
 Author: Archie Ferguson
 Author-email: iamarchieferguson@gmail.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rabbie-0.0.5/README.md` & `rabbie-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.5/rabbie/broker_types/channel.py` & `rabbie-0.0.6/rabbie/broker_types/channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pika.adapters.blocking_connection import BlockingChannel
 from pika.spec import BasicProperties as Properties
 
-from ..encoder import Encoder
+from ..encoder import Encoder, AutoEncoder
 
 
 class Channel:
     def __init__(self, blocking_channel: BlockingChannel) -> None:
         self._channel = blocking_channel
 
     def acknowledge(self, delivery_tag: int = 0, multiple: bool = False):
@@ -49,15 +49,16 @@
     def publish(
         self,
         body: str,
         queue: str,
         exchange: str = None,
         properties: Properties = None,
         mandatory: bool = False,
-        encoder: Encoder = None,
+        encoder: Encoder = AutoEncoder(),
+        **kwargs,
     ):
         """
         This function publishes a message to a specified queue or exchange with optional properties and
         mandatory flag.
 
         Args:
           queue (str): The name of the queue to which the message will be published.
@@ -69,23 +70,27 @@
         set additional properties for the message being published. These properties can include things like
         message headers, message expiration time, message priority, and more. The properties are defined
         using the BasicProperties class from the pika library. If no properties are specified,
           mandatory (bool): A boolean value indicating whether the message is mandatory or not. If set to
         True, the message will be returned to the sender if it cannot be delivered to any queue. If set to
         False, the message will be silently dropped if it cannot be delivered to any queue. Defaults to
         False
+          encoder (Encoder): The encoder to use when encoding messages. Default is AutoEncoder
+        Any other arguments will get passed into the queue declaration.
         """
         # If the encoder is not None, we need to reassign message to an 'Encoded' version
         if encoder:
             body = encoder.encode(body)
 
             # We also want to override the content_type, if properties are given
             if properties is not None:
                 properties.content_type = encoder.content_type()
 
+        self._channel.queue_declare(queue, **kwargs)
+
         self._channel.basic_publish(
             exchange=exchange or "",
             routing_key=queue,
             body=str(body),
             properties=properties,
             mandatory=mandatory,
         )
```

### Comparing `rabbie-0.0.5/rabbie/consumer/consumer.py` & `rabbie-0.0.6/rabbie/consumer/consumer.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.5/rabbie/consumer/listener/listener.py` & `rabbie-0.0.6/rabbie/consumer/listener/listener.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.5/rabbie/consumer/microconsumer.py` & `rabbie-0.0.6/rabbie/consumer/microconsumer.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.5/rabbie/producer/producer.py` & `rabbie-0.0.6/rabbie/producer/producer.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.5/rabbie/producer/publisher/publisher.py` & `rabbie-0.0.6/rabbie/producer/publisher/publisher.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.5/rabbie/supervisor/supervisor.py` & `rabbie-0.0.6/rabbie/supervisor/supervisor.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.5/rabbie.egg-info/PKG-INFO` & `rabbie-0.0.6/rabbie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbie
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple, decorator interface for AMQP based message brokers
 Home-page: https://github.com/scuffi/rabbie
 Author: Archie Ferguson
 Author-email: iamarchieferguson@gmail.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rabbie-0.0.5/rabbie.egg-info/SOURCES.txt` & `rabbie-0.0.6/rabbie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.5/setup.py` & `rabbie-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-version = "0.0.5"
+version = "0.0.6"
 requirements = ["pika", "multiprocess", "rich", "watchdog"]
 
 setup(
     name="rabbie",
     version=version,
     author="Archie Ferguson",
     author_email="iamarchieferguson@gmail.com",
```

### Comparing `rabbie-0.0.5/tests/test_consumer.py` & `rabbie-0.0.6/tests/test_consumer.py`

 * *Files identical despite different names*

