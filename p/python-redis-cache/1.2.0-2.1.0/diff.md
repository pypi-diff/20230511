# Comparing `tmp/python-redis-cache-1.2.0.tar.gz` & `tmp/python-redis-cache-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-redis-cache-1.2.0.tar", last modified: Fri Oct 22 08:23:57 2021, max compression
+gzip compressed data, was "python-redis-cache-2.1.0.tar", last modified: Thu May 11 21:13:56 2023, max compression
```

## Comparing `python-redis-cache-1.2.0.tar` & `python-redis-cache-2.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-22 08:23:57.000000 python-redis-cache-1.2.0/
--rw-r--r--   0 root         (0) root         (0)     1069 2021-10-22 08:23:51.000000 python-redis-cache-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2973 2021-10-22 08:23:57.000000 python-redis-cache-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2668 2021-10-22 08:23:51.000000 python-redis-cache-1.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)      189 2021-10-22 08:23:51.000000 python-redis-cache-1.2.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-22 08:23:57.000000 python-redis-cache-1.2.0/python_redis_cache.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2973 2021-10-22 08:23:57.000000 python-redis-cache-1.2.0/python_redis_cache.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      243 2021-10-22 08:23:57.000000 python-redis-cache-1.2.0/python_redis_cache.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-22 08:23:57.000000 python-redis-cache-1.2.0/python_redis_cache.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2021-10-22 08:23:57.000000 python-redis-cache-1.2.0/python_redis_cache.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-22 08:23:57.000000 python-redis-cache-1.2.0/redis_cache/
--rw-r--r--   0 root         (0) root         (0)     5750 2021-10-22 08:23:51.000000 python-redis-cache-1.2.0/redis_cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)       94 2021-10-22 08:23:57.000000 python-redis-cache-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      775 2021-10-22 08:23:52.000000 python-redis-cache-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 21:13:56.413146 python-redis-cache-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-05-11 21:13:52.000000 python-redis-cache-2.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-05-11 21:13:56.413146 python-redis-cache-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2897 2023-05-11 21:13:52.000000 python-redis-cache-2.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-11 21:13:52.000000 python-redis-cache-2.1.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 21:13:56.413146 python-redis-cache-2.1.0/python_redis_cache.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-05-11 21:13:56.000000 python-redis-cache-2.1.0/python_redis_cache.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      243 2023-05-11 21:13:56.000000 python-redis-cache-2.1.0/python_redis_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 21:13:56.000000 python-redis-cache-2.1.0/python_redis_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-11 21:13:56.000000 python-redis-cache-2.1.0/python_redis_cache.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 21:13:56.413146 python-redis-cache-2.1.0/redis_cache/
+-rw-r--r--   0 root         (0) root         (0)     7518 2023-05-11 21:13:52.000000 python-redis-cache-2.1.0/redis_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-05-11 21:13:56.413146 python-redis-cache-2.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      760 2023-05-11 21:13:52.000000 python-redis-cache-2.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python-redis-cache-1.2.0/LICENSE` & `python-redis-cache-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-redis-cache-1.2.0/PKG-INFO` & `python-redis-cache-2.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: python-redis-cache
-Version: 1.2.0
+Version: 2.1.0
 Summary: Basic Redis caching for functions
 Home-page: http://github.com/taylorhakes/python-redis-cache
 Author: Taylor Hakes
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![CI](https://github.com/taylorhakes/python-redis-cache/workflows/CI/badge.svg?event=push)](https://github.com/taylorhakes/python-redis-cache/actions?query=event%3Apush+branch%3Amaster+workflow%3ACI)
 [![pypi](https://img.shields.io/pypi/v/python-redis-cache.svg)](https://pypi.python.org/pypi/python-redis-cache)
 [![versions](https://img.shields.io/pypi/pyversions/python-redis-cache.svg)](https://github.com/taylorhakes/python-redis-cache)
 [![license](https://img.shields.io/github/license/taylorhakes/python-redis-cache.svg)](https://github.com/taylorhakes/python-redis-cache/blob/master/LICENSE)
 
 # python-redis-cache
 Simple redis cache for Python functions
 
 ### Requirements
 - Redis 5+
-- Python 3.6+
+- Python 3.7+
 
 ## How to install
 ```
 pip install python-redis-cache
 ```
 
 ## How to use
@@ -59,17 +58,24 @@
 https://security.stackexchange.com/questions/183966/safely-load-a-pickle-file
 
 - **ttl** - is based on the time from when it's first inserted in the cache, not based on the last access
 - **limit** - The limit will revoke keys (once it hits the limit) based on FIFO, not based on LRU
 
 ## API
 ```python
-RedisCache(redis_client, prefix="rc", serializer=dumps, deserializer=loads)
+# Create the redis cache
+cache = RedisCache(redis_client, prefix="rc", serializer=dumps, deserializer=loads)
 
-RedisCache.cache(ttl=None, limit=None, namespace=None)
+# Cache decorator to go on functions, see above
+cache.cache(ttl=..., limit=..., namespace=...) -> Callable[[Callable], Callable]
+
+# Get multiple values from the cache
+cache.mget([{"fn": my_func, "args": [1,2], "kwargs": {}}, ...]) -> List[Any]
+
+Redis
 
 # Cached function API
 
 # Returns a cached value, if it exists in cache. Saves value in cache if it doesn't exist
 cached_func(*args, *kwargs)
 
 # Invalidates a single value
@@ -79,9 +85,7 @@
 cached_func.invalidate_all()
 ```
 
 - prefix - The string to prefix the redis keys with
 - serializer/deserializer - functions to convert arguments and return value to a string (user JSON by default)
 - ttl - The time in seconds to cache the return value
 - namespace - The string namespace of the cache. This is useful for allowing multiple functions to use the same cache. By default its `f'{function.__module__}.{function.__file__}'`
-
-
```

### Comparing `python-redis-cache-1.2.0/README.md` & `python-redis-cache-2.1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![license](https://img.shields.io/github/license/taylorhakes/python-redis-cache.svg)](https://github.com/taylorhakes/python-redis-cache/blob/master/LICENSE)
 
 # python-redis-cache
 Simple redis cache for Python functions
 
 ### Requirements
 - Redis 5+
-- Python 3.6+
+- Python 3.7+
 
 ## How to install
 ```
 pip install python-redis-cache
 ```
 
 ## How to use
@@ -47,17 +47,24 @@
 https://security.stackexchange.com/questions/183966/safely-load-a-pickle-file
 
 - **ttl** - is based on the time from when it's first inserted in the cache, not based on the last access
 - **limit** - The limit will revoke keys (once it hits the limit) based on FIFO, not based on LRU
 
 ## API
 ```python
-RedisCache(redis_client, prefix="rc", serializer=dumps, deserializer=loads)
+# Create the redis cache
+cache = RedisCache(redis_client, prefix="rc", serializer=dumps, deserializer=loads)
 
-RedisCache.cache(ttl=None, limit=None, namespace=None)
+# Cache decorator to go on functions, see above
+cache.cache(ttl=..., limit=..., namespace=...) -> Callable[[Callable], Callable]
+
+# Get multiple values from the cache
+cache.mget([{"fn": my_func, "args": [1,2], "kwargs": {}}, ...]) -> List[Any]
+
+Redis
 
 # Cached function API
 
 # Returns a cached value, if it exists in cache. Saves value in cache if it doesn't exist
 cached_func(*args, *kwargs)
 
 # Invalidates a single value
```

### Comparing `python-redis-cache-1.2.0/python_redis_cache.egg-info/PKG-INFO` & `python-redis-cache-2.1.0/python_redis_cache.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: python-redis-cache
-Version: 1.2.0
+Version: 2.1.0
 Summary: Basic Redis caching for functions
 Home-page: http://github.com/taylorhakes/python-redis-cache
 Author: Taylor Hakes
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![CI](https://github.com/taylorhakes/python-redis-cache/workflows/CI/badge.svg?event=push)](https://github.com/taylorhakes/python-redis-cache/actions?query=event%3Apush+branch%3Amaster+workflow%3ACI)
 [![pypi](https://img.shields.io/pypi/v/python-redis-cache.svg)](https://pypi.python.org/pypi/python-redis-cache)
 [![versions](https://img.shields.io/pypi/pyversions/python-redis-cache.svg)](https://github.com/taylorhakes/python-redis-cache)
 [![license](https://img.shields.io/github/license/taylorhakes/python-redis-cache.svg)](https://github.com/taylorhakes/python-redis-cache/blob/master/LICENSE)
 
 # python-redis-cache
 Simple redis cache for Python functions
 
 ### Requirements
 - Redis 5+
-- Python 3.6+
+- Python 3.7+
 
 ## How to install
 ```
 pip install python-redis-cache
 ```
 
 ## How to use
@@ -59,17 +58,24 @@
 https://security.stackexchange.com/questions/183966/safely-load-a-pickle-file
 
 - **ttl** - is based on the time from when it's first inserted in the cache, not based on the last access
 - **limit** - The limit will revoke keys (once it hits the limit) based on FIFO, not based on LRU
 
 ## API
 ```python
-RedisCache(redis_client, prefix="rc", serializer=dumps, deserializer=loads)
+# Create the redis cache
+cache = RedisCache(redis_client, prefix="rc", serializer=dumps, deserializer=loads)
 
-RedisCache.cache(ttl=None, limit=None, namespace=None)
+# Cache decorator to go on functions, see above
+cache.cache(ttl=..., limit=..., namespace=...) -> Callable[[Callable], Callable]
+
+# Get multiple values from the cache
+cache.mget([{"fn": my_func, "args": [1,2], "kwargs": {}}, ...]) -> List[Any]
+
+Redis
 
 # Cached function API
 
 # Returns a cached value, if it exists in cache. Saves value in cache if it doesn't exist
 cached_func(*args, *kwargs)
 
 # Invalidates a single value
@@ -79,9 +85,7 @@
 cached_func.invalidate_all()
 ```
 
 - prefix - The string to prefix the redis keys with
 - serializer/deserializer - functions to convert arguments and return value to a string (user JSON by default)
 - ttl - The time in seconds to cache the return value
 - namespace - The string namespace of the cache. This is useful for allowing multiple functions to use the same cache. By default its `f'{function.__module__}.{function.__file__}'`
-
-
```

### Comparing `python-redis-cache-1.2.0/setup.py` & `python-redis-cache-2.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
-__version__ = "1.2.0"
+__version__ = "2.1.0"
 
-setup(name='python-redis-cache',
-      version=__version__,
-      description='Basic Redis caching for functions',
-      long_description=long_description,
-      long_description_content_type='text/markdown',
-      url='http://github.com/taylorhakes/python-redis-cache',
-      author='Taylor Hakes',
-      license='MIT',
-      python_requires='>=3.6',
-      packages=find_packages(),
-      setup_requires=['pytest-runner==5.2'],
-      tests_require=['pytest==5.4.3', 'redis==3.5.3'],
+setup(
+    name='python-redis-cache',
+    version=__version__,
+    description='Basic Redis caching for functions',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='http://github.com/taylorhakes/python-redis-cache',
+    author='Taylor Hakes',
+    license='MIT',
+    python_requires='>=3.6',
+    packages=find_packages(),
+    setup_requires=['pytest-runner==5.3.1'],
+    tests_require=['pytest==6.2.5', 'redis==3.5.3'],
 )
```

