# Comparing `tmp/verbit-streaming-sdk-0.8.1.tar.gz` & `tmp/verbit-streaming-sdk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/verbit-streaming-sdk-0.8.1.tar", last modified: Thu Feb 24 08:57:40 2022, max compression
+gzip compressed data, was "verbit-streaming-sdk-0.9.0.tar", last modified: Sun May  1 08:05:45 2022, max compression
```

## Comparing `verbit-streaming-sdk-0.8.1.tar` & `verbit-streaming-sdk-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 eliasor    (501) staff       (20)        0 2022-02-24 08:57:40.000000 verbit-streaming-sdk-0.8.1/
--rw-r--r--   0 eliasor    (501) staff       (20)     8344 2022-02-24 08:57:40.000000 verbit-streaming-sdk-0.8.1/PKG-INFO
-drwxr-xr-x   0 eliasor    (501) staff       (20)        0 2022-02-24 08:57:40.000000 verbit-streaming-sdk-0.8.1/verbit_streaming_sdk.egg-info/
--rw-r--r--   0 eliasor    (501) staff       (20)     8344 2022-02-24 08:57:40.000000 verbit-streaming-sdk-0.8.1/verbit_streaming_sdk.egg-info/PKG-INFO
--rw-r--r--   0 eliasor    (501) staff       (20)        1 2022-02-24 08:57:40.000000 verbit-streaming-sdk-0.8.1/verbit_streaming_sdk.egg-info/not-zip-safe
--rw-r--r--   0 eliasor    (501) staff       (20)      307 2022-02-24 08:57:40.000000 verbit-streaming-sdk-0.8.1/verbit_streaming_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 eliasor    (501) staff       (20)       40 2022-02-24 08:57:40.000000 verbit-streaming-sdk-0.8.1/verbit_streaming_sdk.egg-info/requires.txt
--rw-r--r--   0 eliasor    (501) staff       (20)        7 2022-02-24 08:57:40.000000 verbit-streaming-sdk-0.8.1/verbit_streaming_sdk.egg-info/top_level.txt
--rw-r--r--   0 eliasor    (501) staff       (20)        1 2022-02-24 08:57:40.000000 verbit-streaming-sdk-0.8.1/verbit_streaming_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 eliasor    (501) staff       (20)     6909 2022-02-24 08:57:28.000000 verbit-streaming-sdk-0.8.1/README.md
--rw-r--r--   0 eliasor    (501) staff       (20)      544 2022-02-24 08:57:28.000000 verbit-streaming-sdk-0.8.1/setup.py
--rw-r--r--   0 eliasor    (501) staff       (20)       38 2022-02-24 08:57:40.000000 verbit-streaming-sdk-0.8.1/setup.cfg
-drwxr-xr-x   0 eliasor    (501) staff       (20)        0 2022-02-24 08:57:40.000000 verbit-streaming-sdk-0.8.1/verbit/
--rwxr-xr-x   0 eliasor    (501) staff       (20)    11734 2022-02-07 18:02:30.000000 verbit-streaming-sdk-0.8.1/verbit/streaming_client.py
+drwxr-xr-x   0 eliasor    (501) staff       (20)        0 2022-05-01 08:05:45.384261 verbit-streaming-sdk-0.9.0/
+-rw-r--r--   0 eliasor    (501) staff       (20)    11036 2022-05-01 08:05:45.364496 verbit-streaming-sdk-0.9.0/PKG-INFO
+-rw-r--r--   0 eliasor    (501) staff       (20)     9281 2022-05-01 08:05:16.000000 verbit-streaming-sdk-0.9.0/README.md
+-rw-r--r--   0 eliasor    (501) staff       (20)      104 2022-01-13 11:37:56.000000 verbit-streaming-sdk-0.9.0/pyproject.toml
+-rw-r--r--   0 eliasor    (501) staff       (20)       38 2022-05-01 08:05:45.384489 verbit-streaming-sdk-0.9.0/setup.cfg
+-rw-r--r--   0 eliasor    (501) staff       (20)      544 2022-05-01 08:05:16.000000 verbit-streaming-sdk-0.9.0/setup.py
+drwxr-xr-x   0 eliasor    (501) staff       (20)        0 2022-05-01 08:05:45.322577 verbit-streaming-sdk-0.9.0/verbit/
+-rwxr-xr-x   0 eliasor    (501) staff       (20)    24349 2022-05-01 08:05:16.000000 verbit-streaming-sdk-0.9.0/verbit/streaming_client.py
+drwxr-xr-x   0 eliasor    (501) staff       (20)        0 2022-05-01 08:05:45.344370 verbit-streaming-sdk-0.9.0/verbit_streaming_sdk.egg-info/
+-rw-r--r--   0 eliasor    (501) staff       (20)    11036 2022-05-01 08:05:45.000000 verbit-streaming-sdk-0.9.0/verbit_streaming_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 eliasor    (501) staff       (20)      322 2022-05-01 08:05:45.000000 verbit-streaming-sdk-0.9.0/verbit_streaming_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 eliasor    (501) staff       (20)        1 2022-05-01 08:05:45.000000 verbit-streaming-sdk-0.9.0/verbit_streaming_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 eliasor    (501) staff       (20)        1 2022-05-01 08:05:45.000000 verbit-streaming-sdk-0.9.0/verbit_streaming_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 eliasor    (501) staff       (20)       40 2022-05-01 08:05:45.000000 verbit-streaming-sdk-0.9.0/verbit_streaming_sdk.egg-info/requires.txt
+-rw-r--r--   0 eliasor    (501) staff       (20)        7 2022-05-01 08:05:45.000000 verbit-streaming-sdk-0.9.0/verbit_streaming_sdk.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `verbit-streaming-sdk-0.8.1/PKG-INFO` & `verbit-streaming-sdk-0.9.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,150 +1,180 @@
-Metadata-Version: 2.1
-Name: verbit-streaming-sdk
-Version: 0.8.1
-Summary: Client SDK for Verbit's Streaming Speech Recognition services
-Home-page: https://github.com/verbit-ai/verbit-streaming-python-sdk
-License: UNKNOWN
-Description: # Verbit Streaming Python SDK
-        
-        ## Overview
-        
-        This package is a Python SDK for Verbit's Streaming Transcription API.
-        It can also be used as a reference implementation for porting to other programming languages.
-        You can use it as-is (see installation instructions below), or use it as an example for implementing your own custom client.
-        
-        The package includes a Python client for streaming media and getting responses from Verbit's Streaming Speech Recognition services via a WebSocket connection.
-        
-        ## Installation
-        
-        To install this package run:
-        
-            pip install --upgrade verbit-streaming-sdk
-        
-        ### Requirements
-        
-        - Python 3.8+
-        
-        ## Usage
-        
-        ### Ordering API
-        In order to use Verbit's Streaming Speech Recognition services, you must place an order using Verbit's Ordering API. Your request to the Ordering API must specify that the desired input and output schemes are streaming through a WebSocket. Upon successful placement of the order, you will be issued an authentication token which can be used to initiate a WebSocket connection.
-        
-        These two APIs and their respective SDKs are separated on purpose because placing orders to Verbit's Transcription services does not necessarily imply media streaming (you might want to upload a file instead).
-        Also, the services which operate order placement and the actual streaming of media are commonly distinct, therefore we find it useful to separate the SDKs to allow maximal flexibility for our customers.
-        
-        Please refer to our documentation here: [Ordering API](https://platform.verbit.co/api_docs).
-        
-        ### Streaming audio and getting responses
-        
-        Create the client, and pass in the `Access Token` acquired from the Ordering API:
-        
-        ```python
-        from verbit.streaming_client import WebSocketStreamingClient
-        
-        client = WebSocketStreamingClient(access_token="ACCESS TOKEN")
-        ```
-        
-        Create a generator function which yields chunks of audio (objects supporting the `bytes-like` interface).
-        The StreamingClient will use your generator as input, iterating it and sending each audio chunk to the Speech Recognition service.
-        
-        **Important: The Speech Recognition service expects the audio chunks to arrive at a realtime pace, or slower. Faster than realtime pace may cause the service to behave unexpectedly.**
-        
-        _Note:
-        The current version of the service supports only raw PCM format (pcm_s16le - PCM signed 16-bit little-endian).
-        Your generator should output audio chunks in this format._
-        
-        #### End of Stream
-        When the media generator is exhausted, the client should send an End-of-Stream (non-binary) message to the service. 
-        The End-of-Stream message should have the following structure:
-        ```
-        {
-           "event": "EOS"
-        }
-        ```
-        
-        ### Example
-        
-        The following example reads audio from a WAV file and streams it to the Speech Recognition service:
-        
-        ```python
-        import wave
-        from math import ceil
-        from time import sleep
-        from verbit.streaming_client import WebSocketStreamingClient, MediaConfig, ResponseType
-        
-        CHUNK_DURATION_SECONDS = 0.1
-        AUDIO_FILENAME = 'example.wav'
-        
-        def media_generator_wavefile(filename, chunk_duration):
-            """
-            Example generator, for streaming a 'WAV' audio-file, simulating realtime playback-rate using sleep()
-            """
-        
-            with wave.open(str(filename), 'rb') as wav:
-                nchannels, samplewidth, sample_rate, nframes, _, _ = wav.getparams()
-                samples_per_chunk = ceil(chunk_duration * sample_rate)
-                chunk_bytes = wav.readframes(samples_per_chunk)
-                while chunk_bytes:
-                    yield chunk_bytes
-                    chunk_bytes = wav.readframes(samples_per_chunk)
-                    sleep(chunk_duration)
-        
-        media_generator = media_generator_wavefile(AUDIO_FILENAME, CHUNK_DURATION_SECONDS)
-        
-        media_config = MediaConfig(format='S16LE',      # signed 16-bit little-endian PCM
-                                   num_channels=1,      # number of audio channels
-                                   sample_rate=16000,   # in Hz
-                                   sample_width=2)      # in bytes
-        
-        response_types = ResponseType.Transcript | ResponseType.Captions
-            
-        client = WebSocketStreamingClient(access_token="ACCESS TOKEN")
-        
-        response_generator = client.start_stream(media_generator=media_generator,
-                                                 media_config=media_config,
-                                                 response_types=response_types)
-        ```
-        
-        The client's `start_stream()` function returns a generator which can be iterated to fetch the Speech Recognition responses:
-        ```python
-        # get recognition responses
-        print('Waiting for responses ...')
-        for response in response_generator:
-            resp_type = response['response']['type']
-            alternatives = response['response']['alternatives']
-            alt0_transcript = alternatives[0]['transcript']
-            print(f'{resp_type}: {alt0_transcript}')
-        ```
-        
-        
-        ### Responses
-        
-        Responses received through the WebSocket are JSON objects with a specific schema (a full description of which can be found in [examples/responses/schema.md](https://github.com/verbit-ai/verbit-streaming-python-sdk/blob/main/examples/responses/schema.md)).
-        There are two types of responses - "transcript" and "captions":
-        
-        1. **Transcript**: this type of response contains the recognized words since the beginning of the current utterance. Like in real human speech, the stream of words is segmented into utterances in automatic speech recognition. An utterance is recognized incrementally, processing more of the incoming audio at each step. Each utterance starts at a specific start-time and extends its end-time with each step, yielding the most updated result.
-        Note that sequential updates for the same utterance will overlap, each response superseding the previous one - until a response signaling the end of the utterance is received (having `is_final == True`).
-        The `alternatives` array might contain different hypotheses, ordered by confidence level.
-        
-            Example "transcript" responses can be found in [examples/responses/transcript.md](https://github.com/verbit-ai/verbit-streaming-python-sdk/blob/main/examples/responses/transcript.md).
-        
-        
-        2. **Captions**: this type of response contains the recognized words within a specific time window. In contrast to the incremental nature of "transcript"-type responses, the "captions"-type responses are non-overlapping and consecutive. 
-        Only one "captions"-type response covering a specific time-span in the audio will be returned (or none, if no words were uttered).
-        The `is_final` field is always `True` because no updates will be output for the same time-span. The `alternatives` array will always have only one item for captions.
-        
-            Example "captions" responses can be found in [examples/responses/captions.md](https://github.com/verbit-ai/verbit-streaming-python-sdk/blob/main/examples/responses/captions.md).
-        
-        ### Testing
-        This client SDK comes with a set of unit-tests that can be used to ensure the correct functionality of the streaming client.
-        
-        To run the unit-tests:
-        ```bash
-        pip install pytest
-        pip install -r tests/requirements_test.txt
-        pytest
-        ```
-        
-Platform: UNKNOWN
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+# Verbit Streaming Python SDK
+
+## Overview
+
+This package is a Python SDK for Verbit's Streaming Transcription API.
+It can also be used as a reference implementation for porting to other programming languages.
+You can use it as-is (see installation instructions below), or use it as an example for implementing your own custom client.
+
+The package includes a Python client for streaming media and getting responses from Verbit's Streaming Speech Recognition services via a WebSocket connection.
+
+## Installation
+
+To install this package run:
+
+    pip install --upgrade verbit-streaming-sdk
+
+### Requirements
+
+- Python 3.8+
+
+## Usage
+
+### Ordering API
+In order to use Verbit's Streaming Speech Recognition services, you must place an order using Verbit's Ordering API. Your request to the Ordering API must specify that the desired input and output schemes are streaming through a WebSocket. Upon successful placement of the order, you will be issued an authentication token which can be used to initiate a WebSocket connection.
+
+These two APIs and their respective SDKs are separated on purpose because placing orders to Verbit's Transcription services does not necessarily imply media streaming (you might want to upload a file instead).
+Also, the services which operate order placement and the actual streaming of media are commonly distinct, therefore we find it useful to separate the SDKs to allow maximal flexibility for our customers.
+
+Please refer to our documentation here: [Ordering API](https://platform.verbit.co/api_docs).
+
+### Creating a WebSocketStreamingClient
+
+Create the client, and pass in the `Access Token` acquired from the Ordering API:
+
+```python
+from verbit.streaming_client import WebSocketStreamingClient
+
+client = WebSocketStreamingClient(access_token="ACCESS TOKEN")
+```
+
+### Streaming media via WebSocket
+
+Create a generator function which yields chunks of audio (objects supporting the `bytes-like` interface).
+The `WebSocketStreamingClient` will use your generator as input, iterating it and sending each audio chunk to the Speech Recognition service.
+
+**Important: The Speech Recognition service expects the audio chunks to arrive at a realtime pace, or slower. Faster than realtime pace may cause the service to behave unexpectedly.**
+
+
+#### Example
+
+The following example reads audio from a WAV file and streams it to the Speech Recognition Service:
+
+```python
+import wave
+from math import ceil
+from time import sleep
+from verbit.streaming_client import WebSocketStreamingClient, MediaConfig, ResponseType
+
+CHUNK_DURATION_SECONDS = 0.1
+AUDIO_FILENAME = 'example.wav'
+
+def media_generator_wavefile(filename, chunk_duration):
+    """
+    Example generator, for streaming a 'WAV' audio-file, simulating realtime playback-rate using sleep()
+    """
+
+    with wave.open(str(filename), 'rb') as wav:
+        nchannels, samplewidth, sample_rate, nframes, _, _ = wav.getparams()
+        samples_per_chunk = ceil(chunk_duration * sample_rate)
+        chunk_bytes = wav.readframes(samples_per_chunk)
+        while chunk_bytes:
+            yield chunk_bytes
+            chunk_bytes = wav.readframes(samples_per_chunk)
+            sleep(chunk_duration)
+
+media_generator = media_generator_wavefile(AUDIO_FILENAME, CHUNK_DURATION_SECONDS)
+
+media_config = MediaConfig(format='S16LE',      # signed 16-bit little-endian PCM
+                           num_channels=1,      # number of audio channels
+                           sample_rate=16000,   # in Hz
+                           sample_width=2)      # in bytes
+
+response_types = ResponseType.Transcript | ResponseType.Captions
+    
+client = WebSocketStreamingClient(access_token="ACCESS TOKEN")
+
+response_generator = client.start_stream(media_generator=media_generator,
+                                         media_config=media_config,
+                                         response_types=response_types)
+```
+
+### Providing media via an external source
+
+It is possible to use an external media source to provide media to the Speech Recognition Service.
+To do so, you need to specify the relevant input method when booking the session via Verbit's Ordering API.
+
+In such a scenario, you should **not** provide a media generator to the `WebSocketStreamingClient`. 
+Connecting the `WebSocketStreamingClient` to the Speech Recognition Service will initiate the session
+and signal the server to start consuming media from the external media source.
+Therefore, **you should only connect the `WebSocketStreamingClient` to the service after the external media source is ready.**
+
+#### Example
+
+The following example connects to the Speech Recognition Service without providing a media generator:
+
+```python
+from verbit.streaming_client import WebSocketStreamingClient, ResponseType
+
+response_types = ResponseType.Transcript | ResponseType.Captions
+    
+client = WebSocketStreamingClient(access_token="ACCESS TOKEN")
+
+response_generator = client.start_with_external_source(response_types=response_types)
+```
+
+
+### Getting responses
+
+The client's `start_stream()` and `start_with_external_source()` methods return a generator which can be iterated to fetch the Speech Recognition responses:
+```python
+# get recognition responses
+print('Waiting for responses ...')
+for response in response_generator:
+    resp_type = response['response']['type']
+    alternatives = response['response']['alternatives']
+    alt0_transcript = alternatives[0]['transcript']
+    print(f'{resp_type}: {alt0_transcript}')
+```
+
+#### End of Stream
+When the media generator is exhausted, the client sends an End-of-Stream (non-binary) message to the service.
+
+In a scenario where the media is coming from an external source, it is the user's responsibility to send the End-of-Stream message to the service.
+
+The End-of-Stream message can be sent using the `send_eos_event()` method, and it has the following structure:
+```
+{
+   "event": "EOS"
+}
+```
+
+### Responses
+
+Responses received through the WebSocket are JSON objects with a specific schema (a full description of which can be found in [examples/responses/schema.md](https://github.com/verbit-ai/verbit-streaming-python-sdk/blob/main/examples/responses/schema.md)).
+There are two types of responses - "transcript" and "captions":
+
+1. **Transcript**: this type of response contains the recognized words since the beginning of the current utterance. Like in real human speech, the stream of words is segmented into utterances in automatic speech recognition. An utterance is recognized incrementally, processing more of the incoming audio at each step. Each utterance starts at a specific start-time and extends its end-time with each step, yielding the most updated result.
+Note that sequential updates for the same utterance will overlap, each response superseding the previous one - until a response signaling the end of the utterance is received (having `is_final == True`).
+The `alternatives` array might contain different hypotheses, ordered by confidence level.
+
+    Example "transcript" responses can be found in [examples/responses/transcript.md](https://github.com/verbit-ai/verbit-streaming-python-sdk/blob/main/examples/responses/transcript.md).
+
+
+2. **Captions**: this type of response contains the recognized words within a specific time window. In contrast to the incremental nature of "transcript"-type responses, the "captions"-type responses are non-overlapping and consecutive. 
+Only one "captions"-type response covering a specific time-span in the audio will be returned (or none, if no words were uttered).
+The `is_final` field is always `True` because no updates will be output for the same time-span. The `alternatives` array will always have only one item for captions.
+
+    Example "captions" responses can be found in [examples/responses/captions.md](https://github.com/verbit-ai/verbit-streaming-python-sdk/blob/main/examples/responses/captions.md).
+
+### Error handling and recovery
+
+#### Initial connection
+In case the WebSocket client fails to establish the initial connection with the service, e.g. due to temporary unavailability, 
+it will perform exponential retry, up to [`max_connection_retry_seconds`](https://github.com/verbit-ai/verbit-streaming-python-sdk/blob/main/verbit/streaming_client.py#L108) (configurable).
+
+#### During a session
+In case the connection to the service is dropped during a session, the behavior of the WebSocket client will depend on the implementation chosen by the user.
+This client SDK contains two implementations, which have the same interface, but differ in their error handling behavior:
+1. `WebSocketStreamingClientSingleConnection` - the base implementation; does not attempt to reconnect in case the connection was dropped prematurely. It can be useful, for example, if you would like to implement your own connection error handling logic.
+2. `WebSocketStreamingClient` - the default implementation; will attempt to reconnect in case the connection was closed prematurely, as many times as needed, until the final response is received (or some non-retryable error occurrs).
+
+### Testing
+This client SDK comes with a set of unit-tests that can be used to ensure the correct functionality of the streaming client.
+
+To run the unit-tests:
+```bash
+pip install pytest
+pip install -r tests/requirements_test.txt
+pytest
+```
```

### Comparing `verbit-streaming-sdk-0.8.1/verbit_streaming_sdk.egg-info/PKG-INFO` & `verbit-streaming-sdk-0.9.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verbit-streaming-sdk
-Version: 0.8.1
+Version: 0.9.0
 Summary: Client SDK for Verbit's Streaming Speech Recognition services
 Home-page: https://github.com/verbit-ai/verbit-streaming-python-sdk
 License: UNKNOWN
 Description: # Verbit Streaming Python SDK
         
         ## Overview
         
@@ -30,45 +30,35 @@
         In order to use Verbit's Streaming Speech Recognition services, you must place an order using Verbit's Ordering API. Your request to the Ordering API must specify that the desired input and output schemes are streaming through a WebSocket. Upon successful placement of the order, you will be issued an authentication token which can be used to initiate a WebSocket connection.
         
         These two APIs and their respective SDKs are separated on purpose because placing orders to Verbit's Transcription services does not necessarily imply media streaming (you might want to upload a file instead).
         Also, the services which operate order placement and the actual streaming of media are commonly distinct, therefore we find it useful to separate the SDKs to allow maximal flexibility for our customers.
         
         Please refer to our documentation here: [Ordering API](https://platform.verbit.co/api_docs).
         
-        ### Streaming audio and getting responses
+        ### Creating a WebSocketStreamingClient
         
         Create the client, and pass in the `Access Token` acquired from the Ordering API:
         
         ```python
         from verbit.streaming_client import WebSocketStreamingClient
         
         client = WebSocketStreamingClient(access_token="ACCESS TOKEN")
         ```
         
+        ### Streaming media via WebSocket
+        
         Create a generator function which yields chunks of audio (objects supporting the `bytes-like` interface).
-        The StreamingClient will use your generator as input, iterating it and sending each audio chunk to the Speech Recognition service.
+        The `WebSocketStreamingClient` will use your generator as input, iterating it and sending each audio chunk to the Speech Recognition service.
         
         **Important: The Speech Recognition service expects the audio chunks to arrive at a realtime pace, or slower. Faster than realtime pace may cause the service to behave unexpectedly.**
         
-        _Note:
-        The current version of the service supports only raw PCM format (pcm_s16le - PCM signed 16-bit little-endian).
-        Your generator should output audio chunks in this format._
         
-        #### End of Stream
-        When the media generator is exhausted, the client should send an End-of-Stream (non-binary) message to the service. 
-        The End-of-Stream message should have the following structure:
-        ```
-        {
-           "event": "EOS"
-        }
-        ```
+        #### Example
         
-        ### Example
-        
-        The following example reads audio from a WAV file and streams it to the Speech Recognition service:
+        The following example reads audio from a WAV file and streams it to the Speech Recognition Service:
         
         ```python
         import wave
         from math import ceil
         from time import sleep
         from verbit.streaming_client import WebSocketStreamingClient, MediaConfig, ResponseType
         
@@ -101,25 +91,63 @@
         client = WebSocketStreamingClient(access_token="ACCESS TOKEN")
         
         response_generator = client.start_stream(media_generator=media_generator,
                                                  media_config=media_config,
                                                  response_types=response_types)
         ```
         
-        The client's `start_stream()` function returns a generator which can be iterated to fetch the Speech Recognition responses:
+        ### Providing media via an external source
+        
+        It is possible to use an external media source to provide media to the Speech Recognition Service.
+        To do so, you need to specify the relevant input method when booking the session via Verbit's Ordering API.
+        
+        In such a scenario, you should **not** provide a media generator to the `WebSocketStreamingClient`. 
+        Connecting the `WebSocketStreamingClient` to the Speech Recognition Service will initiate the session
+        and signal the server to start consuming media from the external media source.
+        Therefore, **you should only connect the `WebSocketStreamingClient` to the service after the external media source is ready.**
+        
+        #### Example
+        
+        The following example connects to the Speech Recognition Service without providing a media generator:
+        
+        ```python
+        from verbit.streaming_client import WebSocketStreamingClient, ResponseType
+        
+        response_types = ResponseType.Transcript | ResponseType.Captions
+            
+        client = WebSocketStreamingClient(access_token="ACCESS TOKEN")
+        
+        response_generator = client.start_with_external_source(response_types=response_types)
+        ```
+        
+        
+        ### Getting responses
+        
+        The client's `start_stream()` and `start_with_external_source()` methods return a generator which can be iterated to fetch the Speech Recognition responses:
         ```python
         # get recognition responses
         print('Waiting for responses ...')
         for response in response_generator:
             resp_type = response['response']['type']
             alternatives = response['response']['alternatives']
             alt0_transcript = alternatives[0]['transcript']
             print(f'{resp_type}: {alt0_transcript}')
         ```
         
+        #### End of Stream
+        When the media generator is exhausted, the client sends an End-of-Stream (non-binary) message to the service.
+        
+        In a scenario where the media is coming from an external source, it is the user's responsibility to send the End-of-Stream message to the service.
+        
+        The End-of-Stream message can be sent using the `send_eos_event()` method, and it has the following structure:
+        ```
+        {
+           "event": "EOS"
+        }
+        ```
         
         ### Responses
         
         Responses received through the WebSocket are JSON objects with a specific schema (a full description of which can be found in [examples/responses/schema.md](https://github.com/verbit-ai/verbit-streaming-python-sdk/blob/main/examples/responses/schema.md)).
         There are two types of responses - "transcript" and "captions":
         
         1. **Transcript**: this type of response contains the recognized words since the beginning of the current utterance. Like in real human speech, the stream of words is segmented into utterances in automatic speech recognition. An utterance is recognized incrementally, processing more of the incoming audio at each step. Each utterance starts at a specific start-time and extends its end-time with each step, yielding the most updated result.
@@ -131,14 +159,26 @@
         
         2. **Captions**: this type of response contains the recognized words within a specific time window. In contrast to the incremental nature of "transcript"-type responses, the "captions"-type responses are non-overlapping and consecutive. 
         Only one "captions"-type response covering a specific time-span in the audio will be returned (or none, if no words were uttered).
         The `is_final` field is always `True` because no updates will be output for the same time-span. The `alternatives` array will always have only one item for captions.
         
             Example "captions" responses can be found in [examples/responses/captions.md](https://github.com/verbit-ai/verbit-streaming-python-sdk/blob/main/examples/responses/captions.md).
         
+        ### Error handling and recovery
+        
+        #### Initial connection
+        In case the WebSocket client fails to establish the initial connection with the service, e.g. due to temporary unavailability, 
+        it will perform exponential retry, up to [`max_connection_retry_seconds`](https://github.com/verbit-ai/verbit-streaming-python-sdk/blob/main/verbit/streaming_client.py#L108) (configurable).
+        
+        #### During a session
+        In case the connection to the service is dropped during a session, the behavior of the WebSocket client will depend on the implementation chosen by the user.
+        This client SDK contains two implementations, which have the same interface, but differ in their error handling behavior:
+        1. `WebSocketStreamingClientSingleConnection` - the base implementation; does not attempt to reconnect in case the connection was dropped prematurely. It can be useful, for example, if you would like to implement your own connection error handling logic.
+        2. `WebSocketStreamingClient` - the default implementation; will attempt to reconnect in case the connection was closed prematurely, as many times as needed, until the final response is received (or some non-retryable error occurrs).
+        
         ### Testing
         This client SDK comes with a set of unit-tests that can be used to ensure the correct functionality of the streaming client.
         
         To run the unit-tests:
         ```bash
         pip install pytest
         pip install -r tests/requirements_test.txt
```

### Comparing `verbit-streaming-sdk-0.8.1/setup.py` & `verbit-streaming-sdk-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 setup(
     name='verbit-streaming-sdk',
     description="Client SDK for Verbit's Streaming Speech Recognition services",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/verbit-ai/verbit-streaming-python-sdk',
 
-    version='0.8.1',
+    version='0.9.0',
 
     packages=['verbit'],
     package_dir={'verbit': 'verbit'},
     python_requires=">=3.8",
     install_requires=[
         'websocket-client~=1.2.3',
         'tenacity~=8.0.1'
```

